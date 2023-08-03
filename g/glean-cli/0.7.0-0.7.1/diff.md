# Comparing `tmp/glean-cli-0.7.0.tar.gz` & `tmp/glean-cli-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glean-cli-0.7.0.tar", last modified: Wed Jul 26 17:57:21 2023, max compression
+gzip compressed data, was "glean-cli-0.7.1.tar", last modified: Thu Aug  3 20:24:22 2023, max compression
```

## Comparing `glean-cli-0.7.0.tar` & `glean-cli-0.7.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.259591 glean-cli-0.7.0/
--rw-r--r--   0 calderhoover   (501) staff       (20)    11357 2023-03-17 14:57:47.000000 glean-cli-0.7.0/LICENSE
--rw-r--r--   0 calderhoover   (501) staff       (20)     1209 2023-07-26 17:57:21.259642 glean-cli-0.7.0/PKG-INFO
--rw-r--r--   0 calderhoover   (501) staff       (20)      758 2023-07-26 17:48:44.000000 glean-cli-0.7.0/README.md
--rw-r--r--   0 calderhoover   (501) staff       (20)      103 2023-03-17 14:57:47.000000 glean-cli-0.7.0/pyproject.toml
--rw-r--r--   0 calderhoover   (501) staff       (20)      831 2023-07-26 17:57:21.259904 glean-cli-0.7.0/setup.cfg
--rw-r--r--   0 calderhoover   (501) staff       (20)       38 2023-03-17 14:57:47.000000 glean-cli-0.7.0/setup.py
-drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.254325 glean-cli-0.7.0/src/
-drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.256541 glean-cli-0.7.0/src/glean/
--rw-r--r--   0 calderhoover   (501) staff       (20)       18 2023-07-26 17:48:47.000000 glean-cli-0.7.0/src/glean/__init__.py
--rw-r--r--   0 calderhoover   (501) staff       (20)    31225 2023-07-26 17:48:44.000000 glean-cli-0.7.0/src/glean/cli.py
--rw-r--r--   0 calderhoover   (501) staff       (20)      146 2023-07-26 17:48:44.000000 glean-cli-0.7.0/src/glean/constants.py
--rw-r--r--   0 calderhoover   (501) staff       (20)     1598 2023-03-17 14:57:47.000000 glean-cli-0.7.0/src/glean/credentials.py
--rw-r--r--   0 calderhoover   (501) staff       (20)     3904 2023-07-11 21:20:42.000000 glean-cli-0.7.0/src/glean/filesystem.py
--rw-r--r--   0 calderhoover   (501) staff       (20)    17269 2023-07-26 17:48:44.000000 glean-cli-0.7.0/src/glean/glean_api.py
-drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.257542 glean-cli-0.7.0/src/glean/utils/
--rw-r--r--   0 calderhoover   (501) staff       (20)        0 2023-03-17 14:57:47.000000 glean-cli-0.7.0/src/glean/utils/__init__.py
--rw-r--r--   0 calderhoover   (501) staff       (20)      509 2023-03-17 14:57:47.000000 glean-cli-0.7.0/src/glean/utils/cli.py
--rw-r--r--   0 calderhoover   (501) staff       (20)     2622 2023-07-11 21:20:42.000000 glean-cli-0.7.0/src/glean/utils/grn.py
--rw-r--r--   0 calderhoover   (501) staff       (20)     1356 2023-07-11 21:20:42.000000 glean-cli-0.7.0/src/glean/utils/resource.py
--rw-r--r--   0 calderhoover   (501) staff       (20)     1089 2023-07-11 21:20:42.000000 glean-cli-0.7.0/src/glean/utils/validate_config.py
-drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.258437 glean-cli-0.7.0/src/glean_cli.egg-info/
--rw-r--r--   0 calderhoover   (501) staff       (20)     1209 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/PKG-INFO
--rw-r--r--   0 calderhoover   (501) staff       (20)      639 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/SOURCES.txt
--rw-r--r--   0 calderhoover   (501) staff       (20)        1 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/dependency_links.txt
--rw-r--r--   0 calderhoover   (501) staff       (20)       41 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/entry_points.txt
--rw-r--r--   0 calderhoover   (501) staff       (20)      116 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/requires.txt
--rw-r--r--   0 calderhoover   (501) staff       (20)        6 2023-07-26 17:57:21.000000 glean-cli-0.7.0/src/glean_cli.egg-info/top_level.txt
-drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-07-26 17:57:21.259433 glean-cli-0.7.0/tests/
--rw-r--r--   0 calderhoover   (501) staff       (20)      309 2023-03-17 14:57:47.000000 glean-cli-0.7.0/tests/test_cli.py
--rw-r--r--   0 calderhoover   (501) staff       (20)     1652 2023-03-17 14:57:47.000000 glean-cli-0.7.0/tests/test_credentials.py
--rw-r--r--   0 calderhoover   (501) staff       (20)     4632 2023-07-11 21:20:42.000000 glean-cli-0.7.0/tests/test_filesystem.py
--rw-r--r--   0 calderhoover   (501) staff       (20)      666 2023-03-17 14:57:47.000000 glean-cli-0.7.0/tests/test_glean_api.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 20:24:22.587281 glean-cli-0.7.1/
+-rw-r--r--   0 dse        (501) staff       (20)    11357 2021-08-09 13:38:38.000000 glean-cli-0.7.1/LICENSE
+-rw-r--r--   0 dse        (501) staff       (20)     1209 2023-08-03 20:24:22.587358 glean-cli-0.7.1/PKG-INFO
+-rw-r--r--   0 dse        (501) staff       (20)      758 2023-08-01 21:35:43.000000 glean-cli-0.7.1/README.md
+-rw-r--r--   0 dse        (501) staff       (20)      103 2021-08-09 13:48:34.000000 glean-cli-0.7.1/pyproject.toml
+-rw-r--r--   0 dse        (501) staff       (20)      835 2023-08-03 20:24:22.587756 glean-cli-0.7.1/setup.cfg
+-rw-r--r--   0 dse        (501) staff       (20)       38 2021-09-03 21:01:45.000000 glean-cli-0.7.1/setup.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 20:24:22.581622 glean-cli-0.7.1/src/
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 20:24:22.583972 glean-cli-0.7.1/src/glean/
+-rw-r--r--   0 dse        (501) staff       (20)       18 2023-08-03 20:24:01.000000 glean-cli-0.7.1/src/glean/__init__.py
+-rw-r--r--   0 dse        (501) staff       (20)    31701 2023-08-01 21:35:43.000000 glean-cli-0.7.1/src/glean/cli.py
+-rw-r--r--   0 dse        (501) staff       (20)      146 2023-08-01 21:35:43.000000 glean-cli-0.7.1/src/glean/constants.py
+-rw-r--r--   0 dse        (501) staff       (20)     1598 2022-10-27 21:08:22.000000 glean-cli-0.7.1/src/glean/credentials.py
+-rw-r--r--   0 dse        (501) staff       (20)     3904 2023-06-16 13:01:39.000000 glean-cli-0.7.1/src/glean/filesystem.py
+-rw-r--r--   0 dse        (501) staff       (20)    17544 2023-08-01 21:35:43.000000 glean-cli-0.7.1/src/glean/glean_api.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 20:24:22.585257 glean-cli-0.7.1/src/glean/utils/
+-rw-r--r--   0 dse        (501) staff       (20)        0 2022-10-27 21:08:22.000000 glean-cli-0.7.1/src/glean/utils/__init__.py
+-rw-r--r--   0 dse        (501) staff       (20)      509 2022-10-27 21:08:22.000000 glean-cli-0.7.1/src/glean/utils/cli.py
+-rw-r--r--   0 dse        (501) staff       (20)     2622 2023-06-15 15:12:56.000000 glean-cli-0.7.1/src/glean/utils/grn.py
+-rw-r--r--   0 dse        (501) staff       (20)     1356 2023-06-20 18:52:16.000000 glean-cli-0.7.1/src/glean/utils/resource.py
+-rw-r--r--   0 dse        (501) staff       (20)     1089 2023-06-15 15:12:56.000000 glean-cli-0.7.1/src/glean/utils/validate_config.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 20:24:22.586152 glean-cli-0.7.1/src/glean_cli.egg-info/
+-rw-r--r--   0 dse        (501) staff       (20)     1209 2023-08-03 20:24:22.000000 glean-cli-0.7.1/src/glean_cli.egg-info/PKG-INFO
+-rw-r--r--   0 dse        (501) staff       (20)      639 2023-08-03 20:24:22.000000 glean-cli-0.7.1/src/glean_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 dse        (501) staff       (20)        1 2023-08-03 20:24:22.000000 glean-cli-0.7.1/src/glean_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 dse        (501) staff       (20)       41 2023-08-03 20:24:22.000000 glean-cli-0.7.1/src/glean_cli.egg-info/entry_points.txt
+-rw-r--r--   0 dse        (501) staff       (20)      121 2023-08-03 20:24:22.000000 glean-cli-0.7.1/src/glean_cli.egg-info/requires.txt
+-rw-r--r--   0 dse        (501) staff       (20)        6 2023-08-03 20:24:22.000000 glean-cli-0.7.1/src/glean_cli.egg-info/top_level.txt
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 20:24:22.587142 glean-cli-0.7.1/tests/
+-rw-r--r--   0 dse        (501) staff       (20)      309 2022-10-27 21:08:22.000000 glean-cli-0.7.1/tests/test_cli.py
+-rw-r--r--   0 dse        (501) staff       (20)     1652 2022-10-27 21:08:22.000000 glean-cli-0.7.1/tests/test_credentials.py
+-rw-r--r--   0 dse        (501) staff       (20)     4632 2023-06-20 18:52:16.000000 glean-cli-0.7.1/tests/test_filesystem.py
+-rw-r--r--   0 dse        (501) staff       (20)      666 2022-10-27 21:08:22.000000 glean-cli-0.7.1/tests/test_glean_api.py
```

### Comparing `glean-cli-0.7.0/LICENSE` & `glean-cli-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.0/PKG-INFO` & `glean-cli-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.7.0
+Version: 0.7.1
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.7.0/README.md` & `glean-cli-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.0/setup.cfg` & `glean-cli-0.7.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,13 @@
 where = src
 
 [options.entry_points]
 console_scripts = 
 	glean = glean.cli:main
 
 [options.extras_require]
-test = 
-	pytest
+test = pytest; cram
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `glean-cli-0.7.0/src/glean/cli.py` & `glean-cli-0.7.1/src/glean/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,31 +127,33 @@
 @click.option(
     "--project-id",
     type=str,
     required=False,
     help="If specified, creates an access key for this project ID. Required if your Glean user is a member of multiple projects.",
 )
 @click.pass_context
-def start(
-    ctx: click.Context, project_id: Optional[str]
-):
+def start(ctx: click.Context, project_id: Optional[str]):
     """Log into or sign up for a Glean account and create an access key to get started.
 
     If `--credentials-filepath` is passed, will save the access key in that location.
 
     If an access key already exists for your project, you'll need to delete it first before
     this command can generate a new one for you.
     """
     credentials_filepath = ctx.obj["credentials_filepath"]
     if os.path.exists(credentials_filepath):
-        click.echo("If you continue, the file at the following location will be overwritten with your new access key:")
+        click.echo(
+            "If you continue, the file at the following location will be overwritten with your new access key:"
+        )
         click.echo()
         click.echo(credentials_filepath)
         click.echo()
-        click.echo("💡 To save your new access key to a different file path, re-run this command with that path passed via the `--credentials-filepath` option.")
+        click.echo(
+            "💡 To save your new access key to a different file path, re-run this command with that path passed via the `--credentials-filepath` option."
+        )
         click.echo()
         if not click.confirm("Continue and overwrite existing file?"):
             raise click.Abort()
         click.echo()
 
     create_access_key(ctx.obj["credentials_filepath"], project_id)
 
@@ -165,14 +167,15 @@
     "filepath", type=click.Path(exists=True, dir_okay=False, allow_dash=True)
 )
 @click.pass_context
 def upload(ctx, database, filepath):
     """Pushes a file to a Glean duckdb database connection that can be queried using duckdb or used as the basis for a data model."""
 
     s = Session()
+    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
     project_id = login(s, ctx.obj["credentials"])
     fp = os.path.expanduser(filepath)
 
     click.echo("📄 Uploading file to Glean...")
     filename = upload_files_to_glean(s, project_id, database, fp)
     click.echo(f'✅ successfully uploaded "{filename}"')
 
@@ -404,14 +407,15 @@
             )
         resource_id = grn_components.gluid
 
     SUPPORTED_TYPES = ["dashboard", "saved_view", "model", "color_palette"]
     local_by_path = {
         k: v for k, v in local_resources(Path(".")).items() if v.type in SUPPORTED_TYPES
     }
+    click.echo(f"🔎 Found {len(local_by_path)} Glean resources in working directory.")
 
     def get_grn(path: PurePosixPath, resource: Resource) -> GRNComponents:
         RESOURCE_TYPE_TO_ABBREV = {
             "model": "m",
             "saved_view": "sv",
             "dashboard": "dsb",
             "color_palette": "palette",
@@ -471,26 +475,27 @@
     result = pull_resource(s, project_id, resource_type, resource_id)
     if result.get("errors"):
         _echo_pull_errors_and_exit(result["errors"])
         return
 
     remote: list[Resource] = result["configs"]
 
-    updated_files = []
+    touched_files = [] # either created or modified
+    num_updated = 0
     for resource in remote:
         assert resource.grn is not None
         with suppress(ValueError):
             index = local_grns.index(resource.grn)
             # we've matched the resource to a local file
             (_, path, local_resource) = local_by_grn[index]
             if local_resource.raw == resource.raw:
                 continue
-
-            updated_files.append(Path(path))
             # the resource has changed!
+            num_updated += 1
+            touched_files.append(Path(path))
             with open(Path(path), "w") as f:
                 yaml.dump(resource.raw, f, Dumper=yaml.RoundTripDumper)
 
             continue
 
         # not present locally, so we need to make a new file
         name = "".join(
@@ -504,24 +509,27 @@
             if i > 0:
                 path = Path(f"{name}_{i}.yml")
             else:
                 path = Path(f"{name}.yml")
             if path.exists():
                 continue
 
-            updated_files.append(path)
+            touched_files.append(path)
             with open(path, "w") as f:
                 yaml.dump(resource.raw, f, Dumper=yaml.RoundTripDumper)
 
             break
 
     click.echo()
-    if updated_files:
-        click.echo("✅ Done. Files created or modified:")
-        _echo_list([str(p) for p in updated_files])
+    if touched_files:
+        click.echo(f"✅ Done. {len(touched_files)} files were created or modified:")
+        _echo_list(list(sorted([str(p) for p in touched_files])))
+        click.echo()
+        if num_updated < len(local_by_path):
+            click.echo(f"{len(local_by_path) - num_updated} files were not modified.")
     else:
         click.echo("✅ Done. No files were updated.")
 
 
 def _handle_dbt_args(dbt_manifest_path, run_dbt_parse, dbt_flags):
     """Convenience wrapper for running `dbt parse` before `glean preview` or `glean deploy`.
     Must be run from your Glean project directory.
```

### Comparing `glean-cli-0.7.0/src/glean/credentials.py` & `glean-cli-0.7.1/src/glean/credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.0/src/glean/filesystem.py` & `glean-cli-0.7.1/src/glean/filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.0/src/glean/glean_api.py` & `glean-cli-0.7.1/src/glean/glean_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,33 +30,36 @@
     invalid_project_id = None
 
     # Populated if access key was successfully created.
     project_name = None
     access_key_id = None
     access_key_token = None
     project_id = None
+    user_email = None
+    user_full_name = None
 
     # Populated if this is a new user.
-    new_user_name = None
+    is_new_user = None
 
     # Populated if we encountered a request error while finishing authentication.
     request_error = False
 
     class CallbackHandler(BaseHTTPRequestHandler):
         def do_GET(self):
             nonlocal has_multiple_projects
             
             nonlocal invalid_project_id
 
             nonlocal project_name
             nonlocal access_key_id
             nonlocal access_key_token
             nonlocal project_id
-
-            nonlocal new_user_name
+            nonlocal user_email
+            nonlocal user_full_name
+            nonlocal is_new_user
 
             nonlocal request_error
 
             query = urlparse(self.path).query
             parsed_query = parse_qs(query)
 
             # Utility for grabbing a query param from parsed_query.
@@ -67,33 +70,38 @@
 
             invalid_project_id = get_query_param("invalid_project_id")
 
             project_name = get_query_param("project_name")
             access_key_id = get_query_param("access_key_id")
             access_key_token = get_query_param("access_key_token")
             project_id = get_query_param("project_id")
+            user_email = get_query_param("user_email")
+            user_full_name = get_query_param("user_full_name")
 
-            new_user_name = get_query_param("new_user_name")
+            is_new_user = get_query_param("is_new_user")
 
             # We expect either all newly created access key info or the project name
             # of the existing access key to be passed. If neither is true, indicate
             # a bad request.
             if not (
                 has_multiple_projects or
                 invalid_project_id or
-                (project_name and access_key_id and access_key_token and project_id)
+                (project_name and access_key_id and access_key_token and project_id and user_email and user_full_name)
             ):
                 request_error = True
                 self.send_response(302)
                 self.send_header('Location', f"{GLEAN_BASE_URI}/cliAuthConfirmation/error")
                 self.end_headers()
                 return
 
             self.send_response(302)
-            self.send_header('Location', f"{GLEAN_BASE_URI}/cliAuthConfirmation/success")
+            if is_new_user:
+                self.send_header('Location', f"{GLEAN_BASE_URI}/cliAuthConfirmation/success/newUser?userFullName={user_full_name}")
+            else:
+                self.send_header('Location', f"{GLEAN_BASE_URI}/cliAuthConfirmation/success/existingUser?userEmail={user_email}")
             self.end_headers()
             return
         
         # Disables logging in the CLI, which we don't want to expose to the user
         # unless in debug mode.
         def log_message(self, *args):
             if GLEAN_DEBUG:
@@ -147,22 +155,21 @@
         "access_key_id": access_key_id,
         "access_key_token": access_key_token,
         "project_id": project_id
     }))
     click.echo(f"✅ Saved new access key for {click.style(project_name, bold=True)} to {credentials_filepath}")
     click.echo()
 
-    if new_user_name:
-        click.echo(f"Welcome {new_user_name}! We created a new Glean project for you.")
-        click.echo("Go to the following link to set up a database connection:")
-        click.echo(f"{GLEAN_BASE_URI}/app/mb")
+    if is_new_user:
+        terminal_size = os.get_terminal_size()
+        click.echo("─" * terminal_size.columns)
+        click.echo()
+        click.echo(f"👋 Welcome {user_full_name}! We created a new Glean project for you.")
         click.echo()
-        click.echo("Once you're done, build your first data model by following one of these guides:")
-        click.echo("1. Build with Glean's website: https://docs.glean.io/docs/data-modeling/add-data-model")
-        click.echo("2. Push your dbt models directly into Glean: https://docs.glean.io/docs/data-ops/dbt-integration")
+        click.echo(f"{click.style('Go to the following link to set up a database connection:', bold=True)} {GLEAN_BASE_URI}/app/mb")
         click.echo()
 
 
 def login(session: Session, credentials: CliCredentials):
     """Authenticates the session with the provided credentials.
 
     :return The user's project ID, if successfully logged in.
```

### Comparing `glean-cli-0.7.0/src/glean/utils/grn.py` & `glean-cli-0.7.1/src/glean/utils/grn.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.0/src/glean/utils/resource.py` & `glean-cli-0.7.1/src/glean/utils/resource.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.0/src/glean/utils/validate_config.py` & `glean-cli-0.7.1/src/glean/utils/validate_config.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.0/src/glean_cli.egg-info/PKG-INFO` & `glean-cli-0.7.1/src/glean_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.7.0
+Version: 0.7.1
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.7.0/src/glean_cli.egg-info/SOURCES.txt` & `glean-cli-0.7.1/src/glean_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.0/tests/test_credentials.py` & `glean-cli-0.7.1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.0/tests/test_filesystem.py` & `glean-cli-0.7.1/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.0/tests/test_glean_api.py` & `glean-cli-0.7.1/tests/test_glean_api.py`

 * *Files identical despite different names*

