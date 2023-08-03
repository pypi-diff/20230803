# Comparing `tmp/gridworks_cert-0.3.2.tar.gz` & `tmp/gridworks_cert-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_cert-0.3.2.tar", max compression
+gzip compressed data, was "gridworks_cert-0.4.0.tar", max compression
```

## Comparing `gridworks_cert-0.3.2.tar` & `gridworks_cert-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-07-31 14:57:45.144558 gridworks_cert-0.3.2/LICENSE
--rw-r--r--   0        0        0     4088 2023-07-31 14:58:05.818039 gridworks_cert-0.3.2/README.md
--rw-r--r--   0        0        0     2164 2023-07-31 14:58:05.818039 gridworks_cert-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/__init__.py
--rw-r--r--   0        0        0      658 2023-07-31 14:58:05.818039 gridworks_cert-0.3.2/src/gwcert/__main__.py
--rw-r--r--   0        0        0       99 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/ca/__init__.py
--rw-r--r--   0        0        0     7416 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/ca/__main__.py
--rw-r--r--   0        0        0      172 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/key/__init__.py
--rw-r--r--   0        0        0    21477 2023-07-31 14:58:05.818039 gridworks_cert-0.3.2/src/gwcert/key/__main__.py
--rw-r--r--   0        0        0      196 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/paths.py
--rw-r--r--   0        0        0        0 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/py.typed
--rw-r--r--   0        0        0     5087 1970-01-01 00:00:00.000000 gridworks_cert-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-03 00:13:35.035691 gridworks_cert-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4088 2023-08-03 00:13:35.035691 gridworks_cert-0.4.0/README.md
+-rw-r--r--   0        0        0     2165 2023-08-03 00:13:56.732980 gridworks_cert-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/__init__.py
+-rw-r--r--   0        0        0      658 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/__main__.py
+-rw-r--r--   0        0        0       99 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/ca/__init__.py
+-rw-r--r--   0        0        0     7416 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/ca/__main__.py
+-rw-r--r--   0        0        0      172 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/key/__init__.py
+-rw-r--r--   0        0        0    22025 2023-08-03 00:13:56.732980 gridworks_cert-0.4.0/src/gwcert/key/__main__.py
+-rw-r--r--   0        0        0      196 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/paths.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/py.typed
+-rw-r--r--   0        0        0     5080 1970-01-01 00:00:00.000000 gridworks_cert-0.4.0/PKG-INFO
```

### Comparing `gridworks_cert-0.3.2/LICENSE` & `gridworks_cert-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.3.2/README.md` & `gridworks_cert-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.3.2/pyproject.toml` & `gridworks_cert-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-cert"
-version = "0.3.2"
+version = "0.4.0"
 description = "TLS certificate management tools for GridWorks"
 authors = ["Andrew Schweitzer <schweitz72@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-cert"
 repository = "https://github.com/thegridelectric/gridworks-cert"
 documentation = "https://gridworks-cert.readthedocs.io"
@@ -20,15 +20,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ownca = ">=0.4.0"
 typer = ">=0.9.0"
 xdg = ">=6.0.0"
 rich = ">=12.0.0"
-trogon = "^0.5.0"
+trogon = ">=0.5.0"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `gridworks_cert-0.3.2/src/gwcert/__main__.py` & `gridworks_cert-0.4.0/src/gwcert/__main__.py`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.3.2/src/gwcert/ca/__main__.py` & `gridworks_cert-0.4.0/src/gwcert/ca/__main__.py`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.3.2/src/gwcert/key/__main__.py` & `gridworks_cert-0.4.0/src/gwcert/key/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,18 @@
             )
     else:
         # explicit output path specified. Parameters output_suffix and certs_dir will be ignored.
         output_path = name_as_path
     return output_path
 
 
+def _private_from_public_path(public_path: Path, private_suffix: str = ".pem") -> Path:
+    return public_path.parent / "private" / (public_path.stem + private_suffix)
+
+
 def _store_file(
     output_path: Path,
     data_bytes: bytes,
     permission: Optional[int] = None,
 ) -> None:
     parent_dir = output_path.parent
     if not parent_dir.exists():
@@ -112,17 +116,26 @@
 
 
 @app.command()
 def rsa(
     name: Annotated[
         str,
         typer.Argument(
-            help="'name' of generated key, or explict path to generated key file."
+            help="'name' of generated key, or explict path to generated public key file."
         ),
     ],
+    private_key_path: Annotated[
+        Optional[Path],
+        typer.Option(
+            help=(
+                "Optional explicit path to private key file. If absent, private key path is derived from "
+                "public key output path."
+            )
+        ),
+    ] = None,
     certs_dir: Annotated[
         Path, typer.Option(help="Base storage directory for named certs")
     ] = DEFAULT_CERTS_DIR,
     public_exponent: Annotated[
         int,
         typer.Option(
             help="The public exponent of the new key. Either 65537 or 3 (for legacy purposes). Almost everyone should use 65537."
@@ -146,22 +159,23 @@
 ) -> None:
     """
     Create public/private key pair using RSA.
 
     Writes public and private key files, by default named:
 
         $HOME/.local/share/gridworks/ca/certs/name/name.pub
-        $HOME/.local/share/gridworks/ca/certs/name/name.pem
+        $HOME/.local/share/gridworks/ca/certs/name/private/name.pem
 
     Output files can be explicitly named by passing a path-like string for a ".pem" file to the name parameter.
     """
-    private_key_path = get_output_path(
-        name_or_output_path=name, output_suffix=".pem", certs_dir=certs_dir
+    public_key_path = get_output_path(
+        name_or_output_path=name, output_suffix=".pub", certs_dir=certs_dir
     )
-    public_key_path = private_key_path.with_suffix(".pub")
+    if private_key_path is None:
+        private_key_path = _private_from_public_path(public_key_path)
     if not force and (private_key_path.exists() or public_key_path.exists()):
         rich.print(
             "One or more output files [yellow][bold]already exist. Doing nothing.[/yellow][/bold]"
         )
         rich.print(
             f"  private key file  exists:{str(private_key_path.exists()):5s}  {private_key_path}"
         )
@@ -233,15 +247,15 @@
     ] = False,
 ) -> None:
     """
     Create Certificate Signing Request from a private key.
 
     Uses input files, by default named:
 
-        $HOME/.local/share/gridworks/ca/certs/name/name.pub
+        $HOME/.local/share/gridworks/ca/certs/name/private/name.pem
 
     Writes a CSR file, by default named:
 
         $HOME/.local/share/gridworks/ca/certs/name/name.csr
 
     Input file can be explicitly named with the --private-key-path paramter.
     Output file can be explicitly named by passing a path-like string for a ".csr" file to the name parameter.
@@ -252,20 +266,19 @@
     )
     if not force and csr_path.exists():
         rich.print(
             f"CSR file {csr_path} [yellow][bold]already exists. Doing nothing.[/yellow][/bold]"
         )
         rich.print("\nUse --force to overwrite csr file")
         return
-    if private_key_path is None:
-        private_key_path = csr_path.with_suffix(".pem")
 
+    if private_key_path is None:
+        private_key_path = _private_from_public_path(csr_path)
     if not private_key_path.exists():
         raise ValueError(f"Private key path {private_key_path} does not exist")
-
     with private_key_path.open("rb") as f:
         key = serialization.load_pem_private_key(f.read(), password=None)
 
     if not common_name:
         common_name = csr_path.stem
 
     if not dns_names:
@@ -480,32 +493,32 @@
 
 @app.command()
 def add(
     ctx: typer.Context,
     name: Annotated[
         str,
         typer.Argument(
-            help="'name' of generated identity, or explict path to generated private key file."
+            help="'name' of generated identity, or explict path to generated certificate file."
         ),
     ],
     csr_path: Annotated[
         Optional[Path],
         typer.Option(
             help=(
-                "Optional explicit path to Certificate Signing Request. If absent, CSR path is derived from the"
+                "Optional explicit path to Certificate Signing Request. If absent, CSR path is derived from the "
                 "private key output path."
             )
         ),
     ] = None,
-    certificate_path: Annotated[
+    private_key_path: Annotated[
         Optional[Path],
         typer.Option(
             help=(
-                "Optional explicit path to Certificate Signing Request. If absent, CSR path is derived from the"
-                "private key output path."
+                "Optional explicit path to private key. If absent, private key path is derived from the "
+                "certificate output path."
             )
         ),
     ] = None,
     certs_dir: Annotated[
         Path, typer.Option(help="Base storage directory for named certs")
     ] = DEFAULT_CERTS_DIR,
     public_exponent: Annotated[
@@ -563,30 +576,30 @@
     ] = 825,
 ) -> None:
     """Generate public/private RSA key pair, CSR and certificate for a named identity.
 
     Writes public/private key, CSR and certificate files, by default named:
 
         $HOME/.local/share/gridworks/ca/certs/name/name.pub
-        $HOME/.local/share/gridworks/ca/certs/name/name.pem
+        $HOME/.local/share/gridworks/ca/certs/name/private/name.pem
         $HOME/.local/share/gridworks/ca/certs/name/name.csr
         $HOME/.local/share/gridworks/ca/certs/name/name.crt
 
     Input file can be explicitly named with the --ca-certificate-path and --ca-private-key-path parameters.
     Output file can be explicitly named by passing a path-like string for a ".pem" file to the name parameter and/or
     with --csr-path and --certificate-path parameters.
     """
-    private_key_path = get_output_path(
-        name_or_output_path=name, output_suffix=".pem", certs_dir=certs_dir
+    certificate_path = get_output_path(
+        name_or_output_path=name, output_suffix=".crt", certs_dir=certs_dir
     )
-    public_key_path = private_key_path.with_suffix(".pub")
+    public_key_path = certificate_path.with_suffix(".pub")
+    if private_key_path is None:
+        private_key_path = _private_from_public_path(certificate_path)
     if csr_path is None:
-        csr_path = private_key_path.with_suffix(".csr")
-    if certificate_path is None:
-        certificate_path = private_key_path.with_suffix(".crt")
+        csr_path = certificate_path.with_suffix(".csr")
     if not force and (
         private_key_path.exists()
         or public_key_path.exists()
         or csr_path.exists()
         or certificate_path.exists()
     ):
         rich.print(
@@ -604,15 +617,15 @@
         rich.print(
             f"  Certificate file  exists:{str(certificate_path.exists()):5s}  {private_key_path}"
         )
         rich.print("\nUse --force to overwrite keys")
         return
     ctx.invoke(
         rsa,
-        name=name,
+        name=public_key_path,
         certs_dir=certs_dir,
         public_exponent=public_exponent,
         key_size=key_size,
         force=force,
     )
     ctx.invoke(
         csr,
```

### Comparing `gridworks_cert-0.3.2/PKG-INFO` & `gridworks_cert-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gridworks-cert
-Version: 0.3.2
+Version: 0.4.0
 Summary: TLS certificate management tools for GridWorks
 Home-page: https://github.com/thegridelectric/gridworks-cert
 License: MIT
 Author: Andrew Schweitzer
 Author-email: schweitz72@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ownca (>=0.4.0)
 Requires-Dist: rich (>=12.0.0)
-Requires-Dist: trogon (>=0.5.0,<0.6.0)
+Requires-Dist: trogon (>=0.5.0)
 Requires-Dist: typer (>=0.9.0)
 Requires-Dist: xdg (>=6.0.0)
 Project-URL: Changelog, https://github.com/thegridelectric/gridworks-cert/releases
 Project-URL: Documentation, https://gridworks-cert.readthedocs.io
 Project-URL: Repository, https://github.com/thegridelectric/gridworks-cert
 Description-Content-Type: text/markdown
```

