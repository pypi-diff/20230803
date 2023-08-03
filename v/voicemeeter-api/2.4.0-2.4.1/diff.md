# Comparing `tmp/voicemeeter_api-2.4.0.tar.gz` & `tmp/voicemeeter_api-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_api-2.4.0.tar", max compression
+gzip compressed data, was "voicemeeter_api-2.4.1.tar", max compression
```

## Comparing `voicemeeter_api-2.4.0.tar` & `voicemeeter_api-2.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.4.0/LICENSE
--rw-r--r--   0        0        0     1102 2023-08-02 14:42:32.480639 voicemeeter_api-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    18957 2023-08-01 15:15:42.523592 voicemeeter_api-2.4.0/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.4.0/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8226 2023-07-18 12:50:39.247222 voicemeeter_api-2.4.0/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     4618 2023-08-02 14:26:03.847115 voicemeeter_api-2.4.0/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1194 2023-07-25 17:25:27.080618 voicemeeter_api-2.4.0/voicemeeterlib/command.py
--rw-r--r--   0        0        0     6050 2023-08-01 16:48:00.788867 voicemeeter_api-2.4.0/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2023-07-25 17:25:30.796461 voicemeeter_api-2.4.0/voicemeeterlib/device.py
--rw-r--r--   0        0        0      666 2023-08-02 14:34:34.328692 voicemeeter_api-2.4.0/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.4.0/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7792 2023-07-28 09:25:54.751960 voicemeeter_api-2.4.0/voicemeeterlib/factory.py
--rw-r--r--   0        0        0     1091 2023-07-25 17:25:27.080618 voicemeeter_api-2.4.0/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1800 2023-07-25 17:25:30.842924 voicemeeter_api-2.4.0/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2628 2023-07-18 13:00:26.971422 voicemeeter_api-2.4.0/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1512 2023-07-25 17:25:30.885025 voicemeeter_api-2.4.0/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.4.0/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6485 2023-07-28 09:25:54.753959 voicemeeter_api-2.4.0/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.4.0/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0    12341 2023-08-01 15:15:42.523592 voicemeeter_api-2.4.0/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    15352 2023-07-22 11:42:06.374784 voicemeeter_api-2.4.0/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     2277 2023-08-01 15:15:42.525096 voicemeeter_api-2.4.0/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2930 2023-07-18 13:06:02.678934 voicemeeter_api-2.4.0/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     2436 2023-07-21 11:41:24.422287 voicemeeter_api-2.4.0/voicemeeterlib/util.py
--rw-r--r--   0        0        0     6055 2023-07-20 10:04:33.726657 voicemeeter_api-2.4.0/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    18745 1970-01-01 00:00:00.000000 voicemeeter_api-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.4.1/LICENSE
+-rw-r--r--   0        0        0     1102 2023-08-02 16:17:38.349085 voicemeeter_api-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0    18957 2023-08-01 15:15:42.523592 voicemeeter_api-2.4.1/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.4.1/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8226 2023-07-18 12:50:39.247222 voicemeeter_api-2.4.1/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4618 2023-08-02 14:26:03.847115 voicemeeter_api-2.4.1/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-07-25 17:25:27.080618 voicemeeter_api-2.4.1/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     6050 2023-08-01 16:48:00.788867 voicemeeter_api-2.4.1/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2023-07-25 17:25:30.796461 voicemeeter_api-2.4.1/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      666 2023-08-02 14:34:34.328692 voicemeeter_api-2.4.1/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.4.1/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7778 2023-08-02 16:12:16.446060 voicemeeter_api-2.4.1/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-07-25 17:25:27.080618 voicemeeter_api-2.4.1/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-07-25 17:25:30.842924 voicemeeter_api-2.4.1/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2628 2023-07-18 13:00:26.971422 voicemeeter_api-2.4.1/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1512 2023-07-25 17:25:30.885025 voicemeeter_api-2.4.1/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.4.1/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6485 2023-07-28 09:25:54.753959 voicemeeter_api-2.4.1/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.4.1/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    12303 2023-08-02 16:11:06.719892 voicemeeter_api-2.4.1/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15352 2023-07-22 11:42:06.374784 voicemeeter_api-2.4.1/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-08-01 15:15:42.525096 voicemeeter_api-2.4.1/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2930 2023-07-18 13:06:02.678934 voicemeeter_api-2.4.1/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     2436 2023-07-21 11:41:24.422287 voicemeeter_api-2.4.1/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     6055 2023-07-20 10:04:33.726657 voicemeeter_api-2.4.1/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    18745 1970-01-01 00:00:00.000000 voicemeeter_api-2.4.1/PKG-INFO
```

### Comparing `voicemeeter_api-2.4.0/LICENSE` & `voicemeeter_api-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/pyproject.toml` & `voicemeeter_api-2.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-api"
-version = "2.4.0"
+version = "2.4.1"
 description = "A Python wrapper for the Voiceemeter API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-api-python"
 
 packages = [{ include = "voicemeeterlib" }]
```

### Comparing `voicemeeter_api-2.4.0/README.md` & `voicemeeter_api-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/bus.py` & `voicemeeter_api-2.4.1/voicemeeterlib/bus.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/cbindings.py` & `voicemeeter_api-2.4.1/voicemeeterlib/cbindings.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/command.py` & `voicemeeter_api-2.4.1/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/config.py` & `voicemeeter_api-2.4.1/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/device.py` & `voicemeeter_api-2.4.1/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/error.py` & `voicemeeter_api-2.4.1/voicemeeterlib/error.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/event.py` & `voicemeeter_api-2.4.1/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/factory.py` & `voicemeeter_api-2.4.1/voicemeeterlib/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from abc import abstractmethod
 from enum import IntEnum
 from functools import cached_property
-from typing import Iterable, NoReturn
+from typing import Iterable
 
 from . import misc
 from .bus import request_bus_obj as bus
 from .command import Command
 from .config import request_config as configs
 from .device import Device
 from .error import VMError
@@ -47,15 +47,15 @@
             f"Finished building option for {self._factory}",
             f"Finished building recorder for {self._factory}",
             f"Finished building patch for {self._factory}",
             f"Finished building fx for {self._factory}",
         )
         self.logger = logger.getChild(self.__class__.__name__)
 
-    def _pinfo(self, name: str) -> NoReturn:
+    def _pinfo(self, name: str) -> None:
         """prints progress status for each step"""
         name = name.split("_")[1]
         self.logger.debug(self._info[int(getattr(self.BuilderProgress, name))])
 
     def make_strip(self):
         self._factory.strip = tuple(
             strip(i < self.kind.phys_in, self._factory, i)
```

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/inst.py` & `voicemeeter_api-2.4.1/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/iremote.py` & `voicemeeter_api-2.4.1/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/kinds.py` & `voicemeeter_api-2.4.1/voicemeeterlib/kinds.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/macrobutton.py` & `voicemeeter_api-2.4.1/voicemeeterlib/macrobutton.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/meta.py` & `voicemeeter_api-2.4.1/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/misc.py` & `voicemeeter_api-2.4.1/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/recorder.py` & `voicemeeter_api-2.4.1/voicemeeterlib/recorder.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/remote.py` & `voicemeeter_api-2.4.1/voicemeeterlib/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ctypes as ct
 import logging
 import time
 from abc import abstractmethod
 from queue import Queue
-from typing import Iterable, NoReturn, Optional, Union
+from typing import Iterable, Optional, Union
 
 from .cbindings import CBindings
 from .error import CAPIError, VMError
 from .event import Event
 from .inst import bits
 from .kinds import KindId
 from .misc import Midi, VmGui
@@ -58,28 +58,28 @@
         self.logger.debug("initiating events thread")
         queue = Queue()
         self.updater = Updater(self, queue)
         self.updater.start()
         self.producer = Producer(self, queue)
         self.producer.start()
 
-    def login(self) -> NoReturn:
+    def login(self) -> None:
         """Login to the API, initialize dirty parameters"""
         self.gui.launched = self.call(self.bind_login, ok=(0, 1)) == 0
         if not self.gui.launched:
             self.logger.info(
                 "Voicemeeter engine running but GUI not launched. Launching the GUI now."
             )
             self.run_voicemeeter(self.kind.name)
         self.logger.info(
             f"{type(self).__name__}: Successfully logged into {self} version {self.version}"
         )
         self.clear_dirty()
 
-    def run_voicemeeter(self, kind_id: str) -> NoReturn:
+    def run_voicemeeter(self, kind_id: str) -> None:
         if kind_id not in (kind.name.lower() for kind in KindId):
             raise VMError(f"Unexpected Voicemeeter type: '{kind_id}'")
         if kind_id == "potato" and bits == 8:
             value = KindId[kind_id.upper()].value + 3
         else:
             value = KindId[kind_id.upper()].value
         self.call(self.bind_run_voicemeeter, value)
@@ -129,15 +129,15 @@
         """True iff levels have been updated."""
         self._strip_buf, self._bus_buf = self._get_levels()
         return not (
             self.cache.get("strip_level") == self._strip_buf
             and self.cache.get("bus_level") == self._bus_buf
         )
 
-    def clear_dirty(self) -> NoReturn:
+    def clear_dirty(self) -> None:
         try:
             while self.pdirty or self.mdirty:
                 pass
         except CAPIError as e:
             if not (e.fn_name == "VBVMR_MacroButton_IsDirty" and e.code == -9):
                 raise
             self.logger.error(f"{e} clearing pdirty only.")
@@ -151,15 +151,15 @@
             buf = ct.create_unicode_buffer(512)
             self.call(self.bind_get_parameter_string_w, param.encode(), ct.byref(buf))
         else:
             buf = ct.c_float()
             self.call(self.bind_get_parameter_float, param.encode(), ct.byref(buf))
         return buf.value
 
-    def set(self, param: str, val: Union[str, float]) -> NoReturn:
+    def set(self, param: str, val: Union[str, float]) -> None:
         """Sets a string or float parameter. Caches value"""
         if isinstance(val, str):
             if len(val) >= 512:
                 raise VMError("String is too long")
             self.call(
                 self.bind_set_parameter_string_w, param.encode(), ct.c_wchar_p(val)
             )
@@ -187,15 +187,15 @@
                 "are you using an old version of the API?",
             )
             raise CAPIError(
                 "VBVMR_MacroButton_GetStatus", -9, msg=" ".join(ERR_MSG)
             ) from e
         return int(c_state.value)
 
-    def set_buttonstatus(self, id_: int, val: int, mode: int) -> NoReturn:
+    def set_buttonstatus(self, id_: int, val: int, mode: int) -> None:
         """Sets a macrobutton parameter. Caches value"""
         c_state = ct.c_float(float(val))
         try:
             self.call(
                 self.bind_macro_button_set_status,
                 ct.c_long(id_),
                 c_state,
@@ -330,17 +330,17 @@
         self.apply(config)
         self.logger.info(f"Profile '{name}' applied!")
 
     def end_thread(self):
         self.logger.debug("events thread shutdown started")
         self.running = False
 
-    def logout(self) -> NoReturn:
+    def logout(self) -> None:
         """Logout of the API"""
         time.sleep(0.1)
         self.call(self.bind_logout)
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
 
-    def __exit__(self, exc_type, exc_value, exc_traceback) -> NoReturn:
+    def __exit__(self, exc_type, exc_value, exc_traceback) -> None:
         """teardown procedures"""
         self.end_thread()
         self.logout()
```

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/strip.py` & `voicemeeter_api-2.4.1/voicemeeterlib/strip.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/subject.py` & `voicemeeter_api-2.4.1/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/updater.py` & `voicemeeter_api-2.4.1/voicemeeterlib/updater.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/util.py` & `voicemeeter_api-2.4.1/voicemeeterlib/util.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/voicemeeterlib/vban.py` & `voicemeeter_api-2.4.1/voicemeeterlib/vban.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.0/PKG-INFO` & `voicemeeter_api-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 2.4.0
+Version: 2.4.1
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

