# Comparing `tmp/polymeasure-0.1.2.tar.gz` & `tmp/polymeasure-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymeasure-0.1.2.tar", last modified: Thu Jul 27 21:11:58 2023, max compression
+gzip compressed data, was "polymeasure-0.1.3.tar", last modified: Wed Aug  2 22:12:24 2023, max compression
```

## Comparing `polymeasure-0.1.2.tar` & `polymeasure-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 21:11:58.339180 polymeasure-0.1.2/
--rw-rw-rw-   0        0        0     1109 2023-07-22 12:44:08.000000 polymeasure-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5676 2023-07-27 21:11:58.338179 polymeasure-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5112 2023-07-23 11:15:31.000000 polymeasure-0.1.2/README.md
--rw-rw-rw-   0        0        0      644 2023-07-27 21:09:28.000000 polymeasure-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 21:11:58.339180 polymeasure-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-27 21:11:58.323180 polymeasure-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 21:11:58.332180 polymeasure-0.1.2/src/polymeasure/
--rw-rw-rw-   0        0        0      117 2023-07-22 12:44:08.000000 polymeasure-0.1.2/src/polymeasure/__init__.py
--rw-rw-rw-   0        0        0    43122 2023-07-27 21:04:38.000000 polymeasure-0.1.2/src/polymeasure/core.py
--rw-rw-rw-   0        0        0     2944 2023-07-27 21:09:28.000000 polymeasure-0.1.2/src/polymeasure/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-27 21:11:58.335179 polymeasure-0.1.2/src/polymeasure.egg-info/
--rw-rw-rw-   0        0        0     5676 2023-07-27 21:11:58.000000 polymeasure-0.1.2/src/polymeasure.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-07-27 21:11:58.000000 polymeasure-0.1.2/src/polymeasure.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 21:11:58.000000 polymeasure-0.1.2/src/polymeasure.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-27 21:11:58.000000 polymeasure-0.1.2/src/polymeasure.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 21:11:58.337181 polymeasure-0.1.2/tests/
--rw-rw-rw-   0        0        0      405 2023-07-24 01:15:59.000000 polymeasure-0.1.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:12:24.209994 polymeasure-0.1.3/
+-rw-rw-rw-   0        0        0     1109 2023-07-22 12:44:08.000000 polymeasure-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5869 2023-08-02 22:12:24.208994 polymeasure-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5311 2023-08-02 22:06:45.000000 polymeasure-0.1.3/README.md
+-rw-rw-rw-   0        0        0      657 2023-07-29 22:58:15.000000 polymeasure-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 22:12:24.209994 polymeasure-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 22:12:24.193993 polymeasure-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 22:12:24.201994 polymeasure-0.1.3/src/polymeasure/
+-rw-rw-rw-   0        0        0      117 2023-07-22 12:44:08.000000 polymeasure-0.1.3/src/polymeasure/__init__.py
+-rw-rw-rw-   0        0        0    43045 2023-08-02 21:45:26.000000 polymeasure-0.1.3/src/polymeasure/core.py
+-rw-rw-rw-   0        0        0     5824 2023-08-01 05:08:31.000000 polymeasure-0.1.3/src/polymeasure/standard.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:12:24.205994 polymeasure-0.1.3/src/polymeasure.egg-info/
+-rw-rw-rw-   0        0        0     5869 2023-08-02 22:12:24.000000 polymeasure-0.1.3/src/polymeasure.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-08-02 22:12:24.000000 polymeasure-0.1.3/src/polymeasure.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 22:12:24.000000 polymeasure-0.1.3/src/polymeasure.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-02 22:12:24.000000 polymeasure-0.1.3/src/polymeasure.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 22:12:24.207994 polymeasure-0.1.3/tests/
+-rw-rw-rw-   0        0        0      405 2023-07-24 01:15:59.000000 polymeasure-0.1.3/tests/test.py
```

### Comparing `polymeasure-0.1.2/LICENSE` & `polymeasure-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polymeasure-0.1.2/PKG-INFO` & `polymeasure-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: polymeasure
-Version: 0.1.2
-Summary: A python analysis package for building SQL expressions.
+Version: 0.1.3
+Summary: A python analysis package for SQL data modelling.
 Author-email: Josh Grant <jagmanjg@gmail.com>
 Project-URL: Homepage, https://github.com/jgrant-the-giant/polymeasure
 Project-URL: Bug Tracker, https://github.com/jgrant-the-giant/polymeasure/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -23,16 +23,19 @@
 PolyMeasures have three main components
 
 - an inner view, also a PolyMeasure
 - a set of outer PolyMeasures to evaluate over that view, and
 - a set of dimensions to group the inner view by when evaluating the outer view(s).
 
 The function `evaluate()` returns a SQL statement, built recursively from those components.
+Filtering clauses like where and having can be supplied as arguments to the PolyMeasure or evaluate() call.
+Where clauses are abstract python `FilterExpression` objects that can be given dynamic behaviours 
+depending on evaluation context.
 
-In the documentation we drop the name parameter and write
+In this documentation we drop the name parameter and write
 
 `M( Outer * Dim; Inner: Where, Context )`
 
 when describing a PolyMeasure, in line with the order of the other parameters of importance.
 
 ## How it works in a nutshell
 
@@ -63,52 +66,49 @@
   where Where
   <<context>>
 ```
 
 ## How it works
 
 
-The context can be parameters like having or order by clauses.
-The where parameter specifies additional filters to apply to the
-
 There are two classes of PolyMeasures - those with a free view, where Outer = None, or a bound view
 which already exists in the database.
 A bound measure with the usual arguments will be denoted `B( Inner * Dim; Outer: Where )`
 and a free measure denoted `F( Inner * Dim; Outer: Where )`. Free views become handy expressions like
 "count(*) of any inner table" or "count(*) over dimensions of the inner table".
 
 Free measures take on the context of the inner query in a PolyMeasure, rather than referencing a basic
 view in the schema. This allows a single PolyMeasure object to perform a double aggregation over a given
-view, where we group once, then group the resulting rowset again and perform some aggregation.
+view, where we group once, then group the resulting row set again and perform some aggregation.
 
 If a free measure is supplied to the outer measure list, it will query the corresponding inner measure list.
 Free measures should not be supplied as the inner measure of a PolyMeasure, unless the outer measures can supply
 their own inner bindings.
 
 Bound measures should have a default string value for the view, appropriate to the schema.
-Using the supplied factory method BoundedMeasure will return a super-classed PolyMeasure
+Using the supplied factory method bound_objects will return a super-classed PolyMeasure and FilterExpression objects
 keyed to a specific view, for convenience.
 
 In the following examples, we assume one unique bounded measure exists,
 B = B(dim=Rowset(), inner=main_view), which acts as the ultimate "leaf" measure.
 The class Free is also provided, which defaults the measure view to Free instead, and is aliased F.
 
 The Outer and Inner arguments are PolyMeasure vectors, which each can return tables of any dimension.
 When different dimensions are supplied in the outer measures, self.dim is used to group the inner view,
 but each measure still evaluates by matching only on its own dimension, if specified.
 No attempt is made to reconcile the dimensions between inner and outer arguments - if a measure requests
 a column that doesn't exist in dim(M) (the inner dimension specified by M), then the SQL parser
 will let you know :)
 
-When supplied as an argument, a tuple is interpreted as a "Dummy PolyMeasure" (name, inner, [dim]),
+When supplied as an argument, a tuple is interpreted as a "Dummy PolyMeasure" (name, outer, [dim]),
 where dim can be omitted. These measures are always free.
 
 When defining dimensions, [] means group by the whole table,
-RowSet means do not group the view. None is a wildcard, which means the measure will default
-to the dimensions of the enclosing measure after dimension promotion.
+RowSet means do not group the view at all. None is a wildcard, which means the measure will default
+to the dimensions of the enclosing measure after dimension promotion. None and [] will behave identically in most cases.
 
 The view and where parameters are applied to the inner query, Inner * Dim.
 For example if you want to apply a filter context to Outer directly (which is the final output aggregation),
 use M( Inner * Dim; F(Outer: Where_Outer): View, Where)
 
 ==========================================
```

### Comparing `polymeasure-0.1.2/README.md` & `polymeasure-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 PolyMeasures have three main components
 
 - an inner view, also a PolyMeasure
 - a set of outer PolyMeasures to evaluate over that view, and
 - a set of dimensions to group the inner view by when evaluating the outer view(s).
 
 The function `evaluate()` returns a SQL statement, built recursively from those components.
+Filtering clauses like where and having can be supplied as arguments to the PolyMeasure or evaluate() call.
+Where clauses are abstract python `FilterExpression` objects that can be given dynamic behaviours 
+depending on evaluation context.
 
-In the documentation we drop the name parameter and write
+In this documentation we drop the name parameter and write
 
 `M( Outer * Dim; Inner: Where, Context )`
 
 when describing a PolyMeasure, in line with the order of the other parameters of importance.
 
 ## How it works in a nutshell
 
@@ -49,52 +52,49 @@
   where Where
   <<context>>
 ```
 
 ## How it works
 
 
-The context can be parameters like having or order by clauses.
-The where parameter specifies additional filters to apply to the
-
 There are two classes of PolyMeasures - those with a free view, where Outer = None, or a bound view
 which already exists in the database.
 A bound measure with the usual arguments will be denoted `B( Inner * Dim; Outer: Where )`
 and a free measure denoted `F( Inner * Dim; Outer: Where )`. Free views become handy expressions like
 "count(*) of any inner table" or "count(*) over dimensions of the inner table".
 
 Free measures take on the context of the inner query in a PolyMeasure, rather than referencing a basic
 view in the schema. This allows a single PolyMeasure object to perform a double aggregation over a given
-view, where we group once, then group the resulting rowset again and perform some aggregation.
+view, where we group once, then group the resulting row set again and perform some aggregation.
 
 If a free measure is supplied to the outer measure list, it will query the corresponding inner measure list.
 Free measures should not be supplied as the inner measure of a PolyMeasure, unless the outer measures can supply
 their own inner bindings.
 
 Bound measures should have a default string value for the view, appropriate to the schema.
-Using the supplied factory method BoundedMeasure will return a super-classed PolyMeasure
+Using the supplied factory method bound_objects will return a super-classed PolyMeasure and FilterExpression objects
 keyed to a specific view, for convenience.
 
 In the following examples, we assume one unique bounded measure exists,
 B = B(dim=Rowset(), inner=main_view), which acts as the ultimate "leaf" measure.
 The class Free is also provided, which defaults the measure view to Free instead, and is aliased F.
 
 The Outer and Inner arguments are PolyMeasure vectors, which each can return tables of any dimension.
 When different dimensions are supplied in the outer measures, self.dim is used to group the inner view,
 but each measure still evaluates by matching only on its own dimension, if specified.
 No attempt is made to reconcile the dimensions between inner and outer arguments - if a measure requests
 a column that doesn't exist in dim(M) (the inner dimension specified by M), then the SQL parser
 will let you know :)
 
-When supplied as an argument, a tuple is interpreted as a "Dummy PolyMeasure" (name, inner, [dim]),
+When supplied as an argument, a tuple is interpreted as a "Dummy PolyMeasure" (name, outer, [dim]),
 where dim can be omitted. These measures are always free.
 
 When defining dimensions, [] means group by the whole table,
-RowSet means do not group the view. None is a wildcard, which means the measure will default
-to the dimensions of the enclosing measure after dimension promotion.
+RowSet means do not group the view at all. None is a wildcard, which means the measure will default
+to the dimensions of the enclosing measure after dimension promotion. None and [] will behave identically in most cases.
 
 The view and where parameters are applied to the inner query, Inner * Dim.
 For example if you want to apply a filter context to Outer directly (which is the final output aggregation),
 use M( Inner * Dim; F(Outer: Where_Outer): View, Where)
 
 ==========================================
```

### Comparing `polymeasure-0.1.2/pyproject.toml` & `polymeasure-0.1.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "sqlparse>=0.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "polymeasure"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Josh Grant", email="jagmanjg@gmail.com" },
 ]
-description = "A python analysis package for building SQL expressions."
+description = "A python analysis package for SQL data modelling."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `polymeasure-0.1.2/src/polymeasure/core.py` & `polymeasure-0.1.3/src/polymeasure/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -724,15 +724,15 @@
         if star_expression is not None and star_expression:
             groupby_dimensions = [star_expression]
         else:
             groupby_dimensions = evaluate_dimensions if allow_grouping else []
 
         # null queries have well defined inner measures but they do not have a select statement from them..
         is_null_query = (wildcard_dimensions.dimensions is None and not wildcard_dimensions.rowset) and (
-                self.outer_dimension.wildcard and not self.outer_dimension.rowset)
+            self.outer_dimension.wildcard and not self.outer_dimension.rowset)
 
         # Treat this query as a source query, do not alias the final from statement
         evaluate_as_source = self._check_primitive(evaluate_inner) or is_null_query
 
         # filter these where statements using include/exclude and dimensionality
         # These where statements are given to outer and inner measures
         # self.where are added in afterwards..
@@ -897,41 +897,38 @@
         for measure in self.outer:
 
             # if measure.primitive or (not measure.free and self.source):
             #     use_alias = False
             # else:
             #     use_alias = True
 
-            if measure.primitive:
+            if measure.primitive and (len(measure.outer) == 1) or not measure.source:
 
                 # The recursion now has a primitive measure which can be evaluated directly.
+                # Lock the passthrough wheres to the current original alias - this is the right place to do it
 
-                if len(measure.outer) == 1:
-
-                    # Lock the passthrough wheres to the current original alias - this is the right place to do it
-
-                    locked_where = [
-                        expression.fix_outer(original_alias) for expression in passthrough_where
-                    ]
-
-                    # if measure.free and measure.outer_dimension.wildcard and self.outer_dimension.rowset:
-                    if measure.free and wildcard_inner is None:
-                        # Generated when a rowset query doesn't need a subquery expression
-                        primitive_sql_list = primitive_sql_list + measure._get_primitive_expression(
-                            inner_alias=original_alias, override_name=override_name, update_columns=update_columns)
+                locked_where = [
+                    expression.fix_outer(original_alias) for expression in passthrough_where
+                ]
+
+                # if measure.free and measure.outer_dimension.wildcard and self.outer_dimension.rowset:
+                if measure.free and wildcard_inner is None:
+                    # Generated when a rowset query doesn't need a subquery expression
+                    primitive_sql_list = primitive_sql_list + measure._get_primitive_expression(
+                        inner_alias=original_alias, override_name=override_name, update_columns=update_columns)
+                else:
+                    if update_columns:
+                        alias_type = 'set'
                     else:
-                        if update_columns:
-                            alias_type = 'set'
-                        else:
-                            alias_type = None
-                        primitive_sql_list = primitive_sql_list + [measure._evaluate(
-                            locked_where, depth + 1, breadth, wildcard_inner,
-                            wildcard_dimensions, aliased=True, allow_grouping=False,
-                            override_name=override_name, update_columns=update_columns, alias_type=alias_type
-                        )]
+                        alias_type = None
+                    primitive_sql_list = primitive_sql_list + [measure._evaluate(
+                        locked_where, depth + 1, breadth, wildcard_inner,
+                        wildcard_dimensions, aliased=True, allow_grouping=False,
+                        override_name=override_name, update_columns=update_columns, alias_type=alias_type
+                    )]
 
 
             else:
 
                 primitive_sql_list = primitive_sql_list + measure._get_primitive_sql_list(
                     # This is a non-primitive measure that has no opportunity to evaluate its
                     # own where clauses, so they are appended here.
```

### Comparing `polymeasure-0.1.2/src/polymeasure.egg-info/PKG-INFO` & `polymeasure-0.1.3/src/polymeasure.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: polymeasure
-Version: 0.1.2
-Summary: A python analysis package for building SQL expressions.
+Version: 0.1.3
+Summary: A python analysis package for SQL data modelling.
 Author-email: Josh Grant <jagmanjg@gmail.com>
 Project-URL: Homepage, https://github.com/jgrant-the-giant/polymeasure
 Project-URL: Bug Tracker, https://github.com/jgrant-the-giant/polymeasure/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -23,16 +23,19 @@
 PolyMeasures have three main components
 
 - an inner view, also a PolyMeasure
 - a set of outer PolyMeasures to evaluate over that view, and
 - a set of dimensions to group the inner view by when evaluating the outer view(s).
 
 The function `evaluate()` returns a SQL statement, built recursively from those components.
+Filtering clauses like where and having can be supplied as arguments to the PolyMeasure or evaluate() call.
+Where clauses are abstract python `FilterExpression` objects that can be given dynamic behaviours 
+depending on evaluation context.
 
-In the documentation we drop the name parameter and write
+In this documentation we drop the name parameter and write
 
 `M( Outer * Dim; Inner: Where, Context )`
 
 when describing a PolyMeasure, in line with the order of the other parameters of importance.
 
 ## How it works in a nutshell
 
@@ -63,52 +66,49 @@
   where Where
   <<context>>
 ```
 
 ## How it works
 
 
-The context can be parameters like having or order by clauses.
-The where parameter specifies additional filters to apply to the
-
 There are two classes of PolyMeasures - those with a free view, where Outer = None, or a bound view
 which already exists in the database.
 A bound measure with the usual arguments will be denoted `B( Inner * Dim; Outer: Where )`
 and a free measure denoted `F( Inner * Dim; Outer: Where )`. Free views become handy expressions like
 "count(*) of any inner table" or "count(*) over dimensions of the inner table".
 
 Free measures take on the context of the inner query in a PolyMeasure, rather than referencing a basic
 view in the schema. This allows a single PolyMeasure object to perform a double aggregation over a given
-view, where we group once, then group the resulting rowset again and perform some aggregation.
+view, where we group once, then group the resulting row set again and perform some aggregation.
 
 If a free measure is supplied to the outer measure list, it will query the corresponding inner measure list.
 Free measures should not be supplied as the inner measure of a PolyMeasure, unless the outer measures can supply
 their own inner bindings.
 
 Bound measures should have a default string value for the view, appropriate to the schema.
-Using the supplied factory method BoundedMeasure will return a super-classed PolyMeasure
+Using the supplied factory method bound_objects will return a super-classed PolyMeasure and FilterExpression objects
 keyed to a specific view, for convenience.
 
 In the following examples, we assume one unique bounded measure exists,
 B = B(dim=Rowset(), inner=main_view), which acts as the ultimate "leaf" measure.
 The class Free is also provided, which defaults the measure view to Free instead, and is aliased F.
 
 The Outer and Inner arguments are PolyMeasure vectors, which each can return tables of any dimension.
 When different dimensions are supplied in the outer measures, self.dim is used to group the inner view,
 but each measure still evaluates by matching only on its own dimension, if specified.
 No attempt is made to reconcile the dimensions between inner and outer arguments - if a measure requests
 a column that doesn't exist in dim(M) (the inner dimension specified by M), then the SQL parser
 will let you know :)
 
-When supplied as an argument, a tuple is interpreted as a "Dummy PolyMeasure" (name, inner, [dim]),
+When supplied as an argument, a tuple is interpreted as a "Dummy PolyMeasure" (name, outer, [dim]),
 where dim can be omitted. These measures are always free.
 
 When defining dimensions, [] means group by the whole table,
-RowSet means do not group the view. None is a wildcard, which means the measure will default
-to the dimensions of the enclosing measure after dimension promotion.
+RowSet means do not group the view at all. None is a wildcard, which means the measure will default
+to the dimensions of the enclosing measure after dimension promotion. None and [] will behave identically in most cases.
 
 The view and where parameters are applied to the inner query, Inner * Dim.
 For example if you want to apply a filter context to Outer directly (which is the final output aggregation),
 use M( Inner * Dim; F(Outer: Where_Outer): View, Where)
 
 ==========================================
```

