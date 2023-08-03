# Comparing `tmp/camSort-0.2.8.tar.gz` & `tmp/camSort-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/camSort-0.2.8.tar", last modified: Wed Aug  2 09:35:50 2023, max compression
+gzip compressed data, was "dist/camSort-0.2.9.tar", last modified: Thu Aug  3 05:24:10 2023, max compression
```

## Comparing `camSort-0.2.8.tar` & `camSort-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-02 09:35:50.000000 camSort-0.2.8/
--rw-r--r--   0 macbook    (501) staff       (20)     2435 2023-08-02 09:35:50.000000 camSort-0.2.8/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     1529 2023-08-01 07:52:20.000000 camSort-0.2.8/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort/
--rw-r--r--   0 macbook    (501) staff       (20)   235338 2023-08-02 09:34:25.000000 camSort-0.2.8/camSort/stringSort.c
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     2435 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      208 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       24 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       99 2023-08-02 08:57:15.000000 camSort-0.2.8/pyproject.toml
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-02 09:35:50.000000 camSort-0.2.8/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1043 2023-08-02 09:34:18.000000 camSort-0.2.8/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 05:24:10.000000 camSort-0.2.9/
+-rw-r--r--   0 macbook    (501) staff       (20)     2435 2023-08-03 05:24:10.000000 camSort-0.2.9/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     1529 2023-08-01 07:52:20.000000 camSort-0.2.9/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort/
+-rw-r--r--   0 macbook    (501) staff       (20)   270002 2023-08-03 05:23:07.000000 camSort-0.2.9/camSort/stringSort.c
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     2435 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      208 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       24 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-03 05:24:10.000000 camSort-0.2.9/camSort.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       99 2023-08-02 08:57:15.000000 camSort-0.2.9/pyproject.toml
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-03 05:24:10.000000 camSort-0.2.9/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1043 2023-08-03 05:23:49.000000 camSort-0.2.9/setup.py
```

### Comparing `camSort-0.2.8/PKG-INFO` & `camSort-0.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camSort
-Version: 0.2.8
+Version: 0.2.9
 Summary: make sorted() fast for strings
 Home-page: UNKNOWN
 Author: ['cameronbae / cameron jay']
 Author-email: <contact@camjay.io>
 License: UNKNOWN
 Description: 
         # camSort
```

### Comparing `camSort-0.2.8/README.md` & `camSort-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `camSort-0.2.8/camSort/stringSort.c` & `camSort-0.2.9/camSort/stringSort.c`

 * *Files 9% similar despite different names*

```diff
@@ -839,21 +839,23 @@
  *     cdef public:
  *         str str
  */
 struct __pyx_obj_7camSort_10stringSort_StringWithKey {
   PyObject_HEAD
   struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *__pyx_vtab;
   PyObject *str;
-  PY_LONG_LONG key;
+  PyObject *key;
 };
 
 
 
 struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey {
   PY_LONG_LONG (*calculate_key)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *);
+  PyObject *(*calculate_key_alpha)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *);
+  PY_LONG_LONG (*calculate_key_length_alpha)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *);
 };
 static struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *__pyx_vtabptr_7camSort_10stringSort_StringWithKey;
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
@@ -935,14 +937,23 @@
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
 /* UnicodeAsUCS4.proto */
 static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject*);
 
 /* object_ord.proto */
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyObject_Ord(c)\
     (likely(PyUnicode_Check(c)) ? (long)__Pyx_PyUnicode_AsPy_UCS4(c) : __Pyx__PyObject_Ord(c))
@@ -988,14 +999,66 @@
 #endif
 
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
+/* PyFunctionFastCall.proto */
+#if CYTHON_FAST_PYCALL
+#define __Pyx_PyFunction_FastCall(func, args, nargs)\
+    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
+#if 1 || PY_VERSION_HEX < 0x030600B1
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
+#else
+#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
+#endif
+#define __Pyx_BUILD_ASSERT_EXPR(cond)\
+    (sizeof(char [1 - 2*!(cond)]) - 1)
+#ifndef Py_MEMBER_SIZE
+#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
+#endif
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
+  #define __Pxy_PyFrame_Initialize_Offsets()\
+    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
+     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
+  #define __Pyx_PyFrame_GetLocalsplus(frame)\
+    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif
+
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
+/* PyObjectCallMethO.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
+#endif
+
+/* PyObjectCallNoArg.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+#else
+#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
+#endif
+
+/* PyCFunctionFastCall.proto */
+#if CYTHON_FAST_PYCCALL
+static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
+#else
+#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
+#endif
+
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
 /* PyErrExceptionMatches.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
 static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
 #define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
@@ -1066,59 +1129,14 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
 
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
-/* PyFunctionFastCall.proto */
-#if CYTHON_FAST_PYCALL
-#define __Pyx_PyFunction_FastCall(func, args, nargs)\
-    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
-#endif
-#define __Pyx_BUILD_ASSERT_EXPR(cond)\
-    (sizeof(char [1 - 2*!(cond)]) - 1)
-#ifndef Py_MEMBER_SIZE
-#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
-#endif
-  static size_t __pyx_pyframe_localsplus_offset = 0;
-  #include "frameobject.h"
-  #define __Pxy_PyFrame_Initialize_Offsets()\
-    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
-     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
-  #define __Pyx_PyFrame_GetLocalsplus(frame)\
-    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif
-
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
-#endif
-
-/* PyObjectCallMethO.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
-#endif
-
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
-
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
@@ -1204,17 +1222,14 @@
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
-static CYTHON_INLINE PY_LONG_LONG __Pyx_PyInt_As_PY_LONG_LONG(PyObject *);
-
-/* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
@@ -1232,14 +1247,16 @@
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto*/
+static PyObject *__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_alpha(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto*/
+static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_length_alpha(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto*/
 
 /* Module declarations from 'camSort.stringSort' */
 static PyTypeObject *__pyx_ptype_7camSort_10stringSort_StringWithKey = 0;
 static PyObject *__pyx_f_7camSort_10stringSort___pyx_unpickle_StringWithKey__set_state(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "camSort.stringSort"
 extern int __pyx_module_is_main_camSort__stringSort;
 int __pyx_module_is_main_camSort__stringSort = 0;
@@ -1251,59 +1268,73 @@
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_str[] = "str";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
+static const char __pyx_k_alpha[] = "alpha";
 static const char __pyx_k_array[] = "array";
+static const char __pyx_k_lower[] = "lower";
 static const char __pyx_k_import[] = "__import__";
+static const char __pyx_k_length[] = "length";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_sorted[] = "sorted";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_byLength[] = "byLength";
 static const char __pyx_k_getstate[] = "__getstate__";
+static const char __pyx_k_key_type[] = "key_type";
 static const char __pyx_k_operator[] = "operator";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_attrgetter[] = "attrgetter";
+static const char __pyx_k_byAlphabet[] = "byAlphabet";
 static const char __pyx_k_input_list[] = "input_list";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_sorted_array[] = "sorted_array";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_StringWithKey[] = "StringWithKey";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
+static const char __pyx_k_length_and_alpha[] = "length_and_alpha";
 static const char __pyx_k_camSort_stringSort[] = "camSort.stringSort";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_byLengthAndAlphabet[] = "byLengthAndAlphabet";
 static const char __pyx_k_camSort_stringSort_pyx[] = "camSort/stringSort.pyx";
 static const char __pyx_k_pyx_unpickle_StringWithKey[] = "__pyx_unpickle_StringWithKey";
 static const char __pyx_k_Incompatible_checksums_s_vs_0xef[] = "Incompatible checksums (%s vs 0xef4e75e = (key, str))";
 static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xef;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_StringWithKey;
+static PyObject *__pyx_n_u_alpha;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_attrgetter;
+static PyObject *__pyx_n_s_byAlphabet;
 static PyObject *__pyx_n_s_byLength;
+static PyObject *__pyx_n_s_byLengthAndAlphabet;
 static PyObject *__pyx_n_s_camSort_stringSort;
 static PyObject *__pyx_kp_s_camSort_stringSort_pyx;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_input_list;
 static PyObject *__pyx_n_s_key;
 static PyObject *__pyx_n_u_key;
+static PyObject *__pyx_n_s_key_type;
+static PyObject *__pyx_n_u_length;
+static PyObject *__pyx_n_u_length_and_alpha;
+static PyObject *__pyx_n_s_lower;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_n;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_n_s_operator;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pyx_PickleError;
@@ -1321,149 +1352,251 @@
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_sorted;
 static PyObject *__pyx_n_s_sorted_array;
 static PyObject *__pyx_n_s_str;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_update;
-static int __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto */
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str, PyObject *__pyx_v_key_type); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_3str___get__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_2__set__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_4__del__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_3key___get__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_2__set__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_4__del__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_2__reduce_cython__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_4__setstate_cython__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_7camSort_10stringSort_byLength(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
-static PyObject *__pyx_pf_7camSort_10stringSort_2__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_2byLengthAndAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_4byAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_6__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_7camSort_10stringSort_StringWithKey(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_250931038;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__3;
+static PyObject *__pyx_tuple__5;
+static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_codeobj__2;
 static PyObject *__pyx_codeobj__4;
+static PyObject *__pyx_codeobj__6;
+static PyObject *__pyx_codeobj__8;
 /* Late includes */
 
 /* "camSort/stringSort.pyx":9
- *         long long key
+ *         object key  # Changed from long long to object
  * 
- *     def __init__(self, str):             # <<<<<<<<<<<<<<
+ *     def __init__(self, str, key_type='length'):             # <<<<<<<<<<<<<<
  *         self.str = str
- *         self.key = self.calculate_key(str)
+ *         if key_type == 'alpha':
  */
 
 /* Python wrapper */
 static int __pyx_pw_7camSort_10stringSort_13StringWithKey_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_7camSort_10stringSort_13StringWithKey_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_str = 0;
+  PyObject *__pyx_v_key_type = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_str,0};
-    PyObject* values[1] = {0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_str,&__pyx_n_s_key_type,0};
+    PyObject* values[2] = {0,0};
+    values[1] = ((PyObject *)__pyx_n_u_length);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_str)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_key_type);
+          if (value) { values[1] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 9, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
-      goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
     }
     __pyx_v_str = values[0];
+    __pyx_v_key_type = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 9, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 9, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("camSort.stringSort.StringWithKey.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self), __pyx_v_str);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self), __pyx_v_str, __pyx_v_key_type);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str) {
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str, PyObject *__pyx_v_key_type) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "camSort/stringSort.pyx":10
  * 
- *     def __init__(self, str):
+ *     def __init__(self, str, key_type='length'):
  *         self.str = str             # <<<<<<<<<<<<<<
- *         self.key = self.calculate_key(str)
- * 
+ *         if key_type == 'alpha':
+ *             self.key = self.calculate_key_alpha(str)
  */
   if (!(likely(PyUnicode_CheckExact(__pyx_v_str))||((__pyx_v_str) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_str)->tp_name), 0))) __PYX_ERR(0, 10, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_str;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->str);
   __Pyx_DECREF(__pyx_v_self->str);
   __pyx_v_self->str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "camSort/stringSort.pyx":11
- *     def __init__(self, str):
+ *     def __init__(self, str, key_type='length'):
+ *         self.str = str
+ *         if key_type == 'alpha':             # <<<<<<<<<<<<<<
+ *             self.key = self.calculate_key_alpha(str)
+ *         elif key_type == 'length_and_alpha':
+ */
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_key_type, __pyx_n_u_alpha, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (__pyx_t_2) {
+
+    /* "camSort/stringSort.pyx":12
+ *         self.str = str
+ *         if key_type == 'alpha':
+ *             self.key = self.calculate_key_alpha(str)             # <<<<<<<<<<<<<<
+ *         elif key_type == 'length_and_alpha':
+ *             self.key = self.calculate_key_length_alpha(str)
+ */
+    __pyx_t_1 = ((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key_alpha(__pyx_v_self, __pyx_v_str); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_1);
+    __Pyx_GOTREF(__pyx_v_self->key);
+    __Pyx_DECREF(__pyx_v_self->key);
+    __pyx_v_self->key = __pyx_t_1;
+    __pyx_t_1 = 0;
+
+    /* "camSort/stringSort.pyx":11
+ *     def __init__(self, str, key_type='length'):
  *         self.str = str
- *         self.key = self.calculate_key(str)             # <<<<<<<<<<<<<<
+ *         if key_type == 'alpha':             # <<<<<<<<<<<<<<
+ *             self.key = self.calculate_key_alpha(str)
+ *         elif key_type == 'length_and_alpha':
+ */
+    goto __pyx_L3;
+  }
+
+  /* "camSort/stringSort.pyx":13
+ *         if key_type == 'alpha':
+ *             self.key = self.calculate_key_alpha(str)
+ *         elif key_type == 'length_and_alpha':             # <<<<<<<<<<<<<<
+ *             self.key = self.calculate_key_length_alpha(str)
+ *         else:
+ */
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_key_type, __pyx_n_u_length_and_alpha, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (__pyx_t_2) {
+
+    /* "camSort/stringSort.pyx":14
+ *             self.key = self.calculate_key_alpha(str)
+ *         elif key_type == 'length_and_alpha':
+ *             self.key = self.calculate_key_length_alpha(str)             # <<<<<<<<<<<<<<
+ *         else:
+ *             self.key = self.calculate_key(str)
+ */
+    __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key_length_alpha(__pyx_v_self, __pyx_v_str)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_1);
+    __Pyx_GOTREF(__pyx_v_self->key);
+    __Pyx_DECREF(__pyx_v_self->key);
+    __pyx_v_self->key = __pyx_t_1;
+    __pyx_t_1 = 0;
+
+    /* "camSort/stringSort.pyx":13
+ *         if key_type == 'alpha':
+ *             self.key = self.calculate_key_alpha(str)
+ *         elif key_type == 'length_and_alpha':             # <<<<<<<<<<<<<<
+ *             self.key = self.calculate_key_length_alpha(str)
+ *         else:
+ */
+    goto __pyx_L3;
+  }
+
+  /* "camSort/stringSort.pyx":16
+ *             self.key = self.calculate_key_length_alpha(str)
+ *         else:
+ *             self.key = self.calculate_key(str)             # <<<<<<<<<<<<<<
  * 
  *     cdef long long calculate_key(self, str):
  */
-  __pyx_v_self->key = ((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key(__pyx_v_self, __pyx_v_str);
+  /*else*/ {
+    __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key(__pyx_v_self, __pyx_v_str)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_1);
+    __Pyx_GOTREF(__pyx_v_self->key);
+    __Pyx_DECREF(__pyx_v_self->key);
+    __pyx_v_self->key = __pyx_t_1;
+    __pyx_t_1 = 0;
+  }
+  __pyx_L3:;
 
   /* "camSort/stringSort.pyx":9
- *         long long key
+ *         object key  # Changed from long long to object
  * 
- *     def __init__(self, str):             # <<<<<<<<<<<<<<
+ *     def __init__(self, str, key_type='length'):             # <<<<<<<<<<<<<<
  *         self.str = str
- *         self.key = self.calculate_key(str)
+ *         if key_type == 'alpha':
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("camSort.stringSort.StringWithKey.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":13
- *         self.key = self.calculate_key(str)
+/* "camSort/stringSort.pyx":18
+ *             self.key = self.calculate_key(str)
  * 
  *     cdef long long calculate_key(self, str):             # <<<<<<<<<<<<<<
  *         cdef int length = len(str)
  *         cdef long long sum = 0
  */
 
 static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str) {
@@ -1478,114 +1611,114 @@
   PyObject *__pyx_t_4 = NULL;
   long __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calculate_key", 0);
 
-  /* "camSort/stringSort.pyx":14
+  /* "camSort/stringSort.pyx":19
  * 
  *     cdef long long calculate_key(self, str):
  *         cdef int length = len(str)             # <<<<<<<<<<<<<<
  *         cdef long long sum = 0
  *         for c in str:
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_str); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_str); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 19, __pyx_L1_error)
   __pyx_v_length = __pyx_t_1;
 
-  /* "camSort/stringSort.pyx":15
+  /* "camSort/stringSort.pyx":20
  *     cdef long long calculate_key(self, str):
  *         cdef int length = len(str)
  *         cdef long long sum = 0             # <<<<<<<<<<<<<<
  *         for c in str:
  *             sum += ord(c)
  */
   __pyx_v_sum = 0;
 
-  /* "camSort/stringSort.pyx":16
+  /* "camSort/stringSort.pyx":21
  *         cdef int length = len(str)
  *         cdef long long sum = 0
  *         for c in str:             # <<<<<<<<<<<<<<
  *             sum += ord(c)
  *         return length * 10000 + sum
  */
   if (likely(PyList_CheckExact(__pyx_v_str)) || PyTuple_CheckExact(__pyx_v_str)) {
     __pyx_t_2 = __pyx_v_str; __Pyx_INCREF(__pyx_t_2); __pyx_t_1 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_1 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+    __pyx_t_1 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 16, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 21, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 16, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 16, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 21, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 16, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_2);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 16, __pyx_L1_error)
+          else __PYX_ERR(0, 21, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_c, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "camSort/stringSort.pyx":17
+    /* "camSort/stringSort.pyx":22
  *         cdef long long sum = 0
  *         for c in str:
  *             sum += ord(c)             # <<<<<<<<<<<<<<
  *         return length * 10000 + sum
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_Ord(__pyx_v_c); if (unlikely(__pyx_t_5 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 17, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Ord(__pyx_v_c); if (unlikely(__pyx_t_5 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 22, __pyx_L1_error)
     __pyx_v_sum = (__pyx_v_sum + __pyx_t_5);
 
-    /* "camSort/stringSort.pyx":16
+    /* "camSort/stringSort.pyx":21
  *         cdef int length = len(str)
  *         cdef long long sum = 0
  *         for c in str:             # <<<<<<<<<<<<<<
  *             sum += ord(c)
  *         return length * 10000 + sum
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":18
+  /* "camSort/stringSort.pyx":23
  *         for c in str:
  *             sum += ord(c)
  *         return length * 10000 + sum             # <<<<<<<<<<<<<<
  * 
- * def byLength(input_list):
+ *     cdef object calculate_key_alpha(self, str):
  */
   __pyx_r = ((__pyx_v_length * 0x2710) + __pyx_v_sum);
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":13
- *         self.key = self.calculate_key(str)
+  /* "camSort/stringSort.pyx":18
+ *             self.key = self.calculate_key(str)
  * 
  *     cdef long long calculate_key(self, str):             # <<<<<<<<<<<<<<
  *         cdef int length = len(str)
  *         cdef long long sum = 0
  */
 
   /* function exit code */
@@ -1596,19 +1729,143 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_c);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "camSort/stringSort.pyx":25
+ *         return length * 10000 + sum
+ * 
+ *     cdef object calculate_key_alpha(self, str):             # <<<<<<<<<<<<<<
+ *         return str.lower()
+ * 
+ */
+
+static PyObject *__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_alpha(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("calculate_key_alpha", 0);
+
+  /* "camSort/stringSort.pyx":26
+ * 
+ *     cdef object calculate_key_alpha(self, str):
+ *         return str.lower()             # <<<<<<<<<<<<<<
+ * 
+ *     cdef long long calculate_key_length_alpha(self, str):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_str, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "camSort/stringSort.pyx":25
+ *         return length * 10000 + sum
+ * 
+ *     cdef object calculate_key_alpha(self, str):             # <<<<<<<<<<<<<<
+ *         return str.lower()
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("camSort.stringSort.StringWithKey.calculate_key_alpha", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "camSort/stringSort.pyx":28
+ *         return str.lower()
+ * 
+ *     cdef long long calculate_key_length_alpha(self, str):             # <<<<<<<<<<<<<<
+ *         cdef int length = len(str)
+ *         return length * 10000 + self.calculate_key(str)
+ */
+
+static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_length_alpha(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str) {
+  int __pyx_v_length;
+  PY_LONG_LONG __pyx_r;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("calculate_key_length_alpha", 0);
+
+  /* "camSort/stringSort.pyx":29
+ * 
+ *     cdef long long calculate_key_length_alpha(self, str):
+ *         cdef int length = len(str)             # <<<<<<<<<<<<<<
+ *         return length * 10000 + self.calculate_key(str)
+ * 
+ */
+  __pyx_t_1 = PyObject_Length(__pyx_v_str); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_v_length = __pyx_t_1;
+
+  /* "camSort/stringSort.pyx":30
+ *     cdef long long calculate_key_length_alpha(self, str):
+ *         cdef int length = len(str)
+ *         return length * 10000 + self.calculate_key(str)             # <<<<<<<<<<<<<<
+ * 
+ * def byLength(input_list):
+ */
+  __pyx_r = ((__pyx_v_length * 0x2710) + ((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key(__pyx_v_self, __pyx_v_str));
+  goto __pyx_L0;
+
+  /* "camSort/stringSort.pyx":28
+ *         return str.lower()
+ * 
+ *     cdef long long calculate_key_length_alpha(self, str):             # <<<<<<<<<<<<<<
+ *         cdef int length = len(str)
+ *         return length * 10000 + self.calculate_key(str)
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("camSort.stringSort.StringWithKey.calculate_key_length_alpha", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "camSort/stringSort.pyx":6
  * cdef class StringWithKey:
  *     cdef public:
  *         str str             # <<<<<<<<<<<<<<
- *         long long key
+ *         object key  # Changed from long long to object
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3str_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3str_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
@@ -1707,17 +1964,17 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "camSort/stringSort.pyx":7
  *     cdef public:
  *         str str
- *         long long key             # <<<<<<<<<<<<<<
+ *         object key  # Changed from long long to object             # <<<<<<<<<<<<<<
  * 
- *     def __init__(self, str):
+ *     def __init__(self, str, key_type='length'):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3key_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3key_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -1728,31 +1985,21 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_3key___get__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __Pyx_INCREF(__pyx_v_self->key);
+  __pyx_r = __pyx_v_self->key;
   goto __pyx_L0;
 
   /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("camSort.stringSort.StringWithKey.key.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
@@ -1767,29 +2014,52 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_2__set__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  PY_LONG_LONG __pyx_t_1;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_value); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 7, __pyx_L1_error)
-  __pyx_v_self->key = __pyx_t_1;
+  __Pyx_INCREF(__pyx_v_value);
+  __Pyx_GIVEREF(__pyx_v_value);
+  __Pyx_GOTREF(__pyx_v_self->key);
+  __Pyx_DECREF(__pyx_v_self->key);
+  __pyx_v_self->key = __pyx_v_value;
+
+  /* function exit code */
+  __pyx_r = 0;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_7camSort_10stringSort_13StringWithKey_3key_5__del__(PyObject *__pyx_v_self); /*proto*/
+static int __pyx_pw_7camSort_10stringSort_13StringWithKey_3key_5__del__(PyObject *__pyx_v_self) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_4__del__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_4__del__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__", 0);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  __Pyx_GOTREF(__pyx_v_self->key);
+  __Pyx_DECREF(__pyx_v_self->key);
+  __pyx_v_self->key = Py_None;
 
   /* function exit code */
   __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_AddTraceback("camSort.stringSort.StringWithKey.key.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
@@ -1812,90 +2082,89 @@
 static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_2__reduce_cython__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_2;
   int __pyx_t_3;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.key, self.str)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->key); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __Pyx_INCREF(__pyx_v_self->key);
+  __Pyx_GIVEREF(__pyx_v_self->key);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_self->key);
   __Pyx_INCREF(__pyx_v_self->str);
   __Pyx_GIVEREF(__pyx_v_self->str);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_self->str);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_self->str);
+  __pyx_v_state = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_v_state = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
 
   /* "(tree fragment)":6
  *     cdef bint use_setstate
  *     state = (self.key, self.str)
  *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
  *     if _dict is not None:
  *         state += (_dict,)
  */
-  __pyx_t_2 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_v__dict = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v__dict = __pyx_t_1;
+  __pyx_t_1 = 0;
 
   /* "(tree fragment)":7
  *     state = (self.key, self.str)
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:             # <<<<<<<<<<<<<<
  *         state += (_dict,)
  *         use_setstate = True
  */
-  __pyx_t_3 = (__pyx_v__dict != Py_None);
-  __pyx_t_4 = (__pyx_t_3 != 0);
-  if (__pyx_t_4) {
+  __pyx_t_2 = (__pyx_v__dict != Py_None);
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":8
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  *         state += (_dict,)             # <<<<<<<<<<<<<<
  *         use_setstate = True
  *     else:
  */
-    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 8, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v__dict);
     __Pyx_GIVEREF(__pyx_v__dict);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v__dict);
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_1));
-    __pyx_t_1 = 0;
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict);
+    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_4));
+    __pyx_t_4 = 0;
 
     /* "(tree fragment)":9
  *     if _dict is not None:
  *         state += (_dict,)
  *         use_setstate = True             # <<<<<<<<<<<<<<
  *     else:
- *         use_setstate = self.str is not None
+ *         use_setstate = self.key is not None or self.str is not None
  */
     __pyx_v_use_setstate = 1;
 
     /* "(tree fragment)":7
  *     state = (self.key, self.str)
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:             # <<<<<<<<<<<<<<
@@ -1904,73 +2173,83 @@
  */
     goto __pyx_L3;
   }
 
   /* "(tree fragment)":11
  *         use_setstate = True
  *     else:
- *         use_setstate = self.str is not None             # <<<<<<<<<<<<<<
+ *         use_setstate = self.key is not None or self.str is not None             # <<<<<<<<<<<<<<
  *     if use_setstate:
  *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, None), state
  */
   /*else*/ {
-    __pyx_t_4 = (__pyx_v_self->str != ((PyObject*)Py_None));
-    __pyx_v_use_setstate = __pyx_t_4;
+    __pyx_t_2 = (__pyx_v_self->key != Py_None);
+    __pyx_t_5 = (__pyx_t_2 != 0);
+    if (!__pyx_t_5) {
+    } else {
+      __pyx_t_3 = __pyx_t_5;
+      goto __pyx_L4_bool_binop_done;
+    }
+    __pyx_t_5 = (__pyx_v_self->str != ((PyObject*)Py_None));
+    __pyx_t_2 = (__pyx_t_5 != 0);
+    __pyx_t_3 = __pyx_t_2;
+    __pyx_L4_bool_binop_done:;
+    __pyx_v_use_setstate = __pyx_t_3;
   }
   __pyx_L3:;
 
   /* "(tree fragment)":12
  *     else:
- *         use_setstate = self.str is not None
+ *         use_setstate = self.key is not None or self.str is not None
  *     if use_setstate:             # <<<<<<<<<<<<<<
  *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, None), state
  *     else:
  */
-  __pyx_t_4 = (__pyx_v_use_setstate != 0);
-  if (__pyx_t_4) {
+  __pyx_t_3 = (__pyx_v_use_setstate != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":13
- *         use_setstate = self.str is not None
+ *         use_setstate = self.key is not None or self.str is not None
  *     if use_setstate:
  *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, None), state             # <<<<<<<<<<<<<<
  *     else:
  *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, state)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pyx_unpickle_StringWithKey); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_StringWithKey); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_INCREF(__pyx_int_250931038);
     __Pyx_GIVEREF(__pyx_int_250931038);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_int_250931038);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_250931038);
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
-    PyTuple_SET_ITEM(__pyx_t_2, 2, Py_None);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None);
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_1);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
-    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_v_state);
+    __pyx_t_4 = 0;
     __pyx_t_1 = 0;
-    __pyx_t_2 = 0;
-    __pyx_r = __pyx_t_5;
-    __pyx_t_5 = 0;
+    __pyx_r = __pyx_t_6;
+    __pyx_t_6 = 0;
     goto __pyx_L0;
 
     /* "(tree fragment)":12
  *     else:
- *         use_setstate = self.str is not None
+ *         use_setstate = self.key is not None or self.str is not None
  *     if use_setstate:             # <<<<<<<<<<<<<<
  *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, None), state
  *     else:
  */
   }
 
   /* "(tree fragment)":15
@@ -1978,51 +2257,51 @@
  *     else:
  *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, state)             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_StringWithKey__set_state(self, __pyx_state)
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle_StringWithKey); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_pyx_unpickle_StringWithKey); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_INCREF(__pyx_int_250931038);
     __Pyx_GIVEREF(__pyx_int_250931038);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_int_250931038);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_250931038);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
-    PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_v_state);
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
-    __pyx_t_5 = 0;
-    __pyx_t_2 = 0;
-    __pyx_r = __pyx_t_1;
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_6 = 0;
     __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_4;
+    __pyx_t_4 = 0;
     goto __pyx_L0;
   }
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("camSort.stringSort.StringWithKey.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -2084,16 +2363,16 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/stringSort.pyx":20
- *         return length * 10000 + sum
+/* "camSort/stringSort.pyx":32
+ *         return length * 10000 + self.calculate_key(str)
  * 
  * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
 
 /* Python wrapper */
@@ -2126,199 +2405,202 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("byLength", 0);
 
-  /* "camSort/stringSort.pyx":21
+  /* "camSort/stringSort.pyx":33
  * 
  * def byLength(input_list):
  *     cdef int n = len(input_list)             # <<<<<<<<<<<<<<
  *     cdef list array = [StringWithKey(s) for s in input_list]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 33, __pyx_L1_error)
   __pyx_v_n = __pyx_t_1;
 
-  /* "camSort/stringSort.pyx":22
+  /* "camSort/stringSort.pyx":34
  * def byLength(input_list):
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]             # <<<<<<<<<<<<<<
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))
  */
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L5_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (likely(PyList_CheckExact(__pyx_v_input_list)) || PyTuple_CheckExact(__pyx_v_input_list)) {
       __pyx_t_3 = __pyx_v_input_list; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L5_error)
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 22, __pyx_L5_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 22, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 34, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 22, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 22, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 34, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 22, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_3);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 22, __pyx_L5_error)
+            else __PYX_ERR(0, 34, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_s, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_7genexpr__pyx_v_s); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 22, __pyx_L5_error)
+      __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_7genexpr__pyx_v_s); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 22, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 34, __pyx_L5_error)
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
 
-  /* "camSort/stringSort.pyx":24
+  /* "camSort/stringSort.pyx":36
  *     cdef list array = [StringWithKey(s) for s in input_list]
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))             # <<<<<<<<<<<<<<
  *     return [s.str for s in sorted_array]
+ * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_array);
   __Pyx_GIVEREF(__pyx_v_array);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_array);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 36, __pyx_L1_error)
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
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_5) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_5) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_sorted_array = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "camSort/stringSort.pyx":25
+  /* "camSort/stringSort.pyx":37
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))
  *     return [s.str for s in sorted_array]             # <<<<<<<<<<<<<<
+ * 
+ * def byLengthAndAlphabet(input_list):
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 25, __pyx_L11_error)
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (likely(PyList_CheckExact(__pyx_v_sorted_array)) || PyTuple_CheckExact(__pyx_v_sorted_array)) {
       __pyx_t_3 = __pyx_v_sorted_array; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L11_error)
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 25, __pyx_L11_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L11_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 25, __pyx_L11_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 37, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L11_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 25, __pyx_L11_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 37, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L11_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_4(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 25, __pyx_L11_error)
+            else __PYX_ERR(0, 37, __pyx_L11_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_s, __pyx_t_2);
       __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L11_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 25, __pyx_L11_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 37, __pyx_L11_error)
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
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "camSort/stringSort.pyx":20
- *         return length * 10000 + sum
+  /* "camSort/stringSort.pyx":32
+ *         return length * 10000 + self.calculate_key(str)
  * 
  * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
 
   /* function exit code */
@@ -2336,24 +2618,551 @@
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_s);
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "camSort/stringSort.pyx":39
+ *     return [s.str for s in sorted_array]
+ * 
+ * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
+ *     cdef int n = len(input_list)
+ *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7camSort_10stringSort_3byLengthAndAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_3byLengthAndAlphabet = {"byLengthAndAlphabet", (PyCFunction)__pyx_pw_7camSort_10stringSort_3byLengthAndAlphabet, METH_O, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_3byLengthAndAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("byLengthAndAlphabet (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_2byLengthAndAlphabet(__pyx_self, ((PyObject *)__pyx_v_input_list));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7camSort_10stringSort_2byLengthAndAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+  CYTHON_UNUSED int __pyx_v_n;
+  PyObject *__pyx_v_array = 0;
+  PyObject *__pyx_v_sorted_array = NULL;
+  PyObject *__pyx_8genexpr2__pyx_v_s = NULL;
+  PyObject *__pyx_8genexpr3__pyx_v_s = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *(*__pyx_t_4)(PyObject *);
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("byLengthAndAlphabet", 0);
+
+  /* "camSort/stringSort.pyx":40
+ * 
+ * def byLengthAndAlphabet(input_list):
+ *     cdef int n = len(input_list)             # <<<<<<<<<<<<<<
+ *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
+ * 
+ */
+  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_v_n = __pyx_t_1;
+
+  /* "camSort/stringSort.pyx":41
+ * def byLengthAndAlphabet(input_list):
+ *     cdef int n = len(input_list)
+ *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]             # <<<<<<<<<<<<<<
+ * 
+ *     sorted_array = sorted(array, key=attrgetter('key'))
+ */
+  { /* enter inner scope */
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L5_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (likely(PyList_CheckExact(__pyx_v_input_list)) || PyTuple_CheckExact(__pyx_v_input_list)) {
+      __pyx_t_3 = __pyx_v_input_list; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
+      __pyx_t_4 = NULL;
+    } else {
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L5_error)
+    }
+    for (;;) {
+      if (likely(!__pyx_t_4)) {
+        if (likely(PyList_CheckExact(__pyx_t_3))) {
+          if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 41, __pyx_L5_error)
+          #else
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_5);
+          #endif
+        } else {
+          if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 41, __pyx_L5_error)
+          #else
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_5);
+          #endif
+        }
+      } else {
+        __pyx_t_5 = __pyx_t_4(__pyx_t_3);
+        if (unlikely(!__pyx_t_5)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(0, 41, __pyx_L5_error)
+          }
+          break;
+        }
+        __Pyx_GOTREF(__pyx_t_5);
+      }
+      __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_s, __pyx_t_5);
+      __pyx_t_5 = 0;
+      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_8genexpr2__pyx_v_s);
+      __Pyx_GIVEREF(__pyx_8genexpr2__pyx_v_s);
+      PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_8genexpr2__pyx_v_s);
+      __Pyx_INCREF(__pyx_n_u_length_and_alpha);
+      __Pyx_GIVEREF(__pyx_n_u_length_and_alpha);
+      PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_n_u_length_and_alpha);
+      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 41, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 41, __pyx_L5_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_s); __pyx_8genexpr2__pyx_v_s = 0;
+    goto __pyx_L8_exit_scope;
+    __pyx_L5_error:;
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_s); __pyx_8genexpr2__pyx_v_s = 0;
+    goto __pyx_L1_error;
+    __pyx_L8_exit_scope:;
+  } /* exit inner scope */
+  __pyx_v_array = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "camSort/stringSort.pyx":43
+ *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
+ * 
+ *     sorted_array = sorted(array, key=attrgetter('key'))             # <<<<<<<<<<<<<<
+ *     return [s.str for s in sorted_array]
+ * 
+ */
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_v_array);
+  __Pyx_GIVEREF(__pyx_v_array);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_array);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_7 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_7)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_7);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
+    }
+  }
+  __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_n_u_key) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_u_key);
+  __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_6) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_sorted_array = __pyx_t_6;
+  __pyx_t_6 = 0;
+
+  /* "camSort/stringSort.pyx":44
+ * 
+ *     sorted_array = sorted(array, key=attrgetter('key'))
+ *     return [s.str for s in sorted_array]             # <<<<<<<<<<<<<<
+ * 
+ * def byAlphabet(input_list):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  { /* enter inner scope */
+    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 44, __pyx_L11_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (likely(PyList_CheckExact(__pyx_v_sorted_array)) || PyTuple_CheckExact(__pyx_v_sorted_array)) {
+      __pyx_t_3 = __pyx_v_sorted_array; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
+      __pyx_t_4 = NULL;
+    } else {
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L11_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L11_error)
+    }
+    for (;;) {
+      if (likely(!__pyx_t_4)) {
+        if (likely(PyList_CheckExact(__pyx_t_3))) {
+          if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 44, __pyx_L11_error)
+          #else
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L11_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        } else {
+          if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 44, __pyx_L11_error)
+          #else
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L11_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        }
+      } else {
+        __pyx_t_2 = __pyx_t_4(__pyx_t_3);
+        if (unlikely(!__pyx_t_2)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(0, 44, __pyx_L11_error)
+          }
+          break;
+        }
+        __Pyx_GOTREF(__pyx_t_2);
+      }
+      __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_s, __pyx_t_2);
+      __pyx_t_2 = 0;
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr3__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L11_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 44, __pyx_L11_error)
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_s); __pyx_8genexpr3__pyx_v_s = 0;
+    goto __pyx_L14_exit_scope;
+    __pyx_L11_error:;
+    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_s); __pyx_8genexpr3__pyx_v_s = 0;
+    goto __pyx_L1_error;
+    __pyx_L14_exit_scope:;
+  } /* exit inner scope */
+  __pyx_r = __pyx_t_6;
+  __pyx_t_6 = 0;
+  goto __pyx_L0;
+
+  /* "camSort/stringSort.pyx":39
+ *     return [s.str for s in sorted_array]
+ * 
+ * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
+ *     cdef int n = len(input_list)
+ *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("camSort.stringSort.byLengthAndAlphabet", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_array);
+  __Pyx_XDECREF(__pyx_v_sorted_array);
+  __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_s);
+  __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_s);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "camSort/stringSort.pyx":46
+ *     return [s.str for s in sorted_array]
+ * 
+ * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
+ *     cdef int n = len(input_list)
+ *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7camSort_10stringSort_5byAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_5byAlphabet = {"byAlphabet", (PyCFunction)__pyx_pw_7camSort_10stringSort_5byAlphabet, METH_O, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_5byAlphabet(PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("byAlphabet (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_4byAlphabet(__pyx_self, ((PyObject *)__pyx_v_input_list));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7camSort_10stringSort_4byAlphabet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+  CYTHON_UNUSED int __pyx_v_n;
+  PyObject *__pyx_v_array = 0;
+  PyObject *__pyx_v_sorted_array = NULL;
+  PyObject *__pyx_8genexpr4__pyx_v_s = NULL;
+  PyObject *__pyx_8genexpr5__pyx_v_s = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *(*__pyx_t_4)(PyObject *);
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("byAlphabet", 0);
+
+  /* "camSort/stringSort.pyx":47
+ * 
+ * def byAlphabet(input_list):
+ *     cdef int n = len(input_list)             # <<<<<<<<<<<<<<
+ *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
+ * 
+ */
+  __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_v_n = __pyx_t_1;
+
+  /* "camSort/stringSort.pyx":48
+ * def byAlphabet(input_list):
+ *     cdef int n = len(input_list)
+ *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]             # <<<<<<<<<<<<<<
+ * 
+ *     sorted_array = sorted(array, key=attrgetter('key'))
+ */
+  { /* enter inner scope */
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L5_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (likely(PyList_CheckExact(__pyx_v_input_list)) || PyTuple_CheckExact(__pyx_v_input_list)) {
+      __pyx_t_3 = __pyx_v_input_list; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
+      __pyx_t_4 = NULL;
+    } else {
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L5_error)
+    }
+    for (;;) {
+      if (likely(!__pyx_t_4)) {
+        if (likely(PyList_CheckExact(__pyx_t_3))) {
+          if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 48, __pyx_L5_error)
+          #else
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_5);
+          #endif
+        } else {
+          if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 48, __pyx_L5_error)
+          #else
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_5);
+          #endif
+        }
+      } else {
+        __pyx_t_5 = __pyx_t_4(__pyx_t_3);
+        if (unlikely(!__pyx_t_5)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(0, 48, __pyx_L5_error)
+          }
+          break;
+        }
+        __Pyx_GOTREF(__pyx_t_5);
+      }
+      __Pyx_XDECREF_SET(__pyx_8genexpr4__pyx_v_s, __pyx_t_5);
+      __pyx_t_5 = 0;
+      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_8genexpr4__pyx_v_s);
+      __Pyx_GIVEREF(__pyx_8genexpr4__pyx_v_s);
+      PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_8genexpr4__pyx_v_s);
+      __Pyx_INCREF(__pyx_n_u_alpha);
+      __Pyx_GIVEREF(__pyx_n_u_alpha);
+      PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_n_u_alpha);
+      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 48, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 48, __pyx_L5_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_s); __pyx_8genexpr4__pyx_v_s = 0;
+    goto __pyx_L8_exit_scope;
+    __pyx_L5_error:;
+    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_s); __pyx_8genexpr4__pyx_v_s = 0;
+    goto __pyx_L1_error;
+    __pyx_L8_exit_scope:;
+  } /* exit inner scope */
+  __pyx_v_array = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "camSort/stringSort.pyx":50
+ *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
+ * 
+ *     sorted_array = sorted(array, key=attrgetter('key'))             # <<<<<<<<<<<<<<
+ *     return [s.str for s in sorted_array]
+ * 
+ */
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_v_array);
+  __Pyx_GIVEREF(__pyx_v_array);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_array);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_7 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_7)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_7);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
+    }
+  }
+  __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_n_u_key) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_u_key);
+  __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_6) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_sorted_array = __pyx_t_6;
+  __pyx_t_6 = 0;
+
+  /* "camSort/stringSort.pyx":51
+ * 
+ *     sorted_array = sorted(array, key=attrgetter('key'))
+ *     return [s.str for s in sorted_array]             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  { /* enter inner scope */
+    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 51, __pyx_L11_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (likely(PyList_CheckExact(__pyx_v_sorted_array)) || PyTuple_CheckExact(__pyx_v_sorted_array)) {
+      __pyx_t_3 = __pyx_v_sorted_array; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
+      __pyx_t_4 = NULL;
+    } else {
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L11_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L11_error)
+    }
+    for (;;) {
+      if (likely(!__pyx_t_4)) {
+        if (likely(PyList_CheckExact(__pyx_t_3))) {
+          if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 51, __pyx_L11_error)
+          #else
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L11_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        } else {
+          if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 51, __pyx_L11_error)
+          #else
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L11_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        }
+      } else {
+        __pyx_t_2 = __pyx_t_4(__pyx_t_3);
+        if (unlikely(!__pyx_t_2)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(0, 51, __pyx_L11_error)
+          }
+          break;
+        }
+        __Pyx_GOTREF(__pyx_t_2);
+      }
+      __Pyx_XDECREF_SET(__pyx_8genexpr5__pyx_v_s, __pyx_t_2);
+      __pyx_t_2 = 0;
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr5__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L11_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 51, __pyx_L11_error)
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_s); __pyx_8genexpr5__pyx_v_s = 0;
+    goto __pyx_L14_exit_scope;
+    __pyx_L11_error:;
+    __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_s); __pyx_8genexpr5__pyx_v_s = 0;
+    goto __pyx_L1_error;
+    __pyx_L14_exit_scope:;
+  } /* exit inner scope */
+  __pyx_r = __pyx_t_6;
+  __pyx_t_6 = 0;
+  goto __pyx_L0;
+
+  /* "camSort/stringSort.pyx":46
+ *     return [s.str for s in sorted_array]
+ * 
+ * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
+ *     cdef int n = len(input_list)
+ *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("camSort.stringSort.byAlphabet", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_array);
+  __Pyx_XDECREF(__pyx_v_sorted_array);
+  __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_s);
+  __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_s);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "(tree fragment)":1
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_10stringSort_3__pyx_unpickle_StringWithKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_7camSort_10stringSort_3__pyx_unpickle_StringWithKey = {"__pyx_unpickle_StringWithKey", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7camSort_10stringSort_3__pyx_unpickle_StringWithKey, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7camSort_10stringSort_3__pyx_unpickle_StringWithKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7camSort_10stringSort_7__pyx_unpickle_StringWithKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_7__pyx_unpickle_StringWithKey = {"__pyx_unpickle_StringWithKey", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7camSort_10stringSort_7__pyx_unpickle_StringWithKey, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_7__pyx_unpickle_StringWithKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -2411,22 +3220,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_StringWithKey", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_StringWithKey", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7camSort_10stringSort_2__pyx_unpickle_StringWithKey(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_6__pyx_unpickle_StringWithKey(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_10stringSort_2__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7camSort_10stringSort_6__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -2613,22 +3422,21 @@
  *     if len(__pyx_state) > 2 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_7camSort_10stringSort___pyx_unpickle_StringWithKey__set_state(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PY_LONG_LONG __pyx_t_2;
-  int __pyx_t_3;
-  Py_ssize_t __pyx_t_4;
+  int __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  int __pyx_t_4;
   int __pyx_t_5;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_StringWithKey__set_state", 0);
 
   /* "(tree fragment)":12
  *     return __pyx_result
@@ -2639,17 +3447,19 @@
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_2 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->key = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->key);
+  __Pyx_DECREF(__pyx_v___pyx_result->key);
+  __pyx_v___pyx_result->key = __pyx_t_1;
+  __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
@@ -2665,59 +3475,59 @@
  *     if len(__pyx_state) > 2 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
  *         __pyx_result.__dict__.update(__pyx_state[2])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(1, 13, __pyx_L1_error)
   }
-  __pyx_t_4 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
-  __pyx_t_5 = ((__pyx_t_4 > 2) != 0);
-  if (__pyx_t_5) {
+  __pyx_t_3 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_4 = ((__pyx_t_3 > 2) != 0);
+  if (__pyx_t_4) {
   } else {
-    __pyx_t_3 = __pyx_t_5;
+    __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_5 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
-  __pyx_t_6 = (__pyx_t_5 != 0);
-  __pyx_t_3 = __pyx_t_6;
+  __pyx_t_4 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_4 != 0);
+  __pyx_t_2 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
-  if (__pyx_t_3) {
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":14
  *     __pyx_result.key = __pyx_state[0]; __pyx_result.str = __pyx_state[1]
  *     if len(__pyx_state) > 2 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[2])             # <<<<<<<<<<<<<<
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_update); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 14, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_v___pyx_state == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(1, 14, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 14, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_9 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_9)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_9);
+    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_8 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_7);
-    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "(tree fragment)":13
  * cdef __pyx_unpickle_StringWithKey__set_state(StringWithKey __pyx_result, tuple __pyx_state):
  *     __pyx_result.key = __pyx_state[0]; __pyx_result.str = __pyx_state[1]
  *     if len(__pyx_state) > 2 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
  *         __pyx_result.__dict__.update(__pyx_state[2])
@@ -2733,17 +3543,17 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_StringWithKey__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -2757,28 +3567,49 @@
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
   p = ((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)o);
   p->__pyx_vtab = __pyx_vtabptr_7camSort_10stringSort_StringWithKey;
   p->str = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  p->key = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_7camSort_10stringSort_StringWithKey(PyObject *o) {
   struct __pyx_obj_7camSort_10stringSort_StringWithKey *p = (struct __pyx_obj_7camSort_10stringSort_StringWithKey *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
+  PyObject_GC_UnTrack(o);
   Py_CLEAR(p->str);
+  Py_CLEAR(p->key);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
+static int __pyx_tp_traverse_7camSort_10stringSort_StringWithKey(PyObject *o, visitproc v, void *a) {
+  int e;
+  struct __pyx_obj_7camSort_10stringSort_StringWithKey *p = (struct __pyx_obj_7camSort_10stringSort_StringWithKey *)o;
+  if (p->key) {
+    e = (*v)(p->key, a); if (e) return e;
+  }
+  return 0;
+}
+
+static int __pyx_tp_clear_7camSort_10stringSort_StringWithKey(PyObject *o) {
+  PyObject* tmp;
+  struct __pyx_obj_7camSort_10stringSort_StringWithKey *p = (struct __pyx_obj_7camSort_10stringSort_StringWithKey *)o;
+  tmp = ((PyObject*)p->key);
+  p->key = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  return 0;
+}
+
 static PyObject *__pyx_getprop_7camSort_10stringSort_13StringWithKey_str(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_7camSort_10stringSort_13StringWithKey_3str_1__get__(o);
 }
 
 static int __pyx_setprop_7camSort_10stringSort_13StringWithKey_str(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
   if (v) {
     return __pyx_pw_7camSort_10stringSort_13StringWithKey_3str_3__set__(o, v);
@@ -2793,16 +3624,15 @@
 }
 
 static int __pyx_setprop_7camSort_10stringSort_13StringWithKey_key(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
   if (v) {
     return __pyx_pw_7camSort_10stringSort_13StringWithKey_3key_3__set__(o, v);
   }
   else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
+    return __pyx_pw_7camSort_10stringSort_13StringWithKey_3key_5__del__(o);
   }
 }
 
 static PyMethodDef __pyx_methods_7camSort_10stringSort_StringWithKey[] = {
   {"__reduce_cython__", (PyCFunction)__pyx_pw_7camSort_10stringSort_13StringWithKey_3__reduce_cython__, METH_NOARGS, 0},
   {"__setstate_cython__", (PyCFunction)__pyx_pw_7camSort_10stringSort_13StringWithKey_5__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
@@ -2840,18 +3670,18 @@
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  0, /*tp_traverse*/
-  0, /*tp_clear*/
+  __pyx_tp_traverse_7camSort_10stringSort_StringWithKey, /*tp_traverse*/
+  __pyx_tp_clear_7camSort_10stringSort_StringWithKey, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_7camSort_10stringSort_StringWithKey, /*tp_methods*/
   0, /*tp_members*/
   __pyx_getsets_7camSort_10stringSort_StringWithKey, /*tp_getset*/
@@ -2928,26 +3758,33 @@
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_s_Incompatible_checksums_s_vs_0xef, __pyx_k_Incompatible_checksums_s_vs_0xef, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xef), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_StringWithKey, __pyx_k_StringWithKey, sizeof(__pyx_k_StringWithKey), 0, 0, 1, 1},
+  {&__pyx_n_u_alpha, __pyx_k_alpha, sizeof(__pyx_k_alpha), 0, 1, 0, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_attrgetter, __pyx_k_attrgetter, sizeof(__pyx_k_attrgetter), 0, 0, 1, 1},
+  {&__pyx_n_s_byAlphabet, __pyx_k_byAlphabet, sizeof(__pyx_k_byAlphabet), 0, 0, 1, 1},
   {&__pyx_n_s_byLength, __pyx_k_byLength, sizeof(__pyx_k_byLength), 0, 0, 1, 1},
+  {&__pyx_n_s_byLengthAndAlphabet, __pyx_k_byLengthAndAlphabet, sizeof(__pyx_k_byLengthAndAlphabet), 0, 0, 1, 1},
   {&__pyx_n_s_camSort_stringSort, __pyx_k_camSort_stringSort, sizeof(__pyx_k_camSort_stringSort), 0, 0, 1, 1},
   {&__pyx_kp_s_camSort_stringSort_pyx, __pyx_k_camSort_stringSort_pyx, sizeof(__pyx_k_camSort_stringSort_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_input_list, __pyx_k_input_list, sizeof(__pyx_k_input_list), 0, 0, 1, 1},
   {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
   {&__pyx_n_u_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 1, 0, 1},
+  {&__pyx_n_s_key_type, __pyx_k_key_type, sizeof(__pyx_k_key_type), 0, 0, 1, 1},
+  {&__pyx_n_u_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 1, 0, 1},
+  {&__pyx_n_u_length_and_alpha, __pyx_k_length_and_alpha, sizeof(__pyx_k_length_and_alpha), 0, 1, 0, 1},
+  {&__pyx_n_s_lower, __pyx_k_lower, sizeof(__pyx_k_lower), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_n_s_operator, __pyx_k_operator, sizeof(__pyx_k_operator), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
@@ -2968,45 +3805,69 @@
   {&__pyx_n_s_str, __pyx_k_str, sizeof(__pyx_k_str), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 36, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "camSort/stringSort.pyx":20
- *         return length * 10000 + sum
+  /* "camSort/stringSort.pyx":32
+ *         return length * 10000 + self.calculate_key(str)
  * 
  * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
-  __pyx_tuple_ = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLength, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLength, 32, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 32, __pyx_L1_error)
+
+  /* "camSort/stringSort.pyx":39
+ *     return [s.str for s in sorted_array]
+ * 
+ * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
+ *     cdef int n = len(input_list)
+ *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
+ */
+  __pyx_tuple__3 = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLengthAndAlphabet, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 39, __pyx_L1_error)
+
+  /* "camSort/stringSort.pyx":46
+ *     return [s.str for s in sorted_array]
+ * 
+ * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
+ *     cdef int n = len(input_list)
+ *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
+ */
+  __pyx_tuple__5 = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byAlphabet, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 46, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__3 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StringWithKey, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StringWithKey, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -3055,14 +3916,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_7camSort_10stringSort_StringWithKey = &__pyx_vtable_7camSort_10stringSort_StringWithKey;
   __pyx_vtable_7camSort_10stringSort_StringWithKey.calculate_key = (PY_LONG_LONG (*)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *))__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key;
+  __pyx_vtable_7camSort_10stringSort_StringWithKey.calculate_key_alpha = (PyObject *(*)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *))__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_alpha;
+  __pyx_vtable_7camSort_10stringSort_StringWithKey.calculate_key_length_alpha = (PY_LONG_LONG (*)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *))__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key_length_alpha;
   if (PyType_Ready(&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7camSort_10stringSort_StringWithKey.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7camSort_10stringSort_StringWithKey.tp_dictoffset && __pyx_type_7camSort_10stringSort_StringWithKey.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7camSort_10stringSort_StringWithKey.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
@@ -3320,32 +4183,56 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_attrgetter, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "camSort/stringSort.pyx":20
- *         return length * 10000 + sum
+  /* "camSort/stringSort.pyx":32
+ *         return length * 10000 + self.calculate_key(str)
  * 
  * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_1byLength, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_1byLength, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLength, __pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLength, __pyx_t_2) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "camSort/stringSort.pyx":39
+ *     return [s.str for s in sorted_array]
+ * 
+ * def byLengthAndAlphabet(input_list):             # <<<<<<<<<<<<<<
+ *     cdef int n = len(input_list)
+ *     cdef list array = [StringWithKey(s, 'length_and_alpha') for s in input_list]
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_3byLengthAndAlphabet, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLengthAndAlphabet, __pyx_t_2) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "camSort/stringSort.pyx":46
+ *     return [s.str for s in sorted_array]
+ * 
+ * def byAlphabet(input_list):             # <<<<<<<<<<<<<<
+ *     cdef int n = len(input_list)
+ *     cdef list array = [StringWithKey(s, 'alpha') for s in input_list]
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_5byAlphabet, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byAlphabet, __pyx_t_2) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_3__pyx_unpickle_StringWithKey, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_7__pyx_unpickle_StringWithKey, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_StringWithKey, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "camSort/stringSort.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * from operator import attrgetter
@@ -3565,14 +4452,163 @@
     }
     PyErr_Format(PyExc_TypeError,
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
+}
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
+}
+
 /* UnicodeAsUCS4 */
 static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject* x) {
    Py_ssize_t length;
    #if CYTHON_PEP393_ENABLED
    length = PyUnicode_GET_LENGTH(x);
    if (likely(length == 1)) {
        return PyUnicode_READ_CHAR(x, 0);
@@ -3691,151 +4727,14 @@
     }
 #ifdef WITH_THREAD
     if (nogil)
         PyGILState_Release(state);
 #endif
 }
 
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-}
-#endif
-
-/* GetAttr */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
-#if CYTHON_USE_TYPE_SLOTS
-#if PY_MAJOR_VERSION >= 3
-    if (likely(PyUnicode_Check(n)))
-#else
-    if (likely(PyString_Check(n)))
-#endif
-        return __Pyx_PyObject_GetAttrStr(o, n);
-#endif
-    return PyObject_GetAttr(o, n);
-}
-
-/* GetAttr3 */
-static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        return NULL;
-    __Pyx_PyErr_Clear();
-    Py_INCREF(d);
-    return d;
-}
-static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
-    PyObject *r = __Pyx_GetAttr(o, n);
-    return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
-}
-
-/* PyDictVersioning */
-#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
-    PyObject *dict = Py_TYPE(obj)->tp_dict;
-    return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
-}
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
-    PyObject **dictptr = NULL;
-    Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
-    if (offset) {
-#if CYTHON_COMPILING_IN_CPYTHON
-        dictptr = (likely(offset > 0)) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
-#else
-        dictptr = _PyObject_GetDictPtr(obj);
-#endif
-    }
-    return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
-}
-static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
-    PyObject *dict = Py_TYPE(obj)->tp_dict;
-    if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
-        return 0;
-    return obj_dict_version == __Pyx_get_object_dict_version(obj);
-}
-#endif
-
-/* GetModuleGlobalName */
-#if CYTHON_USE_DICT_VERSIONS
-static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
-#else
-static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
-#endif
-{
-    PyObject *result;
-#if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
-    result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    } else if (unlikely(PyErr_Occurred())) {
-        return NULL;
-    }
-#else
-    result = PyDict_GetItem(__pyx_d, name);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    }
-#endif
-#else
-    result = PyObject_GetItem(__pyx_d, name);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    }
-    PyErr_Clear();
-#endif
-    return __Pyx_GetBuiltinName(name);
-}
-
-/* PyCFunctionFastCall */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
-    }
-}
-#endif
-
 /* PyFunctionFastCall */
 #if CYTHON_FAST_PYCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
@@ -3987,14 +4886,59 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
+/* PyObjectCallNoArg */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+#if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+    }
+#endif
+#ifdef __Pyx_CyFunction_USED
+    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+#else
+    if (likely(PyCFunction_Check(func)))
+#endif
+    {
+        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+            return __Pyx_PyObject_CallMethO(func, NULL);
+        }
+    }
+    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
+}
+#endif
+
+/* PyCFunctionFastCall */
+#if CYTHON_FAST_PYCCALL
+static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
+    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
+    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
+    PyObject *self = PyCFunction_GET_SELF(func);
+    int flags = PyCFunction_GET_FLAGS(func);
+    assert(PyCFunction_Check(func));
+    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
+    assert(nargs >= 0);
+    assert(nargs == 0 || args != NULL);
+    /* _PyCFunction_FastCallDict() must not be called with an exception set,
+       because it may clear it (directly or indirectly) and so the
+       caller loses its exception */
+    assert(!PyErr_Occurred());
+    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
+        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
+    } else {
+        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
+    }
+}
+#endif
+
 /* PyObjectCallOneArg */
 #if CYTHON_COMPILING_IN_CPYTHON
 static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *result;
     PyObject *args = PyTuple_New(1);
     if (unlikely(!args)) return NULL;
     Py_INCREF(arg);
@@ -4027,14 +4971,128 @@
     if (unlikely(!args)) return NULL;
     result = __Pyx_PyObject_Call(func, args, NULL);
     Py_DECREF(args);
     return result;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    PyObject *exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+    if (unlikely(PyTuple_Check(err)))
+        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+}
+#endif
+
+/* GetAttr */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
+#if CYTHON_USE_TYPE_SLOTS
+#if PY_MAJOR_VERSION >= 3
+    if (likely(PyUnicode_Check(n)))
+#else
+    if (likely(PyString_Check(n)))
+#endif
+        return __Pyx_PyObject_GetAttrStr(o, n);
+#endif
+    return PyObject_GetAttr(o, n);
+}
+
+/* GetAttr3 */
+static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        return NULL;
+    __Pyx_PyErr_Clear();
+    Py_INCREF(d);
+    return d;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
+    PyObject *r = __Pyx_GetAttr(o, n);
+    return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
+}
+
+/* PyDictVersioning */
+#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
+}
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
+    PyObject **dictptr = NULL;
+    Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
+    if (offset) {
+#if CYTHON_COMPILING_IN_CPYTHON
+        dictptr = (likely(offset > 0)) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
+#else
+        dictptr = _PyObject_GetDictPtr(obj);
+#endif
+    }
+    return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
+}
+static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
+        return 0;
+    return obj_dict_version == __Pyx_get_object_dict_version(obj);
+}
+#endif
+
+/* GetModuleGlobalName */
+#if CYTHON_USE_DICT_VERSIONS
+static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
+#else
+static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
+#endif
+{
+    PyObject *result;
+#if !CYTHON_AVOID_BORROWED_REFS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+    result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
+    } else if (unlikely(PyErr_Occurred())) {
+        return NULL;
+    }
+#else
+    result = PyDict_GetItem(__pyx_d, name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
+    }
+#endif
+#else
+    result = PyObject_GetItem(__pyx_d, name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
+    }
+    PyErr_Clear();
+#endif
+    return __Pyx_GetBuiltinName(name);
+}
+
 /* PyObjectCall2Args */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
@@ -4780,14 +5838,36 @@
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
+/* CIntFromPyVerify */
+#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
+#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
+#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
+    {\
+        func_type value = func_value;\
+        if (sizeof(target_type) < sizeof(func_type)) {\
+            if (unlikely(value != (func_type) (target_type) value)) {\
+                func_type zero = 0;\
+                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
+                    return (target_type) -1;\
+                if (is_unsigned && unlikely(value < zero))\
+                    goto raise_neg_overflow;\
+                else\
+                    goto raise_overflow;\
+            }\
+        }\
+        return (target_type) value;\
+    }
+
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value) {
     const PY_LONG_LONG neg_one = (PY_LONG_LONG) ((PY_LONG_LONG) 0 - (PY_LONG_LONG) 1), const_zero = (PY_LONG_LONG) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(PY_LONG_LONG) < sizeof(long)) {
             return PyInt_FromLong((long) value);
@@ -4811,36 +5891,14 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(PY_LONG_LONG),
                                      little, !is_unsigned);
     }
 }
 
-/* CIntFromPyVerify */
-#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
-#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
-#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
-    {\
-        func_type value = func_value;\
-        if (sizeof(target_type) < sizeof(func_type)) {\
-            if (unlikely(value != (func_type) (target_type) value)) {\
-                func_type zero = 0;\
-                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
-                    return (target_type) -1;\
-                if (is_unsigned && unlikely(value < zero))\
-                    goto raise_neg_overflow;\
-                else\
-                    goto raise_overflow;\
-            }\
-        }\
-        return (target_type) value;\
-    }
-
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
     const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
@@ -4865,203 +5923,14 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE PY_LONG_LONG __Pyx_PyInt_As_PY_LONG_LONG(PyObject *x) {
-    const PY_LONG_LONG neg_one = (PY_LONG_LONG) ((PY_LONG_LONG) 0 - (PY_LONG_LONG) 1), const_zero = (PY_LONG_LONG) 0;
-    const int is_unsigned = neg_one > const_zero;
-#if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_Check(x))) {
-        if (sizeof(PY_LONG_LONG) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, PyInt_AS_LONG(x))
-        } else {
-            long val = PyInt_AS_LONG(x);
-            if (is_unsigned && unlikely(val < 0)) {
-                goto raise_neg_overflow;
-            }
-            return (PY_LONG_LONG) val;
-        }
-    } else
-#endif
-    if (likely(PyLong_Check(x))) {
-        if (is_unsigned) {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (PY_LONG_LONG) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(PY_LONG_LONG) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(PY_LONG_LONG) >= 2 * PyLong_SHIFT) {
-                            return (PY_LONG_LONG) (((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(PY_LONG_LONG) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(PY_LONG_LONG) >= 3 * PyLong_SHIFT) {
-                            return (PY_LONG_LONG) (((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(PY_LONG_LONG) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(PY_LONG_LONG) >= 4 * PyLong_SHIFT) {
-                            return (PY_LONG_LONG) (((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
-                        }
-                    }
-                    break;
-            }
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-            if (unlikely(Py_SIZE(x) < 0)) {
-                goto raise_neg_overflow;
-            }
-#else
-            {
-                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                if (unlikely(result < 0))
-                    return (PY_LONG_LONG) -1;
-                if (unlikely(result == 1))
-                    goto raise_neg_overflow;
-            }
-#endif
-            if (sizeof(PY_LONG_LONG) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, unsigned long, PyLong_AsUnsignedLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(PY_LONG_LONG) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
-#endif
-            }
-        } else {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (PY_LONG_LONG) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(PY_LONG_LONG,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(PY_LONG_LONG) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                            return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                        }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(PY_LONG_LONG) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                            return (PY_LONG_LONG) ((((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                        }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                            return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(PY_LONG_LONG) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                            return (PY_LONG_LONG) ((((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                        }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                            return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(PY_LONG_LONG) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                            return (PY_LONG_LONG) ((((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                        }
-                    }
-                    break;
-            }
-#endif
-            if (sizeof(PY_LONG_LONG) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, long, PyLong_AsLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(PY_LONG_LONG) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, PY_LONG_LONG, PyLong_AsLongLong(x))
-#endif
-            }
-        }
-        {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
-            PY_LONG_LONG val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
- #endif
-            if (likely(v)) {
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
-#endif
-            return (PY_LONG_LONG) -1;
-        }
-    } else {
-        PY_LONG_LONG val;
-        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (PY_LONG_LONG) -1;
-        val = __Pyx_PyInt_As_PY_LONG_LONG(tmp);
-        Py_DECREF(tmp);
-        return val;
-    }
-raise_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to PY_LONG_LONG");
-    return (PY_LONG_LONG) -1;
-raise_neg_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to PY_LONG_LONG");
-    return (PY_LONG_LONG) -1;
-}
-
-/* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
     const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
```

### Comparing `camSort-0.2.8/camSort.egg-info/PKG-INFO` & `camSort-0.2.9/camSort.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camSort
-Version: 0.2.8
+Version: 0.2.9
 Summary: make sorted() fast for strings
 Home-page: UNKNOWN
 Author: ['cameronbae / cameron jay']
 Author-email: <contact@camjay.io>
 License: UNKNOWN
 Description: 
         # camSort
```

### Comparing `camSort-0.2.8/setup.py` & `camSort-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
 
     name="camSort",
-    version="0.2.8",
+    version="0.2.9",
     install_requires=["setuptools", "wheel", "cython"],
 
     ext_modules = cythonize(['camSort/stringSort.pyx']),
 
     author=["cameronbae / cameron jay"],
     author_email="<contact@camjay.io>",
     description="make sorted() fast for strings",
```

