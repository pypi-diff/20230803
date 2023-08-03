# Comparing `tmp/eule-1.0.1.tar.gz` & `tmp/eule-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eule-1.0.1.tar", max compression
+gzip compressed data, was "eule-1.0.2.tar", max compression
```

## Comparing `eule-1.0.1.tar` & `eule-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-02-27 21:15:10.623533 eule-1.0.1/LICENSE
--rw-r--r--   0        0        0     2143 2023-05-18 18:13:32.035040 eule-1.0.1/README.md
--rw-r--r--   0        0        0      225 2023-05-18 17:59:12.995691 eule-1.0.1/eule/__init__.py
--rw-r--r--   0        0        0     5833 2023-05-18 18:53:33.608403 eule-1.0.1/eule/eule.py
--rw-r--r--   0        0        0     3015 2023-05-18 17:42:29.587779 eule-1.0.1/eule/utils.py
--rw-r--r--   0        0        0     1358 2023-05-18 19:13:25.369049 eule-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 eule-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-27 21:15:10.623533 eule-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2282 2023-08-02 21:04:00.838489 eule-1.0.2/README.md
+-rw-r--r--   0        0        0      238 2023-08-02 20:31:12.518816 eule-1.0.2/eule/__init__.py
+-rw-r--r--   0        0        0     7909 2023-08-02 20:09:21.545705 eule-1.0.2/eule/eule.py
+-rw-r--r--   0        0        0     3061 2023-08-02 13:56:37.435220 eule-1.0.2/eule/utils.py
+-rw-r--r--   0        0        0     1358 2023-08-02 21:18:10.157800 eule-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3351 1970-01-01 00:00:00.000000 eule-1.0.2/PKG-INFO
```

### Comparing `eule-1.0.1/LICENSE` & `eule-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eule-1.0.1/eule/eule.py` & `eule-1.0.2/eule/eule.py`

 * *Files 20% similar despite different names*

```diff
@@ -153,8 +153,88 @@
     boundaries = dict(map(lambda key: (key, []), setsKeys))
 
     for setKey in setsKeys:
         for eulerSetKeys in eulerSetsKeys:
             if setKey in eulerSetKeys:
                 boundaries[setKey] = union(boundaries[setKey], difference(eulerSetKeys, [setKey]))
                 
-    return {setKey: sorted(neighborsKeys) for setKey, neighborsKeys in boundaries.items()}
+    return {setKey: sorted(neighborsKeys) for setKey, neighborsKeys in boundaries.items()}
+
+class Euler(object):
+    def __init__(self, sets):
+        self.sets=deepcopy(sets)
+        self.esets=euler(sets)
+
+    def __getitem__(self, keys):
+        if not isinstance(keys, tuple):
+            try:
+                return self.sets[keys]
+
+            except:
+                raise KeyError(keys)
+        
+        else:
+            elements=[]
+            try:
+                for key in keys:
+                    elements=union(self.sets[key], elements)
+
+                return elements
+            except:
+                keys=str(keys)
+                header=f"The keys must be among keys: ({keys})."
+                
+                msg=f"{header}"
+
+                raise TypeError(msg)
+    
+    def __repr__(self):
+        return str(self.as_dict())
+
+    def euler_keys(self):
+        return euler_keys(self.sets)
+
+    def euler_boundaries(self):
+        return euler_boundaries(self.sets)
+
+    def as_dict(self):
+        return self.esets
+    
+    def match(self, items: set):
+        if not isinstance(items, set):
+            raise TypeError("Items must be of type 'set'")
+        
+        # Initial value: Empty set
+        set_keys=set()
+
+        # Loop along euler set key tuples
+        for key, value in self.sets.items():
+            intersection_elems=items.intersection(set(value))
+
+            # Match operator produces the non-repeated union of euler keys which
+            # has its value set as items subset.
+            if(len(intersection_elems)==len(value)):
+                set_keys.add(key)
+            
+        
+        return set_keys
+
+    def remove_key(self, key):
+        if(key in list(self.sets.keys())):
+            self.sets = {
+                key_: value \
+                for key_, value in self.sets.items() \
+                if key_ is not key 
+            }
+
+            self.esets=euler(self.sets)
+        
+        else:
+            keys=list(self.sets.keys())
+
+            msg1=f"Key {key} is not available on current set."
+            msg2=f"Available keys are: {keys}"
+            
+            warn(msg1+" "+msg2)
+
+    
+
```

### Comparing `eule-1.0.1/eule/utils.py` & `eule-1.0.2/eule/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     :param function func: Reduce callback
     :param dict elems: list of elements
     :param dict elem0: first elements 
     """
     return reduce(func, elems + [elem0])
 
-def uniq(lst):
+def uniq(lst:list):
     """This map returns list with unique elements
 
     :param list lst: array of elements entries 
     :returns: list with unique elements 
     :rtype: list
     """
     return list(unique(lst))
@@ -54,60 +54,60 @@
     :rtype: dict
     """
     def non_empty_mask(key):
         return (len(sets[key]) != 0)
 
     return list(filter(non_empty_mask, sets.keys(), ),)
 
-def update_tuple(tuple_, value):
+def update_tuple(tuple_:tuple, value):
     """This map updates and sorts a tuple with a value
 
     :param tuple of elements:
     :param value: element to update
     :returns: an ordered and updated tuple
     :rtype: tuple
     """
     
     tuple_lst=list(tuplify(tuple_))
     tuple_lst.append(value)
     
     return tuple(tuple_lst)
 
-def list_to_set(arr):
+def list_to_set(arr:list):
     """This map converts a list into a set
 
     :param list of elements:  
     :returns: a set-converted list
     :rtype: set
     """
     return {s for s in arr}
 
-def union(listA, listB):
+def union(listA:list, listB:list):
     """This map returns the union of two lists without repetition
 
     :param listA:
     :param listB:
     :returns: list with non-repeated elements
     :rtype: list
     """
 
     return list(list_to_set(listA).union(list_to_set(listB)))
 
-def difference(listA, listB):
+def difference(listA:list, listB:list):
     """This map returns the difference of a list respective to other, without repetition
 
     :param listA:
     :param listB:
     :returns: difference list with non-repeated elements
     :rtype: list
     """
     
     return list(list_to_set(listA)-(list_to_set(listB)))
 
-def intersection(listA, listB):
+def intersection(listA:list, listB:list):
     """This map returns the intersection of a list respective to other, without repetition
 
     :param listA:
     :param listB:
     :returns: intersection list with non-repeated elements
     :rtype: list
     """
```

### Comparing `eule-1.0.1/pyproject.toml` & `eule-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eule"
-version = "1.0.1"
+version = "1.0.2"
 description = "Euler diagrams in python"
 authors = ["Bruno Peixoto <brunolnetto@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "eule"}]
 homepage = "https://pypi.org/project/eule/"
 repository = "https://github.com/trouchet/eule"
@@ -37,15 +37,15 @@
 tox = "^4.0.19"
 flake8 = "^6.0.0"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 pytest-watch = "^4.2.0"
 pylint = "^2.15.9"
 wheel = "^0.38.4"
-watchdog = "^2.2.0"
+watchdog = "^3.0.0"
 isort = "^5.11.4"
 mypy = "^0.991"
 types-mock = "^4.0.15.2"
 pygments = "^2.14.0"
 
 [tool.ruff]
 line-length = 100
```

### Comparing `eule-1.0.1/PKG-INFO` & `eule-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eule
-Version: 1.0.1
+Version: 1.0.2
 Summary: Euler diagrams in python
 Home-page: https://pypi.org/project/eule/
 License: MIT
 Keywords: euler-diagram,sets
 Author: Bruno Peixoto
 Author-email: brunolnetto@gmail.com
 Requires-Python: >=3.8.1,<4.0
@@ -22,15 +22,15 @@
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: types-toml (>=0.10.8.5,<0.11.0.0)
 Project-URL: Repository, https://github.com/trouchet/eule
 Description-Content-Type: text/markdown
 
-![a night owl](https://github.com/trouchet/eule/blob/master/images/eule_small.png?raw=true)
+![a night owl](https://github.com/trouchet/eule/blob/main/images/eule_small.png?raw=true)
 
 [![Version](https://img.shields.io/pypi/v/eule.svg)](https://pypi.python.org/pypi/eule)
 [![python](https://img.shields.io/pypi/pyversions/eule.svg)](https://pypi.org/project/eule/)
 [![downloads](https://img.shields.io/pypi/dm/eule)](https://pypi.org/project/eule/)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/trouchet/eule/HEAD)
 
 [![codecov](https://codecov.io/gh/trouchet/eule/branch/main/graph/badge.svg?token=PJMBaLIqar)](https://codecov.io/gh/trouchet/eule)
@@ -41,15 +41,15 @@
 
 1. the library: on URL <https://eule.readthedocs.io>;
 2. Euler diagrams: on wikipedia article <https://en.wikipedia.org/wiki/Euler_diagram>
 
 Motivation
 ================
 
-<img src="https://github.com/trouchet/eule/blob/master/images/euler_venn.png?raw=true" width="400" height="364"/>
+<img src="https://github.com/trouchet/eule/blob/main/images/euler_venn.png?raw=true" width="400" height="364"/>
 
 How to install
 ================
 
 We run the command on desired installation environment:
 
 ``` {.bash}
@@ -59,38 +59,45 @@
 Minimal example
 ================
 
 We run command `python example.py` on the folder with file `example.py` and following content:
 
 ``` {.python}
 #!/usr/bin/env python
-from eule import euler
+from eule import euler, euler_keys, euler_boundaries
 
 sets = {
     'a': [1, 2, 3],
     'b': [2, 3, 4],
     'c': [3, 4, 5],
     'd': [3, 5, 6]
 }
 
 euler_diagram = euler(sets)
-euler_keys = euler_keys(sets)
-euler_boundaries = euler_boundaries(sets)
+euler_keys_ = euler_keys(sets)
+euler_boundaries_ = euler_boundaries(sets)
 
 # Euler dictionary: 
-# {'a,b': [2], 'b,c': [4], 'a,b,c,d': [3], 'c,d': [5], 'd': [6], 'a': [1]}
+# {
+#     ('b', 'c'): [4],
+#     ('c', 'd'): [5],
+#     ('a', 'b', 'c', 'd'): [3],
+#     ('d',): [6],
+#     ('a', 'b'): [2],
+#     ('a',): [1]
+# }
 print(euler_diagram)
 
 # Euler keys list:
-# ['a,b', 'b,c', 'a,b,c,d', 'c,d', 'd', 'a']
-print(euler_keys)
+# [('b', 'c'), ('c', 'd'), ('a', 'b', 'c', 'd'), ('d',), ('a', 'b'), ('a',)]
+print(euler_keys_)
 
 # Euler boundaries dictionary: 
 # {
-#   'a': ['b', 'c', 'd'], 
-#   'b': ['a', 'c', 'd'], 
-#   'c': ['a', 'b', 'd'], 
-#   'd': ['a', 'b', 'c']
+#     'a': ['b', 'c', 'd'],
+#     'b': ['a', 'c', 'd'],
+#     'c': ['a', 'b', 'd'],
+#     'd': ['a', 'b', 'c']
 # }
-print(euler_boundaries)
+print(euler_boundaries_)
 ```
```

