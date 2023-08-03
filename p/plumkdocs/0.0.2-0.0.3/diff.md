# Comparing `tmp/plumkdocs-0.0.2.tar.gz` & `tmp/plumkdocs-0.0.3.tar.gz`

## Comparing `plumkdocs-0.0.2.tar` & `plumkdocs-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 plumkdocs-0.0.2/plumkdocs/__init__.py
--rwxr-xr-x   0        0        0     9456 2020-02-02 00:00:00.000000 plumkdocs-0.0.2/plumkdocs/main.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plumkdocs-0.0.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plumkdocs-0.0.2/LICENSE.txt
--rwxr-xr-x   0        0        0     2332 2020-02-02 00:00:00.000000 plumkdocs-0.0.2/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 plumkdocs-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 plumkdocs-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 plumkdocs-0.0.3/plumkdocs/__init__.py
+-rwxr-xr-x   0        0        0     9602 2020-02-02 00:00:00.000000 plumkdocs-0.0.3/plumkdocs/main.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plumkdocs-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plumkdocs-0.0.3/LICENSE.txt
+-rwxr-xr-x   0        0        0     3206 2020-02-02 00:00:00.000000 plumkdocs-0.0.3/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 plumkdocs-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5194 2020-02-02 00:00:00.000000 plumkdocs-0.0.3/PKG-INFO
```

### Comparing `plumkdocs-0.0.2/plumkdocs/main.py` & `plumkdocs-0.0.3/plumkdocs/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,17 +100,14 @@
                     table += f"<td>{markdown(r.description)}</td>"
                 else:
                     table += "<td></td>"
                 table += "</tr>"
             table += "</tbody></table></div></div>"
             text += table
 
-        # Add an horizontal line
-        text += "<hr>"
-
         return text
 
     @staticmethod
     def param_to_string(names, types, defaults):
         namestring = f"{names}"
         typestring = ": " + strip_modules(str(types)) if types != inspect._empty else ""
         defaultstring = f" = {defaults}" if defaults != inspect._empty else ""
@@ -196,22 +193,26 @@
         "jaxdf.core.": "",
     }
     for key, value in to_change.items():
         string = string.replace(key, value)
     return string
 
 
+def get_base_docs(plum_func):
+    _, func = plum_func[0]
+    return func._doc
+
 def _extract_implementations(plum_func):
-    name, function = plum_func
+    name, func = plum_func
     implementations = []
 
-    for signature, method in zip(function.methods.keys(), function.methods.values()):
-        method = method[0].__wrapped__
-        params = inspect.signature(method).parameters
-        docs = inspect.getdoc(method)
+    for method in func.methods:
+        implementation = method.implementation
+        params = inspect.signature(implementation).parameters
+        docs = inspect.getdoc(implementation)
 
         # Deal with empty docstrings
         docs = "" if docs is None else docs
 
         implementations.append(Implementation(name, params, docs))
 
     # Remove implementations with the same _signature
@@ -248,21 +249,27 @@
         func = func[func.keys()[0]][0].__wrapped__.__name__
         return func
 
     operators = [v for v in sorted(operators, key=lambda item: item[0])]
 
     implementations = list(map(_extract_implementations, operators))
 
+    base_docs = get_base_docs(operators)
+
     # Concatenate all implementations into a string
-    text = ""
+    text = base_docs + '\n'
+    text += "<h3>Concrete implementations:</h3>"
     for fun in implementations:
         # text += f'## `{fun[0].name}`\n\n'
         for i in fun:
             text += "".join(str(i)) + "\n"
         # text += '\n<hr/>\n'
+    
+    # Add an horizontal line
+    text += "<hr>"
     return text
 
 
 # -----------------------------------------------------------------------------
 # define_env
 # contains the macros definitions
```

### Comparing `plumkdocs-0.0.2/LICENSE.txt` & `plumkdocs-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plumkdocs-0.0.2/README.md` & `plumkdocs-0.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,68 @@
 # pluMkdocs
 
-A very, very hacky way to document multiple dispatch function implemented using the wonderful [plum](https://github.com/wesselb/plum) package
+A very, very hacky way to document multiple dispatch function implemented using the wonderful [plum](https://github.com/beartype/plum) package
 
-## Desclaimer
+## ⚠️ Desclaimer
 
 Have I mentioned that this is very hacky? It raises a whole lot of warnings, the vast majority of which I don't understand. Also, it is not heavly tested and only checked against mkdocs-material. It contains a lot of hard coded stuff and is not very flexible. It is also not very well documented.
 
-I'm uploading this with the hope that someone will find it useful and will improve it. Contributions welcome :)
+I'm uploading this with the hope that someone will find it useful and will improve it. **Contributions welcome** :)
 
 Also, I need this as a dependency for other projects, so I will probably not be able to maintain this very well.
 
 ## How to use
 
+For a quickstart, check out the example in `example_module` and the `index.md` page in the `docs` folder. To see it in action, `cd` into `example_module` and run `mkdocs serve`. 
+
+The source code contains something like this:
+
+```python
+# Define some function to test
+@dispatch.abstract
+def foo(a, b):
+    """Base description of the generic `foo` function"""
+    pass
+
+@dispatch
+def foo(a: int, b: int):
+    """Add two integers.
+
+    Args:
+        a (int): First integer.
+        b (int): Second integer.
+    
+    Returns:
+        int: Sum of a and b.
+    """
+    return a + b
+
+@dispatch
+def foo(a: str, b: str):
+    """Concatenate two strings.
+
+    Args:
+        a (str): First string.
+        b (str): Second string.
+    
+    Returns:
+        str: Concatenation of a and b.
+    """
+    return a + b
+
+...
+
+```
+
+You should see something like this in the documentation:
+
+![example](static/example.png)
+
+#### More details
+
 This package exposes an `implementations` macro that can be used to list the dispatched implementations of a function in your mkdocs.
 
 To use it, in your `mkdocs.yml` file, make sure to load the `mkdocs-macros` plugin using
 
 ```yaml
 plugins:
   macros:
@@ -40,18 +87,19 @@
     def implementations(module: str, function=None):
         return mod_to_string(module, function)
 ```
 
 In both cases, you can then use the `implementations` macro in your markdown files, like so:
 
 ```markdown
-## My awesome function
-
-Following are all the implementations for my awesome `foo` function in the package `my_package`:
-
+... some markdown ...
 
 {{ implementations('my_package', 'foo') }}
+
+... some more markdown ...
 ```
 
 This will list all the implementations of the `foo` function in the `my_package` module. The docstrings will be (hopefully) correctly formatted, and the code will be highlighted using the `pygments` syntax highlighter. The signature of each method will also be displayed.
 
+## Examples
+
 To see a working example, check out the [`jaxdf`](https://ucl-bug.github.io/jaxdf/) and [`jwave`](https://ucl-bug.github.io/jwave/) documentation.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `plumkdocs-0.0.2/pyproject.toml` & `plumkdocs-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 classifiers = [
   "Intended Audience :: Education",
   "Intended Audience :: Science/Research",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
-version="0.0.2"
+version="0.0.3"
 dependencies = [
   "pygments>=2.12.0",
   "plum-dispatch",
   "griffe",
   "markdown",
 ]
```

### Comparing `plumkdocs-0.0.2/PKG-INFO` & `plumkdocs-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plumkdocs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Hacky mkdocs documentation for plum-dispatch 
 Project-URL: Homepage, https://github.com/astanziola/plumkdocs
 Project-URL: Bug Tracker, https://github.com/astanziola/plumkdocs/issues
 Author-email: Antonio Stanziola <stanziola.antonio@gmail.com>
 License: MIT License
         
         Copyright (c) 2017 Wessel Bruinsma
@@ -37,26 +37,73 @@
 Requires-Dist: markdown
 Requires-Dist: plum-dispatch
 Requires-Dist: pygments>=2.12.0
 Description-Content-Type: text/markdown
 
 # pluMkdocs
 
-A very, very hacky way to document multiple dispatch function implemented using the wonderful [plum](https://github.com/wesselb/plum) package
+A very, very hacky way to document multiple dispatch function implemented using the wonderful [plum](https://github.com/beartype/plum) package
 
-## Desclaimer
+## ⚠️ Desclaimer
 
 Have I mentioned that this is very hacky? It raises a whole lot of warnings, the vast majority of which I don't understand. Also, it is not heavly tested and only checked against mkdocs-material. It contains a lot of hard coded stuff and is not very flexible. It is also not very well documented.
 
-I'm uploading this with the hope that someone will find it useful and will improve it. Contributions welcome :)
+I'm uploading this with the hope that someone will find it useful and will improve it. **Contributions welcome** :)
 
 Also, I need this as a dependency for other projects, so I will probably not be able to maintain this very well.
 
 ## How to use
 
+For a quickstart, check out the example in `example_module` and the `index.md` page in the `docs` folder. To see it in action, `cd` into `example_module` and run `mkdocs serve`. 
+
+The source code contains something like this:
+
+```python
+# Define some function to test
+@dispatch.abstract
+def foo(a, b):
+    """Base description of the generic `foo` function"""
+    pass
+
+@dispatch
+def foo(a: int, b: int):
+    """Add two integers.
+
+    Args:
+        a (int): First integer.
+        b (int): Second integer.
+    
+    Returns:
+        int: Sum of a and b.
+    """
+    return a + b
+
+@dispatch
+def foo(a: str, b: str):
+    """Concatenate two strings.
+
+    Args:
+        a (str): First string.
+        b (str): Second string.
+    
+    Returns:
+        str: Concatenation of a and b.
+    """
+    return a + b
+
+...
+
+```
+
+You should see something like this in the documentation:
+
+![example](static/example.png)
+
+#### More details
+
 This package exposes an `implementations` macro that can be used to list the dispatched implementations of a function in your mkdocs.
 
 To use it, in your `mkdocs.yml` file, make sure to load the `mkdocs-macros` plugin using
 
 ```yaml
 plugins:
   macros:
@@ -81,18 +128,19 @@
     def implementations(module: str, function=None):
         return mod_to_string(module, function)
 ```
 
 In both cases, you can then use the `implementations` macro in your markdown files, like so:
 
 ```markdown
-## My awesome function
-
-Following are all the implementations for my awesome `foo` function in the package `my_package`:
-
+... some markdown ...
 
 {{ implementations('my_package', 'foo') }}
+
+... some more markdown ...
 ```
 
 This will list all the implementations of the `foo` function in the `my_package` module. The docstrings will be (hopefully) correctly formatted, and the code will be highlighted using the `pygments` syntax highlighter. The signature of each method will also be displayed.
 
+## Examples
+
 To see a working example, check out the [`jaxdf`](https://ucl-bug.github.io/jaxdf/) and [`jwave`](https://ucl-bug.github.io/jwave/) documentation.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

