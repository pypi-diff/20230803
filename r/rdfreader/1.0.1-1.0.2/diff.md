# Comparing `tmp/rdfreader-1.0.1.tar.gz` & `tmp/rdfreader-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfreader-1.0.1.tar", max compression
+gzip compressed data, was "rdfreader-1.0.2.tar", max compression
```

## Comparing `rdfreader-1.0.1.tar` & `rdfreader-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3771 2023-06-15 08:56:21.444375 rdfreader-1.0.1/README.md
--rw-r--r--   0        0        0     1056 2023-06-15 08:56:21.448375 rdfreader-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       49 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/chem/__init__.py
--rw-r--r--   0        0        0     4977 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/chem/mol.py
--rw-r--r--   0        0        0     4775 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/chem/reaction.py
--rw-r--r--   0        0        0      881 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/chem/utils.py
--rw-r--r--   0        0        0      246 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/exceptions.py
--rw-r--r--   0        0        0     2758 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/parse/molblock.py
--rw-r--r--   0        0        0     8105 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/parse/rxnblock.py
--rw-r--r--   0        0        0    10225 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/parse/utils.py
--rw-r--r--   0        0        0     4951 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/rdf.py
--rw-r--r--   0        0        0      985 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/write.py
--rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 rdfreader-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3771 2023-08-03 09:13:30.571225 rdfreader-1.0.2/README.md
+-rw-r--r--   0        0        0     1061 2023-08-03 09:13:30.575225 rdfreader-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-08-03 09:13:30.575225 rdfreader-1.0.2/rdfreader/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 09:13:30.575225 rdfreader-1.0.2/rdfreader/chem/__init__.py
+-rw-r--r--   0        0        0     4977 2023-08-03 09:13:30.575225 rdfreader-1.0.2/rdfreader/chem/mol.py
+-rw-r--r--   0        0        0     4775 2023-08-03 09:13:30.575225 rdfreader-1.0.2/rdfreader/chem/reaction.py
+-rw-r--r--   0        0        0      881 2023-08-03 09:13:30.575225 rdfreader-1.0.2/rdfreader/chem/utils.py
+-rw-r--r--   0        0        0      246 2023-08-03 09:13:30.575225 rdfreader-1.0.2/rdfreader/exceptions.py
+-rw-r--r--   0        0        0     2758 2023-08-03 09:13:30.575225 rdfreader-1.0.2/rdfreader/parse/molblock.py
+-rw-r--r--   0        0        0     8105 2023-08-03 09:13:30.575225 rdfreader-1.0.2/rdfreader/parse/rxnblock.py
+-rw-r--r--   0        0        0    10329 2023-08-03 09:13:30.575225 rdfreader-1.0.2/rdfreader/parse/utils.py
+-rw-r--r--   0        0        0     4951 2023-08-03 09:13:30.575225 rdfreader-1.0.2/rdfreader/rdf.py
+-rw-r--r--   0        0        0      985 2023-08-03 09:13:30.575225 rdfreader-1.0.2/rdfreader/write.py
+-rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 rdfreader-1.0.2/PKG-INFO
```

### Comparing `rdfreader-1.0.1/README.md` & `rdfreader-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.1/pyproject.toml` & `rdfreader-1.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "rdfreader"
-version = "1.0.1"  
+version = "1.0.2"
 description = "Read the full contents of CTAB .rdf files in python. Captures RXN and MOL record using RDKit and reads additional data fields (including solvents/catalysts/agents)."
 authors = ["deepmatter <enquiries@deepmatter.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/deepmatterltd/rdfreader/"
 homepage = "https://www.deepmatter.io"
 keywords = ["chemistry", "rdkit", "rdf", "rxn", "mol", "reaction", "molecule", "reader", "parser", "deepmatter", "ctab", "cheminformatics"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering :: Chemistry",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9, <4.0"
 rdkit = "^2022.9.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pre-commit = "^2.20.0"
 pytest-mock = "^3.10.0"
 sphinx = "^6.2.1"
```

### Comparing `rdfreader-1.0.1/rdfreader/chem/mol.py` & `rdfreader-1.0.2/rdfreader/chem/mol.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.1/rdfreader/chem/reaction.py` & `rdfreader-1.0.2/rdfreader/chem/reaction.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.1/rdfreader/chem/utils.py` & `rdfreader-1.0.2/rdfreader/chem/utils.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.1/rdfreader/parse/molblock.py` & `rdfreader-1.0.2/rdfreader/parse/molblock.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.1/rdfreader/parse/rxnblock.py` & `rdfreader-1.0.2/rdfreader/parse/rxnblock.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.1/rdfreader/parse/utils.py` & `rdfreader-1.0.2/rdfreader/parse/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,14 +285,17 @@
     # add a leading underscore if string starts with a number
     if string[0].isdigit():
         string = f"_{string}"
 
     # replace all non-alphanumeric characters with an underscore
     string = re.sub(r"[^a-zA-Z0-9_]", "_", string)
 
+    # replace multiple underscores with a single underscore
+    string = re.sub(r"_{2,}", "_", string)
+
     # lower case the string
     string = string.lower()
 
     # remove trailing underscores
     string = string.rstrip("_")
 
     return string
```

### Comparing `rdfreader-1.0.1/rdfreader/rdf.py` & `rdfreader-1.0.2/rdfreader/rdf.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.1/rdfreader/write.py` & `rdfreader-1.0.2/rdfreader/write.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.1/PKG-INFO` & `rdfreader-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfreader
-Version: 1.0.1
+Version: 1.0.2
 Summary: Read the full contents of CTAB .rdf files in python. Captures RXN and MOL record using RDKit and reads additional data fields (including solvents/catalysts/agents).
 Home-page: https://www.deepmatter.io
 License: MIT
 Keywords: chemistry,rdkit,rdf,rxn,mol,reaction,molecule,reader,parser,deepmatter,ctab,cheminformatics
 Author: deepmatter
 Author-email: enquiries@deepmatter.io
 Requires-Python: >=3.9,<4.0
```

