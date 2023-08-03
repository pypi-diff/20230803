# Comparing `tmp/dfv-0.8.0.tar.gz` & `tmp/dfv-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfv-0.8.0.tar", max compression
+gzip compressed data, was "dfv-0.9.0.tar", max compression
```

## Comparing `dfv-0.8.0.tar` & `dfv-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0    17876 2023-08-02 20:07:26.193267 dfv-0.8.0/dfv/__init__.py
--rw-r--r--   0        0        0    29012 2023-08-02 20:07:54.981616 dfv-0.8.0/dfv/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10456 2023-07-31 19:21:19.730323 dfv-0.8.0/dfv/__pycache__/test_element.cpython-311.pyc
--rw-r--r--   0        0        0     8642 2023-07-29 08:01:02.515193 dfv-0.8.0/dfv/__pycache__/test_form.cpython-311.pyc
--rw-r--r--   0        0        0    26025 2023-07-29 07:35:17.728831 dfv-0.8.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc
--rw-r--r--   0        0        0     4496 2023-08-02 19:49:36.096341 dfv-0.8.0/dfv/__pycache__/test_view.cpython-311.pyc
--rw-r--r--   0        0        0     3349 2023-07-02 06:35:19.618381 dfv-0.8.0/dfv/static/dfv.js
--rw-r--r--   0        0        0       10 2023-07-10 11:13:07.132615 dfv-0.8.0/dfv/templates/dfv/tests/TemplateResponse.html
--rw-r--r--   0        0        0        0 2023-03-23 19:33:22.527857 dfv-0.8.0/dfv/templatetags/__init__.py
--rw-r--r--   0        0        0      165 2023-07-01 11:11:20.768600 dfv-0.8.0/dfv/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      764 2023-07-01 11:32:03.019367 dfv-0.8.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc
--rw-r--r--   0        0        0      326 2023-07-01 11:32:01.379348 dfv-0.8.0/dfv/templatetags/dfv.py
--rw-r--r--   0        0        0     4328 2023-07-31 19:19:29.401041 dfv-0.8.0/dfv/test_element.py
--rw-r--r--   0        0        0     3340 2023-07-29 08:01:00.971175 dfv-0.8.0/dfv/test_form.py
--rw-r--r--   0        0        0     8657 2023-07-29 07:35:17.128824 dfv-0.8.0/dfv/test_params_to_args.py
--rw-r--r--   0        0        0     1646 2023-08-02 19:49:35.828337 dfv-0.8.0/dfv/test_view.py
--rw-r--r--   0        0        0     1438 2023-08-02 20:07:31.369330 dfv-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 dfv-0.8.0/setup.py
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 dfv-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    18140 2023-08-03 20:01:49.636175 dfv-0.9.0/dfv/__init__.py
+-rw-r--r--   0        0        0    29289 2023-08-03 20:02:07.700378 dfv-0.9.0/dfv/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10456 2023-07-31 19:21:19.730323 dfv-0.9.0/dfv/__pycache__/test_element.cpython-311.pyc
+-rw-r--r--   0        0        0     8943 2023-08-03 20:11:45.546785 dfv-0.9.0/dfv/__pycache__/test_form.cpython-311.pyc
+-rw-r--r--   0        0        0    26094 2023-08-03 20:14:36.564782 dfv-0.9.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc
+-rw-r--r--   0        0        0     5515 2023-08-03 20:02:07.984381 dfv-0.9.0/dfv/__pycache__/test_view.cpython-311.pyc
+-rw-r--r--   0        0        0     1079 2023-08-03 20:08:08.064405 dfv-0.9.0/dfv/__pycache__/testutils.cpython-311.pyc
+-rw-r--r--   0        0        0     3349 2023-07-02 06:35:19.618381 dfv-0.9.0/dfv/static/dfv.js
+-rw-r--r--   0        0        0       10 2023-07-10 11:13:07.132615 dfv-0.9.0/dfv/templates/dfv/tests/TemplateResponse.html
+-rw-r--r--   0        0        0        0 2023-03-23 19:33:22.527857 dfv-0.9.0/dfv/templatetags/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-01 11:11:20.768600 dfv-0.9.0/dfv/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      764 2023-07-01 11:32:03.019367 dfv-0.9.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc
+-rw-r--r--   0        0        0      326 2023-07-01 11:32:01.379348 dfv-0.9.0/dfv/templatetags/dfv.py
+-rw-r--r--   0        0        0     4328 2023-07-31 19:19:29.401041 dfv-0.9.0/dfv/test_element.py
+-rw-r--r--   0        0        0     3649 2023-08-03 20:11:44.550774 dfv-0.9.0/dfv/test_form.py
+-rw-r--r--   0        0        0     8583 2023-08-03 20:13:39.056111 dfv-0.9.0/dfv/test_params_to_args.py
+-rw-r--r--   0        0        0     2306 2023-08-03 20:02:07.184372 dfv-0.9.0/dfv/test_view.py
+-rw-r--r--   0        0        0      538 2023-08-03 20:07:56.000273 dfv-0.9.0/dfv/testutils.py
+-rw-r--r--   0        0        0     1436 2023-08-03 20:14:45.228884 dfv-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 dfv-0.9.0/setup.py
+-rw-r--r--   0        0        0      536 1970-01-01 00:00:00.000000 dfv-0.9.0/PKG-INFO
```

### Comparing `dfv-0.8.0/dfv/__init__.py` & `dfv-0.9.0/dfv/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,23 +185,29 @@
         return inner
 
     return decorator
 
 
 def is_view_fn_request_target(request: HttpRequest):
     stack = get_view_fn_call_stack_from_request(request, create=False)
-    return stack is None or len(stack) == 1
+    if stack is None:
+        raise Exception("This function can only be called from within a DFV view.")
+    if len(stack) != 1:
+        return False
+
+    called_view: Callable = stack[0]
+    return called_view.__qualname__ == request.resolver_match.func.__qualname__
 
 
 def is_head(request: HttpRequest):
     return is_view_fn_request_target(request) and request.method == "HEAD"
 
 
 def is_get(request: HttpRequest):
-    return request.method == "GET"
+    return is_view_fn_request_target(request) and request.method == "GET"
 
 
 def is_post(request: HttpRequest):
     return is_view_fn_request_target(request) and request.method == "POST"
 
 
 def is_put(request: HttpRequest):
```

### Comparing `dfv-0.8.0/dfv/__pycache__/__init__.cpython-311.pyc` & `dfv-0.9.0/dfv/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x7eb7ca64 (Wed Aug  2 20:07:26 2023 UTC)
-files sz: 17876
+moddate:  0xad07cc64 (Thu Aug  3 20:01:49 2023 UTC)
+files sz: 18140
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 14
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -401,329 +401,329 @@
    190         748 LOAD_CONST              29 ('request')
                750 LOAD_NAME               23 (HttpRequest)
                752 BUILD_TUPLE              2
                754 LOAD_CONST              36 (<code object is_view_fn_request_target, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 190>)
                756 MAKE_FUNCTION            4 (annotations)
                758 STORE_NAME              46 (is_view_fn_request_target)
    
-   195         760 LOAD_CONST              29 ('request')
+   201         760 LOAD_CONST              29 ('request')
                762 LOAD_NAME               23 (HttpRequest)
                764 BUILD_TUPLE              2
-               766 LOAD_CONST              37 (<code object is_head, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 195>)
+               766 LOAD_CONST              37 (<code object is_head, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 201>)
                768 MAKE_FUNCTION            4 (annotations)
                770 STORE_NAME              47 (is_head)
    
-   199         772 LOAD_CONST              29 ('request')
+   205         772 LOAD_CONST              29 ('request')
                774 LOAD_NAME               23 (HttpRequest)
                776 BUILD_TUPLE              2
-               778 LOAD_CONST              38 (<code object is_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 199>)
+               778 LOAD_CONST              38 (<code object is_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 205>)
                780 MAKE_FUNCTION            4 (annotations)
                782 STORE_NAME              48 (is_get)
    
-   203         784 LOAD_CONST              29 ('request')
+   209         784 LOAD_CONST              29 ('request')
                786 LOAD_NAME               23 (HttpRequest)
                788 BUILD_TUPLE              2
-               790 LOAD_CONST              39 (<code object is_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 203>)
+               790 LOAD_CONST              39 (<code object is_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 209>)
                792 MAKE_FUNCTION            4 (annotations)
                794 STORE_NAME              49 (is_post)
    
-   207         796 LOAD_CONST              29 ('request')
+   213         796 LOAD_CONST              29 ('request')
                798 LOAD_NAME               23 (HttpRequest)
                800 BUILD_TUPLE              2
-               802 LOAD_CONST              40 (<code object is_put, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 207>)
+               802 LOAD_CONST              40 (<code object is_put, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 213>)
                804 MAKE_FUNCTION            4 (annotations)
                806 STORE_NAME              50 (is_put)
    
-   211         808 LOAD_CONST              29 ('request')
+   217         808 LOAD_CONST              29 ('request')
                810 LOAD_NAME               23 (HttpRequest)
                812 BUILD_TUPLE              2
-               814 LOAD_CONST              41 (<code object is_patch, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 211>)
+               814 LOAD_CONST              41 (<code object is_patch, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 217>)
                816 MAKE_FUNCTION            4 (annotations)
                818 STORE_NAME              51 (is_patch)
    
-   215         820 LOAD_CONST              29 ('request')
+   221         820 LOAD_CONST              29 ('request')
                822 LOAD_NAME               23 (HttpRequest)
                824 BUILD_TUPLE              2
-               826 LOAD_CONST              42 (<code object is_delete, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 215>)
+               826 LOAD_CONST              42 (<code object is_delete, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 221>)
                828 MAKE_FUNCTION            4 (annotations)
                830 STORE_NAME              52 (is_delete)
    
-   226         832 LOAD_CONST              21 (False)
+   232         832 LOAD_CONST              21 (False)
    
-   227         834 LOAD_CONST              20 (True)
+   233         834 LOAD_CONST              20 (True)
    
-   224         836 LOAD_CONST              43 (('auto_param', 'auto_form'))
+   230         836 LOAD_CONST              43 (('auto_param', 'auto_form'))
                838 BUILD_CONST_KEY_MAP      2
                840 LOAD_CONST              44 ('auto_param')
    
-   226         842 LOAD_NAME               44 (bool)
+   232         842 LOAD_NAME               44 (bool)
                844 LOAD_NAME               10 (Literal)
                846 LOAD_CONST              45 (('get', 'post'))
                848 BINARY_SUBSCR
                858 BINARY_OP                7 (|)
    
-   224         862 LOAD_CONST              46 ('auto_form')
+   230         862 LOAD_CONST              46 ('auto_form')
    
-   227         864 LOAD_NAME               11 (Optional)
+   233         864 LOAD_NAME               11 (Optional)
                866 LOAD_NAME               44 (bool)
                868 LOAD_NAME               38 (str)
                870 BINARY_OP                7 (|)
                874 BINARY_SUBSCR
    
-   224         884 LOAD_CONST              15 ('return')
+   230         884 LOAD_CONST              15 ('return')
    
-   228         886 LOAD_NAME                9 (Callable)
+   234         886 LOAD_NAME                9 (Callable)
                888 LOAD_NAME                9 (Callable)
                890 LOAD_NAME               32 (P)
                892 LOAD_NAME               33 (R)
                894 BUILD_TUPLE              2
                896 BINARY_SUBSCR
                906 BUILD_LIST               1
                908 LOAD_NAME                9 (Callable)
                910 LOAD_NAME               32 (P)
                912 LOAD_NAME               33 (R)
                914 BUILD_TUPLE              2
                916 BINARY_SUBSCR
                926 BUILD_TUPLE              2
                928 BINARY_SUBSCR
    
-   224         938 BUILD_TUPLE              6
-               940 LOAD_CONST              47 (<code object inject_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 224>)
+   230         938 BUILD_TUPLE              6
+               940 LOAD_CONST              47 (<code object inject_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 230>)
                942 MAKE_FUNCTION            6 (kwdefaults, annotations)
                944 STORE_NAME              53 (inject_args)
    
-   258         946 LOAD_NAME               53 (inject_args)
+   264         946 LOAD_NAME               53 (inject_args)
                948 STORE_NAME              54 (_inject_args)
    
-   261         950 LOAD_NAME                0 (dataclasses)
+   267         950 LOAD_NAME                0 (dataclasses)
                952 LOAD_ATTR               55 (dataclass)
    
-   262         962 PUSH_NULL
+   268         962 PUSH_NULL
                964 LOAD_BUILD_CLASS
-               966 LOAD_CONST              48 (<code object InjectedParam, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 261>)
+               966 LOAD_CONST              48 (<code object InjectedParam, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 267>)
                968 MAKE_FUNCTION            0
                970 LOAD_CONST              49 ('InjectedParam')
                972 PRECALL                  2
                976 CALL                     2
    
-   261         986 PRECALL                  0
+   267         986 PRECALL                  0
                990 CALL                     0
    
-   262        1000 STORE_NAME              56 (InjectedParam)
+   268        1000 STORE_NAME              56 (InjectedParam)
    
-   279        1002 LOAD_CONST              50 ('view_fn')
+   285        1002 LOAD_CONST              50 ('view_fn')
    
-   280        1004 LOAD_NAME                9 (Callable)
+   286        1004 LOAD_NAME                9 (Callable)
               1006 LOAD_NAME                8 (Any)
               1008 BUILD_LIST               1
               1010 LOAD_NAME                8 (Any)
               1012 BUILD_TUPLE              2
               1014 BINARY_SUBSCR
    
-   279        1024 LOAD_CONST              51 ('ip')
+   285        1024 LOAD_CONST              51 ('ip')
    
-   281        1026 LOAD_NAME               56 (InjectedParam)
+   287        1026 LOAD_NAME               56 (InjectedParam)
    
-   279        1028 LOAD_CONST              52 ('name')
+   285        1028 LOAD_CONST              52 ('name')
    
-   282        1030 LOAD_NAME               38 (str)
+   288        1030 LOAD_NAME               38 (str)
    
-   279        1032 LOAD_CONST              53 ('parameter')
+   285        1032 LOAD_CONST              53 ('parameter')
    
-   283        1034 LOAD_NAME                2 (inspect)
+   289        1034 LOAD_NAME                2 (inspect)
               1036 LOAD_ATTR               57 (Parameter)
    
-   279        1046 BUILD_TUPLE              8
-              1048 LOAD_CONST              54 (<code object _setup_injected_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 279>)
+   285        1046 BUILD_TUPLE              8
+              1048 LOAD_CONST              54 (<code object _setup_injected_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 285>)
               1050 MAKE_FUNCTION            4 (annotations)
               1052 STORE_NAME              58 (_setup_injected_param)
    
-   306        1054 NOP
+   312        1054 NOP
    
-   302        1056 LOAD_CONST              81 ((True,))
+   308        1056 LOAD_CONST              81 ((True,))
               1058 LOAD_CONST              50 ('view_fn')
    
-   303        1060 LOAD_NAME                9 (Callable)
+   309        1060 LOAD_NAME                9 (Callable)
               1062 LOAD_NAME                8 (Any)
               1064 BUILD_LIST               1
               1066 LOAD_NAME                8 (Any)
               1068 BUILD_TUPLE              2
               1070 BINARY_SUBSCR
    
-   302        1080 LOAD_CONST              55 ('parameters')
+   308        1080 LOAD_CONST              55 ('parameters')
    
-   304        1082 LOAD_NAME               39 (list)
+   310        1082 LOAD_NAME               39 (list)
               1084 LOAD_NAME                2 (inspect)
               1086 LOAD_ATTR               57 (Parameter)
               1096 BINARY_SUBSCR
    
-   302        1106 LOAD_CONST              44 ('auto_param')
+   308        1106 LOAD_CONST              44 ('auto_param')
    
-   305        1108 LOAD_NAME               44 (bool)
+   311        1108 LOAD_NAME               44 (bool)
               1110 LOAD_NAME               10 (Literal)
               1112 LOAD_CONST              56 ('get')
               1114 BINARY_SUBSCR
               1124 BINARY_OP                7 (|)
               1128 LOAD_NAME               10 (Literal)
               1130 LOAD_CONST              57 ('post')
               1132 BINARY_SUBSCR
               1142 BINARY_OP                7 (|)
    
-   302        1146 LOAD_CONST              46 ('auto_form')
+   308        1146 LOAD_CONST              46 ('auto_form')
    
-   306        1148 LOAD_NAME               11 (Optional)
+   312        1148 LOAD_NAME               11 (Optional)
               1150 LOAD_NAME               44 (bool)
               1152 LOAD_NAME               38 (str)
               1154 BINARY_OP                7 (|)
               1158 BINARY_SUBSCR
    
-   302        1168 LOAD_CONST              15 ('return')
+   308        1168 LOAD_CONST              15 ('return')
    
-   307        1170 LOAD_NAME               59 (dict)
+   313        1170 LOAD_NAME               59 (dict)
               1172 LOAD_NAME               38 (str)
               1174 LOAD_NAME               56 (InjectedParam)
               1176 BUILD_TUPLE              2
               1178 BINARY_SUBSCR
    
-   302        1188 BUILD_TUPLE             10
-              1190 LOAD_CONST              58 (<code object _extract_injected_params, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 302>)
+   308        1188 BUILD_TUPLE             10
+              1190 LOAD_CONST              58 (<code object _extract_injected_params, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 308>)
               1192 MAKE_FUNCTION            5 (defaults, annotations)
               1194 STORE_NAME              60 (_extract_injected_params)
    
-   366        1196 LOAD_NAME                0 (dataclasses)
+   372        1196 LOAD_NAME                0 (dataclasses)
               1198 LOAD_ATTR               55 (dataclass)
    
-   367        1208 PUSH_NULL
+   373        1208 PUSH_NULL
               1210 LOAD_BUILD_CLASS
-              1212 LOAD_CONST              59 (<code object InjectedParamQuery, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 366>)
+              1212 LOAD_CONST              59 (<code object InjectedParamQuery, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 372>)
               1214 MAKE_FUNCTION            0
               1216 LOAD_CONST              60 ('InjectedParamQuery')
               1218 LOAD_NAME               56 (InjectedParam)
               1220 PRECALL                  3
               1224 CALL                     3
    
-   366        1234 PRECALL                  0
+   372        1234 PRECALL                  0
               1238 CALL                     0
    
-   367        1248 STORE_NAME              61 (InjectedParamQuery)
+   373        1248 STORE_NAME              61 (InjectedParamQuery)
    
-   414        1250 LOAD_NAME                0 (dataclasses)
+   420        1250 LOAD_NAME                0 (dataclasses)
               1252 LOAD_ATTR               55 (dataclass)
    
-   415        1262 PUSH_NULL
+   421        1262 PUSH_NULL
               1264 LOAD_BUILD_CLASS
-              1266 LOAD_CONST              61 (<code object InjectedParamQueryGet, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 414>)
+              1266 LOAD_CONST              61 (<code object InjectedParamQueryGet, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 420>)
               1268 MAKE_FUNCTION            0
               1270 LOAD_CONST              62 ('InjectedParamQueryGet')
               1272 LOAD_NAME               61 (InjectedParamQuery)
               1274 PRECALL                  3
               1278 CALL                     3
    
-   414        1288 PRECALL                  0
+   420        1288 PRECALL                  0
               1292 CALL                     0
    
-   415        1302 STORE_NAME              62 (InjectedParamQueryGet)
+   421        1302 STORE_NAME              62 (InjectedParamQueryGet)
    
-   427        1304 LOAD_NAME                0 (dataclasses)
+   433        1304 LOAD_NAME                0 (dataclasses)
               1306 LOAD_ATTR               55 (dataclass)
    
-   428        1316 PUSH_NULL
+   434        1316 PUSH_NULL
               1318 LOAD_BUILD_CLASS
-              1320 LOAD_CONST              63 (<code object InjectedParamQueryPost, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 427>)
+              1320 LOAD_CONST              63 (<code object InjectedParamQueryPost, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 433>)
               1322 MAKE_FUNCTION            0
               1324 LOAD_CONST              64 ('InjectedParamQueryPost')
               1326 LOAD_NAME               61 (InjectedParamQuery)
               1328 PRECALL                  3
               1332 CALL                     3
    
-   427        1342 PRECALL                  0
+   433        1342 PRECALL                  0
               1346 CALL                     0
    
-   428        1356 STORE_NAME              63 (InjectedParamQueryPost)
+   434        1356 STORE_NAME              63 (InjectedParamQueryPost)
    
-   440        1358 LOAD_CONST              82 ((None, True))
+   446        1358 LOAD_CONST              82 ((None, True))
               1360 LOAD_CONST              15 ('return')
               1362 LOAD_NAME                8 (Any)
               1364 BUILD_TUPLE              2
-              1366 LOAD_CONST              65 (<code object param_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 440>)
+              1366 LOAD_CONST              65 (<code object param_get, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 446>)
               1368 MAKE_FUNCTION            5 (defaults, annotations)
               1370 STORE_NAME              64 (param_get)
    
-   444        1372 LOAD_CONST              82 ((None, True))
+   450        1372 LOAD_CONST              82 ((None, True))
               1374 LOAD_CONST              15 ('return')
               1376 LOAD_NAME                8 (Any)
               1378 BUILD_TUPLE              2
-              1380 LOAD_CONST              66 (<code object param_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 444>)
+              1380 LOAD_CONST              66 (<code object param_post, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 450>)
               1382 MAKE_FUNCTION            5 (defaults, annotations)
               1384 STORE_NAME              65 (param_post)
    
-   448        1386 PUSH_NULL
+   454        1386 PUSH_NULL
               1388 LOAD_NAME                4 (typing)
               1390 LOAD_ATTR               66 (cast)
               1400 LOAD_NAME                8 (Any)
               1402 LOAD_CONST               1 (None)
               1404 PRECALL                  2
               1408 CALL                     2
               1418 LOAD_CONST              20 (True)
               1420 BUILD_TUPLE              2
               1422 LOAD_CONST              67 ('default')
               1424 LOAD_NAME               34 (T)
               1426 LOAD_CONST              15 ('return')
               1428 LOAD_NAME               34 (T)
               1430 BUILD_TUPLE              4
-              1432 LOAD_CONST              68 (<code object param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 448>)
+              1432 LOAD_CONST              68 (<code object param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 454>)
               1434 MAKE_FUNCTION            5 (defaults, annotations)
               1436 STORE_NAME              67 (param)
    
-   452        1438 LOAD_CONST              69 ('values')
+   458        1438 LOAD_CONST              69 ('values')
               1440 LOAD_NAME               39 (list)
               1442 LOAD_NAME                4 (typing)
               1444 LOAD_ATTR                8 (Any)
               1454 BINARY_SUBSCR
               1464 LOAD_CONST              70 ('target_type')
               1466 LOAD_NAME               68 (type)
               1468 BUILD_TUPLE              4
-              1470 LOAD_CONST              71 (<code object _convert_value_to_type, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 452>)
+              1470 LOAD_CONST              71 (<code object _convert_value_to_type, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 458>)
               1472 MAKE_FUNCTION            4 (annotations)
               1474 STORE_NAME              69 (_convert_value_to_type)
    
-   487        1476 PUSH_NULL
+   493        1476 PUSH_NULL
               1478 LOAD_BUILD_CLASS
-              1480 LOAD_CONST              72 (<code object InjectedParamForm, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 487>)
+              1480 LOAD_CONST              72 (<code object InjectedParamForm, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 493>)
               1482 MAKE_FUNCTION            0
               1484 LOAD_CONST              73 ('InjectedParamForm')
               1486 LOAD_NAME               56 (InjectedParam)
               1488 PRECALL                  3
               1492 CALL                     3
               1502 STORE_NAME              70 (InjectedParamForm)
    
-   533        1504 LOAD_CONST              15 ('return')
+   539        1504 LOAD_CONST              15 ('return')
               1506 LOAD_NAME                8 (Any)
               1508 BUILD_TUPLE              2
-              1510 LOAD_CONST              74 (<code object handle_form, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 533>)
+              1510 LOAD_CONST              74 (<code object handle_form, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 539>)
               1512 MAKE_FUNCTION            4 (annotations)
               1514 STORE_NAME              71 (handle_form)
    
-   542        1516 LOAD_CONST              75 ('querydict')
+   548        1516 LOAD_CONST              75 ('querydict')
               1518 LOAD_NAME               59 (dict)
               1520 LOAD_CONST              15 ('return')
               1522 LOAD_NAME               26 (QueryDict)
               1524 BUILD_TUPLE              4
-              1526 LOAD_CONST              76 (<code object querydict_key_removed, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 542>)
+              1526 LOAD_CONST              76 (<code object querydict_key_removed, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 548>)
               1528 MAKE_FUNCTION            4 (annotations)
               1530 STORE_NAME              72 (querydict_key_removed)
    
-   549        1532 LOAD_CONST              77 ('args')
+   555        1532 LOAD_CONST              77 ('args')
               1534 LOAD_NAME               39 (list)
               1536 LOAD_NAME                8 (Any)
               1538 BINARY_SUBSCR
               1548 LOAD_CONST              15 ('return')
               1550 LOAD_NAME               23 (HttpRequest)
               1552 BUILD_TUPLE              4
-              1554 LOAD_CONST              78 (<code object _get_request_from_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 549>)
+              1554 LOAD_CONST              78 (<code object _get_request_from_args, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 555>)
               1556 MAKE_FUNCTION            4 (annotations)
               1558 STORE_NAME              73 (_get_request_from_args)
               1560 LOAD_CONST               1 (None)
               1562 RETURN_VALUE
    consts
       0
       None
@@ -1750,66 +1750,94 @@
          cellvars   ('decorators', 'handle_args')
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'view'
          firstlineno 156
          lnotab 0x06060401040104012c027214
       code
          argcount  : 1
-         nlocals   : 2
+         nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c006401ac02a6020000ab02000000
-            00000000007d017c016400750070127403000000000000000000007c01a6
-            010000ab01000000000000000064036b02000000005300
+            00000000007d017c01800f7403000000000000000000006403a6010000ab
+            01000000000000000082017405000000000000000000007c01a6010000ab
+            01000000000000000064046b03000000007202640153007c016405190000
+            000000000000007d027c026a0300000000000000007c006a040000000000
+            0000006a0500000000000000006a0300000000000000006b020000000053
+            00
          190           0 RESUME                   0
          
          191           2 LOAD_GLOBAL              1 (NULL + get_view_fn_call_stack_from_request)
                       14 LOAD_FAST                0 (request)
                       16 LOAD_CONST               1 (False)
                       18 KW_NAMES                 2
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_FAST               1 (stack)
          
          192          36 LOAD_FAST                1 (stack)
-                      38 LOAD_CONST               0 (None)
-                      40 IS_OP                    0
-                      42 JUMP_IF_TRUE_OR_POP     18 (to 80)
-                      44 LOAD_GLOBAL              3 (NULL + len)
-                      56 LOAD_FAST                1 (stack)
-                      58 PRECALL                  1
-                      62 CALL                     1
-                      72 LOAD_CONST               3 (1)
-                      74 COMPARE_OP               2 (==)
-                 >>   80 RETURN_VALUE
+                      38 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 70)
+         
+         193          40 LOAD_GLOBAL              3 (NULL + Exception)
+                      52 LOAD_CONST               3 ('This function can only be called from within a DFV view.')
+                      54 PRECALL                  1
+                      58 CALL                     1
+                      68 RAISE_VARARGS            1
+         
+         194     >>   70 LOAD_GLOBAL              5 (NULL + len)
+                      82 LOAD_FAST                1 (stack)
+                      84 PRECALL                  1
+                      88 CALL                     1
+                      98 LOAD_CONST               4 (1)
+                     100 COMPARE_OP               3 (!=)
+                     106 POP_JUMP_FORWARD_IF_FALSE     2 (to 112)
+         
+         195         108 LOAD_CONST               1 (False)
+                     110 RETURN_VALUE
+         
+         197     >>  112 LOAD_FAST                1 (stack)
+                     114 LOAD_CONST               5 (0)
+                     116 BINARY_SUBSCR
+                     126 STORE_FAST               2 (called_view)
+         
+         198         128 LOAD_FAST                2 (called_view)
+                     130 LOAD_ATTR                3 (__qualname__)
+                     140 LOAD_FAST                0 (request)
+                     142 LOAD_ATTR                4 (resolver_match)
+                     152 LOAD_ATTR                5 (func)
+                     162 LOAD_ATTR                3 (__qualname__)
+                     172 COMPARE_OP               2 (==)
+                     178 RETURN_VALUE
          consts
             None
             False
             ('create',)
+            'This function can only be called from within a DFV view.'
             1
-         names      ('get_view_fn_call_stack_from_request', 'len')
-         varnames   ('request', 'stack')
+            0
+         names      ('get_view_fn_call_stack_from_request', 'Exception', 'len', '__qualname__', 'resolver_match', 'func')
+         varnames   ('request', 'stack', 'called_view')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_view_fn_request_target'
          firstlineno 190
-         lnotab 0x02012201
+         lnotab 0x0201220104011e01260104021001
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             006f0a7c006a01000000000000000064016b02000000005300
-         195           0 RESUME                   0
+         201           0 RESUME                   0
          
-         196           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+         202           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 JUMP_IF_FALSE_OR_POP    10 (to 52)
                       32 LOAD_FAST                0 (request)
                       34 LOAD_ATTR                1 (method)
                       44 LOAD_CONST               1 ('HEAD')
@@ -1820,51 +1848,58 @@
             'HEAD'
          names      ('is_view_fn_request_target', 'method')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_head'
-         firstlineno 195
+         firstlineno 201
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
-         stacksize : 2
+         stacksize : 3
          flags     : 3
-         code 0x97007c006a00000000000000000064016b02000000005300
-         199           0 RESUME                   0
+         code
+            0x97007401000000000000000000007c00a6010000ab0100000000000000
+            006f0a7c006a01000000000000000064016b02000000005300
+         205           0 RESUME                   0
          
-         200           2 LOAD_FAST                0 (request)
-                       4 LOAD_ATTR                0 (method)
-                      14 LOAD_CONST               1 ('GET')
-                      16 COMPARE_OP               2 (==)
-                      22 RETURN_VALUE
+         206           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+                      14 LOAD_FAST                0 (request)
+                      16 PRECALL                  1
+                      20 CALL                     1
+                      30 JUMP_IF_FALSE_OR_POP    10 (to 52)
+                      32 LOAD_FAST                0 (request)
+                      34 LOAD_ATTR                1 (method)
+                      44 LOAD_CONST               1 ('GET')
+                      46 COMPARE_OP               2 (==)
+                 >>   52 RETURN_VALUE
          consts
             None
             'GET'
-         names      ('method',)
+         names      ('is_view_fn_request_target', 'method')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_get'
-         firstlineno 199
+         firstlineno 205
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             006f0a7c006a01000000000000000064016b02000000005300
-         203           0 RESUME                   0
+         209           0 RESUME                   0
          
-         204           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+         210           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 JUMP_IF_FALSE_OR_POP    10 (to 52)
                       32 LOAD_FAST                0 (request)
                       34 LOAD_ATTR                1 (method)
                       44 LOAD_CONST               1 ('POST')
@@ -1875,27 +1910,27 @@
             'POST'
          names      ('is_view_fn_request_target', 'method')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_post'
-         firstlineno 203
+         firstlineno 209
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             006f0a7c006a01000000000000000064016b02000000005300
-         207           0 RESUME                   0
+         213           0 RESUME                   0
          
-         208           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+         214           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 JUMP_IF_FALSE_OR_POP    10 (to 52)
                       32 LOAD_FAST                0 (request)
                       34 LOAD_ATTR                1 (method)
                       44 LOAD_CONST               1 ('PUT')
@@ -1906,27 +1941,27 @@
             'PUT'
          names      ('is_view_fn_request_target', 'method')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_put'
-         firstlineno 207
+         firstlineno 213
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             006f0a7c006a01000000000000000064016b02000000005300
-         211           0 RESUME                   0
+         217           0 RESUME                   0
          
-         212           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+         218           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 JUMP_IF_FALSE_OR_POP    10 (to 52)
                       32 LOAD_FAST                0 (request)
                       34 LOAD_ATTR                1 (method)
                       44 LOAD_CONST               1 ('PATCH')
@@ -1937,27 +1972,27 @@
             'PATCH'
          names      ('is_view_fn_request_target', 'method')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_patch'
-         firstlineno 211
+         firstlineno 217
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             006f0a7c006a01000000000000000064016b02000000005300
-         215           0 RESUME                   0
+         221           0 RESUME                   0
          
-         216           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
+         222           2 LOAD_GLOBAL              1 (NULL + is_view_fn_request_target)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 JUMP_IF_FALSE_OR_POP    10 (to 52)
                       32 LOAD_FAST                0 (request)
                       34 LOAD_ATTR                1 (method)
                       44 LOAD_CONST               1 ('DELETE')
@@ -1968,15 +2003,15 @@
             'DELETE'
          names      ('is_view_fn_request_target', 'method')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'is_delete'
-         firstlineno 215
+         firstlineno 221
          lnotab 0x0201
       ('auto_param', 'auto_form')
       'auto_param'
       ('get', 'post')
       'auto_form'
       code
          argcount  : 0
@@ -1988,17 +2023,17 @@
             000000740400000000000000000000660219000000000000000000640274
             000000000000000000000074020000000000000000000074040000000000
             000000000066021900000000000000000066048801880066026403840c7d
             027c025300
                        0 MAKE_CELL                0 (auto_param)
                        2 MAKE_CELL                1 (auto_form)
          
-         224           4 RESUME                   0
+         230           4 RESUME                   0
          
-         229           6 LOAD_CONST               1 ('fn')
+         235           6 LOAD_CONST               1 ('fn')
                        8 LOAD_GLOBAL              0 (Callable)
                       20 LOAD_GLOBAL              2 (P)
                       32 LOAD_GLOBAL              4 (R)
                       44 BUILD_TUPLE              2
                       46 BINARY_SUBSCR
                       56 LOAD_CONST               2 ('return')
                       58 LOAD_GLOBAL              0 (Callable)
@@ -2006,19 +2041,19 @@
                       82 LOAD_GLOBAL              4 (R)
                       94 BUILD_TUPLE              2
                       96 BINARY_SUBSCR
                      106 BUILD_TUPLE              4
                      108 LOAD_CLOSURE             1 (auto_form)
                      110 LOAD_CLOSURE             0 (auto_param)
                      112 BUILD_TUPLE              2
-                     114 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 229>)
+                     114 LOAD_CONST               3 (<code object decorator, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 235>)
                      116 MAKE_FUNCTION           12 (annotations, closure)
                      118 STORE_FAST               2 (decorator)
          
-         254         120 LOAD_FAST                2 (decorator)
+         260         120 LOAD_FAST                2 (decorator)
                      122 RETURN_VALUE
          consts
             None
             'fn'
             'return'
             code
                argcount  : 1
@@ -2038,89 +2073,89 @@
                   04741600000000000000000000660688038800880466036405840ca60000
                   00ab0000000000000000007d027c025300
                              0 COPY_FREE_VARS           2
                              2 MAKE_CELL                0 (fn)
                              4 MAKE_CELL                3 (arg_names)
                              6 MAKE_CELL                4 (injected_params)
                
-               229           8 RESUME                   0
+               235           8 RESUME                   0
                
-               230          10 LOAD_GLOBAL              1 (NULL + list)
+               236          10 LOAD_GLOBAL              1 (NULL + list)
                
-               231          22 LOAD_GLOBAL              3 (NULL + inspect)
+               237          22 LOAD_GLOBAL              3 (NULL + inspect)
                             34 LOAD_ATTR                2 (signature)
                             44 LOAD_DEREF               0 (fn)
                             46 PRECALL                  1
                             50 CALL                     1
                             60 LOAD_ATTR                3 (parameters)
                             70 LOAD_METHOD              4 (values)
                             92 PRECALL                  0
                             96 CALL                     0
                
-               230         106 PRECALL                  1
+               236         106 PRECALL                  1
                            110 CALL                     1
                            120 STORE_FAST               1 (parameters)
                
-               233         122 LOAD_GLOBAL             11 (NULL + _extract_injected_params)
+               239         122 LOAD_GLOBAL             11 (NULL + _extract_injected_params)
                
-               234         134 LOAD_DEREF               0 (fn)
+               240         134 LOAD_DEREF               0 (fn)
                            136 LOAD_FAST                1 (parameters)
                            138 LOAD_DEREF               6 (auto_param)
                            140 LOAD_DEREF               5 (auto_form)
                
-               233         142 PRECALL                  4
+               239         142 PRECALL                  4
                            146 CALL                     4
                            156 STORE_DEREF              4 (injected_params)
                
-               236         158 LOAD_CONST               1 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 236>)
+               242         158 LOAD_CONST               1 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 242>)
                            160 MAKE_FUNCTION            0
                            162 LOAD_FAST                1 (parameters)
                            164 GET_ITER
                            166 PRECALL                  0
                            170 CALL                     0
                            180 STORE_DEREF              3 (arg_names)
                
-               238         182 LOAD_GLOBAL             13 (NULL + functools)
+               244         182 LOAD_GLOBAL             13 (NULL + functools)
                            194 LOAD_ATTR                7 (wraps)
                            204 LOAD_DEREF               0 (fn)
                            206 PRECALL                  1
                            210 CALL                     1
                
-               239         220 LOAD_CONST               2 ('args')
+               245         220 LOAD_CONST               2 ('args')
                            222 LOAD_GLOBAL             16 (P)
                            234 LOAD_ATTR                9 (args)
                            244 LOAD_CONST               3 ('kwargs')
                            246 LOAD_GLOBAL             16 (P)
                            258 LOAD_ATTR               10 (kwargs)
                            268 LOAD_CONST               4 ('return')
                            270 LOAD_GLOBAL             22 (R)
                            282 BUILD_TUPLE              6
                            284 LOAD_CLOSURE             3 (arg_names)
                            286 LOAD_CLOSURE             0 (fn)
                            288 LOAD_CLOSURE             4 (injected_params)
                            290 BUILD_TUPLE              3
-                           292 LOAD_CONST               5 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 238>)
+                           292 LOAD_CONST               5 (<code object inner, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 244>)
                            294 MAKE_FUNCTION           12 (annotations, closure)
                
-               238         296 PRECALL                  0
+               244         296 PRECALL                  0
                            300 CALL                     0
                
-               239         310 STORE_FAST               2 (inner)
+               245         310 STORE_FAST               2 (inner)
                
-               252         312 LOAD_FAST                2 (inner)
+               258         312 LOAD_FAST                2 (inner)
                            314 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     236           0 RESUME                   0
+                     242           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (p)
                                   10 LOAD_FAST                1 (p)
                                   12 LOAD_ATTR                0 (name)
                                   22 LIST_APPEND              2
@@ -2129,15 +2164,15 @@
                      consts
                      names      ('name',)
                      varnames   ('.0', 'p')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<listcomp>'
-                     firstlineno 236
+                     firstlineno 242
                      lnotab 0x
                   'args'
                   'kwargs'
                   'return'
                   code
                      argcount  : 0
                      nlocals   : 6
@@ -2155,90 +2190,90 @@
                         020000ab020000000000000000a6010000ab0100000000000000007c017c
                         0319000000000000000000a6020000ab0200000000000000007d057c0581
                         1c740b000000000000000000006a06000000000000000074100000000000
                         00000000007c05a6020000ab0200000000000000006302010053008c8602
                         0089077c0069007c01a4018e015300
                                    0 COPY_FREE_VARS           3
                      
-                     238           2 RESUME                   0
+                     244           2 RESUME                   0
                      
-                     240           4 LOAD_DEREF               6 (arg_names)
+                     246           4 LOAD_DEREF               6 (arg_names)
                                    6 LOAD_CONST               0 (None)
                                    8 LOAD_GLOBAL              1 (NULL + len)
                                   20 LOAD_FAST                0 (args)
                                   22 PRECALL                  1
                                   26 CALL                     1
                                   36 BUILD_SLICE              2
                                   38 BINARY_SUBSCR
                                   48 STORE_FAST               2 (supplied_args)
                      
-                     241          50 LOAD_DEREF               8 (injected_params)
+                     247          50 LOAD_DEREF               8 (injected_params)
                                   52 LOAD_METHOD              1 (items)
                                   74 PRECALL                  0
                                   78 CALL                     0
                                   88 GET_ITER
                              >>   90 FOR_ITER               133 (to 358)
                                   92 UNPACK_SEQUENCE          2
                                   96 STORE_FAST               3 (name)
                                   98 STORE_FAST               4 (ip)
                      
-                     242         100 LOAD_FAST                3 (name)
+                     248         100 LOAD_FAST                3 (name)
                                  102 LOAD_FAST                1 (kwargs)
                                  104 CONTAINS_OP              1
                                  106 POP_JUMP_FORWARD_IF_FALSE   124 (to 356)
                                  108 LOAD_FAST                3 (name)
                                  110 LOAD_FAST                2 (supplied_args)
                                  112 CONTAINS_OP              1
                                  114 POP_JUMP_FORWARD_IF_FALSE   120 (to 356)
                      
-                     243         116 LOAD_FAST                4 (ip)
+                     249         116 LOAD_FAST                4 (ip)
                                  118 LOAD_METHOD              2 (get_value)
                                  140 LOAD_FAST                0 (args)
                                  142 LOAD_FAST                1 (kwargs)
                                  144 PRECALL                  2
                                  148 CALL                     2
                                  158 LOAD_FAST                1 (kwargs)
                                  160 LOAD_FAST                3 (name)
                                  162 STORE_SUBSCR
                      
-                     244         166 LOAD_FAST                4 (ip)
+                     250         166 LOAD_FAST                4 (ip)
                                  168 LOAD_METHOD              3 (replace_response)
                      
-                     245         190 LOAD_GLOBAL              9 (NULL + _get_request_from_args)
+                     251         190 LOAD_GLOBAL              9 (NULL + _get_request_from_args)
                                  202 LOAD_GLOBAL             11 (NULL + typing)
                                  214 LOAD_ATTR                6 (cast)
                                  224 LOAD_GLOBAL             14 (Any)
                                  236 LOAD_FAST                0 (args)
                                  238 PRECALL                  2
                                  242 CALL                     2
                                  252 PRECALL                  1
                                  256 CALL                     1
                                  266 LOAD_FAST                1 (kwargs)
                                  268 LOAD_FAST                3 (name)
                                  270 BINARY_SUBSCR
                      
-                     244         280 PRECALL                  2
+                     250         280 PRECALL                  2
                                  284 CALL                     2
                                  294 STORE_FAST               5 (replace_response)
                      
-                     247         296 LOAD_FAST                5 (replace_response)
+                     253         296 LOAD_FAST                5 (replace_response)
                                  298 POP_JUMP_FORWARD_IF_NONE    28 (to 356)
                      
-                     248         300 LOAD_GLOBAL             11 (NULL + typing)
+                     254         300 LOAD_GLOBAL             11 (NULL + typing)
                                  312 LOAD_ATTR                6 (cast)
                                  322 LOAD_GLOBAL             16 (R)
                                  334 LOAD_FAST                5 (replace_response)
                                  336 PRECALL                  2
                                  340 CALL                     2
                                  350 SWAP                     2
                                  352 POP_TOP
                                  354 RETURN_VALUE
                              >>  356 JUMP_BACKWARD          134 (to 90)
                      
-                     250     >>  358 PUSH_NULL
+                     256     >>  358 PUSH_NULL
                                  360 LOAD_DEREF               7 (fn)
                                  362 LOAD_FAST                0 (args)
                                  364 BUILD_MAP                0
                                  366 LOAD_FAST                1 (kwargs)
                                  368 DICT_MERGE               1
                                  370 CALL_FUNCTION_EX         1
                                  372 RETURN_VALUE
@@ -2246,31 +2281,31 @@
                         None
                      names      ('len', 'items', 'get_value', 'replace_response', '_get_request_from_args', 'typing', 'cast', 'Any', 'R')
                      varnames   ('args', 'kwargs', 'supplied_args', 'name', 'ip', 'replace_response')
                      freevars   ('arg_names', 'fn', 'injected_params')
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       'inner'
-                     firstlineno 238
+                     firstlineno 244
                      lnotab 0x04022e0132011001320118015aff100304013a02
                names      ('list', 'inspect', 'signature', 'parameters', 'values', '_extract_injected_params', 'functools', 'wraps', 'P', 'args', 'kwargs', 'R')
                varnames   ('fn', 'parameters', 'inner')
                freevars   ('auto_form', 'auto_param')
                cellvars   ('fn', 'arg_names', 'injected_params')
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'decorator'
-               firstlineno 229
+               firstlineno 235
                lnotab 0x0a010c0154ff10030c0108ff1003180226014cff0e01020d
          names      ('Callable', 'P', 'R')
          varnames   ('auto_param', 'auto_form', 'decorator')
          freevars   ()
          cellvars   ('auto_param', 'auto_form')
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'inject_args'
-         firstlineno 224
+         firstlineno 230
          lnotab 0x06057219
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
@@ -2279,48 +2314,48 @@
             036a0400000000000000006401ac02a6010000ab0100000000000000005a
             086509650764043c000000020065036a0400000000000000006401ac02a6
             010000ab0100000000000000005a0a650b650c6701650c66021900000000
             0000000000650764053c000000640684005a0d6407650c6408650e650665
             0c6602190000000000000000006409650c6606640a84045a0f640b651064
             0c650c640965116512190000000000000000006606640d84045a13640e53
             00
-         261           0 RESUME                   0
+         267           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParam')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         263          12 PUSH_NULL
+         269          12 PUSH_NULL
                       14 LOAD_NAME                3 (dataclasses)
                       16 LOAD_ATTR                4 (field)
                       26 LOAD_CONST               1 (False)
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_NAME               5 (name)
                       46 LOAD_NAME                6 (str)
                       48 LOAD_NAME                7 (__annotations__)
                       50 LOAD_CONST               3 ('name')
                       52 STORE_SUBSCR
          
-         264          56 PUSH_NULL
+         270          56 PUSH_NULL
                       58 LOAD_NAME                3 (dataclasses)
                       60 LOAD_ATTR                4 (field)
                       70 LOAD_CONST               1 (False)
                       72 KW_NAMES                 2
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_NAME               8 (target_type)
                       90 LOAD_NAME                9 (type)
                       92 LOAD_NAME                7 (__annotations__)
                       94 LOAD_CONST               4 ('target_type')
                       96 STORE_SUBSCR
          
-         265         100 PUSH_NULL
+         271         100 PUSH_NULL
                      102 LOAD_NAME                3 (dataclasses)
                      104 LOAD_ATTR                4 (field)
                      114 LOAD_CONST               1 (False)
                      116 KW_NAMES                 2
                      118 PRECALL                  1
                      122 CALL                     1
                      132 STORE_NAME              10 (view_fn)
@@ -2330,49 +2365,49 @@
                      140 LOAD_NAME               12 (Any)
                      142 BUILD_TUPLE              2
                      144 BINARY_SUBSCR
                      154 LOAD_NAME                7 (__annotations__)
                      156 LOAD_CONST               5 ('view_fn')
                      158 STORE_SUBSCR
          
-         267         162 LOAD_CONST               6 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 267>)
+         273         162 LOAD_CONST               6 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 273>)
                      164 MAKE_FUNCTION            0
                      166 STORE_NAME              13 (check)
          
-         270         168 LOAD_CONST               7 ('args')
+         276         168 LOAD_CONST               7 ('args')
                      170 LOAD_NAME               12 (Any)
                      172 LOAD_CONST               8 ('kwargs')
                      174 LOAD_NAME               14 (dict)
                      176 LOAD_NAME                6 (str)
                      178 LOAD_NAME               12 (Any)
                      180 BUILD_TUPLE              2
                      182 BINARY_SUBSCR
                      192 LOAD_CONST               9 ('return')
                      194 LOAD_NAME               12 (Any)
                      196 BUILD_TUPLE              6
-                     198 LOAD_CONST              10 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 270>)
+                     198 LOAD_CONST              10 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 276>)
                      200 MAKE_FUNCTION            4 (annotations)
                      202 STORE_NAME              15 (get_value)
          
-         273         204 LOAD_CONST              11 ('request')
+         279         204 LOAD_CONST              11 ('request')
          
-         274         206 LOAD_NAME               16 (HttpRequest)
+         280         206 LOAD_NAME               16 (HttpRequest)
          
-         273         208 LOAD_CONST              12 ('value')
+         279         208 LOAD_CONST              12 ('value')
          
-         274         210 LOAD_NAME               12 (Any)
+         280         210 LOAD_NAME               12 (Any)
          
-         273         212 LOAD_CONST               9 ('return')
+         279         212 LOAD_CONST               9 ('return')
          
-         275         214 LOAD_NAME               17 (Optional)
+         281         214 LOAD_NAME               17 (Optional)
                      216 LOAD_NAME               18 (HttpResponse)
                      218 BINARY_SUBSCR
          
-         273         228 BUILD_TUPLE              6
-                     230 LOAD_CONST              13 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 273>)
+         279         228 BUILD_TUPLE              6
+                     230 LOAD_CONST              13 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 279>)
                      232 MAKE_FUNCTION            4 (annotations)
                      234 STORE_NAME              19 (replace_response)
                      236 LOAD_CONST              14 (None)
                      238 RETURN_VALUE
          consts
             'InjectedParam'
             False
@@ -2382,81 +2417,81 @@
             'view_fn'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               267           0 RESUME                   0
+               273           0 RESUME                   0
                
-               268           2 LOAD_CONST               0 (None)
+               274           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'check'
-               firstlineno 267
+               firstlineno 273
                lnotab 0x0201
             'args'
             'kwargs'
             'return'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               270           0 RESUME                   0
+               276           0 RESUME                   0
                
-               271           2 LOAD_CONST               0 (None)
+               277           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'get_value'
-               firstlineno 270
+               firstlineno 276
                lnotab 0x0201
             'request'
             'value'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               273           0 RESUME                   0
+               279           0 RESUME                   0
                
-               276           2 LOAD_CONST               0 (None)
+               282           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'request', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'replace_response'
-               firstlineno 273
+               firstlineno 279
                lnotab 0x0203
             None
          names      ('__name__', '__module__', '__qualname__', 'dataclasses', 'field', 'name', 'str', '__annotations__', 'target_type', 'type', 'view_fn', 'Callable', 'Any', 'check', 'dict', 'get_value', 'HttpRequest', 'Optional', 'HttpResponse', 'replace_response')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParam'
-         firstlineno 261
+         firstlineno 267
          lnotab 0x0c022c012c013e0206032403020102ff020102ff02020efe
       'InjectedParam'
       'view_fn'
       'ip'
       'name'
       'parameter'
       code
@@ -2476,104 +2511,104 @@
             000000741400000000000000000000a6020000ab02000000000000000072
             257c036a0500000000000000006a05000000000000000081197413000000
             000000000000007c036a0500000000000000006a050000000000000000a6
             010000ab0100000000000000006e067416000000000000000000007c015f
             0c00000000000000007c007c015f0d00000000000000007c01a00e000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             0001007c015300
-         279           0 RESUME                   0
+         285           0 RESUME                   0
          
-         285           2 LOAD_FAST                2 (name)
+         291           2 LOAD_FAST                2 (name)
                        4 LOAD_FAST                1 (ip)
                        6 STORE_ATTR               0 (name)
          
-         288          16 LOAD_FAST                3 (parameter)
+         294          16 LOAD_FAST                3 (parameter)
                       18 LOAD_ATTR                1 (annotation)
                       28 LOAD_GLOBAL              4 (inspect)
                       40 LOAD_ATTR                3 (Signature)
                       50 LOAD_ATTR                4 (empty)
                       60 IS_OP                    1
                       62 POP_JUMP_FORWARD_IF_FALSE     7 (to 78)
          
-         287          64 LOAD_FAST                3 (parameter)
+         293          64 LOAD_FAST                3 (parameter)
                       66 LOAD_ATTR                1 (annotation)
                       76 JUMP_FORWARD           139 (to 356)
          
-         290     >>   78 LOAD_FAST                3 (parameter)
+         296     >>   78 LOAD_FAST                3 (parameter)
                       80 LOAD_ATTR                5 (default)
                       90 LOAD_GLOBAL              4 (inspect)
                      102 LOAD_ATTR                6 (Parameter)
                      112 LOAD_ATTR                4 (empty)
                      122 IS_OP                    1
                      124 POP_JUMP_FORWARD_IF_FALSE    46 (to 218)
          
-         291         126 LOAD_GLOBAL             15 (NULL + isinstance)
+         297         126 LOAD_GLOBAL             15 (NULL + isinstance)
                      138 LOAD_FAST                3 (parameter)
                      140 LOAD_ATTR                5 (default)
                      150 LOAD_GLOBAL             16 (InjectedParam)
                      162 PRECALL                  2
                      166 CALL                     2
          
-         290         176 POP_JUMP_FORWARD_IF_TRUE    20 (to 218)
+         296         176 POP_JUMP_FORWARD_IF_TRUE    20 (to 218)
          
-         289         178 LOAD_GLOBAL             19 (NULL + type)
+         295         178 LOAD_GLOBAL             19 (NULL + type)
                      190 LOAD_FAST                3 (parameter)
                      192 LOAD_ATTR                5 (default)
                      202 PRECALL                  1
                      206 CALL                     1
                      216 JUMP_FORWARD            69 (to 356)
          
-         293     >>  218 LOAD_GLOBAL             15 (NULL + isinstance)
+         299     >>  218 LOAD_GLOBAL             15 (NULL + isinstance)
                      230 LOAD_FAST                3 (parameter)
                      232 LOAD_ATTR                5 (default)
                      242 LOAD_GLOBAL             20 (InjectedParamQuery)
                      254 PRECALL                  2
                      258 CALL                     2
          
-         292         268 POP_JUMP_FORWARD_IF_FALSE    37 (to 344)
+         298         268 POP_JUMP_FORWARD_IF_FALSE    37 (to 344)
          
-         294         270 LOAD_FAST                3 (parameter)
+         300         270 LOAD_FAST                3 (parameter)
                      272 LOAD_ATTR                5 (default)
                      282 LOAD_ATTR                5 (default)
                      292 POP_JUMP_FORWARD_IF_NONE    25 (to 344)
          
-         292         294 LOAD_GLOBAL             19 (NULL + type)
+         298         294 LOAD_GLOBAL             19 (NULL + type)
                      306 LOAD_FAST                3 (parameter)
                      308 LOAD_ATTR                5 (default)
                      318 LOAD_ATTR                5 (default)
                      328 PRECALL                  1
                      332 CALL                     1
                      342 JUMP_FORWARD             6 (to 356)
          
-         295     >>  344 LOAD_GLOBAL             22 (str)
+         301     >>  344 LOAD_GLOBAL             22 (str)
          
-         286     >>  356 LOAD_FAST                1 (ip)
+         292     >>  356 LOAD_FAST                1 (ip)
                      358 STORE_ATTR              12 (target_type)
          
-         297         368 LOAD_FAST                0 (view_fn)
+         303         368 LOAD_FAST                0 (view_fn)
                      370 LOAD_FAST                1 (ip)
                      372 STORE_ATTR              13 (view_fn)
          
-         298         382 LOAD_FAST                1 (ip)
+         304         382 LOAD_FAST                1 (ip)
                      384 LOAD_METHOD             14 (check)
                      406 PRECALL                  0
                      410 CALL                     0
                      420 POP_TOP
          
-         299         422 LOAD_FAST                1 (ip)
+         305         422 LOAD_FAST                1 (ip)
                      424 RETURN_VALUE
          consts
             None
          names      ('name', 'annotation', 'inspect', 'Signature', 'empty', 'default', 'Parameter', 'isinstance', 'InjectedParam', 'type', 'InjectedParamQuery', 'str', 'target_type', 'view_fn', 'check')
          varnames   ('view_fn', 'ip', 'name', 'parameter')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_setup_injected_param'
-         firstlineno 279
+         firstlineno 285
          lnotab
             0x02060e0330ff0e03300132ff02ff280432ff020218fe32030cf70c0b0e
             012801
       'parameters'
       'get'
       'post'
       code
@@ -2605,212 +2640,212 @@
             07000000000000000000007c007421000000000000000000007c08ac06a6
             010000ab0100000000000000007c066a0400000000000000007c06a60400
             00ab0400000000000000007c047c066a0400000000000000003c00000090
             018c497c0264086b0200000000722d7407000000000000000000007c0074
             23000000000000000000007c08ac06a6010000ab0100000000000000007c
             066a0400000000000000007c06a6040000ab0400000000000000007c047c
             066a0400000000000000003c00000090018c7e7c045300
-         302           0 RESUME                   0
+         308           0 RESUME                   0
          
-         311           2 BUILD_MAP                0
+         317           2 BUILD_MAP                0
                        4 STORE_FAST               4 (result)
          
-         314           6 LOAD_FAST                1 (parameters)
+         320           6 LOAD_FAST                1 (parameters)
                        8 LOAD_CONST               1 (1)
                       10 LOAD_CONST               2 (None)
                       12 BUILD_SLICE              2
                       14 BINARY_SUBSCR
                       24 STORE_FAST               1 (parameters)
          
-         316          26 LOAD_CONST               3 (False)
+         322          26 LOAD_CONST               3 (False)
                       28 STORE_FAST               5 (found_form_arg)
          
-         317          30 LOAD_FAST                1 (parameters)
+         323          30 LOAD_FAST                1 (parameters)
                       32 GET_ITER
                  >>   34 EXTENDED_ARG             1
                       36 FOR_ITER               380 (to 798)
                       38 STORE_FAST               6 (arg)
          
-         318          40 LOAD_GLOBAL              1 (NULL + isinstance)
+         324          40 LOAD_GLOBAL              1 (NULL + isinstance)
                       52 LOAD_FAST                6 (arg)
                       54 LOAD_ATTR                1 (default)
                       64 LOAD_GLOBAL              4 (InjectedParam)
                       76 PRECALL                  2
                       80 CALL                     2
                       90 POP_JUMP_FORWARD_IF_FALSE    39 (to 170)
          
-         319          92 LOAD_FAST                6 (arg)
+         325          92 LOAD_FAST                6 (arg)
                       94 LOAD_ATTR                1 (default)
                      104 STORE_FAST               7 (ip)
          
-         320         106 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         326         106 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
                      118 LOAD_FAST                0 (view_fn)
                      120 LOAD_FAST                7 (ip)
                      122 LOAD_FAST                6 (arg)
                      124 LOAD_ATTR                4 (name)
                      134 LOAD_FAST                6 (arg)
                      136 PRECALL                  4
                      140 CALL                     4
                      150 LOAD_FAST                4 (result)
                      152 LOAD_FAST                7 (ip)
                      154 LOAD_ATTR                4 (name)
                      164 STORE_SUBSCR
                      168 JUMP_BACKWARD           68 (to 34)
          
-         325     >>  170 LOAD_FAST                6 (arg)
+         331     >>  170 LOAD_FAST                6 (arg)
                      172 LOAD_ATTR                1 (default)
                      182 LOAD_GLOBAL             10 (inspect)
                      194 LOAD_ATTR                6 (Parameter)
                      204 LOAD_ATTR                7 (empty)
                      214 COMPARE_OP               3 (!=)
                      220 POP_JUMP_FORWARD_IF_FALSE     7 (to 236)
                      222 LOAD_FAST                6 (arg)
                      224 LOAD_ATTR                1 (default)
                      234 JUMP_FORWARD             1 (to 238)
                  >>  236 LOAD_CONST               2 (None)
          
-         324     >>  238 STORE_FAST               8 (default_value)
+         330     >>  238 STORE_FAST               8 (default_value)
          
-         329         240 LOAD_FAST                3 (auto_form)
+         335         240 LOAD_FAST                3 (auto_form)
          
-         328         242 POP_JUMP_FORWARD_IF_FALSE   120 (to 484)
+         334         242 POP_JUMP_FORWARD_IF_FALSE   120 (to 484)
          
-         330         244 LOAD_GLOBAL              1 (NULL + isinstance)
+         336         244 LOAD_GLOBAL              1 (NULL + isinstance)
                      256 LOAD_FAST                6 (arg)
                      258 LOAD_ATTR                8 (annotation)
                      268 LOAD_GLOBAL             18 (type)
                      280 PRECALL                  2
                      284 CALL                     2
          
-         328         294 POP_JUMP_FORWARD_IF_FALSE    94 (to 484)
+         334         294 POP_JUMP_FORWARD_IF_FALSE    94 (to 484)
          
-         331         296 LOAD_GLOBAL             21 (NULL + issubclass)
+         337         296 LOAD_GLOBAL             21 (NULL + issubclass)
                      308 LOAD_FAST                6 (arg)
                      310 LOAD_ATTR                8 (annotation)
                      320 LOAD_GLOBAL             22 (forms)
                      332 LOAD_ATTR               12 (BaseForm)
                      342 PRECALL                  2
                      346 CALL                     2
          
-         328         356 POP_JUMP_FORWARD_IF_FALSE    63 (to 484)
+         334         356 POP_JUMP_FORWARD_IF_FALSE    63 (to 484)
          
-         333         358 LOAD_FAST                5 (found_form_arg)
+         339         358 LOAD_FAST                5 (found_form_arg)
                      360 POP_JUMP_FORWARD_IF_FALSE    15 (to 392)
          
-         334         362 LOAD_GLOBAL             27 (NULL + Exception)
+         340         362 LOAD_GLOBAL             27 (NULL + Exception)
          
-         335         374 LOAD_CONST               4 ('You can only have one Form argument in a view function.')
+         341         374 LOAD_CONST               4 ('You can only have one Form argument in a view function.')
          
-         334         376 PRECALL                  1
+         340         376 PRECALL                  1
                      380 CALL                     1
                      390 RAISE_VARARGS            1
          
-         337     >>  392 LOAD_CONST               5 (True)
+         343     >>  392 LOAD_CONST               5 (True)
                      394 STORE_FAST               5 (found_form_arg)
          
-         338         396 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         344         396 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
          
-         339         408 LOAD_FAST                0 (view_fn)
+         345         408 LOAD_FAST                0 (view_fn)
                      410 LOAD_GLOBAL             29 (NULL + handle_form)
                      422 PRECALL                  0
                      426 CALL                     0
                      436 LOAD_FAST                6 (arg)
                      438 LOAD_ATTR                4 (name)
                      448 LOAD_FAST                6 (arg)
          
-         338         450 PRECALL                  4
+         344         450 PRECALL                  4
                      454 CALL                     4
                      464 LOAD_FAST                4 (result)
                      466 LOAD_FAST                6 (arg)
                      468 LOAD_ATTR                4 (name)
                      478 STORE_SUBSCR
                      482 JUMP_BACKWARD          225 (to 34)
          
-         342     >>  484 LOAD_FAST                2 (auto_param)
+         348     >>  484 LOAD_FAST                2 (auto_param)
                      486 LOAD_CONST               5 (True)
                      488 IS_OP                    0
                      490 POP_JUMP_FORWARD_IF_FALSE    47 (to 586)
          
-         343         492 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         349         492 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
          
-         344         504 LOAD_FAST                0 (view_fn)
+         350         504 LOAD_FAST                0 (view_fn)
                      506 LOAD_GLOBAL             31 (NULL + InjectedParamQuery)
                      518 LOAD_FAST                8 (default_value)
                      520 KW_NAMES                 6
                      522 PRECALL                  1
                      526 CALL                     1
                      536 LOAD_FAST                6 (arg)
                      538 LOAD_ATTR                4 (name)
                      548 LOAD_FAST                6 (arg)
          
-         343         550 PRECALL                  4
+         349         550 PRECALL                  4
                      554 CALL                     4
                      564 LOAD_FAST                4 (result)
                      566 LOAD_FAST                6 (arg)
                      568 LOAD_ATTR                4 (name)
                      578 STORE_SUBSCR
                      582 EXTENDED_ARG             1
                      584 JUMP_BACKWARD          276 (to 34)
          
-         346     >>  586 LOAD_FAST                2 (auto_param)
+         352     >>  586 LOAD_FAST                2 (auto_param)
                      588 LOAD_CONST               7 ('get')
                      590 COMPARE_OP               2 (==)
                      596 POP_JUMP_FORWARD_IF_FALSE    47 (to 692)
          
-         347         598 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         353         598 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
          
-         348         610 LOAD_FAST                0 (view_fn)
+         354         610 LOAD_FAST                0 (view_fn)
                      612 LOAD_GLOBAL             33 (NULL + InjectedParamQueryGet)
                      624 LOAD_FAST                8 (default_value)
                      626 KW_NAMES                 6
                      628 PRECALL                  1
                      632 CALL                     1
                      642 LOAD_FAST                6 (arg)
                      644 LOAD_ATTR                4 (name)
                      654 LOAD_FAST                6 (arg)
          
-         347         656 PRECALL                  4
+         353         656 PRECALL                  4
                      660 CALL                     4
                      670 LOAD_FAST                4 (result)
                      672 LOAD_FAST                6 (arg)
                      674 LOAD_ATTR                4 (name)
                      684 STORE_SUBSCR
                      688 EXTENDED_ARG             1
                      690 JUMP_BACKWARD          329 (to 34)
          
-         350     >>  692 LOAD_FAST                2 (auto_param)
+         356     >>  692 LOAD_FAST                2 (auto_param)
                      694 LOAD_CONST               8 ('post')
                      696 COMPARE_OP               2 (==)
                      702 POP_JUMP_FORWARD_IF_FALSE    45 (to 794)
          
-         351         704 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
+         357         704 LOAD_GLOBAL              7 (NULL + _setup_injected_param)
          
-         352         716 LOAD_FAST                0 (view_fn)
+         358         716 LOAD_FAST                0 (view_fn)
          
-         353         718 LOAD_GLOBAL             35 (NULL + InjectedParamQueryPost)
+         359         718 LOAD_GLOBAL             35 (NULL + InjectedParamQueryPost)
                      730 LOAD_FAST                8 (default_value)
                      732 KW_NAMES                 6
                      734 PRECALL                  1
                      738 CALL                     1
          
-         354         748 LOAD_FAST                6 (arg)
+         360         748 LOAD_FAST                6 (arg)
                      750 LOAD_ATTR                4 (name)
          
-         355         760 LOAD_FAST                6 (arg)
+         361         760 LOAD_FAST                6 (arg)
          
-         351         762 PRECALL                  4
+         357         762 PRECALL                  4
                      766 CALL                     4
                      776 LOAD_FAST                4 (result)
                      778 LOAD_FAST                6 (arg)
                      780 LOAD_ATTR                4 (name)
                      790 STORE_SUBSCR
                  >>  794 EXTENDED_ARG             1
                      796 JUMP_BACKWARD          382 (to 34)
          
-         358     >>  798 LOAD_FAST                4 (result)
+         364     >>  798 LOAD_FAST                4 (result)
                      800 RETURN_VALUE
          consts
             '\n    Extracts all injected parameters from the given list of function arguments.\n    '
             1
             None
             False
             'You can only have one Form argument in a view function.'
@@ -2820,15 +2855,15 @@
             'post'
          names      ('isinstance', 'default', 'InjectedParam', '_setup_injected_param', 'name', 'inspect', 'Parameter', 'empty', 'annotation', 'type', 'issubclass', 'forms', 'BaseForm', 'Exception', 'handle_form', 'InjectedParamQuery', 'InjectedParamQueryGet', 'InjectedParamQueryPost')
          varnames   ('view_fn', 'parameters', 'auto_param', 'auto_form', 'result', 'found_form_arg', 'arg', 'ip', 'default_value')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_extract_injected_params'
-         firstlineno 302
+         firstlineno 308
          lnotab
             0x02090403140204010a0134010e01400544ff020502ff020232fe02033c
             fd020504010c0102ff100304010c012aff220408010c012eff24030c010c
             012eff24030c010c0102011e010c0102fc2407
       code
          argcount  : 0
          nlocals   : 0
@@ -2839,90 +2874,90 @@
             02a6010000ab0100000000000000005a0565066507190000000000000000
             00650864033c000000020065036a0400000000000000006401ac02a60100
             00ab0100000000000000005a09650a650864043c000000020065036a0400
             000000000000006405ac02a6010000ab0100000000000000005a0b650c65
             0864063c000000640784005a0d6408650e6602640984045a0f6408650e66
             02640a84045a10640b650a640c65116507650a6602190000000000000000
             006604640d84045a1264015300
-         366           0 RESUME                   0
+         372           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQuery')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         368          12 PUSH_NULL
+         374          12 PUSH_NULL
                       14 LOAD_NAME                3 (dataclasses)
                       16 LOAD_ATTR                4 (field)
                       26 LOAD_CONST               1 (None)
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_NAME               5 (query_param_name)
                       46 LOAD_NAME                6 (Optional)
                       48 LOAD_NAME                7 (str)
                       50 BINARY_SUBSCR
                       60 LOAD_NAME                8 (__annotations__)
                       62 LOAD_CONST               3 ('query_param_name')
                       64 STORE_SUBSCR
          
-         369          68 PUSH_NULL
+         375          68 PUSH_NULL
                       70 LOAD_NAME                3 (dataclasses)
                       72 LOAD_ATTR                4 (field)
                       82 LOAD_CONST               1 (None)
                       84 KW_NAMES                 2
                       86 PRECALL                  1
                       90 CALL                     1
                      100 STORE_NAME               9 (default)
                      102 LOAD_NAME               10 (Any)
                      104 LOAD_NAME                8 (__annotations__)
                      106 LOAD_CONST               4 ('default')
                      108 STORE_SUBSCR
          
-         370         112 PUSH_NULL
+         376         112 PUSH_NULL
                      114 LOAD_NAME                3 (dataclasses)
                      116 LOAD_ATTR                4 (field)
                      126 LOAD_CONST               5 (True)
                      128 KW_NAMES                 2
                      130 PRECALL                  1
                      134 CALL                     1
                      144 STORE_NAME              11 (consume)
                      146 LOAD_NAME               12 (bool)
                      148 LOAD_NAME                8 (__annotations__)
                      150 LOAD_CONST               6 ('consume')
                      152 STORE_SUBSCR
          
-         372         156 LOAD_CONST               7 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 372>)
+         378         156 LOAD_CONST               7 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 378>)
                      158 MAKE_FUNCTION            0
                      160 STORE_NAME              13 (check)
          
-         376         162 LOAD_CONST               8 ('request')
+         382         162 LOAD_CONST               8 ('request')
                      164 LOAD_NAME               14 (HttpRequest)
                      166 BUILD_TUPLE              2
-                     168 LOAD_CONST               9 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 376>)
+                     168 LOAD_CONST               9 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 382>)
                      170 MAKE_FUNCTION            4 (annotations)
                      172 STORE_NAME              15 (_create_lookup_dict)
          
-         383         174 LOAD_CONST               8 ('request')
+         389         174 LOAD_CONST               8 ('request')
                      176 LOAD_NAME               14 (HttpRequest)
                      178 BUILD_TUPLE              2
-                     180 LOAD_CONST              10 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 383>)
+                     180 LOAD_CONST              10 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 389>)
                      182 MAKE_FUNCTION            4 (annotations)
                      184 STORE_NAME              16 (_consume_param)
          
-         393         186 LOAD_CONST              11 ('args')
+         399         186 LOAD_CONST              11 ('args')
                      188 LOAD_NAME               10 (Any)
                      190 LOAD_CONST              12 ('kwargs')
                      192 LOAD_NAME               17 (dict)
                      194 LOAD_NAME                7 (str)
                      196 LOAD_NAME               10 (Any)
                      198 BUILD_TUPLE              2
                      200 BINARY_SUBSCR
                      210 BUILD_TUPLE              4
-                     212 LOAD_CONST              13 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 393>)
+                     212 LOAD_CONST              13 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 399>)
                      214 MAKE_FUNCTION            4 (annotations)
                      216 STORE_NAME              18 (get_value)
                      218 LOAD_CONST               1 (None)
                      220 RETURN_VALUE
          consts
             'InjectedParamQuery'
             None
@@ -2935,38 +2970,38 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000800e7c006a0100000000000000007c
                   005f0000000000000000006400530064005300
-               372           0 RESUME                   0
+               378           0 RESUME                   0
                
-               373           2 LOAD_FAST                0 (self)
+               379           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 44)
                
-               374          16 LOAD_FAST                0 (self)
+               380          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (name)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               0 (query_param_name)
                             40 LOAD_CONST               0 (None)
                             42 RETURN_VALUE
                
-               373     >>   44 LOAD_CONST               0 (None)
+               379     >>   44 LOAD_CONST               0 (None)
                             46 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'check'
-               firstlineno 372
+               firstlineno 378
                lnotab 0x02010e011cff
             'request'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
@@ -2977,55 +3012,55 @@
                   00000000007d027401000000000000000000006a01000000000000000074
                   04000000000000000000007c016a040000000000000000a6020000ab0200
                   000000000000008a05880566016402840889054400a6000000ab00000000
                   00000000007d037c037c027a0700005300
                              0 MAKE_CELL                4 (getqd)
                              2 MAKE_CELL                5 (postqd)
                
-               376           4 RESUME                   0
+               382           4 RESUME                   0
                
-               377           6 LOAD_GLOBAL              1 (NULL + typing)
+               383           6 LOAD_GLOBAL              1 (NULL + typing)
                             18 LOAD_ATTR                1 (cast)
                             28 LOAD_GLOBAL              4 (QueryDict)
                             40 LOAD_FAST                1 (request)
                             42 LOAD_ATTR                3 (GET)
                             52 PRECALL                  2
                             56 CALL                     2
                             66 STORE_DEREF              4 (getqd)
                
-               378          68 LOAD_CLOSURE             4 (getqd)
+               384          68 LOAD_CLOSURE             4 (getqd)
                             70 BUILD_TUPLE              1
-                            72 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 378>)
+                            72 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 384>)
                             74 MAKE_FUNCTION            8 (closure)
                             76 LOAD_DEREF               4 (getqd)
                             78 GET_ITER
                             80 PRECALL                  0
                             84 CALL                     0
                             94 STORE_FAST               2 (getd)
                
-               379          96 LOAD_GLOBAL              1 (NULL + typing)
+               385          96 LOAD_GLOBAL              1 (NULL + typing)
                            108 LOAD_ATTR                1 (cast)
                            118 LOAD_GLOBAL              4 (QueryDict)
                            130 LOAD_FAST                1 (request)
                            132 LOAD_ATTR                4 (POST)
                            142 PRECALL                  2
                            146 CALL                     2
                            156 STORE_DEREF              5 (postqd)
                
-               380         158 LOAD_CLOSURE             5 (postqd)
+               386         158 LOAD_CLOSURE             5 (postqd)
                            160 BUILD_TUPLE              1
-                           162 LOAD_CONST               2 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 380>)
+                           162 LOAD_CONST               2 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 386>)
                            164 MAKE_FUNCTION            8 (closure)
                            166 LOAD_DEREF               5 (postqd)
                            168 GET_ITER
                            170 PRECALL                  0
                            174 CALL                     0
                            184 STORE_FAST               3 (postd)
                
-               381         186 LOAD_FAST                3 (postd)
+               387         186 LOAD_FAST                3 (postd)
                            188 LOAD_FAST                2 (getd)
                            190 BINARY_OP                7 (|)
                            194 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
@@ -3034,15 +3069,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     378           2 RESUME                   0
+                     384           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (getqd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -3055,28 +3090,28 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('getqd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 378
+                     firstlineno 384
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 6
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     380           2 RESUME                   0
+                     386           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (postqd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -3089,23 +3124,23 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('postqd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 380
+                     firstlineno 386
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'GET', 'POST')
                varnames   ('self', 'request', 'getd', 'postd')
                freevars   ()
                cellvars   ('getqd', 'postqd')
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 376
+               firstlineno 382
                lnotab 0x06013e011c013e011c01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
@@ -3115,79 +3150,79 @@
                   020000ab0200000000000000007c006a000000000000000000a6020000ab
                   0200000000000000007c015f010000000000000000640053007c006a0000
                   000000000000007c016a0600000000000000007600723974050000000000
                   00000000007407000000000000000000006a040000000000000000740a00
                   0000000000000000007c016a060000000000000000a6020000ab02000000
                   00000000007c006a000000000000000000a6020000ab0200000000000000
                   007c015f0600000000000000006400530064005300
-               383           0 RESUME                   0
+               389           0 RESUME                   0
                
-               384           2 LOAD_FAST                0 (self)
+               390           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (GET)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               385          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               391          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               386          42 LOAD_GLOBAL              7 (NULL + typing)
+               392          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (GET)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               385         114 PRECALL                  2
+               391         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (GET)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               388     >>  144 LOAD_FAST                0 (self)
+               394     >>  144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                0 (query_param_name)
                            156 LOAD_FAST                1 (request)
                            158 LOAD_ATTR                6 (POST)
                            168 CONTAINS_OP              0
                            170 POP_JUMP_FORWARD_IF_FALSE    57 (to 286)
                
-               389         172 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               395         172 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               390         184 LOAD_GLOBAL              7 (NULL + typing)
+               396         184 LOAD_GLOBAL              7 (NULL + typing)
                            196 LOAD_ATTR                4 (cast)
                            206 LOAD_GLOBAL             10 (Any)
                            218 LOAD_FAST                1 (request)
                            220 LOAD_ATTR                6 (POST)
                            230 PRECALL                  2
                            234 CALL                     2
                            244 LOAD_FAST                0 (self)
                            246 LOAD_ATTR                0 (query_param_name)
                
-               389         256 PRECALL                  2
+               395         256 PRECALL                  2
                            260 CALL                     2
                            270 LOAD_FAST                1 (request)
                            272 STORE_ATTR               6 (POST)
                            282 LOAD_CONST               0 (None)
                            284 RETURN_VALUE
                
-               388     >>  286 LOAD_CONST               0 (None)
+               394     >>  286 LOAD_CONST               0 (None)
                            288 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'GET', 'querydict_key_removed', 'typing', 'cast', 'Any', 'POST')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 383
+               firstlineno 389
                lnotab 0x02011c010c0148ff1e031c010c0148ff1eff
             'args'
             'kwargs'
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
@@ -3202,87 +3237,87 @@
                   0000000000000000007c006a070000000000000000a6020000ab02000000
                   000000000072026400530074110000000000000000000064017c006a0300
                   000000000000009b0064029d03a6010000ab01000000000000000082017c
                   006a09000000000000000072157c00a00a00000000000000000000000000
                   000000000000007c03a6010000ab01000000000000000001007417000000
                   000000000000007c057c006a070000000000000000a6020000ab02000000
                   00000000005300
-               393           0 RESUME                   0
+               399           0 RESUME                   0
                
-               394           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
+               400           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
                             14 LOAD_FAST                1 (args)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               3 (request)
                
-               395          32 LOAD_FAST                0 (self)
+               401          32 LOAD_FAST                0 (self)
                             34 LOAD_METHOD              1 (_create_lookup_dict)
                             56 LOAD_FAST                3 (request)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 STORE_FAST               4 (lookup_dict)
                
-               396          74 LOAD_FAST                4 (lookup_dict)
+               402          74 LOAD_FAST                4 (lookup_dict)
                             76 LOAD_METHOD              2 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (query_param_name)
                            110 LOAD_CONST               0 (None)
                            112 PRECALL                  2
                            116 CALL                     2
                            126 STORE_FAST               5 (values)
                
-               398         128 LOAD_FAST                5 (values)
+               404         128 LOAD_FAST                5 (values)
                            130 POP_JUMP_FORWARD_IF_NOT_NONE    68 (to 268)
                
-               399         132 LOAD_FAST                0 (self)
+               405         132 LOAD_FAST                0 (self)
                            134 LOAD_ATTR                4 (default)
                            144 POP_JUMP_FORWARD_IF_NONE     9 (to 164)
                
-               400         146 LOAD_FAST                0 (self)
+               406         146 LOAD_FAST                0 (self)
                            148 LOAD_ATTR                4 (default)
                            158 BUILD_LIST               1
                            160 STORE_FAST               5 (values)
                            162 JUMP_FORWARD            52 (to 268)
                
-               401     >>  164 LOAD_GLOBAL             11 (NULL + issubclass)
+               407     >>  164 LOAD_GLOBAL             11 (NULL + issubclass)
                            176 LOAD_GLOBAL             12 (NoneType)
                            188 LOAD_FAST                0 (self)
                            190 LOAD_ATTR                7 (target_type)
                            200 PRECALL                  2
                            204 CALL                     2
                            214 POP_JUMP_FORWARD_IF_FALSE     2 (to 220)
                
-               402         216 LOAD_CONST               0 (None)
+               408         216 LOAD_CONST               0 (None)
                            218 RETURN_VALUE
                
-               404     >>  220 LOAD_GLOBAL             17 (NULL + Exception)
+               410     >>  220 LOAD_GLOBAL             17 (NULL + Exception)
                
-               405         232 LOAD_CONST               1 ("No value found for request parameter '")
+               411         232 LOAD_CONST               1 ("No value found for request parameter '")
                            234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                3 (query_param_name)
                            246 FORMAT_VALUE             0
                            248 LOAD_CONST               2 ("'")
                            250 BUILD_STRING             3
                
-               404         252 PRECALL                  1
+               410         252 PRECALL                  1
                            256 CALL                     1
                            266 RAISE_VARARGS            1
                
-               408     >>  268 LOAD_FAST                0 (self)
+               414     >>  268 LOAD_FAST                0 (self)
                            270 LOAD_ATTR                9 (consume)
                            280 POP_JUMP_FORWARD_IF_FALSE    21 (to 324)
                
-               409         282 LOAD_FAST                0 (self)
+               415         282 LOAD_FAST                0 (self)
                            284 LOAD_METHOD             10 (_consume_param)
                            306 LOAD_FAST                3 (request)
                            308 PRECALL                  1
                            312 CALL                     1
                            322 POP_TOP
                
-               411     >>  324 LOAD_GLOBAL             23 (NULL + _convert_value_to_type)
+               417     >>  324 LOAD_GLOBAL             23 (NULL + _convert_value_to_type)
                            336 LOAD_FAST                5 (values)
                            338 LOAD_FAST                0 (self)
                            340 LOAD_ATTR                7 (target_type)
                            350 PRECALL                  2
                            354 CALL                     2
                            364 RETURN_VALUE
                consts
@@ -3291,50 +3326,50 @@
                   "'"
                names      ('_get_request_from_args', '_create_lookup_dict', 'get', 'query_param_name', 'default', 'issubclass', 'NoneType', 'target_type', 'Exception', 'consume', '_consume_param', '_convert_value_to_type')
                varnames   ('self', 'args', 'kwargs', 'request', 'lookup_dict', 'values')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'get_value'
-               firstlineno 393
+               firstlineno 399
                lnotab 0x02011e012a01360204010e011201340104020c0114ff10040e012a02
          names      ('__name__', '__module__', '__qualname__', 'dataclasses', 'field', 'query_param_name', 'Optional', 'str', '__annotations__', 'default', 'Any', 'consume', 'bool', 'check', 'HttpRequest', '_create_lookup_dict', '_consume_param', 'dict', 'get_value')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQuery'
-         firstlineno 366
+         firstlineno 372
          lnotab 0x0c0238012c012c0206040c070c0a
       'InjectedParamQuery'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640165036602640284045a0464016503660264
             0384045a0564045300
-         414           0 RESUME                   0
+         420           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQueryGet')
                        8 STORE_NAME               2 (__qualname__)
          
-         416          10 LOAD_CONST               1 ('request')
+         422          10 LOAD_CONST               1 ('request')
                       12 LOAD_NAME                3 (HttpRequest)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 416>)
+                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 422>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (_create_lookup_dict)
          
-         420          22 LOAD_CONST               1 ('request')
+         426          22 LOAD_CONST               1 ('request')
                       24 LOAD_NAME                3 (HttpRequest)
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 420>)
+                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 426>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               5 (_consume_param)
                       34 LOAD_CONST               4 (None)
                       36 RETURN_VALUE
          consts
             'InjectedParamQueryGet'
             'request'
@@ -3346,28 +3381,28 @@
                code
                   0x870297007401000000000000000000006a010000000000000000740400
                   0000000000000000007c016a030000000000000000a6020000ab02000000
                   00000000008a02880266016401840889024400a6000000ab000000000000
                   0000005300
                              0 MAKE_CELL                2 (qd)
                
-               416           2 RESUME                   0
+               422           2 RESUME                   0
                
-               417           4 LOAD_GLOBAL              1 (NULL + typing)
+               423           4 LOAD_GLOBAL              1 (NULL + typing)
                             16 LOAD_ATTR                1 (cast)
                             26 LOAD_GLOBAL              4 (QueryDict)
                             38 LOAD_FAST                1 (request)
                             40 LOAD_ATTR                3 (GET)
                             50 PRECALL                  2
                             54 CALL                     2
                             64 STORE_DEREF              2 (qd)
                
-               418          66 LOAD_CLOSURE             2 (qd)
+               424          66 LOAD_CLOSURE             2 (qd)
                             68 BUILD_TUPLE              1
-                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 418>)
+                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 424>)
                             72 MAKE_FUNCTION            8 (closure)
                             74 LOAD_DEREF               2 (qd)
                             76 GET_ITER
                             78 PRECALL                  0
                             82 CALL                     0
                             92 RETURN_VALUE
                consts
@@ -3379,15 +3414,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     418           2 RESUME                   0
+                     424           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (qd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -3400,110 +3435,110 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('qd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 418
+                     firstlineno 424
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'GET')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ('qd',)
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 416
+               firstlineno 422
                lnotab 0x04013e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000007c016a010000000000000000760072
                   397405000000000000000000007407000000000000000000006a04000000
                   0000000000740a000000000000000000007c016a010000000000000000a6
                   020000ab0200000000000000007c006a000000000000000000a6020000ab
                   0200000000000000007c015f0100000000000000006400530064005300
-               420           0 RESUME                   0
+               426           0 RESUME                   0
                
-               421           2 LOAD_FAST                0 (self)
+               427           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (GET)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               422          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               428          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               423          42 LOAD_GLOBAL              7 (NULL + typing)
+               429          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (GET)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               422         114 PRECALL                  2
+               428         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (GET)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               421     >>  144 LOAD_CONST               0 (None)
+               427     >>  144 LOAD_CONST               0 (None)
                            146 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'GET', 'querydict_key_removed', 'typing', 'cast', 'Any')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 420
+               firstlineno 426
                lnotab 0x02011c010c0148ff1eff
             None
          names      ('__name__', '__module__', '__qualname__', 'HttpRequest', '_create_lookup_dict', '_consume_param')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQueryGet'
-         firstlineno 414
+         firstlineno 420
          lnotab 0x0a020c04
       'InjectedParamQueryGet'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640165036602640284045a0464016503660264
             0384045a0564045300
-         427           0 RESUME                   0
+         433           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamQueryPost')
                        8 STORE_NAME               2 (__qualname__)
          
-         429          10 LOAD_CONST               1 ('request')
+         435          10 LOAD_CONST               1 ('request')
                       12 LOAD_NAME                3 (HttpRequest)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 429>)
+                      16 LOAD_CONST               2 (<code object _create_lookup_dict, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 435>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (_create_lookup_dict)
          
-         433          22 LOAD_CONST               1 ('request')
+         439          22 LOAD_CONST               1 ('request')
                       24 LOAD_NAME                3 (HttpRequest)
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 433>)
+                      28 LOAD_CONST               3 (<code object _consume_param, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 439>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               5 (_consume_param)
                       34 LOAD_CONST               4 (None)
                       36 RETURN_VALUE
          consts
             'InjectedParamQueryPost'
             'request'
@@ -3515,28 +3550,28 @@
                code
                   0x870297007401000000000000000000006a010000000000000000740400
                   0000000000000000007c016a030000000000000000a6020000ab02000000
                   00000000008a02880266016401840889024400a6000000ab000000000000
                   0000005300
                              0 MAKE_CELL                2 (qd)
                
-               429           2 RESUME                   0
+               435           2 RESUME                   0
                
-               430           4 LOAD_GLOBAL              1 (NULL + typing)
+               436           4 LOAD_GLOBAL              1 (NULL + typing)
                             16 LOAD_ATTR                1 (cast)
                             26 LOAD_GLOBAL              4 (QueryDict)
                             38 LOAD_FAST                1 (request)
                             40 LOAD_ATTR                3 (POST)
                             50 PRECALL                  2
                             54 CALL                     2
                             64 STORE_DEREF              2 (qd)
                
-               431          66 LOAD_CLOSURE             2 (qd)
+               437          66 LOAD_CLOSURE             2 (qd)
                             68 BUILD_TUPLE              1
-                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 431>)
+                            70 LOAD_CONST               1 (<code object <dictcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 437>)
                             72 MAKE_FUNCTION            8 (closure)
                             74 LOAD_DEREF               2 (qd)
                             76 GET_ITER
                             78 PRECALL                  0
                             82 CALL                     0
                             92 RETURN_VALUE
                consts
@@ -3548,15 +3583,15 @@
                      flags     : 19
                      code
                         0x9501970069007c005d187d017c018902a0000000000000000000000000
                         0000000000000000007c01a6010000ab01000000000000000093028c1953
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     431           2 RESUME                   0
+                     437           2 RESUME                   0
                                    4 BUILD_MAP                0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                24 (to 58)
                                   10 STORE_FAST               1 (name)
                                   12 LOAD_FAST                1 (name)
                                   14 LOAD_DEREF               2 (qd)
                                   16 LOAD_METHOD              0 (getlist)
@@ -3569,96 +3604,96 @@
                      consts
                      names      ('getlist',)
                      varnames   ('.0', 'name')
                      freevars   ('qd',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                      name       '<dictcomp>'
-                     firstlineno 431
+                     firstlineno 437
                      lnotab 0x
                names      ('typing', 'cast', 'QueryDict', 'POST')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ('qd',)
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_create_lookup_dict'
-               firstlineno 429
+               firstlineno 435
                lnotab 0x04013e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000007c016a010000000000000000760072
                   397405000000000000000000007407000000000000000000006a04000000
                   0000000000740a000000000000000000007c016a010000000000000000a6
                   020000ab0200000000000000007c006a000000000000000000a6020000ab
                   0200000000000000007c015f0100000000000000006400530064005300
-               433           0 RESUME                   0
+               439           0 RESUME                   0
                
-               434           2 LOAD_FAST                0 (self)
+               440           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query_param_name)
                             14 LOAD_FAST                1 (request)
                             16 LOAD_ATTR                1 (POST)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    57 (to 144)
                
-               435          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
+               441          30 LOAD_GLOBAL              5 (NULL + querydict_key_removed)
                
-               436          42 LOAD_GLOBAL              7 (NULL + typing)
+               442          42 LOAD_GLOBAL              7 (NULL + typing)
                             54 LOAD_ATTR                4 (cast)
                             64 LOAD_GLOBAL             10 (Any)
                             76 LOAD_FAST                1 (request)
                             78 LOAD_ATTR                1 (POST)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (query_param_name)
                
-               435         114 PRECALL                  2
+               441         114 PRECALL                  2
                            118 CALL                     2
                            128 LOAD_FAST                1 (request)
                            130 STORE_ATTR               1 (POST)
                            140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                
-               434     >>  144 LOAD_CONST               0 (None)
+               440     >>  144 LOAD_CONST               0 (None)
                            146 RETURN_VALUE
                consts
                   None
                names      ('query_param_name', 'POST', 'querydict_key_removed', 'typing', 'cast', 'Any')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '_consume_param'
-               firstlineno 433
+               firstlineno 439
                lnotab 0x02011c010c0148ff1eff
             None
          names      ('__name__', '__module__', '__qualname__', 'HttpRequest', '_create_lookup_dict', '_consume_param')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamQueryPost'
-         firstlineno 427
+         firstlineno 433
          lnotab 0x0a020c04
       'InjectedParamQueryPost'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c007c01ac01a6020000ab02000000
             00000000005300
-         440           0 RESUME                   0
+         446           0 RESUME                   0
          
-         441           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryGet)
+         447           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryGet)
                       14 LOAD_FAST                0 (default)
                       16 LOAD_FAST                1 (consume)
                       18 KW_NAMES                 1
                       20 PRECALL                  2
                       24 CALL                     2
                       34 RETURN_VALUE
          consts
@@ -3666,27 +3701,27 @@
             ('default', 'consume')
          names      ('InjectedParamQueryGet',)
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param_get'
-         firstlineno 440
+         firstlineno 446
          lnotab 0x0201
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c007c01ac01a6020000ab02000000
             00000000005300
-         444           0 RESUME                   0
+         450           0 RESUME                   0
          
-         445           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryPost)
+         451           2 LOAD_GLOBAL              1 (NULL + InjectedParamQueryPost)
                       14 LOAD_FAST                0 (default)
                       16 LOAD_FAST                1 (consume)
                       18 KW_NAMES                 1
                       20 PRECALL                  2
                       24 CALL                     2
                       34 RETURN_VALUE
          consts
@@ -3694,29 +3729,29 @@
             ('default', 'consume')
          names      ('InjectedParamQueryPost',)
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param_post'
-         firstlineno 444
+         firstlineno 450
          lnotab 0x0201
       'default'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007404000000
             000000000000007407000000000000000000007c007c01ac01a6020000ab
             020000000000000000a6020000ab0200000000000000005300
-         448           0 RESUME                   0
+         454           0 RESUME                   0
          
-         449           2 LOAD_GLOBAL              1 (NULL + typing)
+         455           2 LOAD_GLOBAL              1 (NULL + typing)
                       14 LOAD_ATTR                1 (cast)
                       24 LOAD_GLOBAL              4 (T)
                       36 LOAD_GLOBAL              7 (NULL + InjectedParamQuery)
                       48 LOAD_FAST                0 (default)
                       50 LOAD_FAST                1 (consume)
                       52 KW_NAMES                 1
                       54 PRECALL                  2
@@ -3729,15 +3764,15 @@
             ('default', 'consume')
          names      ('typing', 'cast', 'T', 'InjectedParamQuery')
          varnames   ('default', 'consume')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'param'
-         firstlineno 448
+         firstlineno 454
          lnotab 0x0201
       'values'
       'target_type'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 6
@@ -3763,148 +3798,148 @@
             00720264056e0164065300740b0000000000000000000074140000000000
             00000000006a0b00000000000000007c01a6020000ab0200000000000000
             0072147415000000000000000000006a0b00000000000000007c02a60100
             00ab010000000000000000530074190000000000000000000064077c019b
             0064087c029b009d04a6010000ab0100000000000000008201
                        0 MAKE_CELL                3 (list_type)
          
-         452           2 RESUME                   0
+         458           2 RESUME                   0
          
-         454           4 LOAD_GLOBAL              1 (NULL + typing)
+         460           4 LOAD_GLOBAL              1 (NULL + typing)
                       16 LOAD_ATTR                1 (get_origin)
                       26 LOAD_FAST                1 (target_type)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 LOAD_GLOBAL              4 (list)
                       54 COMPARE_OP               2 (==)
                       60 POP_JUMP_FORWARD_IF_FALSE    40 (to 142)
          
-         455          62 LOAD_GLOBAL              1 (NULL + typing)
+         461          62 LOAD_GLOBAL              1 (NULL + typing)
                       74 LOAD_ATTR                3 (get_args)
                       84 LOAD_FAST                1 (target_type)
                       86 PRECALL                  1
                       90 CALL                     1
                      100 LOAD_CONST               1 (0)
                      102 BINARY_SUBSCR
                      112 STORE_DEREF              3 (list_type)
          
-         456         114 LOAD_CLOSURE             3 (list_type)
+         462         114 LOAD_CLOSURE             3 (list_type)
                      116 BUILD_TUPLE              1
-                     118 LOAD_CONST               2 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 456>)
+                     118 LOAD_CONST               2 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 462>)
                      120 MAKE_FUNCTION            8 (closure)
                      122 LOAD_FAST                0 (values)
                      124 GET_ITER
                      126 PRECALL                  0
                      130 CALL                     0
                      140 RETURN_VALUE
          
-         458     >>  142 LOAD_FAST                1 (target_type)
+         464     >>  142 LOAD_FAST                1 (target_type)
                      144 LOAD_GLOBAL              4 (list)
                      156 COMPARE_OP               2 (==)
                      162 POP_JUMP_FORWARD_IF_FALSE    12 (to 188)
          
-         459         164 LOAD_CONST               3 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 459>)
+         465         164 LOAD_CONST               3 (<code object <listcomp>, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 465>)
                      166 MAKE_FUNCTION            0
                      168 LOAD_FAST                0 (values)
                      170 GET_ITER
                      172 PRECALL                  0
                      176 CALL                     0
                      186 RETURN_VALUE
          
-         462     >>  188 LOAD_FAST                0 (values)
+         468     >>  188 LOAD_FAST                0 (values)
                      190 LOAD_CONST               1 (0)
                      192 BINARY_SUBSCR
                      202 STORE_FAST               2 (value)
          
-         464         204 LOAD_FAST                2 (value)
+         470         204 LOAD_FAST                2 (value)
                      206 POP_JUMP_FORWARD_IF_NOT_NONE     1 (to 210)
          
-         465         208 JUMP_FORWARD           201 (to 612)
+         471         208 JUMP_FORWARD           201 (to 612)
          
-         466     >>  210 LOAD_GLOBAL              9 (NULL + isinstance)
+         472     >>  210 LOAD_GLOBAL              9 (NULL + isinstance)
                      222 LOAD_FAST                2 (value)
                      224 LOAD_FAST                1 (target_type)
                      226 PRECALL                  2
                      230 CALL                     2
                      240 POP_JUMP_FORWARD_IF_FALSE     2 (to 246)
          
-         467         242 LOAD_FAST                2 (value)
+         473         242 LOAD_FAST                2 (value)
                      244 RETURN_VALUE
          
-         468     >>  246 LOAD_GLOBAL             11 (NULL + issubclass)
+         474     >>  246 LOAD_GLOBAL             11 (NULL + issubclass)
                      258 LOAD_GLOBAL             12 (str)
                      270 LOAD_FAST                1 (target_type)
                      272 PRECALL                  2
                      276 CALL                     2
                      286 POP_JUMP_FORWARD_IF_FALSE    15 (to 318)
          
-         469         288 LOAD_GLOBAL             13 (NULL + str)
+         475         288 LOAD_GLOBAL             13 (NULL + str)
                      300 LOAD_FAST                2 (value)
                      302 PRECALL                  1
                      306 CALL                     1
                      316 RETURN_VALUE
          
-         470     >>  318 LOAD_GLOBAL             11 (NULL + issubclass)
+         476     >>  318 LOAD_GLOBAL             11 (NULL + issubclass)
                      330 LOAD_GLOBAL             14 (int)
                      342 LOAD_FAST                1 (target_type)
                      344 PRECALL                  2
                      348 CALL                     2
                      358 POP_JUMP_FORWARD_IF_FALSE    15 (to 390)
          
-         471         360 LOAD_GLOBAL             15 (NULL + int)
+         477         360 LOAD_GLOBAL             15 (NULL + int)
                      372 LOAD_FAST                2 (value)
                      374 PRECALL                  1
                      378 CALL                     1
                      388 RETURN_VALUE
          
-         472     >>  390 LOAD_GLOBAL             11 (NULL + issubclass)
+         478     >>  390 LOAD_GLOBAL             11 (NULL + issubclass)
                      402 LOAD_GLOBAL             16 (float)
                      414 LOAD_FAST                1 (target_type)
                      416 PRECALL                  2
                      420 CALL                     2
                      430 POP_JUMP_FORWARD_IF_FALSE    15 (to 462)
          
-         473         432 LOAD_GLOBAL             17 (NULL + float)
+         479         432 LOAD_GLOBAL             17 (NULL + float)
                      444 LOAD_FAST                2 (value)
                      446 PRECALL                  1
                      450 CALL                     1
                      460 RETURN_VALUE
          
-         474     >>  462 LOAD_GLOBAL             11 (NULL + issubclass)
+         480     >>  462 LOAD_GLOBAL             11 (NULL + issubclass)
                      474 LOAD_GLOBAL             18 (bool)
                      486 LOAD_FAST                1 (target_type)
                      488 PRECALL                  2
                      492 CALL                     2
                      502 POP_JUMP_FORWARD_IF_FALSE     8 (to 520)
          
-         475         504 LOAD_FAST                2 (value)
+         481         504 LOAD_FAST                2 (value)
                      506 LOAD_CONST               4 ((False, '', 'false', 'False'))
                      508 CONTAINS_OP              0
                      510 POP_JUMP_FORWARD_IF_FALSE     2 (to 516)
                      512 LOAD_CONST               5 (False)
                      514 JUMP_FORWARD             1 (to 518)
                  >>  516 LOAD_CONST               6 (True)
                  >>  518 RETURN_VALUE
          
-         476     >>  520 LOAD_GLOBAL             11 (NULL + issubclass)
+         482     >>  520 LOAD_GLOBAL             11 (NULL + issubclass)
                      532 LOAD_GLOBAL             20 (uuid)
                      544 LOAD_ATTR               11 (UUID)
                      554 LOAD_FAST                1 (target_type)
                      556 PRECALL                  2
                      560 CALL                     2
                      570 POP_JUMP_FORWARD_IF_FALSE    20 (to 612)
          
-         477         572 LOAD_GLOBAL             21 (NULL + uuid)
+         483         572 LOAD_GLOBAL             21 (NULL + uuid)
                      584 LOAD_ATTR               11 (UUID)
                      594 LOAD_FAST                2 (value)
                      596 PRECALL                  1
                      600 CALL                     1
                      610 RETURN_VALUE
          
-         479     >>  612 LOAD_GLOBAL             25 (NULL + ValueError)
+         485     >>  612 LOAD_GLOBAL             25 (NULL + ValueError)
                      624 LOAD_CONST               7 ('Unsupported type: ')
                      626 LOAD_FAST                1 (target_type)
                      628 FORMAT_VALUE             0
                      630 LOAD_CONST               8 (' for value: ')
                      632 LOAD_FAST                2 (value)
                      634 FORMAT_VALUE             0
                      636 BUILD_STRING             4
@@ -3920,15 +3955,15 @@
                stacksize : 6
                flags     : 19
                code
                   0x9501970067007c005d137d017401000000000000000000007c01670189
                   02a6020000ab02000000000000000091028c145300
                              0 COPY_FREE_VARS           1
                
-               456           2 RESUME                   0
+               462           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                19 (to 48)
                             10 STORE_FAST               1 (v)
                             12 LOAD_GLOBAL              1 (NULL + _convert_value_to_type)
                             24 LOAD_FAST                1 (v)
                             26 BUILD_LIST               1
@@ -3941,25 +3976,25 @@
                consts
                names      ('_convert_value_to_type',)
                varnames   ('.0', 'v')
                freevars   ('list_type',)
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '<listcomp>'
-               firstlineno 456
+               firstlineno 462
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 19
                code
                   0x970067007c005d187d017401000000000000000000007c016701740200
                   000000000000000000a6020000ab02000000000000000091028c195300
-               459           0 RESUME                   0
+               465           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                24 (to 56)
                              8 STORE_FAST               1 (v)
                             10 LOAD_GLOBAL              1 (NULL + _convert_value_to_type)
                             22 LOAD_FAST                1 (v)
                             24 BUILD_LIST               1
@@ -3972,81 +4007,81 @@
                consts
                names      ('_convert_value_to_type', 'str')
                varnames   ('.0', 'v')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       '<listcomp>'
-               firstlineno 459
+               firstlineno 465
                lnotab 0x
             (False, '', 'false', 'False')
             False
             True
             'Unsupported type: '
             ' for value: '
          names      ('typing', 'get_origin', 'list', 'get_args', 'isinstance', 'issubclass', 'str', 'int', 'float', 'bool', 'uuid', 'UUID', 'ValueError')
          varnames   ('values', 'target_type', 'value')
          freevars   ()
          cellvars   ('list_type',)
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_convert_value_to_type'
-         firstlineno 452
+         firstlineno 458
          lnotab
             0x04023a0134011c0216011803100204010201200104012a011e012a011e
             012a011e012a01100134012802
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a02640184005a0364026504640365056506650466
             02190000000000000000006604640484045a0764056508640665096a0a00
             000000000000006407650b650c190000000000000000006606640884045a
             0d64095300
-         487           0 RESUME                   0
+         493           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InjectedParamForm')
                        8 STORE_NAME               2 (__qualname__)
          
-         488          10 LOAD_CONST               1 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 488>)
+         494          10 LOAD_CONST               1 (<code object check, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 494>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (check)
          
-         494          16 LOAD_CONST               2 ('args')
+         500          16 LOAD_CONST               2 ('args')
                       18 LOAD_NAME                4 (Any)
                       20 LOAD_CONST               3 ('kwargs')
                       22 LOAD_NAME                5 (dict)
                       24 LOAD_NAME                6 (str)
                       26 LOAD_NAME                4 (Any)
                       28 BUILD_TUPLE              2
                       30 BINARY_SUBSCR
                       40 BUILD_TUPLE              4
-                      42 LOAD_CONST               4 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 494>)
+                      42 LOAD_CONST               4 (<code object get_value, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 500>)
                       44 MAKE_FUNCTION            4 (annotations)
                       46 STORE_NAME               7 (get_value)
          
-         506          48 LOAD_CONST               5 ('request')
+         512          48 LOAD_CONST               5 ('request')
          
-         507          50 LOAD_NAME                8 (HttpRequest)
+         513          50 LOAD_NAME                8 (HttpRequest)
          
-         506          52 LOAD_CONST               6 ('value')
+         512          52 LOAD_CONST               6 ('value')
          
-         507          54 LOAD_NAME                9 (forms)
+         513          54 LOAD_NAME                9 (forms)
                       56 LOAD_ATTR               10 (Form)
          
-         506          66 LOAD_CONST               7 ('return')
+         512          66 LOAD_CONST               7 ('return')
          
-         508          68 LOAD_NAME               11 (Optional)
+         514          68 LOAD_NAME               11 (Optional)
                       70 LOAD_NAME               12 (HttpResponse)
                       72 BINARY_SUBSCR
          
-         506          82 BUILD_TUPLE              6
-                      84 LOAD_CONST               8 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 506>)
+         512          82 BUILD_TUPLE              6
+                      84 LOAD_CONST               8 (<code object replace_response, file "/home/roman/prjs/python/dfv/dfv/__init__.py", line 512>)
                       86 MAKE_FUNCTION            4 (annotations)
                       88 STORE_NAME              13 (replace_response)
                       90 LOAD_CONST               9 (None)
                       92 RETURN_VALUE
          consts
             'InjectedParamForm'
             code
@@ -4055,49 +4090,49 @@
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000740400
                   0000000000000000006a030000000000000000a6020000ab020000000000
                   000000731774090000000000000000000064017c006a0100000000000000
                   009b009d02a6010000ab010000000000000000820164005300
-               488           0 RESUME                   0
+               494           0 RESUME                   0
                
-               489           2 LOAD_GLOBAL              1 (NULL + issubclass)
+               495           2 LOAD_GLOBAL              1 (NULL + issubclass)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (target_type)
                             26 LOAD_GLOBAL              4 (forms)
                             38 LOAD_ATTR                3 (BaseForm)
                             48 PRECALL                  2
                             52 CALL                     2
                             62 POP_JUMP_FORWARD_IF_TRUE    23 (to 110)
                
-               490          64 LOAD_GLOBAL              9 (NULL + Exception)
+               496          64 LOAD_GLOBAL              9 (NULL + Exception)
                
-               491          76 LOAD_CONST               1 ('argument type for handle_form() must be a subclass of django.forms.BaseForm, got ')
+               497          76 LOAD_CONST               1 ('argument type for handle_form() must be a subclass of django.forms.BaseForm, got ')
                             78 LOAD_FAST                0 (self)
                             80 LOAD_ATTR                1 (target_type)
                             90 FORMAT_VALUE             0
                             92 BUILD_STRING             2
                
-               490          94 PRECALL                  1
+               496          94 PRECALL                  1
                             98 CALL                     1
                            108 RAISE_VARARGS            1
                
-               489     >>  110 LOAD_CONST               0 (None)
+               495     >>  110 LOAD_CONST               0 (None)
                            112 RETURN_VALUE
                consts
                   None
                   'argument type for handle_form() must be a subclass of django.forms.BaseForm, got '
                names      ('issubclass', 'target_type', 'forms', 'BaseForm', 'Exception')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'check'
-               firstlineno 488
+               firstlineno 494
                lnotab 0x02013e010c0112ff10ff
             'args'
             'kwargs'
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
@@ -4114,99 +4149,99 @@
                   0000000000000000007d057c05a00a000000000000000000000000000000
                   00000000007417000000000000000000006a0c00000000000000007c036a
                   0d0000000000000000a6010000ab010000000000000000a6010000ab0100
                   0000000000000001007c00a0020000000000000000000000000000000000
                   0000007c05ac03a6010000ab0100000000000000007d046e147c00a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   0000007d047c045300
-               494           0 RESUME                   0
+               500           0 RESUME                   0
                
-               495           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
+               501           2 LOAD_GLOBAL              1 (NULL + _get_request_from_args)
                             14 LOAD_FAST                1 (args)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               3 (request)
                
-               496          32 LOAD_GLOBAL              3 (NULL + is_post)
+               502          32 LOAD_GLOBAL              3 (NULL + is_post)
                             44 LOAD_FAST                3 (request)
                             46 PRECALL                  1
                             50 CALL                     1
                             60 POP_JUMP_FORWARD_IF_FALSE    34 (to 130)
                
-               497          62 LOAD_FAST                0 (self)
+               503          62 LOAD_FAST                0 (self)
                             64 LOAD_METHOD              2 (target_type)
                             86 LOAD_FAST                3 (request)
                             88 LOAD_ATTR                3 (POST)
                             98 LOAD_FAST                3 (request)
                            100 LOAD_ATTR                4 (FILES)
                            110 KW_NAMES                 1
                            112 PRECALL                  2
                            116 CALL                     2
                            126 STORE_FAST               4 (form)
                            128 JUMP_FORWARD           147 (to 424)
                
-               498     >>  130 LOAD_FAST                3 (request)
+               504     >>  130 LOAD_FAST                3 (request)
                            132 LOAD_ATTR                5 (content_type)
                            142 LOAD_CONST               2 ('application/json')
                            144 COMPARE_OP               2 (==)
                            150 POP_JUMP_FORWARD_IF_FALSE   116 (to 384)
                
-               499         152 LOAD_GLOBAL             13 (NULL + typing)
+               505         152 LOAD_GLOBAL             13 (NULL + typing)
                            164 LOAD_ATTR                7 (cast)
                            174 LOAD_GLOBAL             16 (QueryDict)
                            186 LOAD_FAST                3 (request)
                            188 LOAD_ATTR                3 (POST)
                            198 PRECALL                  2
                            202 CALL                     2
                            212 LOAD_METHOD              9 (copy)
                            234 PRECALL                  0
                            238 CALL                     0
                            248 STORE_FAST               5 (new_post_dict)
                
-               500         250 LOAD_FAST                5 (new_post_dict)
+               506         250 LOAD_FAST                5 (new_post_dict)
                            252 LOAD_METHOD             10 (update)
                            274 LOAD_GLOBAL             23 (NULL + json)
                            286 LOAD_ATTR               12 (loads)
                            296 LOAD_FAST                3 (request)
                            298 LOAD_ATTR               13 (body)
                            308 PRECALL                  1
                            312 CALL                     1
                            322 PRECALL                  1
                            326 CALL                     1
                            336 POP_TOP
                
-               501         338 LOAD_FAST                0 (self)
+               507         338 LOAD_FAST                0 (self)
                            340 LOAD_METHOD              2 (target_type)
                            362 LOAD_FAST                5 (new_post_dict)
                            364 KW_NAMES                 3
                            366 PRECALL                  1
                            370 CALL                     1
                            380 STORE_FAST               4 (form)
                            382 JUMP_FORWARD            20 (to 424)
                
-               503     >>  384 LOAD_FAST                0 (self)
+               509     >>  384 LOAD_FAST                0 (self)
                            386 LOAD_METHOD              2 (target_type)
                            408 PRECALL                  0
                            412 CALL                     0
                            422 STORE_FAST               4 (form)
                
-               504     >>  424 LOAD_FAST                4 (form)
+               510     >>  424 LOAD_FAST                4 (form)
                            426 RETURN_VALUE
                consts
                   None
                   ('data', 'files')
                   'application/json'
                   ('data',)
                names      ('_get_request_from_args', 'is_post', 'target_type', 'POST', 'FILES', 'content_type', 'typing', 'cast', 'QueryDict', 'copy', 'update', 'json', 'loads', 'body')
                varnames   ('self', 'args', 'kwargs', 'request', 'form', 'new_post_dict')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'get_value'
-               firstlineno 494
+               firstlineno 500
                lnotab 0x02011e011e0144011601620158012e022801
             'request'
             'value'
             'return'
             code
                argcount  : 3
                nlocals   : 7
@@ -4225,228 +4260,228 @@
                   0000000000a6010000ab0100000000000000007c066a0b00000000000000
                   0064049c037c047c056a0a00000000000000003c0000008c557419000000
                   000000000000007c037c047413000000000000000000007c02a00d000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   00a6010000ab0100000000000000007c02a0040000000000000000000000
                   000000000000000000a6000000ab00000000000000000064059c04a60100
                   00ab010000000000000000530064005300
-               506           0 RESUME                   0
+               512           0 RESUME                   0
                
-               509           2 LOAD_GLOBAL              1 (NULL + is_patch)
+               515           2 LOAD_GLOBAL              1 (NULL + is_patch)
                             14 LOAD_FAST                1 (request)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 POP_JUMP_FORWARD_IF_FALSE   215 (to 462)
                             32 LOAD_FAST                1 (request)
                             34 LOAD_ATTR                1 (content_type)
                             44 LOAD_CONST               1 ('application/json')
                             46 COMPARE_OP               2 (==)
                             52 POP_JUMP_FORWARD_IF_FALSE   204 (to 462)
                
-               510          54 LOAD_FAST                1 (request)
+               516          54 LOAD_FAST                1 (request)
                             56 LOAD_ATTR                2 (headers)
                             66 LOAD_METHOD              3 (get)
                             88 LOAD_CONST               2 ('X-DFV-Validate-Field')
                             90 PRECALL                  1
                             94 CALL                     1
                            104 STORE_FAST               3 (validate_field)
                
-               511         106 LOAD_FAST                2 (value)
+               517         106 LOAD_FAST                2 (value)
                            108 LOAD_METHOD              4 (is_valid)
                            130 PRECALL                  0
                            134 CALL                     0
                            144 POP_TOP
                
-               512         146 BUILD_MAP                0
+               518         146 BUILD_MAP                0
                            148 STORE_FAST               4 (fields)
                
-               513         150 LOAD_FAST                2 (value)
+               519         150 LOAD_FAST                2 (value)
                            152 GET_ITER
                        >>  154 FOR_ITER                84 (to 324)
                            156 STORE_FAST               5 (bound_field)
                
-               514         158 LOAD_FAST                5 (bound_field)
+               520         158 LOAD_FAST                5 (bound_field)
                            160 LOAD_ATTR                5 (field)
                            170 LOAD_ATTR                6 (widget)
                            180 STORE_FAST               6 (widget)
                
-               516         182 LOAD_GLOBAL             15 (NULL + len)
+               522         182 LOAD_GLOBAL             15 (NULL + len)
                            194 LOAD_FAST                5 (bound_field)
                            196 LOAD_ATTR                8 (errors)
                            206 PRECALL                  1
                            210 CALL                     1
                            220 LOAD_CONST               3 (0)
                            222 COMPARE_OP               2 (==)
                
-               517         228 LOAD_GLOBAL             19 (NULL + str)
+               523         228 LOAD_GLOBAL             19 (NULL + str)
                            240 LOAD_FAST                2 (value)
                            242 LOAD_FAST                5 (bound_field)
                            244 LOAD_ATTR               10 (name)
                            254 BINARY_SUBSCR
                            264 LOAD_ATTR                8 (errors)
                            274 PRECALL                  1
                            278 CALL                     1
                
-               518         288 LOAD_FAST                6 (widget)
+               524         288 LOAD_FAST                6 (widget)
                            290 LOAD_ATTR               11 (attrs)
                
-               515         300 LOAD_CONST               4 (('valid', 'errors', 'attrs'))
+               521         300 LOAD_CONST               4 (('valid', 'errors', 'attrs'))
                            302 BUILD_CONST_KEY_MAP      3
                            304 LOAD_FAST                4 (fields)
                            306 LOAD_FAST                5 (bound_field)
                            308 LOAD_ATTR               10 (name)
                            318 STORE_SUBSCR
                            322 JUMP_BACKWARD           85 (to 154)
                
-               521     >>  324 LOAD_GLOBAL             25 (NULL + JsonResponse)
+               527     >>  324 LOAD_GLOBAL             25 (NULL + JsonResponse)
                
-               523         336 LOAD_FAST                3 (validate_field)
+               529         336 LOAD_FAST                3 (validate_field)
                
-               524         338 LOAD_FAST                4 (fields)
+               530         338 LOAD_FAST                4 (fields)
                
-               525         340 LOAD_GLOBAL             19 (NULL + str)
+               531         340 LOAD_GLOBAL             19 (NULL + str)
                            352 LOAD_FAST                2 (value)
                            354 LOAD_METHOD             13 (non_field_errors)
                            376 PRECALL                  0
                            380 CALL                     0
                            390 PRECALL                  1
                            394 CALL                     1
                
-               526         404 LOAD_FAST                2 (value)
+               532         404 LOAD_FAST                2 (value)
                            406 LOAD_METHOD              4 (is_valid)
                            428 PRECALL                  0
                            432 CALL                     0
                
-               522         442 LOAD_CONST               5 (('name', 'fields', 'non_field_errors', 'form_valid'))
+               528         442 LOAD_CONST               5 (('name', 'fields', 'non_field_errors', 'form_valid'))
                            444 BUILD_CONST_KEY_MAP      4
                
-               521         446 PRECALL                  1
+               527         446 PRECALL                  1
                            450 CALL                     1
                            460 RETURN_VALUE
                
-               530     >>  462 LOAD_CONST               0 (None)
+               536     >>  462 LOAD_CONST               0 (None)
                            464 RETURN_VALUE
                consts
                   None
                   'application/json'
                   'X-DFV-Validate-Field'
                   0
                   ('valid', 'errors', 'attrs')
                   ('name', 'fields', 'non_field_errors', 'form_valid')
                names      ('is_patch', 'content_type', 'headers', 'get', 'is_valid', 'field', 'widget', 'len', 'errors', 'str', 'name', 'attrs', 'JsonResponse', 'non_field_errors')
                varnames   ('self', 'request', 'value', 'validate_field', 'fields', 'bound_field', 'widget')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
                name       'replace_response'
-               firstlineno 506
+               firstlineno 512
                lnotab
                   0x02033401340128010401080118022e013c010cfd18060c020201020140
                   0126fc04ff1009
             None
          names      ('__name__', '__module__', '__qualname__', 'check', 'Any', 'dict', 'str', 'get_value', 'HttpRequest', 'forms', 'Form', 'Optional', 'HttpResponse', 'replace_response')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'InjectedParamForm'
-         firstlineno 487
+         firstlineno 493
          lnotab 0x0a010606200c020102ff02010cff02020efe
       'InjectedParamForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab00000000000000000053
             00
-         533           0 RESUME                   0
+         539           0 RESUME                   0
          
-         534           2 LOAD_GLOBAL              1 (NULL + InjectedParamForm)
+         540           2 LOAD_GLOBAL              1 (NULL + InjectedParamForm)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 RETURN_VALUE
          consts
             None
          names      ('InjectedParamForm',)
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'handle_form'
-         firstlineno 533
+         firstlineno 539
          lnotab 0x0201
       'querydict'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401ac02a6010000ab010000000000
             0000007d027c02a00100000000000000000000000000000000000000007c
             00a6010000ab01000000000000000001007c027c013d007c025300
-         542           0 RESUME                   0
+         548           0 RESUME                   0
          
-         543           2 LOAD_GLOBAL              1 (NULL + QueryDict)
+         549           2 LOAD_GLOBAL              1 (NULL + QueryDict)
                       14 LOAD_CONST               1 (True)
                       16 KW_NAMES                 2
                       18 PRECALL                  1
                       22 CALL                     1
                       32 STORE_FAST               2 (temp)
          
-         544          34 LOAD_FAST                2 (temp)
+         550          34 LOAD_FAST                2 (temp)
                       36 LOAD_METHOD              1 (update)
                       58 LOAD_FAST                0 (querydict)
                       60 PRECALL                  1
                       64 CALL                     1
                       74 POP_TOP
          
-         545          76 LOAD_FAST                2 (temp)
+         551          76 LOAD_FAST                2 (temp)
                       78 LOAD_FAST                1 (key)
                       80 DELETE_SUBSCR
          
-         546          82 LOAD_FAST                2 (temp)
+         552          82 LOAD_FAST                2 (temp)
                       84 RETURN_VALUE
          consts
             None
             True
             ('mutable',)
          names      ('QueryDict', 'update')
          varnames   ('querydict', 'key', 'temp')
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       'querydict_key_removed'
-         firstlineno 542
+         firstlineno 548
          lnotab 0x020120012a010601
       'args'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x97007c006401190000000000000000005300
-         549           0 RESUME                   0
+         555           0 RESUME                   0
          
-         550           2 LOAD_FAST                0 (args)
+         556           2 LOAD_FAST                0 (args)
                        4 LOAD_CONST               1 (0)
                        6 BINARY_SUBSCR
                       16 RETURN_VALUE
          consts
             None
             0
          names      ()
          varnames   ('args',)
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/__init__.py'
          name       '_get_request_from_args'
-         firstlineno 549
+         firstlineno 555
          lnotab 0x0201
       (None,)
       ('outerHTML',)
       (True,)
       (None, True)
    names      ('dataclasses', 'functools', 'inspect', 'json', 'typing', 'uuid', 'types', 'NoneType', 'Any', 'Callable', 'Literal', 'Optional', 'ParamSpec', 'TypeVar', 'lxml.html', 'lxml', 'wrapt', 'django', 'forms', 'django.contrib.auth', 'decorators', 'auth_decorators', 'django.http', 'HttpRequest', 'HttpResponse', 'JsonResponse', 'QueryDict', 'django.template.response', 'TemplateResponse', 'django.utils.safestring', 'mark_safe', 'SafeString', 'P', 'R', 'T', 'ObjectProxy', 'ElementResponse', 'response_to_str', 'str', 'list', 'element', 'swap_oob', 'overload', 'get_view_fn_call_stack_from_request', 'bool', 'view', 'is_view_fn_request_target', 'is_head', 'is_get', 'is_post', 'is_put', 'is_patch', 'is_delete', 'inject_args', '_inject_args', 'dataclass', 'InjectedParam', 'Parameter', '_setup_injected_param', 'dict', '_extract_injected_params', 'InjectedParamQuery', 'InjectedParamQueryGet', 'InjectedParamQueryPost', 'param_get', 'param_post', 'cast', 'param', 'type', '_convert_value_to_type', 'InjectedParamForm', 'handle_form', 'querydict_key_removed', '_get_request_from_args')
    varnames   ()
@@ -4457,12 +4492,12 @@
    firstlineno 1
    lnotab
       0x00ff02010801080108010801080108010c012002080108010c010c0118
       010c0110021601160116082621160902ff02030201020102010201020102
       0102f706010eff02060efa02081af8020a34f6082e02ff040102ff020102
       ff020202fe08150c011aff0e0102040c01020102ff020102ff02021afe06
       ff0e01020702ff040102ff02021afe080b0201020102fc06021afe020534
-      fb08220c050c040c040c040c040c040c0b020102fd060214fe020314fd02
+      fb08220c0b0c040c040c040c040c040c0b020102fd060214fe020314fd02
       0434fc082204030c0118ff0e010211020114ff020202fe020302fd02040c
       fc081b02fc040114ff020218fe020326fd020414fc020512fb08400c011a
       ff0e01022f0c011aff0e01020c0c011aff0e01020c0e040e04340426231c
       2e0c091007
```

### Comparing `dfv-0.8.0/dfv/__pycache__/test_element.cpython-311.pyc` & `dfv-0.9.0/dfv/__pycache__/test_element.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.8.0/dfv/__pycache__/test_form.cpython-311.pyc` & `dfv-0.9.0/dfv/__pycache__/test_form.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,52 +1,53 @@
 magic:    0xa70d0d0a
-moddate:  0x3cc7c464 (Sat Jul 29 08:01:00 2023 UTC)
-files sz: 3340
+moddate:  0x000acc64 (Thu Aug  3 20:11:44 2023 UTC)
+files sz: 3649
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c005a00640064026c016d025a020100640064036c036d
-      045a040100640064016c055a05640064016c015a01640064046c056d065a
+      0x9700640064016c005a00640064016c015a01640064026c016d025a0201
+      00640064036c036d045a040100640064016c055a05640064046c056d065a
       060100640064056c076d085a080100640064066c096d0a5a0a0100640064
-      076c0b6d0c5a0c6d0d5a0d01000200470064088400640965066a0e000000
-      0000000000a6030000ab0300000000000000005a0f02004700640a840064
-      0b6504a6030000ab0300000000000000005a1064015300
+      076c0b6d0c5a0c6d0d5a0d0100640064086c0e6d0f5a0f6d105a10010064
+      0064096c116d125a12010002004700640a8400640b65066a130000000000
+      000000a6030000ab0300000000000000005a1402004700640c8400640d65
+      04a6030000ab0300000000000000005a1564015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (json)
                  8 STORE_NAME               0 (json)
    
      2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('Any',))
+                12 LOAD_CONST               1 (None)
                 14 IMPORT_NAME              1 (typing)
-                16 IMPORT_FROM              2 (Any)
-                18 STORE_NAME               2 (Any)
-                20 POP_TOP
+                16 STORE_NAME               1 (typing)
    
-     3          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               3 (('TestCase',))
-                26 IMPORT_NAME              3 (unittest)
-                28 IMPORT_FROM              4 (TestCase)
-                30 STORE_NAME               4 (TestCase)
-                32 POP_TOP
+     3          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               2 (('Any',))
+                22 IMPORT_NAME              1 (typing)
+                24 IMPORT_FROM              2 (Any)
+                26 STORE_NAME               2 (Any)
+                28 POP_TOP
    
-     5          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               1 (None)
-                38 IMPORT_NAME              5 (django)
-                40 STORE_NAME               5 (django)
+     4          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('TestCase',))
+                34 IMPORT_NAME              3 (unittest)
+                36 IMPORT_FROM              4 (TestCase)
+                38 STORE_NAME               4 (TestCase)
+                40 POP_TOP
    
      6          42 LOAD_CONST               0 (0)
                 44 LOAD_CONST               1 (None)
-                46 IMPORT_NAME              1 (typing)
-                48 STORE_NAME               1 (typing)
+                46 IMPORT_NAME              5 (django)
+                48 STORE_NAME               5 (django)
    
      7          50 LOAD_CONST               0 (0)
                 52 LOAD_CONST               4 (('forms',))
                 54 IMPORT_NAME              5 (django)
                 56 IMPORT_FROM              6 (forms)
                 58 STORE_NAME               6 (forms)
                 60 POP_TOP
@@ -61,77 +62,95 @@
      9          74 LOAD_CONST               0 (0)
                 76 LOAD_CONST               6 (('RequestFactory',))
                 78 IMPORT_NAME              9 (django.test)
                 80 IMPORT_FROM             10 (RequestFactory)
                 82 STORE_NAME              10 (RequestFactory)
                 84 POP_TOP
    
-    11          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               7 (('inject_args', 'handle_form'))
-                90 IMPORT_NAME             11 (dfv)
-                92 IMPORT_FROM             12 (inject_args)
-                94 STORE_NAME              12 (inject_args)
-                96 IMPORT_FROM             13 (handle_form)
-                98 STORE_NAME              13 (handle_form)
+    10          86 LOAD_CONST               0 (0)
+                88 LOAD_CONST               7 (('path', 'resolve'))
+                90 IMPORT_NAME             11 (django.urls)
+                92 IMPORT_FROM             12 (path)
+                94 STORE_NAME              12 (path)
+                96 IMPORT_FROM             13 (resolve)
+                98 STORE_NAME              13 (resolve)
                100 POP_TOP
    
-    14         102 PUSH_NULL
-               104 LOAD_BUILD_CLASS
-               106 LOAD_CONST               8 (<code object TestForm, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 14>)
-               108 MAKE_FUNCTION            0
-               110 LOAD_CONST               9 ('TestForm')
-               112 LOAD_NAME                6 (forms)
-               114 LOAD_ATTR               14 (Form)
-               124 PRECALL                  3
-               128 CALL                     3
-               138 STORE_NAME              15 (TestForm)
+    12         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               8 (('handle_form', 'view'))
+               106 IMPORT_NAME             14 (dfv)
+               108 IMPORT_FROM             15 (handle_form)
+               110 STORE_NAME              15 (handle_form)
+               112 IMPORT_FROM             16 (view)
+               114 STORE_NAME              16 (view)
+               116 POP_TOP
    
-    19         140 PUSH_NULL
-               142 LOAD_BUILD_CLASS
-               144 LOAD_CONST              10 (<code object ParamsToArgsDecoratorTestCase, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 19>)
-               146 MAKE_FUNCTION            0
-               148 LOAD_CONST              11 ('ParamsToArgsDecoratorTestCase')
-               150 LOAD_NAME                4 (TestCase)
+    13         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST               9 (('create_resolved_request',))
+               122 IMPORT_NAME             17 (dfv.testutils)
+               124 IMPORT_FROM             18 (create_resolved_request)
+               126 STORE_NAME              18 (create_resolved_request)
+               128 POP_TOP
+   
+    16         130 PUSH_NULL
+               132 LOAD_BUILD_CLASS
+               134 LOAD_CONST              10 (<code object TestForm, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 16>)
+               136 MAKE_FUNCTION            0
+               138 LOAD_CONST              11 ('TestForm')
+               140 LOAD_NAME                6 (forms)
+               142 LOAD_ATTR               19 (Form)
                152 PRECALL                  3
                156 CALL                     3
-               166 STORE_NAME              16 (ParamsToArgsDecoratorTestCase)
-               168 LOAD_CONST               1 (None)
-               170 RETURN_VALUE
+               166 STORE_NAME              20 (TestForm)
+   
+    21         168 PUSH_NULL
+               170 LOAD_BUILD_CLASS
+               172 LOAD_CONST              12 (<code object ParamsToArgsDecoratorTestCase, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 21>)
+               174 MAKE_FUNCTION            0
+               176 LOAD_CONST              13 ('ParamsToArgsDecoratorTestCase')
+               178 LOAD_NAME                4 (TestCase)
+               180 PRECALL                  3
+               184 CALL                     3
+               194 STORE_NAME              21 (ParamsToArgsDecoratorTestCase)
+               196 LOAD_CONST               1 (None)
+               198 RETURN_VALUE
    consts
       0
       None
       ('Any',)
       ('TestCase',)
       ('forms',)
       ('HttpResponse',)
       ('RequestFactory',)
-      ('inject_args', 'handle_form')
+      ('path', 'resolve')
+      ('handle_form', 'view')
+      ('create_resolved_request',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02020065036a040000000000000000a6000000ab
             0000000000000000005a05020065036a040000000000000000a6000000ab
             0000000000000000005a0664015300
-          14           0 RESUME                   0
+          16           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('TestForm')
                        8 STORE_NAME               2 (__qualname__)
          
-          15          10 PUSH_NULL
+          17          10 PUSH_NULL
                       12 LOAD_NAME                3 (forms)
                       14 LOAD_ATTR                4 (CharField)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_NAME               5 (p1)
          
-          16          40 PUSH_NULL
+          18          40 PUSH_NULL
                       42 LOAD_NAME                3 (forms)
                       44 LOAD_ATTR                4 (CharField)
                       54 PRECALL                  0
                       58 CALL                     0
                       68 STORE_NAME               6 (p2)
                       70 LOAD_CONST               1 (None)
                       72 RETURN_VALUE
@@ -140,68 +159,68 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'forms', 'CharField', 'p1', 'p2')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
          name       'TestForm'
-         firstlineno 14
+         firstlineno 16
          lnotab 0x0a011e01
       'TestForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c000000640c640484045a
             05640584005a06640684005a07640784005a08640884005a09640984005a
             0a640a84005a0b640b84005a0c64035300
-          19           0 RESUME                   0
+          21           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParamsToArgsDecoratorTestCase')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          20          12 LOAD_NAME                3 (RequestFactory)
+          22          12 LOAD_NAME                3 (RequestFactory)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('factory')
                       18 STORE_SUBSCR
          
-          22          22 LOAD_CONST              12 (('return', None))
-                      24 LOAD_CONST               4 (<code object setUp, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 22>)
+          24          22 LOAD_CONST              12 (('return', None))
+                      24 LOAD_CONST               4 (<code object setUp, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 24>)
                       26 MAKE_FUNCTION            4 (annotations)
                       28 STORE_NAME               5 (setUp)
          
-          26          30 LOAD_CONST               5 (<code object test_error_missing_form_type, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 26>)
+          28          30 LOAD_CONST               5 (<code object test_error_missing_form_type, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 28>)
                       32 MAKE_FUNCTION            0
                       34 STORE_NAME               6 (test_error_missing_form_type)
          
-          38          36 LOAD_CONST               6 (<code object test_error_wrong_form_type, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 38>)
+          40          36 LOAD_CONST               6 (<code object test_error_wrong_form_type, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 40>)
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               7 (test_error_wrong_form_type)
          
-          50          42 LOAD_CONST               7 (<code object test_form_explicit, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 50>)
+          52          42 LOAD_CONST               7 (<code object test_form_explicit, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 52>)
                       44 MAKE_FUNCTION            0
                       46 STORE_NAME               8 (test_form_explicit)
          
-          58          48 LOAD_CONST               8 (<code object test_form_implicit, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 58>)
+          60          48 LOAD_CONST               8 (<code object test_form_implicit, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 60>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               9 (test_form_implicit)
          
-          66          54 LOAD_CONST               9 (<code object test_form_get, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 66>)
+          70          54 LOAD_CONST               9 (<code object test_form_get, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 70>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME              10 (test_form_get)
          
-          75          60 LOAD_CONST              10 (<code object test_form_post, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 75>)
+          79          60 LOAD_CONST              10 (<code object test_form_post, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 79>)
                       62 MAKE_FUNCTION            0
                       64 STORE_NAME              11 (test_form_post)
          
-          86          66 LOAD_CONST              11 (<code object test_form_patch, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 86>)
+          90          66 LOAD_CONST              11 (<code object test_form_patch, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 90>)
                       68 MAKE_FUNCTION            0
                       70 STORE_NAME              12 (test_form_patch)
                       72 LOAD_CONST               3 (None)
                       74 RETURN_VALUE
          consts
             'ParamsToArgsDecoratorTestCase'
             'factory'
@@ -212,64 +231,64 @@
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000007c
                   005f0100000000000000007405000000000000000000006a030000000000
                   000000a6000000ab000000000000000000010064005300
-                22           0 RESUME                   0
+                24           0 RESUME                   0
                
-                23           2 LOAD_GLOBAL              1 (NULL + RequestFactory)
+                25           2 LOAD_GLOBAL              1 (NULL + RequestFactory)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (factory)
                
-                24          40 LOAD_GLOBAL              5 (NULL + django)
+                26          40 LOAD_GLOBAL              5 (NULL + django)
                             52 LOAD_ATTR                3 (setup)
                             62 PRECALL                  0
                             66 CALL                     0
                             76 POP_TOP
                             78 LOAD_CONST               0 (None)
                             80 RETURN_VALUE
                consts
                   None
                names      ('RequestFactory', 'factory', 'django', 'setup')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                name       'setUp'
-               firstlineno 22
+               firstlineno 24
                lnotab 0x02012601
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x9700640184007d017c00a0000000000000000000000000000000000000
                   00000074020000000000000000000064027c01a6030000ab030000000000
                   000000010064005300
-                26           0 RESUME                   0
+                28           0 RESUME                   0
                
-                27           2 LOAD_CONST               1 (<code object test, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 27>)
+                29           2 LOAD_CONST               1 (<code object test, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 29>)
                              4 MAKE_FUNCTION            0
                              6 STORE_FAST               1 (test)
                
-                32           8 LOAD_FAST                0 (self)
+                34           8 LOAD_FAST                0 (self)
                             10 LOAD_METHOD              0 (assertRaisesRegex)
                
-                33          32 LOAD_GLOBAL              2 (Exception)
+                35          32 LOAD_GLOBAL              2 (Exception)
                
-                34          44 LOAD_CONST               2 ('argument type for handle_form\\(\\) must be a subclass of django.forms.BaseForm')
+                36          44 LOAD_CONST               2 ('argument type for handle_form\\(\\) must be a subclass of django.forms.BaseForm')
                
-                35          46 LOAD_FAST                1 (test)
+                37          46 LOAD_FAST                1 (test)
                
-                32          48 PRECALL                  3
+                34          48 PRECALL                  3
                             52 CALL                     3
                             62 POP_TOP
                             64 LOAD_CONST               0 (None)
                             66 RETURN_VALUE
                consts
                   None
                   code
@@ -277,102 +296,102 @@
                      nlocals   : 1
                      stacksize : 3
                      flags     : 19
                      code
                         0x9700740100000000000000000000a6000000ab00000000000000000074
                         0300000000000000000000a6000000ab0000000000000000006601640184
                         01a6000000ab0000000000000000007d0064005300
-                      27           0 RESUME                   0
+                      29           0 RESUME                   0
                      
-                      28           2 LOAD_GLOBAL              1 (NULL + inject_args)
+                      30           2 LOAD_GLOBAL              1 (NULL + view)
                                   14 PRECALL                  0
                                   18 CALL                     0
                      
-                      29          28 LOAD_GLOBAL              3 (NULL + handle_form)
+                      31          28 LOAD_GLOBAL              3 (NULL + handle_form)
                                   40 PRECALL                  0
                                   44 CALL                     0
                                   54 BUILD_TUPLE              1
-                                  56 LOAD_CONST               1 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 28>)
+                                  56 LOAD_CONST               1 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 30>)
                                   58 MAKE_FUNCTION            1 (defaults)
                      
-                      28          60 PRECALL                  0
+                      30          60 PRECALL                  0
                                   64 CALL                     0
                      
-                      29          74 STORE_FAST               0 (viewfn)
+                      31          74 STORE_FAST               0 (viewfn)
                                   76 LOAD_CONST               0 (None)
                                   78 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 2
                            nlocals   : 2
                            stacksize : 3
                            flags     : 19
                            code
                               0x97007401000000000000000000007c01a6010000ab0100000000000000
                               005300
-                            28           0 RESUME                   0
+                            30           0 RESUME                   0
                            
-                            30           2 LOAD_GLOBAL              1 (NULL + HttpResponse)
+                            32           2 LOAD_GLOBAL              1 (NULL + HttpResponse)
                                         14 LOAD_FAST                1 (form)
                                         16 PRECALL                  1
                                         20 CALL                     1
                                         30 RETURN_VALUE
                            consts
                               None
                            names      ('HttpResponse',)
                            varnames   ('_request', 'form')
                            freevars   ()
                            cellvars   ()
                            filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                            name       'viewfn'
-                           firstlineno 28
+                           firstlineno 30
                            lnotab 0x0202
-                     names      ('inject_args', 'handle_form')
+                     names      ('view', 'handle_form')
                      varnames   ('viewfn',)
                      freevars   ()
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                      name       'test'
-                     firstlineno 27
+                     firstlineno 29
                      lnotab 0x02011a0120ff0e01
                   'argument type for handle_form\\(\\) must be a subclass of django.forms.BaseForm'
                names      ('assertRaisesRegex', 'Exception')
                varnames   ('self', 'test')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                name       'test_error_missing_form_type'
-               firstlineno 26
+               firstlineno 28
                lnotab 0x0201060518010c01020102fd
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x9700640184007d017c00a0000000000000000000000000000000000000
                   00000074020000000000000000000064027c01a6030000ab030000000000
                   000000010064005300
-                38           0 RESUME                   0
+                40           0 RESUME                   0
                
-                39           2 LOAD_CONST               1 (<code object test, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 39>)
+                41           2 LOAD_CONST               1 (<code object test, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 41>)
                              4 MAKE_FUNCTION            0
                              6 STORE_FAST               1 (test)
                
-                44           8 LOAD_FAST                0 (self)
+                46           8 LOAD_FAST                0 (self)
                             10 LOAD_METHOD              0 (assertRaisesRegex)
                
-                45          32 LOAD_GLOBAL              2 (Exception)
+                47          32 LOAD_GLOBAL              2 (Exception)
                
-                46          44 LOAD_CONST               2 ('argument type for handle_form\\(\\) must be a subclass of django.forms.BaseForm')
+                48          44 LOAD_CONST               2 ('argument type for handle_form\\(\\) must be a subclass of django.forms.BaseForm')
                
-                47          46 LOAD_FAST                1 (test)
+                49          46 LOAD_FAST                1 (test)
                
-                44          48 PRECALL                  3
+                46          48 PRECALL                  3
                             52 CALL                     3
                             62 POP_TOP
                             64 LOAD_CONST               0 (None)
                             66 RETURN_VALUE
                consts
                   None
                   code
@@ -381,137 +400,135 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x9700740100000000000000000000a6000000ab00000000000000000074
                         0300000000000000000000a6000000ab0000000000000000006601640174
                         0400000000000000000000660264028405a6000000ab0000000000000000
                         007d0064005300
-                      39           0 RESUME                   0
+                      41           0 RESUME                   0
                      
-                      40           2 LOAD_GLOBAL              1 (NULL + inject_args)
+                      42           2 LOAD_GLOBAL              1 (NULL + view)
                                   14 PRECALL                  0
                                   18 CALL                     0
                      
-                      41          28 LOAD_GLOBAL              3 (NULL + handle_form)
+                      43          28 LOAD_GLOBAL              3 (NULL + handle_form)
                                   40 PRECALL                  0
                                   44 CALL                     0
                                   54 BUILD_TUPLE              1
                                   56 LOAD_CONST               1 ('_form')
                                   58 LOAD_GLOBAL              4 (str)
                                   70 BUILD_TUPLE              2
-                                  72 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 40>)
+                                  72 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 42>)
                                   74 MAKE_FUNCTION            5 (defaults, annotations)
                      
-                      40          76 PRECALL                  0
+                      42          76 PRECALL                  0
                                   80 CALL                     0
                      
-                      41          90 STORE_FAST               0 (viewfn)
+                      43          90 STORE_FAST               0 (viewfn)
                                   92 LOAD_CONST               0 (None)
                                   94 RETURN_VALUE
                      consts
                         None
                         '_form'
                         code
                            argcount  : 2
                            nlocals   : 2
                            stacksize : 3
                            flags     : 19
                            code
                               0x97007401000000000000000000006401a6010000ab0100000000000000
                               005300
-                            40           0 RESUME                   0
+                            42           0 RESUME                   0
                            
-                            42           2 LOAD_GLOBAL              1 (NULL + HttpResponse)
+                            44           2 LOAD_GLOBAL              1 (NULL + HttpResponse)
                                         14 LOAD_CONST               1 ('')
                                         16 PRECALL                  1
                                         20 CALL                     1
                                         30 RETURN_VALUE
                            consts
                               None
                               ''
                            names      ('HttpResponse',)
                            varnames   ('_request', '_form')
                            freevars   ()
                            cellvars   ()
                            filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                            name       'viewfn'
-                           firstlineno 40
+                           firstlineno 42
                            lnotab 0x0202
-                     names      ('inject_args', 'handle_form', 'str')
+                     names      ('view', 'handle_form', 'str')
                      varnames   ('viewfn',)
                      freevars   ()
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                      name       'test'
-                     firstlineno 39
+                     firstlineno 41
                      lnotab 0x02011a0130ff0e01
                   'argument type for handle_form\\(\\) must be a subclass of django.forms.BaseForm'
                names      ('assertRaisesRegex', 'Exception')
                varnames   ('self', 'test')
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                name       'test_error_wrong_form_type'
-               firstlineno 38
+               firstlineno 40
                lnotab 0x0201060518010c01020102fd
             code
                argcount  : 1
                nlocals   : 2
-               stacksize : 8
+               stacksize : 9
                flags     : 3
                code
                   0x87009700740100000000000000000000a6000000ab0000000000000000
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
-                  000000000000007d0102007c0189006a030000000000000000a004000000
-                  000000000000000000000000000000000064036404640564069c02a60200
-                  00ab020000000000000000a6010000ab0100000000000000000100640053
-                  00
+                  000000000000007d0102007c017407000000000000000000007c01640364
+                  04640564069c02a6030000ab030000000000000000a6010000ab01000000
+                  0000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-                50           2 RESUME                   0
+                52           2 RESUME                   0
                
-                51           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                53           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                52          30 LOAD_GLOBAL              3 (NULL + handle_form)
+                54          30 LOAD_GLOBAL              3 (NULL + handle_form)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('form')
                             60 LOAD_GLOBAL              4 (TestForm)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 51>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 53>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-                51          82 PRECALL                  0
+                53          82 PRECALL                  0
                             86 CALL                     0
                
-                52          96 STORE_FAST               1 (viewfn)
+                54          96 STORE_FAST               1 (viewfn)
                
-                56          98 PUSH_NULL
+                58          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
-                           102 LOAD_DEREF               0 (self)
-                           104 LOAD_ATTR                3 (factory)
-                           114 LOAD_METHOD              4 (post)
-                           136 LOAD_CONST               3 ('/')
-                           138 LOAD_CONST               4 ('a')
-                           140 LOAD_CONST               5 ('b')
-                           142 LOAD_CONST               6 (('p1', 'p2'))
-                           144 BUILD_CONST_KEY_MAP      2
-                           146 PRECALL                  2
-                           150 CALL                     2
-                           160 PRECALL                  1
-                           164 CALL                     1
-                           174 POP_TOP
-                           176 LOAD_CONST               0 (None)
-                           178 RETURN_VALUE
+                           102 LOAD_GLOBAL              7 (NULL + create_resolved_request)
+                           114 LOAD_FAST                1 (viewfn)
+                           116 LOAD_CONST               3 ('POST')
+                           118 LOAD_CONST               4 ('a')
+                           120 LOAD_CONST               5 ('b')
+                           122 LOAD_CONST               6 (('p1', 'p2'))
+                           124 BUILD_CONST_KEY_MAP      2
+                           126 PRECALL                  3
+                           130 CALL                     3
+                           140 PRECALL                  1
+                           144 CALL                     1
+                           154 POP_TOP
+                           156 LOAD_CONST               0 (None)
+                           158 RETURN_VALUE
                consts
                   None
                   'form'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 5
@@ -519,111 +536,112 @@
                      code
                         0x950197008902a000000000000000000000000000000000000000000074
                         03000000000000000000007c01a6010000ab010000000000000000740400
                         000000000000000000a6020000ab02000000000000000001007407000000
                         000000000000006401a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      51           2 RESUME                   0
+                      53           2 RESUME                   0
                      
-                      53           4 LOAD_DEREF               2 (self)
+                      55           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_GLOBAL              3 (NULL + type)
                                   40 LOAD_FAST                1 (form)
                                   42 PRECALL                  1
                                   46 CALL                     1
                                   56 LOAD_GLOBAL              4 (TestForm)
                                   68 PRECALL                  2
                                   72 CALL                     2
                                   82 POP_TOP
                      
-                      54          84 LOAD_GLOBAL              7 (NULL + HttpResponse)
+                      56          84 LOAD_GLOBAL              7 (NULL + HttpResponse)
                                   96 LOAD_CONST               1 ('')
                                   98 PRECALL                  1
                                  102 CALL                     1
                                  112 RETURN_VALUE
                      consts
                         None
                         ''
                      names      ('assertEqual', 'type', 'TestForm', 'HttpResponse')
                      varnames   ('_request', 'form')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                      name       'viewfn'
-                     firstlineno 51
+                     firstlineno 53
                      lnotab 0x04025001
-                  '/'
+                  'POST'
                   'a'
                   'b'
                   ('p1', 'p2')
-               names      ('inject_args', 'handle_form', 'TestForm', 'factory', 'post')
+               names      ('view', 'handle_form', 'TestForm', 'create_resolved_request')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                name       'test_form_explicit'
-               firstlineno 50
+               firstlineno 52
                lnotab 0x04011a0134ff0e010204
             code
                argcount  : 1
                nlocals   : 2
-               stacksize : 8
+               stacksize : 9
                flags     : 3
                code
                   0x87009700740100000000000000000000a6000000ab0000000000000000
                   0064017402000000000000000000006602880066016402840ca6000000ab
                   0000000000000000007d0102007405000000000000000000006a03000000
                   00000000007408000000000000000000007c01a6020000ab020000000000
-                  00000089006a050000000000000000a00600000000000000000000000000
-                  0000000000000064036404640564069c02a6020000ab0200000000000000
-                  00a6010000ab010000000000000000010064005300
+                  000000740b000000000000000000007c0164036404640564069c02a60300
+                  00ab030000000000000000a6010000ab0100000000000000000100640053
+                  00
                              0 MAKE_CELL                0 (self)
                
-                58           2 RESUME                   0
+                60           2 RESUME                   0
                
-                59           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                61           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                60          30 LOAD_CONST               1 ('form')
+                62          30 LOAD_CONST               1 ('form')
                             32 LOAD_GLOBAL              2 (TestForm)
                             44 BUILD_TUPLE              2
                             46 LOAD_CLOSURE             0 (self)
                             48 BUILD_TUPLE              1
-                            50 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 59>)
+                            50 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 61>)
                             52 MAKE_FUNCTION           12 (annotations, closure)
                
-                59          54 PRECALL                  0
+                61          54 PRECALL                  0
                             58 CALL                     0
                
-                60          68 STORE_FAST               1 (viewfn)
+                62          68 STORE_FAST               1 (viewfn)
                
-                64          70 PUSH_NULL
+                66          70 PUSH_NULL
                             72 LOAD_GLOBAL              5 (NULL + typing)
                             84 LOAD_ATTR                3 (cast)
                             94 LOAD_GLOBAL              8 (Any)
                            106 LOAD_FAST                1 (viewfn)
                            108 PRECALL                  2
                            112 CALL                     2
-                           122 LOAD_DEREF               0 (self)
-                           124 LOAD_ATTR                5 (factory)
-                           134 LOAD_METHOD              6 (post)
-                           156 LOAD_CONST               3 ('/')
-                           158 LOAD_CONST               4 ('a')
-                           160 LOAD_CONST               5 ('b')
-                           162 LOAD_CONST               6 (('p1', 'p2'))
-                           164 BUILD_CONST_KEY_MAP      2
-                           166 PRECALL                  2
-                           170 CALL                     2
-                           180 PRECALL                  1
-                           184 CALL                     1
-                           194 POP_TOP
-                           196 LOAD_CONST               0 (None)
-                           198 RETURN_VALUE
+               
+                67         122 LOAD_GLOBAL             11 (NULL + create_resolved_request)
+                           134 LOAD_FAST                1 (viewfn)
+                           136 LOAD_CONST               3 ('POST')
+                           138 LOAD_CONST               4 ('a')
+                           140 LOAD_CONST               5 ('b')
+                           142 LOAD_CONST               6 (('p1', 'p2'))
+                           144 BUILD_CONST_KEY_MAP      2
+                           146 PRECALL                  3
+                           150 CALL                     3
+               
+                66         160 PRECALL                  1
+                           164 CALL                     1
+                           174 POP_TOP
+                           176 LOAD_CONST               0 (None)
+                           178 RETURN_VALUE
                consts
                   None
                   'form'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 5
@@ -631,105 +649,108 @@
                      code
                         0x950197008902a000000000000000000000000000000000000000000074
                         03000000000000000000007c01a6010000ab010000000000000000740400
                         000000000000000000a6020000ab02000000000000000001007407000000
                         000000000000006401a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      59           2 RESUME                   0
+                      61           2 RESUME                   0
                      
-                      61           4 LOAD_DEREF               2 (self)
+                      63           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_GLOBAL              3 (NULL + type)
                                   40 LOAD_FAST                1 (form)
                                   42 PRECALL                  1
                                   46 CALL                     1
                                   56 LOAD_GLOBAL              4 (TestForm)
                                   68 PRECALL                  2
                                   72 CALL                     2
                                   82 POP_TOP
                      
-                      62          84 LOAD_GLOBAL              7 (NULL + HttpResponse)
+                      64          84 LOAD_GLOBAL              7 (NULL + HttpResponse)
                                   96 LOAD_CONST               1 ('')
                                   98 PRECALL                  1
                                  102 CALL                     1
                                  112 RETURN_VALUE
                      consts
                         None
                         ''
                      names      ('assertEqual', 'type', 'TestForm', 'HttpResponse')
                      varnames   ('_request', 'form')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                      name       'viewfn'
-                     firstlineno 59
+                     firstlineno 61
                      lnotab 0x04025001
-                  '/'
+                  'POST'
                   'a'
                   'b'
                   ('p1', 'p2')
-               names      ('inject_args', 'TestForm', 'typing', 'cast', 'Any', 'factory', 'post')
+               names      ('view', 'TestForm', 'typing', 'cast', 'Any', 'create_resolved_request')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                name       'test_form_implicit'
-               firstlineno 58
-               lnotab 0x04011a0118ff0e010204
+               firstlineno 60
+               lnotab 0x04011a0118ff0e010204340126ff
             code
                argcount  : 1
                nlocals   : 2
-               stacksize : 5
+               stacksize : 9
                flags     : 3
                code
                   0x87009700740100000000000000000000a6000000ab0000000000000000
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
-                  000000000000007d0102007c0189006a030000000000000000a004000000
-                  00000000000000000000000000000000006403a6010000ab010000000000
-                  000000a6010000ab010000000000000000010064005300
+                  000000000000007d0102007c017407000000000000000000007c01640364
+                  04640564069c02a6030000ab030000000000000000a6010000ab01000000
+                  0000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-                66           2 RESUME                   0
+                70           2 RESUME                   0
                
-                67           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                71           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                68          30 LOAD_GLOBAL              3 (NULL + handle_form)
+                72          30 LOAD_GLOBAL              3 (NULL + handle_form)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('form')
                             60 LOAD_GLOBAL              4 (TestForm)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 67>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 71>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-                67          82 PRECALL                  0
+                71          82 PRECALL                  0
                             86 CALL                     0
                
-                68          96 STORE_FAST               1 (viewfn)
+                72          96 STORE_FAST               1 (viewfn)
                
-                73          98 PUSH_NULL
+                77          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
-                           102 LOAD_DEREF               0 (self)
-                           104 LOAD_ATTR                3 (factory)
-                           114 LOAD_METHOD              4 (get)
-                           136 LOAD_CONST               3 ('/')
-                           138 PRECALL                  1
-                           142 CALL                     1
-                           152 PRECALL                  1
-                           156 CALL                     1
-                           166 POP_TOP
-                           168 LOAD_CONST               0 (None)
-                           170 RETURN_VALUE
+                           102 LOAD_GLOBAL              7 (NULL + create_resolved_request)
+                           114 LOAD_FAST                1 (viewfn)
+                           116 LOAD_CONST               3 ('GET')
+                           118 LOAD_CONST               4 ('a')
+                           120 LOAD_CONST               5 ('b')
+                           122 LOAD_CONST               6 (('p1', 'p2'))
+                           124 BUILD_CONST_KEY_MAP      2
+                           126 PRECALL                  3
+                           130 CALL                     3
+                           140 PRECALL                  1
+                           144 CALL                     1
+                           154 POP_TOP
+                           156 LOAD_CONST               0 (None)
+                           158 RETURN_VALUE
                consts
                   None
                   'form'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
@@ -739,114 +760,115 @@
                         016a010000000000000000a6010000ab01000000000000000001008902a0
                         0000000000000000000000000000000000000000007c01a0020000000000
                         000000000000000000000000000000a6000000ab000000000000000000a6
                         010000ab01000000000000000001007407000000000000000000006401a6
                         010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      67           2 RESUME                   0
+                      71           2 RESUME                   0
                      
-                      69           4 LOAD_DEREF               2 (self)
+                      73           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertFalse)
                                   28 LOAD_FAST                1 (form)
                                   30 LOAD_ATTR                1 (is_bound)
                                   40 PRECALL                  1
                                   44 CALL                     1
                                   54 POP_TOP
                      
-                      70          56 LOAD_DEREF               2 (self)
+                      74          56 LOAD_DEREF               2 (self)
                                   58 LOAD_METHOD              0 (assertFalse)
                                   80 LOAD_FAST                1 (form)
                                   82 LOAD_METHOD              2 (is_valid)
                                  104 PRECALL                  0
                                  108 CALL                     0
                                  118 PRECALL                  1
                                  122 CALL                     1
                                  132 POP_TOP
                      
-                      71         134 LOAD_GLOBAL              7 (NULL + HttpResponse)
+                      75         134 LOAD_GLOBAL              7 (NULL + HttpResponse)
                                  146 LOAD_CONST               1 ('')
                                  148 PRECALL                  1
                                  152 CALL                     1
                                  162 RETURN_VALUE
                      consts
                         None
                         ''
                      names      ('assertFalse', 'is_bound', 'is_valid', 'HttpResponse')
                      varnames   ('_request', 'form')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                      name       'viewfn'
-                     firstlineno 67
+                     firstlineno 71
                      lnotab 0x040234014e01
-                  '/'
-               names      ('inject_args', 'handle_form', 'TestForm', 'factory', 'get')
+                  'GET'
+                  'a'
+                  'b'
+                  ('p1', 'p2')
+               names      ('view', 'handle_form', 'TestForm', 'create_resolved_request')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                name       'test_form_get'
-               firstlineno 66
+               firstlineno 70
                lnotab 0x04011a0134ff0e010205
             code
                argcount  : 1
                nlocals   : 2
-               stacksize : 8
+               stacksize : 9
                flags     : 3
                code
                   0x87009700740100000000000000000000a6000000ab0000000000000000
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
-                  000000000000007d0102007c0189006a030000000000000000a004000000
-                  000000000000000000000000000000000064036404640564069c02a60200
-                  00ab020000000000000000a6010000ab0100000000000000000100640053
-                  00
+                  000000000000007d0102007c017407000000000000000000007c01640364
+                  04640564069c02a6030000ab030000000000000000a6010000ab01000000
+                  0000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-                75           2 RESUME                   0
+                79           2 RESUME                   0
                
-                76           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                80           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                77          30 LOAD_GLOBAL              3 (NULL + handle_form)
+                81          30 LOAD_GLOBAL              3 (NULL + handle_form)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('form')
                             60 LOAD_GLOBAL              4 (TestForm)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 76>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 80>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-                76          82 PRECALL                  0
+                80          82 PRECALL                  0
                             86 CALL                     0
                
-                77          96 STORE_FAST               1 (viewfn)
+                81          96 STORE_FAST               1 (viewfn)
                
-                84          98 PUSH_NULL
+                88          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
-                           102 LOAD_DEREF               0 (self)
-                           104 LOAD_ATTR                3 (factory)
-                           114 LOAD_METHOD              4 (post)
-                           136 LOAD_CONST               3 ('/')
-                           138 LOAD_CONST               4 ('a')
-                           140 LOAD_CONST               5 ('b')
-                           142 LOAD_CONST               6 (('p1', 'p2'))
-                           144 BUILD_CONST_KEY_MAP      2
-                           146 PRECALL                  2
-                           150 CALL                     2
-                           160 PRECALL                  1
-                           164 CALL                     1
-                           174 POP_TOP
-                           176 LOAD_CONST               0 (None)
-                           178 RETURN_VALUE
+                           102 LOAD_GLOBAL              7 (NULL + create_resolved_request)
+                           114 LOAD_FAST                1 (viewfn)
+                           116 LOAD_CONST               3 ('POST')
+                           118 LOAD_CONST               4 ('a')
+                           120 LOAD_CONST               5 ('b')
+                           122 LOAD_CONST               6 (('p1', 'p2'))
+                           124 BUILD_CONST_KEY_MAP      2
+                           126 PRECALL                  3
+                           130 CALL                     3
+                           140 PRECALL                  1
+                           144 CALL                     1
+                           154 POP_TOP
+                           156 LOAD_CONST               0 (None)
+                           158 RETURN_VALUE
                consts
                   None
                   'form'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
@@ -860,57 +882,57 @@
                         0000000000000000007c016a040000000000000000640119000000000000
                         0000006402a6020000ab02000000000000000001008902a0030000000000
                         0000000000000000000000000000007c016a040000000000000000640319
                         0000000000000000006404a6020000ab0200000000000000000100740b00
                         0000000000000000006405a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      76           2 RESUME                   0
+                      80           2 RESUME                   0
                      
-                      78           4 LOAD_DEREF               2 (self)
+                      82           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertTrue)
                                   28 LOAD_FAST                1 (form)
                                   30 LOAD_ATTR                1 (is_bound)
                                   40 PRECALL                  1
                                   44 CALL                     1
                                   54 POP_TOP
                      
-                      79          56 LOAD_DEREF               2 (self)
+                      83          56 LOAD_DEREF               2 (self)
                                   58 LOAD_METHOD              0 (assertTrue)
                                   80 LOAD_FAST                1 (form)
                                   82 LOAD_METHOD              2 (is_valid)
                                  104 PRECALL                  0
                                  108 CALL                     0
                                  118 PRECALL                  1
                                  122 CALL                     1
                                  132 POP_TOP
                      
-                      80         134 LOAD_DEREF               2 (self)
+                      84         134 LOAD_DEREF               2 (self)
                                  136 LOAD_METHOD              3 (assertEqual)
                                  158 LOAD_FAST                1 (form)
                                  160 LOAD_ATTR                4 (cleaned_data)
                                  170 LOAD_CONST               1 ('p1')
                                  172 BINARY_SUBSCR
                                  182 LOAD_CONST               2 ('a')
                                  184 PRECALL                  2
                                  188 CALL                     2
                                  198 POP_TOP
                      
-                      81         200 LOAD_DEREF               2 (self)
+                      85         200 LOAD_DEREF               2 (self)
                                  202 LOAD_METHOD              3 (assertEqual)
                                  224 LOAD_FAST                1 (form)
                                  226 LOAD_ATTR                4 (cleaned_data)
                                  236 LOAD_CONST               3 ('p2')
                                  238 BINARY_SUBSCR
                                  248 LOAD_CONST               4 ('b')
                                  250 PRECALL                  2
                                  254 CALL                     2
                                  264 POP_TOP
                      
-                      82         266 LOAD_GLOBAL             11 (NULL + HttpResponse)
+                      86         266 LOAD_GLOBAL             11 (NULL + HttpResponse)
                                  278 LOAD_CONST               5 ('')
                                  280 PRECALL                  1
                                  284 CALL                     1
                                  294 RETURN_VALUE
                      consts
                         None
                         'p1'
@@ -920,185 +942,210 @@
                         ''
                      names      ('assertTrue', 'is_bound', 'is_valid', 'assertEqual', 'cleaned_data', 'HttpResponse')
                      varnames   ('_request', 'form')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                      name       'viewfn'
-                     firstlineno 76
+                     firstlineno 80
                      lnotab 0x040234014e0142014201
-                  '/'
+                  'POST'
                   'a'
                   'b'
                   ('p1', 'p2')
-               names      ('inject_args', 'handle_form', 'TestForm', 'factory', 'post')
+               names      ('view', 'handle_form', 'TestForm', 'create_resolved_request')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                name       'test_form_post'
-               firstlineno 75
+               firstlineno 79
                lnotab 0x04011a0134ff0e010207
             code
                argcount  : 1
-               nlocals   : 7
+               nlocals   : 9
                stacksize : 8
                flags     : 3
                code
                   0x87009700740100000000000000000000a6000000ab0000000000000000
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
-                  000000000000007d0189006a030000000000000000a00400000000000000
-                  000000000000000000000000006403740b000000000000000000006a0600
-                  000000000000006404640564069c02a6010000ab01000000000000000064
-                  07640864096901ac0aa6040000ab0400000000000000007d0202007c017c
-                  02a6010000ab0100000000000000007d038900a007000000000000000000
-                  00000000000000000000007c036a080000000000000000640ba6020000ab
-                  02000000000000000001008900a007000000000000000000000000000000
-                  00000000007c03640c190000000000000000006407a6020000ab02000000
-                  00000000000100740b000000000000000000006a0900000000000000007c
-                  036a0a0000000000000000a6010000ab0100000000000000007d048900a0
-                  0700000000000000000000000000000000000000007c04640d1900000000
-                  00000000006409a6020000ab02000000000000000001007c04640e190000
-                  000000000000006409190000000000000000007d058900a0070000000000
-                  0000000000000000000000000000007c05640f1900000000000000000064
-                  10a6020000ab02000000000000000001007c04640e190000000000000000
-                  006411190000000000000000007d068900a0070000000000000000000000
-                  0000000000000000007c06640f190000000000000000006412a6020000ab
-                  020000000000000000010064005300
+                  000000000000007d0174070000000000000000000064037c016404ac05a6
+                  030000ab03000000000000000066017d0274090000000000000000000064
+                  067c02ac07a6020000ab0200000000000000007d0389006a050000000000
+                  000000a00600000000000000000000000000000000000000006408740f00
+                  0000000000000000006a0800000000000000006409640a640b9c02a60100
+                  00ab010000000000000000640c640d640e6901ac0fa6040000ab04000000
+                  00000000007d047c037c045f09000000000000000002007c017c04a60100
+                  00ab0100000000000000007d058900a00a00000000000000000000000000
+                  000000000000007c056a0b00000000000000006410a6020000ab02000000
+                  000000000001008900a00a00000000000000000000000000000000000000
+                  007c05641119000000000000000000640ca6020000ab0200000000000000
+                  000100740f000000000000000000006a0c00000000000000007c056a0d00
+                  00000000000000a6010000ab0100000000000000007d068900a00a000000
+                  00000000000000000000000000000000007c066412190000000000000000
+                  00640ea6020000ab02000000000000000001007c06641319000000000000
+                  000000640e190000000000000000007d078900a00a000000000000000000
+                  00000000000000000000007c076414190000000000000000006415a60200
+                  00ab02000000000000000001007c06641319000000000000000000641619
+                  0000000000000000007d088900a00a000000000000000000000000000000
+                  00000000007c086414190000000000000000006417a6020000ab02000000
+                  0000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-                86           2 RESUME                   0
+                90           2 RESUME                   0
                
-                87           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                91           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                88          30 LOAD_GLOBAL              3 (NULL + handle_form)
+                92          30 LOAD_GLOBAL              3 (NULL + handle_form)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('form')
                             60 LOAD_GLOBAL              4 (TestForm)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 87>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_form.py", line 91>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-                87          82 PRECALL                  0
+                91          82 PRECALL                  0
                             86 CALL                     0
                
-                88          96 STORE_FAST               1 (viewfn)
+                92          96 STORE_FAST               1 (viewfn)
                
-                93          98 LOAD_DEREF               0 (self)
-                           100 LOAD_ATTR                3 (factory)
-                           110 LOAD_METHOD              4 (patch)
-               
-                94         132 LOAD_CONST               3 ('/')
-               
-                95         134 LOAD_GLOBAL             11 (NULL + json)
-                           146 LOAD_ATTR                6 (dumps)
-                           156 LOAD_CONST               4 ('')
-                           158 LOAD_CONST               5 ('b')
-                           160 LOAD_CONST               6 (('p1', 'p2'))
-                           162 BUILD_CONST_KEY_MAP      2
-                           164 PRECALL                  1
-                           168 CALL                     1
-               
-                96         178 LOAD_CONST               7 ('application/json')
-               
-                97         180 LOAD_CONST               8 ('X-DFV-Validate-Field')
-                           182 LOAD_CONST               9 ('p1')
-                           184 BUILD_MAP                1
-               
-                93         186 KW_NAMES                10
-                           188 PRECALL                  4
-                           192 CALL                     4
-                           202 STORE_FAST               2 (request)
-               
-                99         204 PUSH_NULL
-                           206 LOAD_FAST                1 (viewfn)
-                           208 LOAD_FAST                2 (request)
-                           210 PRECALL                  1
-                           214 CALL                     1
-                           224 STORE_FAST               3 (response)
-               
-               100         226 LOAD_DEREF               0 (self)
-                           228 LOAD_METHOD              7 (assertEqual)
-                           250 LOAD_FAST                3 (response)
-                           252 LOAD_ATTR                8 (status_code)
-                           262 LOAD_CONST              11 (200)
-                           264 PRECALL                  2
-                           268 CALL                     2
-                           278 POP_TOP
-               
-               101         280 LOAD_DEREF               0 (self)
-                           282 LOAD_METHOD              7 (assertEqual)
-                           304 LOAD_FAST                3 (response)
-                           306 LOAD_CONST              12 ('Content-Type')
-                           308 BINARY_SUBSCR
-                           318 LOAD_CONST               7 ('application/json')
-                           320 PRECALL                  2
-                           324 CALL                     2
-                           334 POP_TOP
-               
-               102         336 LOAD_GLOBAL             11 (NULL + json)
-                           348 LOAD_ATTR                9 (loads)
-                           358 LOAD_FAST                3 (response)
-                           360 LOAD_ATTR               10 (content)
-                           370 PRECALL                  1
-                           374 CALL                     1
-                           384 STORE_FAST               4 (body)
-               
-               103         386 LOAD_DEREF               0 (self)
-                           388 LOAD_METHOD              7 (assertEqual)
-                           410 LOAD_FAST                4 (body)
-                           412 LOAD_CONST              13 ('name')
-                           414 BINARY_SUBSCR
-                           424 LOAD_CONST               9 ('p1')
-                           426 PRECALL                  2
-                           430 CALL                     2
-                           440 POP_TOP
-               
-               104         442 LOAD_FAST                4 (body)
-                           444 LOAD_CONST              14 ('fields')
-                           446 BINARY_SUBSCR
-                           456 LOAD_CONST               9 ('p1')
-                           458 BINARY_SUBSCR
-                           468 STORE_FAST               5 (field_p1)
-               
-               105         470 LOAD_DEREF               0 (self)
-                           472 LOAD_METHOD              7 (assertEqual)
-                           494 LOAD_FAST                5 (field_p1)
-                           496 LOAD_CONST              15 ('valid')
-                           498 BINARY_SUBSCR
-                           508 LOAD_CONST              16 (False)
-                           510 PRECALL                  2
-                           514 CALL                     2
-                           524 POP_TOP
-               
-               106         526 LOAD_FAST                4 (body)
-                           528 LOAD_CONST              14 ('fields')
-                           530 BINARY_SUBSCR
-                           540 LOAD_CONST              17 ('p2')
-                           542 BINARY_SUBSCR
-                           552 STORE_FAST               6 (field_p2)
-               
-               107         554 LOAD_DEREF               0 (self)
-                           556 LOAD_METHOD              7 (assertEqual)
-                           578 LOAD_FAST                6 (field_p2)
-                           580 LOAD_CONST              15 ('valid')
-                           582 BINARY_SUBSCR
-                           592 LOAD_CONST              18 (True)
-                           594 PRECALL                  2
-                           598 CALL                     2
-                           608 POP_TOP
-                           610 LOAD_CONST               0 (None)
-                           612 RETURN_VALUE
+                97          98 LOAD_GLOBAL              7 (NULL + path)
+                           110 LOAD_CONST               3 ('view/')
+                           112 LOAD_FAST                1 (viewfn)
+                           114 LOAD_CONST               4 ('a view')
+                           116 KW_NAMES                 5
+                           118 PRECALL                  3
+                           122 CALL                     3
+                           132 BUILD_TUPLE              1
+                           134 STORE_FAST               2 (urlpatterns)
+               
+                98         136 LOAD_GLOBAL              9 (NULL + resolve)
+                           148 LOAD_CONST               6 ('/view/')
+                           150 LOAD_FAST                2 (urlpatterns)
+                           152 KW_NAMES                 7
+                           154 PRECALL                  2
+                           158 CALL                     2
+                           168 STORE_FAST               3 (resolved)
+               
+                99         170 LOAD_DEREF               0 (self)
+                           172 LOAD_ATTR                5 (factory)
+                           182 LOAD_METHOD              6 (patch)
+               
+               100         204 LOAD_CONST               8 ('/')
+               
+               101         206 LOAD_GLOBAL             15 (NULL + json)
+                           218 LOAD_ATTR                8 (dumps)
+                           228 LOAD_CONST               9 ('')
+                           230 LOAD_CONST              10 ('b')
+                           232 LOAD_CONST              11 (('p1', 'p2'))
+                           234 BUILD_CONST_KEY_MAP      2
+                           236 PRECALL                  1
+                           240 CALL                     1
+               
+               102         250 LOAD_CONST              12 ('application/json')
+               
+               103         252 LOAD_CONST              13 ('X-DFV-Validate-Field')
+                           254 LOAD_CONST              14 ('p1')
+                           256 BUILD_MAP                1
+               
+                99         258 KW_NAMES                15
+                           260 PRECALL                  4
+                           264 CALL                     4
+                           274 STORE_FAST               4 (request)
+               
+               105         276 LOAD_FAST                3 (resolved)
+                           278 LOAD_FAST                4 (request)
+                           280 STORE_ATTR               9 (resolver_match)
+               
+               107         290 PUSH_NULL
+                           292 LOAD_FAST                1 (viewfn)
+                           294 LOAD_FAST                4 (request)
+                           296 PRECALL                  1
+                           300 CALL                     1
+                           310 STORE_FAST               5 (response)
+               
+               108         312 LOAD_DEREF               0 (self)
+                           314 LOAD_METHOD             10 (assertEqual)
+                           336 LOAD_FAST                5 (response)
+                           338 LOAD_ATTR               11 (status_code)
+                           348 LOAD_CONST              16 (200)
+                           350 PRECALL                  2
+                           354 CALL                     2
+                           364 POP_TOP
+               
+               109         366 LOAD_DEREF               0 (self)
+                           368 LOAD_METHOD             10 (assertEqual)
+                           390 LOAD_FAST                5 (response)
+                           392 LOAD_CONST              17 ('Content-Type')
+                           394 BINARY_SUBSCR
+                           404 LOAD_CONST              12 ('application/json')
+                           406 PRECALL                  2
+                           410 CALL                     2
+                           420 POP_TOP
+               
+               110         422 LOAD_GLOBAL             15 (NULL + json)
+                           434 LOAD_ATTR               12 (loads)
+                           444 LOAD_FAST                5 (response)
+                           446 LOAD_ATTR               13 (content)
+                           456 PRECALL                  1
+                           460 CALL                     1
+                           470 STORE_FAST               6 (body)
+               
+               111         472 LOAD_DEREF               0 (self)
+                           474 LOAD_METHOD             10 (assertEqual)
+                           496 LOAD_FAST                6 (body)
+                           498 LOAD_CONST              18 ('name')
+                           500 BINARY_SUBSCR
+                           510 LOAD_CONST              14 ('p1')
+                           512 PRECALL                  2
+                           516 CALL                     2
+                           526 POP_TOP
+               
+               112         528 LOAD_FAST                6 (body)
+                           530 LOAD_CONST              19 ('fields')
+                           532 BINARY_SUBSCR
+                           542 LOAD_CONST              14 ('p1')
+                           544 BINARY_SUBSCR
+                           554 STORE_FAST               7 (field_p1)
+               
+               113         556 LOAD_DEREF               0 (self)
+                           558 LOAD_METHOD             10 (assertEqual)
+                           580 LOAD_FAST                7 (field_p1)
+                           582 LOAD_CONST              20 ('valid')
+                           584 BINARY_SUBSCR
+                           594 LOAD_CONST              21 (False)
+                           596 PRECALL                  2
+                           600 CALL                     2
+                           610 POP_TOP
+               
+               114         612 LOAD_FAST                6 (body)
+                           614 LOAD_CONST              19 ('fields')
+                           616 BINARY_SUBSCR
+                           626 LOAD_CONST              22 ('p2')
+                           628 BINARY_SUBSCR
+                           638 STORE_FAST               8 (field_p2)
+               
+               115         640 LOAD_DEREF               0 (self)
+                           642 LOAD_METHOD             10 (assertEqual)
+                           664 LOAD_FAST                8 (field_p2)
+                           666 LOAD_CONST              20 ('valid')
+                           668 BINARY_SUBSCR
+                           678 LOAD_CONST              23 (True)
+                           680 PRECALL                  2
+                           684 CALL                     2
+                           694 POP_TOP
+                           696 LOAD_CONST               0 (None)
+                           698 RETURN_VALUE
                consts
                   None
                   'form'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
@@ -1108,50 +1155,55 @@
                         016a010000000000000000a6010000ab01000000000000000001008902a0
                         0200000000000000000000000000000000000000007c01a0030000000000
                         000000000000000000000000000000a6000000ab000000000000000000a6
                         010000ab01000000000000000001007409000000000000000000006401a6
                         010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      87           2 RESUME                   0
+                      91           2 RESUME                   0
                      
-                      89           4 LOAD_DEREF               2 (self)
+                      93           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertTrue)
                                   28 LOAD_FAST                1 (form)
                                   30 LOAD_ATTR                1 (is_bound)
                                   40 PRECALL                  1
                                   44 CALL                     1
                                   54 POP_TOP
                      
-                      90          56 LOAD_DEREF               2 (self)
+                      94          56 LOAD_DEREF               2 (self)
                                   58 LOAD_METHOD              2 (assertFalse)
                                   80 LOAD_FAST                1 (form)
                                   82 LOAD_METHOD              3 (is_valid)
                                  104 PRECALL                  0
                                  108 CALL                     0
                                  118 PRECALL                  1
                                  122 CALL                     1
                                  132 POP_TOP
                      
-                      91         134 LOAD_GLOBAL              9 (NULL + HttpResponse)
+                      95         134 LOAD_GLOBAL              9 (NULL + HttpResponse)
                                  146 LOAD_CONST               1 ('')
                                  148 PRECALL                  1
                                  152 CALL                     1
                                  162 RETURN_VALUE
                      consts
                         None
                         ''
                      names      ('assertTrue', 'is_bound', 'assertFalse', 'is_valid', 'HttpResponse')
                      varnames   ('_request', 'form')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                      name       'viewfn'
-                     firstlineno 87
+                     firstlineno 91
                      lnotab 0x040234014e01
+                  'view/'
+                  'a view'
+                  ('name',)
+                  '/view/'
+                  ('urlconf',)
                   '/'
                   ''
                   'b'
                   ('p1', 'p2')
                   'application/json'
                   'X-DFV-Validate-Field'
                   'p1'
@@ -1160,35 +1212,35 @@
                   'Content-Type'
                   'name'
                   'fields'
                   'valid'
                   False
                   'p2'
                   True
-               names      ('inject_args', 'handle_form', 'TestForm', 'factory', 'patch', 'json', 'dumps', 'assertEqual', 'status_code', 'loads', 'content')
-               varnames   ('self', 'viewfn', 'request', 'response', 'body', 'field_p1', 'field_p2')
+               names      ('view', 'handle_form', 'TestForm', 'path', 'resolve', 'factory', 'patch', 'json', 'dumps', 'resolver_match', 'assertEqual', 'status_code', 'loads', 'content')
+               varnames   ('self', 'viewfn', 'urlpatterns', 'resolved', 'request', 'response', 'body', 'field_p1', 'field_p2')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
                name       'test_form_patch'
-               firstlineno 86
+               firstlineno 90
                lnotab
-                  0x04011a0134ff0e010205220102012c01020106fc120616013601380132
-                  0138011c0138011c01
+                  0x04011a0134ff0e01020526012201220102012c01020106fc12060e0216
+                  0136013801320138011c0138011c01
             ('return', None)
          names      ('__name__', '__module__', '__qualname__', 'RequestFactory', '__annotations__', 'setUp', 'test_error_missing_form_type', 'test_error_wrong_form_type', 'test_form_explicit', 'test_form_implicit', 'test_form_get', 'test_form_post', 'test_form_patch')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
          name       'ParamsToArgsDecoratorTestCase'
-         firstlineno 19
-         lnotab 0x0c010a020804060c060c060806080609060b
+         firstlineno 21
+         lnotab 0x0c010a020804060c060c0608060a0609060b
       'ParamsToArgsDecoratorTestCase'
-   names      ('json', 'typing', 'Any', 'unittest', 'TestCase', 'django', 'forms', 'django.http', 'HttpResponse', 'django.test', 'RequestFactory', 'dfv', 'inject_args', 'handle_form', 'Form', 'TestForm', 'ParamsToArgsDecoratorTestCase')
+   names      ('json', 'typing', 'Any', 'unittest', 'TestCase', 'django', 'forms', 'django.http', 'HttpResponse', 'django.test', 'RequestFactory', 'django.urls', 'path', 'resolve', 'dfv', 'handle_form', 'view', 'dfv.testutils', 'create_resolved_request', 'Form', 'TestForm', 'ParamsToArgsDecoratorTestCase')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/roman/prjs/python/dfv/dfv/test_form.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010c010c02080108010c010c010c0210032605
+   lnotab 0x00ff0201080108010c010c0208010c010c010c01100210010c032605
```

### Comparing `dfv-0.8.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc` & `dfv-0.9.0/dfv/__pycache__/test_params_to_args.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0x35c1c464 (Sat Jul 29 07:35:17 2023 UTC)
-files sz: 8657
+moddate:  0x730acc64 (Thu Aug  3 20:13:39 2023 UTC)
+files sz: 8583
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c006d015a016d025a020100640064
       036c036d045a040100640064016c055a05640064046c056d065a06010064
       0064056c076d085a080100640064066c096d0a5a0a0100640064076c0b6d
-      0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f0100020047006408840064096504a6
-      030000ab0300000000000000005a1064015300
+      0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a100100640064086c116d125a
+      1201000200470064098400640a6504a6030000ab0300000000000000005a
+      1364015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (typing)
                  8 STORE_NAME               0 (typing)
    
@@ -58,185 +59,195 @@
                 72 LOAD_CONST               6 (('RequestFactory',))
                 74 IMPORT_NAME              9 (django.test)
                 76 IMPORT_FROM             10 (RequestFactory)
                 78 STORE_NAME              10 (RequestFactory)
                 80 POP_TOP
    
     10          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               7 (('inject_args', 'param', 'param_get', 'param_post'))
+                84 LOAD_CONST               7 (('inject_args', 'param', 'param_get', 'param_post', 'view'))
                 86 IMPORT_NAME             11 (dfv)
                 88 IMPORT_FROM             12 (inject_args)
                 90 STORE_NAME              12 (inject_args)
                 92 IMPORT_FROM             13 (param)
                 94 STORE_NAME              13 (param)
                 96 IMPORT_FROM             14 (param_get)
                 98 STORE_NAME              14 (param_get)
                100 IMPORT_FROM             15 (param_post)
                102 STORE_NAME              15 (param_post)
-               104 POP_TOP
+               104 IMPORT_FROM             16 (view)
+               106 STORE_NAME              16 (view)
+               108 POP_TOP
    
-    13         106 PUSH_NULL
-               108 LOAD_BUILD_CLASS
-               110 LOAD_CONST               8 (<code object ParamsToArgsDecoratorTestCase, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 13>)
-               112 MAKE_FUNCTION            0
-               114 LOAD_CONST               9 ('ParamsToArgsDecoratorTestCase')
-               116 LOAD_NAME                4 (TestCase)
-               118 PRECALL                  3
-               122 CALL                     3
-               132 STORE_NAME              16 (ParamsToArgsDecoratorTestCase)
-               134 LOAD_CONST               1 (None)
-               136 RETURN_VALUE
+    11         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               8 (('create_resolved_request',))
+               114 IMPORT_NAME             17 (dfv.testutils)
+               116 IMPORT_FROM             18 (create_resolved_request)
+               118 STORE_NAME              18 (create_resolved_request)
+               120 POP_TOP
+   
+    14         122 PUSH_NULL
+               124 LOAD_BUILD_CLASS
+               126 LOAD_CONST               9 (<code object ParamsToArgsDecoratorTestCase, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 14>)
+               128 MAKE_FUNCTION            0
+               130 LOAD_CONST              10 ('ParamsToArgsDecoratorTestCase')
+               132 LOAD_NAME                4 (TestCase)
+               134 PRECALL                  3
+               138 CALL                     3
+               148 STORE_NAME              19 (ParamsToArgsDecoratorTestCase)
+               150 LOAD_CONST               1 (None)
+               152 RETURN_VALUE
    consts
       0
       None
       ('Any', 'Optional')
       ('TestCase',)
       ('forms',)
       ('HttpResponse',)
       ('RequestFactory',)
-      ('inject_args', 'param', 'param_get', 'param_post')
+      ('inject_args', 'param', 'param_get', 'param_post', 'view')
+      ('create_resolved_request',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006421640484045a
             05640584005a06640684005a07640784005a08640884005a09640984005a
             0a640a84005a0b640b84005a0c640c84005a0d640d84005a0e640e84005a
             0f640f84005a10641084005a11641184005a12641284005a13641384005a
             14641484005a15641584005a16641684005a17641784005a18641884005a
             19641984005a1a641a84005a1b641b84005a1c641c84005a1d641d84005a
             1e641e84005a1f641f84005a20642084005a2164035300
-          13           0 RESUME                   0
+          14           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParamsToArgsDecoratorTestCase')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          14          12 LOAD_NAME                3 (RequestFactory)
+          15          12 LOAD_NAME                3 (RequestFactory)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('factory')
                       18 STORE_SUBSCR
          
-          16          22 LOAD_CONST              33 (('return', None))
-                      24 LOAD_CONST               4 (<code object setUp, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 16>)
+          17          22 LOAD_CONST              33 (('return', None))
+                      24 LOAD_CONST               4 (<code object setUp, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 17>)
                       26 MAKE_FUNCTION            4 (annotations)
                       28 STORE_NAME               5 (setUp)
          
-          20          30 LOAD_CONST               5 (<code object test_without_type_annotation, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 20>)
+          21          30 LOAD_CONST               5 (<code object test_without_type_annotation, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 21>)
                       32 MAKE_FUNCTION            0
                       34 STORE_NAME               6 (test_without_type_annotation)
          
-          34          36 LOAD_CONST               6 (<code object test_param_default_defines_target_type, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 34>)
+          35          36 LOAD_CONST               6 (<code object test_param_default_defines_target_type, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 35>)
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               7 (test_param_default_defines_target_type)
          
-          43          42 LOAD_CONST               7 (<code object test_missing_param_raises_exception, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 43>)
+          44          42 LOAD_CONST               7 (<code object test_missing_param_raises_exception, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 44>)
                       44 MAKE_FUNCTION            0
                       46 STORE_NAME               8 (test_missing_param_raises_exception)
          
-          53          48 LOAD_CONST               8 (<code object test_optional, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 53>)
+          54          48 LOAD_CONST               8 (<code object test_optional, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 54>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               9 (test_optional)
          
-          65          54 LOAD_CONST               9 (<code object test_optional_with_type_conversion, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 65>)
+          66          54 LOAD_CONST               9 (<code object test_optional_with_type_conversion, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 66>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME              10 (test_optional_with_type_conversion)
          
-          75          60 LOAD_CONST              10 (<code object test_type_conversion_int, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 75>)
+          76          60 LOAD_CONST              10 (<code object test_type_conversion_int, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 76>)
                       62 MAKE_FUNCTION            0
                       64 STORE_NAME              11 (test_type_conversion_int)
          
-          82          66 LOAD_CONST              11 (<code object test_type_conversion_float, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 82>)
+          83          66 LOAD_CONST              11 (<code object test_type_conversion_float, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 83>)
                       68 MAKE_FUNCTION            0
                       70 STORE_NAME              12 (test_type_conversion_float)
          
-          90          72 LOAD_CONST              12 (<code object test_type_conversion_bool, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 90>)
+          91          72 LOAD_CONST              12 (<code object test_type_conversion_bool, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 91>)
                       74 MAKE_FUNCTION            0
                       76 STORE_NAME              13 (test_type_conversion_bool)
          
-         104          78 LOAD_CONST              13 (<code object test_type_conversion_list_unannotated, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 104>)
+         105          78 LOAD_CONST              13 (<code object test_type_conversion_list_unannotated, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 105>)
                       80 MAKE_FUNCTION            0
                       82 STORE_NAME              14 (test_type_conversion_list_unannotated)
          
-         113          84 LOAD_CONST              14 (<code object test_type_conversion_list_annotated, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 113>)
+         114          84 LOAD_CONST              14 (<code object test_type_conversion_list_annotated, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 114>)
                       86 MAKE_FUNCTION            0
                       88 STORE_NAME              15 (test_type_conversion_list_annotated)
          
-         122          90 LOAD_CONST              15 (<code object test_post, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 122>)
+         123          90 LOAD_CONST              15 (<code object test_post, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 123>)
                       92 MAKE_FUNCTION            0
                       94 STORE_NAME              16 (test_post)
          
-         134          96 LOAD_CONST              16 (<code object test_get_and_post_order, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 134>)
+         135          96 LOAD_CONST              16 (<code object test_get_and_post_order, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 135>)
                       98 MAKE_FUNCTION            0
                      100 STORE_NAME              17 (test_get_and_post_order)
          
-         141         102 LOAD_CONST              17 (<code object test_function_call_arg_overrides_param, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 141>)
+         142         102 LOAD_CONST              17 (<code object test_function_call_arg_overrides_param, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 142>)
                      104 MAKE_FUNCTION            0
                      106 STORE_NAME              18 (test_function_call_arg_overrides_param)
          
-         148         108 LOAD_CONST              18 (<code object test_function_call_kwarg_overrides_param, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 148>)
+         149         108 LOAD_CONST              18 (<code object test_function_call_kwarg_overrides_param, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 149>)
                      110 MAKE_FUNCTION            0
                      112 STORE_NAME              19 (test_function_call_kwarg_overrides_param)
          
-         155         114 LOAD_CONST              19 (<code object test_param_consume_true, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 155>)
+         156         114 LOAD_CONST              19 (<code object test_param_consume_true, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 156>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              20 (test_param_consume_true)
          
-         163         120 LOAD_CONST              20 (<code object test_param_consume_false, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 163>)
+         164         120 LOAD_CONST              20 (<code object test_param_consume_false, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 164>)
                      122 MAKE_FUNCTION            0
                      124 STORE_NAME              21 (test_param_consume_false)
          
-         171         126 LOAD_CONST              21 (<code object test_param_consume_get, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 171>)
+         172         126 LOAD_CONST              21 (<code object test_param_consume_get, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 172>)
                      128 MAKE_FUNCTION            0
                      130 STORE_NAME              22 (test_param_consume_get)
          
-         179         132 LOAD_CONST              22 (<code object test_param_consume_post, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 179>)
+         180         132 LOAD_CONST              22 (<code object test_param_consume_post, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 180>)
                      134 MAKE_FUNCTION            0
                      136 STORE_NAME              23 (test_param_consume_post)
          
-         187         138 LOAD_CONST              23 (<code object test_auto_default_value, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 187>)
+         188         138 LOAD_CONST              23 (<code object test_auto_default_value, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 188>)
                      140 MAKE_FUNCTION            0
                      142 STORE_NAME              24 (test_auto_default_value)
          
-         195         144 LOAD_CONST              24 (<code object test_auto_param_false, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 195>)
+         196         144 LOAD_CONST              24 (<code object test_auto_param_false, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 196>)
                      146 MAKE_FUNCTION            0
                      148 STORE_NAME              25 (test_auto_param_false)
          
-         209         150 LOAD_CONST              25 (<code object test_auto_param_true, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 209>)
+         210         150 LOAD_CONST              25 (<code object test_auto_param_true, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 210>)
                      152 MAKE_FUNCTION            0
                      154 STORE_NAME              26 (test_auto_param_true)
          
-         217         156 LOAD_CONST              26 (<code object test_auto_param_get, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 217>)
+         218         156 LOAD_CONST              26 (<code object test_auto_param_get, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 218>)
                      158 MAKE_FUNCTION            0
                      160 STORE_NAME              27 (test_auto_param_get)
          
-         225         162 LOAD_CONST              27 (<code object test_auto_param_get_does_not_receive_post_params, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 225>)
+         226         162 LOAD_CONST              27 (<code object test_auto_param_get_does_not_receive_post_params, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 226>)
                      164 MAKE_FUNCTION            0
                      166 STORE_NAME              28 (test_auto_param_get_does_not_receive_post_params)
          
-         234         168 LOAD_CONST              28 (<code object test_auto_param_post, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 234>)
+         235         168 LOAD_CONST              28 (<code object test_auto_param_post, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 235>)
                      170 MAKE_FUNCTION            0
                      172 STORE_NAME              29 (test_auto_param_post)
          
-         242         174 LOAD_CONST              29 (<code object test_auto_param_post_does_not_receive_get_params, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 242>)
+         243         174 LOAD_CONST              29 (<code object test_auto_param_post_does_not_receive_get_params, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 243>)
                      176 MAKE_FUNCTION            0
                      178 STORE_NAME              30 (test_auto_param_post_does_not_receive_get_params)
          
-         251         180 LOAD_CONST              30 (<code object test_auto_param_form, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 251>)
+         252         180 LOAD_CONST              30 (<code object test_auto_param_form, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 252>)
                      182 MAKE_FUNCTION            0
                      184 STORE_NAME              31 (test_auto_param_form)
          
-         263         186 LOAD_CONST              31 (<code object test_multiple_form_params_raises_exception, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 263>)
+         264         186 LOAD_CONST              31 (<code object test_multiple_form_params_raises_exception, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 264>)
                      188 MAKE_FUNCTION            0
                      190 STORE_NAME              32 (test_multiple_form_params_raises_exception)
          
-         277         192 LOAD_CONST              32 (<code object test_auto_param_form_is_false, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 277>)
+         278         192 LOAD_CONST              32 (<code object test_auto_param_form_is_false, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 278>)
                      194 MAKE_FUNCTION            0
                      196 STORE_NAME              33 (test_auto_param_form_is_false)
                      198 LOAD_CONST               3 (None)
                      200 RETURN_VALUE
          consts
             'ParamsToArgsDecoratorTestCase'
             'factory'
@@ -247,38 +258,38 @@
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000007c
                   005f0100000000000000007405000000000000000000006a030000000000
                   000000a6000000ab000000000000000000010064005300
-                16           0 RESUME                   0
+                17           0 RESUME                   0
                
-                17           2 LOAD_GLOBAL              1 (NULL + RequestFactory)
+                18           2 LOAD_GLOBAL              1 (NULL + RequestFactory)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (factory)
                
-                18          40 LOAD_GLOBAL              5 (NULL + django)
+                19          40 LOAD_GLOBAL              5 (NULL + django)
                             52 LOAD_ATTR                3 (setup)
                             62 PRECALL                  0
                             66 CALL                     0
                             76 POP_TOP
                             78 LOAD_CONST               0 (None)
                             80 RETURN_VALUE
                consts
                   None
                names      ('RequestFactory', 'factory', 'django', 'setup')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'setUp'
-               firstlineno 16
+               firstlineno 17
                lnotab 0x02012601
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
@@ -288,52 +299,52 @@
                   018409a6000000ab0000000000000000007d0102007c0189006a02000000
                   0000000000a00300000000000000000000000000000000000000006402a6
                   010000ab010000000000000000a6010000ab0100000000000000007d0289
                   00a00400000000000000000000000000000000000000007c026a05000000
                   00000000006403a6020000ab020000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-                20           2 RESUME                   0
+                21           2 RESUME                   0
                
-                21           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                22           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                24          30 LOAD_GLOBAL              3 (NULL + param_get)
+                25          30 LOAD_GLOBAL              3 (NULL + param_get)
                             42 PRECALL                  0
                             46 CALL                     0
                
-                25          56 LOAD_GLOBAL              3 (NULL + param_get)
+                26          56 LOAD_GLOBAL              3 (NULL + param_get)
                             68 PRECALL                  0
                             72 CALL                     0
                
-                22          82 BUILD_TUPLE              2
+                23          82 BUILD_TUPLE              2
                             84 LOAD_CLOSURE             0 (self)
                             86 BUILD_TUPLE              1
-                            88 LOAD_CONST               1 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 21>)
+                            88 LOAD_CONST               1 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 22>)
                             90 MAKE_FUNCTION            9 (defaults, closure)
                
-                21          92 PRECALL                  0
+                22          92 PRECALL                  0
                             96 CALL                     0
                
-                22         106 STORE_FAST               1 (viewfn)
+                23         106 STORE_FAST               1 (viewfn)
                
-                31         108 PUSH_NULL
+                32         108 PUSH_NULL
                            110 LOAD_FAST                1 (viewfn)
                            112 LOAD_DEREF               0 (self)
                            114 LOAD_ATTR                2 (factory)
                            124 LOAD_METHOD              3 (get)
                            146 LOAD_CONST               2 ('/?p1=a&p2=b')
                            148 PRECALL                  1
                            152 CALL                     1
                            162 PRECALL                  1
                            166 CALL                     1
                            176 STORE_FAST               2 (result)
                
-                32         178 LOAD_DEREF               0 (self)
+                33         178 LOAD_DEREF               0 (self)
                            180 LOAD_METHOD              4 (assertEqual)
                            202 LOAD_FAST                2 (result)
                            204 LOAD_ATTR                5 (status_code)
                            214 LOAD_CONST               3 (200)
                            216 PRECALL                  2
                            220 CALL                     2
                            230 POP_TOP
@@ -350,33 +361,33 @@
                         0x950197008903a00000000000000000000000000000000000000000007c
                         016401a6020000ab02000000000000000001008903a00000000000000000
                         000000000000000000000000007c026402a6020000ab0200000000000000
                         0001007403000000000000000000006403a6010000ab0100000000000000
                         005300
                                    0 COPY_FREE_VARS           1
                      
-                      21           2 RESUME                   0
+                      22           2 RESUME                   0
                      
-                      27           4 LOAD_DEREF               3 (self)
+                      28           4 LOAD_DEREF               3 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                      28          48 LOAD_DEREF               3 (self)
+                      29          48 LOAD_DEREF               3 (self)
                                   50 LOAD_METHOD              0 (assertEqual)
                                   72 LOAD_FAST                2 (p2)
                                   74 LOAD_CONST               2 ('b')
                                   76 PRECALL                  2
                                   80 CALL                     2
                                   90 POP_TOP
                      
-                      29          92 LOAD_GLOBAL              3 (NULL + HttpResponse)
+                      30          92 LOAD_GLOBAL              3 (NULL + HttpResponse)
                                  104 LOAD_CONST               3 ('')
                                  106 PRECALL                  1
                                  110 CALL                     1
                                  120 RETURN_VALUE
                      consts
                         None
                         'a'
@@ -384,25 +395,25 @@
                         ''
                      names      ('assertEqual', 'HttpResponse')
                      varnames   ('_request', 'p1', 'p2')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 21
+                     firstlineno 22
                      lnotab 0x04062c012c01
                   '/?p1=a&p2=b'
                   200
-               names      ('inject_args', 'param_get', 'factory', 'get', 'assertEqual', 'status_code')
+               names      ('view', 'param_get', 'factory', 'get', 'assertEqual', 'status_code')
                varnames   ('self', 'viewfn', 'result')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_without_type_annotation'
-               firstlineno 20
+               firstlineno 21
                lnotab 0x04011a031a011afd0aff0e0102094601
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
@@ -412,49 +423,49 @@
                   0189006a020000000000000000a003000000000000000000000000000000
                   00000000006404a6010000ab010000000000000000a6010000ab01000000
                   00000000007d028900a00400000000000000000000000000000000000000
                   007c026a0500000000000000006405a6020000ab02000000000000000001
                   0064005300
                              0 MAKE_CELL                0 (self)
                
-                34           2 RESUME                   0
+                35           2 RESUME                   0
                
-                35           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                36           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                36          30 LOAD_GLOBAL              3 (NULL + param)
+                37          30 LOAD_GLOBAL              3 (NULL + param)
                             42 LOAD_CONST               1 (123)
                             44 KW_NAMES                 2
                             46 PRECALL                  1
                             50 CALL                     1
                             60 BUILD_TUPLE              1
                             62 LOAD_CLOSURE             0 (self)
                             64 BUILD_TUPLE              1
-                            66 LOAD_CONST               3 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 35>)
+                            66 LOAD_CONST               3 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 36>)
                             68 MAKE_FUNCTION            9 (defaults, closure)
                
-                35          70 PRECALL                  0
+                36          70 PRECALL                  0
                             74 CALL                     0
                
-                36          84 STORE_FAST               1 (viewfn)
+                37          84 STORE_FAST               1 (viewfn)
                
-                40          86 PUSH_NULL
+                41          86 PUSH_NULL
                             88 LOAD_FAST                1 (viewfn)
                             90 LOAD_DEREF               0 (self)
                             92 LOAD_ATTR                2 (factory)
                            102 LOAD_METHOD              3 (get)
                            124 LOAD_CONST               4 ('/?p1=999')
                            126 PRECALL                  1
                            130 CALL                     1
                            140 PRECALL                  1
                            144 CALL                     1
                            154 STORE_FAST               2 (result)
                
-                41         156 LOAD_DEREF               0 (self)
+                42         156 LOAD_DEREF               0 (self)
                            158 LOAD_METHOD              4 (assertEqual)
                            180 LOAD_FAST                2 (result)
                            182 LOAD_ATTR                5 (status_code)
                            192 LOAD_CONST               5 (200)
                            194 PRECALL                  2
                            198 CALL                     2
                            208 POP_TOP
@@ -471,50 +482,50 @@
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab02000000000000000001007403000000000000000000
                         006402a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      35           2 RESUME                   0
+                      36           2 RESUME                   0
                      
-                      37           4 LOAD_DEREF               2 (self)
+                      38           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 (999)
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                      38          48 LOAD_GLOBAL              3 (NULL + HttpResponse)
+                      39          48 LOAD_GLOBAL              3 (NULL + HttpResponse)
                                   60 LOAD_CONST               2 ('')
                                   62 PRECALL                  1
                                   66 CALL                     1
                                   76 RETURN_VALUE
                      consts
                         None
                         999
                         ''
                      names      ('assertEqual', 'HttpResponse')
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 35
+                     firstlineno 36
                      lnotab 0x04022c01
                   '/?p1=999'
                   200
-               names      ('inject_args', 'param', 'factory', 'get', 'assertEqual', 'status_code')
+               names      ('view', 'param', 'factory', 'get', 'assertEqual', 'status_code')
                varnames   ('self', 'viewfn', 'result')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_param_default_defines_target_type'
-               firstlineno 34
+               firstlineno 35
                lnotab 0x04011a0128ff0e0102044601
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
@@ -523,42 +534,42 @@
                   018800660164018409a6000000ab0000000000000000008a028800880266
                   02640284087d018900a00200000000000000000000000000000000000000
                   007406000000000000000000007c01a6020000ab02000000000000000001
                   0064005300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                2 (viewfn)
                
-                43           4 RESUME                   0
+                44           4 RESUME                   0
                
-                44           6 LOAD_GLOBAL              1 (NULL + inject_args)
+                45           6 LOAD_GLOBAL              1 (NULL + view)
                             18 PRECALL                  0
                             22 CALL                     0
                
-                45          32 LOAD_GLOBAL              3 (NULL + param_get)
+                46          32 LOAD_GLOBAL              3 (NULL + param_get)
                             44 PRECALL                  0
                             48 CALL                     0
                             58 BUILD_TUPLE              1
                             60 LOAD_CLOSURE             0 (self)
                             62 BUILD_TUPLE              1
-                            64 LOAD_CONST               1 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 44>)
+                            64 LOAD_CONST               1 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 45>)
                             66 MAKE_FUNCTION            9 (defaults, closure)
                
-                44          68 PRECALL                  0
+                45          68 PRECALL                  0
                             72 CALL                     0
                
-                45          82 STORE_DEREF              2 (viewfn)
+                46          82 STORE_DEREF              2 (viewfn)
                
-                48          84 LOAD_CLOSURE             0 (self)
+                49          84 LOAD_CLOSURE             0 (self)
                             86 LOAD_CLOSURE             2 (viewfn)
                             88 BUILD_TUPLE              2
-                            90 LOAD_CONST               2 (<code object test, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 48>)
+                            90 LOAD_CONST               2 (<code object test, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 49>)
                             92 MAKE_FUNCTION            8 (closure)
                             94 STORE_FAST               1 (test)
                
-                51          96 LOAD_DEREF               0 (self)
+                52          96 LOAD_DEREF               0 (self)
                             98 LOAD_METHOD              2 (assertRaises)
                            120 LOAD_GLOBAL              6 (Exception)
                            132 LOAD_FAST                1 (test)
                            134 PRECALL                  2
                            138 CALL                     2
                            148 POP_TOP
                            150 LOAD_CONST               0 (None)
@@ -571,17 +582,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                      44           2 RESUME                   0
+                      45           2 RESUME                   0
                      
-                      46           4 LOAD_DEREF               2 (self)
+                      47           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 (1)
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -591,30 +602,30 @@
                         1
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 44
+                     firstlineno 45
                      lnotab 0x0402
                   code
                      argcount  : 0
                      nlocals   : 0
                      stacksize : 5
                      flags     : 19
                      code
                         0x950297000200890189006a000000000000000000a00100000000000000
                         000000000000000000000000006401a6010000ab010000000000000000a6
                         010000ab010000000000000000010064005300
                                    0 COPY_FREE_VARS           2
                      
-                      48           2 RESUME                   0
+                      49           2 RESUME                   0
                      
-                      49           4 PUSH_NULL
+                      50           4 PUSH_NULL
                                    6 LOAD_DEREF               1 (viewfn)
                                    8 LOAD_DEREF               0 (self)
                                   10 LOAD_ATTR                0 (factory)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('/')
                                   44 PRECALL                  1
                                   48 CALL                     1
@@ -628,23 +639,23 @@
                         '/'
                      names      ('factory', 'get')
                      varnames   ()
                      freevars   ('self', 'viewfn')
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'test'
-                     firstlineno 48
+                     firstlineno 49
                      lnotab 0x0401
-               names      ('inject_args', 'param_get', 'assertRaises', 'Exception')
+               names      ('view', 'param_get', 'assertRaises', 'Exception')
                varnames   ('self', 'test')
                freevars   ()
                cellvars   ('self', 'viewfn')
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_missing_param_raises_exception'
-               firstlineno 43
+               firstlineno 44
                lnotab 0x06011a0124ff0e0102030c03
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
                flags     : 3
                code
@@ -655,53 +666,53 @@
                   040000000000000000000019000000000000000000660488006601640384
                   0da6000000ab0000000000000000007d0102007c0189006a040000000000
                   000000a00500000000000000000000000000000000000000006404a60100
                   00ab010000000000000000a6010000ab0100000000000000000100640053
                   00
                              0 MAKE_CELL                0 (self)
                
-                53           2 RESUME                   0
+                54           2 RESUME                   0
                
-                54           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                55           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                57          30 LOAD_GLOBAL              3 (NULL + param_get)
+                58          30 LOAD_GLOBAL              3 (NULL + param_get)
                             42 PRECALL                  0
                             46 CALL                     0
                
-                58          56 LOAD_GLOBAL              3 (NULL + param_get)
+                59          56 LOAD_GLOBAL              3 (NULL + param_get)
                             68 PRECALL                  0
                             72 CALL                     0
                
-                55          82 BUILD_TUPLE              2
+                56          82 BUILD_TUPLE              2
                             84 LOAD_CONST               1 ('p1')
                
-                57          86 LOAD_GLOBAL              4 (str)
+                58          86 LOAD_GLOBAL              4 (str)
                             98 LOAD_CONST               0 (None)
                            100 BINARY_OP                7 (|)
                
-                55         104 LOAD_CONST               2 ('p2')
+                56         104 LOAD_CONST               2 ('p2')
                
-                58         106 LOAD_GLOBAL              6 (Optional)
+                59         106 LOAD_GLOBAL              6 (Optional)
                            118 LOAD_GLOBAL              4 (str)
                            130 BINARY_SUBSCR
                
-                55         140 BUILD_TUPLE              4
+                56         140 BUILD_TUPLE              4
                            142 LOAD_CLOSURE             0 (self)
                            144 BUILD_TUPLE              1
-                           146 LOAD_CONST               3 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 54>)
+                           146 LOAD_CONST               3 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 55>)
                            148 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-                54         150 PRECALL                  0
+                55         150 PRECALL                  0
                            154 CALL                     0
                
-                55         164 STORE_FAST               1 (viewfn)
+                56         164 STORE_FAST               1 (viewfn)
                
-                63         166 PUSH_NULL
+                64         166 PUSH_NULL
                            168 LOAD_FAST                1 (viewfn)
                            170 LOAD_DEREF               0 (self)
                            172 LOAD_ATTR                4 (factory)
                            182 LOAD_METHOD              5 (get)
                            204 LOAD_CONST               4 ('/')
                            206 PRECALL                  1
                            210 CALL                     1
@@ -722,25 +733,25 @@
                      code
                         0x950197008903a00000000000000000000000000000000000000000007c
                         016400a6020000ab02000000000000000001008903a00000000000000000
                         000000000000000000000000007c026400a6020000ab0200000000000000
                         00010064005300
                                    0 COPY_FREE_VARS           1
                      
-                      54           2 RESUME                   0
+                      55           2 RESUME                   0
                      
-                      60           4 LOAD_DEREF               3 (self)
+                      61           4 LOAD_DEREF               3 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               0 (None)
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                      61          48 LOAD_DEREF               3 (self)
+                      62          48 LOAD_DEREF               3 (self)
                                   50 LOAD_METHOD              0 (assertEqual)
                                   72 LOAD_FAST                2 (p2)
                                   74 LOAD_CONST               0 (None)
                                   76 PRECALL                  2
                                   80 CALL                     2
                                   90 POP_TOP
                                   92 LOAD_CONST               0 (None)
@@ -749,24 +760,24 @@
                         None
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1', 'p2')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 54
+                     firstlineno 55
                      lnotab 0x04062c01
                   '/'
-               names      ('inject_args', 'param_get', 'str', 'Optional', 'factory', 'get')
+               names      ('view', 'param_get', 'str', 'Optional', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_optional'
-               firstlineno 53
+               firstlineno 54
                lnotab 0x04011a031a011afd040212fe020322fd0aff0e010208
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -775,43 +786,43 @@
                   017404000000000000000000007406000000000000000000001900000000
                   00000000006602880066016402840da6000000ab0000000000000000007d
                   0102007c0189006a040000000000000000a0050000000000000000000000
                   0000000000000000006403a6010000ab010000000000000000a6010000ab
                   010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-                65           2 RESUME                   0
+                66           2 RESUME                   0
                
-                66           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                67           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                69          30 LOAD_GLOBAL              3 (NULL + param_get)
+                70          30 LOAD_GLOBAL              3 (NULL + param_get)
                             42 PRECALL                  0
                             46 CALL                     0
                
-                67          56 BUILD_TUPLE              1
+                68          56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('p1')
                
-                69          60 LOAD_GLOBAL              4 (Optional)
+                70          60 LOAD_GLOBAL              4 (Optional)
                             72 LOAD_GLOBAL              6 (int)
                             84 BINARY_SUBSCR
                
-                67          94 BUILD_TUPLE              2
+                68          94 BUILD_TUPLE              2
                             96 LOAD_CLOSURE             0 (self)
                             98 BUILD_TUPLE              1
-                           100 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 66>)
+                           100 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 67>)
                            102 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-                66         104 PRECALL                  0
+                67         104 PRECALL                  0
                            108 CALL                     0
                
-                67         118 STORE_FAST               1 (viewfn)
+                68         118 STORE_FAST               1 (viewfn)
                
-                73         120 PUSH_NULL
+                74         120 PUSH_NULL
                            122 LOAD_FAST                1 (viewfn)
                            124 LOAD_DEREF               0 (self)
                            126 LOAD_ATTR                4 (factory)
                            136 LOAD_METHOD              5 (get)
                            158 LOAD_CONST               3 ('/?p1=1')
                            160 PRECALL                  1
                            164 CALL                     1
@@ -829,17 +840,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                      66           2 RESUME                   0
+                      67           2 RESUME                   0
                      
-                      71           4 LOAD_DEREF               2 (self)
+                      72           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 (1)
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -849,24 +860,24 @@
                         1
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 66
+                     firstlineno 67
                      lnotab 0x0405
                   '/?p1=1'
-               names      ('inject_args', 'param_get', 'Optional', 'int', 'factory', 'get')
+               names      ('view', 'param_get', 'Optional', 'int', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_optional_with_type_conversion'
-               firstlineno 65
+               firstlineno 66
                lnotab 0x04011a031afe040222fe0aff0e010206
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -874,38 +885,38 @@
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
                   000000000000007d0102007c0189006a030000000000000000a004000000
                   00000000000000000000000000000000006403a6010000ab010000000000
                   000000a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-                75           2 RESUME                   0
+                76           2 RESUME                   0
                
-                76           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                77           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                77          30 LOAD_GLOBAL              3 (NULL + param_get)
+                78          30 LOAD_GLOBAL              3 (NULL + param_get)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('p1')
                             60 LOAD_GLOBAL              4 (int)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 76>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 77>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-                76          82 PRECALL                  0
+                77          82 PRECALL                  0
                             86 CALL                     0
                
-                77          96 STORE_FAST               1 (viewfn)
+                78          96 STORE_FAST               1 (viewfn)
                
-                80          98 PUSH_NULL
+                81          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
                            102 LOAD_DEREF               0 (self)
                            104 LOAD_ATTR                3 (factory)
                            114 LOAD_METHOD              4 (get)
                            136 LOAD_CONST               3 ('/?p1=1')
                            138 PRECALL                  1
                            142 CALL                     1
@@ -923,17 +934,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                      76           2 RESUME                   0
+                      77           2 RESUME                   0
                      
-                      78           4 LOAD_DEREF               2 (self)
+                      79           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 (1)
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -943,24 +954,24 @@
                         1
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 76
+                     firstlineno 77
                      lnotab 0x0402
                   '/?p1=1'
-               names      ('inject_args', 'param_get', 'int', 'factory', 'get')
+               names      ('view', 'param_get', 'int', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_type_conversion_int'
-               firstlineno 75
+               firstlineno 76
                lnotab 0x04011a0134ff0e010203
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -968,38 +979,38 @@
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
                   000000000000007d0102007c0189006a030000000000000000a004000000
                   00000000000000000000000000000000006403a6010000ab010000000000
                   000000a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-                82           2 RESUME                   0
+                83           2 RESUME                   0
                
-                83           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                84           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                84          30 LOAD_GLOBAL              3 (NULL + param_get)
+                85          30 LOAD_GLOBAL              3 (NULL + param_get)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('p1')
                             60 LOAD_GLOBAL              4 (float)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 83>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 84>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-                83          82 PRECALL                  0
+                84          82 PRECALL                  0
                             86 CALL                     0
                
-                84          96 STORE_FAST               1 (viewfn)
+                85          96 STORE_FAST               1 (viewfn)
                
-                88          98 PUSH_NULL
+                89          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
                            102 LOAD_DEREF               0 (self)
                            104 LOAD_ATTR                3 (factory)
                            114 LOAD_METHOD              4 (get)
                            136 LOAD_CONST               3 ('/?p1=1.1')
                            138 PRECALL                  1
                            142 CALL                     1
@@ -1020,25 +1031,25 @@
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab02000000000000000001008902a00000000000000000
                         000000000000000000000000007403000000000000000000007c01a60100
                         00ab010000000000000000740400000000000000000000a6020000ab0200
                         00000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                      83           2 RESUME                   0
+                      84           2 RESUME                   0
                      
-                      85           4 LOAD_DEREF               2 (self)
+                      86           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 (1.1)
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                      86          48 LOAD_DEREF               2 (self)
+                      87          48 LOAD_DEREF               2 (self)
                                   50 LOAD_METHOD              0 (assertEqual)
                                   72 LOAD_GLOBAL              3 (NULL + type)
                                   84 LOAD_FAST                1 (p1)
                                   86 PRECALL                  1
                                   90 CALL                     1
                                  100 LOAD_GLOBAL              4 (float)
                                  112 PRECALL                  2
@@ -1051,24 +1062,24 @@
                         1.1
                      names      ('assertEqual', 'type', 'float')
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 83
+                     firstlineno 84
                      lnotab 0x04022c01
                   '/?p1=1.1'
-               names      ('inject_args', 'param_get', 'float', 'factory', 'get')
+               names      ('view', 'param_get', 'float', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_type_conversion_float'
-               firstlineno 82
+               firstlineno 83
                lnotab 0x04011a0134ff0e010204
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
@@ -1079,57 +1090,57 @@
                   000000000064027404000000000000000000006403740400000000000000
                   0000006606880066016404840da6000000ab0000000000000000007d0102
                   007c0189006a030000000000000000a00400000000000000000000000000
                   000000000000006405a6010000ab010000000000000000a6010000ab0100
                   00000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-                90           2 RESUME                   0
+                91           2 RESUME                   0
                
-                91           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                92           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-                94          30 LOAD_GLOBAL              3 (NULL + param_get)
+                95          30 LOAD_GLOBAL              3 (NULL + param_get)
                             42 PRECALL                  0
                             46 CALL                     0
                
-                95          56 LOAD_GLOBAL              3 (NULL + param_get)
+                96          56 LOAD_GLOBAL              3 (NULL + param_get)
                             68 PRECALL                  0
                             72 CALL                     0
                
-                96          82 LOAD_GLOBAL              3 (NULL + param_get)
+                97          82 LOAD_GLOBAL              3 (NULL + param_get)
                             94 PRECALL                  0
                             98 CALL                     0
                
-                92         108 BUILD_TUPLE              3
+                93         108 BUILD_TUPLE              3
                            110 LOAD_CONST               1 ('p1')
                
-                94         112 LOAD_GLOBAL              4 (bool)
+                95         112 LOAD_GLOBAL              4 (bool)
                
-                92         124 LOAD_CONST               2 ('p2')
+                93         124 LOAD_CONST               2 ('p2')
                
-                95         126 LOAD_GLOBAL              4 (bool)
+                96         126 LOAD_GLOBAL              4 (bool)
                
-                92         138 LOAD_CONST               3 ('p3')
+                93         138 LOAD_CONST               3 ('p3')
                
-                96         140 LOAD_GLOBAL              4 (bool)
+                97         140 LOAD_GLOBAL              4 (bool)
                
-                92         152 BUILD_TUPLE              6
+                93         152 BUILD_TUPLE              6
                            154 LOAD_CLOSURE             0 (self)
                            156 BUILD_TUPLE              1
-                           158 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 91>)
+                           158 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 92>)
                            160 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-                91         162 PRECALL                  0
+                92         162 PRECALL                  0
                            166 CALL                     0
                
-                92         176 STORE_FAST               1 (viewfn)
+                93         176 STORE_FAST               1 (viewfn)
                
-               102         178 PUSH_NULL
+               103         178 PUSH_NULL
                            180 LOAD_FAST                1 (viewfn)
                            182 LOAD_DEREF               0 (self)
                            184 LOAD_ATTR                3 (factory)
                            194 LOAD_METHOD              4 (get)
                            216 LOAD_CONST               5 ('/?p1=false&p2=False&p3')
                            218 PRECALL                  1
                            222 CALL                     1
@@ -1152,33 +1163,33 @@
                         0x950197008904a00000000000000000000000000000000000000000007c
                         016401a6020000ab02000000000000000001008904a00000000000000000
                         000000000000000000000000007c026401a6020000ab0200000000000000
                         0001008904a00000000000000000000000000000000000000000007c0364
                         01a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                      91           2 RESUME                   0
+                      92           2 RESUME                   0
                      
-                      98           4 LOAD_DEREF               4 (self)
+                      99           4 LOAD_DEREF               4 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 (False)
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                      99          48 LOAD_DEREF               4 (self)
+                     100          48 LOAD_DEREF               4 (self)
                                   50 LOAD_METHOD              0 (assertEqual)
                                   72 LOAD_FAST                2 (p2)
                                   74 LOAD_CONST               1 (False)
                                   76 PRECALL                  2
                                   80 CALL                     2
                                   90 POP_TOP
                      
-                     100          92 LOAD_DEREF               4 (self)
+                     101          92 LOAD_DEREF               4 (self)
                                   94 LOAD_METHOD              0 (assertEqual)
                                  116 LOAD_FAST                3 (p3)
                                  118 LOAD_CONST               1 (False)
                                  120 PRECALL                  2
                                  124 CALL                     2
                                  134 POP_TOP
                                  136 LOAD_CONST               0 (None)
@@ -1188,24 +1199,24 @@
                         False
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1', 'p2', 'p3')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 91
+                     firstlineno 92
                      lnotab 0x04072c012c01
                   '/?p1=false&p2=False&p3'
-               names      ('inject_args', 'param_get', 'bool', 'factory', 'get')
+               names      ('view', 'param_get', 'bool', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_type_conversion_bool'
-               firstlineno 90
+               firstlineno 91
                lnotab 0x04011a031a011a011afc04020cfe02030cfd02040cfc0aff0e01020a
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -1213,38 +1224,38 @@
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
                   000000000000007d0102007c0189006a030000000000000000a004000000
                   00000000000000000000000000000000006403a6010000ab010000000000
                   000000a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               104           2 RESUME                   0
+               105           2 RESUME                   0
                
-               105           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               106           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-               106          30 LOAD_GLOBAL              3 (NULL + param_get)
+               107          30 LOAD_GLOBAL              3 (NULL + param_get)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('p1')
                             60 LOAD_GLOBAL              4 (list)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 105>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 106>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               105          82 PRECALL                  0
+               106          82 PRECALL                  0
                             86 CALL                     0
                
-               106          96 STORE_FAST               1 (viewfn)
+               107          96 STORE_FAST               1 (viewfn)
                
-               111          98 PUSH_NULL
+               112          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
                            102 LOAD_DEREF               0 (self)
                            104 LOAD_ATTR                3 (factory)
                            114 LOAD_METHOD              4 (get)
                            136 LOAD_CONST               3 ('/?p1=a&p1=b')
                            138 PRECALL                  1
                            142 CALL                     1
@@ -1267,37 +1278,37 @@
                         000000000000000000a6020000ab02000000000000000001008902a00300
                         0000000000000000000000000000000000000064017c017600a6010000ab
                         01000000000000000001008902a003000000000000000000000000000000
                         000000000064027c017600a6010000ab0100000000000000000100640053
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     105           2 RESUME                   0
+                     106           2 RESUME                   0
                      
-                     107           4 LOAD_DEREF               2 (self)
+                     108           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_GLOBAL              3 (NULL + type)
                                   40 LOAD_FAST                1 (p1)
                                   42 PRECALL                  1
                                   46 CALL                     1
                                   56 LOAD_GLOBAL              4 (list)
                                   68 PRECALL                  2
                                   72 CALL                     2
                                   82 POP_TOP
                      
-                     108          84 LOAD_DEREF               2 (self)
+                     109          84 LOAD_DEREF               2 (self)
                                   86 LOAD_METHOD              3 (assertTrue)
                                  108 LOAD_CONST               1 ('a')
                                  110 LOAD_FAST                1 (p1)
                                  112 CONTAINS_OP              0
                                  114 PRECALL                  1
                                  118 CALL                     1
                                  128 POP_TOP
                      
-                     109         130 LOAD_DEREF               2 (self)
+                     110         130 LOAD_DEREF               2 (self)
                                  132 LOAD_METHOD              3 (assertTrue)
                                  154 LOAD_CONST               2 ('b')
                                  156 LOAD_FAST                1 (p1)
                                  158 CONTAINS_OP              0
                                  160 PRECALL                  1
                                  164 CALL                     1
                                  174 POP_TOP
@@ -1309,24 +1320,24 @@
                         'b'
                      names      ('assertEqual', 'type', 'list', 'assertTrue')
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 105
+                     firstlineno 106
                      lnotab 0x040250012e01
                   '/?p1=a&p1=b'
-               names      ('inject_args', 'param_get', 'list', 'factory', 'get')
+               names      ('view', 'param_get', 'list', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_type_conversion_list_unannotated'
-               firstlineno 104
+               firstlineno 105
                lnotab 0x04011a0134ff0e010205
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -1335,40 +1346,40 @@
                   017404000000000000000000007406000000000000000000001900000000
                   00000000006602880066016402840da6000000ab0000000000000000007d
                   0102007c0189006a040000000000000000a0050000000000000000000000
                   0000000000000000006403a6010000ab010000000000000000a6010000ab
                   010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               113           2 RESUME                   0
+               114           2 RESUME                   0
                
-               114           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               115           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-               115          30 LOAD_GLOBAL              3 (NULL + param_get)
+               116          30 LOAD_GLOBAL              3 (NULL + param_get)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('p1')
                             60 LOAD_GLOBAL              4 (list)
                             72 LOAD_GLOBAL              6 (int)
                             84 BINARY_SUBSCR
                             94 BUILD_TUPLE              2
                             96 LOAD_CLOSURE             0 (self)
                             98 BUILD_TUPLE              1
-                           100 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 114>)
+                           100 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 115>)
                            102 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               114         104 PRECALL                  0
+               115         104 PRECALL                  0
                            108 CALL                     0
                
-               115         118 STORE_FAST               1 (viewfn)
+               116         118 STORE_FAST               1 (viewfn)
                
-               120         120 PUSH_NULL
+               121         120 PUSH_NULL
                            122 LOAD_FAST                1 (viewfn)
                            124 LOAD_DEREF               0 (self)
                            126 LOAD_ATTR                4 (factory)
                            136 LOAD_METHOD              5 (get)
                            158 LOAD_CONST               3 ('/?p1=1&p1=2')
                            160 PRECALL                  1
                            164 CALL                     1
@@ -1391,37 +1402,37 @@
                         000000000000000000a6020000ab02000000000000000001008902a00300
                         0000000000000000000000000000000000000064017c017600a6010000ab
                         01000000000000000001008902a003000000000000000000000000000000
                         000000000064027c017600a6010000ab0100000000000000000100640053
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     114           2 RESUME                   0
+                     115           2 RESUME                   0
                      
-                     116           4 LOAD_DEREF               2 (self)
+                     117           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_GLOBAL              3 (NULL + type)
                                   40 LOAD_FAST                1 (p1)
                                   42 PRECALL                  1
                                   46 CALL                     1
                                   56 LOAD_GLOBAL              4 (list)
                                   68 PRECALL                  2
                                   72 CALL                     2
                                   82 POP_TOP
                      
-                     117          84 LOAD_DEREF               2 (self)
+                     118          84 LOAD_DEREF               2 (self)
                                   86 LOAD_METHOD              3 (assertTrue)
                                  108 LOAD_CONST               1 (1)
                                  110 LOAD_FAST                1 (p1)
                                  112 CONTAINS_OP              0
                                  114 PRECALL                  1
                                  118 CALL                     1
                                  128 POP_TOP
                      
-                     118         130 LOAD_DEREF               2 (self)
+                     119         130 LOAD_DEREF               2 (self)
                                  132 LOAD_METHOD              3 (assertTrue)
                                  154 LOAD_CONST               2 (2)
                                  156 LOAD_FAST                1 (p1)
                                  158 CONTAINS_OP              0
                                  160 PRECALL                  1
                                  164 CALL                     1
                                  174 POP_TOP
@@ -1433,24 +1444,24 @@
                         2
                      names      ('assertEqual', 'type', 'list', 'assertTrue')
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 114
+                     firstlineno 115
                      lnotab 0x040250012e01
                   '/?p1=1&p1=2'
-               names      ('inject_args', 'param_get', 'list', 'int', 'factory', 'get')
+               names      ('view', 'param_get', 'list', 'int', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_type_conversion_list_annotated'
-               firstlineno 113
+               firstlineno 114
                lnotab 0x04011a014aff0e010205
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
@@ -1460,49 +1471,49 @@
                   000000000000000000640274040000000000000000000066048800660164
                   03840da6000000ab0000000000000000007d0102007c0189006a03000000
                   0000000000a0040000000000000000000000000000000000000000640464
                   05640664079c02a6020000ab020000000000000000a6010000ab01000000
                   0000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               122           2 RESUME                   0
+               123           2 RESUME                   0
                
-               123           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               124           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-               126          30 LOAD_GLOBAL              3 (NULL + param_post)
+               127          30 LOAD_GLOBAL              3 (NULL + param_post)
                             42 PRECALL                  0
                             46 CALL                     0
                
-               127          56 LOAD_GLOBAL              3 (NULL + param_post)
+               128          56 LOAD_GLOBAL              3 (NULL + param_post)
                             68 PRECALL                  0
                             72 CALL                     0
                
-               124          82 BUILD_TUPLE              2
+               125          82 BUILD_TUPLE              2
                             84 LOAD_CONST               1 ('p1')
                
-               126          86 LOAD_GLOBAL              4 (str)
+               127          86 LOAD_GLOBAL              4 (str)
                
-               124          98 LOAD_CONST               2 ('p2')
+               125          98 LOAD_CONST               2 ('p2')
                
-               127         100 LOAD_GLOBAL              4 (str)
+               128         100 LOAD_GLOBAL              4 (str)
                
-               124         112 BUILD_TUPLE              4
+               125         112 BUILD_TUPLE              4
                            114 LOAD_CLOSURE             0 (self)
                            116 BUILD_TUPLE              1
-                           118 LOAD_CONST               3 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 123>)
+                           118 LOAD_CONST               3 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 124>)
                            120 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               123         122 PRECALL                  0
+               124         122 PRECALL                  0
                            126 CALL                     0
                
-               124         136 STORE_FAST               1 (viewfn)
+               125         136 STORE_FAST               1 (viewfn)
                
-               132         138 PUSH_NULL
+               133         138 PUSH_NULL
                            140 LOAD_FAST                1 (viewfn)
                            142 LOAD_DEREF               0 (self)
                            144 LOAD_ATTR                3 (factory)
                            154 LOAD_METHOD              4 (post)
                            176 LOAD_CONST               4 ('/')
                            178 LOAD_CONST               5 ('a')
                            180 LOAD_CONST               6 ('b')
@@ -1527,25 +1538,25 @@
                      code
                         0x950197008903a00000000000000000000000000000000000000000007c
                         016401a6020000ab02000000000000000001008903a00000000000000000
                         000000000000000000000000007c026402a6020000ab0200000000000000
                         00010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     123           2 RESUME                   0
+                     124           2 RESUME                   0
                      
-                     129           4 LOAD_DEREF               3 (self)
+                     130           4 LOAD_DEREF               3 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                     130          48 LOAD_DEREF               3 (self)
+                     131          48 LOAD_DEREF               3 (self)
                                   50 LOAD_METHOD              0 (assertEqual)
                                   72 LOAD_FAST                2 (p2)
                                   74 LOAD_CONST               2 ('b')
                                   76 PRECALL                  2
                                   80 CALL                     2
                                   90 POP_TOP
                                   92 LOAD_CONST               0 (None)
@@ -1556,27 +1567,27 @@
                         'b'
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1', 'p2')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 123
+                     firstlineno 124
                      lnotab 0x04062c01
                   '/'
                   'a'
                   'b'
                   ('p1', 'p2')
-               names      ('inject_args', 'param_post', 'str', 'factory', 'post')
+               names      ('view', 'param_post', 'str', 'factory', 'post')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_post'
-               firstlineno 122
+               firstlineno 123
                lnotab 0x04011a031a011afd04020cfe02030cfd0aff0e010208
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
                flags     : 3
                code
@@ -1584,38 +1595,38 @@
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
                   000000000000007d0102007c0189006a030000000000000000a004000000
                   00000000000000000000000000000000006403640164046901a6020000ab
                   020000000000000000a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               134           2 RESUME                   0
+               135           2 RESUME                   0
                
-               135           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               136           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-               136          30 LOAD_GLOBAL              3 (NULL + param)
+               137          30 LOAD_GLOBAL              3 (NULL + param)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('p1')
                             60 LOAD_GLOBAL              4 (str)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 135>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 136>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               135          82 PRECALL                  0
+               136          82 PRECALL                  0
                             86 CALL                     0
                
-               136          96 STORE_FAST               1 (viewfn)
+               137          96 STORE_FAST               1 (viewfn)
                
-               139          98 PUSH_NULL
+               140          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
                            102 LOAD_DEREF               0 (self)
                            104 LOAD_ATTR                3 (factory)
                            114 LOAD_METHOD              4 (post)
                            136 LOAD_CONST               3 ('/?p1=a')
                            138 LOAD_CONST               1 ('p1')
                            140 LOAD_CONST               4 ('b')
@@ -1636,17 +1647,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     135           2 RESUME                   0
+                     136           2 RESUME                   0
                      
-                     137           4 LOAD_DEREF               2 (self)
+                     138           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -1656,25 +1667,25 @@
                         'a'
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 135
+                     firstlineno 136
                      lnotab 0x0402
                   '/?p1=a'
                   'b'
-               names      ('inject_args', 'param', 'str', 'factory', 'post')
+               names      ('view', 'param', 'str', 'factory', 'post')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_get_and_post_order'
-               firstlineno 134
+               firstlineno 135
                lnotab 0x04011a0134ff0e010203
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -1682,38 +1693,38 @@
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
                   000000000000007d0102007c0189006a030000000000000000a004000000
                   00000000000000000000000000000000006403a6010000ab010000000000
                   0000006404a6020000ab020000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               141           2 RESUME                   0
+               142           2 RESUME                   0
                
-               142           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               143           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-               143          30 LOAD_GLOBAL              3 (NULL + param)
+               144          30 LOAD_GLOBAL              3 (NULL + param)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('p1')
                             60 LOAD_GLOBAL              4 (str)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 142>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 143>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               142          82 PRECALL                  0
+               143          82 PRECALL                  0
                             86 CALL                     0
                
-               143          96 STORE_FAST               1 (viewfn)
+               144          96 STORE_FAST               1 (viewfn)
                
-               146          98 PUSH_NULL
+               147          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
                            102 LOAD_DEREF               0 (self)
                            104 LOAD_ATTR                3 (factory)
                            114 LOAD_METHOD              4 (get)
                            136 LOAD_CONST               3 ('/?p1=a')
                            138 PRECALL                  1
                            142 CALL                     1
@@ -1732,17 +1743,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     142           2 RESUME                   0
+                     143           2 RESUME                   0
                      
-                     144           4 LOAD_DEREF               2 (self)
+                     145           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('b')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -1752,25 +1763,25 @@
                         'b'
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 142
+                     firstlineno 143
                      lnotab 0x0402
                   '/?p1=a'
                   'b'
-               names      ('inject_args', 'param', 'str', 'factory', 'get')
+               names      ('view', 'param', 'str', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_function_call_arg_overrides_param'
-               firstlineno 141
+               firstlineno 142
                lnotab 0x04011a0134ff0e010203
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -1778,38 +1789,38 @@
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
                   000000000000007d0102007c0189006a030000000000000000a004000000
                   00000000000000000000000000000000006403a6010000ab010000000000
                   0000006404ac05a6020000ab020000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               148           2 RESUME                   0
+               149           2 RESUME                   0
                
-               149           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               150           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-               150          30 LOAD_GLOBAL              3 (NULL + param)
+               151          30 LOAD_GLOBAL              3 (NULL + param)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('p1')
                             60 LOAD_GLOBAL              4 (str)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 149>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 150>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               149          82 PRECALL                  0
+               150          82 PRECALL                  0
                             86 CALL                     0
                
-               150          96 STORE_FAST               1 (viewfn)
+               151          96 STORE_FAST               1 (viewfn)
                
-               153          98 PUSH_NULL
+               154          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
                            102 LOAD_DEREF               0 (self)
                            104 LOAD_ATTR                3 (factory)
                            114 LOAD_METHOD              4 (get)
                            136 LOAD_CONST               3 ('/?p1=a')
                            138 PRECALL                  1
                            142 CALL                     1
@@ -1829,17 +1840,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     149           2 RESUME                   0
+                     150           2 RESUME                   0
                      
-                     151           4 LOAD_DEREF               2 (self)
+                     152           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('b')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -1849,26 +1860,26 @@
                         'b'
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 149
+                     firstlineno 150
                      lnotab 0x0402
                   '/?p1=a'
                   'b'
                   ('p1',)
-               names      ('inject_args', 'param', 'str', 'factory', 'get')
+               names      ('view', 'param', 'str', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_function_call_kwarg_overrides_param'
-               firstlineno 148
+               firstlineno 149
                lnotab 0x04011a0134ff0e010203
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -1876,38 +1887,38 @@
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
                   000000000000007d0102007c0189006a030000000000000000a004000000
                   00000000000000000000000000000000006403a6010000ab010000000000
                   000000a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               155           2 RESUME                   0
+               156           2 RESUME                   0
                
-               156           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               157           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-               157          30 LOAD_GLOBAL              3 (NULL + param)
+               158          30 LOAD_GLOBAL              3 (NULL + param)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('p1')
                             60 LOAD_GLOBAL              4 (str)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 156>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 157>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               156          82 PRECALL                  0
+               157          82 PRECALL                  0
                             86 CALL                     0
                
-               157          96 STORE_FAST               1 (viewfn)
+               158          96 STORE_FAST               1 (viewfn)
                
-               161          98 PUSH_NULL
+               162          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
                            102 LOAD_DEREF               0 (self)
                            104 LOAD_ATTR                3 (factory)
                            114 LOAD_METHOD              4 (get)
                            136 LOAD_CONST               3 ('/?p1=a')
                            138 PRECALL                  1
                            142 CALL                     1
@@ -1927,25 +1938,25 @@
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab02000000000000000001008902a00100000000000000
                         0000000000000000000000000064027c006a020000000000000000a60200
                         00ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     156           2 RESUME                   0
+                     157           2 RESUME                   0
                      
-                     158           4 LOAD_DEREF               2 (self)
+                     159           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                     159          48 LOAD_DEREF               2 (self)
+                     160          48 LOAD_DEREF               2 (self)
                                   50 LOAD_METHOD              1 (assertNotIn)
                                   72 LOAD_CONST               2 ('p1')
                                   74 LOAD_FAST                0 (request)
                                   76 LOAD_ATTR                2 (GET)
                                   86 PRECALL                  2
                                   90 CALL                     2
                                  100 POP_TOP
@@ -1957,24 +1968,24 @@
                         'p1'
                      names      ('assertEqual', 'assertNotIn', 'GET')
                      varnames   ('request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 156
+                     firstlineno 157
                      lnotab 0x04022c01
                   '/?p1=a'
-               names      ('inject_args', 'param', 'str', 'factory', 'get')
+               names      ('view', 'param', 'str', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_param_consume_true'
-               firstlineno 155
+               firstlineno 156
                lnotab 0x04011a0134ff0e010204
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -1982,40 +1993,40 @@
                   007403000000000000000000006401ac02a6010000ab0100000000000000
                   00660164037404000000000000000000006602880066016404840da60000
                   00ab0000000000000000007d0102007c0189006a030000000000000000a0
                   0400000000000000000000000000000000000000006405a6010000ab0100
                   00000000000000a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               163           2 RESUME                   0
+               164           2 RESUME                   0
                
-               164           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               165           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-               165          30 LOAD_GLOBAL              3 (NULL + param)
+               166          30 LOAD_GLOBAL              3 (NULL + param)
                             42 LOAD_CONST               1 (False)
                             44 KW_NAMES                 2
                             46 PRECALL                  1
                             50 CALL                     1
                             60 BUILD_TUPLE              1
                             62 LOAD_CONST               3 ('p1')
                             64 LOAD_GLOBAL              4 (str)
                             76 BUILD_TUPLE              2
                             78 LOAD_CLOSURE             0 (self)
                             80 BUILD_TUPLE              1
-                            82 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 164>)
+                            82 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 165>)
                             84 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               164          86 PRECALL                  0
+               165          86 PRECALL                  0
                             90 CALL                     0
                
-               165         100 STORE_FAST               1 (viewfn)
+               166         100 STORE_FAST               1 (viewfn)
                
-               169         102 PUSH_NULL
+               170         102 PUSH_NULL
                            104 LOAD_FAST                1 (viewfn)
                            106 LOAD_DEREF               0 (self)
                            108 LOAD_ATTR                3 (factory)
                            118 LOAD_METHOD              4 (get)
                            140 LOAD_CONST               5 ('/?p1=a')
                            142 PRECALL                  1
                            146 CALL                     1
@@ -2037,25 +2048,25 @@
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab02000000000000000001008902a00100000000000000
                         0000000000000000000000000064027c006a020000000000000000a60200
                         00ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     164           2 RESUME                   0
+                     165           2 RESUME                   0
                      
-                     166           4 LOAD_DEREF               2 (self)
+                     167           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                     167          48 LOAD_DEREF               2 (self)
+                     168          48 LOAD_DEREF               2 (self)
                                   50 LOAD_METHOD              1 (assertIn)
                                   72 LOAD_CONST               2 ('p1')
                                   74 LOAD_FAST                0 (request)
                                   76 LOAD_ATTR                2 (GET)
                                   86 PRECALL                  2
                                   90 CALL                     2
                                  100 POP_TOP
@@ -2067,24 +2078,24 @@
                         'p1'
                      names      ('assertEqual', 'assertIn', 'GET')
                      varnames   ('request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 164
+                     firstlineno 165
                      lnotab 0x04022c01
                   '/?p1=a'
-               names      ('inject_args', 'param', 'str', 'factory', 'get')
+               names      ('view', 'param', 'str', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_param_consume_false'
-               firstlineno 163
+               firstlineno 164
                lnotab 0x04011a0138ff0e010204
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -2092,38 +2103,38 @@
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
                   000000000000007d0102007c0189006a030000000000000000a004000000
                   00000000000000000000000000000000006403a6010000ab010000000000
                   000000a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               171           2 RESUME                   0
+               172           2 RESUME                   0
                
-               172           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               173           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-               173          30 LOAD_GLOBAL              3 (NULL + param_get)
+               174          30 LOAD_GLOBAL              3 (NULL + param_get)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('p1')
                             60 LOAD_GLOBAL              4 (str)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 172>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 173>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               172          82 PRECALL                  0
+               173          82 PRECALL                  0
                             86 CALL                     0
                
-               173          96 STORE_FAST               1 (viewfn)
+               174          96 STORE_FAST               1 (viewfn)
                
-               177          98 PUSH_NULL
+               178          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
                            102 LOAD_DEREF               0 (self)
                            104 LOAD_ATTR                3 (factory)
                            114 LOAD_METHOD              4 (get)
                            136 LOAD_CONST               3 ('/?p1=a')
                            138 PRECALL                  1
                            142 CALL                     1
@@ -2143,25 +2154,25 @@
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab02000000000000000001008902a00100000000000000
                         0000000000000000000000000064027c006a020000000000000000a60200
                         00ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     172           2 RESUME                   0
+                     173           2 RESUME                   0
                      
-                     174           4 LOAD_DEREF               2 (self)
+                     175           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                     175          48 LOAD_DEREF               2 (self)
+                     176          48 LOAD_DEREF               2 (self)
                                   50 LOAD_METHOD              1 (assertNotIn)
                                   72 LOAD_CONST               2 ('p1')
                                   74 LOAD_FAST                0 (request)
                                   76 LOAD_ATTR                2 (GET)
                                   86 PRECALL                  2
                                   90 CALL                     2
                                  100 POP_TOP
@@ -2173,24 +2184,24 @@
                         'p1'
                      names      ('assertEqual', 'assertNotIn', 'GET')
                      varnames   ('request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 172
+                     firstlineno 173
                      lnotab 0x04022c01
                   '/?p1=a'
-               names      ('inject_args', 'param_get', 'str', 'factory', 'get')
+               names      ('view', 'param_get', 'str', 'factory', 'get')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_param_consume_get'
-               firstlineno 171
+               firstlineno 172
                lnotab 0x04011a0134ff0e010204
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
                flags     : 3
                code
@@ -2198,38 +2209,38 @@
                   00740300000000000000000000a6000000ab000000000000000000660164
                   017404000000000000000000006602880066016402840da6000000ab0000
                   000000000000007d0102007c0189006a030000000000000000a004000000
                   00000000000000000000000000000000006403640164046901a6020000ab
                   020000000000000000a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               179           2 RESUME                   0
+               180           2 RESUME                   0
                
-               180           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               181           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-               181          30 LOAD_GLOBAL              3 (NULL + param_post)
+               182          30 LOAD_GLOBAL              3 (NULL + param_post)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 BUILD_TUPLE              1
                             58 LOAD_CONST               1 ('p1')
                             60 LOAD_GLOBAL              4 (str)
                             72 BUILD_TUPLE              2
                             74 LOAD_CLOSURE             0 (self)
                             76 BUILD_TUPLE              1
-                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 180>)
+                            78 LOAD_CONST               2 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 181>)
                             80 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               180          82 PRECALL                  0
+               181          82 PRECALL                  0
                             86 CALL                     0
                
-               181          96 STORE_FAST               1 (viewfn)
+               182          96 STORE_FAST               1 (viewfn)
                
-               185          98 PUSH_NULL
+               186          98 PUSH_NULL
                            100 LOAD_FAST                1 (viewfn)
                            102 LOAD_DEREF               0 (self)
                            104 LOAD_ATTR                3 (factory)
                            114 LOAD_METHOD              4 (post)
                            136 LOAD_CONST               3 ('/')
                            138 LOAD_CONST               1 ('p1')
                            140 LOAD_CONST               4 ('a')
@@ -2252,25 +2263,25 @@
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab02000000000000000001008902a00100000000000000
                         0000000000000000000000000064027c006a020000000000000000a60200
                         00ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     180           2 RESUME                   0
+                     181           2 RESUME                   0
                      
-                     182           4 LOAD_DEREF               2 (self)
+                     183           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                     183          48 LOAD_DEREF               2 (self)
+                     184          48 LOAD_DEREF               2 (self)
                                   50 LOAD_METHOD              1 (assertNotIn)
                                   72 LOAD_CONST               2 ('p1')
                                   74 LOAD_FAST                0 (request)
                                   76 LOAD_ATTR                2 (POST)
                                   86 PRECALL                  2
                                   90 CALL                     2
                                  100 POP_TOP
@@ -2282,25 +2293,25 @@
                         'p1'
                      names      ('assertEqual', 'assertNotIn', 'POST')
                      varnames   ('request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 180
+                     firstlineno 181
                      lnotab 0x04022c01
                   '/'
                   'a'
-               names      ('inject_args', 'param_post', 'str', 'factory', 'post')
+               names      ('view', 'param_post', 'str', 'factory', 'post')
                varnames   ('self', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_param_consume_post'
-               firstlineno 179
+               firstlineno 180
                lnotab 0x04011a0134ff0e010204
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
@@ -2310,48 +2321,48 @@
                   00ab0000000000000000007d017407000000000000000000006a04000000
                   0000000000740a000000000000000000007c01a6020000ab020000000000
                   0000007d0202007c0289006a060000000000000000a00700000000000000
                   000000000000000000000000006405a6010000ab010000000000000000a6
                   010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               187           2 RESUME                   0
+               188           2 RESUME                   0
                
-               188           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               189           4 LOAD_GLOBAL              1 (NULL + view)
                             16 PRECALL                  0
                             20 CALL                     0
                
-               189          30 LOAD_GLOBAL              3 (NULL + param)
+               190          30 LOAD_GLOBAL              3 (NULL + param)
                             42 LOAD_CONST               1 ('a')
                             44 KW_NAMES                 2
                             46 PRECALL                  1
                             50 CALL                     1
                             60 BUILD_TUPLE              1
                             62 LOAD_CONST               3 ('p1')
                             64 LOAD_GLOBAL              4 (str)
                             76 BUILD_TUPLE              2
                             78 LOAD_CLOSURE             0 (self)
                             80 BUILD_TUPLE              1
-                            82 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 188>)
+                            82 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 189>)
                             84 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               188          86 PRECALL                  0
+               189          86 PRECALL                  0
                             90 CALL                     0
                
-               189         100 STORE_FAST               1 (viewfn)
+               190         100 STORE_FAST               1 (viewfn)
                
-               192         102 LOAD_GLOBAL              7 (NULL + typing)
+               193         102 LOAD_GLOBAL              7 (NULL + typing)
                            114 LOAD_ATTR                4 (cast)
                            124 LOAD_GLOBAL             10 (Any)
                            136 LOAD_FAST                1 (viewfn)
                            138 PRECALL                  2
                            142 CALL                     2
                            152 STORE_FAST               2 (untyped_viewfn)
                
-               193         154 PUSH_NULL
+               194         154 PUSH_NULL
                            156 LOAD_FAST                2 (untyped_viewfn)
                            158 LOAD_DEREF               0 (self)
                            160 LOAD_ATTR                6 (factory)
                            170 LOAD_METHOD              7 (get)
                            192 LOAD_CONST               5 ('/')
                            194 PRECALL                  1
                            198 CALL                     1
@@ -2371,17 +2382,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     188           2 RESUME                   0
+                     189           2 RESUME                   0
                      
-                     190           4 LOAD_DEREF               2 (self)
+                     191           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -2391,24 +2402,24 @@
                         'a'
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 188
+                     firstlineno 189
                      lnotab 0x0402
                   '/'
-               names      ('inject_args', 'param', 'str', 'typing', 'cast', 'Any', 'factory', 'get')
+               names      ('view', 'param', 'str', 'typing', 'cast', 'Any', 'factory', 'get')
                varnames   ('self', 'viewfn', 'untyped_viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_auto_default_value'
-               firstlineno 187
+               firstlineno 188
                lnotab 0x04011a0138ff0e0102033401
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
@@ -2418,58 +2429,58 @@
                   0300000000000000007408000000000000000000007c01a6020000ab0200
                   000000000000008a03880088036602640584087d028900a0050000000000
                   000000000000000000000000000000740c0000000000000000000064067c
                   02a6030000ab030000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                3 (untyped_viewfn)
                
-               195           4 RESUME                   0
+               196           4 RESUME                   0
                
-               196           6 LOAD_GLOBAL              1 (NULL + inject_args)
+               197           6 LOAD_GLOBAL              1 (NULL + inject_args)
                             18 LOAD_CONST               1 (False)
                             20 KW_NAMES                 2
                             22 PRECALL                  1
                             26 CALL                     1
                
-               197          36 LOAD_CONST               3 ('p1')
+               198          36 LOAD_CONST               3 ('p1')
                             38 LOAD_GLOBAL              2 (str)
                             50 BUILD_TUPLE              2
                             52 LOAD_CLOSURE             0 (self)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 196>)
+                            56 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 197>)
                             58 MAKE_FUNCTION           12 (annotations, closure)
                
-               196          60 PRECALL                  0
+               197          60 PRECALL                  0
                             64 CALL                     0
                
-               197          74 STORE_FAST               1 (viewfn)
+               198          74 STORE_FAST               1 (viewfn)
                
-               200          76 LOAD_GLOBAL              5 (NULL + typing)
+               201          76 LOAD_GLOBAL              5 (NULL + typing)
                             88 LOAD_ATTR                3 (cast)
                             98 LOAD_GLOBAL              8 (Any)
                            110 LOAD_FAST                1 (viewfn)
                            112 PRECALL                  2
                            116 CALL                     2
                            126 STORE_DEREF              3 (untyped_viewfn)
                
-               202         128 LOAD_CLOSURE             0 (self)
+               203         128 LOAD_CLOSURE             0 (self)
                            130 LOAD_CLOSURE             3 (untyped_viewfn)
                            132 BUILD_TUPLE              2
-                           134 LOAD_CONST               5 (<code object test, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 202>)
+                           134 LOAD_CONST               5 (<code object test, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 203>)
                            136 MAKE_FUNCTION            8 (closure)
                            138 STORE_FAST               2 (test)
                
-               205         140 LOAD_DEREF               0 (self)
+               206         140 LOAD_DEREF               0 (self)
                            142 LOAD_METHOD              5 (assertRaisesRegex)
                
-               206         164 LOAD_GLOBAL             12 (Exception)
+               207         164 LOAD_GLOBAL             12 (Exception)
                            176 LOAD_CONST               6 ("missing 1 required positional argument: 'p1'")
                            178 LOAD_FAST                2 (test)
                
-               205         180 PRECALL                  3
+               206         180 PRECALL                  3
                            184 CALL                     3
                            194 POP_TOP
                            196 LOAD_CONST               0 (None)
                            198 RETURN_VALUE
                consts
                   None
                   False
@@ -2481,17 +2492,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     196           2 RESUME                   0
+                     197           2 RESUME                   0
                      
-                     198           4 LOAD_DEREF               2 (self)
+                     199           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -2501,30 +2512,30 @@
                         'a'
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 196
+                     firstlineno 197
                      lnotab 0x0402
                   code
                      argcount  : 0
                      nlocals   : 0
                      stacksize : 5
                      flags     : 19
                      code
                         0x950297000200890189006a000000000000000000a00100000000000000
                         000000000000000000000000006401a6010000ab010000000000000000a6
                         010000ab010000000000000000010064005300
                                    0 COPY_FREE_VARS           2
                      
-                     202           2 RESUME                   0
+                     203           2 RESUME                   0
                      
-                     203           4 PUSH_NULL
+                     204           4 PUSH_NULL
                                    6 LOAD_DEREF               1 (untyped_viewfn)
                                    8 LOAD_DEREF               0 (self)
                                   10 LOAD_ATTR                0 (factory)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('/?p1=a')
                                   44 PRECALL                  1
                                   48 CALL                     1
@@ -2538,24 +2549,24 @@
                         '/?p1=a'
                      names      ('factory', 'get')
                      varnames   ()
                      freevars   ('self', 'untyped_viewfn')
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'test'
-                     firstlineno 202
+                     firstlineno 203
                      lnotab 0x0401
                   "missing 1 required positional argument: 'p1'"
                names      ('inject_args', 'str', 'typing', 'cast', 'Any', 'assertRaisesRegex', 'Exception')
                varnames   ('self', 'viewfn', 'test')
                freevars   ()
                cellvars   ('self', 'untyped_viewfn')
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_auto_param_false'
-               firstlineno 195
+               firstlineno 196
                lnotab 0x06011e0118ff0e01020334020c03180110ff
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
@@ -2564,44 +2575,44 @@
                   000000ab0000000000000000007d017405000000000000000000006a0300
                   000000000000007408000000000000000000007c01a6020000ab02000000
                   00000000007d0202007c0289006a050000000000000000a0060000000000
                   0000000000000000000000000000006405a6010000ab0100000000000000
                   00a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               209           2 RESUME                   0
+               210           2 RESUME                   0
                
-               210           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               211           4 LOAD_GLOBAL              1 (NULL + inject_args)
                             16 LOAD_CONST               1 (True)
                             18 KW_NAMES                 2
                             20 PRECALL                  1
                             24 CALL                     1
                
-               211          34 LOAD_CONST               3 ('p1')
+               212          34 LOAD_CONST               3 ('p1')
                             36 LOAD_GLOBAL              2 (str)
                             48 BUILD_TUPLE              2
                             50 LOAD_CLOSURE             0 (self)
                             52 BUILD_TUPLE              1
-                            54 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 210>)
+                            54 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 211>)
                             56 MAKE_FUNCTION           12 (annotations, closure)
                
-               210          58 PRECALL                  0
+               211          58 PRECALL                  0
                             62 CALL                     0
                
-               211          72 STORE_FAST               1 (viewfn)
+               212          72 STORE_FAST               1 (viewfn)
                
-               214          74 LOAD_GLOBAL              5 (NULL + typing)
+               215          74 LOAD_GLOBAL              5 (NULL + typing)
                             86 LOAD_ATTR                3 (cast)
                             96 LOAD_GLOBAL              8 (Any)
                            108 LOAD_FAST                1 (viewfn)
                            110 PRECALL                  2
                            114 CALL                     2
                            124 STORE_FAST               2 (untyped_viewfn)
                
-               215         126 PUSH_NULL
+               216         126 PUSH_NULL
                            128 LOAD_FAST                2 (untyped_viewfn)
                            130 LOAD_DEREF               0 (self)
                            132 LOAD_ATTR                5 (factory)
                            142 LOAD_METHOD              6 (get)
                            164 LOAD_CONST               5 ('/?p1=a')
                            166 PRECALL                  1
                            170 CALL                     1
@@ -2621,17 +2632,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     210           2 RESUME                   0
+                     211           2 RESUME                   0
                      
-                     212           4 LOAD_DEREF               2 (self)
+                     213           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -2641,24 +2652,24 @@
                         'a'
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 210
+                     firstlineno 211
                      lnotab 0x0402
                   '/?p1=a'
                names      ('inject_args', 'str', 'typing', 'cast', 'Any', 'factory', 'get')
                varnames   ('self', 'viewfn', 'untyped_viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_auto_param_true'
-               firstlineno 209
+               firstlineno 210
                lnotab 0x04011e0118ff0e0102033401
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
@@ -2667,44 +2678,44 @@
                   000000ab0000000000000000007d017405000000000000000000006a0300
                   000000000000007408000000000000000000007c01a6020000ab02000000
                   00000000007d0202007c0289006a050000000000000000a0060000000000
                   0000000000000000000000000000006405a6010000ab0100000000000000
                   00a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               217           2 RESUME                   0
+               218           2 RESUME                   0
                
-               218           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               219           4 LOAD_GLOBAL              1 (NULL + inject_args)
                             16 LOAD_CONST               1 ('get')
                             18 KW_NAMES                 2
                             20 PRECALL                  1
                             24 CALL                     1
                
-               219          34 LOAD_CONST               3 ('p1')
+               220          34 LOAD_CONST               3 ('p1')
                             36 LOAD_GLOBAL              2 (str)
                             48 BUILD_TUPLE              2
                             50 LOAD_CLOSURE             0 (self)
                             52 BUILD_TUPLE              1
-                            54 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 218>)
+                            54 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 219>)
                             56 MAKE_FUNCTION           12 (annotations, closure)
                
-               218          58 PRECALL                  0
+               219          58 PRECALL                  0
                             62 CALL                     0
                
-               219          72 STORE_FAST               1 (viewfn)
+               220          72 STORE_FAST               1 (viewfn)
                
-               222          74 LOAD_GLOBAL              5 (NULL + typing)
+               223          74 LOAD_GLOBAL              5 (NULL + typing)
                             86 LOAD_ATTR                3 (cast)
                             96 LOAD_GLOBAL              8 (Any)
                            108 LOAD_FAST                1 (viewfn)
                            110 PRECALL                  2
                            114 CALL                     2
                            124 STORE_FAST               2 (untyped_viewfn)
                
-               223         126 PUSH_NULL
+               224         126 PUSH_NULL
                            128 LOAD_FAST                2 (untyped_viewfn)
                            130 LOAD_DEREF               0 (self)
                            132 LOAD_ATTR                5 (factory)
                            142 LOAD_METHOD              6 (get)
                            164 LOAD_CONST               5 ('/?p1=a')
                            166 PRECALL                  1
                            170 CALL                     1
@@ -2724,17 +2735,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     218           2 RESUME                   0
+                     219           2 RESUME                   0
                      
-                     220           4 LOAD_DEREF               2 (self)
+                     221           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -2744,24 +2755,24 @@
                         'a'
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 218
+                     firstlineno 219
                      lnotab 0x0402
                   '/?p1=a'
                names      ('inject_args', 'str', 'typing', 'cast', 'Any', 'factory', 'get')
                varnames   ('self', 'viewfn', 'untyped_viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_auto_param_get'
-               firstlineno 217
+               firstlineno 218
                lnotab 0x04011e0118ff0e0102033401
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 7
                flags     : 3
                code
@@ -2770,45 +2781,45 @@
                   0da6000000ab0000000000000000007d017405000000000000000000006a
                   0300000000000000007408000000000000000000007c01a6020000ab0200
                   000000000000007d0202007c0289006a050000000000000000a006000000
                   00000000000000000000000000000000006406640764086901a6020000ab
                   020000000000000000a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               225           2 RESUME                   0
+               226           2 RESUME                   0
                
-               226           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               227           4 LOAD_GLOBAL              1 (NULL + inject_args)
                             16 LOAD_CONST               1 ('get')
                             18 KW_NAMES                 2
                             20 PRECALL                  1
                             24 CALL                     1
                
-               227          34 LOAD_CONST               9 (('b',))
+               228          34 LOAD_CONST               9 (('b',))
                             36 LOAD_CONST               4 ('p1')
                             38 LOAD_GLOBAL              2 (str)
                             50 BUILD_TUPLE              2
                             52 LOAD_CLOSURE             0 (self)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               5 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 226>)
+                            56 LOAD_CONST               5 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 227>)
                             58 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               226          60 PRECALL                  0
+               227          60 PRECALL                  0
                             64 CALL                     0
                
-               227          74 STORE_FAST               1 (viewfn)
+               228          74 STORE_FAST               1 (viewfn)
                
-               231          76 LOAD_GLOBAL              5 (NULL + typing)
+               232          76 LOAD_GLOBAL              5 (NULL + typing)
                             88 LOAD_ATTR                3 (cast)
                             98 LOAD_GLOBAL              8 (Any)
                            110 LOAD_FAST                1 (viewfn)
                            112 PRECALL                  2
                            116 CALL                     2
                            126 STORE_FAST               2 (untyped_viewfn)
                
-               232         128 PUSH_NULL
+               233         128 PUSH_NULL
                            130 LOAD_FAST                2 (untyped_viewfn)
                            132 LOAD_DEREF               0 (self)
                            134 LOAD_ATTR                5 (factory)
                            144 LOAD_METHOD              6 (post)
                            166 LOAD_CONST               6 ('/?p1=a')
                            168 LOAD_CONST               7 ('p2')
                            170 LOAD_CONST               8 ('x')
@@ -2834,25 +2845,25 @@
                      code
                         0x950197008903a00000000000000000000000000000000000000000007c
                         016401a6020000ab02000000000000000001008903a00000000000000000
                         000000000000000000000000007c026402a6020000ab0200000000000000
                         00010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     226           2 RESUME                   0
+                     227           2 RESUME                   0
                      
-                     228           4 LOAD_DEREF               3 (self)
+                     229           4 LOAD_DEREF               3 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                     229          48 LOAD_DEREF               3 (self)
+                     230          48 LOAD_DEREF               3 (self)
                                   50 LOAD_METHOD              0 (assertEqual)
                                   72 LOAD_FAST                2 (p2)
                                   74 LOAD_CONST               2 ('b')
                                   76 PRECALL                  2
                                   80 CALL                     2
                                   90 POP_TOP
                                   92 LOAD_CONST               0 (None)
@@ -2863,27 +2874,27 @@
                         'b'
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1', 'p2')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 226
+                     firstlineno 227
                      lnotab 0x04022c01
                   '/?p1=a'
                   'p2'
                   'x'
                   ('b',)
                names      ('inject_args', 'str', 'typing', 'cast', 'Any', 'factory', 'post')
                varnames   ('self', 'viewfn', 'untyped_viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_auto_param_get_does_not_receive_post_params'
-               firstlineno 225
+               firstlineno 226
                lnotab 0x04011e011aff0e0102043401
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 7
                flags     : 3
                code
@@ -2892,44 +2903,44 @@
                   000000ab0000000000000000007d017405000000000000000000006a0300
                   000000000000007408000000000000000000007c01a6020000ab02000000
                   00000000007d0202007c0289006a050000000000000000a0060000000000
                   0000000000000000000000000000006405640364066901a6020000ab0200
                   00000000000000a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               234           2 RESUME                   0
+               235           2 RESUME                   0
                
-               235           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               236           4 LOAD_GLOBAL              1 (NULL + inject_args)
                             16 LOAD_CONST               1 ('post')
                             18 KW_NAMES                 2
                             20 PRECALL                  1
                             24 CALL                     1
                
-               236          34 LOAD_CONST               3 ('p1')
+               237          34 LOAD_CONST               3 ('p1')
                             36 LOAD_GLOBAL              2 (str)
                             48 BUILD_TUPLE              2
                             50 LOAD_CLOSURE             0 (self)
                             52 BUILD_TUPLE              1
-                            54 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 235>)
+                            54 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 236>)
                             56 MAKE_FUNCTION           12 (annotations, closure)
                
-               235          58 PRECALL                  0
+               236          58 PRECALL                  0
                             62 CALL                     0
                
-               236          72 STORE_FAST               1 (viewfn)
+               237          72 STORE_FAST               1 (viewfn)
                
-               239          74 LOAD_GLOBAL              5 (NULL + typing)
+               240          74 LOAD_GLOBAL              5 (NULL + typing)
                             86 LOAD_ATTR                3 (cast)
                             96 LOAD_GLOBAL              8 (Any)
                            108 LOAD_FAST                1 (viewfn)
                            110 PRECALL                  2
                            114 CALL                     2
                            124 STORE_FAST               2 (untyped_viewfn)
                
-               240         126 PUSH_NULL
+               241         126 PUSH_NULL
                            128 LOAD_FAST                2 (untyped_viewfn)
                            130 LOAD_DEREF               0 (self)
                            132 LOAD_ATTR                5 (factory)
                            142 LOAD_METHOD              6 (post)
                            164 LOAD_CONST               5 ('/')
                            166 LOAD_CONST               3 ('p1')
                            168 LOAD_CONST               6 ('a')
@@ -2952,17 +2963,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a00000000000000000000000000000000000000000007c
                         016401a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     235           2 RESUME                   0
+                     236           2 RESUME                   0
                      
-                     237           4 LOAD_DEREF               2 (self)
+                     238           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -2972,25 +2983,25 @@
                         'a'
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 235
+                     firstlineno 236
                      lnotab 0x0402
                   '/'
                   'a'
                names      ('inject_args', 'str', 'typing', 'cast', 'Any', 'factory', 'post')
                varnames   ('self', 'viewfn', 'untyped_viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_auto_param_post'
-               firstlineno 234
+               firstlineno 235
                lnotab 0x04011e0118ff0e0102033401
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 7
                flags     : 3
                code
@@ -2999,45 +3010,45 @@
                   0da6000000ab0000000000000000007d017405000000000000000000006a
                   0300000000000000007408000000000000000000007c01a6020000ab0200
                   000000000000007d0202007c0289006a050000000000000000a006000000
                   00000000000000000000000000000000006406640464076901a6020000ab
                   020000000000000000a6010000ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               242           2 RESUME                   0
+               243           2 RESUME                   0
                
-               243           4 LOAD_GLOBAL              1 (NULL + inject_args)
+               244           4 LOAD_GLOBAL              1 (NULL + inject_args)
                             16 LOAD_CONST               1 ('post')
                             18 KW_NAMES                 2
                             20 PRECALL                  1
                             24 CALL                     1
                
-               244          34 LOAD_CONST               8 (('b',))
+               245          34 LOAD_CONST               8 (('b',))
                             36 LOAD_CONST               4 ('p1')
                             38 LOAD_GLOBAL              2 (str)
                             50 BUILD_TUPLE              2
                             52 LOAD_CLOSURE             0 (self)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               5 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 243>)
+                            56 LOAD_CONST               5 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 244>)
                             58 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               243          60 PRECALL                  0
+               244          60 PRECALL                  0
                             64 CALL                     0
                
-               244          74 STORE_FAST               1 (viewfn)
+               245          74 STORE_FAST               1 (viewfn)
                
-               248          76 LOAD_GLOBAL              5 (NULL + typing)
+               249          76 LOAD_GLOBAL              5 (NULL + typing)
                             88 LOAD_ATTR                3 (cast)
                             98 LOAD_GLOBAL              8 (Any)
                            110 LOAD_FAST                1 (viewfn)
                            112 PRECALL                  2
                            116 CALL                     2
                            126 STORE_FAST               2 (untyped_viewfn)
                
-               249         128 PUSH_NULL
+               250         128 PUSH_NULL
                            130 LOAD_FAST                2 (untyped_viewfn)
                            132 LOAD_DEREF               0 (self)
                            134 LOAD_ATTR                5 (factory)
                            144 LOAD_METHOD              6 (post)
                            166 LOAD_CONST               6 ('/p2=x')
                            168 LOAD_CONST               4 ('p1')
                            170 LOAD_CONST               7 ('a')
@@ -3063,25 +3074,25 @@
                      code
                         0x950197008903a00000000000000000000000000000000000000000007c
                         016401a6020000ab02000000000000000001008903a00000000000000000
                         000000000000000000000000007c026402a6020000ab0200000000000000
                         00010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     243           2 RESUME                   0
+                     244           2 RESUME                   0
                      
-                     245           4 LOAD_DEREF               3 (self)
+                     246           4 LOAD_DEREF               3 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_FAST                1 (p1)
                                   30 LOAD_CONST               1 ('a')
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                      
-                     246          48 LOAD_DEREF               3 (self)
+                     247          48 LOAD_DEREF               3 (self)
                                   50 LOAD_METHOD              0 (assertEqual)
                                   72 LOAD_FAST                2 (p2)
                                   74 LOAD_CONST               2 ('b')
                                   76 PRECALL                  2
                                   80 CALL                     2
                                   90 POP_TOP
                                   92 LOAD_CONST               0 (None)
@@ -3092,126 +3103,124 @@
                         'b'
                      names      ('assertEqual',)
                      varnames   ('_request', 'p1', 'p2')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 243
+                     firstlineno 244
                      lnotab 0x04022c01
                   '/p2=x'
                   'a'
                   ('b',)
                names      ('inject_args', 'str', 'typing', 'cast', 'Any', 'factory', 'post')
                varnames   ('self', 'viewfn', 'untyped_viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_auto_param_post_does_not_receive_get_params'
-               firstlineno 242
+               firstlineno 243
                lnotab 0x04011e011aff0e0102043401
             code
                argcount  : 1
                nlocals   : 3
-               stacksize : 8
+               stacksize : 9
                flags     : 3
                code
                   0x870087039700020047006401840064027400000000000000000000006a
                   010000000000000000a6030000ab0300000000000000008a037405000000
                   00000000000000a6000000ab000000000000000000640389036602880388
                   0066026404840ca6000000ab0000000000000000007d0174070000000000
                   00000000006a040000000000000000740a000000000000000000007c01a6
-                  020000ab0200000000000000007d0202007c0289006a0600000000000000
-                  00a007000000000000000000000000000000000000000064056406640764
-                  089c02a6020000ab020000000000000000a6010000ab0100000000000000
-                  00010064005300
+                  020000ab0200000000000000007d0202007c02740d000000000000000000
+                  007c0164056406640764089c02a6030000ab030000000000000000a60100
+                  00ab010000000000000000010064005300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                3 (TestForm)
                
-               251           4 RESUME                   0
+               252           4 RESUME                   0
                
-               252           6 PUSH_NULL
+               253           6 PUSH_NULL
                              8 LOAD_BUILD_CLASS
-                            10 LOAD_CONST               1 (<code object TestForm, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 252>)
+                            10 LOAD_CONST               1 (<code object TestForm, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 253>)
                             12 MAKE_FUNCTION            0
                             14 LOAD_CONST               2 ('TestForm')
                             16 LOAD_GLOBAL              0 (forms)
                             28 LOAD_ATTR                1 (Form)
                             38 PRECALL                  3
                             42 CALL                     3
                             52 STORE_DEREF              3 (TestForm)
                
-               256          54 LOAD_GLOBAL              5 (NULL + inject_args)
+               257          54 LOAD_GLOBAL              5 (NULL + view)
                             66 PRECALL                  0
                             70 CALL                     0
                
-               257          80 LOAD_CONST               3 ('form')
+               258          80 LOAD_CONST               3 ('form')
                             82 LOAD_DEREF               3 (TestForm)
                             84 BUILD_TUPLE              2
                             86 LOAD_CLOSURE             3 (TestForm)
                             88 LOAD_CLOSURE             0 (self)
                             90 BUILD_TUPLE              2
-                            92 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 256>)
+                            92 LOAD_CONST               4 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 257>)
                             94 MAKE_FUNCTION           12 (annotations, closure)
                
-               256          96 PRECALL                  0
+               257          96 PRECALL                  0
                            100 CALL                     0
                
-               257         110 STORE_FAST               1 (viewfn)
+               258         110 STORE_FAST               1 (viewfn)
                
-               260         112 LOAD_GLOBAL              7 (NULL + typing)
+               261         112 LOAD_GLOBAL              7 (NULL + typing)
                            124 LOAD_ATTR                4 (cast)
                            134 LOAD_GLOBAL             10 (Any)
                            146 LOAD_FAST                1 (viewfn)
                            148 PRECALL                  2
                            152 CALL                     2
                            162 STORE_FAST               2 (untyped_viewfn)
                
-               261         164 PUSH_NULL
+               262         164 PUSH_NULL
                            166 LOAD_FAST                2 (untyped_viewfn)
-                           168 LOAD_DEREF               0 (self)
-                           170 LOAD_ATTR                6 (factory)
-                           180 LOAD_METHOD              7 (post)
-                           202 LOAD_CONST               5 ('/')
-                           204 LOAD_CONST               6 ('a')
-                           206 LOAD_CONST               7 ('b')
-                           208 LOAD_CONST               8 (('p1', 'p2'))
-                           210 BUILD_CONST_KEY_MAP      2
-                           212 PRECALL                  2
-                           216 CALL                     2
-                           226 PRECALL                  1
-                           230 CALL                     1
-                           240 POP_TOP
-                           242 LOAD_CONST               0 (None)
-                           244 RETURN_VALUE
+                           168 LOAD_GLOBAL             13 (NULL + create_resolved_request)
+                           180 LOAD_FAST                1 (viewfn)
+                           182 LOAD_CONST               5 ('POST')
+                           184 LOAD_CONST               6 ('a')
+                           186 LOAD_CONST               7 ('b')
+                           188 LOAD_CONST               8 (('p1', 'p2'))
+                           190 BUILD_CONST_KEY_MAP      2
+                           192 PRECALL                  3
+                           196 CALL                     3
+                           206 PRECALL                  1
+                           210 CALL                     1
+                           220 POP_TOP
+                           222 LOAD_CONST               0 (None)
+                           224 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 0
                      nlocals   : 0
                      stacksize : 2
                      flags     : 0
                      code
                         0x970065005a0164005a02020065036a040000000000000000a6000000ab
                         0000000000000000005a05020065036a040000000000000000a6000000ab
                         0000000000000000005a0664015300
-                     252           0 RESUME                   0
+                     253           0 RESUME                   0
                                    2 LOAD_NAME                0 (__name__)
                                    4 STORE_NAME               1 (__module__)
                                    6 LOAD_CONST               0 ('ParamsToArgsDecoratorTestCase.test_auto_param_form.<locals>.TestForm')
                                    8 STORE_NAME               2 (__qualname__)
                      
-                     253          10 PUSH_NULL
+                     254          10 PUSH_NULL
                                   12 LOAD_NAME                3 (forms)
                                   14 LOAD_ATTR                4 (TextInput)
                                   24 PRECALL                  0
                                   28 CALL                     0
                                   38 STORE_NAME               5 (p1)
                      
-                     254          40 PUSH_NULL
+                     255          40 PUSH_NULL
                                   42 LOAD_NAME                3 (forms)
                                   44 LOAD_ATTR                4 (TextInput)
                                   54 PRECALL                  0
                                   58 CALL                     0
                                   68 STORE_NAME               6 (p2)
                                   70 LOAD_CONST               1 (None)
                                   72 RETURN_VALUE
@@ -3220,32 +3229,32 @@
                         None
                      names      ('__name__', '__module__', '__qualname__', 'forms', 'TextInput', 'p1', 'p2')
                      varnames   ()
                      freevars   ()
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'TestForm'
-                     firstlineno 252
+                     firstlineno 253
                      lnotab 0x0a011e01
                   'TestForm'
                   'form'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x950297008903a000000000000000000000000000000000000000000074
                         03000000000000000000007c01a6010000ab0100000000000000008902a6
                         020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           2
                      
-                     256           2 RESUME                   0
+                     257           2 RESUME                   0
                      
-                     258           4 LOAD_DEREF               3 (self)
+                     259           4 LOAD_DEREF               3 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_GLOBAL              3 (NULL + type)
                                   40 LOAD_FAST                1 (form)
                                   42 PRECALL                  1
                                   46 CALL                     1
                                   56 LOAD_DEREF               2 (TestForm)
                                   58 PRECALL                  2
@@ -3257,68 +3266,68 @@
                         None
                      names      ('assertEqual', 'type')
                      varnames   ('_request', 'form')
                      freevars   ('TestForm', 'self')
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 256
+                     firstlineno 257
                      lnotab 0x0402
-                  '/'
+                  'POST'
                   'a'
                   'b'
                   ('p1', 'p2')
-               names      ('forms', 'Form', 'inject_args', 'typing', 'cast', 'Any', 'factory', 'post')
+               names      ('forms', 'Form', 'view', 'typing', 'cast', 'Any', 'create_resolved_request')
                varnames   ('self', 'viewfn', 'untyped_viewfn')
                freevars   ()
                cellvars   ('self', 'TestForm')
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_auto_param_form'
-               firstlineno 251
+               firstlineno 252
                lnotab 0x060130041a0110ff0e0102033401
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x87029700020047006401840064027400000000000000000000006a0100
                   00000000000000a6030000ab0300000000000000008a0288026601640384
                   087d017c00a0020000000000000000000000000000000000000000740600
                   00000000000000000064047c01a6030000ab030000000000000000010064
                   005300
                              0 MAKE_CELL                2 (TestForm)
                
-               263           2 RESUME                   0
+               264           2 RESUME                   0
                
-               264           4 PUSH_NULL
+               265           4 PUSH_NULL
                              6 LOAD_BUILD_CLASS
-                             8 LOAD_CONST               1 (<code object TestForm, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 264>)
+                             8 LOAD_CONST               1 (<code object TestForm, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 265>)
                             10 MAKE_FUNCTION            0
                             12 LOAD_CONST               2 ('TestForm')
                             14 LOAD_GLOBAL              0 (forms)
                             26 LOAD_ATTR                1 (Form)
                             36 PRECALL                  3
                             40 CALL                     3
                             50 STORE_DEREF              2 (TestForm)
                
-               268          52 LOAD_CLOSURE             2 (TestForm)
+               269          52 LOAD_CLOSURE             2 (TestForm)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               3 (<code object test, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 268>)
+                            56 LOAD_CONST               3 (<code object test, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 269>)
                             58 MAKE_FUNCTION            8 (closure)
                             60 STORE_FAST               1 (test)
                
-               273          62 LOAD_FAST                0 (self)
+               274          62 LOAD_FAST                0 (self)
                             64 LOAD_METHOD              2 (assertRaisesRegex)
                
-               274          86 LOAD_GLOBAL              6 (Exception)
+               275          86 LOAD_GLOBAL              6 (Exception)
                             98 LOAD_CONST               4 ('You can only have one Form argument in a view function')
                            100 LOAD_FAST                1 (test)
                
-               273         102 PRECALL                  3
+               274         102 PRECALL                  3
                            106 CALL                     3
                            116 POP_TOP
                            118 LOAD_CONST               0 (None)
                            120 RETURN_VALUE
                consts
                   None
                   code
@@ -3326,28 +3335,28 @@
                      nlocals   : 0
                      stacksize : 2
                      flags     : 0
                      code
                         0x970065005a0164005a02020065036a040000000000000000a6000000ab
                         0000000000000000005a05020065036a040000000000000000a6000000ab
                         0000000000000000005a0664015300
-                     264           0 RESUME                   0
+                     265           0 RESUME                   0
                                    2 LOAD_NAME                0 (__name__)
                                    4 STORE_NAME               1 (__module__)
                                    6 LOAD_CONST               0 ('ParamsToArgsDecoratorTestCase.test_multiple_form_params_raises_exception.<locals>.TestForm')
                                    8 STORE_NAME               2 (__qualname__)
                      
-                     265          10 PUSH_NULL
+                     266          10 PUSH_NULL
                                   12 LOAD_NAME                3 (forms)
                                   14 LOAD_ATTR                4 (TextInput)
                                   24 PRECALL                  0
                                   28 CALL                     0
                                   38 STORE_NAME               5 (p1)
                      
-                     266          40 PUSH_NULL
+                     267          40 PUSH_NULL
                                   42 LOAD_NAME                3 (forms)
                                   44 LOAD_ATTR                4 (TextInput)
                                   54 PRECALL                  0
                                   58 CALL                     0
                                   68 STORE_NAME               6 (p2)
                                   70 LOAD_CONST               1 (None)
                                   72 RETURN_VALUE
@@ -3356,88 +3365,88 @@
                         None
                      names      ('__name__', '__module__', '__qualname__', 'forms', 'TextInput', 'p1', 'p2')
                      varnames   ()
                      freevars   ()
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'TestForm'
-                     firstlineno 264
+                     firstlineno 265
                      lnotab 0x0a011e01
                   'TestForm'
                   code
                      argcount  : 0
                      nlocals   : 1
                      stacksize : 5
                      flags     : 19
                      code
                         0x95019700740100000000000000000000a6000000ab0000000000000000
                         006401890164028901660464038404a6000000ab0000000000000000007d
                         0064005300
                                    0 COPY_FREE_VARS           1
                      
-                     268           2 RESUME                   0
+                     269           2 RESUME                   0
                      
-                     269           4 LOAD_GLOBAL              1 (NULL + inject_args)
+                     270           4 LOAD_GLOBAL              1 (NULL + view)
                                   16 PRECALL                  0
                                   20 CALL                     0
                      
-                     270          30 LOAD_CONST               1 ('_form1')
+                     271          30 LOAD_CONST               1 ('_form1')
                                   32 LOAD_DEREF               1 (TestForm)
                                   34 LOAD_CONST               2 ('_form2')
                                   36 LOAD_DEREF               1 (TestForm)
                                   38 BUILD_TUPLE              4
-                                  40 LOAD_CONST               3 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 269>)
+                                  40 LOAD_CONST               3 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 270>)
                                   42 MAKE_FUNCTION            4 (annotations)
                      
-                     269          44 PRECALL                  0
+                     270          44 PRECALL                  0
                                   48 CALL                     0
                      
-                     270          58 STORE_FAST               0 (viewfn)
+                     271          58 STORE_FAST               0 (viewfn)
                                   60 LOAD_CONST               0 (None)
                                   62 RETURN_VALUE
                      consts
                         None
                         '_form1'
                         '_form2'
                         code
                            argcount  : 3
                            nlocals   : 3
                            stacksize : 1
                            flags     : 19
                            code 0x970064005300
-                           269           0 RESUME                   0
+                           270           0 RESUME                   0
                            
-                           271           2 LOAD_CONST               0 (None)
+                           272           2 LOAD_CONST               0 (None)
                                          4 RETURN_VALUE
                            consts
                               None
                            names      ()
                            varnames   ('_request', '_form1', '_form2')
                            freevars   ()
                            cellvars   ()
                            filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                            name       'viewfn'
-                           firstlineno 269
+                           firstlineno 270
                            lnotab 0x0202
-                     names      ('inject_args',)
+                     names      ('view',)
                      varnames   ('viewfn',)
                      freevars   ('TestForm',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'test'
-                     firstlineno 268
+                     firstlineno 269
                      lnotab 0x04011a010eff0e01
                   'You can only have one Form argument in a view function'
                names      ('forms', 'Form', 'assertRaisesRegex', 'Exception')
                varnames   ('self', 'test')
                freevars   ()
                cellvars   ('TestForm',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_multiple_form_params_raises_exception'
-               firstlineno 263
+               firstlineno 264
                lnotab 0x040130040a05180110ff
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 8
                flags     : 3
                code
@@ -3447,50 +3456,50 @@
                   0000000000000000007c0119000000000000000000660288006601640684
                   0da6000000ab0000000000000000007d0202007c0289006a040000000000
                   000000a00500000000000000000000000000000000000000006407640864
                   09640a9c02a6020000ab020000000000000000a6010000ab010000000000
                   000000010064005300
                              0 MAKE_CELL                0 (self)
                
-               277           2 RESUME                   0
+               278           2 RESUME                   0
                
-               278           4 PUSH_NULL
+               279           4 PUSH_NULL
                              6 LOAD_BUILD_CLASS
-                             8 LOAD_CONST               1 (<code object TestForm, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 278>)
+                             8 LOAD_CONST               1 (<code object TestForm, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 279>)
                             10 MAKE_FUNCTION            0
                             12 LOAD_CONST               2 ('TestForm')
                             14 LOAD_GLOBAL              0 (forms)
                             26 LOAD_ATTR                1 (Form)
                             36 PRECALL                  3
                             40 CALL                     3
                             50 STORE_FAST               1 (TestForm)
                
-               282          52 LOAD_GLOBAL              5 (NULL + inject_args)
+               283          52 LOAD_GLOBAL              5 (NULL + inject_args)
                             64 LOAD_CONST               3 (False)
                             66 KW_NAMES                 4
                             68 PRECALL                  1
                             72 CALL                     1
                
-               283          82 LOAD_CONST              11 ((None,))
+               284          82 LOAD_CONST              11 ((None,))
                             84 LOAD_CONST               5 ('form')
                             86 LOAD_GLOBAL              6 (Optional)
                             98 LOAD_FAST                1 (TestForm)
                            100 BINARY_SUBSCR
                            110 BUILD_TUPLE              2
                            112 LOAD_CLOSURE             0 (self)
                            114 BUILD_TUPLE              1
-                           116 LOAD_CONST               6 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 282>)
+                           116 LOAD_CONST               6 (<code object viewfn, file "/home/roman/prjs/python/dfv/dfv/test_params_to_args.py", line 283>)
                            118 MAKE_FUNCTION           13 (defaults, annotations, closure)
                
-               282         120 PRECALL                  0
+               283         120 PRECALL                  0
                            124 CALL                     0
                
-               283         134 STORE_FAST               2 (viewfn)
+               284         134 STORE_FAST               2 (viewfn)
                
-               286         136 PUSH_NULL
+               287         136 PUSH_NULL
                            138 LOAD_FAST                2 (viewfn)
                            140 LOAD_DEREF               0 (self)
                            142 LOAD_ATTR                4 (factory)
                            152 LOAD_METHOD              5 (post)
                            174 LOAD_CONST               7 ('/')
                            176 LOAD_CONST               8 ('a')
                            178 LOAD_CONST               9 ('b')
@@ -3510,28 +3519,28 @@
                      nlocals   : 0
                      stacksize : 2
                      flags     : 0
                      code
                         0x970065005a0164005a02020065036a040000000000000000a6000000ab
                         0000000000000000005a05020065036a040000000000000000a6000000ab
                         0000000000000000005a0664015300
-                     278           0 RESUME                   0
+                     279           0 RESUME                   0
                                    2 LOAD_NAME                0 (__name__)
                                    4 STORE_NAME               1 (__module__)
                                    6 LOAD_CONST               0 ('ParamsToArgsDecoratorTestCase.test_auto_param_form_is_false.<locals>.TestForm')
                                    8 STORE_NAME               2 (__qualname__)
                      
-                     279          10 PUSH_NULL
+                     280          10 PUSH_NULL
                                   12 LOAD_NAME                3 (forms)
                                   14 LOAD_ATTR                4 (TextInput)
                                   24 PRECALL                  0
                                   28 CALL                     0
                                   38 STORE_NAME               5 (p1)
                      
-                     280          40 PUSH_NULL
+                     281          40 PUSH_NULL
                                   42 LOAD_NAME                3 (forms)
                                   44 LOAD_ATTR                4 (TextInput)
                                   54 PRECALL                  0
                                   58 CALL                     0
                                   68 STORE_NAME               6 (p2)
                                   70 LOAD_CONST               1 (None)
                                   72 RETURN_VALUE
@@ -3540,15 +3549,15 @@
                         None
                      names      ('__name__', '__module__', '__qualname__', 'forms', 'TextInput', 'p1', 'p2')
                      varnames   ()
                      freevars   ()
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'TestForm'
-                     firstlineno 278
+                     firstlineno 279
                      lnotab 0x0a011e01
                   'TestForm'
                   False
                   ('auto_form',)
                   'form'
                   code
                      argcount  : 2
@@ -3556,17 +3565,17 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x950197008902a000000000000000000000000000000000000000000064
                         007c01a6020000ab020000000000000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     282           2 RESUME                   0
+                     283           2 RESUME                   0
                      
-                     284           4 LOAD_DEREF               2 (self)
+                     285           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (assertEqual)
                                   28 LOAD_CONST               0 (None)
                                   30 LOAD_FAST                1 (form)
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 POP_TOP
                                   48 LOAD_CONST               0 (None)
@@ -3575,43 +3584,43 @@
                         None
                      names      ('assertEqual',)
                      varnames   ('_request', 'form')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                      name       'viewfn'
-                     firstlineno 282
+                     firstlineno 283
                      lnotab 0x0402
                   '/'
                   'a'
                   'b'
                   ('p1', 'p2')
                   (None,)
                names      ('forms', 'Form', 'inject_args', 'Optional', 'factory', 'post')
                varnames   ('self', 'TestForm', 'viewfn')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
                name       'test_auto_param_form_is_false'
-               firstlineno 277
+               firstlineno 278
                lnotab 0x040130041e0126ff0e010203
             ('return', None)
          names      ('__name__', '__module__', '__qualname__', 'RequestFactory', '__annotations__', 'setUp', 'test_without_type_annotation', 'test_param_default_defines_target_type', 'test_missing_param_raises_exception', 'test_optional', 'test_optional_with_type_conversion', 'test_type_conversion_int', 'test_type_conversion_float', 'test_type_conversion_bool', 'test_type_conversion_list_unannotated', 'test_type_conversion_list_annotated', 'test_post', 'test_get_and_post_order', 'test_function_call_arg_overrides_param', 'test_function_call_kwarg_overrides_param', 'test_param_consume_true', 'test_param_consume_false', 'test_param_consume_get', 'test_param_consume_post', 'test_auto_default_value', 'test_auto_param_false', 'test_auto_param_true', 'test_auto_param_get', 'test_auto_param_get_does_not_receive_post_params', 'test_auto_param_post', 'test_auto_param_post_does_not_receive_get_params', 'test_auto_param_form', 'test_multiple_form_params_raises_exception', 'test_auto_param_form_is_false')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
          name       'ParamsToArgsDecoratorTestCase'
-         firstlineno 13
+         firstlineno 14
          lnotab
             0x0c010a020804060e0609060a060c060a06070608060e06090609060c06
             070607060706080608060806080608060e06080608060906080609060c06
             0e
       'ParamsToArgsDecoratorTestCase'
-   names      ('typing', 'Any', 'Optional', 'unittest', 'TestCase', 'django', 'forms', 'django.http', 'HttpResponse', 'django.test', 'RequestFactory', 'dfv', 'inject_args', 'param', 'param_get', 'param_post', 'ParamsToArgsDecoratorTestCase')
+   names      ('typing', 'Any', 'Optional', 'unittest', 'TestCase', 'django', 'forms', 'django.http', 'HttpResponse', 'django.test', 'RequestFactory', 'dfv', 'inject_args', 'param', 'param_get', 'param_post', 'view', 'dfv.testutils', 'create_resolved_request', 'ParamsToArgsDecoratorTestCase')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/roman/prjs/python/dfv/dfv/test_params_to_args.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201080110010c0208010c010c010c021803
+   lnotab 0x00ff0201080110010c0208010c010c010c021c010c03
```

### Comparing `dfv-0.8.0/dfv/static/dfv.js` & `dfv-0.9.0/dfv/static/dfv.js`

 * *Files identical despite different names*

### Comparing `dfv-0.8.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc` & `dfv-0.9.0/dfv/templatetags/__pycache__/dfv.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dfv-0.8.0/dfv/test_element.py` & `dfv-0.9.0/dfv/test_element.py`

 * *Files identical despite different names*

### Comparing `dfv-0.8.0/dfv/test_form.py` & `dfv-0.9.0/dfv/test_form.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
+import typing
 from typing import Any
 from unittest import TestCase
 
 import django
-import typing
 from django import forms
 from django.http import HttpResponse
 from django.test import RequestFactory
+from django.urls import path, resolve
 
-from dfv import inject_args, handle_form
+from dfv import handle_form, view
+from dfv.testutils import create_resolved_request
 
 
 class TestForm(forms.Form):
     p1 = forms.CharField()
     p2 = forms.CharField()
 
 
@@ -21,85 +23,91 @@
 
     def setUp(self) -> None:
         self.factory = RequestFactory()
         django.setup()
 
     def test_error_missing_form_type(self):
         def test():
-            @inject_args()
+            @view()
             def viewfn(_request, form=handle_form()):
                 return HttpResponse(form)
 
         self.assertRaisesRegex(
             Exception,
             r"argument type for handle_form\(\) must be a subclass of django.forms.BaseForm",
             test,
         )
 
     def test_error_wrong_form_type(self):
         def test():
-            @inject_args()
+            @view()
             def viewfn(_request, _form: str = handle_form()):
                 return HttpResponse("")
 
         self.assertRaisesRegex(
             Exception,
             r"argument type for handle_form\(\) must be a subclass of django.forms.BaseForm",
             test,
         )
 
     def test_form_explicit(self):
-        @inject_args()
+        @view()
         def viewfn(_request, form: TestForm = handle_form()):
             self.assertEqual(type(form), TestForm)
             return HttpResponse("")
 
-        viewfn(self.factory.post("/", {"p1": "a", "p2": "b"}))
+        viewfn(create_resolved_request(viewfn, "POST", {"p1": "a", "p2": "b"}))
 
     def test_form_implicit(self):
-        @inject_args()
+        @view()
         def viewfn(_request, form: TestForm):
             self.assertEqual(type(form), TestForm)
             return HttpResponse("")
 
-        typing.cast(Any, viewfn)(self.factory.post("/", {"p1": "a", "p2": "b"}))
+        typing.cast(Any, viewfn)(
+            create_resolved_request(viewfn, "POST", {"p1": "a", "p2": "b"})
+        )
 
     def test_form_get(self):
-        @inject_args()
+        @view()
         def viewfn(_request, form: TestForm = handle_form()):
             self.assertFalse(form.is_bound)
             self.assertFalse(form.is_valid())
             return HttpResponse("")
 
-        viewfn(self.factory.get("/"))
+        viewfn(create_resolved_request(viewfn, "GET", {"p1": "a", "p2": "b"}))
 
     def test_form_post(self):
-        @inject_args()
+        @view()
         def viewfn(_request, form: TestForm = handle_form()):
             self.assertTrue(form.is_bound)
             self.assertTrue(form.is_valid())
             self.assertEqual(form.cleaned_data["p1"], "a")
             self.assertEqual(form.cleaned_data["p2"], "b")
             return HttpResponse("")
 
-        viewfn(self.factory.post("/", {"p1": "a", "p2": "b"}))
+        viewfn(create_resolved_request(viewfn, "POST", {"p1": "a", "p2": "b"}))
 
     def test_form_patch(self):
-        @inject_args()
+        @view()
         def viewfn(_request, form: TestForm = handle_form()):
             self.assertTrue(form.is_bound)
             self.assertFalse(form.is_valid())
             return HttpResponse("")
 
+        urlpatterns = (path("view/", viewfn, name="a view"),)
+        resolved = resolve("/view/", urlconf=urlpatterns)
         request = self.factory.patch(
             "/",
             json.dumps({"p1": "", "p2": "b"}),
             "application/json",
             headers={"X-DFV-Validate-Field": "p1"},
         )
+        request.resolver_match = resolved
+
         response = viewfn(request)
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response["Content-Type"], "application/json")
         body = json.loads(response.content)
         self.assertEqual(body["name"], "p1")
         field_p1 = body["fields"]["p1"]
         self.assertEqual(field_p1["valid"], False)
```

### Comparing `dfv-0.8.0/dfv/test_params_to_args.py` & `dfv-0.9.0/dfv/test_params_to_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,193 +3,194 @@
 from unittest import TestCase
 
 import django
 from django import forms
 from django.http import HttpResponse
 from django.test import RequestFactory
 
-from dfv import inject_args, param, param_get, param_post
+from dfv import inject_args, param, param_get, param_post, view
+from dfv.testutils import create_resolved_request
 
 
 class ParamsToArgsDecoratorTestCase(TestCase):
     factory: RequestFactory
 
     def setUp(self) -> None:
         self.factory = RequestFactory()
         django.setup()
 
     def test_without_type_annotation(self):
-        @inject_args()
+        @view()
         def viewfn(
             _request,
             p1=param_get(),
             p2=param_get(),
         ):
             self.assertEqual(p1, "a")
             self.assertEqual(p2, "b")
             return HttpResponse("")
 
         result = viewfn(self.factory.get("/?p1=a&p2=b"))
         self.assertEqual(result.status_code, 200)
 
     def test_param_default_defines_target_type(self):
-        @inject_args()
+        @view()
         def viewfn(_request, p1=param(default=123)):
             self.assertEqual(p1, 999)
             return HttpResponse("")
 
         result = viewfn(self.factory.get("/?p1=999"))
         self.assertEqual(result.status_code, 200)
 
     def test_missing_param_raises_exception(self):
-        @inject_args()
+        @view()
         def viewfn(_request, p1=param_get()):
             self.assertEqual(p1, 1)
 
         def test():
             viewfn(self.factory.get("/"))
 
         self.assertRaises(Exception, test)
 
     def test_optional(self):
-        @inject_args()
+        @view()
         def viewfn(
             _request,
             p1: str | None = param_get(),
             p2: Optional[str] = param_get(),
         ):
             self.assertEqual(p1, None)
             self.assertEqual(p2, None)
 
         viewfn(self.factory.get("/"))
 
     def test_optional_with_type_conversion(self):
-        @inject_args()
+        @view()
         def viewfn(
             _request,
             p1: Optional[int] = param_get(),
         ):
             self.assertEqual(p1, 1)
 
         viewfn(self.factory.get("/?p1=1"))
 
     def test_type_conversion_int(self):
-        @inject_args()
+        @view()
         def viewfn(_request, p1: int = param_get()):
             self.assertEqual(p1, 1)
 
         viewfn(self.factory.get("/?p1=1"))
 
     def test_type_conversion_float(self):
-        @inject_args()
+        @view()
         def viewfn(_request, p1: float = param_get()):
             self.assertEqual(p1, 1.1)
             self.assertEqual(type(p1), float)
 
         viewfn(self.factory.get("/?p1=1.1"))
 
     def test_type_conversion_bool(self):
-        @inject_args()
+        @view()
         def viewfn(
             _request,
             p1: bool = param_get(),
             p2: bool = param_get(),
             p3: bool = param_get(),
         ):
             self.assertEqual(p1, False)
             self.assertEqual(p2, False)
             self.assertEqual(p3, False)
 
         viewfn(self.factory.get("/?p1=false&p2=False&p3"))
 
     def test_type_conversion_list_unannotated(self):
-        @inject_args()
+        @view()
         def viewfn(_request, p1: list = param_get()):
             self.assertEqual(type(p1), list)
             self.assertTrue("a" in p1)
             self.assertTrue("b" in p1)
 
         viewfn(self.factory.get("/?p1=a&p1=b"))
 
     def test_type_conversion_list_annotated(self):
-        @inject_args()
+        @view()
         def viewfn(_request, p1: list[int] = param_get()):
             self.assertEqual(type(p1), list)
             self.assertTrue(1 in p1)
             self.assertTrue(2 in p1)
 
         viewfn(self.factory.get("/?p1=1&p1=2"))
 
     def test_post(self):
-        @inject_args()
+        @view()
         def viewfn(
             _request,
             p1: str = param_post(),
             p2: str = param_post(),
         ):
             self.assertEqual(p1, "a")
             self.assertEqual(p2, "b")
 
         viewfn(self.factory.post("/", {"p1": "a", "p2": "b"}))
 
     def test_get_and_post_order(self):
-        @inject_args()
+        @view()
         def viewfn(_request, p1: str = param()):
             self.assertEqual(p1, "a")
 
         viewfn(self.factory.post("/?p1=a", {"p1": "b"}))
 
     def test_function_call_arg_overrides_param(self):
-        @inject_args()
+        @view()
         def viewfn(_request, p1: str = param()):
             self.assertEqual(p1, "b")
 
         viewfn(self.factory.get("/?p1=a"), "b")
 
     def test_function_call_kwarg_overrides_param(self):
-        @inject_args()
+        @view()
         def viewfn(_request, p1: str = param()):
             self.assertEqual(p1, "b")
 
         viewfn(self.factory.get("/?p1=a"), p1="b")
 
     def test_param_consume_true(self):
-        @inject_args()
+        @view()
         def viewfn(request, p1: str = param()):
             self.assertEqual(p1, "a")
             self.assertNotIn("p1", request.GET)
 
         viewfn(self.factory.get("/?p1=a"))
 
     def test_param_consume_false(self):
-        @inject_args()
+        @view()
         def viewfn(request, p1: str = param(consume=False)):
             self.assertEqual(p1, "a")
             self.assertIn("p1", request.GET)
 
         viewfn(self.factory.get("/?p1=a"))
 
     def test_param_consume_get(self):
-        @inject_args()
+        @view()
         def viewfn(request, p1: str = param_get()):
             self.assertEqual(p1, "a")
             self.assertNotIn("p1", request.GET)
 
         viewfn(self.factory.get("/?p1=a"))
 
     def test_param_consume_post(self):
-        @inject_args()
+        @view()
         def viewfn(request, p1: str = param_post()):
             self.assertEqual(p1, "a")
             self.assertNotIn("p1", request.POST)
 
         viewfn(self.factory.post("/", {"p1": "a"}))
 
     def test_auto_default_value(self):
-        @inject_args()
+        @view()
         def viewfn(_request, p1: str = param(default="a")):
             self.assertEqual(p1, "a")
 
         untyped_viewfn = typing.cast(Any, viewfn)
         untyped_viewfn(self.factory.get("/"))
 
     def test_auto_param_false(self):
@@ -249,28 +250,28 @@
         untyped_viewfn(self.factory.post("/p2=x", {"p1": "a"}))
 
     def test_auto_param_form(self):
         class TestForm(forms.Form):
             p1 = forms.TextInput()
             p2 = forms.TextInput()
 
-        @inject_args()
+        @view()
         def viewfn(_request, form: TestForm):
             self.assertEqual(type(form), TestForm)
 
         untyped_viewfn = typing.cast(Any, viewfn)
-        untyped_viewfn(self.factory.post("/", {"p1": "a", "p2": "b"}))
+        untyped_viewfn(create_resolved_request(viewfn, "POST", {"p1": "a", "p2": "b"}))
 
     def test_multiple_form_params_raises_exception(self):
         class TestForm(forms.Form):
             p1 = forms.TextInput()
             p2 = forms.TextInput()
 
         def test():
-            @inject_args()
+            @view()
             def viewfn(_request, _form1: TestForm, _form2: TestForm):
                 pass
 
         self.assertRaisesRegex(
             Exception, "You can only have one Form argument in a view function", test
         )
```

### Comparing `dfv-0.8.0/pyproject.toml` & `dfv-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "dfv"
-version = "0.8.0"
+version = "0.9.0"
 description = "Django Function Views"
 authors = ["Roman Roelofsen <romanroe@gmail.com>"]
 include = ["dfv"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
-django = "^4.1.7"
+django = "4.2.4"
 django-htmx = "^1.14.0"
 lxml = "^4.9.2"
 wrapt = "^1.15.0"
 typeguard = "*"
 
 [tool.poetry.dev-dependencies]
 whitenoise = "^6.5.0"
 django-debug-toolbar = "*"
 django-browser-reload = "^1.7.0"
 django-widget-tweaks = "^1.4.12"
 django-extensions = "^3.1.5"
 black = {extras = ["d"], version = "^23.1.0"}
 django-click = "^2.3.0"
-ruff = "^0.0.280"
+ruff = "0.0.282"
 mypy = "1.4.1"
 coverage = "^7.2.1"
 psycopg = "^3.1.9"
 tblib = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `dfv-0.8.0/setup.py` & `dfv-0.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['dfv', 'dfv.templatetags']
 
 package_data = \
 {'': ['*'], 'dfv': ['static/*', 'templates/dfv/tests/*']}
 
 install_requires = \
 ['django-htmx>=1.14.0,<2.0.0',
- 'django>=4.1.7,<5.0.0',
+ 'django==4.2.4',
  'lxml>=4.9.2,<5.0.0',
  'typeguard',
  'wrapt>=1.15.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'dfv',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Django Function Views',
     'long_description': 'None',
     'author': 'Roman Roelofsen',
     'author_email': 'romanroe@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dfv-0.8.0/PKG-INFO` & `dfv-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dfv
-Version: 0.8.0
+Version: 0.9.0
 Summary: Django Function Views
 Author: Roman Roelofsen
 Author-email: romanroe@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django (>=4.1.7,<5.0.0)
+Requires-Dist: django (==4.2.4)
 Requires-Dist: django-htmx (>=1.14.0,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: typeguard
 Requires-Dist: wrapt (>=1.15.0,<2.0.0)
```

