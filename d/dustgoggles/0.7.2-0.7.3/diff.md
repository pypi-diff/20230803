# Comparing `tmp/dustgoggles-0.7.2.tar.gz` & `tmp/dustgoggles-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dustgoggles-0.7.2.tar", last modified: Mon Jun  5 13:54:05 2023, max compression
+gzip compressed data, was "dustgoggles-0.7.3.tar", last modified: Thu Aug  3 13:41:14 2023, max compression
```

## Comparing `dustgoggles-0.7.2.tar` & `dustgoggles-0.7.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/
--rw-r--r--   0 sierra    (1000) sierra    (1000)     1524 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/LICENSE
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      326 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/PKG-INFO
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 13:54:05.427861 dustgoggles-0.7.2/dustgoggles/
--rw-r--r--   0 sierra    (1000) sierra    (1000)       22 2023-06-05 13:50:03.000000 dustgoggles-0.7.2/dustgoggles/__init__.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/dustgoggles/codex/
--rw-r--r--   0 sierra    (1000) sierra    (1000)        0 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/codex/__init__.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     3518 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/codex/_array_holding_area.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     5794 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/codex/codecs.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)    33342 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/codex/implements.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     3351 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/codex/memutilz.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     9250 2023-05-30 13:53:39.000000 dustgoggles-0.7.2/dustgoggles/composition.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     6086 2023-05-30 13:53:39.000000 dustgoggles-0.7.2/dustgoggles/dynamic.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     3738 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/func.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     5422 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/mosaic.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     8586 2023-06-05 13:31:46.000000 dustgoggles-0.7.2/dustgoggles/pivot.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     4035 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/scrape.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)    13514 2023-05-30 13:53:39.000000 dustgoggles-0.7.2/dustgoggles/structures.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/dustgoggles/test_utils/
--rw-r--r--   0 sierra    (1000) sierra    (1000)       20 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/test_utils/__init__.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     2519 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/test_utils/core.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     2036 2023-05-30 13:53:39.000000 dustgoggles-0.7.2/dustgoggles/tracker.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/dustgoggles.egg-info/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      326 2023-06-05 13:54:05.000000 dustgoggles-0.7.2/dustgoggles.egg-info/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      625 2023-06-05 13:54:05.000000 dustgoggles-0.7.2/dustgoggles.egg-info/SOURCES.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2023-06-05 13:54:05.000000 dustgoggles-0.7.2/dustgoggles.egg-info/dependency_links.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       87 2023-06-05 13:54:05.000000 dustgoggles-0.7.2/dustgoggles.egg-info/requires.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       12 2023-06-05 13:54:05.000000 dustgoggles-0.7.2/dustgoggles.egg-info/top_level.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/setup.cfg
--rw-r--r--   0 sierra    (1000) sierra    (1000)      494 2023-06-05 13:50:03.000000 dustgoggles-0.7.2/setup.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-08-03 13:41:14.028306 dustgoggles-0.7.3/
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     1524 2023-05-30 13:48:19.000000 dustgoggles-0.7.3/LICENSE
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      326 2023-08-03 13:41:14.028306 dustgoggles-0.7.3/PKG-INFO
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-08-03 13:41:14.028306 dustgoggles-0.7.3/dustgoggles/
+-rw-r--r--   0 sierra    (1000) sierra    (1000)       22 2023-08-03 13:31:40.000000 dustgoggles-0.7.3/dustgoggles/__init__.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-08-03 13:41:14.028306 dustgoggles-0.7.3/dustgoggles/codex/
+-rw-r--r--   0 sierra    (1000) sierra    (1000)        0 2023-05-30 13:48:19.000000 dustgoggles-0.7.3/dustgoggles/codex/__init__.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     3518 2023-05-30 13:48:19.000000 dustgoggles-0.7.3/dustgoggles/codex/_array_holding_area.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     5794 2023-05-30 13:48:19.000000 dustgoggles-0.7.3/dustgoggles/codex/codecs.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)    33342 2023-05-30 13:48:19.000000 dustgoggles-0.7.3/dustgoggles/codex/implements.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     3351 2023-05-30 13:48:19.000000 dustgoggles-0.7.3/dustgoggles/codex/memutilz.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    10605 2023-06-30 04:02:32.000000 dustgoggles-0.7.3/dustgoggles/composition.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     6155 2023-06-30 04:02:32.000000 dustgoggles-0.7.3/dustgoggles/dynamic.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     3738 2023-05-30 13:48:19.000000 dustgoggles-0.7.3/dustgoggles/func.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     5422 2023-05-30 13:48:19.000000 dustgoggles-0.7.3/dustgoggles/mosaic.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     8901 2023-08-03 13:29:28.000000 dustgoggles-0.7.3/dustgoggles/pivot.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     4035 2023-05-30 13:48:19.000000 dustgoggles-0.7.3/dustgoggles/scrape.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)    13514 2023-05-30 13:53:39.000000 dustgoggles-0.7.3/dustgoggles/structures.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-08-03 13:41:14.028306 dustgoggles-0.7.3/dustgoggles/test_utils/
+-rw-r--r--   0 sierra    (1000) sierra    (1000)       20 2023-05-30 13:48:19.000000 dustgoggles-0.7.3/dustgoggles/test_utils/__init__.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     2519 2023-05-30 13:48:19.000000 dustgoggles-0.7.3/dustgoggles/test_utils/core.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2377 2023-06-30 04:02:32.000000 dustgoggles-0.7.3/dustgoggles/tracker.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-08-03 13:41:14.028306 dustgoggles-0.7.3/dustgoggles.egg-info/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      326 2023-08-03 13:41:14.000000 dustgoggles-0.7.3/dustgoggles.egg-info/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      625 2023-08-03 13:41:14.000000 dustgoggles-0.7.3/dustgoggles.egg-info/SOURCES.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2023-08-03 13:41:14.000000 dustgoggles-0.7.3/dustgoggles.egg-info/dependency_links.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      102 2023-08-03 13:41:14.000000 dustgoggles-0.7.3/dustgoggles.egg-info/requires.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       12 2023-08-03 13:41:14.000000 dustgoggles-0.7.3/dustgoggles.egg-info/top_level.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2023-08-03 13:41:14.028306 dustgoggles-0.7.3/setup.cfg
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      512 2023-08-03 13:31:40.000000 dustgoggles-0.7.3/setup.py
```

### Comparing `dustgoggles-0.7.2/LICENSE` & `dustgoggles-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.2/dustgoggles/codex/_array_holding_area.py` & `dustgoggles-0.7.3/dustgoggles/codex/_array_holding_area.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.2/dustgoggles/codex/codecs.py` & `dustgoggles-0.7.3/dustgoggles/codex/codecs.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.2/dustgoggles/codex/implements.py` & `dustgoggles-0.7.3/dustgoggles/codex/implements.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.2/dustgoggles/codex/memutilz.py` & `dustgoggles-0.7.3/dustgoggles/codex/memutilz.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.2/dustgoggles/composition.py` & `dustgoggles-0.7.3/dustgoggles/composition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from itertools import count
 from operator import attrgetter
-from typing import Optional, Union, Mapping, Any, Callable, Sequence, Hashable
+from typing import Optional, Union, Mapping, Any, Callable, Sequence, Hashable, \
+    MutableSequence
 
 from cytoolz import identity, keyfilter, first
 
+from dustgoggles.dynamic import exc_report
 from dustgoggles.func import naturals
 from dustgoggles.structures import enumerate_as_mapping, reindex_mapping
-from dustgoggles.tracker import TrivialTracker
+from dustgoggles.tracker import TrivialTracker, Tracker
 
 
 class Composition:
     """
     class defining a composition of steps, optionally with
     additional input, output, and i/o points ("inserts" and "sends") --
     conceptually like a signal processing chain but _not_ designed for
@@ -21,31 +24,39 @@
             Union[Mapping[Any, Callable], Sequence[Callable]]
         ] = None,
         sends: Optional[Union[Mapping[Any, Sequence], Sequence]] = None,
         inserts: Optional[
             Union[Mapping[Any, Mapping], Sequence[Mapping]]
         ] = None,
         name: Optional[str] = None,
-        tracker: Optional[TrivialTracker] = None
+        tracker: Optional[TrivialTracker] = None,
+        optional = False
     ):
+        self.captures = None
         self.name = "untitled Composition" if name is None else name
         if tracker is not None:
             tracker.name = self.name
         self.tracker = tracker
         if steps is None:
             steps = [identity]
         self.steps = enumerate_as_mapping(steps)
         self.tracker = tracker
         # sends and inserts could be defaultdicts, but in this case the
         # representation is ugly and the convenience is small.
         self.sends = enumerate_as_mapping(sends)
         self.inserts = enumerate_as_mapping(inserts)
+        self.optional = optional
         if self.tracker is not None:
-            for k in self.steps.keys():
-                self._add_track_send(k)
+            self._add_track_sends()
+
+    def track(self):
+        if self.tracker is not None:
+            return
+        self.tracker = Tracker()
+        self._add_track_sends()
 
     def _check_for_step(self, step_name: Hashable) -> Any:
         if step_name not in self.steps.keys():
             raise KeyError(f"{step_name} is not an element of the pipeline.")
         return self.steps[step_name]
 
     def add_step(self, step: Callable, name: Optional[Hashable] = None):
@@ -55,14 +66,18 @@
         pipeline; otherwise, replace the current step at "name".
         """
         if name is None:
             name = len(self.steps) + 1
         self.steps[name] = step
         self._add_track_send(name)
 
+    def _add_track_sends(self):
+        for k in self.steps.keys():
+            self._add_track_send(k)
+
     def _add_track_send(self, step_name: Hashable):
         if self.tracker is None:
             return
         self.add_send(
             step_name,
             pipe=_track_factory(self.tracker, step_name, self.steps[step_name])
         )
@@ -101,24 +116,40 @@
                     continue
                 pipe(state)
             elif pipe is None:
                 self.place_into(state, target, index)
             else:
                 self.place_into(pipe(state), target, index)
 
+    def add_captures(self):
+        """add captures to all steps."""
+        self.captures = {step: [None] for step in self.steps}
+        for k, v in self.captures.items():
+            self.add_capture(k, v)
+
+    def add_capture(
+        self, step_name: Hashable, target: Optional[MutableSequence]
+    ):
+        """
+        creates a send to a simple capture object that stores the last output
+        of that pipeline step.
+        """
+        target = [None] if target is None else target
+        self.add_send(step_name, target=target, pointer=0)
+
     def add_send(
         self,
         step_name: Hashable,
         pipe: Optional[Callable] = None,
         target: Optional[Any] = None,
         pointer: Union[str, int, None] = None
     ):
         """
         adds a send to the pipeline after step_name; sends to pointer
-        at target after processing through pipe. a string or int isas an
+        at target after processing through pipe. a string or int is an
         insert into the step named 'target' of self. if no target is given,
         merely calls pipe and sends its output to nowhere. you are allowed
         to create sends from nonexistent step names, but they will do nothing
         unless that step name is later assigned.
         """
         if (target is None) and (pipe is None):
             raise ValueError(
@@ -207,19 +238,30 @@
         state = signal
         for step_name in self.steps.keys():
             state = self._do_step(step_name, state)
             yield state
 
     def execute(self, signal: Any = None, **special_kwargs):
         """execute the pipeline, initializing it with signal."""
-        iterpipe = self.itercall(signal, **special_kwargs)
-        state = None
-        for state in iterpipe:
-            pass
-        return state
+        step_ix = -1
+        try:
+            iterpipe = self.itercall(signal, **special_kwargs)
+            state = None
+            for step_ix, state in zip(count(), iterpipe):
+                pass
+            return state
+        except Exception as ex:
+            if self.tracker is not None:
+                self.tracker.track(
+                    self.steps[tuple(self.steps.keys())[step_ix + 1]],
+                    **exc_report(ex, stepback=0)
+                )
+            if self.optional is True:
+                return None
+            raise
 
     def iter(self):
         raise NotImplementedError
 
     def _bind_special_runtime_kwargs(self, special_kwargs):
         """
         apply kwargs at time of execution across multiple steps
```

### Comparing `dustgoggles-0.7.2/dustgoggles/dynamic.py` & `dustgoggles-0.7.3/dustgoggles/dynamic.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,18 +52,20 @@
 
 
 def define(code: CodeType, globals_: Optional[dict] = None) -> FunctionType:
     globals_ = globals_ if globals_ is not None else globals()
     return FunctionType(code, globals_)
 
 
-def exc_report(exc):
+def exc_report(exc, stepback=1):
     if exc is None:
         return {}
-    stack = traceback.extract_tb(exc.__traceback__)[:-2]
+    stack = traceback.extract_tb(exc.__traceback__)
+    if stepback > 0:
+        stack = stack[: -(1 + stepback)]
     return {
         "exception": exc,
         "lineno": tuple([a.lineno for a in stack]),
         "stack": tuple([a.name for a in stack]),
         "time": dt.datetime.now().isoformat()[:-3],
     }
```

### Comparing `dustgoggles-0.7.2/dustgoggles/func.py` & `dustgoggles-0.7.3/dustgoggles/func.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.2/dustgoggles/mosaic.py` & `dustgoggles-0.7.3/dustgoggles/mosaic.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.2/dustgoggles/pivot.py` & `dustgoggles-0.7.3/dustgoggles/pivot.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,46 +48,54 @@
         test_equality = dataframe.loc[:, column] == dataframe.loc[:, column]
         if not test_equality.all(axis=None):
             raise ValueError
     return dataframe.loc[:, ~dataframe.columns.duplicated()]
 
 
 def extract_constants(
-    df, to_dict=True, drop_constants=False, how="rows", dropna=True
+    df: pd.DataFrame,
+    to_dict=True,
+    drop_constants=False,
+    how="rows",
+    dropna=True
 ):
     """
     extract 'constant' values from a dataframe -- by default, columns with
     the same value in each row; if how == 'columns', then indices with the
     same value in each column. if to_dict is True, transforms them into a
     dictionary with keys equal to column/index names and values equal to the
     constant values. if drop_constants is True, also removes these
     constant-valued rows/columns from the returned dataframe.
     returns the constants (as a dict if specified) and either the
     variable-only or full original dataframe (as specified)
     """
+    if how not in ("rows", "columns"):
+        raise ValueError(f"unknown how {how}")
     if how == "rows":
-        axis = 0
-    elif how == "columns":
-        axis = 1
+        constant_indices = pd.Series(False, df.columns)
     else:
-        raise ValueError(f"unknown how {how}")
+        constant_indices = pd.Series(False, df.index)
     try:
-        constant_indices = df.nunique(axis=axis, dropna=dropna) <= 1
+        method = "iterrows" if how == "columns" else "items"
+        for ix, series in getattr(df, method)():
+            series = series if dropna is False else series.dropna()
+            if (series == series.iloc[0]).all():
+                constant_indices.loc[ix] = True
     except TypeError:
-        if axis == 1:
+        # TODO: still necessary?
+        if how == "columns":
             raise NotImplementedError("nested fields not supported columnwise")
-        constant_indices = pd.Series(False, df.columns)
         for c in df.columns:
             if isinstance(df[c].iloc[0], list):
                 test_series = df[c].map(tuple)
             else:
                 test_series = df[c]
-            if test_series.nunique(dropna=dropna) <= 1:
+            if (test_series.iloc[0] == test_series).all():
                 constant_indices.loc[c] = True
-    if axis == 0:
+    if how == "rows":
         constants = df.loc[:, constant_indices]
         variables = df.loc[:, ~constant_indices]
     else:
         constants = df.loc[constant_indices]
         variables = df.loc[~constant_indices]
     if to_dict:
         constants = constants.iloc[0].to_dict()
```

### Comparing `dustgoggles-0.7.2/dustgoggles/scrape.py` & `dustgoggles-0.7.3/dustgoggles/scrape.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.2/dustgoggles/structures.py` & `dustgoggles-0.7.3/dustgoggles/structures.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.2/dustgoggles/test_utils/core.py` & `dustgoggles-0.7.3/dustgoggles/test_utils/core.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.2/dustgoggles/tracker.py` & `dustgoggles-0.7.3/dustgoggles/tracker.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,23 +14,29 @@
 
     def clear(self):
         pass
 
     def set_metadata(self, **metadata):
         pass
 
+    log = None
     history = None
 
 
 class Tracker(TrivialTracker):
     """watches where it's been"""
 
     def __init__(self, name=None, identifier="", outdir=None):
         self.history, self.metadata, self.counter = [], {}, count(1)
         self.name = name
+        self.log = {
+            "name": self.name,
+            "init_timestamp": dt.datetime.now().isoformat(),
+            "history": self.history,
+        }
         if outdir is None:
             outdir = Path(__file__).parent.parent / ".tracker_logs"
         if identifier != "":
             identifier = f"{identifier}_"
         outdir.mkdir(exist_ok=True)
         self.outpath = Path(outdir, f"{identifier}{self.name}.json")
 
@@ -42,35 +48,40 @@
     def track(self, func, **metadata):
         if "__name__" in dir(func):
             target = func.__name__
         else:
             target = str(func)
         caller = currentframe().f_back
         info = getframeinfo(caller)
-        rec = {
-            'target': target,
-            'caller': info.function,
-            'lineno': info.lineno,
-            'trackcount': next(self.counter),
-            'trackname': self.name
-        } | self.metadata | metadata
+        rec = (
+            {
+                "target": target,
+                "caller": info.function,
+                "lineno": info.lineno,
+                "trackcount": next(self.counter),
+            }
+            | self.metadata
+            | metadata
+        )
         self.history.append(rec)
 
     def set_metadata(self, **metadata):
         self.metadata |= metadata
 
     def _get_paused(self):
         return self._paused
 
     def _set_paused(self, state: bool):
         self._paused = state
 
     def dump(self):
         if self.paused is True:
             return
-        log = {'time': dt.datetime.now().isoformat(), 'history': self.history}
         # TODO: do this more cleverly with incremental writes etc.
+        self.log["write_timestamp"] = dt.datetime.now().isoformat()
+        key_order = sorted(self.log.keys(), key=lambda n: "history" in n)
+        self.log = {k: self.log[k] for k in key_order}
         with self.outpath.open("a") as stream:
-            json.dump(log, stream)
+            json.dump(self.log, stream, indent=2)
 
     _paused = False
     paused = property(_get_paused, _set_paused)
```

### Comparing `dustgoggles-0.7.2/dustgoggles.egg-info/SOURCES.txt` & `dustgoggles-0.7.3/dustgoggles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

