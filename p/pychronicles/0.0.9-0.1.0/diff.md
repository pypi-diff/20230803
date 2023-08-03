# Comparing `tmp/pychronicles-0.0.9.tar.gz` & `tmp/pychronicles-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychronicles-0.0.9.tar", last modified: Tue Oct 18 15:29:36 2022, max compression
+gzip compressed data, was "pychronicles-0.1.0.tar", max compression
```

## Comparing `pychronicles-0.0.9.tar` & `pychronicles-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,12 @@
-drwxrwxr-x   0 tguyet    (1001) tguyet    (1001)        0 2022-10-18 15:29:36.044332 pychronicles-0.0.9/
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)       25 2022-10-18 10:07:43.000000 pychronicles-0.0.9/MANIFEST.in
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     5491 2022-10-18 15:29:36.044332 pychronicles-0.0.9/PKG-INFO
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     4239 2022-10-18 10:07:43.000000 pychronicles-0.0.9/README.md
-drwxrwxr-x   0 tguyet    (1001) tguyet    (1001)        0 2022-10-18 15:29:36.044332 pychronicles-0.0.9/pychronicles/
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)      325 2022-10-18 10:07:43.000000 pychronicles-0.0.9/pychronicles/__init__.py
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)   905848 2022-10-18 15:27:54.000000 pychronicles-0.0.9/pychronicles/chronicle.c
--rwxrwxr-x   0 tguyet    (1001) tguyet    (1001)  7746896 2022-10-18 15:28:06.000000 pychronicles-0.0.9/pychronicles/chronicle.cpython-38-x86_64-linux-gnu.so
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)    25019 2022-10-18 15:23:49.000000 pychronicles-0.0.9/pychronicles/chronicle.py
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)    10490 2022-10-18 15:24:12.000000 pychronicles-0.0.9/pychronicles/fchronicle.py
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     6155 2022-10-18 14:16:22.000000 pychronicles-0.0.9/pychronicles/mtlformula.py
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     6276 2022-10-18 14:17:23.000000 pychronicles-0.0.9/pychronicles/pandas_tpatterns.py
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     4803 2022-10-18 10:07:43.000000 pychronicles-0.0.9/pychronicles/timedsequence.py
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     3346 2022-10-18 10:07:43.000000 pychronicles-0.0.9/pychronicles/utils.py
-drwxrwxr-x   0 tguyet    (1001) tguyet    (1001)        0 2022-10-18 15:29:36.044332 pychronicles-0.0.9/pychronicles.egg-info/
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     5491 2022-10-18 15:29:35.000000 pychronicles-0.0.9/pychronicles.egg-info/PKG-INFO
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)      525 2022-10-18 15:29:36.000000 pychronicles-0.0.9/pychronicles.egg-info/SOURCES.txt
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)        1 2022-10-18 15:29:35.000000 pychronicles-0.0.9/pychronicles.egg-info/dependency_links.txt
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)       59 2022-10-18 15:29:35.000000 pychronicles-0.0.9/pychronicles.egg-info/requires.txt
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)       19 2022-10-18 15:29:35.000000 pychronicles-0.0.9/pychronicles.egg-info/top_level.txt
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)       38 2022-10-18 15:29:36.044332 pychronicles-0.0.9/setup.cfg
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     1205 2022-10-18 15:28:55.000000 pychronicles-0.0.9/setup.py
-drwxrwxr-x   0 tguyet    (1001) tguyet    (1001)        0 2022-10-18 15:29:36.044332 pychronicles-0.0.9/tests/
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)        0 2022-10-18 15:20:11.000000 pychronicles-0.0.9/tests/__init__.py
--rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     2536 2022-10-18 15:21:18.000000 pychronicles-0.0.9/tests/test_timedsequences.py
+-rw-r--r--   0        0        0    15360 2023-08-02 20:13:48.928040 pychronicles-0.1.0/README.md
+-rw-r--r--   0        0        0      462 2023-08-03 07:08:23.372728 pychronicles-0.1.0/pychronicles/__init__.py
+-rw-r--r--   0        0        0     5418 2023-08-03 07:07:28.133668 pychronicles-0.1.0/pychronicles/abstraction.py
+-rw-r--r--   0        0        0    35547 2023-08-03 07:07:29.861638 pychronicles-0.1.0/pychronicles/chronicle.py
+-rw-r--r--   0        0        0    12520 2023-08-03 07:07:32.677590 pychronicles-0.1.0/pychronicles/fchronicle.py
+-rwxr-xr-x   0        0        0     6003 2023-08-03 07:07:37.453509 pychronicles-0.1.0/pychronicles/mining/chronicle_mining.py
+-rw-r--r--   0        0        0     6535 2023-08-02 16:24:23.282630 pychronicles-0.1.0/pychronicles/mtlformula.py
+-rw-r--r--   0        0        0    14527 2023-08-03 07:07:34.397561 pychronicles-0.1.0/pychronicles/pandas_tpatterns.py
+-rw-r--r--   0        0        0     7652 2023-08-02 20:13:48.932040 pychronicles-0.1.0/pychronicles/timedsequence.py
+-rw-r--r--   0        0        0     3872 2023-08-03 07:07:36.013533 pychronicles-0.1.0/pychronicles/utils.py
+-rw-r--r--   0        0        0      517 2023-08-03 07:11:34.153485 pychronicles-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16276 1970-01-01 00:00:00.000000 pychronicles-0.1.0/PKG-INFO
```

### Comparing `pychronicles-0.0.9/pychronicles/chronicle.py` & `pychronicles-0.1.0/pychronicles/chronicle.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,310 +1,534 @@
 #!/bin/python3
 # -*- coding: utf-8 -*-
-"""
-Chronicles with pure NumPy implementation
+"""The module mainly defines the implementation of `Chronicle` class. This class provides the 
+basic functionalities to specify a chronicle and to recognize or enumerate chronicle occurrences 
+in a timed sequence (see TimeSequence class).
+
+Warning
+--------
+There are two possible modelings of time constraints: float or numpy.timedelta64. 
+The user has to be consistent: all temporal constraints must use the same type of duration and it must be consistent with 
+the one of the timed sequences (if you use chronicles on timed sequences)
+
+Example
+--------
+
+The following example illustrates the main functionalities of the `Chronicle` class.
+
+.. code-block:: python
+
+    # Example of sequence
+    seq = [ ("a", 1), ("c", 2), ("b", 3), ("a", 8), ("a", 10), ("b", 12), ("a", 15), ("c", 17), ("b", 20), ("c", 23), ("c", 25), ("b", 26), ("c", 28), ("b", 30) ]
+
+    dates = np.array(
+        [np.datetime64("1970-01-01") + np.timedelta64(e[1], "D") for e in seq],
+        dtype="datetime64",
+    )
+    data = np.array([e[0] for e in seq])
+
+    ts = TimedSequence(dates, data)
+
+    c = Chronicle()
+    c.add_event(0, "a")
+    c.add_event(1, "b")
+    c.add_event(2, "c")
+    c.add_constraint(0, 1, (np.timedelta64(4, "D"), np.timedelta64(10, "D")))
+    c.add_constraint(0, 2, (np.timedelta64(2, "D"), np.timedelta64(8, "D")))
+    c.add_constraint(1, 2, (np.timedelta64(3, "D"), np.timedelta64(13, "D")))
+    
+    try:
+        import matplotlib.pyplot as plt
+        c.draw()
+        plt.show()
+    except:
+        pass
+
+    print(c)
+    c.minimize()
+    print(c)
+
+    reco = c.match(ts)
+    print(f"Reconnaissance de la chronique: [{reco}]!")
+
+    reco = c.recognize(ts)
+    print(f"Reconnaissance de la chronique: [{reco}]!")
+
+    print(c)
+    c2 = c.copy()
+    c2.add_constraint(0, 2, (np.timedelta64(4, "D"), np.timedelta64(4, "D")))
+    print(c)
+
+    #################################
+    # Sequence with floats
+
+    dates = np.array([float(e[1]) for e in seq], dtype="float")
+    data = np.array([e[0] for e in seq])
+
+    ts = TimedSequence(dates, data)
+
+    c = Chronicle()
+    c.add_event(0, "a")
+    c.add_event(1, "b")
+    c.add_event(2, "c")
+    c.add_constraint(0, 1, (4.0, 10.0))
+    c.add_constraint(0, 2, (2.0, 8.0))
+    c.add_constraint(1, 2, (3.0, 13.0))
+
+    print(c)
+    c.minimize()
+    print(c)
+
+    reco = c.match(ts)
+    print(f"Reconnaissance de la chronique: [{reco}]!")
+
+    reco = c.recognize(ts)
+    print(f"Reconnaissance de la chronique: [{reco}]!")
 
-@author: Thomas Guyet
-@date: 08/2022
-@institution: Inria
-
-Perspectives:
----------------
-    * replace events types (int/str) by any event type with a __le__(item) function
-        where item is an element of a timeseries.
+    print(c)
+    c2 = c.copy()
+    c2.add_constraint(0, 2, (np.timedelta64(4, "D"), np.timedelta64(4, "D")))
+    print(c)
+
+Todo
+-----
+    Replace events types (int/str) by any event type with a __le__(item) function
+    where item is an element of a timeseries.
+
+:Authors:
+    Thomas Guyet, Inria
+:Date:
+    08/2023
 """
 
 import warnings
 import numpy as np
 import scipy.sparse.csgraph
 from datetime import datetime as dt
 
 ## typing features
-from typing import TypeVar, Union, Dict, Mapping,Tuple, Sequence, Any
+from typing import TypeVar, Union, Dict, Mapping, Tuple, Sequence, Any
 from pychronicles.timedsequence import TimedSequence
 
-#definition of a data frame type
-Chronicle = TypeVar('pychronicles.chronicle.Chronicle')
-#TimedSequence= TypeVar('pychronicles.timedsequence.TimedSequence')
+# definition of a data frame type
+Chronicle = TypeVar("pychronicles.chronicle.Chronicle")
+# TimedSequence= TypeVar('pychronicles.timedsequence.TimedSequence')
 ###
 
-maxdate=np.datetime64(dt.max)
+maxdate = np.datetime64(dt.max)
+
 
-def resize(l:Sequence[Any], n:int, d: Any = None):
+def resize(l: Sequence[Any], n: int, d: Any = None):
+    """:meta private:"""
     while len(l) < n:
         l.append(d)
 
 
-def days_to_timedelta64(val:float) -> np.timedelta64:
+def days_to_timedelta64(val: float) -> np.timedelta64:
     """
     Convertion function from number of days (float) to a time delta
 
-    parameters
-    ----------
-    - val (float)
-        number of days
-    return
-    -------
-
+    Parameters
+    -----------
+    val: float
+        number of days (can have several digits after the decimal point)
+
+    Returns
+    --------
+    numpy.timedelta64
+        A timedelta object that correspond to a duration of `val` days
+    
+    :meta private:
     """
     nbdays = int(val)
-    rest_hours = (val%1)*24
-    ret = np.timedelta64(nbdays,"D")
+    rest_hours = (val % 1) * 24
+    ret = np.timedelta64(nbdays, "D")
+
+    if rest_hours == 0:
+        return ret
 
-    if rest_hours==0: return ret
+    rest_minutes = (rest_hours % 1) * 60
+    rest_hours = int(rest_hours)
+    ret += np.timedelta64(rest_hours, "h")
 
-    rest_minutes = (rest_hours%1)*60
-    rest_hours=int(rest_hours)
-    ret += np.timedelta64(rest_hours,"h")
+    if rest_minutes == 0:
+        return ret
 
-    if rest_minutes==0: return ret
+    rest_seconds = (rest_minutes % 1) * 60
+    rest_minutes = int(rest_minutes)
+    ret += np.timedelta64(rest_minutes, "m")
 
-    rest_seconds = (rest_minutes%1)*60
-    rest_minutes=int(rest_minutes)
-    ret += np.timedelta64(rest_minutes,"m")
+    if rest_seconds == 0:
+        return ret
 
-    if rest_seconds==0: return ret
+    rest_milliseconds = (rest_seconds % 1) * 1000
+    rest_seconds = int(rest_seconds)
 
-    rest_milliseconds = (rest_seconds%1)*1000
-    rest_seconds=int(rest_seconds)
+    rest_milliseconds = int(rest_milliseconds)
 
-    rest_milliseconds=int(rest_milliseconds)
+    return (
+        ret
+        + np.timedelta64(rest_seconds, "s")
+        + np.timedelta64(rest_milliseconds, "ms")
+    )
 
-    return ret + np.timedelta64(rest_seconds,"s")+ np.timedelta64(rest_milliseconds,"ms")
 
+CONSTR_TYPE_UNDEFINED = 0
+CONSTR_TYPE_DELTATIME = 1
+CONSTR_TYPE_FLOAT = 2
 
-CONSTR_TYPE_UNDEFINED=0
-CONSTR_TYPE_DELTATIME=1
-CONSTR_TYPE_FLOAT=2
 
 class Chronicle:
     """Class for a chronicle pattern modeling
     -> enables to have partially defined chronicles
 
     Attributes
     ----------
-    sequence : [int|str]
-        a list of events.
-        It may work (without guarantee) with any event type equipped with an `__eq__()` operator.
-
-    tconst: {(np.timedelta64, np.timedelta64)}
-        a map assigning an temporal constraint (lower and upper bounds) of the delay
-        between the events in the key.
-        The delay is expressed in timedelta.
-        It is possible to define infinite intervals using `None` for one bound
-        (e.g. `(None, np.timedelta(56,'D'))` ). With discourage the use of `(None,None)` that
-        may reduce the algorithm efficiency compare to not have any constraints.
-
-    pid : int
-        chronicle identifier
-
-    inconsistent: bool
-        `True` is the chronicle is inconsistent and had a consistency check (through minimization)
-
-    Methods:
-    ---------
-
-    add_item(self, pos, item)
-        Add item at position pos. Replace the existing item if it exists
-
-    add_constraint(self, ei, ej, const)
-        Add a temporal constraint (couple) from event ei to ej
-
-    delete(self, pos)
-        remove the item at position pos
-
-    delete_constr(self, ei, ej)
-        destroy the constrains from ei to ej
+        sequence: [int|str]
+            a list of events representing a multiset.
+            It may work (without guarantee) with any event type equipped with an `__eq__()` operator.
+
+        tconst: {(int,int):(numpy.timedelta64, numpy.timedelta64)}
+            a map assigning an temporal constraint (lower and upper bounds) of the delay
+            between the events in the key.
+            The delay is expressed in timedelta.
+            It is possible to define infinite intervals using `None` for one bound
+            (e.g. `(None, numpy.timedelta(56,'D'))` ). With discourage the use of `(None,None)` that
+            may reduce the algorithm efficiency compare to not have any constraints.
 
-    clean(self)
-        destroy useless items and constraints (but does not remove all)
+        pid : int
+            chronicle identifier
 
-    minimize(self)
-        minimize the temporal constraints. It applies a Floyd-Warshall algorithm.
+        inconsistent: bool
+            `True` is the chronicle is inconsistent and had a consistency check (through minimization)
 
-    recognize(self, s)
-        return the list of all occurrences of the chronicle in the sequence s
+        constr_type: int
+            Specify the type of constrainted used
 
-    match(self,s)
-        return True whether their is at least one occurrence of the chronicle in
-        the sequence s, and false otherwise.
-        This function is faster than the recognize function
+    
     """
 
-    npat:int = 0
+    npat: int = 0
 
     def __init__(self):
-        """
-        """
+        """ """
 
-        self.tconst : Union(Mapping[Tuple[np.timedelta64,np.timedelta64]],Mapping[Tuple[float,float]]) ={}
-                        #temporal constraints,
-                        # keys: couple (ei,ej) where ei is a index in the item
-                        #   in the multiset
-                        # values: couple (lb,ub)
-
-        self.inconsistent:bool = False
-        self.name:str = ""
-        self.sequence:Mapping[int,str] = {}      # description of the pattern events
-        self.pid : int =Chronicle.npat   # pattern id
+        self.tconst: Union(
+            Mapping[Tuple[np.timedelta64, np.timedelta64]], Mapping[Tuple[float, float]]
+        ) = {}
+        # temporal constraints,
+        # keys: couple (ei,ej) where ei is a index in the item
+        #   in the multiset
+        # values: couple (lb,ub)
+
+        self.inconsistent: bool = False
+        self.name: str = ""
+        self.sequence: Mapping[
+            int, Union[str, int]
+        ] = {}  # description of the pattern events
+        self.pid: int = Chronicle.npat  # pattern id
         Chronicle.npat += 1
-        self.constr_type= CONSTR_TYPE_UNDEFINED
+        self.constr_type = CONSTR_TYPE_UNDEFINED
 
     def copy(self):
         C = Chronicle()
         C.inconsistent = self.inconsistent
-        if self.name!="":
-            C.name = self.name+"_copy"
+        if self.name != "":
+            C.name = self.name + "_copy"
         C.sequence = self.sequence.copy()
         C.tconst = self.tconst.copy()
         return C
 
-    def add_event(self, pos:int , event_query : str) -> None:
-        """Add an event to the chronicle multiset at a given position
-        An event is represented by an event query.
-        """
-        self.sequence[pos] = event_query
-
-    def add_constraint(self, ei:int, ej:int, constr: Union[Tuple[np.timedelta64, np.timedelta64],Tuple[float, float]]) -> None:
-        """Add a constraint-template to the chronicle pattern
-        - ei, ej : int
+    def add_event(self, pos: int, label: str) -> None:
+        """Add an event to the chronicle multiset at a given position.
+
+        An event is usually an item belonging to the vocabulary of the timed sequences or
+        it can also be a query when used in combinaison with dataframe.
+        For more details about labels as a query in the context of dataframe, see 
+
+        Parameters
+        ----------
+        pos: int
+            identifier of the event in the chronicle multiset
+        
+        label: str
+            The label of the event defines the nature of the event. Only string are possible.
+        """
+        self.sequence[pos] = label
+
+    def add_constraint(
+        self,
+        ei: int,
+        ej: int,
+        constr: Union[Tuple[np.timedelta64, np.timedelta64], Tuple[float, float]],
+    ) -> None:
+        """Add a temporal constraint (couple $[m,M]$) from event ei to ej
+
+        Parameters
+        ----------
+        ei, ej : int
             index of the events in the multiset
-        - constr: (np.timedelta64, np.timedelta64) or (float, float)
-            A couple representing the temporal constraint to add between ei and ej
+        constr: (np.timedelta64, np.timedelta64) or (float, float)
+            A couple representing the temporal constraint to add between `ei` and `ej`. 
+            The temporal constraints gives the minimum and the maximum delay between the
+            occurrences of the events.
 
-        ei and ej must be ordered (ei<ej) otherwise it is automatically
+        `ei` and `ej` are internally ordered (`ei<ej`). If not ordered, it is automatically
         reversed (with a reversed temporal constraint).
         If there is already a existing constraint between the two events, it is overrided.
         """
 
         if not type(constr) is tuple:
-            raise ValueError("error: constraint must be a tuple (=> constraint not added)")
-
-        if len(constr)!=2:
-            raise ValueError("error: constraint must have 2 values (=> constraint not added)")
-
-        if self.constr_type==CONSTR_TYPE_UNDEFINED:
-            if isinstance(constr[0],np.timedelta64):
-                self.constr_type=CONSTR_TYPE_DELTATIME
-            elif isinstance(constr[0],float):
-                self.constr_type=CONSTR_TYPE_FLOAT
+            raise ValueError(
+                "error: constraint must be a tuple (=> constraint not added)"
+            )
+
+        if len(constr) != 2:
+            raise ValueError(
+                "error: constraint must have 2 values (=> constraint not added)"
+            )
+
+        if self.constr_type == CONSTR_TYPE_UNDEFINED:
+            if isinstance(constr[0], np.timedelta64):
+                self.constr_type = CONSTR_TYPE_DELTATIME
+            elif isinstance(constr[0], float):
+                self.constr_type = CONSTR_TYPE_FLOAT
             else:
-                raise ValueError("error: expected type TimeDelta64 or float for temporal constraints (=> constraint not added)")
-
-        if self.constr_type==CONSTR_TYPE_DELTATIME and (not isinstance(constr[0],np.timedelta64) or not isinstance(constr[1],np.timedelta64)):
-            raise ValueError("error: expected type TimeDelta64 for temporal constraints (=> constraint not added)")
-
-        if self.constr_type==CONSTR_TYPE_FLOAT and (not isinstance(constr[0],float) or not isinstance(constr[1],float)):
-            raise ValueError("error: expected type Float for temporal constraints (=> constraint not added)")
-
-        if ei==ej:
-            raise ValueError("error: impossible to add the constraint with two identical events (=> constraint not added)")
-
-        if ej<ei:
-            ei,ej=ej,ei
-            constr = (-constr[1],-constr[0])
+                raise ValueError(
+                    "error: expected type TimeDelta64 or float for temporal constraints (=> constraint not added)"
+                )
+
+        if self.constr_type == CONSTR_TYPE_DELTATIME and (
+            not isinstance(constr[0], np.timedelta64)
+            or not isinstance(constr[1], np.timedelta64)
+        ):
+            raise ValueError(
+                "error: expected type TimeDelta64 for temporal constraints (=> constraint not added)"
+            )
+
+        if self.constr_type == CONSTR_TYPE_FLOAT and (
+            not isinstance(constr[0], float) or not isinstance(constr[1], float)
+        ):
+            raise ValueError(
+                "error: expected type Float for temporal constraints (=> constraint not added)"
+            )
+
+        if ei == ej:
+            raise ValueError(
+                "error: impossible to add the constraint with two identical events (=> constraint not added)"
+            )
+
+        if ej < ei:
+            ei, ej = ej, ei
+            constr = (-constr[1], -constr[0])
 
         try:
-            self.tconst[(ei,ej)] = constr
+            self.tconst[(ei, ej)] = constr
         except IndexError:
             raise IndexError("add_constraint: index_error (=> constraint not added)")
 
-    def __getitem__(self, i:Union[int, Tuple[int,int]] ) -> Union[str,Tuple[np.timedelta64, np.timedelta64],Tuple[float, float]]:
-        """return the item at position i in the multiset if i is an integer
-        and return the constraint between i[0] and i[1] if i is a couple
+    def __getitem__(
+        self, i: Union[int, Tuple[int, int]]
+    ) -> Union[str, Tuple[np.timedelta64, np.timedelta64], Tuple[float, float]]:
+        """
+        Function to redefine the behavior of the `[]`operator. 
+        This function has two different behaviors depending on its parameter. In case the 
+        parameter is an integer `i`, then it this integer designates an event and the operator
+        will returns the label of the i-th event of the chronicle.
+        In case the parameter is a couple of integers `(i,j)`, then it designed a constraint and it returns
+        the correspondong temporal constraints (if any).
+
+        Parameters
+        ----------
+        i: int or (int,int)
+            A position in the multiset, or (ei,ej): a pair of positions denoting a temporal constraints
+
+        Returns
+        -------
+            The item at position i in the multiset if i is an integer and return the
+            constraint between i[0] and i[1] if i is a couple
+
+        Example
+        ---------
+        .. code-block:: python
+
+            >>> c = Chronicle()
+            >>> c.add_event(0, "a")
+            >>> c.add_event(1, "b")
+            >>> c.add_event(2, "c")
+            >>> c.add_constraint(0, 1, (4.0, 10.0) )
+            >>> c.add_constraint(1, 2, (3.0,13.0) ) 
+            >>> c[2]
+            'c'
+            >>> c[(1,2)]
+            (3.0, 13.0)
+        
         """
         if not type(i) is tuple:
             return self.sequence[i]
         else:
             try:
-                return self.tconst[(min(i[0],i[1]),max(i[0],i[1]))]
+                return self.tconst[(min(i[0], i[1]), max(i[0], i[1]))]
             except KeyError:
                 return None
 
     def __len__(self) -> int:
-        """ Length of the patterns (number of items)
-        """
+        """Length of the patterns (number of items)"""
         if not self.sequence:
             return 0
-        return max(self.sequence.keys())+1
+        return max(self.sequence.keys()) + 1
 
     def __str__(self) -> str:
-        s = "C"+str(self.pid)+"\t {{["+ '],['.join([str(v) for k,v in self.sequence.items()]) + "]}}\n"
-        for k,v in self.tconst.items():
-            s += str(k[0]) + "," + str(k[1]) + ": " + str(v)+"\n"
+        """Default inline printing of a chronicle"""
+        s = (
+            "C"
+            + str(self.pid)
+            + "\t {{["
+            + "],[".join([str(v) for k, v in self.sequence.items()])
+            + "]}}\n"
+        )
+        for k, v in self.tconst.items():
+            s += str(k[0]) + "," + str(k[1]) + ": " + str(v) + "\n"
         return s
 
-    def delete(self, itempos : int) -> None:
-        self.sequence[ itempos ]=None
+    def delete(self, itempos: int) -> None:
+        """Remove all events at position pos.
+        The placeholder at position pos will still exists after deletion but the event is None.
+
+        Parameters
+        ----------
+        itempos : int
+            Position at which the event must be removed
+
+        Warning
+        --------
+        This function does not remove any temporal constraint.
+        """
+        self.sequence[itempos] = None
 
     def clean(self) -> None:
+        """Destroy useless items and constraints (but does not remove all)"""
         for itempos in list(self.sequence.keys()):
-            if self.sequence[ itempos ]==None:
-                del self.sequence[ itempos ]
+            if self.sequence[itempos] == None:
+                del self.sequence[itempos]
         posmax = max(self.sequence.keys())
         for p in list(self.tconst.keys()):
-            if p[0]>posmax or p[1]>posmax:
+            if p[0] > posmax or p[1] > posmax:
                 del self.tconst[p]
 
+    def delete_constr(self, ei: int, ej: int) -> None:
+        """Destroy the constrains from `ei` to `ej` (if any).
+        The user can ignore the order of the event indices.
 
-    def delete_constr(self, ei:int, ej:int) -> None:
+        Parameters
+        ----------
+        ei, ej: int
+            Indices of the events in the chronicle."""
         try:
-            del self.tconst[(ei,ej)]
+            del self.tconst[(min(ei, ej), max(ei, ej))]
         except KeyError:
             pass
 
     def minimize(self) -> None:
-        if self.constr_type==CONSTR_TYPE_UNDEFINED: 
-            #no constraint defined at all
-            self.constr_type=CONSTR_TYPE_FLOAT
-
-        #construction of distance graph
-        mat=np.matrix( np.zeros( (max(self.sequence.keys())+1,max(self.sequence.keys())+1) ))
-        for i in range(max(self.sequence.keys())+1):
-            for j in range(i+1,max(self.sequence.keys())+1):
-                if (i,j) in self.tconst:
-                    if self.constr_type==CONSTR_TYPE_DELTATIME:
-                        #Hack the division converts a time delta in a number of days (float)
-                        mat[i,j] = self.tconst[ (i,j) ][1]/np.timedelta64(1,'D')
-                        mat[j,i] = -self.tconst[ (i,j) ][0]/np.timedelta64(1,'D')
+        """Minimization of the temporal constraints. It transforms the set of temporal
+        constraints into the maximal _equivalent_ set of constraints.
+        **The recognition of minimized chronicles is often more efficient and equivalent to
+        the recognition of the initial chronicle.**
+
+        In case the set of temporal constraints are inconsistent, the flag `inconsistent`
+        is set to `True` and the function throws a warning.
+        In this case, the temporal constraints are not modified.
+        Note that inconsistent chronicles will not have any occurrences. It is the user
+        responsability to not prevent from attempting the recognition of such patterns.
+
+        In case the temporal constraints are expressed with `np.timedelta`, the temporal
+        constraints are first transformed in number of days. This may change the values
+        of all the temporal constraints.
+        The transformation is based on a Floyd-Warshall algorithm.
+
+        Example
+        -------
+        .. code-block:: python
+
+            >>> c = Chronicle()
+            >>> c.add_event(0, "a")
+            >>> c.add_event(1, "b")
+            >>> c.add_event(2, "c")
+            >>> c.add_constraint(0, 1, (4.0, 10.0) )
+            >>> c.add_constraint(1, 2, (3.0,13.0) ) 
+            >>> print(c)
+            C0       {{[a],[b],[c]}}
+            0,1: (4.0, 10.0)
+            1,2: (3.0, 13.0)
+            >>> c.minimize()
+            >>> print(c)
+            C0       {{[a],[b],[c]}}
+            0,1: (4.0, 10.0)
+            1,2: (3.0, 13.0)
+            0,2: (7.0, 23.0)
+        
+        """
+        if self.constr_type == CONSTR_TYPE_UNDEFINED:
+            # no constraint defined at all
+            self.constr_type = CONSTR_TYPE_FLOAT
+
+        # construction of distance graph
+        mat = np.matrix(
+            np.zeros((max(self.sequence.keys()) + 1, max(self.sequence.keys()) + 1))
+        )
+        for i in range(max(self.sequence.keys()) + 1):
+            for j in range(i + 1, max(self.sequence.keys()) + 1):
+                if (i, j) in self.tconst:
+                    if self.constr_type == CONSTR_TYPE_DELTATIME:
+                        # Hack the division converts a time delta in a number of days (float)
+                        mat[i, j] = self.tconst[(i, j)][1] / np.timedelta64(1, "D")
+                        mat[j, i] = -self.tconst[(i, j)][0] / np.timedelta64(1, "D")
                     else:
-                        mat[i,j] = self.tconst[ (i,j) ][1]
-                        mat[j,i] = -self.tconst[ (i,j) ][0]
+                        mat[i, j] = self.tconst[(i, j)][1]
+                        mat[j, i] = -self.tconst[(i, j)][0]
                 else:
-                    mat[i,j] = float("inf")
-                    mat[j,i] = -float("inf")
+                    mat[i, j] = float("inf")
+                    mat[j, i] = -float("inf")
         try:
-            matfw = scipy.sparse.csgraph.floyd_warshall( mat )
-            #construction of simplified chronicle
-            for i in range(max(self.sequence.keys())+1):
-                for j in range(i+1,max(self.sequence.keys())+1):
-                    if matfw[j,i]!=float('inf') or matfw[i,j]!=float('inf'):
-                        if self.constr_type==CONSTR_TYPE_DELTATIME:
-                            self.tconst[ (i,j) ] = (
-                                days_to_timedelta64(-matfw[j,i]) if matfw[j,i]!=-float('inf') else None,
-                                days_to_timedelta64(matfw[i,j]) if matfw[i,j]!=float('inf') else None )
+            matfw = scipy.sparse.csgraph.floyd_warshall(mat)
+            # construction of simplified chronicle
+            for i in range(max(self.sequence.keys()) + 1):
+                for j in range(i + 1, max(self.sequence.keys()) + 1):
+                    if matfw[j, i] != float("inf") or matfw[i, j] != float("inf"):
+                        if self.constr_type == CONSTR_TYPE_DELTATIME:
+                            self.tconst[(i, j)] = (
+                                days_to_timedelta64(-matfw[j, i])
+                                if matfw[j, i] != -float("inf")
+                                else None,
+                                days_to_timedelta64(matfw[i, j])
+                                if matfw[i, j] != float("inf")
+                                else None,
+                            )
                         else:
-                            self.tconst[ (i,j) ] = (
-                                -matfw[j,i] if matfw[j,i]!=-float('inf') else None,
-                                matfw[i,j] if matfw[i,j]!=float('inf') else None )
+                            self.tconst[(i, j)] = (
+                                -matfw[j, i] if matfw[j, i] != -float("inf") else None,
+                                matfw[i, j] if matfw[i, j] != float("inf") else None,
+                            )
         except scipy.sparse.csgraph._shortest_path.NegativeCycleError:
             warnings.warn("*** Minimisation: Inconsistent chronicle ***")
             self.inconsistent = True
-    ################
-
 
     ################ All occurrences exact recognition #####################
-    
-    def __complete_recognition__(self,
-                                 occurrence: Union[Sequence[np.datetime64],Sequence[float]],
-                                 gamma: Sequence[int],
-                                 kr: int,
-                                 df_seq: TimedSequence) -> Union[Sequence[ Sequence[ Tuple[np.datetime64,np.datetime64] ] ], Sequence[ Sequence[ Tuple[float,float] ] ]]:
-        """
 
+    def __complete_recognition__(
+        self,
+        occurrence: Union[Sequence[np.datetime64], Sequence[float]],
+        gamma: Sequence[int],
+        kr: int,
+        df_seq: TimedSequence,
+    ) -> Union[
+        Sequence[Sequence[Tuple[np.datetime64, np.datetime64]]],
+        Sequence[Sequence[Tuple[float, float]]],
+    ]:
+        """
 
         Parameters
         ----------
         occurrence : Union[ Sequence[int], Sequence[datetime] ]
             Current occurrence to complete.
         gamma : list[int]
             Order of the exploration of the chronicle items
@@ -315,62 +539,93 @@
 
         Returns
         -------
         Sequence[ Sequence[ Tuple[datetime,datetime] ] ]
             return a list of occurrences that add the description of the matching
             of the kr-th item of the chronicle to the occurrence
 
+        :meta private:
         """
 
-        item_index : int = gamma[kr]
+        item_index: int = gamma[kr]
 
-        if not item_index in self.sequence: #end of chronicle multiset -> end of recursion
+        if (
+            not item_index in self.sequence
+        ):  # end of chronicle multiset -> end of recursion
             return [occurrence]
 
-        itemquery = self.sequence[ item_index ] #item of the chronicle
+        itemquery = self.sequence[item_index]  # item of the chronicle
 
-        occurrences:Union[Sequence[ Sequence[ Tuple[np.datetime64,np.datetime64] ] ], Sequence[ Sequence[ Tuple[float,float] ] ]] = []
-
-        df_select = df_seq[ (df_seq >= occurrence[item_index][0]) &
-                            (df_seq<=occurrence[item_index][1]) ]
+        occurrences: Union[
+            Sequence[Sequence[Tuple[np.datetime64, np.datetime64]]],
+            Sequence[Sequence[Tuple[float, float]]],
+        ] = []
+
+        df_select = df_seq[
+            (df_seq >= occurrence[item_index][0])
+            & (df_seq <= occurrence[item_index][1])
+        ]
         for p in df_select[df_select == itemquery]._dates:
-            #create a new occurrence to be modified
+            # create a new occurrence to be modified
             new_occ = occurrence[:]
-            new_occ[item_index] = (p,p)
+            new_occ[item_index] = (p, p)
 
-            satisfiable=True
-            #propagate chronicle constraints to events that has not yet been explored
-            for k,v in self.tconst.items():
-                if (k[0]==item_index) and\
-                         (k[1] in self.sequence) and\
-                         not (k[1] in gamma[:kr]):
-                    new_occ[ k[1] ] = (max(new_occ[ k[1] ][0], p+v[0] if v[0] is not None else -maxdate),\
-                                        min(new_occ[ k[1] ][1], p+v[1] if v[1] is not None else maxdate))
-                    if new_occ[ k[1] ][0]>new_occ[ k[1] ][1]:
-                        #if empty interval, it is not satisfiable
-                        satisfiable=False
+            satisfiable = True
+            # propagate chronicle constraints to events that has not yet been explored
+            for k, v in self.tconst.items():
+                if (
+                    (k[0] == item_index)
+                    and (k[1] in self.sequence)
+                    and not (k[1] in gamma[:kr])
+                ):
+                    new_occ[k[1]] = (
+                        max(
+                            new_occ[k[1]][0], p + v[0] if v[0] is not None else -maxdate
+                        ),
+                        min(
+                            new_occ[k[1]][1], p + v[1] if v[1] is not None else maxdate
+                        ),
+                    )
+                    if new_occ[k[1]][0] > new_occ[k[1]][1]:
+                        # if empty interval, it is not satisfiable
+                        satisfiable = False
                         break
-                elif (k[1]==item_index) and (k[0] in self.sequence) and \
-                        not (k[0] in gamma[:kr]):
-                    new_occ[ k[0] ] = (max(new_occ[ k[0] ][0], p-v[1] if v[1] is not None else -maxdate), \
-                                        min(new_occ[ k[0] ][1], p-v[0]  if v[0] is not None else maxdate))
-                    if new_occ[ k[0] ][0]>new_occ[ k[0] ][1]:
-                        #if empty interval, it is not satisfiable
-                        satisfiable=False
+                elif (
+                    (k[1] == item_index)
+                    and (k[0] in self.sequence)
+                    and not (k[0] in gamma[:kr])
+                ):
+                    new_occ[k[0]] = (
+                        max(
+                            new_occ[k[0]][0], p - v[1] if v[1] is not None else -maxdate
+                        ),
+                        min(
+                            new_occ[k[0]][1], p - v[0] if v[0] is not None else maxdate
+                        ),
+                    )
+                    if new_occ[k[0]][0] > new_occ[k[0]][1]:
+                        # if empty interval, it is not satisfiable
+                        satisfiable = False
                         break
 
             if satisfiable:
-                #add the occurrence to the list
-                occurrences.append( new_occ )
+                # add the occurrence to the list
+                occurrences.append(new_occ)
         return occurrences
 
-    def __recrecognize__(self, occurrence: Union[Sequence[np.datetime64],Sequence[float]],
-                         gamma: Sequence[int],
-                         kr: int,
-                         df_seq: TimedSequence) -> Union[Sequence[ Sequence[ Tuple[np.datetime64,np.datetime64] ] ],Sequence[ Sequence[ Tuple[float,float] ] ]] :
+    def __recrecognize__(
+        self,
+        occurrence: Union[Sequence[np.datetime64], Sequence[float]],
+        gamma: Sequence[int],
+        kr: int,
+        df_seq: TimedSequence,
+    ) -> Union[
+        Sequence[Sequence[Tuple[np.datetime64, np.datetime64]]],
+        Sequence[Sequence[Tuple[float, float]]],
+    ]:
         """
         Recursive call for occurrence recognition
 
         Parameters
         ----------
         occurrence : [ (p_1,q_1), (p_2,q_2) ...] (list of $n$ couples of position, where $n$ is
             the chronicle size)
@@ -386,264 +641,405 @@
         Returns
         -------
         [ [ (p_1,p_1), (p_2,p_2) ...], [ (p_1,p_1), (p_2,p_2) ...], ...]  (list of lists of
             couples, each list is an occurrence. It contains a list of n couples, where n is
             the chronicle size)
             Returns a list of occurrences recognized from the last_item_index of the chronicle
             until its last item
+            
+        :meta private:
         """
 
-        chro_size=max( self.sequence )+1 #max of the key values
-        if kr==chro_size: # final case
+        chro_size = max(self.sequence) + 1  # max of the key values
+        if kr == chro_size:  # final case
             return [occurrence]
 
         index = gamma[kr]
-        if index==-1: #next item not found
+        if index == -1:  # next item not found
             return []
         occurrences = []
         loc_occs = self.__complete_recognition__(occurrence, gamma, kr, df_seq)
         for occ in loc_occs:
-            reoccs= self.__recrecognize__(occ, gamma, kr+1, df_seq)
+            reoccs = self.__recrecognize__(occ, gamma, kr + 1, df_seq)
             occurrences.extend(reoccs)
         return occurrences
 
-    def recognize(self, df_seq: TimedSequence) -> Union[Sequence[ Sequence[np.datetime64] ],Sequence[ Sequence[ float ] ]] :
+    def recognize(
+        self, df_seq: TimedSequence
+    ) -> Union[Sequence[Sequence[np.datetime64]], Sequence[Sequence[float]]]:
         """
         Enumerates the chronicle occurrences in a sequence.
 
         Parameters
         ----------
-        df_seqs : [ (l,t), ... ], [l,...]
+        df_seqs: `[ (l,t), ... ], [l,...]`
             Description of a temporal sequence of events.
 
             In a sequence the timestamps are datetime.
 
         Returns
         -------
-        [ [ p_1, p_2 ...], [ p_1, p_2 ...], ...]  (list of lists of positions/datetimes, each
+        `[ [ p_1, p_2 ...], [ p_1, p_2 ...], ...]`  (list of lists of positions/datetimes, each
             list is an occurrence. It contains a list of n couples, where n is the chronicle size)
             Return a list of occurrences of the chronicle in the sequences
         """
         if not isinstance(df_seq, TimedSequence):
             raise ValueError("recognize function expects a TimedSequence as input.")
-        if self.constr_type!=CONSTR_TYPE_UNDEFINED and df_seq.dtype!=self.constr_type:
-            raise ValueError("TimedSequence temporal indexing must be coherent with chronicle temporal constraints")
-
-        occurrences : Union[Sequence[ Sequence[np.datetime64] ],Sequence[ Sequence[float] ]] = [] #list of occurrences
+        if (
+            self.constr_type != CONSTR_TYPE_UNDEFINED
+            and df_seq.dtype != self.constr_type
+        ):
+            raise ValueError(
+                "TimedSequence temporal indexing must be coherent with chronicle temporal constraints"
+            )
+
+        occurrences: Union[
+            Sequence[Sequence[np.datetime64]], Sequence[Sequence[float]]
+        ] = []  # list of occurrences
 
-        chro_size=max( self.sequence )+1
-        if chro_size==0 :
+        chro_size = max(self.sequence) + 1
+        if chro_size == 0:
             return occurrences
 
         k = 0
-        gamma = [ p for p in range(df_seq.len()) ]
-        item_index : int = gamma[0]
-        itemquery : str = self.sequence[item_index]
-
+        gamma = [p for p in range(df_seq.len())]
+        item_index: int = gamma[0]
+        itemquery: Union[str, int] = self.sequence[item_index]
 
         for p in df_seq[df_seq == itemquery]._dates:
-
             # create a new occurrence
             new_occ = []
-            resize(new_occ, chro_size, (df_seq.start(),df_seq.end()) )
-            new_occ[item_index] = (p,p)
+            resize(new_occ, chro_size, (df_seq.start(), df_seq.end()))
+            new_occ[item_index] = (p, p)
 
             # propagate chronicle constraints
-            for k,v in self.tconst.items():
-                if (k[0]==item_index) and (k[1] in self.sequence):
-                    new_occ[ k[1] ]= (max(df_seq.start(),p+v[0] if v[0] is not None else -maxdate),
-                                        min(p+v[1] if v[1] is not None else maxdate, df_seq.end()))
-                elif (k[1]==item_index) and (k[0] in self.sequence):
-                    new_occ[ k[0] ]= (max(df_seq.start(),p-v[1] if v[1] is not None else -maxdate),
-                                        min(p-v[0] if v[0] is not None else maxdate, df_seq.end()))
+            for k, v in self.tconst.items():
+                if (k[0] == item_index) and (k[1] in self.sequence):
+                    new_occ[k[1]] = (
+                        max(df_seq.start(), p + v[0] if v[0] is not None else -maxdate),
+                        min(p + v[1] if v[1] is not None else maxdate, df_seq.end()),
+                    )
+                elif (k[1] == item_index) and (k[0] in self.sequence):
+                    new_occ[k[0]] = (
+                        max(df_seq.start(), p - v[1] if v[1] is not None else -maxdate),
+                        min(p - v[0] if v[0] is not None else maxdate, df_seq.end()),
+                    )
 
             # add the occurrence at he end of the occurrences list
             loc_occ = self.__recrecognize__(new_occ, gamma, 1, df_seq)
-            occurrences.extend( loc_occ )
+            occurrences.extend(loc_occ)
 
         ## we return occurrences as a list of list of positions (and we remove the couples, min/max)
-        return [ [e[0] for e in occ] for occ in occurrences]
-
-
+        return [[e[0] for e in occ] for occ in occurrences]
 
     ##################  presence/absence exact detection ###############
 
     def match(self, df_seq: TimedSequence) -> bool:
         """
-        :df_seq : Time series representing a sequence of events with datetime index
+        This function varify whether there is at least one occurrence of the chronicle in
+        the sequence `df_seq`. 
+        
+        This function is in average faster than the recognize function, because it early stopped 
+        as soon as a valid occurrence is found.
 
-        Return true is the chronicle occurs in the sequence
+        Parameters
+        ----------
+        df_seq: Timed sequence representing a sequence of events
+
+        Returns
+        -------
+        bool
+            `True` if the chronicle occurs in the sequence and `False` otherwise
         """
 
         if not isinstance(df_seq, TimedSequence):
             raise ValueError("match function expects a TimedSequence as input.")
 
-        if self.constr_type!=CONSTR_TYPE_UNDEFINED and df_seq.dtype!=self.constr_type:
-            raise ValueError("TimedSequence temporal indexing must be coherent with chronicle temporal constraints")
+        if (
+            self.constr_type != CONSTR_TYPE_UNDEFINED
+            and df_seq.dtype != self.constr_type
+        ):
+            raise ValueError(
+                "TimedSequence temporal indexing must be coherent with chronicle temporal constraints"
+            )
 
-        if len(self.sequence)==0:
+        if len(self.sequence) == 0:
             return False
 
-        chro_size=max( self.sequence.keys() )+1
-        if chro_size==0 :
+        chro_size = max(self.sequence.keys()) + 1
+        if chro_size == 0:
             return False
 
         item_index = 0
         try:
-            item=self.sequence[item_index]
+            item = self.sequence[item_index]
         except KeyError:
             raise Exception("index out of chronicle events list")
 
-        #select all elements that match the item
-        for p in df_seq[ df_seq==item ]._dates:
+        # select all elements that match the item
+        for p in df_seq[df_seq == item]._dates:
             new_occ = []
-            resize(new_occ, chro_size, (df_seq.start(),df_seq.end()))
+            resize(new_occ, chro_size, (df_seq.start(), df_seq.end()))
 
-            new_occ[item_index] = (p,p)
-            #propagate chronicle constraints
+            new_occ[item_index] = (p, p)
+            # propagate chronicle constraints
             for k in self.tconst:
                 v = self.tconst[k]
-                if (k[0]==item_index) and (k[1] in self.sequence):
-                    new_occ[ k[1] ] = (max(df_seq.start(),p+v[0]), min(p+v[1],df_seq.end()))
+                if (k[0] == item_index) and (k[1] in self.sequence):
+                    new_occ[k[1]] = (
+                        max(df_seq.start(), p + v[0]),
+                        min(p + v[1], df_seq.end()),
+                    )
 
-            #ajouter l'occurrence à la liste des occurrences
+            # ajouter l'occurrence à la liste des occurrences
             if self.__is_recrecognize__(new_occ, item_index, df_seq):
                 return True
         return False
 
-    def __is_recrecognize__(self, occurrence: Union[Sequence[ Tuple[np.datetime64,np.datetime64] ],Sequence[ Tuple[float,float] ]],
-                            last_item_index: int,
-                            sequence: TimedSequence) -> bool:
-        """
-        recursive call for occurrence recognition
-        return True is the events from the last_item_index of the chronicle until
-        its last item have been recognized or not
+    def __is_recrecognize__(
+        self,
+        occurrence: Union[
+            Sequence[Tuple[np.datetime64, np.datetime64]], Sequence[Tuple[float, float]]
+        ],
+        last_item_index: int,
+        sequence: TimedSequence,
+    ) -> bool:
+        """
+        Recursive call for occurrence recognition
+
+        Return
+            True if the events from the last_item_index of the chronicle until
+            its last item have been recognized or not
         """
-        chro_size=max( self.sequence )
-        if last_item_index==chro_size:
+        chro_size = max(self.sequence)
+        if last_item_index == chro_size:
             return True
 
-        item_index=last_item_index+1
+        item_index = last_item_index + 1
 
         occ = self.__is_complete_recognition__(occurrence, item_index, sequence)
-        if ( not (occ is None) ) and \
-                self. __is_recrecognize__(occ, item_index, sequence):
+        if (not (occ is None)) and self.__is_recrecognize__(occ, item_index, sequence):
             return True
         return False
 
-    def __is_complete_recognition__(self,
-                                    occurrence: Union[Sequence[ Tuple[np.datetime64,np.datetime64] ],Sequence[ Tuple[float,float] ]],
-                                    item_index: int,
-                                    df_seq:TimedSequence) -> Union[None, Sequence[ Sequence[ Tuple[np.datetime64,np.datetime64] ] ], Sequence[ Sequence[ Tuple[float,float] ] ] ]:
+    def __is_complete_recognition__(
+        self,
+        occurrence: Union[
+            Sequence[Tuple[np.datetime64, np.datetime64]], Sequence[Tuple[float, float]]
+        ],
+        item_index: int,
+        df_seq: TimedSequence,
+    ) -> Union[
+        None,
+        Sequence[Sequence[Tuple[np.datetime64, np.datetime64]]],
+        Sequence[Sequence[Tuple[float, float]]],
+    ]:
         """
-        return a list of occurrences that add the description of the matching of the
-        item_index-th item of the chronicle to the occurrence
+
+        Return
+        -------
+            Returns a list of occurrences that add the description of the matching of the
+            item_index-th item of the chronicle to the occurrence
         """
 
-        if not item_index in self.sequence: #end of chronicle multiset -> end of recursion
+        if (
+            not item_index in self.sequence
+        ):  # end of chronicle multiset -> end of recursion
             return occurrence
 
-        itemquery=self.sequence[item_index] #get the query that is to check
+        itemquery = self.sequence[item_index]  # get the query that is to check
 
-        if occurrence[item_index][0]==occurrence[item_index][1]:
+        if occurrence[item_index][0] == occurrence[item_index][1]:
             # Only one time instant is possible, to return an occurrence we check whether
             #   -> the time instant is before the end of the last event! (HACK: strictly??), or
             #   -> there is at least one even that satisfy the item's query at that time instant
             # Otherwise, it is a deadlock
-            if occurrence[item_index][0]<df_seq.end() and \
-                    (itemquery in df_seq.at( occurrence[item_index][0] ) ):
+            if occurrence[item_index][0] < df_seq.end() and (
+                itemquery in df_seq.at(occurrence[item_index][0])
+            ):
                 return occurrence
             else:
                 return None
 
-        df_select = df_seq[ (df_seq>=occurrence[item_index][0]) &
-                            (df_seq<=occurrence[item_index][1])]
-        for p in df_select[ df_select==itemquery ]._dates:
+        df_select = df_seq[
+            (df_seq >= occurrence[item_index][0])
+            & (df_seq <= occurrence[item_index][1])
+        ]
+        for p in df_select[df_select == itemquery]._dates:
             new_occ = occurrence[:]
-            new_occ[item_index] = (p,p)
+            new_occ[item_index] = (p, p)
 
-            satisfiable=True
-            #propagate chronicle constraints
+            satisfiable = True
+            # propagate chronicle constraints
             for k in self.tconst:
                 v = self.tconst[k]
-                if (k[0]==item_index) and (k[1] in self.sequence):
-                    new_occ[ k[1] ] = (max(new_occ[ k[1] ][0], p+v[0]),
-                                        min(new_occ[ k[1] ][1], p+v[1]))
-                    if new_occ[ k[1] ][0]>new_occ[ k[1] ][1]:
-                        #if empty interval, it is not satisfiable
-                        satisfiable=False
+                if (k[0] == item_index) and (k[1] in self.sequence):
+                    new_occ[k[1]] = (
+                        max(new_occ[k[1]][0], p + v[0]),
+                        min(new_occ[k[1]][1], p + v[1]),
+                    )
+                    if new_occ[k[1]][0] > new_occ[k[1]][1]:
+                        # if empty interval, it is not satisfiable
+                        satisfiable = False
                         break
 
             if satisfiable:
-                #add the occurrence to the list
+                # add the occurrence to the list
                 return new_occ
 
         return None
 
+    def draw(self, ax=None) -> None:
+        """
+        Function to draw a chronicle in a matplotlib figure. This function is based on the 
+        graph drawing capabilities of NetworkX library.
+
+        Parameters
+        ----------
+        ax: Matplotlib Axes object, optional. 
+            When specified, the function draws the graph in the specified Matplotlib axes.
+
+        Warning
+        ----------
+        This functions requires to install networkx and matplotlib. These two librairies are 
+        not in the requirements and must be installed manually by the user to makes work this function.
+
+        Example
+        ----------
+        .. code-block:: python
+
+            import matplotlib.pyplot as plt
+
+            c = Chronicle()
+            c.add_event(0, "a")
+            c.add_event(1, "b")
+            c.add_event(2, "c")
+            c.add_constraint(0, 1, (np.timedelta64(4, "D"), np.timedelta64(10, "D")))
+            c.add_constraint(0, 2, (np.timedelta64(2, "D"), np.timedelta64(8, "D")))
+            c.add_constraint(1, 2, (np.timedelta64(3, "D"), np.timedelta64(13, "D")))
+
+            c.draw()
+
+            plt.show()
+        
+        """
+        try:
+            import networkx as nx
+            import matplotlib.pyplot as plt
+        except:
+            warnings.warn(
+                "drawing chronicles requires to install `networkx` and `matplotlib` libraries."
+            )
+            return
+
+        G = nx.DiGraph()
+        G.add_nodes_from(range(self.__len__()))
+        for k in self.tconst:
+            v = self.tconst[k]
+            G.add_edge(k[0], k[1])
+            G[k[0]][k[1]]["I"] = v
+
+        pos = nx.spring_layout(G)
+        lbl = nx.draw(
+            G, ax=ax, pos=pos, labels=self.sequence, with_labels=True, font_weight="bold"
+        )
+        lbl = nx.draw_networkx_edges(G, ax=ax, pos=pos, arrows=True)
+        lbl = nx.draw_networkx_edge_labels(
+            G,
+            ax=ax, 
+            pos=pos,
+            edge_labels={
+                (u, v): f"[{d['I'][0]},{d['I'][1]}]"
+                for u, v, d in G.edges(data=True)
+            },
+            font_color="red",
+        )
+
 
 if __name__ == "__main__":
     #################################
-    #Example of sequence
-    seq = [('a',1),('c',2),('b',3),('a',8),('a',10),('b',12),('a',15),('c',17),
-            ('b',20),('c',23),('c',25),('b',26),('c',28),('b',30)]
-
-    dates = np.array([np.datetime64('1970-01-01') + np.timedelta64(e[1],'D') for e in seq],
-                        dtype='datetime64')
+    # Example of sequence
+    seq = [
+        ("a", 1),
+        ("c", 2),
+        ("b", 3),
+        ("a", 8),
+        ("a", 10),
+        ("b", 12),
+        ("a", 15),
+        ("c", 17),
+        ("b", 20),
+        ("c", 23),
+        ("c", 25),
+        ("b", 26),
+        ("c", 28),
+        ("b", 30),
+    ]
+
+    dates = np.array(
+        [np.datetime64("1970-01-01") + np.timedelta64(e[1], "D") for e in seq],
+        dtype="datetime64",
+    )
     data = np.array([e[0] for e in seq])
 
     ts = TimedSequence(dates, data)
 
-    c=Chronicle()
-    c.add_event(0,'a')
-    c.add_event(1,'b')
-    c.add_event(2,'c')
-    c.add_constraint(0,1, (np.timedelta64(4,'D'),np.timedelta64(10,'D')))
-    c.add_constraint(0,2, (np.timedelta64(2,'D'),np.timedelta64(8,'D')))
-    c.add_constraint(1,2, (np.timedelta64(3,'D'),np.timedelta64(13,'D')))
+    c = Chronicle()
+    c.add_event(0, "a")
+    c.add_event(1, "b")
+    c.add_event(2, "c")
+    c.add_constraint(0, 1, (np.timedelta64(4, "D"), np.timedelta64(10, "D")))
+    c.add_constraint(0, 2, (np.timedelta64(2, "D"), np.timedelta64(8, "D")))
+    c.add_constraint(1, 2, (np.timedelta64(3, "D"), np.timedelta64(13, "D")))
+    
+    try:
+        import matplotlib.pyplot as plt
+        c.draw()
+        plt.show()
+    except:
+        pass
 
     print(c)
     c.minimize()
     print(c)
 
-    reco=c.match(ts)
+    reco = c.match(ts)
     print(f"Reconnaissance de la chronique: [{reco}]!")
 
-    reco=c.recognize(ts)
+    reco = c.recognize(ts)
     print(f"Reconnaissance de la chronique: [{reco}]!")
 
-
     print(c)
-    c2=c.copy()
-    c2.add_constraint(0, 2, (np.timedelta64(4,'D'),np.timedelta64(4,'D')))
+    c2 = c.copy()
+    c2.add_constraint(0, 2, (np.timedelta64(4, "D"), np.timedelta64(4, "D")))
     print(c)
 
     #################################
     # Sequence with floats
 
-    dates = np.array([float(e[1]) for e in seq], dtype='float')
+    dates = np.array([float(e[1]) for e in seq], dtype="float")
     data = np.array([e[0] for e in seq])
 
     ts = TimedSequence(dates, data)
 
-    c=Chronicle()
-    c.add_event(0,'a')
-    c.add_event(1,'b')
-    c.add_event(2,'c')
-    c.add_constraint(0,1, (4.0,10.0))
-    c.add_constraint(0,2, (2.0,8.0))
-    c.add_constraint(1,2, (3.0,13.0))
+    c = Chronicle()
+    c.add_event(0, "a")
+    c.add_event(1, "b")
+    c.add_event(2, "c")
+    c.add_constraint(0, 1, (4.0, 10.0))
+    c.add_constraint(0, 2, (2.0, 8.0))
+    c.add_constraint(1, 2, (3.0, 13.0))
 
     print(c)
     c.minimize()
     print(c)
 
-    reco=c.match(ts)
+    reco = c.match(ts)
     print(f"Reconnaissance de la chronique: [{reco}]!")
 
-    reco=c.recognize(ts)
+    reco = c.recognize(ts)
     print(f"Reconnaissance de la chronique: [{reco}]!")
 
-
     print(c)
-    c2=c.copy()
-    c2.add_constraint(0, 2, (np.timedelta64(4,'D'),np.timedelta64(4,'D')))
+    c2 = c.copy()
+    c2.add_constraint(0, 2, (np.timedelta64(4, "D"), np.timedelta64(4, "D")))
     print(c)
```

### Comparing `pychronicles-0.0.9/pychronicles/fchronicle.py` & `pychronicles-0.1.0/pychronicles/fchronicle.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,190 +1,256 @@
 #!/bin/python3
 # -*- coding: utf-8 -*-
 """
-Fuzzy chronicle with pure NumPy implementation
+Module that implements the notion of fuzzy chronicle. A fuzzy chronicle is an extension of 
+a chronicle that provides the possibility to make approximated matching. 
+Instead of having strict temporal constraint (satisfied or not), the temporal constraint 
+satistifaction is fuzzyfied.
 
-@author: Thomas Guyet
-@date: 10/2022
-@institution: Inria
+The set of event is not fuzzyfied ... and the recognition of a chronicle in a sequence continues
+to require the occurrence of all its events.
+
+The recognition function (denoted `cmp`) has two parameters:
+* the lambda parameter specificies the level of fuzzyness of temporal constraints. This level of 
+fuzzyness it used to evaluate the similarity measure between a subsequence and the chronicle.
+* the threshold parameter specifies the similarity threshold to decide whether the chronicle is considered 
+to occur or not.
+
+More details about the recognition of fuzzy chronicles can be found in the following article
+
+Example
+--------
+
+The following example illustrates the main functionalities of the `TimeSequence` class.
+
+.. code-block:: python
+
+    ts = TimedSequence(dates, data)
+
+    c = FuzzyChronicle()
+    c.add_event(0, "b")
+    c.add_event(1, "a")
+    c.add_event(2, "c")
+    c.add_constraint(0, 1, (np.timedelta64(13, "D"), np.timedelta64(17, "D")))
+    c.add_constraint(0, 2, (np.timedelta64(1, "D"), np.timedelta64(30, "D")))
+    c.minimize()
+    c.tunit = "D" # this line is required to specify the default temporal unit 
+    print(c)
+
+    occ, sim = c.cmp(ts, 0.95, 0.3)
+    print("similarity:" + str(sim))
+    print("occurrence:" + str(occ))
+
+:Authors:
+    Thomas Guyet, Inria
+:Date:
+    08/2023
 """
 
 import numpy as np
 
 ## typing features
-from typing import TypeVar, Union, Dict, Mapping,Tuple, Sequence, Any
+from typing import TypeVar, Union, Dict, Mapping, Tuple, Sequence, Any
 from pychronicles.timedsequence import TimedSequence
 from pychronicles.chronicle import Chronicle, resize
 
-#definition of a data frame type
-FuzzyChronicle = TypeVar('pychronicles.fchronicle.FuzzyChronicle')
+# definition of a data frame type
+FuzzyChronicle = TypeVar("pychronicles.fchronicle.FuzzyChronicle")
 ###
 
+
 class FuzzyChronicle(Chronicle):
     """Class for a fuzzy chronicle pattern modeling
     Enable efficient recognition of chronicles with approximated intervals.
 
     The ̀`match` and `recognize` functions still work with the semantics of
     classical chronicles.
-
-    Attributes
-    ----------
-
-    Methods:
-    ---------
-
-    cmp(self, s, threshold, lambda)
-        return a list of occurrences with their respective similarity.
     """
 
-    npat:int = 0
+    npat: int = 0
 
     def __init__(self):
-        """
-        """
+        """ """
         super().__init__()
 
-        self.interval_extension : np.timedelta64 = 0 #similarity parameter
-        self.sim_max : float = 0 #internal global variable
-        self.min_reco_sim : float = 1 #minimal similarity value to recognize a chronicle
-        self.lbda : float = 1
-        self.tunit : str ='D'
-
-    def __interval_sim(self,
-                       pos: np.timedelta64,
-                       interval: Tuple[np.timedelta64,np.timedelta64]) -> float:
+        self.interval_extension: np.timedelta64 = 0  # similarity parameter
+        self.sim_max: float = 0  # internal global variable
+        self.min_reco_sim: float = (
+            1  # minimal similarity value to recognize a chronicle
+        )
+        self.lbda: float = 1
+        self.tunit: str = "D"
+
+    def __interval_sim(
+        self, pos: np.timedelta64, interval: Tuple[np.timedelta64, np.timedelta64]
+    ) -> float:
         """
 
         Parameters
         ----------
         pos : np.timedelta64
             DESCRIPTION.
         interval : (np.timedelta64, np.timedelta64)
             Extended interval for chronicle occurrence search with flexible
 
         Returns
         -------
         float
             similarity between a position and an interval.
+
+        :meta private:
         """
 
         # in case it is timedelta types (when datetimes are used), then
         # interval and pos are Timedelta
         # then, interval and pos are transformed in tunits to compute the similarity
         if pos >= interval[0] and pos <= interval[1]:
             return 1
         else:
-            return np.exp(-self.lbda * min( np.abs(interval[0]-pos), np.abs(interval[1]-pos) )/np.timedelta64(1,self.tunit))
-
-
-    def __complete_similarity__(self,
-                                occurrence:Sequence[ Tuple[np.timedelta64,np.timedelta64] ],
-                                cursim : float,
-                                item_index : int,
-                                df_seq: TimedSequence) -> Tuple[ Sequence[ Sequence[ Tuple[np.timedelta64,np.timedelta64] ] ], Sequence[float] ] :
+            return np.exp(
+                -self.lbda
+                * min(np.abs(interval[0] - pos), np.abs(interval[1] - pos))
+                / np.timedelta64(1, self.tunit)
+            )
+
+    def __complete_similarity__(
+        self,
+        occurrence: Sequence[Tuple[np.timedelta64, np.timedelta64]],
+        cursim: float,
+        item_index: int,
+        df_seq: TimedSequence,
+    ) -> Tuple[
+        Sequence[Sequence[Tuple[np.timedelta64, np.timedelta64]]], Sequence[float]
+    ]:
         """
-        :occurrence: [(np.timedelta64,np.timedelta64)]
-            list of position's intervals corresponding to admissible location
-            of the item_index's event in the sequence
-            partial occurrence of the chronicle from item 0 to item_index-1
-        :cursim: double
-            partial similarity measure of the chronicle
-        :df_seq: TimedSequence
-            timed sequence
-        return ...
+        Parameters
+        ----------
+            occurrence: [(np.timedelta64,np.timedelta64)]
+                list of position's intervals corresponding to admissible location
+                of the item_index's event in the sequence
+                partial occurrence of the chronicle from item 0 to item_index-1
+            cursim: double
+                partial similarity measure of the chronicle
+            df_seq: TimedSequence
+                timed sequence
+        Returns
+        -------
+            occurrences: a list of admissible locations specifying the exact location of the first `item_index`-th items
+            sims: a list of the similarity for each of the adminissible locations
+
+        :meta private:
         """
 
-        if not item_index in self.sequence: #end of chronicle multiset -> end of recursion
+        if (
+            not item_index in self.sequence
+        ):  # end of chronicle multiset -> end of recursion
             return [occurrence], [cursim]
 
-        item=self.sequence[item_index]
+        item = self.sequence[item_index]
 
-        if occurrence[item_index][0]==occurrence[item_index][1]:
-            if occurrence[item_index][0]<df_seq.end() and \
-                (item in df_seq.at( occurrence[item_index][0] )):
+        if occurrence[item_index][0] == occurrence[item_index][1]:
+            if occurrence[item_index][0] < df_seq.end() and (
+                item in df_seq.at(occurrence[item_index][0])
+            ):
                 return [occurrence], [cursim]
             else:
-                return [],[]
+                return [], []
 
-        occurrences: Sequence[ Sequence[ Tuple[np.timedelta64,np.timedelta64] ] ] = []
+        occurrences: Sequence[Sequence[Tuple[np.timedelta64, np.timedelta64]]] = []
         sims: Sequence[float] = []
 
-        df_select = df_seq[ (df_seq>=occurrence[item_index][0]) &
-                            (df_seq<=occurrence[item_index][1])]
-        for p in df_select[ df_select==item ]._dates:
-            #create a new occurrence to be modified
+        df_select = df_seq[
+            (df_seq >= occurrence[item_index][0])
+            & (df_seq <= occurrence[item_index][1])
+        ]
+        for p in df_select[df_select == item]._dates:
+            # create a new occurrence to be modified
             new_occ = occurrence[:]
-            new_occ[item_index] = (p,p)
+            new_occ[item_index] = (p, p)
 
             sim = cursim
-            for k,v in self.tconst.items():
-                if (k[1]==item_index) and (k[0] in self.sequence):
+            for k, v in self.tconst.items():
+                if (k[1] == item_index) and (k[0] in self.sequence):
                     # HERE: it is mandatory to have k[0]<item_index to ensure that
                     # occurrence[ k[0] ] is a singleton
-                    assert( occurrence[ k[0] ][0] == occurrence[ k[0] ][1] )
-                    #evaluate the similarity (product of the current sim with local sim)
-                    sim *= self.__interval_sim( p-occurrence[ k[0] ][0], v)
-            if sim < self.sim_max or sim < self.min_reco_sim :
+                    assert occurrence[k[0]][0] == occurrence[k[0]][1]
+                    # evaluate the similarity (product of the current sim with local sim)
+                    sim *= self.__interval_sim(p - occurrence[k[0]][0], v)
+            if sim < self.sim_max or sim < self.min_reco_sim:
                 # The partial distance is below the global similarity
                 # measure => will never generate a better occurrence!
                 # then, discard this occurrence
                 continue
 
-            satisfiable=True
-            #propagate chronicle constraints
-            for k,v in self.tconst.items():
-                if (k[0]==item_index) and (k[1] in self.sequence):
-                    new_occ[ k[1] ] = (max(new_occ[ k[1] ][0], p+v[0]-self.interval_extension),
-                                        min(new_occ[ k[1] ][1], p+v[1]+self.interval_extension))
-                    if new_occ[ k[1] ][0]>new_occ[ k[1] ][1]:
-                        #if empty interval, it is not satisfiable
-                        satisfiable=False
+            satisfiable = True
+            # propagate chronicle constraints
+            for k, v in self.tconst.items():
+                if (k[0] == item_index) and (k[1] in self.sequence):
+                    new_occ[k[1]] = (
+                        max(new_occ[k[1]][0], p + v[0] - self.interval_extension),
+                        min(new_occ[k[1]][1], p + v[1] + self.interval_extension),
+                    )
+                    if new_occ[k[1]][0] > new_occ[k[1]][1]:
+                        # if empty interval, it is not satisfiable
+                        satisfiable = False
                         break
 
             if satisfiable:
-                #add the occurrence to the list, and the corresponding similarity
-                occurrences.append( new_occ )
-                sims.append( sim )
+                # add the occurrence to the list, and the corresponding similarity
+                occurrences.append(new_occ)
+                sims.append(sim)
         return occurrences, sims
 
-    def __simrecognize__(self, occurrence:Sequence[ Tuple[np.timedelta64,np.timedelta64] ],
-                                sim : float,
-                                last_item_index : int,
-                                df_seq: TimedSequence)-> Tuple[ Sequence[ Sequence[ Tuple[np.timedelta64,np.timedelta64] ] ], Sequence[float] ]:
+    def __simrecognize__(
+        self,
+        occurrence: Sequence[Tuple[np.timedelta64, np.timedelta64]],
+        sim: float,
+        last_item_index: int,
+        df_seq: TimedSequence,
+    ) -> Tuple[
+        Sequence[Sequence[Tuple[np.timedelta64, np.timedelta64]]], Sequence[float]
+    ]:
         """
-        recursive call for occurrence recognition
-        return a list of occurrences recognized from the last_item_index of the
+        Recursive call for occurrence recognition
+
+        Returns
+        -------
+        A list of occurrences recognized from the last_item_index of the
         chronicle until its last item
+
+        :meta private:
         """
-        chro_size=max( self.sequence )
-        if last_item_index==chro_size:
-            return [occurrence],[sim]
-
-        item_index=last_item_index+1
-
-        occurrences: Sequence[ Sequence[ Tuple[np.timedelta64,np.timedelta64] ] ] = []
-        sims:Sequence[float] = []
-        loc_occs, loc_sims = self.__complete_similarity__(occurrence, sim, item_index, df_seq)
+        chro_size = max(self.sequence)
+        if last_item_index == chro_size:
+            return [occurrence], [sim]
+
+        item_index = last_item_index + 1
+
+        occurrences: Sequence[Sequence[Tuple[np.timedelta64, np.timedelta64]]] = []
+        sims: Sequence[float] = []
+        loc_occs, loc_sims = self.__complete_similarity__(
+            occurrence, sim, item_index, df_seq
+        )
         for i in range(len(loc_occs)):
-            reoccs,resims= self. __simrecognize__(loc_occs[i], loc_sims[i], item_index, df_seq)
+            reoccs, resims = self.__simrecognize__(
+                loc_occs[i], loc_sims[i], item_index, df_seq
+            )
             occurrences.extend(reoccs)
             sims.extend(resims)
-        return occurrences,sims
+        return occurrences, sims
 
-    def cmp(self,
-            df_seq:TimedSequence,
-            threshold: float,
-            lbda : float =0.01) -> Tuple[ Sequence[ Sequence[ np.timedelta64 ] ], Sequence[float] ]:
+    def cmp(
+        self, df_seq: TimedSequence, threshold: float, lbda: float = 0.01
+    ) -> Tuple[Sequence[Sequence[np.timedelta64]], Sequence[float]]:
         """
-        Method that checks whether the chronicle occurs in the sequence
+        Method that checks whether the chronicle occurs in the sequence and evaluates the simiarlity for each of the occurrences.
 
         Parameters
         ----------
         df_seq : Dataframe, or list of itemsets or list of couples (date, event)
-            DESCRIPTION.
         threshold : float in [0,1]
             minimal similarity measure to recognize a chronicle
         lbda : float >0, optional
             parameter of the similarity measure
 
         Returns
         -------
@@ -194,77 +260,98 @@
             of lists of positions, each list is an occurrence. It contains a list of n couples,
             where n is the chronicle size)
             The second element is the list of similarity between the occurrences and the chronicle.
             A similarity of 1 means an exact matching, lower similarity means that events have been
             found but not with the exact temporal bounds.
 
         """
-        chro_size=max( self.sequence )+1
-        if chro_size==0 :
-            return [],[]
+        chro_size = max(self.sequence) + 1
+        if chro_size == 0:
+            return [], []
 
         self.min_reco_sim = threshold
         self.lbda = lbda
         # computes the analytical maximal interval extension
-        self.interval_extension = int(np.ceil( -1.0/float(lbda)*np.log( float(self.min_reco_sim)) ))
+        self.interval_extension = int(
+            np.ceil(-1.0 / float(lbda) * np.log(float(self.min_reco_sim)))
+        )
 
         item_index = 0
-        item=self.sequence[item_index]
+        item = self.sequence[item_index]
 
-        self.sim_max : float =0
+        self.sim_max: float = 0
 
-        #list of occurrences
-        roccurrences : Sequence[ Sequence[ Tuple[np.timedelta64,np.timedelta64] ] ] = []
+        # list of occurrences
+        roccurrences: Sequence[Sequence[Tuple[np.timedelta64, np.timedelta64]]] = []
         rsims: Sequence[float] = []
 
-        #select all elements that match the item
-        for p in df_seq[ df_seq==item ]._dates:
+        # select all elements that match the item
+        for p in df_seq[df_seq == item]._dates:
             # create a new occurrence
             new_occ = []
-            resize(new_occ, chro_size, (df_seq.start(),df_seq.end()))
-            new_occ[item_index] = (p,p)
+            resize(new_occ, chro_size, (df_seq.start(), df_seq.end()))
+            new_occ[item_index] = (p, p)
 
             # propagate chronicle constraints
-            for k,v in self.tconst.items():
-                if (k[0]==item_index) and (k[1] in self.sequence):
-                    new_occ[ k[1] ] = (max(df_seq.start(),p+v[0]-self.interval_extension),
-                                        min(p+v[1]+self.interval_extension,df_seq.end()))
+            for k, v in self.tconst.items():
+                if (k[0] == item_index) and (k[1] in self.sequence):
+                    new_occ[k[1]] = (
+                        max(df_seq.start(), p + v[0] - self.interval_extension),
+                        min(p + v[1] + self.interval_extension, df_seq.end()),
+                    )
 
             # add the occurrence to the list of occurrences
             occurrences, sims = self.__simrecognize__(new_occ, 1, item_index, df_seq)
             for i in range(len(occurrences)):
-                if sims[i]>self.sim_max:
-                    self.sim_max=sims[i]
-                roccurrences.append( occurrences[i] )
-                rsims.append( sims[i] )
+                if sims[i] > self.sim_max:
+                    self.sim_max = sims[i]
+                roccurrences.append(occurrences[i])
+                rsims.append(sims[i])
+
+        return [[e[0] for e in occ] for occ in roccurrences], rsims
 
-        return [ [e[0] for e in occ] for occ in roccurrences], rsims
 
 if __name__ == "__main__":
     #################################
-    #Example of sequence
-    seq = [('a',1),('c',2),('b',3),('a',8),('a',10),('b',12),('a',15),('c',17),
-            ('b',20),('c',23),('c',25),('b',26),('c',28),('b',30)]
-
-    dates = np.array([np.datetime64('1970-01-01') + np.timedelta64(e[1],'D') for e in seq],
-                        dtype='datetime64')
+    # Example of sequence
+    seq = [
+        ("a", 1),
+        ("c", 2),
+        ("b", 3),
+        ("a", 8),
+        ("a", 10),
+        ("b", 12),
+        ("a", 15),
+        ("c", 17),
+        ("b", 20),
+        ("c", 23),
+        ("c", 25),
+        ("b", 26),
+        ("c", 28),
+        ("b", 30),
+    ]
+
+    dates = np.array(
+        [np.datetime64("1970-01-01") + np.timedelta64(e[1], "D") for e in seq],
+        dtype="datetime64",
+    )
     data = np.array([e[0] for e in seq])
 
     ts = TimedSequence(dates, data)
 
-    c=FuzzyChronicle()
-    c.add_event(0,'b')
-    c.add_event(1,'a')
-    c.add_event(2,'c')
-    c.add_constraint(0,1, (np.timedelta64(13,'D'),np.timedelta64(17,'D')))
-    c.add_constraint(0,2, (np.timedelta64(1,'D'),np.timedelta64(30,'D')))
+    c = FuzzyChronicle()
+    c.add_event(0, "b")
+    c.add_event(1, "a")
+    c.add_event(2, "c")
+    c.add_constraint(0, 1, (np.timedelta64(13, "D"), np.timedelta64(17, "D")))
+    c.add_constraint(0, 2, (np.timedelta64(1, "D"), np.timedelta64(30, "D")))
     c.minimize()
-    c.tunit='D'
+    c.tunit = "D"
     print(c)
 
-    occ,sim = c.cmp(ts,0.95,0.3)
+    occ, sim = c.cmp(ts, 0.95, 0.3)
     print("similarity:" + str(sim))
-    print("occurrence:"+ str(occ))
+    print("occurrence:" + str(occ))
 
-    for i in range(40,100,5):
-        occ,sim = c.cmp(ts,float(i)/100.0,0.3)
-        print("found (",str(float(i)/100.0),"):", occ)
+    for i in range(40, 100, 5):
+        occ, sim = c.cmp(ts, float(i) / 100.0, 0.3)
+        print("found (", str(float(i) / 100.0), "):", occ)
```

### Comparing `pychronicles-0.0.9/pychronicles/mtlformula.py` & `pychronicles-0.1.0/pychronicles/mtlformula.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 #!/bin/python3
 # -*- coding: utf-8 -*-
 """
 MTL formula
 
-@author: Thomas Guyet
-@date: 10/2022
-@institution: Inria
-
-Perspectives:
----------------
+:Authors:
+    Thomas Guyet, Inria
+:Date:
+    08/2023
 """
 
 import pandas as pd
 from pandas.api.extensions import register_dataframe_accessor
 import mtl
 from lark import Lark, Transformer, Token
 
 
-MTL_grammar:str=r"""
+MTL_grammar: str = r"""
 formula: atom | MODAL formula | MODAL "(" formula ")" | MODAL interval "(" formula ")" | formula MODAL_OPERATOR formula
 expr: "(" expr ")" | CNAME | expr OPERATOR expr | NUMBER | "True" | "False" | /\u0060.*\u0060/ | /"[^"]*"/ | /'[^']*'/
 atom: expr EVENT_CMP expr
 
 EVENT_CMP: ("<=" | "!=" | "==" | ">=" | "<" | ">" )
 MODAL: ("G" | "F" | "~")
 MODAL_OPERATOR: ("&" | "^" | "|" | "->" | "<->")
@@ -33,150 +31,176 @@
 %ignore WHITESPACE
 %import common.SIGNED_NUMBER    -> NUMBER
 %import common.CNAME
 """
 
 
 class ExtractMTL(Transformer):
-    """Class that transforms a MTL formula that is based on query expression 
-    into a set of expressions for pandas datasets and a MTL formula that can 
+    """Class that transforms a MTL formula that is based on query expression
+    into a set of expressions for pandas datasets and a MTL formula that can
     be used to query a dataframe
     """
 
     def __init__(self):
         super().__init__()
-        self.atoms={}
+        self.atoms = {}
 
     def expr(self, tree):
         retstr = ""
         for c in tree:
-            if isinstance(c,str):
+            if isinstance(c, str):
                 retstr += c
-            elif isinstance(c,Token):
+            elif isinstance(c, Token):
                 retstr += str(c.value)
         return retstr
 
     def atom(self, tree):
-        formula=tree[0]+str(tree[1].value)+tree[2]
+        formula = tree[0] + str(tree[1].value) + tree[2]
         if formula not in self.atoms:
-            self.atoms[formula] = "expr"+str(len(self.atoms))
-        return mtl.parse( self.atoms[formula] )
+            self.atoms[formula] = "expr" + str(len(self.atoms))
+        return mtl.parse(self.atoms[formula])
 
-    def interval(self,tree):
-        return [str(tree[0]) , str(tree[1]) ]
+    def interval(self, tree):
+        return [str(tree[0]), str(tree[1])]
 
-    def formula(self,tree):
-        retstr=""
-        if isinstance(tree[0],Token):
-            #UNIMODAL operator
-            if len(tree)==3:
-                if tree[0].value=="G":
+    def formula(self, tree):
+        retstr = ""
+        if isinstance(tree[0], Token):
+            # UNIMODAL operator
+            if len(tree) == 3:
+                if tree[0].value == "G":
                     return tree[2].always(lo=float(tree[1][0]), hi=float(tree[1][1]))
-                elif tree[0].value=="F":
-                    return tree[2].eventually(lo=float(tree[1][0]), hi=float(tree[1][1]))
+                elif tree[0].value == "F":
+                    return tree[2].eventually(
+                        lo=float(tree[1][0]), hi=float(tree[1][1])
+                    )
             else:
-                if tree[0].value=="G":
+                if tree[0].value == "G":
                     return tree[1].always()
-                elif tree[0].value=="F":
+                elif tree[0].value == "F":
                     return tree[1].eventually()
-                else: #neg
+                else:  # neg
                     return ~tree[1]
         else:
-            if len(tree)==1:
+            if len(tree) == 1:
                 return tree[0]
             else:
-                assert tree[1].value in ["&","|","^","<->","->"]
-                if tree[1].value=="&":
+                assert tree[1].value in ["&", "|", "^", "<->", "->"]
+                if tree[1].value == "&":
                     return tree[0] & tree[2]
-                if tree[1].value=="|":
+                if tree[1].value == "|":
                     return tree[0] | tree[2]
-                if tree[1].value=="^":
+                if tree[1].value == "^":
                     return tree[0] ^ tree[2]
-                if tree[1].value=="<->":
+                if tree[1].value == "<->":
                     return tree[0].iff(tree[2])
-                if tree[1].value=="->":
+                if tree[1].value == "->":
                     return tree[0].implies(tree[2])
-    
 
-    def parse(self,formula):
-        return self.transform( Lark(MTL_grammar, start="formula").parse(formula) )
+    def parse(self, formula):
+        return self.transform(Lark(MTL_grammar, start="formula").parse(formula))
+
 
 @register_dataframe_accessor("mtl")
 class MTLAccessor:
     def __init__(self, df: pd.DataFrame):
         self._validate(df)
         self._df = df
-        self.simplifer=ExtractMTL()
+        self.simplifer = ExtractMTL()
 
     @staticmethod
     def _validate(df):
         # verify there is a no MultiIndex, and that the Index is made of Integers or Timestamps
         if isinstance(df.index, pd.MultiIndex):
             raise AttributeError("Can not handle multi-indexed dataframes.")
-        if df.index.dtype!=float and df.index.dtype!=int:
+        if df.index.dtype != float and df.index.dtype != int:
             raise AttributeError("Dataframe index has to be convertible in float.")
 
     @staticmethod
     def __lemmatize_query(q):
-        return q.replace(" ", "").replace("'",'"')
+        return q.replace(" ", "").replace("'", '"')
 
     def __transform(self, atoms, dt=1):
-        data={}
-        for k,v in atoms.items():
-            data[v]=[ (e,True) for e in self._df.query(k).index.to_list()]
-            data[v]+=[ (e+dt,False) for e in self._df.query(k).index.to_list()]
+        data = {}
+        for k, v in atoms.items():
+            data[v] = [(e, True) for e in self._df.query(k).index.to_list()]
+            data[v] += [(e + dt, False) for e in self._df.query(k).index.to_list()]
             data[v].sort(key=lambda x: x[0])
         return data
 
-    def match(self, formula : str):
+    def match(self, formula: str):
         """
         formula is a MTL formula
         """
-        dt=1
-        mtl_formula=self.simplifer.transform( Lark(MTL_grammar, start="formula").parse(formula) )
-        data=self.__transform(self.simplifer.atoms,dt)
-        #return mtl_formula(data, time=None, dt=dt, quantitative=False)
+        dt = 1
+        mtl_formula = self.simplifer.transform(
+            Lark(MTL_grammar, start="formula").parse(formula)
+        )
+        data = self.__transform(self.simplifer.atoms, dt)
+        # return mtl_formula(data, time=None, dt=dt, quantitative=False)
         return mtl_formula(data, dt=dt, quantitative=False)
 
 
 if __name__ == "__main__":
     import numpy as np
+
     #################################
-    #Example of sequence
-    seq = [('a',1),('c',2),('b',3),('a',8),('a',10),('b',12),('a',15),('c',17),
-            ('b',20),('c',23),('c',25),('b',26),('c',28),('b',30)]
+    # Example of sequence
+    seq = [
+        ("a", 1),
+        ("c", 2),
+        ("b", 3),
+        ("a", 8),
+        ("a", 10),
+        ("b", 12),
+        ("a", 15),
+        ("c", 17),
+        ("b", 20),
+        ("c", 23),
+        ("c", 25),
+        ("b", 26),
+        ("c", 28),
+        ("b", 30),
+    ]
 
     df = pd.DataFrame(
         {
             "label": [e[0] for e in seq],
-            "str_val": [e[0]*2 for e in seq], #illustration of another columns than "label"
-            "num_val": np.random.randint(10,size=len(seq)), #illustration of another columns than "label"
+            "str_val": [
+                e[0] * 2 for e in seq
+            ],  # illustration of another columns than "label"
+            "num_val": np.random.randint(
+                10, size=len(seq)
+            ),  # illustration of another columns than "label"
         },
-        index = [e[1] for e in seq]
+        index=[e[1] for e in seq],
     )
     print(df)
     print("----------------")
 
-    query=' F(label=="a" & F[2.9,5]( label=="b" & num_val>5 ))'
-    result=df.mtl.match(query)
+    query = ' F(label=="a" & F[2.9,5]( label=="b" & num_val>5 ))'
+    result = df.mtl.match(query)
     print(result)
 
     ##########################################################################
     # Use with a dataframe representing a collection of sequences
 
     # Create a dataframe representing several sequences with complex events, each sequence having its own id
     grpdf = pd.DataFrame(
         {
-         "label": [e[0] for e in seq]*3,
-         "str_val": [e[0]*2 for e in seq]*3, #illustration of another columns than "label"
-         "num_val": np.random.randint(10,size=3*len(seq)), #illustration of another columns than "label"
-         'id': [1]*len(seq)+[2]*len(seq)+[3]*len(seq)
+            "label": [e[0] for e in seq] * 3,
+            "str_val": [e[0] * 2 for e in seq]
+            * 3,  # illustration of another columns than "label"
+            "num_val": np.random.randint(
+                10, size=3 * len(seq)
+            ),  # illustration of another columns than "label"
+            "id": [1] * len(seq) + [2] * len(seq) + [3] * len(seq),
         },
-        index = [e[1] for e in seq]*3
+        index=[e[1] for e in seq] * 3,
     )
-    #print(grpdf)
+    # print(grpdf)
 
     # the match function checks chronicle matches on all the sequences at the same time and
     # returns its answer for each chronicle
     print(f"Does the formula match a dataset of sequences?")
-    reco=grpdf.groupby('id').apply(lambda d: d.mtl.match(query))
-    print(reco)
+    reco = grpdf.groupby("id").apply(lambda d: d.mtl.match(query))
+    print(reco)
```

