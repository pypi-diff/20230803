# Comparing `tmp/markmini-0.2.0.tar.gz` & `tmp/markmini-0.3.0.tar.gz`

## Comparing `markmini-0.2.0.tar` & `markmini-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      229 1970-01-01 00:00:00.000000 markmini-0.2.0/local_dependencies/markmini/Cargo.toml
--rw-r--r--   0     1001      123     9370 2023-08-02 15:41:18.000000 markmini-0.2.0/local_dependencies/markmini/src/lib.rs
--rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 markmini-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123      434 2023-08-02 15:41:18.000000 markmini-0.2.0/README.md
--rw-r--r--   0     1001      123        0 2023-08-02 15:41:18.000000 markmini-0.2.0/__init__.py
--rw-r--r--   0     1001      123       23 2023-08-02 15:41:18.000000 markmini-0.2.0/devreq.txt
--rw-r--r--   0     1001      123        0 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/__init__.py
--rw-r--r--   0     1001      123      979 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/main.py
--rw-r--r--   0     1001      123    15406 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/static/favicon.ico
--rw-r--r--   0     1001      123      493 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/static/main.js
--rw-r--r--   0     1001      123      298 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/static/styles.css
--rw-r--r--   0     1001      123      521 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/templates/index.html
--rw-r--r--   0     1001      123      265 2023-08-02 15:41:18.000000 markmini-0.2.0/markmini.pyi
--rw-r--r--   0     1001      123      316 2023-08-02 15:41:18.000000 markmini-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123      159 2023-08-02 15:41:18.000000 markmini-0.2.0/rundev.py
--rw-r--r--   0     1001      123     1120 2023-08-02 15:41:18.000000 markmini-0.2.0/src/lib.rs
--rw-r--r--   0        0        0    19244 2023-08-02 15:42:06.000000 markmini-0.2.0/Cargo.lock
--rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 markmini-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      229 1970-01-01 00:00:00.000000 markmini-0.3.0/local_dependencies/markmini/Cargo.toml
+-rw-r--r--   0     1001      123     9370 2023-08-03 13:51:14.000000 markmini-0.3.0/local_dependencies/markmini/src/lib.rs
+-rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 markmini-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123      434 2023-08-03 13:51:14.000000 markmini-0.3.0/README.md
+-rw-r--r--   0     1001      123        0 2023-08-03 13:51:14.000000 markmini-0.3.0/__init__.py
+-rw-r--r--   0     1001      123       23 2023-08-03 13:51:14.000000 markmini-0.3.0/devreq.txt
+-rw-r--r--   0     1001      123        0 2023-08-03 13:51:14.000000 markmini-0.3.0/devserver/__init__.py
+-rw-r--r--   0     1001      123      979 2023-08-03 13:51:14.000000 markmini-0.3.0/devserver/main.py
+-rw-r--r--   0     1001      123    15406 2023-08-03 13:51:14.000000 markmini-0.3.0/devserver/static/favicon.ico
+-rw-r--r--   0     1001      123      493 2023-08-03 13:51:14.000000 markmini-0.3.0/devserver/static/main.js
+-rw-r--r--   0     1001      123      298 2023-08-03 13:51:14.000000 markmini-0.3.0/devserver/static/styles.css
+-rw-r--r--   0     1001      123      521 2023-08-03 13:51:14.000000 markmini-0.3.0/devserver/templates/index.html
+-rw-r--r--   0     1001      123      265 2023-08-03 13:51:14.000000 markmini-0.3.0/markmini.pyi
+-rw-r--r--   0     1001      123      316 2023-08-03 13:51:14.000000 markmini-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123      159 2023-08-03 13:51:14.000000 markmini-0.3.0/rundev.py
+-rw-r--r--   0     1001      123     1255 2023-08-03 13:51:14.000000 markmini-0.3.0/src/lib.rs
+-rw-r--r--   0        0        0    19244 2023-08-03 13:52:06.000000 markmini-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 markmini-0.3.0/PKG-INFO
```

### Comparing `markmini-0.2.0/local_dependencies/markmini/src/lib.rs` & `markmini-0.3.0/local_dependencies/markmini/src/lib.rs`

 * *Files identical despite different names*

### Comparing `markmini-0.2.0/devserver/main.py` & `markmini-0.3.0/devserver/main.py`

 * *Files identical despite different names*

### Comparing `markmini-0.2.0/devserver/static/favicon.ico` & `markmini-0.3.0/devserver/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `markmini-0.2.0/devserver/templates/index.html` & `markmini-0.3.0/devserver/templates/index.html`

 * *Files identical despite different names*

### Comparing `markmini-0.2.0/src/lib.rs` & `markmini-0.3.0/src/lib.rs`

 * *Files 21% similar despite different names*

```diff
@@ -8,23 +8,27 @@
     internal: _Markmini,
 }
 
 #[pymethods]
 impl Markmini {
     #[new]
     pub fn new() -> Self {
-        Self {
+        return Self {
             internal: _Markmini::new(),
-        }
+        };
     }
 
     pub fn compile(&self, input: &str) -> String {
         return self.internal.compile(input);
     }
 
+    pub fn compile_comment(&self, input: &str) -> String {
+        return self.internal.compile_comment(input);
+    }
+
     pub fn add_users(
         &mut self,
         usernames: Vec<String>,
         user_ids: Vec<String>,
         links: Vec<String>,
         fullnames: Vec<String>,
     ) {
@@ -41,9 +45,9 @@
     }
 }
 
 // This function is the entrypoint to the python module
 #[pymodule]
 fn markmini_py(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<Markmini>()?;
-    Ok(())
+    return Ok(());
 }
```

### Comparing `markmini-0.2.0/Cargo.lock` & `markmini-0.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -181,24 +181,24 @@
  "lazy_static",
  "pulldown-cmark",
  "regex-lite",
 ]
 
 [[package]]
 name = "markmini-py"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "itertools",
  "markmini",
  "pyo3",
 ]
 
 [[package]]
 name = "markmini-wasm"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "js-sys",
  "markmini",
  "wasm-bindgen",
 ]
 
 [[package]]
```

### Comparing `markmini-0.2.0/PKG-INFO` & `markmini-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markmini
-Version: 0.2.0
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Markmini
```

