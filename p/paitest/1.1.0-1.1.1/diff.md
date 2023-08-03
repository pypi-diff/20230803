# Comparing `tmp/paitest-1.1.0-py3-none-any.whl.zip` & `tmp/paitest-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 25069 bytes, number of entries: 13
+Zip file size: 15356 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       63 b- defN 80-Jan-01 00:00 paitest/__init__.py
 -rw-r--r--  2.0 unx      342 b- defN 80-Jan-01 00:00 paitest/frames/__init__.py
--rw-r--r--  2.0 unx     2581 b- defN 80-Jan-01 00:00 paitest/frames/coord.py
--rw-r--r--  2.0 unx      823 b- defN 80-Jan-01 00:00 paitest/frames/coord.pyi
--rw-r--r--  2.0 unx    14257 b- defN 80-Jan-01 00:00 paitest/frames/frame.py
--rw-r--r--  2.0 unx     4707 b- defN 80-Jan-01 00:00 paitest/frames/frame_params.py
+-rw-r--r--  2.0 unx     8635 b- defN 80-Jan-01 00:00 paitest/frames/coord.py
+-rw-r--r--  2.0 unx     1553 b- defN 80-Jan-01 00:00 paitest/frames/coord.pyi
+-rw-r--r--  2.0 unx    14247 b- defN 80-Jan-01 00:00 paitest/frames/frame.py
+-rw-r--r--  2.0 unx     5239 b- defN 80-Jan-01 00:00 paitest/frames/frame_params.py
 -rw-r--r--  2.0 unx      230 b- defN 80-Jan-01 00:00 paitest/log.py
--rw-r--r--  2.0 unx    18940 b- defN 80-Jan-01 00:00 paitest/paitest.py
--rw-r--r--  2.0 unx     1990 b- defN 80-Jan-01 00:00 paitest/paitest.pyi
--rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 paitest-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3763 b- defN 80-Jan-01 00:00 paitest-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 paitest-1.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1001 b- defN 16-Jan-01 00:00 paitest-1.1.0.dist-info/RECORD
-13 files, 83308 bytes uncompressed, 23423 bytes compressed:  71.9%
+-rw-r--r--  2.0 unx    19487 b- defN 80-Jan-01 00:00 paitest/paitest.py
+-rw-r--r--  2.0 unx     2146 b- defN 80-Jan-01 00:00 paitest/paitest.pyi
+-rw-r--r--  2.0 unx     1067 b- defN 80-Jan-01 00:00 paitest-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3988 b- defN 80-Jan-01 00:00 paitest-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 paitest-1.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1001 b- defN 16-Jan-01 00:00 paitest-1.1.1.dist-info/RECORD
+13 files, 58086 bytes uncompressed, 13710 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: paitest/paitest.py
 Comment: 
 
 Filename: paitest/paitest.pyi
 Comment: 
 
-Filename: paitest-1.1.0.dist-info/LICENSE
+Filename: paitest-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: paitest-1.1.0.dist-info/METADATA
+Filename: paitest-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: paitest-1.1.0.dist-info/WHEEL
+Filename: paitest-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: paitest-1.1.0.dist-info/RECORD
+Filename: paitest-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## paitest/frames/coord.py

```diff
@@ -1,12 +1,18 @@
-from typing import Optional, Tuple, Union
+from typing import Optional, Tuple, Union, overload
 
 
 class Coord:
-    """Coordinate class"""
+    """Coordinates of the cores. Set coordinates (x, y) for every cores.
+
+    Left to right, +X, up to down, +Y.
+    """
+
+    _COORD_MAX_LIMIT = (1 << 5) - 1
+    _COORD_LOW_LIMIT = 0
 
     def __init__(
         self, _x: Union[Tuple[int, int], int], _y: Optional[int] = None
     ) -> None:
         if isinstance(_x, Tuple):
             x, y = _x[0], _x[1]
             if isinstance(_y, int):
@@ -15,69 +21,267 @@
             if isinstance(_y, int):
                 x, y = _x, _y
             else:
                 raise ValueError("Missing Argument: y")
         else:
             raise ValueError("Wrong Argument")
 
-        if not (0 <= x < 32 and 0 <= y < 32):
-            raise ValueError(f"0 <= x < 32, 0 <= y < 32: ({x}, {y})")
-
-        self.x, self.y = x, y
-
-    def __add__(self, other) -> "Coord":
-        return Coord(self.x + other.x, self.y + other.y)
-
-    def __sub__(self, other) -> "CoordOffset":
-        return CoordOffset(self.x - other.x, self.y - other.y)
+        if not (self._COORD_LOW_LIMIT <= x <= self._COORD_MAX_LIMIT and self._COORD_LOW_LIMIT <= y <= self._COORD_MAX_LIMIT):
+            raise ValueError(f"{self._COORD_LOW_LIMIT} <= x <= {self._COORD_MAX_LIMIT}, {self._COORD_LOW_LIMIT} <= y <= {self._COORD_MAX_LIMIT}: ({x}, {y})")
 
-    def __eq__(self, other) -> bool:
-        if isinstance(other, Tuple):
-            return (self.x, self.y) == other
+        self.x: int = x
+        self.y: int = y
 
-        return self.x == other.x and self.y == other.y
+    @classmethod
+    def from_tuple(cls, pos) -> "Coord":
+        return cls(*pos)
+
+    @classmethod
+    def default(cls) -> "Coord":
+        return cls(0, 0)
+
+    def __add__(self, __other: "CoordOffset") -> "Coord":
+        """
+        Examples:
+
+        Coord = Coord + CoordOffset
+        >>> c1 = Coord(1, 1)
+        >>> c2 = c1 + CoordOffset(1, 1)
+        c1: Coord(2, 2)
+
+        NOTE: Coord + Coord is meaningless.
+        """
+        if not isinstance(__other, CoordOffset):
+            raise TypeError(f"Unsupported type: {type(__other)}")
+
+        return Coord(self.x + __other.delta_x, self.y + __other.delta_y)
+
+    @overload
+    def __sub__(self, __other: "Coord") -> "CoordOffset":
+        ...
+
+    @overload
+    def __sub__(self, __other: "CoordOffset") -> "Coord":
+        ...
+
+    def __sub__(
+        self, __other: Union["Coord", "CoordOffset"]
+    ) -> Union["Coord", "CoordOffset"]:
+        """
+        Example:
+        >>> c1 = Coord(1, 1)
+        >>> c2 = Coord(2, 2) - c1
+        c2: CoordOffset(1, 1)
+        """
+        if isinstance(__other, Coord):
+            return CoordOffset(self.x - __other.x, self.y - __other.y)
+
+        if isinstance(__other, CoordOffset):
+            return Coord(self.x - __other.delta_x, self.y - __other.delta_y)
+
+        raise TypeError(f"Unsupported type: {type(__other)}")
+
+    """Operations below are used only when comparing with a Cooord."""
+
+    def __eq__(self, __other: "Coord") -> bool:
+        """
+        Example:
+        >>> Coord(4, 5) == Coord(4, 6)
+        False
+        """
+        if not isinstance(__other, Coord):
+            raise TypeError(f"Unsupported type: {type(__other)}")
+
+        return self.x == __other.x and self.y == __other.y
+
+    def __ne__(self, __other: "Coord") -> bool:
+        """
+        Examples:
+        >>> Coord(4, 5) != Coord(4, 6)
+        True
+
+        >>> Coord(4, 5) != Coord(5, 5)
+        True
+        """
+        if not isinstance(__other, Coord):
+            raise TypeError(f"Unsupported type: {type(__other)}")
+
+        return self.x != __other.x or self.y != __other.y
+
+    def __lt__(self, __other: "Coord") -> bool:
+        """Whether the coord is on the left OR below of __other.
+
+        Examples:
+        >>> Coord(4, 5) < Coord(4, 6)
+        True
+
+        >>> Coord(4, 5) < Coord(5, 5)
+        True
+
+        >>> Coord(4, 5) < Coord(5, 3)
+        True
+        """
+        if not isinstance(__other, Coord):
+            raise TypeError(f"Unsupported type: {type(__other)}")
+
+        return self.x < __other.x or self.y < __other.y
+
+    def __gt__(self, __other: "Coord") -> bool:
+        """Whether the coord is on the right AND above of __other.
+
+        Examples:
+        >>> Coord(5, 5) > Coord(4, 5)
+        True
+
+        >>> Coord(4, 6) > Coord(4, 5)
+        True
+
+        >>> Coord(5, 4) > Coord(4, 5)
+        False
+        """
+        if not isinstance(__other, Coord):
+            raise TypeError(f"Unsupported type: {type(__other)}")
 
-    def __ne__(self, other) -> bool:
-        return self.x != other.x or self.y != other.y
-
-    def __lt__(self, other) -> bool:
-        """Whether on the left or below"""
-        return self.x < other.x or self.y < other.y
-
-    def __gt__(self, other) -> bool:
-        """Whether on the right and above"""
+        # Except the `__eq__`
         return (
-            (self.x > other.x and self.y > other.y)
-            or (self.x == other.x and self.y > other.y)
-            or (self.x > other.x and self.y == other.y)
+            (self.x > __other.x and self.y > __other.y)
+            or (self.x == __other.x and self.y > __other.y)
+            or (self.x > __other.x and self.y == __other.y)
         )
 
-    def __le__(self, other) -> bool:
-        return self.__lt__(other) or self.__eq__(other)
+    def __le__(self, __other: "Coord") -> bool:
+        return self.__lt__(__other) or self.__eq__(__other)
 
-    def __ge__(self, other) -> bool:
-        return self.__gt__(other) or self.__eq__(other)
+    def __ge__(self, __other: "Coord") -> bool:
+        return self.__gt__(__other) or self.__eq__(__other)
 
     def __str__(self) -> str:
         return f"({self.x}, {self.y})"
 
+    def __repr__(self) -> str:
+        return f"Coord({self.x}, {self.y})"
 
-class CoordOffset(Coord):
-    """Coordinate offset class"""
+    def to_tuple(self) -> Tuple[int, int]:
+        """Convert to tuple"""
+        return (self.x, self.y)
+
+    def _to_address(self) -> int:
+        """Convert to address, 10 bits"""
+        return (self.x << 5) | self.y
+
+    @property
+    def address(self) -> int:
+        return self._to_address()
+
+
+class CoordOffset:
+    """Offset of coordinates"""
+
+    _COORDOFFSET_MAX_LIMIT = (1 << 5) - 1
+    _COORDOFFSET_LOW_LIMIT = -(1 << 5)
+
+    def __init__(self, _delta_x: int, _delta_y: int) -> None:
+        if not (self._COORDOFFSET_LOW_LIMIT < _delta_x <= self._COORDOFFSET_MAX_LIMIT and self._COORDOFFSET_LOW_LIMIT < _delta_y <= self._COORDOFFSET_MAX_LIMIT):
+            raise ValueError(f"{self._COORDOFFSET_LOW_LIMIT} < delta_x <= {self._COORDOFFSET_MAX_LIMIT}, {self._COORDOFFSET_LOW_LIMIT} < delta_y <= {self._COORDOFFSET_MAX_LIMIT}: ({_delta_x}, {_delta_y})")
+
+        self.delta_x: int = _delta_x
+        self.delta_y: int = _delta_y
+
+    @overload
+    def __add__(self, __other: Coord) -> Coord:
+        ...
+
+    @overload
+    def __add__(self, __other: "CoordOffset") -> "CoordOffset":
+        ...
+
+    def __add__(
+        self, __other: Union["CoordOffset", Coord]
+    ) -> Union["CoordOffset", Coord]:
+        """
+        Examples:
+        >>> delta_c1 = CoordOffset(1, 1)
+        >>> delta_c2 = delta_c1 + CoordOffset(1, 1)
+        delta_c2: CoordOffset(2, 2)
+
+        Coord = CoordOffset + Coord
+        >>> delta_c = CoordOffset(1, 1)
+        >>> c1 = Coord(2, 3)
+        >>> c2 = delta_c + c1
+        c2: Coord(3, 4)
+        """
+        if isinstance(__other, CoordOffset):
+            return CoordOffset(
+                self.delta_x + __other.delta_x, self.delta_y + __other.delta_y
+            )
+
+        if isinstance(__other, Coord):
+            return Coord(self.delta_x + __other.x, self.delta_y + __other.y)
+
+        raise TypeError(f"Unsupported type: {type(__other)}")
+
+    def __iadd__(self, __other: "CoordOffset") -> "CoordOffset":
+        """
+        Example:
+        >>> delta_c = CoordOffset(1, 1)
+        >>> delta_c += CoordOffset(1, 1)
+        delta_c: CoordOffset(2, 2)
+        """
+        if not isinstance(__other, CoordOffset):
+            raise TypeError(f"Unsupported type: {type(__other)}")
+
+        self.delta_x += __other.delta_x
+        self.delta_y += __other.delta_y
+
+        return self
+
+    def __sub__(self, __other: "CoordOffset") -> "CoordOffset":
+        """
+        Example:
+        >>> delta_c1 = CoordOffset(1, 1)
+        >>> delta_c2 = CoordOffset(2, 2)
+        >>> delta_c = delta_c1 - delta_c2
+        delta_c: CoordOffset(-1, -1)
+        """
+        if not isinstance(__other, CoordOffset):
+            raise TypeError(f"Unsupported type: {type(__other)}")
 
-    def __init__(self, _x: int, _y: int) -> None:
-        if not (-32 < _x < 32 and -32 < _y < 32):
-            raise ValueError(f"-32 < x < 32, -32 < y < 32: ({_x}, {_y})")
-
-        self.x, self.y = _x, _y
-
-    def __add__(self, other):
-        if isinstance(other, CoordOffset):
-            return CoordOffset(self.x + other.x, self.y + other.y)
-        else:
-            return Coord(self.x + other.x, self.y + other.y)
+        return CoordOffset(
+            self.delta_x - __other.delta_x, self.delta_y - __other.delta_y
+        )
 
-    def __sub__(self, other) -> "CoordOffset":
-        if isinstance(other, Coord):
-            raise TypeError("A CoordOffset cannot substract a Coord")
+    def __isub__(self, __other: "CoordOffset") -> "CoordOffset":
+        """
+        Example:
+        >>> delta_c = CoordOffset(1, 1)
+        >>> delta_c -= CoordOffset(1, 1)
+        delta_c: CoordOffset(0, 0)
+        """
+        if not isinstance(__other, CoordOffset):
+            raise TypeError(f"Unsupported type: {type(__other)}")
+
+        self.delta_x -= __other.delta_x
+        self.delta_y -= __other.delta_y
+
+        return self
+
+    def __eq__(self, __other: "CoordOffset") -> bool:
+        """
+        Example:
+        >>> CoordOffset(4, 5) == CoordOffset(4, 6)
+        False
+        """
+        if not isinstance(__other, CoordOffset):
+            raise TypeError(f"Unsupported type: {type(__other)}")
+
+        return self.delta_x == __other.delta_x and self.delta_y == __other.delta_y
+
+    def __ne__(self, __other: "CoordOffset") -> bool:
+        """
+        Example:
+        >>> CoordOffset(4, 5) != CoordOffset(4, 6)
+        True
+        """
+        if not isinstance(__other, CoordOffset):
+            raise TypeError(f"Unsupported type: {type(__other)}")
 
-        return CoordOffset(self.x - other.x, self.y - other.y)
+        return self.delta_x != __other.delta_x or self.delta_y != __other.delta_y
```

## paitest/frames/coord.pyi

```diff
@@ -1,29 +1,40 @@
-from typing import Tuple, overload
+from typing import Tuple, Union, Optional, overload
 
 class Coord:
     x: int = ...
     y: int = ...
+    def __init__(self, _x: Union[Tuple[int, int], int], _y: Optional[int] = None) -> None: ...
+    @classmethod
+    def from_tuple(cls, pos) -> Coord: ...
+    @classmethod
+    def default(cls) -> Coord: ...
+    def __add__(self, __other: CoordOffset) -> Coord: ...
     @overload
-    def __init__(self, _x: Tuple[int, int]) -> None: ...
+    def __sub__(self, __other: Coord) -> CoordOffset: ...
     @overload
-    def __init__(self, _x: int, _y: int) -> None: ...
-    def __add__(self, other) -> Coord: ...
-    def __sub__(self, other) -> CoordOffset: ...
-    def __eq__(self, other) -> bool: ...
-    def __ne__(self, other) -> bool: ...
-    def __lt__(self, other) -> bool: ...
-    def __gt__(self, other) -> bool: ...
-    def __le__(self, other) -> bool: ...
-    def __ge__(self, other) -> bool: ...
+    def __sub__(self, __other: CoordOffset) -> Coord: ...
+    def __eq__(self, __other: Coord) -> bool: ...
+    def __ne__(self, __other: Coord) -> bool: ...
+    def __lt__(self, __other: Coord) -> bool: ...
+    def __gt__(self, __other: Coord) -> bool: ...
+    def __le__(self, __other: Coord) -> bool: ...
+    def __ge__(self, __other: Coord) -> bool: ...
     def __str__(self) -> str: ...
+    def __repr__(self) -> str: ...
+    def to_tuple(self) -> Tuple[int, int]: ...
+    @property
+    def address(self) -> int: ...
 
-    __repr__ = __str__
-
-    ...
-
-class CoordOffset(Coord):
-    def __init__(self, _x: int, _y: int) -> None: ...
-    def __add__(self, other) -> CoordOffset | Coord: ...
-    def __sub__(self, other) -> CoordOffset: ...
-
-    ...
+class CoordOffset:
+    delta_x: int = ...
+    delta_y: int = ...
+    def __init__(self, delta_x: int, delta_y: int) -> None: ...
+    @overload
+    def __add__(self, __other: Coord) -> Coord: ...
+    @overload
+    def __add__(self, __other: CoordOffset) -> CoordOffset: ...
+    def __iadd__(self, __other: CoordOffset) -> CoordOffset: ...
+    def __sub__(self, __other: CoordOffset) -> CoordOffset: ...
+    def __isub__(self, __other: CoordOffset) -> CoordOffset: ...
+    def __eq__(self, __other: CoordOffset) -> bool: ...
+    def __ne__(self, __other: CoordOffset) -> bool: ...
```

## paitest/frames/frame.py

```diff
@@ -94,17 +94,17 @@
     @staticmethod
     def _GenParamReg(
         test_chip_coord: Coord,
         *,
         is_random: bool = True,
         is_legal: bool = False,
         weight_width_type: Optional[WeightPrecisionType] = None,
-        lcn_type: Optional[LCNTypes] = None,
-        input_width_type: Optional[InputWidthType] = None,
-        spike_width_type: Optional[SpikeWidthType] = None,
+        lcn_type: Optional[LCNExtensionType] = None,
+        input_width_type: Optional[InputWidthFormatType] = None,
+        spike_width_type: Optional[SpikeWidthFormatType] = None,
         neuron_num: Optional[int] = None,
         pool_max_en: Optional[bool] = None,
         tick_wait_start: Optional[int] = None,
         tick_wait_end: Optional[int] = None,
         snn_en: Optional[bool] = None,
         target_lcn: Optional[int] = None,
     ) -> Tuple[int, ...]:
@@ -117,18 +117,16 @@
                 # Don't care 'tick_wait_start' split in #1 and #2
                 for _ in range(2):
                     param_reg.append(random.randint(0, FM.GENERAL_PAYLOAD_MASK))
 
                 param_reg[1] = (param_reg[1] & (~CFM.TEST_CHIP_ADDR_HIGH3_MASK)) | high3
                 param_reg.append(low7 << CFM.TEST_CHIP_ADDR_LOW7_OFFSET)
             else:
-                # Do legal geenration
-                pass
-        else:
-            pass
+                # DTODO o legal generation
+                raise NotImplementedError
 
         return tuple(param_reg)
 
     """Functions of Test Frames Generation"""
 
     @staticmethod
     def _GenTestFrame(
@@ -216,16 +214,15 @@
             "tick_wait_end": 0,
             "SNN_EN": 0,
             "target_LCN": 0,
             "test_chip_coord": Coord(0, 0),
         }
 
     def decode(self, frames: Union[int, List[int], Tuple[int, ...]]) -> Dict[str, Any]:
-        """
-        Call for decoding a frame or a valid group of frames.
+        """Call for decoding a frame or a valid group of frames.
 
         Support single frame decoding & a group of 3 frames only.
         """
         if isinstance(frames, int):
             self.groups_len = 1
             self._frame = frames
         else:
@@ -330,15 +327,15 @@
 
     def _decode_testin2(self) -> None:
         pass
 
     def _info(self, subtype: FST) -> None:
         self._general_info()
 
-        if subtype == FST.CONFIG_TYPE2:
+        if subtype is FST.CONFIG_TYPE2:
             return self._config2_info()
         else:
             raise NotImplementedError
 
     def _general_info(self) -> None:
         print("General info of frame: 0x%x" % self._frame)
         print("#1  Frame type:         %s" % self._get_subtype())
@@ -368,16 +365,15 @@
         print("#5  Neuron num:         %d" % self._param_reg_dict["neuron_num"])
         print("#6  Pool max enable:    %d" % self._param_reg_dict["pool_max"])
         print("#7  Tick wait start:    0x%x" % self._param_reg_dict["tick_wait_start"])
         print("#8  Tick wait end:      0x%x" % self._param_reg_dict["tick_wait_end"])
         print("#9  SNN enable:         %d" % self._param_reg_dict["SNN_EN"])
         print("#10 Target LCN:         0x%x" % self._param_reg_dict["target_LCN"])
 
-        # type: ignore
-        test_chip_coord: Coord = self._param_reg_dict["test_chip_coord"]
+        test_chip_coord: Coord = self._param_reg_dict["test_chip_coord"] # type: ignore
         print(
             "#11 Test chip coord:    [0x%02x | 0x%02x]"
             % (test_chip_coord.x, test_chip_coord.y)
         )
 
     def _test2_info(self) -> None:
         pass
@@ -423,16 +419,15 @@
         ) & CFM.TARGET_LCN_MASK
 
         high3 = self._frames_group[1] >> CFM.TEST_CHIP_ADDR_HIGH3_OFFSET
         low7 = self._frames_group[2] >> CFM.TEST_CHIP_ADDR_LOW7_OFFSET
         self._param_reg_dict["test_chip_coord"] = test_chip_addr_combine(high3, low7)
 
     def _decode_direction(self) -> Direction:
-        # type: ignore
-        test_chip_coord: Coord = self._param_reg_dict["test_chip_coord"]
+        test_chip_coord: Coord = self._param_reg_dict["test_chip_coord"] # type: ignore
         offset = test_chip_coord - self._get_chip_coord()
 
         try:
             direction = Direction(offset)
             return direction
         except:
             raise ValueError("Offset is invalid. Check the parameters.")
```

## paitest/frames/frame_params.py

```diff
@@ -1,8 +1,8 @@
-from enum import Enum, Flag, unique
+from enum import Enum, IntEnum, Flag, unique
 
 from .coord import CoordOffset
 
 
 @unique
 class CoreType(Enum):
     CORE_TYPE_OFFLINE = 1
@@ -10,17 +10,17 @@
 
 
 @unique
 class FrameType(Enum):
     """Types of Frames"""
 
     FRAME_CONFIG = 0
-    FRAME_TEST = 0x1
-    FRAME_WORK = 0x2
-    FRAME_UNKNOWN = 0x3
+    FRAME_TEST = 1
+    FRAME_WORK = 2
+    FRAME_UNKNOWN = 3
 
 
 @unique
 class FrameSubType(Flag):
     """Sub-types of Configuration Frames"""
 
     CONFIG_TYPE1 = 0b0000
@@ -155,57 +155,75 @@
 
     """Frame #3"""
     TEST_CHIP_ADDR_LOW7_OFFSET = 23
     TEST_CHIP_ADDR_LOW7_MASK = (1 << 7) - 1
 
 
 @unique
-class WeightPrecisionType(Enum):
-    """Wight precision of crossbar"""
+class WeightPrecisionType(IntEnum):
+    """Weight precision of crossbar. 2-bit.
+
+    - `WEIGHT_WIDTH_XBIT` for X-bit. Default value is `WEIGHT_WIDTH_8BIT`.
+    """
 
     WEIGHT_WIDTH_1BIT = 0
     WEIGHT_WIDTH_2BIT = 1
     WEIGHT_WIDTH_4BIT = 2
-    WEIGHT_WIDTH_8BIT = 3
+    WEIGHT_WIDTH_8BIT = 3  # Default value.
+    WEIGHT_WIDTH_MAX = 4
 
 
 @unique
-class LCNTypes(Enum):
-    """Scale of Fan-in extension"""
+class LCNExtensionType(IntEnum):
+    """Scale of Fan-in extension. 4-bit.
+
+    - X-time LCN extension. Default value is `LCN_1X`.
+
+    NOTE:
+    - For ANN mode, `LCN_1X` = 144x.
+    - For BANN/SNN mode, `LCN_1X` = 1152x.
+    """
 
-    LCN_1X = 0
+    LCN_1X = 0  # Default value.
     LCN_2X = 1
     LCN_4X = 2
     LCN_8X = 3
     LCN_16X = 4
     LCN_32X = 5
     LCN_64X = 6
+    LCN_MAX = 7
 
 
 @unique
-class InputWidthType(Enum):
-    """Format of Input Spike"""
+class InputWidthFormatType(Enum):
+    """Format of input spike. 1-bit.
 
-    INPUT_WIDTH_1BIT = 0
-    INPUT_WIDTH_8BIT = 1
+    - `WIDTH_1BIT`: 1-bit spike. Default value.
+    - `WIDTH_8BIT`: 8-bit activation.
+    """
+
+    WIDTH_1BIT = 0
+    WIDTH_8BIT = 1
 
 
 @unique
-class SpikeWidthType(Enum):
-    """Format of Output Spike"""
+class SpikeWidthFormatType(Enum):
+    """Format of output spike. 1-bit.
+
+    - `WIDTH_1BIT`: 1-bit spike. Default value.
+    - `WIDTH_8BIT`: 8-bit activation.
+    """
 
-    SPIKE_WIDTH_1BIT = 0
-    SPIKE_WIDTH_8BIT = 1
+    WIDTH_1BIT = 0  # Default value.
+    WIDTH_8BIT = 1
 
 
 @unique
 class Direction(Enum):
     """
-    For [x, y]
-    Left to right: +x
-    Top to bottom: +y
+    Left to right: +x, Top to bottom: +y
     """
 
     EAST = CoordOffset(1, 0)
     SOUTH = CoordOffset(0, 1)
     WEST = CoordOffset(-1, 0)
     NORTH = CoordOffset(0, -1)
```

## paitest/paitest.py

```diff
@@ -1,101 +1,116 @@
 import random
 import sys
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
-
 from .frames import Addr2Coord, Coord, Coord2Addr, Direction, FrameGen
 from .frames import FrameMask as FM
 from .frames import FrameSubType as FST
 from .log import logger
+import warnings
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 
 
 class paitest:
     def __init__(
         self,
         direction="EAST",
         fixed_chip_coord: Tuple[int, int] = (0, 0),
+        *,
+        test_chip_coord: Optional[Tuple[int, int]] = None,
     ) -> None:
-        """
-        Params:
-        - direction: The direction relative to the PAICORE. Default is 'EAST'.
-        - fixed_chip_coord: The chip address of the PAICORE under test. Default is (0, 0).
+        """Paitest initialization.
+
+        Arguments:
+            - direction: The direction relative to the PAICORE. Default is 'EAST'.
+            - fixed_chip_coord: The chip address of the PAICORE under test.
+            - test_chip_coord: The address of the FPGA relative to the PAICORE.
+                If you pass one, use this at high priority instead of 'direction'.
         """
         self._verbose: bool = True
         self._fixed_chip_coord: Coord = Coord(fixed_chip_coord)
         self._masked_core_coord: Coord
         self._fixed_core_star_coord: Coord = Coord(0, 0)
         self._test_chip_coord: Coord
 
-        self._ensure_direction(direction)
+        if not isinstance(test_chip_coord, Tuple):
+            warnings.warn(
+                "Parameter 'direction' will be deprecated in the future version. Use 'test_chip_coord' instead.",
+                DeprecationWarning,
+            )
+
+            self._ensure_direction(direction)
+            self._test_chip_coord = self._direction.value + self._fixed_chip_coord
+        else:
+            self._test_chip_coord = Coord(test_chip_coord)
 
     def Get1GroupForNCoresWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
         verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
-        """
-        Generate 1 group(case) for 'N' random cores coordinates with 'N' different parameters.
+        """Generate 1 group(case) for 'N' random cores coordinates with 'N' different parameters.
 
-        Params:
-        - `N`: How many cores coordinates under test.
-        - `save_dir`: Where to save the frames files.
-        - `masked_core_coord`: to avoid generating the specific core coordinate.
-        - `gen_txt`: to save frames into text files instead of default binary files.
-        - `verbose`: whether to display the log.
+        Arguments:
+            - N: How many cores coordinates under test.
+            - save_dir: Where to save the frames files.
+            - masked_core_coord: to avoid generating the specific core coordinate.
+            - gen_txt: to save frames into text files instead of default binary files.
+            - verbose: whether to display the log.
 
-        :return: 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
+        Returns:
+            - 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
         """
         self._ensure_cores(N)
 
         if save_dir:
             work_dir = self._ensure_dir(save_dir)
         else:
             work_dir = None
 
-        # 1. Get the test chip coordinate.
-        test_chip_coord: Coord = self._direction.value + self._fixed_chip_coord
-
-        # 2. Get N core coordinates list.
+        # 1. Get N core coordinates list.
         if isinstance(masked_core_coord, Tuple):
             _masked_core_coord = Coord(masked_core_coord)
         else:
             _masked_core_coord = None
 
         core_coords = self._GetNCoresCoord(N, _masked_core_coord)
 
-        # 3. Get N parameters reg.
+        # 2. Get N parameters reg.
         params = self._GetNParams(N, core_coords, False)
 
         cf_list: List[int] = []
         ti_list: List[int] = []
         to_list: List[int] = []
 
         for i in range(N):
             if verbose:
                 logger.info(f"Generating test group #{i+1}/{N}...")
+            
             core_coord = core_coords[i]
             param = params[i]
 
             for j in range(3):
                 config_frame = FrameGen.GenConfigFrame(
                     FST.CONFIG_TYPE2,
                     self._fixed_chip_coord,
                     core_coord,
                     self._fixed_core_star_coord,
                     param[j],
                 )
                 testout_frame = FrameGen.GenTest2OutFrame(
-                    test_chip_coord, core_coord, self._fixed_core_star_coord, param[j]
+                    self._test_chip_coord,
+                    core_coord,
+                    self._fixed_core_star_coord,
+                    param[j],
                 )
                 cf_list.append(config_frame)
                 to_list.append(testout_frame)
 
                 if verbose:
                     logger.info(
                         "Config frame   #%d/3:  0x%x in group #%d/%d"
@@ -123,45 +138,42 @@
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
         verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
-        """
-        Generate 1 group(case) for 'N' random cores coordinates with the same parameters.
+        """Generate 1 group(case) for 'N' random cores coordinates with the same parameters.
 
-        Params:
-        - `N`: How many cores coordinates under test.
-        - `save_dir`: Where to save the frames files.
-        - `masked_core_coord`: to avoid generating the specific core coordinate.
-        - `gen_txt`: to save frames into text files instead of default binary files.
-        - `verbose`: whether to display the log.
+        Arguments:
+            - N: How many cores coordinates under test.
+            - save_dir: Where to save the frames files.
+            - masked_core_coord: to avoid generating the specific core coordinate.
+            - gen_txt: to save frames into text files instead of default binary files.
+            - verbose: whether to display the log.
 
-        :return: 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
+        Returns:
+            - 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
         """
         self._ensure_cores(N)
 
         if save_dir:
             work_dir = self._ensure_dir(save_dir)
         else:
             work_dir = None
 
-        # 1. Get the test chip coordinate.
-        test_chip_coord = self._direction.value + self._fixed_chip_coord
-
-        # 2. Get N core coordinates list.
+        # 1. Get N core coordinates list.
         if isinstance(masked_core_coord, Tuple):
             _masked_core_coord = Coord(masked_core_coord)
         else:
             _masked_core_coord = None
 
         core_coords = self._GetNCoresCoord(N, _masked_core_coord)
 
-        # 3. Get the parameters reg.
+        # 2. Get the parameters reg.
         param: Tuple[int, ...] = self._Get1Param(core_coords, False)
 
         cf_list: List[int] = []
         ti_list: List[int] = []
         to_list: List[int] = []
 
         for i in range(N):
@@ -174,15 +186,18 @@
                     FST.CONFIG_TYPE2,
                     self._fixed_chip_coord,
                     core_coord,
                     self._fixed_core_star_coord,
                     param[j],
                 )
                 testout_frame = FrameGen.GenTest2OutFrame(
-                    test_chip_coord, core_coord, self._fixed_core_star_coord, param[j]
+                    self._test_chip_coord,
+                    core_coord,
+                    self._fixed_core_star_coord,
+                    param[j],
                 )
                 cf_list.append(config_frame)
                 to_list.append(testout_frame)
 
                 if verbose:
                     logger.info(
                         "Config frame   #%d/3:  0x%x in group #%d/%d"
@@ -210,45 +225,42 @@
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
         verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
-        """
-        Generate 'N' groups(cases) for 1 random core coordinate with 'N' different parameters.
+        """Generate 'N' groups(cases) for 1 random core coordinate with 'N' different parameters.
 
-        Params:
-        - `N`: How many test groups(cases) of 1 core will be generated.
-        - `save_dir`: Where to save the frames files.
-        - `masked_core_coord`: to avoid generating the specific core coordinate.
-        - `gen_txt`: to save frames into text files instead of default binary files.
-        - `verbose`: whether to display the log.
+        Arguments:
+            - N: How many test groups(cases) of 1 core will be generated.
+            - save_dir: Where to save the frames files.
+            - masked_core_coord: to avoid generating the specific core coordinate.
+            - gen_txt: to save frames into text files instead of default binary files.
+            - verbose: whether to display the log.
 
-        :return: 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
+        Returns:
+            - 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
         """
         self._ensure_cores(N)
 
         if save_dir:
             work_dir = self._ensure_dir(save_dir)
         else:
             work_dir = None
 
-        # 1. Get the test chip coordinate.
-        test_chip_coord = self._direction.value + self._fixed_chip_coord
-
-        # 2. Get the core coordinates list.
+        # 1. Get the core coordinates list.
         if isinstance(masked_core_coord, Tuple):
             _masked_core_coord = Coord(masked_core_coord)
         else:
             _masked_core_coord = None
 
         core_coord = self._Get1CoreCoord(_masked_core_coord)
 
-        # 3. Get the parameters reg.
+        # 2. Get the parameters reg.
         params = self._GetNParams(N, core_coord, False)
 
         cf_list: List[int] = []
         ti_list: List[int] = []
         to_list: List[int] = []
 
         for i in range(N):
@@ -261,15 +273,18 @@
                     FST.CONFIG_TYPE2,
                     self._fixed_chip_coord,
                     core_coord,
                     self._fixed_core_star_coord,
                     param[j],
                 )
                 testout_frame = FrameGen.GenTest2OutFrame(
-                    test_chip_coord, core_coord, self._fixed_core_star_coord, param[j]
+                    self._test_chip_coord,
+                    core_coord,
+                    self._fixed_core_star_coord,
+                    param[j],
                 )
                 cf_list.append(config_frame)
                 to_list.append(testout_frame)
 
                 if verbose:
                     logger.info(
                         "Config frame   #%d/3:  0x%x in group #%d/%d"
@@ -294,22 +309,22 @@
         return tuple(cf_list), tuple(ti_list), tuple(to_list)
 
     def ReplaceCoreCoord(
         self,
         frames: Union[int, List[int], Tuple[int, ...]],
         new_core_coord: Optional[Union[Tuple[int, int], Coord]] = None,
     ) -> Union[int, Tuple[int, ...]]:
-        """
-        Replace the core coordinate with the new one.
+        """Replace the core coordinate with the new one.
 
-        Params:
-        - frames: of which the core coordinate you want to replace. It can be a single frame, or a list or tuple.
-        - new_core_coord: The new core coordinate. If not specified, it will generate one randomly.
+        Arguments:
+            - frames: of which the core coordinate you want to replace. It can be a single frame, or a list or tuple.
+            - new_core_coord: The new core coordinate. If not specified, it will generate one randomly.
 
-        :return: the frame or frames after replacement.
+        Returns:
+            - the frame or frames after replacement.
         """
         if isinstance(frames, int):
             _frame = frames
         else:
             _frame = frames[0]
 
         if isinstance(new_core_coord, Tuple):
@@ -334,38 +349,37 @@
 
     @staticmethod
     def SaveFrames(
         save_path: Union[str, Path],
         frames: Union[int, List[int], Tuple[int, ...]],
         byteorder="big",
     ) -> None:
-        """
-        Write frames into specific text or binary file. Files with '.bin' suffix is recommended.
+        """Write frames into specific text or binary file. Files with '.bin' suffix is recommended.
 
-        Params:
-        - save_path: The path of files.
-        - frames: A single frame or list or tuple of frames.
-        - byteorder: Big or little-edian format.
+        Arguments:
+            - save_path: The path of files.
+            - frames: A single frame or list or tuple of frames.
+            - byteorder: Big or little-edian format.
         """
 
         _path = Path(save_path)
         _suffix: str = _path.suffix
 
         if _suffix != ".bin" and _suffix != ".txt":
             raise NotImplementedError(f"File with suffix {_suffix} is not supported!")
 
         assert byteorder in ["little", "big"]
 
         if _suffix == ".bin":
             with open(_path, "wb") as f:
                 if isinstance(frames, int):
-                    f.write(frames.to_bytes(8, byteorder))
+                    f.write(frames.to_bytes(8, byteorder))  # type: ignore
                 else:
                     for frame in frames:
-                        f.write(frame.to_bytes(8, byteorder))
+                        f.write(frame.to_bytes(8, byteorder))  # type: ignore
 
         else:
             if byteorder == "little":
                 logger.warning(
                     "Saving into txt file in little-edian format is not supported!"
                 )
 
@@ -379,24 +393,26 @@
                         _str64 = bin(frame).split("0b")[1]
                         _str64 = _str64.zfill(64)
                         f.write(_str64 + "\n")
 
         logger.info(f"Saved frame(s) into {_path} OK")
 
     def _Get1CoreCoord(self, masked_coord: Optional[Coord] = None) -> Coord:
-        """
-        Generate a random core coordinate. Indicate the masked one to avoid generating the same one
+        """Generate a random core coordinate.
+
+        Indicate the masked one to avoid generating the same one
         """
         return self._GetNCoresCoord(N=1, masked_coord=masked_coord)[0]
 
     def _GetNCoresCoord(
         self, N: int, masked_coord: Optional[Coord] = None
     ) -> List[Coord]:
-        """
-        Generate 'N' unique cores coordinates. Optional for excluding one masked core address
+        """Generate 'N' unique cores coordinates.
+
+        Optional for excluding one masked core address
         """
 
         def _CoordGenerator():
             coordinates = set()
 
             if isinstance(masked_coord, Coord):
                 coordinates.add((masked_coord.x, masked_coord.y))
@@ -429,36 +445,33 @@
 
     def _GetNParams(
         self,
         N: int,
         core_coords: Union[List[Coord], Coord],
         is_legal: bool = False,
     ) -> List[Tuple[int, ...]]:
-        """
-        Generate 'N' random parameters register.
+        """Generate 'N' random parameters register.
 
-        Params:
-        - `is_legal`: whether to generate legal parameters for every core
+        Arguments:
+            - is_legal: whether to generate legal parameters for every core
         """
 
         def _ParamGenerator():
-            test_chip_coord: Coord = self._direction.value + self._fixed_chip_coord
-
             while True:
                 for core_coord in _core_coords:
                     if is_legal:
-                        # TODO: Do legal generation here, including direction config
+                        # TODO Do legal generation here, including direction config
                         raise NotImplementedError
                     else:
                         param = FrameGen.GenConfigGroup(
                             FST.CONFIG_TYPE2,
                             self._fixed_chip_coord,
                             core_coord,
                             self._fixed_core_star_coord,
-                            test_chip_coord,
+                            self._test_chip_coord,
                         )
 
                     yield param
 
         if isinstance(core_coords, Coord):
             _core_coords = [core_coords]
         else:
@@ -480,16 +493,17 @@
         return (frame & mask) | (new_core_addr << FM.GENERAL_CORE_ADDR_OFFSET)
 
     def _ReplaceCoreCoordInNFrames(
         self,
         frames: List[int],
         new_core_coord: Coord,
     ) -> Tuple[int, ...]:
-        """
-        Replace the core coordinate of frames with a specific or random one. Keep the parameters still.
+        """Replace the core coordinate of frames with a specific or random one.
+
+        Keep the parameters still.
         """
         mask = FM.GENERAL_MASK & (
             ~(FM.GENERAL_CORE_ADDR_MASK << FM.GENERAL_CORE_ADDR_OFFSET)
         )
 
         new_core_addr = Coord2Addr(new_core_coord)
```

## paitest/paitest.pyi

```diff
@@ -7,20 +7,24 @@
 
 class paitest:
     if sys.version_info >= (3, 8):
         def __init__(
             self,
             direction: Literal["EAST", "SOUTH", "WEST", "NORTH"] = "EAST",
             fixed_chip_coord: Tuple[int, int] = (0, 0),
+            *,
+            test_chip_coord: Optional[Tuple[int, int]] = None,
         ) -> None: ...
     else:
         def __init__(
             self,
             direction: str = "EAST",
             fixed_chip_coord: Tuple[int, int] = (0, 0),
+            *,
+            test_chip_coord: Optional[Tuple[int, int]] = None,
         ) -> None: ...
 
     def Get1GroupForNCoresWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
```

## Comparing `paitest-1.1.0.dist-info/METADATA` & `paitest-1.1.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: paitest
-Version: 1.1.0
+Version: 1.1.1
 Summary: Test module for PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAITest
-License: AGPL v3.0
+License: MIT
 Keywords: PAICookers,PAITest,PAICORE
 Author: KafCoppelia
 Author-email: k740677208@gmail.com
 Requires-Python: >=3.6,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -24,83 +24,78 @@
 
 # PAITest
 
 </div>
 
 ## 📦 版本
 
-[v1.1.0](https://github.com/PAICookers/PAITest/releases/tag/v1.1.0)
+[v1.1.1](https://github.com/PAICookers/PAITest/releases/tag/v1.1.1)
 
 ✨支持大/小端格式输出
 
-## 🛠️ 使用生成
+## 🛠️ 使用
 
 配置帧及对应测试输入帧，以实现硬件通路的简单测试，后续将芯片实际测试输出帧与预期结果进行对比即可。
 
 ⚠️ 由于配置帧/测试帧I型需要配合串口配置使用，因此目前仅采用**配置/测试帧II型**方案，且 `CHIP_ADDR` 与 `CORE*_ADDR` 均固定为 `(0, 0)`。
 
-1. 实例化 `PAITest`
+1. 实例化 `PAITest`。在这个版本下，参数 `test_chip_coord` 的优先级大于 `direction`；当仅配置 `dirction` 时通过此计算 `test_chip_coord`，否则使用 `test_chip_coord` 参数
 
    ```python
    from paitest import paitest
 
-   # Define the direction of test chip
-   PAITestManager = paitest("EAST")
+   # Set the address of chip under test and the test chip address.
+   PAITestManager = paitest("EAST", (0, 0), test_chip_coord=(1, 0))
    ```
-
-2. `Get1GroupForNCoresWithNParams`，产生一组针对 `N` 个核的配置-测试帧，每个核配置**不同参数**。可以指定单个需要**屏蔽**的核坐标
+2. `Get1GroupForNCoresWithNParams`，产生1组针对 `N` 个核的配置-测试帧，每个核配置**不同参数**。可以指定单个需要**屏蔽**的核坐标
 
    ```python
    groups = 10             # Generate 10 groups
    save_to_dir="./test"    # Save frames into ./test directory
 
    # Generate configuration frames, testin & testout frames
    cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups, save_dir=save_to_dir, verbose=True)
 
    # Mask a cord coordinate so that avoid generating the same coordinate.
    cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups,
        save_dir=save_to_dir, masked_core_coord=(12, 16), gen_txt=True)
    ```
 
    ⚠️ 指定 `verbose=True` 以开启日志显示，默认关闭
-
 3. `Get1GroupForNCoresWith1Param`，产生1组针对 `N` 个核的配置-测试帧，每个核配置**相同参数**。可以指定单个需要**屏蔽**的核坐标
 
    ```python
    # Same as Get1GroupForNCoresWithNParams
    cf, ti, to = PAITestManager.Get1GroupForNCoresWith1Param(10, save_dir="./test")
    ```
-
 4. `GetNGroupsFor1CoreWithNParams`，产生 `N` 组针对1个核的配置-测试帧，每个核配置**不同参数**。可以指定单个需要**屏蔽**的核坐标
 
    ```python
    # Same as Get1GroupForNCoresWithNParams
    cf, ti, to = PAITestManager.GetNGroupsFor1CoreWithNParams(1, save_dir="./test")
    ```
-
 5. `ReplaceCoreCoord`，替换**单个**或**一组**帧中的 `CORE_ADDR` 为指定坐标
 
    ```python
    # Replaced core coordinate with (9, 9)
    replaced = PAITestManager.ReplaceCoreCoord(original_frames, (9, 9))
    ```
 
    ⚠️ 一组指一组完整的配置帧，包含3帧。对于测试输入帧，即为单帧。
-
 6. `SaveFrames`，保存帧数据至指定文件，支持 `.bin` 或 `.txt` 格式，支持指定大/小端输出
 
    ```python
    # Save into binary files with big-edian format(default)
    PAITestManager.SaveFrames("./test/config.bin", replaced, byteorder="big")
 
    # Or text files
    PAITestManager.SaveFrames("./test/config.txt", replaced)
    ```
 
    ⚠️ 指定 `byteorder="big"/"little"` 以大/小端格式储存帧数据，默认大端
 
 ## 🗓️ TODO
 
-- [x] 上板验证
+- [X] 上板验证
 - [ ] 参数检验
 - [ ] 配置/测试帧III/IV型
```

## Comparing `paitest-1.1.0.dist-info/RECORD` & `paitest-1.1.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 paitest/__init__.py,sha256=tDpSaCHeqc6HTLOj_rioHEWo6LyxDQYWlKQh-fryLCo,63
 paitest/frames/__init__.py,sha256=h-JK-OD_NW7z77A0HJwDV3k_QVi2MYoowdrxHGPqImw,342
-paitest/frames/coord.py,sha256=MRVgxWLvvoIxPY5NUEZYqfsFsW-tAUBroH-Y_WmKw84,2581
-paitest/frames/coord.pyi,sha256=bwNKBsEg4mftwxpPboiHhvZnrLdzptSJjhuX09a3Tnw,823
-paitest/frames/frame.py,sha256=nQKk3al98QmJjuKjchVBK9TkBxCmOtuiKWt2w16-oK4,14257
-paitest/frames/frame_params.py,sha256=NhxjycQ7MPm5t4mW_CSDlFHaJG_Sgdxfp_nkxDzZiC0,4707
+paitest/frames/coord.py,sha256=nzOjZ7EI-GiRyEHmkoaR2HY-N2hGISN0ngq7PBGiL8k,8635
+paitest/frames/coord.pyi,sha256=0NH-oqojYIr3PiDEovsz5H7_0NIp_BrXhC9kn78Ci3Q,1553
+paitest/frames/frame.py,sha256=1zak3MLFKP5ZofZa4uaq7ySIz4DVHjTr1zF4ncIoN7g,14247
+paitest/frames/frame_params.py,sha256=awJ4Q3CV2_kPDbEXhrlf7OozuKyQ-dDuMULvaFs0SWc,5239
 paitest/log.py,sha256=0wn34g4m7nr837MwHNNsgZiNr9me-ywlGtfV4-iOTe4,230
-paitest/paitest.py,sha256=Nr7cRU7Z0Fldfh6IhbdcYEAD17RYuZZo3k5oR2cPJMo,18940
-paitest/paitest.pyi,sha256=U0xHoDrYYamSsimotR56Tp2k-i8JEnM2k-5XAIpU_Y8,1990
-paitest-1.1.0.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-paitest-1.1.0.dist-info/METADATA,sha256=tQ4EW9hztChpbyx7QoxgbD48UOrJrdMQFf07rEPaYeI,3763
-paitest-1.1.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-paitest-1.1.0.dist-info/RECORD,,
+paitest/paitest.py,sha256=BY3H0Wq76kjOEMbCeGJk-bYq7yVdWARJ1tB8aAlNews,19487
+paitest/paitest.pyi,sha256=-YLExbkeJiWO4IG8MyDqAYwkzWoQxrIaumNsqswM9Fk,2146
+paitest-1.1.1.dist-info/LICENSE,sha256=X4XrKpP3ip4RN1qZxegkUYv0mgj_Zn94LZ1trevryKo,1067
+paitest-1.1.1.dist-info/METADATA,sha256=a8K63zRV0BsZSTzr35Guw_UvZ2-a5qsHUNKzwGR7U4k,3988
+paitest-1.1.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+paitest-1.1.1.dist-info/RECORD,,
```

