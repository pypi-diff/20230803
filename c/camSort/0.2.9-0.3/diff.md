# Comparing `tmp/camSort-0.2.9.tar.gz` & `tmp/camSort-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/camSort-0.2.9.tar", last modified: Thu Aug  3 05:24:10 2023, max compression
+gzip compressed data, was "dist/camSort-0.3.tar", last modified: Thu Aug  3 09:04:30 2023, max compression
```

## Comparing `camSort-0.2.9.tar` & `camSort-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 05:24:10.000000 camSort-0.2.9/
--rw-r--r--   0 macbook    (501) staff       (20)     2435 2023-08-03 05:24:10.000000 camSort-0.2.9/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     1529 2023-08-01 07:52:20.000000 camSort-0.2.9/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort/
--rw-r--r--   0 macbook    (501) staff       (20)   270002 2023-08-03 05:23:07.000000 camSort-0.2.9/camSort/stringSort.c
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     2435 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      208 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       24 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       99 2023-08-02 08:57:15.000000 camSort-0.2.9/pyproject.toml
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-03 05:24:10.000000 camSort-0.2.9/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1043 2023-08-03 05:23:49.000000 camSort-0.2.9/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 09:04:30.000000 camSort-0.3/
+-rw-r--r--   0 macbook    (501) staff       (20)     2891 2023-08-03 09:04:30.000000 camSort-0.3/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     1915 2023-08-03 09:03:34.000000 camSort-0.3/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 09:04:30.000000 camSort-0.3/camSort/
+-rw-r--r--   0 macbook    (501) staff       (20)   331186 2023-08-03 09:04:30.000000 camSort-0.3/camSort/stringSort.c
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 09:04:30.000000 camSort-0.3/camSort.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     2891 2023-08-03 09:04:30.000000 camSort-0.3/camSort.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      208 2023-08-03 09:04:30.000000 camSort-0.3/camSort.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-03 09:04:30.000000 camSort-0.3/camSort.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       24 2023-08-03 09:04:30.000000 camSort-0.3/camSort.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-03 09:04:30.000000 camSort-0.3/camSort.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       99 2023-08-02 08:57:15.000000 camSort-0.3/pyproject.toml
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-03 09:04:30.000000 camSort-0.3/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1052 2023-08-03 09:04:28.000000 camSort-0.3/setup.py
```

### Comparing `camSort-0.2.9/PKG-INFO` & `camSort-0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,65 @@
 Metadata-Version: 2.1
 Name: camSort
-Version: 0.2.9
+Version: 0.3
 Summary: make sorted() fast for strings
 Home-page: UNKNOWN
 Author: ['cameronbae / cameron jay']
 Author-email: <contact@camjay.io>
 License: UNKNOWN
 Description: 
-        # camSort
+        # camSort 0.3!
         
-        Working on `python 3.7.1`!
+        Working on `python 3.7.3`! (at least I think.)
         
         `camSort` is a Python library that makes sorted() look slow while also using sorted(). It's built on Cython, and provides preallocation to string sorting by using a custom key calculation for each string. Normal key calculation and object creation are often computationally expensive—but here we optimize that with Cython >:)!
         
         ## Overview
         
         The `camSort` library sorts a list of strings by creating a custom object for each string. This custom object, `StringWithKey`, holds the string and a unique key calculated from it. The key is a long integer derived from the sum of Unicode code points of the characters in the string, and the string's length.
         
         The actual sorting operation uses Python's built-in `sorted` function (based on Timsort), however, now with precalculated keys, rather than comparing the strings themselves. Making sorting quite faster.
         
         The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance).
         
         ## Installation
         
-        ```pip install camSort``` or compile locally :)
+        ```pip install camSort```, or build locally :)
         
         ## Usage
         
         ```python
-        import camSort
-        # or
         from camSort import sortStrings
         
         myList = ['your', 'list', 'of', 'strings', ':)!']
         
-        sortedStrings = camSort.sortStrings(myList)
-        # or
-        sortedStrings = sortStrings(myList)
+        # By length
+        sortedStrings = sortStrings.byLength(myList)
+        # By alphabetically
+        sortedStringsCam = stringSort.byAlphabet(stringsToGen)
+        # By sorting alphabetically and length
+        sortedStringsCam = stringSort.byLengthAndAlphabet(stringsToGen)
         
         ```
         
         ## Performance
         
+        Try out the demo.py file!
+        
         Average output on my 2017 macbook pro:
             (1 million strings, with a random legnth of 1 to 1000 chararacters)
         
-        Time taken by Python sorted(): 56.08621883392334 seconds
-        Time taken by camSort: 6.356221914291382 seconds
-Keywords: python,sorted,sort,camSort
+        ```
+        Time taken by Python sorted():               57.62033486366272 seconds
+            Using camSort!
+        Time taken sorting by length:                7.040294170379639 seconds
+        By sorting alphabetically:                   3.804348945617676 seconds
+        By sorting alphabetically and length:        7.213421821594238 seconds
+        ```
+Keywords: python,sorted,sort,camSort,reverse
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `camSort-0.2.9/README.md` & `camSort-0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,48 @@
-# camSort
+# camSort 0.3!
 
-Working on `python 3.7.1`!
+Working on `python 3.7.3`! (at least I think.)
 
 `camSort` is a Python library that makes sorted() look slow while also using sorted(). It's built on Cython, and provides preallocation to string sorting by using a custom key calculation for each string. Normal key calculation and object creation are often computationally expensive—but here we optimize that with Cython >:)!
 
 ## Overview
 
 The `camSort` library sorts a list of strings by creating a custom object for each string. This custom object, `StringWithKey`, holds the string and a unique key calculated from it. The key is a long integer derived from the sum of Unicode code points of the characters in the string, and the string's length.
 
 The actual sorting operation uses Python's built-in `sorted` function (based on Timsort), however, now with precalculated keys, rather than comparing the strings themselves. Making sorting quite faster.
 
 The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance).
 
 ## Installation
 
-```pip install camSort``` or compile locally :)
+```pip install camSort```, or build locally :)
 
 ## Usage
 
 ```python
-import camSort
-# or
 from camSort import sortStrings
 
 myList = ['your', 'list', 'of', 'strings', ':)!']
 
-sortedStrings = camSort.sortStrings(myList)
-# or
-sortedStrings = sortStrings(myList)
+# By length
+sortedStrings = sortStrings.byLength(myList)
+# By alphabetically
+sortedStringsCam = stringSort.byAlphabet(stringsToGen)
+# By sorting alphabetically and length
+sortedStringsCam = stringSort.byLengthAndAlphabet(stringsToGen)
 
 ```
 
 ## Performance
 
+Try out the demo.py file!
+
 Average output on my 2017 macbook pro:
     (1 million strings, with a random legnth of 1 to 1000 chararacters)
 
-Time taken by Python sorted(): 56.08621883392334 seconds
-Time taken by camSort: 6.356221914291382 seconds
+```
+Time taken by Python sorted():               57.62033486366272 seconds
+    Using camSort!
+Time taken sorting by length:                7.040294170379639 seconds
+By sorting alphabetically:                   3.804348945617676 seconds
+By sorting alphabetically and length:        7.213421821594238 seconds
+```
```

### Comparing `camSort-0.2.9/camSort/stringSort.c` & `camSort-0.3/camSort/stringSort.c`

 * *Files 9% similar despite different names*

```diff
@@ -827,14 +827,15 @@
 static const char *__pyx_f[] = {
   "camSort/stringSort.pyx",
   "stringsource",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_7camSort_10stringSort_StringWithKey;
+struct __pyx_obj_7camSort_10stringSort_SortedList;
 
 /* "camSort/stringSort.pyx":4
  * from operator import attrgetter
  * 
  * cdef class StringWithKey:             # <<<<<<<<<<<<<<
  *     cdef public:
  *         str str
@@ -843,14 +844,35 @@
   PyObject_HEAD
   struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *__pyx_vtab;
   PyObject *str;
   PyObject *key;
 };
 
 
+/* "camSort/stringSort.pyx":32
+ *         return length * 10000 + self.calculate_key(str)
+ * 
+ * cdef class SortedList:             # <<<<<<<<<<<<<<
+ *     cdef public:
+ *         list str_list
+ */
+struct __pyx_obj_7camSort_10stringSort_SortedList {
+  PyObject_HEAD
+  PyObject *str_list;
+};
+
+
+
+/* "camSort/stringSort.pyx":4
+ * from operator import attrgetter
+ * 
+ * cdef class StringWithKey:             # <<<<<<<<<<<<<<
+ *     cdef public:
+ *         str str
+ */
 
 struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey {
   PY_LONG_LONG (*calculate_key)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *);
   PyObject *(*calculate_key_alpha)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *);
   PY_LONG_LONG (*calculate_key_length_alpha)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *);
 };
 static struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *__pyx_vtabptr_7camSort_10stringSort_StringWithKey;
@@ -1112,14 +1134,43 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
+/* GetItemInt.proto */
+#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
+               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
+#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
+                                                     int is_list, int wraparound, int boundscheck);
+
+/* ObjectGetItem.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
+#else
+#define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
+#endif
+
 /* ListCompAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
@@ -1141,36 +1192,14 @@
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* GetItemInt.proto */
-#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
-    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
-               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
-#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
-                                                     int is_list, int wraparound, int boundscheck);
-
 /* HasAttr.proto */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
@@ -1252,15 +1281,17 @@
 
 static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto*/
 static PyObject *__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_alpha(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto*/
 static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_length_alpha(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto*/
 
 /* Module declarations from 'camSort.stringSort' */
 static PyTypeObject *__pyx_ptype_7camSort_10stringSort_StringWithKey = 0;
+static PyTypeObject *__pyx_ptype_7camSort_10stringSort_SortedList = 0;
 static PyObject *__pyx_f_7camSort_10stringSort___pyx_unpickle_StringWithKey__set_state(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *); /*proto*/
+static PyObject *__pyx_f_7camSort_10stringSort___pyx_unpickle_SortedList__set_state(struct __pyx_obj_7camSort_10stringSort_SortedList *, PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "camSort.stringSort"
 extern int __pyx_module_is_main_camSort__stringSort;
 int __pyx_module_is_main_camSort__stringSort = 0;
 
 /* Implementation of 'camSort.stringSort' */
 static PyObject *__pyx_builtin_sorted;
 static const char __pyx_k_n[] = "n";
@@ -1283,16 +1314,18 @@
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_byLength[] = "byLength";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_key_type[] = "key_type";
 static const char __pyx_k_operator[] = "operator";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
+static const char __pyx_k_str_list[] = "str_list";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
+static const char __pyx_k_SortedList[] = "SortedList";
 static const char __pyx_k_attrgetter[] = "attrgetter";
 static const char __pyx_k_byAlphabet[] = "byAlphabet";
 static const char __pyx_k_input_list[] = "input_list";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
@@ -1303,18 +1336,22 @@
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_length_and_alpha[] = "length_and_alpha";
 static const char __pyx_k_camSort_stringSort[] = "camSort.stringSort";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_byLengthAndAlphabet[] = "byLengthAndAlphabet";
 static const char __pyx_k_camSort_stringSort_pyx[] = "camSort/stringSort.pyx";
+static const char __pyx_k_pyx_unpickle_SortedList[] = "__pyx_unpickle_SortedList";
 static const char __pyx_k_pyx_unpickle_StringWithKey[] = "__pyx_unpickle_StringWithKey";
+static const char __pyx_k_Incompatible_checksums_s_vs_0x2c[] = "Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))";
 static const char __pyx_k_Incompatible_checksums_s_vs_0xef[] = "Incompatible checksums (%s vs 0xef4e75e = (key, str))";
+static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x2c;
 static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xef;
 static PyObject *__pyx_n_s_PickleError;
+static PyObject *__pyx_n_s_SortedList;
 static PyObject *__pyx_n_s_StringWithKey;
 static PyObject *__pyx_n_u_alpha;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_attrgetter;
 static PyObject *__pyx_n_s_byAlphabet;
 static PyObject *__pyx_n_s_byLength;
 static PyObject *__pyx_n_s_byLengthAndAlphabet;
@@ -1338,51 +1375,70 @@
 static PyObject *__pyx_n_s_operator;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
+static PyObject *__pyx_n_s_pyx_unpickle_SortedList;
 static PyObject *__pyx_n_s_pyx_unpickle_StringWithKey;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_s;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_sorted;
 static PyObject *__pyx_n_s_sorted_array;
 static PyObject *__pyx_n_s_str;
+static PyObject *__pyx_n_s_str_list;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_update;
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str, PyObject *__pyx_v_key_type); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_3str___get__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_2__set__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_4__del__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_3key___get__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_2__set__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_4__del__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_2__reduce_cython__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_4__setstate_cython__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_7camSort_10stringSort_10SortedList___init__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_str_list); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_2reverse(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_4__getitem__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_index); /* proto */
+static Py_ssize_t __pyx_pf_7camSort_10stringSort_10SortedList_6__len__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_8__iter__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_8str_list___get__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
+static int __pyx_pf_7camSort_10stringSort_10SortedList_8str_list_2__set__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static int __pyx_pf_7camSort_10stringSort_10SortedList_8str_list_4__del__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_10__reduce_cython__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_12__setstate_cython__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_byLength(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_2byLengthAndAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_4byAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_6__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_8__pyx_unpickle_SortedList(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_7camSort_10stringSort_StringWithKey(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_7camSort_10stringSort_SortedList(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_int_46947008;
 static PyObject *__pyx_int_250931038;
-static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_codeobj__2;
-static PyObject *__pyx_codeobj__4;
-static PyObject *__pyx_codeobj__6;
-static PyObject *__pyx_codeobj__8;
+static PyObject *__pyx_int_neg_1;
+static PyObject *__pyx_slice_;
+static PyObject *__pyx_tuple__2;
+static PyObject *__pyx_tuple__4;
+static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_tuple__8;
+static PyObject *__pyx_tuple__10;
+static PyObject *__pyx_codeobj__3;
+static PyObject *__pyx_codeobj__5;
+static PyObject *__pyx_codeobj__7;
+static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_codeobj__11;
 /* Late includes */
 
 /* "camSort/stringSort.pyx":9
  *         object key  # Changed from long long to object
  * 
  *     def __init__(self, str, key_type='length'):             # <<<<<<<<<<<<<<
  *         self.str = str
@@ -1831,15 +1887,15 @@
   __pyx_v_length = __pyx_t_1;
 
   /* "camSort/stringSort.pyx":30
  *     cdef long long calculate_key_length_alpha(self, str):
  *         cdef int length = len(str)
  *         return length * 10000 + self.calculate_key(str)             # <<<<<<<<<<<<<<
  * 
- * def byLength(input_list):
+ * cdef class SortedList:
  */
   __pyx_r = ((__pyx_v_length * 0x2710) + ((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key(__pyx_v_self, __pyx_v_str));
   goto __pyx_L0;
 
   /* "camSort/stringSort.pyx":28
  *         return str.lower()
  * 
@@ -2363,16 +2419,801 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":32
- *         return length * 10000 + self.calculate_key(str)
+/* "camSort/stringSort.pyx":36
+ *         list str_list
+ * 
+ *     def __init__(self, str_list):             # <<<<<<<<<<<<<<
+ *         self.str_list = str_list
+ * 
+ */
+
+/* Python wrapper */
+static int __pyx_pw_7camSort_10stringSort_10SortedList_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_7camSort_10stringSort_10SortedList_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_str_list = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_str_list,0};
+    PyObject* values[1] = {0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_str_list)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 36, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+    }
+    __pyx_v_str_list = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 36, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return -1;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList___init__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), __pyx_v_str_list);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_7camSort_10stringSort_10SortedList___init__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_str_list) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__init__", 0);
+
+  /* "camSort/stringSort.pyx":37
+ * 
+ *     def __init__(self, str_list):
+ *         self.str_list = str_list             # <<<<<<<<<<<<<<
+ * 
+ *     def reverse(self):
+ */
+  if (!(likely(PyList_CheckExact(__pyx_v_str_list))||((__pyx_v_str_list) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_v_str_list)->tp_name), 0))) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_1 = __pyx_v_str_list;
+  __Pyx_INCREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v_self->str_list);
+  __Pyx_DECREF(__pyx_v_self->str_list);
+  __pyx_v_self->str_list = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "camSort/stringSort.pyx":36
+ *         list str_list
+ * 
+ *     def __init__(self, str_list):             # <<<<<<<<<<<<<<
+ *         self.str_list = str_list
+ * 
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "camSort/stringSort.pyx":39
+ *         self.str_list = str_list
+ * 
+ *     def reverse(self):             # <<<<<<<<<<<<<<
+ *         # same as: self.str_list.reverse()
+ *         self.str_list = self.str_list[::-1]
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_3reverse(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_3reverse(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("reverse (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_2reverse(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_2reverse(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("reverse", 0);
+
+  /* "camSort/stringSort.pyx":41
+ *     def reverse(self):
+ *         # same as: self.str_list.reverse()
+ *         self.str_list = self.str_list[::-1]             # <<<<<<<<<<<<<<
+ *         return self.str_list
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->str_list, __pyx_slice_); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v_self->str_list);
+  __Pyx_DECREF(__pyx_v_self->str_list);
+  __pyx_v_self->str_list = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "camSort/stringSort.pyx":42
+ *         # same as: self.str_list.reverse()
+ *         self.str_list = self.str_list[::-1]
+ *         return self.str_list             # <<<<<<<<<<<<<<
+ * 
+ *     def __getitem__(self, index):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->str_list);
+  __pyx_r = __pyx_v_self->str_list;
+  goto __pyx_L0;
+
+  /* "camSort/stringSort.pyx":39
+ *         self.str_list = str_list
+ * 
+ *     def reverse(self):             # <<<<<<<<<<<<<<
+ *         # same as: self.str_list.reverse()
+ *         self.str_list = self.str_list[::-1]
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.reverse", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "camSort/stringSort.pyx":44
+ *         return self.str_list
+ * 
+ *     def __getitem__(self, index):             # <<<<<<<<<<<<<<
+ *         return self.str_list[index]
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_5__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_index); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_5__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_index) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__getitem__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_4__getitem__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), ((PyObject *)__pyx_v_index));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_4__getitem__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_index) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__getitem__", 0);
+
+  /* "camSort/stringSort.pyx":45
+ * 
+ *     def __getitem__(self, index):
+ *         return self.str_list[index]             # <<<<<<<<<<<<<<
+ * 
+ *     def __len__(self):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  if (unlikely(__pyx_v_self->str_list == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(0, 45, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->str_list, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "camSort/stringSort.pyx":44
+ *         return self.str_list
+ * 
+ *     def __getitem__(self, index):             # <<<<<<<<<<<<<<
+ *         return self.str_list[index]
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "camSort/stringSort.pyx":47
+ *         return self.str_list[index]
+ * 
+ *     def __len__(self):             # <<<<<<<<<<<<<<
+ *         return len(self.str_list)
+ * 
+ */
+
+/* Python wrapper */
+static Py_ssize_t __pyx_pw_7camSort_10stringSort_10SortedList_7__len__(PyObject *__pyx_v_self); /*proto*/
+static Py_ssize_t __pyx_pw_7camSort_10stringSort_10SortedList_7__len__(PyObject *__pyx_v_self) {
+  Py_ssize_t __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__len__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_6__len__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static Py_ssize_t __pyx_pf_7camSort_10stringSort_10SortedList_6__len__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
+  Py_ssize_t __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__len__", 0);
+
+  /* "camSort/stringSort.pyx":48
+ * 
+ *     def __len__(self):
+ *         return len(self.str_list)             # <<<<<<<<<<<<<<
+ * 
+ *     def __iter__(self):
+ */
+  __pyx_t_1 = __pyx_v_self->str_list;
+  __Pyx_INCREF(__pyx_t_1);
+  if (unlikely(__pyx_t_1 == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(0, 48, __pyx_L1_error)
+  }
+  __pyx_t_2 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 48, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_2;
+  goto __pyx_L0;
+
+  /* "camSort/stringSort.pyx":47
+ *         return self.str_list[index]
+ * 
+ *     def __len__(self):             # <<<<<<<<<<<<<<
+ *         return len(self.str_list)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "camSort/stringSort.pyx":50
+ *         return len(self.str_list)
+ * 
+ *     def __iter__(self):             # <<<<<<<<<<<<<<
+ *         return iter(self.str_list)
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_9__iter__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_9__iter__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__iter__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_8__iter__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_8__iter__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__iter__", 0);
+
+  /* "camSort/stringSort.pyx":51
+ * 
+ *     def __iter__(self):
+ *         return iter(self.str_list)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __pyx_v_self->str_list;
+  __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "camSort/stringSort.pyx":50
+ *         return len(self.str_list)
+ * 
+ *     def __iter__(self):             # <<<<<<<<<<<<<<
+ *         return iter(self.str_list)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.__iter__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "camSort/stringSort.pyx":34
+ * cdef class SortedList:
+ *     cdef public:
+ *         list str_list             # <<<<<<<<<<<<<<
+ * 
+ *     def __init__(self, str_list):
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_8str_list_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_8str_list_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_8str_list___get__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_8str_list___get__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->str_list);
+  __pyx_r = __pyx_v_self->str_list;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_7camSort_10stringSort_10SortedList_8str_list_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_7camSort_10stringSort_10SortedList_8str_list_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_8str_list_2__set__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_7camSort_10stringSort_10SortedList_8str_list_2__set__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__set__", 0);
+  if (!(likely(PyList_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __pyx_v_value;
+  __Pyx_INCREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v_self->str_list);
+  __Pyx_DECREF(__pyx_v_self->str_list);
+  __pyx_v_self->str_list = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.str_list.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_7camSort_10stringSort_10SortedList_8str_list_5__del__(PyObject *__pyx_v_self); /*proto*/
+static int __pyx_pw_7camSort_10stringSort_10SortedList_8str_list_5__del__(PyObject *__pyx_v_self) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_8str_list_4__del__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_7camSort_10stringSort_10SortedList_8str_list_4__del__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__", 0);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  __Pyx_GOTREF(__pyx_v_self->str_list);
+  __Pyx_DECREF(__pyx_v_self->str_list);
+  __pyx_v_self->str_list = ((PyObject*)Py_None);
+
+  /* function exit code */
+  __pyx_r = 0;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_10__reduce_cython__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_10__reduce_cython__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self) {
+  PyObject *__pyx_v_state = 0;
+  PyObject *__pyx_v__dict = 0;
+  int __pyx_v_use_setstate;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+
+  /* "(tree fragment)":5
+ *     cdef object _dict
+ *     cdef bint use_setstate
+ *     state = (self.str_list,)             # <<<<<<<<<<<<<<
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ */
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_v_self->str_list);
+  __Pyx_GIVEREF(__pyx_v_self->str_list);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_self->str_list);
+  __pyx_v_state = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "(tree fragment)":6
+ *     cdef bint use_setstate
+ *     state = (self.str_list,)
+ *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
+ *     if _dict is not None:
+ *         state += (_dict,)
+ */
+  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v__dict = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "(tree fragment)":7
+ *     state = (self.str_list,)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+  __pyx_t_2 = (__pyx_v__dict != Py_None);
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":8
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ *         state += (_dict,)             # <<<<<<<<<<<<<<
+ *         use_setstate = True
+ *     else:
+ */
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_v__dict);
+    __Pyx_GIVEREF(__pyx_v__dict);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict);
+    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_4));
+    __pyx_t_4 = 0;
+
+    /* "(tree fragment)":9
+ *     if _dict is not None:
+ *         state += (_dict,)
+ *         use_setstate = True             # <<<<<<<<<<<<<<
+ *     else:
+ *         use_setstate = self.str_list is not None
+ */
+    __pyx_v_use_setstate = 1;
+
+    /* "(tree fragment)":7
+ *     state = (self.str_list,)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+    goto __pyx_L3;
+  }
+
+  /* "(tree fragment)":11
+ *         use_setstate = True
+ *     else:
+ *         use_setstate = self.str_list is not None             # <<<<<<<<<<<<<<
+ *     if use_setstate:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, None), state
+ */
+  /*else*/ {
+    __pyx_t_3 = (__pyx_v_self->str_list != ((PyObject*)Py_None));
+    __pyx_v_use_setstate = __pyx_t_3;
+  }
+  __pyx_L3:;
+
+  /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = self.str_list is not None
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, None), state
+ *     else:
+ */
+  __pyx_t_3 = (__pyx_v_use_setstate != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":13
+ *         use_setstate = self.str_list is not None
+ *     if use_setstate:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, None), state             # <<<<<<<<<<<<<<
+ *     else:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, state)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_SortedList); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_46947008);
+    __Pyx_GIVEREF(__pyx_int_46947008);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_46947008);
+    __Pyx_INCREF(Py_None);
+    __Pyx_GIVEREF(Py_None);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None);
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_state);
+    __pyx_t_4 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_5;
+    __pyx_t_5 = 0;
+    goto __pyx_L0;
+
+    /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = self.str_list is not None
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, None), state
+ *     else:
+ */
+  }
+
+  /* "(tree fragment)":15
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, None), state
+ *     else:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, state)             # <<<<<<<<<<<<<<
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_SortedList__set_state(self, __pyx_state)
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle_SortedList); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_46947008);
+    __Pyx_GIVEREF(__pyx_int_46947008);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_46947008);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_5 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_4;
+    __pyx_t_4 = 0;
+    goto __pyx_L0;
+  }
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_state);
+  __Pyx_XDECREF(__pyx_v__dict);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_SortedList__set_state(self, __pyx_state)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_10SortedList_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_10SortedList_12__setstate_cython__(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7camSort_10stringSort_10SortedList_12__setstate_cython__(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+
+  /* "(tree fragment)":17
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, state)
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_SortedList__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
+ */
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7camSort_10stringSort___pyx_unpickle_SortedList__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_SortedList, (type(self), 0x2cc5ac0, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_SortedList__set_state(self, __pyx_state)
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("camSort.stringSort.SortedList.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "camSort/stringSort.pyx":54
+ * 
  * 
  * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
 
 /* Python wrapper */
@@ -2405,202 +3246,205 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("byLength", 0);
 
-  /* "camSort/stringSort.pyx":33
+  /* "camSort/stringSort.pyx":55
  * 
  * def byLength(input_list):
  *     cdef int n = len(input_list)             # <<<<<<<<<<<<<<
  *     cdef list array = [StringWithKey(s) for s in input_list]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 55, __pyx_L1_error)
   __pyx_v_n = __pyx_t_1;
 
-  /* "camSort/stringSort.pyx":34
+  /* "camSort/stringSort.pyx":56
  * def byLength(input_list):
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]             # <<<<<<<<<<<<<<
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))
  */
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L5_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (likely(PyList_CheckExact(__pyx_v_input_list)) || PyTuple_CheckExact(__pyx_v_input_list)) {
       __pyx_t_3 = __pyx_v_input_list; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L5_error)
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L5_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 34, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 56, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 34, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 56, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_3);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 34, __pyx_L5_error)
+            else __PYX_ERR(0, 56, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_s, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_7genexpr__pyx_v_s); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L5_error)
+      __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_7genexpr__pyx_v_s); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 34, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 56, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_s); __pyx_7genexpr__pyx_v_s = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_s); __pyx_7genexpr__pyx_v_s = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_array = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":36
+  /* "camSort/stringSort.pyx":58
  *     cdef list array = [StringWithKey(s) for s in input_list]
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))             # <<<<<<<<<<<<<<
- *     return [s.str for s in sorted_array]
+ *     return SortedList([s.str for s in sorted_array])
  * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_array);
   __Pyx_GIVEREF(__pyx_v_array);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_array);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_n_u_key) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_n_u_key);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_5) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_5) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_sorted_array = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "camSort/stringSort.pyx":37
+  /* "camSort/stringSort.pyx":59
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))
- *     return [s.str for s in sorted_array]             # <<<<<<<<<<<<<<
+ *     return SortedList([s.str for s in sorted_array])             # <<<<<<<<<<<<<<
  * 
  * def byLengthAndAlphabet(input_list):
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L11_error)
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (likely(PyList_CheckExact(__pyx_v_sorted_array)) || PyTuple_CheckExact(__pyx_v_sorted_array)) {
       __pyx_t_3 = __pyx_v_sorted_array; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L11_error)
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L11_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 59, __pyx_L11_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 37, __pyx_L11_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 59, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L11_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 37, __pyx_L11_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 59, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L11_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_4(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 37, __pyx_L11_error)
+            else __PYX_ERR(0, 59, __pyx_L11_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_s, __pyx_t_2);
       __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L11_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 37, __pyx_L11_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 59, __pyx_L11_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_s); __pyx_8genexpr1__pyx_v_s = 0;
     goto __pyx_L14_exit_scope;
     __pyx_L11_error:;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_s); __pyx_8genexpr1__pyx_v_s = 0;
     goto __pyx_L1_error;
     __pyx_L14_exit_scope:;
   } /* exit inner scope */
-  __pyx_r = __pyx_t_5;
-  __pyx_t_5 = 0;
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_SortedList), __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":32
- *         return length * 10000 + self.calculate_key(str)
+  /* "camSort/stringSort.pyx":54
+ * 
  * 
  * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
 
   /* function exit code */
@@ -2618,16 +3462,16 @@
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_s);
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":39
- *     return [s.str for s in sorted_array]
+/* "camSort/stringSort.pyx":61
+ *     return SortedList([s.str for s in sorted_array])
  * 
  * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
  */
 
 /* Python wrapper */
@@ -2660,211 +3504,214 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("byLengthAndAlphabet", 0);
 
-  /* "camSort/stringSort.pyx":40
+  /* "camSort/stringSort.pyx":62
  * 
  * def byLengthAndAlphabet(input_list):
  *     cdef int n = len(input_list)             # <<<<<<<<<<<<<<
  *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 62, __pyx_L1_error)
   __pyx_v_n = __pyx_t_1;
 
-  /* "camSort/stringSort.pyx":41
+  /* "camSort/stringSort.pyx":63
  * def byLengthAndAlphabet(input_list):
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]             # <<<<<<<<<<<<<<
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))
  */
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L5_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (likely(PyList_CheckExact(__pyx_v_input_list)) || PyTuple_CheckExact(__pyx_v_input_list)) {
       __pyx_t_3 = __pyx_v_input_list; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L5_error)
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L5_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 41, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 63, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 41, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 63, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_3);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 41, __pyx_L5_error)
+            else __PYX_ERR(0, 63, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_s, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L5_error)
+      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_8genexpr2__pyx_v_s);
       __Pyx_GIVEREF(__pyx_8genexpr2__pyx_v_s);
       PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_8genexpr2__pyx_v_s);
       __Pyx_INCREF(__pyx_n_u_length_and_alpha);
       __Pyx_GIVEREF(__pyx_n_u_length_and_alpha);
       PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_n_u_length_and_alpha);
-      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 41, __pyx_L5_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 63, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 41, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 63, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_s); __pyx_8genexpr2__pyx_v_s = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_s); __pyx_8genexpr2__pyx_v_s = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_array = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":43
+  /* "camSort/stringSort.pyx":65
  *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))             # <<<<<<<<<<<<<<
- *     return [s.str for s in sorted_array]
+ *     return SortedList([s.str for s in sorted_array])
  * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_array);
   __Pyx_GIVEREF(__pyx_v_array);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_array);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_n_u_key) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_u_key);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 43, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_6) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_6) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_sorted_array = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "camSort/stringSort.pyx":44
+  /* "camSort/stringSort.pyx":66
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))
- *     return [s.str for s in sorted_array]             # <<<<<<<<<<<<<<
+ *     return SortedList([s.str for s in sorted_array])             # <<<<<<<<<<<<<<
  * 
  * def byAlphabet(input_list):
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 44, __pyx_L11_error)
+    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 66, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (likely(PyList_CheckExact(__pyx_v_sorted_array)) || PyTuple_CheckExact(__pyx_v_sorted_array)) {
       __pyx_t_3 = __pyx_v_sorted_array; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L11_error)
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L11_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L11_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 44, __pyx_L11_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 66, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L11_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 44, __pyx_L11_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 66, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L11_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_4(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 44, __pyx_L11_error)
+            else __PYX_ERR(0, 66, __pyx_L11_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_s, __pyx_t_2);
       __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr3__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L11_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr3__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 44, __pyx_L11_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 66, __pyx_L11_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_s); __pyx_8genexpr3__pyx_v_s = 0;
     goto __pyx_L14_exit_scope;
     __pyx_L11_error:;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_s); __pyx_8genexpr3__pyx_v_s = 0;
     goto __pyx_L1_error;
     __pyx_L14_exit_scope:;
   } /* exit inner scope */
-  __pyx_r = __pyx_t_6;
-  __pyx_t_6 = 0;
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_SortedList), __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":39
- *     return [s.str for s in sorted_array]
+  /* "camSort/stringSort.pyx":61
+ *     return SortedList([s.str for s in sorted_array])
  * 
  * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
  */
 
   /* function exit code */
@@ -2882,16 +3729,16 @@
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_s);
   __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":46
- *     return [s.str for s in sorted_array]
+/* "camSort/stringSort.pyx":68
+ *     return SortedList([s.str for s in sorted_array])
  * 
  * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
  */
 
 /* Python wrapper */
@@ -2924,210 +3771,211 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("byAlphabet", 0);
 
-  /* "camSort/stringSort.pyx":47
+  /* "camSort/stringSort.pyx":69
  * 
  * def byAlphabet(input_list):
  *     cdef int n = len(input_list)             # <<<<<<<<<<<<<<
  *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 69, __pyx_L1_error)
   __pyx_v_n = __pyx_t_1;
 
-  /* "camSort/stringSort.pyx":48
+  /* "camSort/stringSort.pyx":70
  * def byAlphabet(input_list):
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]             # <<<<<<<<<<<<<<
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))
  */
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L5_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (likely(PyList_CheckExact(__pyx_v_input_list)) || PyTuple_CheckExact(__pyx_v_input_list)) {
       __pyx_t_3 = __pyx_v_input_list; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L5_error)
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L5_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 48, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 70, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 48, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 70, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_3);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 48, __pyx_L5_error)
+            else __PYX_ERR(0, 70, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr4__pyx_v_s, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L5_error)
+      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_8genexpr4__pyx_v_s);
       __Pyx_GIVEREF(__pyx_8genexpr4__pyx_v_s);
       PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_8genexpr4__pyx_v_s);
       __Pyx_INCREF(__pyx_n_u_alpha);
       __Pyx_GIVEREF(__pyx_n_u_alpha);
       PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_n_u_alpha);
-      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 48, __pyx_L5_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 70, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 48, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 70, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_s); __pyx_8genexpr4__pyx_v_s = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_s); __pyx_8genexpr4__pyx_v_s = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_array = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":50
+  /* "camSort/stringSort.pyx":72
  *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))             # <<<<<<<<<<<<<<
- *     return [s.str for s in sorted_array]
- * 
+ *     return SortedList([s.str for s in sorted_array])
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_array);
   __Pyx_GIVEREF(__pyx_v_array);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_array);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_n_u_key) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_u_key);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 50, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_6) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_6) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_sorted_array = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "camSort/stringSort.pyx":51
+  /* "camSort/stringSort.pyx":73
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))
- *     return [s.str for s in sorted_array]             # <<<<<<<<<<<<<<
- * 
+ *     return SortedList([s.str for s in sorted_array])             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 51, __pyx_L11_error)
+    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (likely(PyList_CheckExact(__pyx_v_sorted_array)) || PyTuple_CheckExact(__pyx_v_sorted_array)) {
       __pyx_t_3 = __pyx_v_sorted_array; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L11_error)
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L11_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L11_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 51, __pyx_L11_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 73, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L11_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 51, __pyx_L11_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 73, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L11_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_4(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 51, __pyx_L11_error)
+            else __PYX_ERR(0, 73, __pyx_L11_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr5__pyx_v_s, __pyx_t_2);
       __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr5__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L11_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr5__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 51, __pyx_L11_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 73, __pyx_L11_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_s); __pyx_8genexpr5__pyx_v_s = 0;
     goto __pyx_L14_exit_scope;
     __pyx_L11_error:;
     __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_s); __pyx_8genexpr5__pyx_v_s = 0;
     goto __pyx_L1_error;
     __pyx_L14_exit_scope:;
   } /* exit inner scope */
-  __pyx_r = __pyx_t_6;
-  __pyx_t_6 = 0;
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_SortedList), __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":46
- *     return [s.str for s in sorted_array]
+  /* "camSort/stringSort.pyx":68
+ *     return SortedList([s.str for s in sorted_array])
  * 
  * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
  */
 
   /* function exit code */
@@ -3553,14 +4401,412 @@
   __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_StringWithKey__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
+
+/* "(tree fragment)":1
+ * def __pyx_unpickle_SortedList(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7camSort_10stringSort_9__pyx_unpickle_SortedList(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_9__pyx_unpickle_SortedList = {"__pyx_unpickle_SortedList", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7camSort_10stringSort_9__pyx_unpickle_SortedList, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_9__pyx_unpickle_SortedList(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v___pyx_type = 0;
+  long __pyx_v___pyx_checksum;
+  PyObject *__pyx_v___pyx_state = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__pyx_unpickle_SortedList (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
+    PyObject* values[3] = {0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_type)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_SortedList", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_SortedList", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle_SortedList") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+    }
+    __pyx_v___pyx_type = values[0];
+    __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
+    __pyx_v___pyx_state = values[2];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_SortedList", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_SortedList", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7camSort_10stringSort_8__pyx_unpickle_SortedList(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7camSort_10stringSort_8__pyx_unpickle_SortedList(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_v___pyx_PickleError = 0;
+  PyObject *__pyx_v___pyx_result = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_SortedList", 0);
+
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum != 0x2cc5ac0:             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ */
+  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x2cc5ac0) != 0);
+  if (__pyx_t_1) {
+
+    /* "(tree fragment)":5
+ *     cdef object __pyx_result
+ *     if __pyx_checksum != 0x2cc5ac0:
+ *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ *     __pyx_result = SortedList.__new__(__pyx_type)
+ */
+    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(__pyx_n_s_PickleError);
+    __Pyx_GIVEREF(__pyx_n_s_PickleError);
+    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
+    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(__pyx_t_2);
+    __pyx_v___pyx_PickleError = __pyx_t_2;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "(tree fragment)":6
+ *     if __pyx_checksum != 0x2cc5ac0:
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *     __pyx_result = SortedList.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ */
+    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x2c, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_INCREF(__pyx_v___pyx_PickleError);
+    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
+      }
+    }
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __PYX_ERR(1, 6, __pyx_L1_error)
+
+    /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum != 0x2cc5ac0:             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ */
+  }
+
+  /* "(tree fragment)":7
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ *     __pyx_result = SortedList.__new__(__pyx_type)             # <<<<<<<<<<<<<<
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ */
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7camSort_10stringSort_SortedList), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v___pyx_result = __pyx_t_3;
+  __pyx_t_3 = 0;
+
+  /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ *     __pyx_result = SortedList.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_6 = (__pyx_t_1 != 0);
+  if (__pyx_t_6) {
+
+    /* "(tree fragment)":9
+ *     __pyx_result = SortedList.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
+ *     return __pyx_result
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):
+ */
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_7camSort_10stringSort___pyx_unpickle_SortedList__set_state(((struct __pyx_obj_7camSort_10stringSort_SortedList *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2cc5ac0 = (str_list))" % __pyx_checksum)
+ *     __pyx_result = SortedList.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  }
+
+  /* "(tree fragment)":10
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ *     return __pyx_result             # <<<<<<<<<<<<<<
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_list = __pyx_state[0]
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v___pyx_result);
+  __pyx_r = __pyx_v___pyx_result;
+  goto __pyx_L0;
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_SortedList(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_SortedList", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v___pyx_PickleError);
+  __Pyx_XDECREF(__pyx_v___pyx_result);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":11
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.str_list = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ */
+
+static PyObject *__pyx_f_7camSort_10stringSort___pyx_unpickle_SortedList__set_state(struct __pyx_obj_7camSort_10stringSort_SortedList *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  int __pyx_t_4;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_SortedList__set_state", 0);
+
+  /* "(tree fragment)":12
+ *     return __pyx_result
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_list = __pyx_state[0]             # <<<<<<<<<<<<<<
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[1])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (!(likely(PyList_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->str_list);
+  __Pyx_DECREF(__pyx_v___pyx_result->str_list);
+  __pyx_v___pyx_result->str_list = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "(tree fragment)":13
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_list = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[1])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(1, 13, __pyx_L1_error)
+  }
+  __pyx_t_3 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_4 = ((__pyx_t_3 > 1) != 0);
+  if (__pyx_t_4) {
+  } else {
+    __pyx_t_2 = __pyx_t_4;
+    goto __pyx_L4_bool_binop_done;
+  }
+  __pyx_t_4 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_4 != 0);
+  __pyx_t_2 = __pyx_t_5;
+  __pyx_L4_bool_binop_done:;
+  if (__pyx_t_2) {
+
+    /* "(tree fragment)":14
+ *     __pyx_result.str_list = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[1])             # <<<<<<<<<<<<<<
+ */
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(__pyx_v___pyx_state == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(1, 14, __pyx_L1_error)
+    }
+    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_8 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_8);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "(tree fragment)":13
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_list = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[1])
+ */
+  }
+
+  /* "(tree fragment)":11
+ *         __pyx_unpickle_SortedList__set_state(<SortedList> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_SortedList__set_state(SortedList __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.str_list = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_SortedList__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
 static struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey __pyx_vtable_7camSort_10stringSort_StringWithKey;
 
 static PyObject *__pyx_tp_new_7camSort_10stringSort_StringWithKey(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7camSort_10stringSort_StringWithKey *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
@@ -3709,14 +4955,178 @@
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
 };
 
+static PyObject *__pyx_tp_new_7camSort_10stringSort_SortedList(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_7camSort_10stringSort_SortedList *p;
+  PyObject *o;
+  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
+    o = (*t->tp_alloc)(t, 0);
+  } else {
+    o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
+  }
+  if (unlikely(!o)) return 0;
+  p = ((struct __pyx_obj_7camSort_10stringSort_SortedList *)o);
+  p->str_list = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  return o;
+}
+
+static void __pyx_tp_dealloc_7camSort_10stringSort_SortedList(PyObject *o) {
+  struct __pyx_obj_7camSort_10stringSort_SortedList *p = (struct __pyx_obj_7camSort_10stringSort_SortedList *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+    if (PyObject_CallFinalizerFromDealloc(o)) return;
+  }
+  #endif
+  PyObject_GC_UnTrack(o);
+  Py_CLEAR(p->str_list);
+  (*Py_TYPE(o)->tp_free)(o);
+}
+
+static int __pyx_tp_traverse_7camSort_10stringSort_SortedList(PyObject *o, visitproc v, void *a) {
+  int e;
+  struct __pyx_obj_7camSort_10stringSort_SortedList *p = (struct __pyx_obj_7camSort_10stringSort_SortedList *)o;
+  if (p->str_list) {
+    e = (*v)(p->str_list, a); if (e) return e;
+  }
+  return 0;
+}
+
+static int __pyx_tp_clear_7camSort_10stringSort_SortedList(PyObject *o) {
+  PyObject* tmp;
+  struct __pyx_obj_7camSort_10stringSort_SortedList *p = (struct __pyx_obj_7camSort_10stringSort_SortedList *)o;
+  tmp = ((PyObject*)p->str_list);
+  p->str_list = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  return 0;
+}
+static PyObject *__pyx_sq_item_7camSort_10stringSort_SortedList(PyObject *o, Py_ssize_t i) {
+  PyObject *r;
+  PyObject *x = PyInt_FromSsize_t(i); if(!x) return 0;
+  r = Py_TYPE(o)->tp_as_mapping->mp_subscript(o, x);
+  Py_DECREF(x);
+  return r;
+}
+
+static PyObject *__pyx_getprop_7camSort_10stringSort_10SortedList_str_list(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7camSort_10stringSort_10SortedList_8str_list_1__get__(o);
+}
+
+static int __pyx_setprop_7camSort_10stringSort_10SortedList_str_list(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_7camSort_10stringSort_10SortedList_8str_list_3__set__(o, v);
+  }
+  else {
+    return __pyx_pw_7camSort_10stringSort_10SortedList_8str_list_5__del__(o);
+  }
+}
+
+static PyMethodDef __pyx_methods_7camSort_10stringSort_SortedList[] = {
+  {"reverse", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_3reverse, METH_NOARGS, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_11__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_7camSort_10stringSort_10SortedList_13__setstate_cython__, METH_O, 0},
+  {0, 0, 0, 0}
+};
+
+static struct PyGetSetDef __pyx_getsets_7camSort_10stringSort_SortedList[] = {
+  {(char *)"str_list", __pyx_getprop_7camSort_10stringSort_10SortedList_str_list, __pyx_setprop_7camSort_10stringSort_10SortedList_str_list, (char *)0, 0},
+  {0, 0, 0, 0, 0}
+};
+
+static PySequenceMethods __pyx_tp_as_sequence_SortedList = {
+  __pyx_pw_7camSort_10stringSort_10SortedList_7__len__, /*sq_length*/
+  0, /*sq_concat*/
+  0, /*sq_repeat*/
+  __pyx_sq_item_7camSort_10stringSort_SortedList, /*sq_item*/
+  0, /*sq_slice*/
+  0, /*sq_ass_item*/
+  0, /*sq_ass_slice*/
+  0, /*sq_contains*/
+  0, /*sq_inplace_concat*/
+  0, /*sq_inplace_repeat*/
+};
+
+static PyMappingMethods __pyx_tp_as_mapping_SortedList = {
+  __pyx_pw_7camSort_10stringSort_10SortedList_7__len__, /*mp_length*/
+  __pyx_pw_7camSort_10stringSort_10SortedList_5__getitem__, /*mp_subscript*/
+  0, /*mp_ass_subscript*/
+};
+
+static PyTypeObject __pyx_type_7camSort_10stringSort_SortedList = {
+  PyVarObject_HEAD_INIT(0, 0)
+  "camSort.stringSort.SortedList", /*tp_name*/
+  sizeof(struct __pyx_obj_7camSort_10stringSort_SortedList), /*tp_basicsize*/
+  0, /*tp_itemsize*/
+  __pyx_tp_dealloc_7camSort_10stringSort_SortedList, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
+  0, /*tp_getattr*/
+  0, /*tp_setattr*/
+  #if PY_MAJOR_VERSION < 3
+  0, /*tp_compare*/
+  #endif
+  #if PY_MAJOR_VERSION >= 3
+  0, /*tp_as_async*/
+  #endif
+  0, /*tp_repr*/
+  0, /*tp_as_number*/
+  &__pyx_tp_as_sequence_SortedList, /*tp_as_sequence*/
+  &__pyx_tp_as_mapping_SortedList, /*tp_as_mapping*/
+  0, /*tp_hash*/
+  0, /*tp_call*/
+  0, /*tp_str*/
+  0, /*tp_getattro*/
+  0, /*tp_setattro*/
+  0, /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
+  0, /*tp_doc*/
+  __pyx_tp_traverse_7camSort_10stringSort_SortedList, /*tp_traverse*/
+  __pyx_tp_clear_7camSort_10stringSort_SortedList, /*tp_clear*/
+  0, /*tp_richcompare*/
+  0, /*tp_weaklistoffset*/
+  __pyx_pw_7camSort_10stringSort_10SortedList_9__iter__, /*tp_iter*/
+  0, /*tp_iternext*/
+  __pyx_methods_7camSort_10stringSort_SortedList, /*tp_methods*/
+  0, /*tp_members*/
+  __pyx_getsets_7camSort_10stringSort_SortedList, /*tp_getset*/
+  0, /*tp_base*/
+  0, /*tp_dict*/
+  0, /*tp_descr_get*/
+  0, /*tp_descr_set*/
+  0, /*tp_dictoffset*/
+  __pyx_pw_7camSort_10stringSort_10SortedList_1__init__, /*tp_init*/
+  0, /*tp_alloc*/
+  __pyx_tp_new_7camSort_10stringSort_SortedList, /*tp_new*/
+  0, /*tp_free*/
+  0, /*tp_is_gc*/
+  0, /*tp_bases*/
+  0, /*tp_mro*/
+  0, /*tp_cache*/
+  0, /*tp_subclasses*/
+  0, /*tp_weaklist*/
+  0, /*tp_del*/
+  0, /*tp_version_tag*/
+  #if PY_VERSION_HEX >= 0x030400a1
+  0, /*tp_finalize*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1
+  0, /*tp_vectorcall*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  0, /*tp_print*/
+  #endif
+};
+
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
@@ -3755,16 +5165,18 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
+  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x2c, __pyx_k_Incompatible_checksums_s_vs_0x2c, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x2c), 0, 0, 1, 0},
   {&__pyx_kp_s_Incompatible_checksums_s_vs_0xef, __pyx_k_Incompatible_checksums_s_vs_0xef, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xef), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
+  {&__pyx_n_s_SortedList, __pyx_k_SortedList, sizeof(__pyx_k_SortedList), 0, 0, 1, 1},
   {&__pyx_n_s_StringWithKey, __pyx_k_StringWithKey, sizeof(__pyx_k_StringWithKey), 0, 0, 1, 1},
   {&__pyx_n_u_alpha, __pyx_k_alpha, sizeof(__pyx_k_alpha), 0, 1, 0, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_attrgetter, __pyx_k_attrgetter, sizeof(__pyx_k_attrgetter), 0, 0, 1, 1},
   {&__pyx_n_s_byAlphabet, __pyx_k_byAlphabet, sizeof(__pyx_k_byAlphabet), 0, 0, 1, 1},
   {&__pyx_n_s_byLength, __pyx_k_byLength, sizeof(__pyx_k_byLength), 0, 0, 1, 1},
   {&__pyx_n_s_byLengthAndAlphabet, __pyx_k_byLengthAndAlphabet, sizeof(__pyx_k_byLengthAndAlphabet), 0, 0, 1, 1},
@@ -3788,96 +5200,115 @@
   {&__pyx_n_s_operator, __pyx_k_operator, sizeof(__pyx_k_operator), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_unpickle_SortedList, __pyx_k_pyx_unpickle_SortedList, sizeof(__pyx_k_pyx_unpickle_SortedList), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_StringWithKey, __pyx_k_pyx_unpickle_StringWithKey, sizeof(__pyx_k_pyx_unpickle_StringWithKey), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_sorted, __pyx_k_sorted, sizeof(__pyx_k_sorted), 0, 0, 1, 1},
   {&__pyx_n_s_sorted_array, __pyx_k_sorted_array, sizeof(__pyx_k_sorted_array), 0, 0, 1, 1},
   {&__pyx_n_s_str, __pyx_k_str, sizeof(__pyx_k_str), 0, 0, 1, 1},
+  {&__pyx_n_s_str_list, __pyx_k_str_list, sizeof(__pyx_k_str_list), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 58, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "camSort/stringSort.pyx":32
- *         return length * 10000 + self.calculate_key(str)
+  /* "camSort/stringSort.pyx":41
+ *     def reverse(self):
+ *         # same as: self.str_list.reverse()
+ *         self.str_list = self.str_list[::-1]             # <<<<<<<<<<<<<<
+ *         return self.str_list
+ * 
+ */
+  __pyx_slice_ = PySlice_New(Py_None, Py_None, __pyx_int_neg_1); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice_);
+  __Pyx_GIVEREF(__pyx_slice_);
+
+  /* "camSort/stringSort.pyx":54
+ * 
  * 
  * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
-  __pyx_tuple_ = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLength, 32, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLength, 54, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 54, __pyx_L1_error)
 
-  /* "camSort/stringSort.pyx":39
- *     return [s.str for s in sorted_array]
+  /* "camSort/stringSort.pyx":61
+ *     return SortedList([s.str for s in sorted_array])
  * 
  * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
  */
-  __pyx_tuple__3 = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLengthAndAlphabet, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLengthAndAlphabet, 61, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 61, __pyx_L1_error)
 
-  /* "camSort/stringSort.pyx":46
- *     return [s.str for s in sorted_array]
+  /* "camSort/stringSort.pyx":68
+ *     return SortedList([s.str for s in sorted_array])
  * 
  * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
  */
-  __pyx_tuple__5 = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byAlphabet, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byAlphabet, 68, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 68, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__7 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StringWithKey, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StringWithKey, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_SortedList, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  __pyx_int_46947008 = PyInt_FromLong(46947008L); if (unlikely(!__pyx_int_46947008)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_250931038 = PyInt_FromLong(250931038L); if (unlikely(!__pyx_int_250931038)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -3929,14 +5360,24 @@
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7camSort_10stringSort_StringWithKey.tp_dictoffset && __pyx_type_7camSort_10stringSort_StringWithKey.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7camSort_10stringSort_StringWithKey.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   if (__Pyx_SetVtable(__pyx_type_7camSort_10stringSort_StringWithKey.tp_dict, __pyx_vtabptr_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_StringWithKey, (PyObject *)&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __pyx_ptype_7camSort_10stringSort_StringWithKey = &__pyx_type_7camSort_10stringSort_StringWithKey;
+  if (PyType_Ready(&__pyx_type_7camSort_10stringSort_SortedList) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  #if PY_VERSION_HEX < 0x030800B1
+  __pyx_type_7camSort_10stringSort_SortedList.tp_print = 0;
+  #endif
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7camSort_10stringSort_SortedList.tp_dictoffset && __pyx_type_7camSort_10stringSort_SortedList.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_7camSort_10stringSort_SortedList.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  }
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SortedList, (PyObject *)&__pyx_type_7camSort_10stringSort_SortedList) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7camSort_10stringSort_SortedList) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_ptype_7camSort_10stringSort_SortedList = &__pyx_type_7camSort_10stringSort_SortedList;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -4183,60 +5624,72 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_attrgetter, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":32
- *         return length * 10000 + self.calculate_key(str)
+  /* "camSort/stringSort.pyx":54
+ * 
  * 
  * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_1byLength, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_1byLength, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLength, __pyx_t_2) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLength, __pyx_t_2) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":39
- *     return [s.str for s in sorted_array]
+  /* "camSort/stringSort.pyx":61
+ *     return SortedList([s.str for s in sorted_array])
  * 
  * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_3byLengthAndAlphabet, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_3byLengthAndAlphabet, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLengthAndAlphabet, __pyx_t_2) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLengthAndAlphabet, __pyx_t_2) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":46
- *     return [s.str for s in sorted_array]
+  /* "camSort/stringSort.pyx":68
+ *     return SortedList([s.str for s in sorted_array])
  * 
  * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_5byAlphabet, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_5byAlphabet, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byAlphabet, __pyx_t_2) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byAlphabet, __pyx_t_2) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_7__pyx_unpickle_StringWithKey, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_StringWithKey, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
+  /* "(tree fragment)":11
+ *         __pyx_unpickle_StringWithKey__set_state(<StringWithKey> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_StringWithKey__set_state(StringWithKey __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.key = __pyx_state[0]; __pyx_result.str = __pyx_state[1]
+ *     if len(__pyx_state) > 2 and hasattr(__pyx_result, '__dict__'):
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_9__pyx_unpickle_SortedList, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_SortedList, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
   /* "camSort/stringSort.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * from operator import attrgetter
  * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -5085,14 +6538,130 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (!j) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    } else {
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_item(o, i);
+        }
+    }
+#else
+    if (is_list || PySequence_Check(o)) {
+        return PySequence_GetItem(o, i);
+    }
+#endif
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+}
+
+/* ObjectGetItem */
+#if CYTHON_USE_TYPE_SLOTS
+static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
+    PyObject *runerr;
+    Py_ssize_t key_value;
+    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
+    if (unlikely(!(m && m->sq_item))) {
+        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
+        return NULL;
+    }
+    key_value = __Pyx_PyIndex_AsSsize_t(index);
+    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
+        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
+    }
+    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
+        PyErr_Clear();
+        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
+    }
+    return NULL;
+}
+static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
+    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
+    if (likely(m && m->mp_subscript)) {
+        return m->mp_subscript(obj, key);
+    }
+    return __Pyx_PyObject_GetIndex(obj, key);
+}
+#endif
+
 /* PyObjectCall2Args */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
@@ -5352,101 +6921,14 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
-    PyObject *r;
-    if (!j) return NULL;
-    r = PyObject_GetItem(o, j);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyList_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
-        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyTuple_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
-        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
-                                                     CYTHON_NCP_UNUSED int wraparound,
-                                                     CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
-        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
-            PyObject *r = PyList_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    }
-    else if (PyTuple_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
-            PyObject *r = PyTuple_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return NULL;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_item(o, i);
-        }
-    }
-#else
-    if (is_list || PySequence_Check(o)) {
-        return PySequence_GetItem(o, i);
-    }
-#endif
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-}
-
 /* HasAttr */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
     PyObject *r;
     if (unlikely(!__Pyx_PyBaseString_Check(n))) {
         PyErr_SetString(PyExc_TypeError,
                         "hasattr(): attribute name must be string");
         return -1;
```

### Comparing `camSort-0.2.9/camSort.egg-info/PKG-INFO` & `camSort-0.3/camSort.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,65 @@
 Metadata-Version: 2.1
 Name: camSort
-Version: 0.2.9
+Version: 0.3
 Summary: make sorted() fast for strings
 Home-page: UNKNOWN
 Author: ['cameronbae / cameron jay']
 Author-email: <contact@camjay.io>
 License: UNKNOWN
 Description: 
-        # camSort
+        # camSort 0.3!
         
-        Working on `python 3.7.1`!
+        Working on `python 3.7.3`! (at least I think.)
         
         `camSort` is a Python library that makes sorted() look slow while also using sorted(). It's built on Cython, and provides preallocation to string sorting by using a custom key calculation for each string. Normal key calculation and object creation are often computationally expensive—but here we optimize that with Cython >:)!
         
         ## Overview
         
         The `camSort` library sorts a list of strings by creating a custom object for each string. This custom object, `StringWithKey`, holds the string and a unique key calculated from it. The key is a long integer derived from the sum of Unicode code points of the characters in the string, and the string's length.
         
         The actual sorting operation uses Python's built-in `sorted` function (based on Timsort), however, now with precalculated keys, rather than comparing the strings themselves. Making sorting quite faster.
         
         The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance).
         
         ## Installation
         
-        ```pip install camSort``` or compile locally :)
+        ```pip install camSort```, or build locally :)
         
         ## Usage
         
         ```python
-        import camSort
-        # or
         from camSort import sortStrings
         
         myList = ['your', 'list', 'of', 'strings', ':)!']
         
-        sortedStrings = camSort.sortStrings(myList)
-        # or
-        sortedStrings = sortStrings(myList)
+        # By length
+        sortedStrings = sortStrings.byLength(myList)
+        # By alphabetically
+        sortedStringsCam = stringSort.byAlphabet(stringsToGen)
+        # By sorting alphabetically and length
+        sortedStringsCam = stringSort.byLengthAndAlphabet(stringsToGen)
         
         ```
         
         ## Performance
         
+        Try out the demo.py file!
+        
         Average output on my 2017 macbook pro:
             (1 million strings, with a random legnth of 1 to 1000 chararacters)
         
-        Time taken by Python sorted(): 56.08621883392334 seconds
-        Time taken by camSort: 6.356221914291382 seconds
-Keywords: python,sorted,sort,camSort
+        ```
+        Time taken by Python sorted():               57.62033486366272 seconds
+            Using camSort!
+        Time taken sorting by length:                7.040294170379639 seconds
+        By sorting alphabetically:                   3.804348945617676 seconds
+        By sorting alphabetically and length:        7.213421821594238 seconds
+        ```
+Keywords: python,sorted,sort,camSort,reverse
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `camSort-0.2.9/setup.py` & `camSort-0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
 
     name="camSort",
-    version="0.2.9",
+    version="0.3",
     install_requires=["setuptools", "wheel", "cython"],
 
     ext_modules = cythonize(['camSort/stringSort.pyx']),
 
     author=["cameronbae / cameron jay"],
     author_email="<contact@camjay.io>",
     description="make sorted() fast for strings",
     long_description_content_type="text/markdown",
     long_description=long_description,
-    keywords=['python', 'sorted', 'sort', 'camSort'],
+    keywords=['python', 'sorted', 'sort', 'camSort', 'reverse'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

