# Comparing `tmp/svbench-0.7.5.tar.gz` & `tmp/svbench-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svbench-0.7.5.tar", last modified: Wed Jul 26 12:52:03 2023, max compression
+gzip compressed data, was "svbench-0.7.6.tar", last modified: Thu Aug  3 12:22:02 2023, max compression
```

## Comparing `svbench-0.7.5.tar` & `svbench-0.7.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-26 12:52:03.017789 svbench-0.7.5/
--rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.5/LICENSE.md
--rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.5/MANIFEST.in
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-26 12:52:03.017352 svbench-0.7.5/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.5/README.rst
--rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-07-26 12:52:03.017876 svbench-0.7.5/setup.cfg
--rw-r--r--   0 kezcleal   (501) staff       (20)      496 2023-07-26 08:33:38.000000 svbench-0.7.5/setup.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-26 12:52:03.004702 svbench-0.7.5/svbench/
--rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.5/svbench/.DS_Store
--rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.5/svbench/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     1989 2023-07-19 14:28:51.000000 svbench-0.7.5/svbench/cli.py
--rw-r--r--   0 kezcleal   (501) staff       (20)    71379 2023-07-26 08:37:49.000000 svbench-0.7.5/svbench/io_tools.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.5/svbench/loaders.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-26 12:52:03.016952 svbench-0.7.5/svbench/models/
--rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.5/svbench/models/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.5/svbench/quant_tools.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-26 12:52:03.016545 svbench-0.7.5/svbench.egg-info/
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/SOURCES.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/dependency_links.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/entry_points.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       56 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/requires.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-07-26 12:52:02.000000 svbench-0.7.5/svbench.egg-info/top_level.txt
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-08-03 12:22:02.941811 svbench-0.7.6/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.6/LICENSE.md
+-rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.6/MANIFEST.in
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-08-03 12:22:02.941297 svbench-0.7.6/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1293 2023-07-28 09:45:21.000000 svbench-0.7.6/README.rst
+-rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-08-03 12:22:02.941944 svbench-0.7.6/setup.cfg
+-rw-r--r--   0 kezcleal   (501) staff       (20)      496 2023-08-03 09:36:12.000000 svbench-0.7.6/setup.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-08-03 12:22:02.927940 svbench-0.7.6/svbench/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.6/svbench/.DS_Store
+-rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.6/svbench/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     2390 2023-08-03 10:46:28.000000 svbench-0.7.6/svbench/cli.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)    71534 2023-08-03 09:35:44.000000 svbench-0.7.6/svbench/io_tools.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.6/svbench/loaders.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-08-03 12:22:02.940775 svbench-0.7.6/svbench/models/
+-rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.6/svbench/models/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.6/svbench/quant_tools.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-08-03 12:22:02.940058 svbench-0.7.6/svbench.egg-info/
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-08-03 12:22:02.000000 svbench-0.7.6/svbench.egg-info/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-08-03 12:22:02.000000 svbench-0.7.6/svbench.egg-info/SOURCES.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-08-03 12:22:02.000000 svbench-0.7.6/svbench.egg-info/dependency_links.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-08-03 12:22:02.000000 svbench-0.7.6/svbench.egg-info/entry_points.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       56 2023-08-03 12:22:02.000000 svbench-0.7.6/svbench.egg-info/requires.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-08-03 12:22:02.000000 svbench-0.7.6/svbench.egg-info/top_level.txt
```

### Comparing `svbench-0.7.5/LICENSE.md` & `svbench-0.7.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `svbench-0.7.5/svbench/.DS_Store` & `svbench-0.7.6/svbench/.DS_Store`

 * *Files identical despite different names*

### Comparing `svbench-0.7.5/svbench/cli.py` & `svbench-0.7.6/svbench/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,37 @@
 version = pkg_resources.require("svbench")[0].version
 
 
 @click.command()
 @click.argument('reference_vcf', required=True, type=click.Path())
 @click.argument('query_vcfs', required=True, type=click.Path(), nargs=-1)
 @click.option("--include", help="Include regions .bed file", type=click.Path(), show_default=False, required=False)
-@click.option("--pass-only", help="Assess only PASS variants", is_flag=True, flag_value=True, show_default=False, default=False)
+@click.option("--pass-only", help="Assess only PASS variants in both reference and query", is_flag=True, flag_value=True, show_default=False, default=False)
+@click.option("--pass-ref", help="Assess only PASS variants in reference", is_flag=True, flag_value=True, show_default=False, default=False)
+@click.option("--pass-query", help="Assess only PASS variants in query", is_flag=True, flag_value=True, show_default=False, default=False)
 @click.option("--slop", help="Add intervals +/- slop around breakpoints", default=250, type=int, show_default=True)
 @click.option("--min-size-ref", help="Min SV length", default=0, type=int, show_default=True)
 @click.option("--min-size-query", help="Min SV length", default=30, type=int, show_default=True)
 @click.option("--no-duplicates", help="Don't quantify duplicate true positives", is_flag=True, flag_value=True, show_default=False, default=False)
 @click.version_option()
-def main(reference_vcf, query_vcfs, include, pass_only, slop, min_size_ref, min_size_query, no_duplicates):
-    keep = [svb.Col("FILTER", op="eq", thresh=None)] if pass_only else []
+def main(reference_vcf, query_vcfs, include, pass_only, pass_ref, pass_query, slop, min_size_ref, min_size_query, no_duplicates):
+
+    keep = [svb.Col("FILTER", op="eq", thresh=None)] if pass_only or pass_ref else []
+
     ref = CallSet(dataset="REFERENCE", no_translocations=False).\
         load_vcf(reference_vcf, other_cols=["FILTER"], keep=keep). \
         filter_by_size(min_size_ref, None, keep_translocations=True)
 
     if include:
         ref.filter_include_bed(include, inplace=True)
-    # print(ref.breaks_df.head())
+
     ref.add_intervals(slop)
+    keep2 = [svb.Col("FILTER", op="eq", thresh=None)] if pass_only or pass_query else []
     query = [CallSet(dataset="REFERENCE", caller=path.split("/")[-1], no_translocations=False).
-             load_vcf(path, other_cols=["FILTER"], keep=keep).filter_by_size(min_size_query, None, keep_translocations=True)
+             load_vcf(path, other_cols=["FILTER"], keep=keep2).filter_by_size(min_size_query, None, keep_translocations=True)
              for path in query_vcfs]
 
     if include:
         [i.filter_include_bed(include, inplace=True) for i in query]
     svb.score(ref, query, allow_duplicate_tp=not no_duplicates)
```

### Comparing `svbench-0.7.5/svbench/io_tools.py` & `svbench-0.7.6/svbench/io_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -681,15 +681,17 @@
             df = v.breaks_df
             if df is not None and ol_tree is not None:
                 for index, chrom, start, chrom2, end in zip(df.index, df.chrom, df.start, df.chrom2, df.end):
                     if ol_tree:
                         if chrom not in ol_tree:
                             bad_i.add(index)
                         else:
-                            if not any(ol_tree[chrom].ncls.find_overlap(start, start + 1)) or not any(ol_tree[chrom2].ncls.find_overlap(end, end + 1)):
+                            if chrom not in ol_tree or (chrom2 != chrom and chrom2 not in ol_tree):
+                                bad_i.add(index)
+                            elif not any(ol_tree[chrom].ncls.find_overlap(start, start + 1)) or not any(ol_tree[chrom2].ncls.find_overlap(end, end + 1)):
                                 bad_i.add(index)
             v.breaks_df = v.breaks_df.drop(bad_i)
 
         print("Filtered by include_bed, caller={}, dataset={} rows before {}, after {}".format(v.caller, v.dataset,
                                                                                           l_before,
                                                                                           l_before - len(bad_i)),
               file=stderr)
@@ -873,15 +875,15 @@
                     skip_this = False
                     for m in mate:
                         if m in ignore_mates:
                             skip_this = True
                             break
                         ignore_mates.add(m)
                     if skip_this:
-                        continue
+                            continue
 
             start = int(r.POS)
 
             if ol_tree and chrom in ol_tree:
                 if any(ol_tree[chrom].ncls.find_overlap(start, start + 1)):
                     ol_start = True
                 if not ol_start and include_if == "both":
```

### Comparing `svbench-0.7.5/svbench/loaders.py` & `svbench-0.7.6/svbench/loaders.py`

 * *Files identical despite different names*

### Comparing `svbench-0.7.5/svbench/quant_tools.py` & `svbench-0.7.6/svbench/quant_tools.py`

 * *Files identical despite different names*

