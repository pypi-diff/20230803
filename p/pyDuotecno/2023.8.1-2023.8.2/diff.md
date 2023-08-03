# Comparing `tmp/pyDuotecno-2023.8.1.tar.gz` & `tmp/pyDuotecno-2023.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDuotecno-2023.8.1.tar", last modified: Tue Aug  1 18:30:04 2023, max compression
+gzip compressed data, was "pyDuotecno-2023.8.2.tar", last modified: Thu Aug  3 17:44:03 2023, max compression
```

## Comparing `pyDuotecno-2023.8.1.tar` & `pyDuotecno-2023.8.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:30:04.904312 pyDuotecno-2023.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 18:30:04.904312 pyDuotecno-2023.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:30:04.904312 pyDuotecno-2023.8.1/duotecno/
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/duotecno/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/duotecno/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/duotecno/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/duotecno/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/duotecno/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:30:04.904312 pyDuotecno-2023.8.1/pyDuotecno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 18:30:04.000000 pyDuotecno-2023.8.1/pyDuotecno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-01 18:30:04.000000 pyDuotecno-2023.8.1/pyDuotecno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:30:04.000000 pyDuotecno-2023.8.1/pyDuotecno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:30:04.000000 pyDuotecno-2023.8.1/pyDuotecno.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 18:30:04.000000 pyDuotecno-2023.8.1/pyDuotecno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:30:04.904312 pyDuotecno-2023.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:44:03.715355 pyDuotecno-2023.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 17:43:49.000000 pyDuotecno-2023.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 17:43:49.000000 pyDuotecno-2023.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-03 17:44:03.715355 pyDuotecno-2023.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 17:43:49.000000 pyDuotecno-2023.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:44:03.711355 pyDuotecno-2023.8.2/duotecno/
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-08-03 17:43:49.000000 pyDuotecno-2023.8.2/duotecno/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-03 17:43:49.000000 pyDuotecno-2023.8.2/duotecno/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-08-03 17:43:49.000000 pyDuotecno-2023.8.2/duotecno/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-08-03 17:43:49.000000 pyDuotecno-2023.8.2/duotecno/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-08-03 17:43:49.000000 pyDuotecno-2023.8.2/duotecno/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:44:03.715355 pyDuotecno-2023.8.2/pyDuotecno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-03 17:44:03.000000 pyDuotecno-2023.8.2/pyDuotecno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-03 17:44:03.000000 pyDuotecno-2023.8.2/pyDuotecno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:44:03.000000 pyDuotecno-2023.8.2/pyDuotecno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:44:03.000000 pyDuotecno-2023.8.2/pyDuotecno.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 17:44:03.000000 pyDuotecno-2023.8.2/pyDuotecno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-03 17:43:49.000000 pyDuotecno-2023.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:43:49.000000 pyDuotecno-2023.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:44:03.715355 pyDuotecno-2023.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 17:43:49.000000 pyDuotecno-2023.8.2/setup.py
```

### Comparing `pyDuotecno-2023.8.1/LICENSE` & `pyDuotecno-2023.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.8.1/PKG-INFO` & `pyDuotecno-2023.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2023.8.1/duotecno/controller.py` & `pyDuotecno-2023.8.2/duotecno/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     writer: asyncio.StreamWriter = None
     reader: asyncio.StreamReader = None
     readerTask: asyncio.Task
     loginOK: asyncio.Event
     connectionOK: asyncio.Event
     nodes: dict = {}
 
-    def get_units(self, unit_type) -> list:
+    def get_units(self, unit_type: list | str) -> list:
         res = []
         for node in self.nodes.values():
             for unit in node.get_unit_by_type(unit_type):
                 res.append(unit)
         return res
 
     async def connect(self, host, port, password, testOnly=False) -> None:
```

### Comparing `pyDuotecno-2023.8.1/duotecno/node.py` & `pyDuotecno-2023.8.2/duotecno/node.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from duotecno.unit import (
     BaseUnit,
     SwitchUnit,
     SensUnit,
     DimUnit,
     DuoswitchUnit,
     VirtualUnit,
+    ControlUnit,
 )
 
 
 class Node:
     name: str
     index: int
     nodeType: NodeType
@@ -51,19 +52,22 @@
     def __repr__(self) -> str:
         items = []
         for k, v in self.__dict__.items():
             if k not in ["_log", "writer"]:
                 items.append(f"{k} = {v!r}")
         return "{}[{}]".format(type(self), ", ".join(items))
 
-    def get_unit_by_type(self, unit_type):
+    def get_unit_by_type(self, unit_type: list | str):
+        if isinstance(unit_type, str):
+            unit_type = [unit_type]
         res = []
         for unit in self.units.values():
-            if str(type(unit)) == f"<class 'duotecno.unit.{unit_type}'>":
-                res.append(unit)
+            for unitT in unit_type:
+                if str(type(unit)) == f"<class 'duotecno.unit.{unitT}'>":
+                    res.append(unit)
         return res
 
     async def load(self) -> None:
         self._log.debug(f"Node {self.name}: Requesting units")
         for i in range(self.numUnits - 1):
             await self.writer(f"[209,2,{self.address},{i}]")
 
@@ -77,14 +81,16 @@
                     u = SensUnit
                 elif packet.unitTypeName == "DIM":
                     u = DimUnit
                 elif packet.unitTypeName == "DUOSWITCH":
                     u = DuoswitchUnit
                 elif packet.unitTypeName == "VIRTUAL":
                     u = VirtualUnit
+                elif packet.unitTypeName == "CONTROL":
+                    u = ControlUnit
                 else:
                     self._log.warning(f"Unhandled unitType: {packet.unitTypeName}")
                 self.units[packet.unit] = u(
                     self, name=packet.unitName, unit=packet.unit, writer=self.writer
                 )
                 await self.units[packet.unit].requestStatus()
             if len(self.units) == self.numUnits - 1:
```

### Comparing `pyDuotecno-2023.8.1/duotecno/protocol.py` & `pyDuotecno-2023.8.2/duotecno/protocol.py`

 * *Files 17% similar despite different names*

```diff
@@ -115,20 +115,26 @@
     def __repr__(self) -> str:
         return self.to_json()
 
 
 class BaseNodeUnitMessage(BaseMessage):
     address: int
     unit: int
-    unitType: int
 
     def __init__(self, data):
         super().__init__(data)
         self.address = data.popleft()
         self.unit = data.popleft()
+
+
+class BaseNodeUnitTypeMessage(BaseNodeUnitMessage):
+    unitType: int
+
+    def __init__(self, data):
+        super().__init__(data)
         self.unitType = data.popleft()
 
 
 class EV_CLIENTCONNECTSET_3(BaseMessage):
     loginOk: bool
 
     def __init__(self, data):
@@ -138,14 +144,28 @@
 class EV_NODEDATABASEINFO_0(BaseMessage):
     numNode: int
 
     def __init__(self, data):
         self.numNode = data.popleft()
 
 
+class EV_UNITMACROCOMMAND_0(BaseNodeUnitMessage):
+    event: int
+    state: int
+    code1: int
+    code2: int
+
+    def __init__(self, data):
+        super().__init__(data)
+        self.event = data.popleft()
+        self.state = data.popleft()
+        self.code1 = data.popleft()
+        self.code2 = data.popleft()
+
+
 @unique
 class NodeType(Enum):
     Standard = 1
     Gateway = 4
     Modem = 8
     Gui = 32
 
@@ -203,75 +223,35 @@
         self.lunit = data.popleft()
         self.unitName = "".join([chr(data.popleft()) for _i in range(data.popleft())])
         self.unitType = data.popleft()
         self.unitTypeName = UnitType(self.unitType).name
         self.unitFlags = data.popleft()
 
 
-class EV_UNITSENSSTATUS_0(BaseNodeUnitMessage):
-    controlState: int
-    state: int
-    preset: int
-    value: list
-    sun: list
-    halfsun: list
-    moon: list
-    halfmoon: list
-
-    def __init__(self, data) -> None:
-        super().__init__(data)
-        # config = reserved
-        data.popleft()
-        self.controlState = data.popleft()
-        self.state = data.popleft()
-        self.preset = data.popleft()
-        self.value = [data.popleft(), data.popleft()]
-        self.sun = [data.popleft(), data.popleft()]
-        self.halfsun = [data.popleft(), data.popleft()]
-        self.moon = [data.popleft(), data.popleft()]
-        self.halfmoon = [data.popleft(), data.popleft()]
-
-
-class EV_UNITSENSSTATUS_1(EV_UNITSENSSTATUS_0):
-    offset: list
-    swing: list
-    workingMode: int
-    fanSpeed: int
-    swingMode: int
-
-    def __init__(self, data) -> None:
-        super().__init__(data)
-        self.offset = [data.popleft(), data.popleft()]
-        self.swing = [data.popleft(), data.popleft()]
-        self.workingMode = data.popleft()
-        self.fanSpeed = data.popleft()
-        self.swingMode = data.popleft()
-
-
 @final
 @unique
 class SwitchStatus(Enum):
     OFF = 0
     ON = 1
     PIRTIMED = 2
 
 
-class EV_UNITSWITCHSTATUS_0(BaseNodeUnitMessage):
+class EV_UNITSWITCHSTATUS_0(BaseNodeUnitTypeMessage):
     state: int
     stateName: SwitchStatus
 
     def __init__(self, data) -> None:
         super().__init__(data)
         # config, reserved
         data.popleft()
         self.state = data.popleft()
         self.stateName = SwitchStatus(self.state).name
 
 
-class EV_UNITDIMSTATUS_0(BaseNodeUnitMessage):
+class EV_UNITDIMSTATUS_0(BaseNodeUnitTypeMessage):
     state: int
     stateName: SwitchStatus
     dimValue: int
 
     def __init__(self, data) -> None:
         super().__init__(data)
         # config, reserved
@@ -287,17 +267,150 @@
     IDLE = 0
     IDLE_DOWN = 1
     IDLE_UP = 2
     BUSY_DOWN = 3
     BUSY_UP = 4
 
 
-class EV_UNITDUOSWITCHSTATUS_0(BaseNodeUnitMessage):
+class EV_UNITDUOSWITCHSTATUS_0(BaseNodeUnitTypeMessage):
     state: int
     stateName: DuoswitchStatus
 
     def __init__(self, data) -> None:
         super().__init__(data)
         # config, reserved
         data.popleft()
         self.state = data.popleft()
         self.stateName = DuoswitchStatus(self.state).name
+
+
+@final
+@unique
+class SensType(Enum):
+    TEMPERATURE = 0
+    PH = 1
+    LUX = 2
+    AMPERE = 3
+
+
+@final
+@unique
+class SensControl(Enum):
+    OFF = 0
+    ON = 1
+
+
+@final
+@unique
+class SensState(Enum):
+    IDLE = 0
+    HEATING = 1
+    COOLING = 2
+
+
+@final
+@unique
+class SensPreset(Enum):
+    SUN = 0
+    HALF_SUN = 1
+    MOON = 2
+    HALF_MOON = 3
+
+
+@final
+@unique
+class SensWorkingmode(Enum):
+    AUTO = 0
+    HEATING = 1
+    COOLING = 2
+    DRY = 3
+    FAN = 4
+    UNKNOWN = 255
+
+
+@final
+@unique
+class SensFanspeed(Enum):
+    SPEED1 = 0
+    SPEED2 = 1
+    SPEED3 = 2
+    SPEED4 = 3
+    SPEED5 = 4
+    AUTO = 255
+
+
+def sens_calc_value(msb: int, lsb: int) -> float:
+    val = (256 * msb) + lsb
+    return val / 10
+
+
+class EV_UNITSENSSTATUS_0(BaseNodeUnitTypeMessage):
+    config: int
+    configName: SensType
+    controlState: int
+    controlStateName: SensControl
+    state: int
+    stateName: SensState
+    preset: int
+    presetName: SensPreset
+    value: float
+    sun: float
+    halfsun: float
+    moon: float
+    halfmoon: float
+
+    def __init__(self, data) -> None:
+        super().__init__(data)
+        self.config = data.popleft()
+        self.configName = SensType(self.config).name
+        self.controlState = data.popleft()
+        self.controlStateName = SensControl(self.controlState).name
+        self.state = data.popleft()
+        self.stateName = SensState(self.state).name
+        self.preset = data.popleft()
+        self.presetName = SensPreset(self.preset).name
+        self.value = sens_calc_value(data.popleft(), data.popleft())
+        self.sun = sens_calc_value(data.popleft(), data.popleft())
+        self.halfsun = sens_calc_value(data.popleft(), data.popleft())
+        self.moon = sens_calc_value(data.popleft(), data.popleft())
+        self.halfmoon = sens_calc_value(data.popleft(), data.popleft())
+
+
+class EV_UNITSENSSTATUS_1(EV_UNITSENSSTATUS_0):
+    offset: float
+    swing: float
+    workingMode: int
+    workingModeName: SensWorkingmode
+    fanSpeed: int
+    fanSpeedName: SensFanspeed
+    swingMode: int
+    swingModeName: SensControl
+
+    def __init__(self, data) -> None:
+        super().__init__(data)
+        self.offset = sens_calc_value(data.popleft(), data.popleft())
+        self.swing = sens_calc_value(data.popleft(), data.popleft())
+        self.workingMode = data.popleft()
+        self.workingModeName = SensWorkingmode(self.workingMode).name
+        self.fanSpeed = data.popleft()
+        self.fanSpeedName = SensFanspeed(self.fanSpeed).name
+        self.swingMode = data.popleft()
+        self.swingModeName = SensControl(self.swingMode).name
+
+
+@final
+@unique
+class ControLStatus(Enum):
+    OFF = 0
+    ON = 1
+
+
+class EV_UNITCONTROLSTATUS_0(BaseNodeUnitTypeMessage):
+    status: int
+    statusName: ControLStatus
+
+    def __init__(self, data) -> None:
+        super().__init__(data)
+        # config ignore
+        data.popleft()
+        self.status = data.popleft()
+        self.statusName = ControLStatus(self.status).name
```

### Comparing `pyDuotecno-2023.8.1/duotecno/unit.py` & `pyDuotecno-2023.8.2/duotecno/unit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import final, Awaitable, Callable
 import logging
 from duotecno.protocol import (
     EV_UNITDUOSWITCHSTATUS_0,
     EV_UNITDIMSTATUS_0,
     EV_UNITSWITCHSTATUS_0,
     EV_UNITSENSSTATUS_0,
+    EV_UNITSENSSTATUS_1,
+    EV_UNITCONTROLSTATUS_0,
+    EV_UNITMACROCOMMAND_0,
 )
 
 
 class BaseUnit:
     _unitType: final = None
     _on_status_update: list = []
     name: str
@@ -44,15 +47,15 @@
 
     def on_status_update(self, meth: Callable[[], Awaitable[None]]) -> None:
         self._on_status_update.append(meth)
 
     def __repr__(self) -> str:
         items = []
         for k, v in self.__dict__.items():
-            if k not in ["_log", "writer"]:
+            if k not in ["_log", "writer", "node"]:
                 items.append(f"{k} = {v!r}")
         return "{}[{}]".format(type(self), ", ".join(items))
 
     async def handlePacket(self, packet) -> None:
         self._log.debug(f"Unhandled unit packet: {packet}")
 
     async def requestStatus(self) -> None:
@@ -73,19 +76,24 @@
 class SensUnit(BaseUnit):
     _unitType: final = 4
     _state: int
     _value: int
     _preset: int
 
     async def handlePacket(self, packet) -> None:
-        if isinstance(packet, EV_UNITSENSSTATUS_0):
+        if isinstance(packet, EV_UNITSENSSTATUS_0) or isinstance(
+            packet, EV_UNITSENSSTATUS_1
+        ):
             await self._update(
                 {"state": packet.state, "value": packet.value, "preset": packet.preset}
             )
             return
+        if isinstance(packet, EV_UNITMACROCOMMAND_0):
+            # TODO
+            return
         await super().handlePacket(packet)
 
 
 class DimUnit(BaseUnit):
     _unitType: final = 1
     _state: int
     _value: int
@@ -122,14 +130,25 @@
     _unitType: final = 2
     _state: int = None
 
     async def handlePacket(self, packet) -> None:
         if isinstance(packet, EV_UNITSWITCHSTATUS_0):
             await self._update({"state": packet.state})
             return
+        if isinstance(packet, EV_UNITMACROCOMMAND_0):
+            if packet.event == 5:
+                # pir timed
+                self._update({"state": 2})
+            elif packet.state == 0:
+                # OFF
+                self._update({"state": 0})
+            else:
+                # on
+                self._update({"state": 1})
+            return
         await super().handlePacket(packet)
 
     def is_on(self):
         return self._state
 
     async def turn_on(self):
         """Switch on."""
@@ -164,22 +183,39 @@
         if self._state == 1:
             return True
         return False
 
     async def open(self):
         """Move up."""
         await self.stop()
-        await self.writer(f"[182,0,{self.node.address},{self.unit},4]")
+        await self.writer(f"[182,4,{self.node.address},{self.unit}]")
 
     async def close(self):
         """Move down."""
         await self.stop()
-        await self.writer(f"[182,0,{self.node.address},{self.unit},5]")
+        await self.writer(f"[182,5,{self.node.address},{self.unit}]")
 
     async def stop(self):
         """Stop the motor."""
-        await self.writer(f"[182,0,{self.node.address},{self.unit},3]")
+        await self.writer(f"[182,3,{self.node.address},{self.unit}]")
 
 
 class VirtualUnit(BaseUnit):
     _unitType: final = 7
+    _status: int
+
+    async def handlePacket(self, packet) -> None:
+        if isinstance(packet, EV_UNITCONTROLSTATUS_0):
+            await self._update({"status": packet.status})
+            return
+        if isinstance(packet, EV_UNITMACROCOMMAND_0):
+            await self._update({"status": packet.state})
+            return
+        await super().handlePacket(packet)
+
+    def is_on(self):
+        return self._status
+
+
+class ControlUnit(VirtualUnit):
+    _unitType: final = 3
     pass
```

### Comparing `pyDuotecno-2023.8.1/pyDuotecno.egg-info/PKG-INFO` & `pyDuotecno-2023.8.2/pyDuotecno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2023.8.1/pyproject.toml` & `pyDuotecno-2023.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "pyDuotecno"
 license = {text = "Apache"}
-version = "2023.8.1"
+version = "2023.8.2"
 description = "Open-source home automation platform running on Python 3."
 readme = "README.md"
 authors = [
     {name = "Maikel Punie", email = "maikel.punie@gmail.com"}
 ]
 keywords = ["home", "duotecno", "automation"]
 classifiers = [
@@ -37,15 +37,15 @@
 zip-safe  = false
 include-package-data = true
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "tests.*", "examples", "examples/*"]
 
 [tool.bumpver]
-current_version = "2023.8.1"
+current_version = "2023.8.2"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

