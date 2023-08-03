# Comparing `tmp/exchange_calendars_extensions-0.3.0.tar.gz` & `tmp/exchange_calendars_extensions-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars_extensions-0.3.0.tar", max compression
+gzip compressed data, was "exchange_calendars_extensions-0.3.1.tar", max compression
```

## Comparing `exchange_calendars_extensions-0.3.0.tar` & `exchange_calendars_extensions-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-07-07 08:09:05.766729 exchange_calendars_extensions-0.3.0/LICENSE
--rw-r--r--   0        0        0    30234 2023-07-07 08:09:05.766729 exchange_calendars_extensions-0.3.0/README.md
--rw-r--r--   0        0        0    26680 2023-07-07 08:09:05.766729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/__init__.py
--rw-r--r--   0        0        0    19576 2023-07-07 08:09:05.770729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/changeset.py
--rw-r--r--   0        0        0     6780 2023-07-07 08:09:05.770729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/holiday.py
--rw-r--r--   0        0        0    40255 2023-07-07 08:09:05.770729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/holiday_calendar.py
--rw-r--r--   0        0        0     5673 2023-07-07 08:09:05.770729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/offset.py
--rw-r--r--   0        0        0     2595 2023-07-07 08:09:05.770729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/util.py
--rw-r--r--   0        0        0     2888 2023-07-07 08:09:20.482809 exchange_calendars_extensions-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    31729 1970-01-01 00:00:00.000000 exchange_calendars_extensions-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-03 20:39:58.574271 exchange_calendars_extensions-0.3.1/LICENSE
+-rw-r--r--   0        0        0    30234 2023-08-03 20:39:58.574271 exchange_calendars_extensions-0.3.1/README.md
+-rw-r--r--   0        0        0    27624 2023-08-03 20:39:58.574271 exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/__init__.py
+-rw-r--r--   0        0        0    19576 2023-08-03 20:39:58.574271 exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/changeset.py
+-rw-r--r--   0        0        0     6780 2023-08-03 20:39:58.574271 exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/holiday.py
+-rw-r--r--   0        0        0    40255 2023-08-03 20:39:58.574271 exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/holiday_calendar.py
+-rw-r--r--   0        0        0     5673 2023-08-03 20:39:58.574271 exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/offset.py
+-rw-r--r--   0        0        0     2595 2023-08-03 20:39:58.574271 exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/util.py
+-rw-r--r--   0        0        0     2895 2023-08-03 20:40:11.138154 exchange_calendars_extensions-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    31729 1970-01-01 00:00:00.000000 exchange_calendars_extensions-0.3.1/PKG-INFO
```

### Comparing `exchange_calendars_extensions-0.3.0/LICENSE` & `exchange_calendars_extensions-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.3.0/README.md` & `exchange_calendars_extensions-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/__init__.py` & `exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import functools
 from datetime import time
-from typing import Optional, Callable, Type, Union, Any
+from typing import Optional, Callable, Type, Union, Any, Dict
 
 from exchange_calendars import calendar_utils, register_calendar_type, ExchangeCalendar, get_calendar_names
 from exchange_calendars.calendar_utils import _default_calendar_factories
 from exchange_calendars.exchange_calendar_asex import ASEXExchangeCalendar
 from exchange_calendars.exchange_calendar_xams import XAMSExchangeCalendar
 from exchange_calendars.exchange_calendar_xbru import XBRUExchangeCalendar
 from exchange_calendars.exchange_calendar_xbud import XBUDExchangeCalendar
@@ -31,15 +31,15 @@
 from typing_extensions import ParamSpec, Concatenate
 
 from .changeset import ChangeSet, DayType, DaySpec, DayWithTimeSpec
 from .holiday_calendar import extend_class, ExtendedExchangeCalendar, ExchangeCalendarExtensions
 
 # Dictionary that maps from exchange key to ExchangeCalendarChangeSet. Contains all changesets to apply when creating a
 # new calendar instance.
-_changesets = dict()
+_changesets: Dict[str, ChangeSet] = dict()
 
 # Dictionary that maps from exchange key to ExtendedExchangeCalendar. Contains all extended calendars classes that
 # replace the vanilla classes in exchange_calendars when calling apply_extensions().
 #
 # Note: The values in this dictionary use extend_class() to create the extended classes, respectively for each exchange,
 #     based on the respective vanilla class in exchange_calendars. Also, the changeset_provider is set to a lambda
 #     function that returns the changeset for the respective exchange in _changesets, or None, if no changeset exists.
@@ -87,35 +87,32 @@
     calendar_names = set(get_calendar_names())
 
     def get_changeset_fn(name: str) -> Callable[[], ChangeSet]:
         def fn() -> ChangeSet:
             return _changesets.get(name)
         return fn
 
-    print('Applying generic extension for calendars that have no explicit extension defined.')
     for k in calendar_names - set(_extensions.keys()):
         cls = _default_calendar_factories.get(k)
         if cls is not None:
             # Store the original class for later use.
             _original_classes[k] = cls
             # Create extended class.
             print(f'Extending {k}: {cls}')
             cls = extend_class(cls, day_of_week_expiry=None, changeset_provider=get_changeset_fn(k))
             # Register extended class.
             register_calendar_type(k, cls, force=True)
             # Remove original class from factory cache.
             _remove_calendar_from_factory_cache(k)
 
-    print('Applying extension for calendars with explicit extension defined.')
     for k, v in _extensions.items():
         cls, day_of_week_expiry = v
         # Store the original class for later use.
         _original_classes[k] = cls
         # Create extended class.
-        print(f'Extending {k}: {cls} day_of_week_expiry={day_of_week_expiry}')
         cls = extend_class(cls, day_of_week_expiry=day_of_week_expiry, changeset_provider=get_changeset_fn(k))
         # Register extended class.
         register_calendar_type(k, cls, force=True)
         # Remove original class from factory cache.
         _remove_calendar_from_factory_cache(k)
 
 
@@ -206,16 +203,20 @@
 
         # Call wrapped function with changeset as first positional argument.
         cs = f(cs, *args, **kwargs)
 
 #        if not cs.is_consistent():
 #            raise ValueError(f'Changeset for {str} is inconsistent: {cs}.')
 
-        # Save changeset back to _changesets.
-        _changesets[exchange] = cs
+        if cs is not None:
+            # Save changeset back to _changesets.
+            _changesets[exchange] = cs
+        else:
+            # Remove changeset from _changesets.
+            _changesets.pop(exchange, None)
 
         # Remove calendar for exchange key from factory cache.
         _remove_calendar_from_factory_cache(exchange)
 
         # Return result of wrapped function.
         return None
 
@@ -769,14 +770,26 @@
     Returns
     -------
     None
     """
     _reset_calendar(exchange)
 
 
+def reset_all_calendars() -> None:
+    """
+    Reset all exchange calendars to their original states.
+
+    Returns
+    -------
+    None
+    """
+    # Just clear the dict of changesets.
+    _changesets.clear()
+
+
 @_with_changeset
 def _update_calendar(_: ChangeSet, changes: dict) -> ChangeSet:
     return ChangeSet(**changes)
 
 
 def update_calendar(exchange: str, changes: dict) -> None:
     """
@@ -790,21 +803,56 @@
     Returns
     -------
     None
     """
     _update_calendar(exchange, changes)
 
 
+def get_changes_for_calendar(exchange: str) -> ChangeSet:
+    """
+    Get the changes for an exchange calendar.
+
+    Parameters
+    ----------
+    exchange : str
+        The exchange key for which to get the changes.
+
+    Returns
+    -------
+    ChangeSet
+        The changes for the exchange.
+    """
+    cs: Optional[ChangeSet] = _changesets.get(exchange, None)
+
+    if cs is not None:
+        cs = cs.model_copy(deep=True)
+
+    return cs
+
+
+def get_changes_for_all_calendars() -> dict:
+    """
+    Get the changes for all exchange calendars.
+
+    Returns
+    -------
+    dict
+        The changes for all exchange calendars.
+    """
+    return {k: v.model_copy(deep=True) for k, v in _changesets.items()}
+
+
 # Declare public names.
 __all__ = ["apply_extensions", "remove_extensions", "register_extension", "extend_class", "DayType", "add_day",
            "remove_day", "reset_day", "DaySpec", "DayWithTimeSpec", "add_holiday", "remove_holiday", "reset_holiday",
            "add_special_close", "remove_special_close", "reset_special_close", "add_special_open",
            "remove_special_open", "reset_special_open", "add_quarterly_expiry", "remove_quarterly_expiry",
            "reset_quarterly_expiry", "add_monthly_expiry", "remove_monthly_expiry", "reset_monthly_expiry",
-           "reset_calendar", "update_calendar", "ExtendedExchangeCalendar", "ExchangeCalendarExtensions"]
+           "reset_calendar", "reset_all_calendars", "update_calendar", "get_changes_for_calendar",
+           "get_changes_for_all_calendars", "ChangeSet", "ExtendedExchangeCalendar", "ExchangeCalendarExtensions"]
 
 __version__ = None
 
 try:
     from importlib.metadata import version
     # get version from installed package
     __version__ = version("exchange_calendars_extensions")
```

### Comparing `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/changeset.py` & `exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/changeset.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/holiday.py` & `exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/holiday.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/holiday_calendar.py` & `exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/holiday_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/offset.py` & `exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/offset.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/util.py` & `exchange_calendars_extensions-0.3.1/exchange_calendars_extensions/util.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.3.0/pyproject.toml` & `exchange_calendars_extensions-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "exchange-calendars-extensions"
-version = "0.3.0"
+version = "0.3.1"
 description = "Extensions of the exchange-calendars package"
 license = "Apache-2.0"
 authors = ["Jens Keiner <jens.keiner@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jenskeiner/exchange_calendars_extensions/"
 repository = "https://github.com/jenskeiner/exchange_calendars_extensions/"
 documentation = "https://github.com/jenskeiner/exchange_calendars_extensions/tree/main/docs/"
@@ -32,15 +32,15 @@
 ]
 packages = [{include = "exchange_calendars_extensions"}]
 
 [tool.poetry.dependencies]
 python = "~=3.8"
 exchange-calendars = ">=4.0.1"
 typing-extensions = ">=4.6.2,<4.8.0"
-pydantic = "~=2.0.2"
+pydantic = ">=2.0.2,<2.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.3.1,<7.5.0"
 pytest-cov = "~=4.1.0"
 pre-commit = "~=3.3.3"
```

### Comparing `exchange_calendars_extensions-0.3.0/PKG-INFO` & `exchange_calendars_extensions-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange-calendars-extensions
-Version: 0.3.0
+Version: 0.3.1
 Summary: Extensions of the exchange-calendars package
 Home-page: https://github.com/jenskeiner/exchange_calendars_extensions/
 License: Apache-2.0
 Keywords: exchange,calendar,trading,holidays
 Author: Jens Keiner
 Author-email: jens.keiner@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: exchange-calendars (>=4.0.1)
-Requires-Dist: pydantic (>=2.0.2,<2.1.0)
+Requires-Dist: pydantic (>=2.0.2,<2.2.0)
 Requires-Dist: typing-extensions (>=4.6.2,<4.8.0)
 Project-URL: Documentation, https://github.com/jenskeiner/exchange_calendars_extensions/tree/main/docs/
 Project-URL: Repository, https://github.com/jenskeiner/exchange_calendars_extensions/
 Description-Content-Type: text/markdown
 
 # exchange-calendars-extensions
 [![PyPI](https://img.shields.io/pypi/v/exchange-calendars-extensions)](https://pypi.org/project/exchange-calendars-extensions/) ![Python Support](https://img.shields.io/pypi/pyversions/exchange_calendars_extensions) ![PyPI Downloads](https://img.shields.io/pypi/dd/exchange-calendars-extensions)
```

