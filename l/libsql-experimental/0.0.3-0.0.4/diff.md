# Comparing `tmp/libsql_experimental-0.0.3.tar.gz` & `tmp/libsql_experimental-0.0.4.tar.gz`

## Comparing `libsql_experimental-0.0.3.tar` & `libsql_experimental-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      330 1970-01-01 00:00:00.000000 libsql_experimental-0.0.3/Cargo.toml
--rw-r--r--   0     1001      123     2040 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123       12 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/.gitignore
--rw-r--r--   0     1001      123     1071 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/LICENSE.md
--rw-r--r--   0     1001      123     2436 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/README.md
--rw-r--r--   0     1001      123       10 2023-07-31 09:44:03.000000 libsql_experimental-0.0.3/dist/libsql_experimental-0.0.3.tar.gz
--rw-r--r--   0     1001      123      271 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/example.py
--rwxr-xr-x   0     1001      123      278 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/perf-libsql.py
--rwxr-xr-x   0     1001      123      254 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/perf-sqlite3.py
--rw-r--r--   0     1001      123      379 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/pyproject.toml
--rw-r--r--   0     1001      123     4419 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/src/lib.rs
--rw-r--r--   0     1001      123     1102 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/tests/test_basic.py
--rw-r--r--   0     1001      123    43847 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/Cargo.lock
--rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 libsql_experimental-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      330 1970-01-01 00:00:00.000000 libsql_experimental-0.0.4/Cargo.toml
+-rw-r--r--   0     1001      123     2040 2023-08-03 11:10:53.000000 libsql_experimental-0.0.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123       12 2023-08-03 11:10:53.000000 libsql_experimental-0.0.4/.gitignore
+-rw-r--r--   0     1001      123     1071 2023-08-03 11:10:53.000000 libsql_experimental-0.0.4/LICENSE.md
+-rw-r--r--   0     1001      123     2436 2023-08-03 11:10:53.000000 libsql_experimental-0.0.4/README.md
+-rw-r--r--   0     1001      123       10 2023-08-03 11:12:42.000000 libsql_experimental-0.0.4/dist/libsql_experimental-0.0.4.tar.gz
+-rw-r--r--   0     1001      123      271 2023-08-03 11:10:53.000000 libsql_experimental-0.0.4/example.py
+-rwxr-xr-x   0     1001      123      278 2023-08-03 11:10:53.000000 libsql_experimental-0.0.4/perf-libsql.py
+-rwxr-xr-x   0     1001      123      254 2023-08-03 11:10:53.000000 libsql_experimental-0.0.4/perf-sqlite3.py
+-rw-r--r--   0     1001      123      379 2023-08-03 11:10:53.000000 libsql_experimental-0.0.4/pyproject.toml
+-rw-r--r--   0     1001      123     4971 2023-08-03 11:10:53.000000 libsql_experimental-0.0.4/src/lib.rs
+-rw-r--r--   0     1001      123     1597 2023-08-03 11:10:53.000000 libsql_experimental-0.0.4/tests/test_basic.py
+-rw-r--r--   0     1001      123    43847 2023-08-03 11:10:53.000000 libsql_experimental-0.0.4/Cargo.lock
+-rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 libsql_experimental-0.0.4/PKG-INFO
```

### Comparing `libsql_experimental-0.0.3/.github/workflows/CI.yml` & `libsql_experimental-0.0.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `libsql_experimental-0.0.3/LICENSE.md` & `libsql_experimental-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `libsql_experimental-0.0.3/README.md` & `libsql_experimental-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `libsql_experimental-0.0.3/src/lib.rs` & `libsql_experimental-0.0.4/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
-use pyo3::types::PyTuple;
+use pyo3::types::{PyList, PyTuple};
 
 use ::libsql as libsql_core;
 
 fn to_py_err(error: libsql_core::errors::Error) -> PyErr {
     PyValueError::new_err(format!("{}", error))
 }
 
 #[pyfunction]
 #[pyo3(signature = (database, sync_url=None))]
 fn connect(database: String, sync_url: Option<String>) -> PyResult<Connection> {
     let rt = tokio::runtime::Runtime::new().unwrap();
     let db = match sync_url {
         Some(sync_url) => {
             let opts = libsql_core::Opts::with_http_sync(sync_url);
-            rt.block_on(libsql_core::Database::open_with_opts(database, opts)).map_err(to_py_err)?
-        },
+            rt.block_on(libsql_core::Database::open_with_opts(database, opts))
+                .map_err(to_py_err)?
+        }
         None => libsql_core::Database::open(database).map_err(to_py_err)?,
     };
     Ok(Connection { db, rt })
 }
 
 #[pyclass]
 pub struct Connection {
@@ -87,40 +88,65 @@
 impl Result {
     fn fetchone(self_: PyRef<'_, Self>) -> PyResult<Option<&PyTuple>> {
         match self_.rows {
             Some(ref rows) => {
                 let row = rows.next().map_err(to_py_err)?;
                 match row {
                     Some(row) => {
-                        let mut elements: Vec<Py<PyAny>> = vec![];
-                        for col_idx in 0..rows.column_count() {
-                            let col_type = row.column_type(col_idx).map_err(to_py_err)?;
-                            let value = match col_type {
-                                libsql_core::ValueType::Integer => {
-                                    let value = row.get::<i32>(col_idx).map_err(to_py_err)?;
-                                    value.into_py(self_.py())
-                                }
-                                libsql_core::ValueType::Real => todo!(),
-                                libsql_core::ValueType::Blob => todo!(),
-                                libsql_core::ValueType::Text => {
-                                    let value = row.get::<&str>(col_idx).map_err(to_py_err)?;
-                                    value.into_py(self_.py())
-                                }
-                                libsql_core::ValueType::Null => todo!(),
-                            };
-                            elements.push(value);
-                        }
-                        Ok(Some(PyTuple::new(self_.py(), elements)))
+                        let row = convert_row(self_.py(), row, rows.column_count())?;
+                        Ok(Some(row))
                     }
                     None => Ok(None),
                 }
             }
             None => Ok(None),
         }
     }
+
+    fn fetchall(self_: PyRef<'_, Self>) -> PyResult<Option<&PyList>> {
+        match self_.rows {
+            Some(ref rows) => {
+                let mut elements: Vec<Py<PyAny>> = vec![];
+                loop {
+                    let row = rows.next().map_err(to_py_err)?;
+                    match row {
+                        Some(row) => {
+                            let row = convert_row(self_.py(), row, rows.column_count())?;
+                            elements.push(row.into());
+                        }
+                        None => break,
+                    }
+                }
+                Ok(Some(PyList::new(self_.py(), elements)))
+            }
+            None => Ok(None),
+        }
+    }
+}
+
+fn convert_row(py: Python, row: libsql_core::rows::Row, column_count: i32) -> PyResult<&PyTuple> {
+    let mut elements: Vec<Py<PyAny>> = vec![];
+    for col_idx in 0..column_count {
+        let col_type = row.column_type(col_idx).map_err(to_py_err)?;
+        let value = match col_type {
+            libsql_core::ValueType::Integer => {
+                let value = row.get::<i32>(col_idx).map_err(to_py_err)?;
+                value.into_py(py)
+            }
+            libsql_core::ValueType::Real => todo!(),
+            libsql_core::ValueType::Blob => todo!(),
+            libsql_core::ValueType::Text => {
+                let value = row.get::<&str>(col_idx).map_err(to_py_err)?;
+                value.into_py(py)
+            }
+            libsql_core::ValueType::Null => todo!(),
+        };
+        elements.push(value);
+    }
+    Ok(PyTuple::new(py, elements))
 }
 
 #[pymodule]
 fn libsql_experimental(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(connect, m)?)?;
     m.add_class::<Connection>()?;
     m.add_class::<Cursor>()?;
```

### Comparing `libsql_experimental-0.0.3/Cargo.lock` & `libsql_experimental-0.0.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -599,15 +599,15 @@
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "libsql-python"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
  "libsql",
  "pyo3",
  "tokio",
 ]
 
 [[package]]
```

### Comparing `libsql_experimental-0.0.3/PKG-INFO` & `libsql_experimental-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsql-experimental
-Version: 0.0.3
+Version: 0.0.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

