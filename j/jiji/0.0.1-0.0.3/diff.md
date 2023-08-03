# Comparing `tmp/jiji-0.0.1.tar.gz` & `tmp/jiji-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiji-0.0.1.tar", last modified: Wed Aug  2 17:24:09 2023, max compression
+gzip compressed data, was "jiji-0.0.3.tar", last modified: Thu Aug  3 12:39:37 2023, max compression
```

## Comparing `jiji-0.0.1.tar` & `jiji-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 17:24:09.919810 jiji-0.0.1/
--rw-rw-rw-   0        0        0      145 2023-08-02 17:24:09.918810 jiji-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-08-02 14:07:18.000000 jiji-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 17:24:09.825604 jiji-0.0.1/jiji/
--rw-rw-rw-   0        0        0       23 2023-08-01 11:59:32.000000 jiji-0.0.1/jiji/__init__.py
--rw-rw-rw-   0        0        0      226 2023-08-02 10:57:50.000000 jiji-0.0.1/jiji/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:24:09.851179 jiji-0.0.1/jiji/errors/
--rw-rw-rw-   0        0        0      153 2023-08-01 11:58:18.000000 jiji-0.0.1/jiji/errors/__init__.py
--rw-rw-rw-   0        0        0     2064 2023-08-02 10:37:27.000000 jiji-0.0.1/jiji/filters.py
--rw-rw-rw-   0        0        0     7258 2023-08-02 11:21:32.000000 jiji-0.0.1/jiji/jiji.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:24:09.884030 jiji-0.0.1/jiji/types/
--rw-rw-rw-   0        0        0      249 2023-08-02 10:46:48.000000 jiji-0.0.1/jiji/types/__init__.py
--rw-rw-rw-   0        0        0      123 2023-08-02 10:34:35.000000 jiji-0.0.1/jiji/types/condition.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:24:09.899495 jiji-0.0.1/jiji/types/product/
--rw-rw-rw-   0        0        0     3244 2023-08-02 11:01:09.000000 jiji-0.0.1/jiji/types/product/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:24:09.916298 jiji-0.0.1/jiji/types/search/
--rw-rw-rw-   0        0        0      294 2023-08-02 11:18:37.000000 jiji-0.0.1/jiji/types/search/__init__.py
--rw-rw-rw-   0        0        0      207 2023-08-02 10:30:33.000000 jiji-0.0.1/jiji/types/sort.py
--rw-rw-rw-   0        0        0      141 2023-08-02 11:07:21.000000 jiji-0.0.1/jiji/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:24:09.841147 jiji-0.0.1/jiji.egg-info/
--rw-rw-rw-   0        0        0      145 2023-08-02 17:24:09.000000 jiji-0.0.1/jiji.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-08-02 17:24:09.000000 jiji-0.0.1/jiji.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 17:24:09.000000 jiji-0.0.1/jiji.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-08-02 17:24:09.000000 jiji-0.0.1/jiji.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 17:24:09.919810 jiji-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      375 2023-08-02 17:23:29.000000 jiji-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.582543 jiji-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-03 12:39:37.582543 jiji-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 12:39:24.000000 jiji-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/jiji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/types/condition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji/types/product/
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/types/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji/types/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/types/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/types/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-03 12:39:37.000000 jiji-0.0.3/jiji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-03 12:39:37.000000 jiji-0.0.3/jiji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:39:37.000000 jiji-0.0.3/jiji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 12:39:37.000000 jiji-0.0.3/jiji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:39:37.582543 jiji-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-03 12:39:24.000000 jiji-0.0.3/setup.py
```

### Comparing `jiji-0.0.1/jiji/filters.py` & `jiji-0.0.3/jiji/filters.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from typing import Callable, Union, Dict, Any, Optional
-
-from .types import SortBy
-
-
-class Filter:
-    def __call__(self) -> Dict[str, Any]:
-        raise NotImplementedError
-
-    def __and__(self, other):
-        return And(self, other)
-
-
-class And(Filter):
-    def __init__(self, base, other):
-        self.base = base
-        self.other = other
-
-    def __call__(self, *args, **kwargs) -> Dict[str, Any]:
-        x = self.base(*args, **kwargs)
-        y = self.other(x, *args, **kwargs)
-
-        return y
-
-
-CUSTOM_FILTER_NAME = "CustomFilter"
-
-
-def create(func: Callable, name: str = None, **kwargs) -> Filter:
-    return type(
-        name or func.__name__ or CUSTOM_FILTER_NAME,
-        (Filter,),
-        {"__call__": func, **kwargs},
-    )()
-
-
-def price(
-    min_price: Optional[Union[int, str]] = 0, max_price: Optional[Union[int, str]] = ""
-) -> Filter:
-    def func(flt, prev=None) -> dict:
-        if prev:
-            prev["price_max"] = flt.max_price
-            prev["price_min"] = flt.min_price
-            return prev
-        return {"price_max": flt.max_price, "price_min": flt.min_price}
-
-    return create(
-        func,
-        name="Price",
-        min_price=min_price,
-        max_price=max_price,
-    )
-
-
-#
-#
-# def condition(cond: Union[Conditions, str]) -> Filter:
-#     cond = cond.value if isinstance(cond, Conditions) else cond
-#
-#     def func(flt, prev=None) -> dict:
-#         if prev:
-#             prev["condition"] = flt.condition
-#             return prev
-#         return {"condition": flt.condition}
-#
-#     return create(
-#         func,
-#         name="Condition",
-#         condition=cond,
-#     )
-
-
-def sort_by(sort: Union[str, SortBy]) -> Filter:
-    sort = sort.value if isinstance(sort, SortBy) else sort
-
-    def func(flt, prev=None) -> dict:
-        if prev:
-            prev["sort"] = flt.sort
-            return prev
-        return {"sort": flt.sort}
-
-    return create(
-        func,
-        name="Sort",
-        sort=sort,
-    )
+from typing import Callable, Union, Dict, Any, Optional
+
+from .types import SortBy
+
+
+class Filter:
+    def __call__(self) -> Dict[str, Any]:
+        raise NotImplementedError
+
+    def __and__(self, other):
+        return And(self, other)
+
+
+class And(Filter):
+    def __init__(self, base, other):
+        self.base = base
+        self.other = other
+
+    def __call__(self, *args, **kwargs) -> Dict[str, Any]:
+        x = self.base(*args, **kwargs)
+        y = self.other(x, *args, **kwargs)
+
+        return y
+
+
+CUSTOM_FILTER_NAME = "CustomFilter"
+
+
+def create(func: Callable, name: str = None, **kwargs) -> Filter:
+    return type(
+        name or func.__name__ or CUSTOM_FILTER_NAME,
+        (Filter,),
+        {"__call__": func, **kwargs},
+    )()
+
+
+def price(
+    min_price: Optional[Union[int, str]] = 0, max_price: Optional[Union[int, str]] = ""
+) -> Filter:
+    def func(flt, prev=None) -> dict:
+        if prev:
+            prev["price_max"] = flt.max_price
+            prev["price_min"] = flt.min_price
+            return prev
+        return {"price_max": flt.max_price, "price_min": flt.min_price}
+
+    return create(
+        func,
+        name="Price",
+        min_price=min_price,
+        max_price=max_price,
+    )
+
+
+#
+#
+# def condition(cond: Union[Conditions, str]) -> Filter:
+#     cond = cond.value if isinstance(cond, Conditions) else cond
+#
+#     def func(flt, prev=None) -> dict:
+#         if prev:
+#             prev["condition"] = flt.condition
+#             return prev
+#         return {"condition": flt.condition}
+#
+#     return create(
+#         func,
+#         name="Condition",
+#         condition=cond,
+#     )
+
+
+def sort_by(sort: Union[str, SortBy]) -> Filter:
+    sort = sort.value if isinstance(sort, SortBy) else sort
+
+    def func(flt, prev=None) -> dict:
+        if prev:
+            prev["sort"] = flt.sort
+            return prev
+        return {"sort": flt.sort}
+
+    return create(
+        func,
+        name="Sort",
+        sort=sort,
+    )
```

### Comparing `jiji-0.0.1/jiji/jiji.py` & `jiji-0.0.3/jiji/jiji.py`

 * *Files identical despite different names*

