# Comparing `tmp/mo_sql_parsing-9.428.23214-py2.py3-none-any.whl.zip` & `tmp/mo_sql_parsing-9.429.23215-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 38409 bytes, number of entries: 13
+Zip file size: 38454 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     2530 b- defN 23-Jul-18 01:32 mo_sql_parsing/__init__.py
--rw-rw-rw-  2.0 fat    22382 b- defN 23-Jul-18 01:32 mo_sql_parsing/formatting.py
--rw-rw-rw-  2.0 fat    10695 b- defN 23-Jul-18 01:32 mo_sql_parsing/keywords.py
+-rw-rw-rw-  2.0 fat    22496 b- defN 23-Aug-03 21:55 mo_sql_parsing/formatting.py
+-rw-rw-rw-  2.0 fat    10771 b- defN 23-Aug-03 21:55 mo_sql_parsing/keywords.py
 -rw-rw-rw-  2.0 fat    34299 b- defN 23-Aug-02 00:44 mo_sql_parsing/sql_parser.py
 -rw-rw-rw-  2.0 fat     7357 b- defN 23-Jul-22 13:56 mo_sql_parsing/types.py
--rw-rw-rw-  2.0 fat    23118 b- defN 23-Jul-27 21:40 mo_sql_parsing/utils.py
+-rw-rw-rw-  2.0 fat    23120 b- defN 23-Aug-03 21:55 mo_sql_parsing/utils.py
 -rw-rw-rw-  2.0 fat     2920 b- defN 23-Jul-18 01:32 mo_sql_parsing/windows.py
--rw-rw-rw-  2.0 fat    15922 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9345 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1134 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/RECORD
-13 files, 129829 bytes uncompressed, 36503 bytes compressed:  71.9%
+-rw-rw-rw-  2.0 fat    15922 b- defN 23-Aug-03 21:55 mo_sql_parsing-9.429.23215.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9345 b- defN 23-Aug-03 21:55 mo_sql_parsing-9.429.23215.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Aug-03 21:55 mo_sql_parsing-9.429.23215.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Aug-03 21:55 mo_sql_parsing-9.429.23215.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Aug-03 21:55 mo_sql_parsing-9.429.23215.dist-info/zip-safe
+?rw-rw-r--  2.0 fat     1134 b- defN 23-Aug-03 21:55 mo_sql_parsing-9.429.23215.dist-info/RECORD
+13 files, 130021 bytes uncompressed, 36548 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mo_sql_parsing/utils.py
 Comment: 
 
 Filename: mo_sql_parsing/windows.py
 Comment: 
 
-Filename: mo_sql_parsing-9.428.23214.dist-info/LICENSE
+Filename: mo_sql_parsing-9.429.23215.dist-info/LICENSE
 Comment: 
 
-Filename: mo_sql_parsing-9.428.23214.dist-info/METADATA
+Filename: mo_sql_parsing-9.429.23215.dist-info/METADATA
 Comment: 
 
-Filename: mo_sql_parsing-9.428.23214.dist-info/WHEEL
+Filename: mo_sql_parsing-9.429.23215.dist-info/WHEEL
 Comment: 
 
-Filename: mo_sql_parsing-9.428.23214.dist-info/top_level.txt
+Filename: mo_sql_parsing-9.429.23215.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_sql_parsing-9.428.23214.dist-info/zip-safe
+Filename: mo_sql_parsing-9.429.23215.dist-info/zip-safe
 Comment: 
 
-Filename: mo_sql_parsing-9.428.23214.dist-info/RECORD
+Filename: mo_sql_parsing-9.429.23215.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_sql_parsing/formatting.py

```diff
@@ -308,14 +308,17 @@
         # treat as regular function call
         if isinstance(value, dict) and len(value) == 0:
             return key.upper() + "()"  # NOT SURE IF AN EMPTY dict SHOULD BE DELT WITH HERE, OR IN self.format()
         else:
             params = ", ".join(self.dispatch(p, precedence["from"]) for p in listwrap(value))
             return f"{key.upper()}({params})"
 
+    def _regexp(self, value, prec):
+        return f"{self.dispatch(value[0])} REGEXP {self.dispatch(value[1])}"
+
     def _binary_not(self, value, prec):
         return "~{0}".format(self.dispatch(value))
 
     def _not(self, value, prec):
         op_prec = precedence["not"]
         if prec >= op_prec:
             return f"NOT {self.dispatch(value)}"
```

## mo_sql_parsing/keywords.py

```diff
@@ -115,14 +115,15 @@
     keyword("is distinct from").set_parser_name("eq!")
 )
 INDF = (
     # decisive equality
     # https://prestodb.io/docs/current/functions/comparison.html#is-distinct-from-and-is-not-distinct-from
     keyword("is not distinct from").set_parser_name("ne!")
 )
+REGEXP = keyword("regexp").set_parser_name("rgx")
 NEQ = (Literal("!=") | Literal("<>")).set_parser_name("neq")
 LAMBDA = Literal("->").set_parser_name("lambda")
 
 AND = keyword("and")
 APPLY = keyword("apply")
 BETWEEN = keyword("between")
 CASE = keyword("case").suppress()
@@ -283,14 +284,15 @@
     "binary_and": 4,
     "binary_or": 4,
     "gte": 5,
     "lte": 5,
     "lt": 5,
     "gt": 6,
     "eq": 7,
+    "rgx": 7,
     "neq": 7,
     "missing": 7,
     "exists": 7,
     "at_time_zone": 8,
     "between": 8,
     "not_between": 8,
     "not": 8,
@@ -349,14 +351,15 @@
     NOT_RLIKE,
     SIMILAR_TO,
     NOT_SIMILAR_TO,
     NOT,
     AND,
     OR,
     LAMBDA,
+    REGEXP,
 ]
 
 times = ["now", "today", "tomorrow", "eod"]
 
 durations = {
     "microseconds": "microsecond",
     "microsecond": "microsecond",
```

## mo_sql_parsing/utils.py

```diff
@@ -309,16 +309,16 @@
     if not frum:
         return Call("trim", [tokens["chars"]], {"direction": tokens["direction"]})
     return Call("trim", [frum], {"characters": tokens["chars"], "direction": tokens["direction"]},)
 
 
 def to_index_part(tokens):
     value = dict(tokens)
-    if len(value)==1:
-        return value['value']
+    if len(value) == 1:
+        return value["value"]
     return value
 
 
 def to_kwarg(tokens):
     return {k: v for k, v in [tuple(tokens)]}
```

## Comparing `mo_sql_parsing-9.428.23214.dist-info/LICENSE` & `mo_sql_parsing-9.429.23215.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_sql_parsing-9.428.23214.dist-info/METADATA` & `mo_sql_parsing-9.429.23215.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.428.23214
+Version: 9.429.23215
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
```

## Comparing `mo_sql_parsing-9.428.23214.dist-info/RECORD` & `mo_sql_parsing-9.429.23215.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mo_sql_parsing/__init__.py,sha256=ZbsunSI2YPlPkveviGXQuv_YjCmofsrVOOu6qb500gM,2530
-mo_sql_parsing/formatting.py,sha256=Nzcrs6aWLQRK0hd8QvyPZ4hMF1onIhyvE2iBrtKF-Fw,22382
-mo_sql_parsing/keywords.py,sha256=nFTOQv7VOTDI4Ud3oSJh0-II9FGH4wWXmFRwZ5R3uzk,10695
+mo_sql_parsing/formatting.py,sha256=SZJylVnoVrnrt_ub1a9TO0xUBrKNjHXzxBVxPzvH2dY,22496
+mo_sql_parsing/keywords.py,sha256=r9aDcPatq-iHRQzRkaOcRck8m2OYT39xfWcP65RiJM0,10771
 mo_sql_parsing/sql_parser.py,sha256=WSvORof2TnoekZzZm8Tm60AzEP9NCPSKMfLqFFGI6kU,34299
 mo_sql_parsing/types.py,sha256=tloEMsDgghBPm9O9MjyMLj8lUJ2ALTMdPEv3hU841HY,7357
-mo_sql_parsing/utils.py,sha256=r5EAEgGlIINl3UPN18Hk7LS4pQzeA_GLytRP-CI79aE,23118
+mo_sql_parsing/utils.py,sha256=m8PgHljpjica6PrVaPY4IAq6xUyl3tor5BGJ0n3bvF8,23120
 mo_sql_parsing/windows.py,sha256=KelC9CZopR53tb0xAPxWsbxt59ieR_kNmM37FFcMjzE,2920
-mo_sql_parsing-9.428.23214.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
-mo_sql_parsing-9.428.23214.dist-info/METADATA,sha256=ngF9Tq9yBtsh85G2gGhBImcN1Q5o5QjgLQh-fxckRUk,9345
-mo_sql_parsing-9.428.23214.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_sql_parsing-9.428.23214.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
-mo_sql_parsing-9.428.23214.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-mo_sql_parsing-9.428.23214.dist-info/RECORD,,
+mo_sql_parsing-9.429.23215.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
+mo_sql_parsing-9.429.23215.dist-info/METADATA,sha256=Rn8eHvH7e_P5o7PArmQTcwEY5QsU9exwX2mJnY7dtAI,9345
+mo_sql_parsing-9.429.23215.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_sql_parsing-9.429.23215.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
+mo_sql_parsing-9.429.23215.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+mo_sql_parsing-9.429.23215.dist-info/RECORD,,
```

