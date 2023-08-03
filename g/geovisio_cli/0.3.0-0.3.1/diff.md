# Comparing `tmp/geovisio_cli-0.3.0.tar.gz` & `tmp/geovisio_cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovisio_cli-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geovisio_cli-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geovisio_cli-0.3.0.tar` & `geovisio_cli-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,42 @@
--rw-r--r--   0        0        0       56 2023-07-18 08:40:07.314737 geovisio_cli-0.3.0/.gitignore
--rw-r--r--   0        0        0     1413 2023-06-22 09:18:10.500879 geovisio_cli-0.3.0/.gitlab-ci.yml
--rw-r--r--   0        0        0       91 2023-07-17 08:45:58.280836 geovisio_cli-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4277 2023-07-20 07:08:49.784332 geovisio_cli-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.3.0/LICENSE
--rw-r--r--   0        0        0      590 2023-05-24 13:17:27.558420 geovisio_cli-0.3.0/Makefile
--rw-r--r--   0        0        0     7732 2023-07-17 08:45:58.280836 geovisio_cli-0.3.0/README.md
--rw-r--r--   0        0        0     3801 2023-07-20 07:08:49.784332 geovisio_cli-0.3.0/USAGE.md
--rw-r--r--   0        0        0       53 2023-07-20 07:08:49.784332 geovisio_cli-0.3.0/geovisio_cli/__init__.py
--rw-r--r--   0        0        0     6173 2023-05-24 13:17:27.558420 geovisio_cli-0.3.0/geovisio_cli/auth.py
--rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.3.0/geovisio_cli/exception.py
--rw-r--r--   0        0        0     7245 2023-07-18 13:06:30.484101 geovisio_cli-0.3.0/geovisio_cli/main.py
--rw-r--r--   0        0        0      136 2023-05-24 13:17:27.558420 geovisio_cli-0.3.0/geovisio_cli/model.py
--rw-r--r--   0        0        0    28868 2023-07-20 07:02:18.052530 geovisio_cli-0.3.0/geovisio_cli/sequence.py
--rw-r--r--   0        0        0     2107 2023-06-22 09:18:10.500879 geovisio_cli-0.3.0/geovisio_cli/utils.py
--rw-r--r--   0        0        0     1314 2023-07-18 10:05:38.231634 geovisio_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      234 2023-06-19 17:19:08.702865 geovisio_cli-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.3.0/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.3.0/tests/fixtures/e2.jpg
--rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.3.0/tests/fixtures/e3.jpg
--rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.3.0/tests/fixtures/invalid_pic.jpg
--rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.3.0/tests/fixtures/not_a_pic.md
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.3.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     3327 2023-05-24 13:17:27.558420 geovisio_cli-0.3.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     2189 2023-05-22 08:59:23.607560 geovisio_cli-0.3.0/tests/integration/docker-compose-geovisio.yml
--rw-r--r--   0        0        0      584 2023-05-22 08:59:23.607560 geovisio_cli-0.3.0/tests/integration/docker-compose-gitlab-override.yml
--rw-r--r--   0        0        0    76457 2023-05-22 08:59:23.611560 geovisio_cli-0.3.0/tests/integration/keycloak-realm.json
--rw-r--r--   0        0        0     3280 2023-07-18 08:40:07.314737 geovisio_cli-0.3.0/tests/integration/test_auth.py
--rw-r--r--   0        0        0      369 2023-05-24 13:17:27.558420 geovisio_cli-0.3.0/tests/integration/test_status.py
--rw-r--r--   0        0        0     7391 2023-07-18 08:40:07.314737 geovisio_cli-0.3.0/tests/integration/test_upload.py
--rw-r--r--   0        0        0      642 2023-07-17 15:59:13.279607 geovisio_cli-0.3.0/tests/test_process.py
--rw-r--r--   0        0        0    21252 2023-07-18 13:06:30.484101 geovisio_cli-0.3.0/tests/test_sequence.py
--rw-r--r--   0        0        0      682 2023-06-22 09:18:10.500879 geovisio_cli-0.3.0/tests/test_utils.py
--rw-r--r--   0        0        0     9053 1970-01-01 00:00:00.000000 geovisio_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       56 2023-07-18 08:40:07.314737 geovisio_cli-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1413 2023-06-22 09:18:10.500879 geovisio_cli-0.3.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0       91 2023-07-17 08:45:58.280836 geovisio_cli-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4616 2023-08-03 12:40:17.267072 geovisio_cli-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.3.1/LICENSE
+-rw-r--r--   0        0        0      590 2023-05-24 13:17:27.558420 geovisio_cli-0.3.1/Makefile
+-rw-r--r--   0        0        0     8030 2023-08-03 11:31:18.004507 geovisio_cli-0.3.1/README.md
+-rw-r--r--   0        0        0     4546 2023-08-03 11:31:18.008508 geovisio_cli-0.3.1/USAGE.md
+-rw-r--r--   0        0        0       53 2023-08-03 12:40:17.267072 geovisio_cli-0.3.1/geovisio_cli/__init__.py
+-rw-r--r--   0        0        0     6480 2023-08-03 11:31:18.008508 geovisio_cli-0.3.1/geovisio_cli/auth.py
+-rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.3.1/geovisio_cli/exception.py
+-rw-r--r--   0        0        0     8861 2023-08-03 11:31:18.008508 geovisio_cli-0.3.1/geovisio_cli/main.py
+-rw-r--r--   0        0        0     5978 2023-07-20 14:40:02.264538 geovisio_cli-0.3.1/geovisio_cli/model.py
+-rw-r--r--   0        0        0        0 2023-07-20 14:40:02.264538 geovisio_cli-0.3.1/geovisio_cli/sequences/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 14:40:02.264538 geovisio_cli-0.3.1/geovisio_cli/sequences/process/__init__.py
+-rw-r--r--   0        0        0     9399 2023-07-20 14:40:02.264538 geovisio_cli-0.3.1/geovisio_cli/sequences/process/standard.py
+-rw-r--r--   0        0        0     5369 2023-08-03 11:31:18.008508 geovisio_cli-0.3.1/geovisio_cli/sequences/status.py
+-rw-r--r--   0        0        0     9837 2023-08-03 11:31:18.008508 geovisio_cli-0.3.1/geovisio_cli/sequences/upload.py
+-rw-r--r--   0        0        0     2319 2023-08-03 11:31:18.008508 geovisio_cli-0.3.1/geovisio_cli/utils.py
+-rw-r--r--   0        0        0     1314 2023-07-18 10:05:38.231634 geovisio_cli-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-19 17:19:08.702865 geovisio_cli-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.3.1/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.3.1/tests/fixtures/e2.jpg
+-rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.3.1/tests/fixtures/e3.jpg
+-rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.3.1/tests/fixtures/invalid_pic.jpg
+-rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.3.1/tests/fixtures/not_a_pic.md
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.3.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3327 2023-05-24 13:17:27.558420 geovisio_cli-0.3.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2189 2023-08-03 11:31:18.008508 geovisio_cli-0.3.1/tests/integration/docker-compose-geovisio.yml
+-rw-r--r--   0        0        0      584 2023-05-22 08:59:23.607560 geovisio_cli-0.3.1/tests/integration/docker-compose-gitlab-override.yml
+-rw-r--r--   0        0        0    76457 2023-05-22 08:59:23.611560 geovisio_cli-0.3.1/tests/integration/keycloak-realm.json
+-rw-r--r--   0        0        0     3490 2023-08-03 11:31:18.008508 geovisio_cli-0.3.1/tests/integration/test_auth.py
+-rw-r--r--   0        0        0      563 2023-08-03 11:31:18.008508 geovisio_cli-0.3.1/tests/integration/test_status.py
+-rw-r--r--   0        0        0     8055 2023-08-03 11:31:18.008508 geovisio_cli-0.3.1/tests/integration/test_upload.py
+-rw-r--r--   0        0        0     4992 2023-07-20 14:40:02.268538 geovisio_cli-0.3.1/tests/test_model.py
+-rw-r--r--   0        0        0      660 2023-07-20 14:40:02.268538 geovisio_cli-0.3.1/tests/test_process.py
+-rw-r--r--   0        0        0    12923 2023-07-20 14:40:02.268538 geovisio_cli-0.3.1/tests/test_sequence_standard.py
+-rw-r--r--   0        0        0     4285 2023-08-03 11:31:18.008508 geovisio_cli-0.3.1/tests/test_sequence_upload.py
+-rw-r--r--   0        0        0      682 2023-06-22 09:18:10.500879 geovisio_cli-0.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0     9351 1970-01-01 00:00:00.000000 geovisio_cli-0.3.1/PKG-INFO
```

### Comparing `geovisio_cli-0.3.0/.gitlab-ci.yml` & `geovisio_cli-0.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/CHANGELOG.md` & `geovisio_cli-0.3.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.3.1] - 2023-08-03
+
+### Added
+- Add `--picture-upload-timeout` to upload, to change the timeout of a picture upload
+- Add `--disable-cert-check` to all commands, to disable ssl certificate check. This should not be used, unless if you -really- know what you are doing.
 
 ## [0.3.0] - 2023-07-20
 
 ### Added
 - CLI now supports splitting a sequence into multiple sequences when distance or time exceeds a given delta. These can be set on upload with `--split-time` or `--split-distance` parameters.
 
 
@@ -86,15 +91,16 @@
 
 ## [0.0.1] - 2023-03-14
 
 ### Added
 - Basic scripts for uploading pictures to a GeoVisio API
 
 
-[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.3.0...main
+[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.3.1...main
+[0.3.0]: https://gitlab.com/geovisio/cli/-/compare/0.3.0...0.3.1
 [0.3.0]: https://gitlab.com/geovisio/cli/-/compare/0.2.3...0.3.0
 [0.2.3]: https://gitlab.com/geovisio/cli/-/compare/0.2.2...0.2.3
 [0.2.2]: https://gitlab.com/geovisio/cli/-/compare/0.2.1...0.2.2
 [0.2.1]: https://gitlab.com/geovisio/cli/-/compare/0.2.0...0.2.1
 [0.2.0]: https://gitlab.com/geovisio/cli/-/compare/0.1.0...0.2.0
 [0.1.0]: https://gitlab.com/geovisio/cli/-/compare/0.0.5...0.1.0
 [0.0.5]: https://gitlab.com/geovisio/cli/-/compare/0.0.4...0.0.5
```

### Comparing `geovisio_cli-0.3.0/CODE_OF_CONDUCT.md` & `geovisio_cli-0.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/LICENSE` & `geovisio_cli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/Makefile` & `geovisio_cli-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/README.md` & `geovisio_cli-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -164,14 +164,20 @@
 
 If you don't have Docker Compose, or want to use an existing GeoVisio test instance (to speed up tests), you can pass the `--external-geovisio-url` option to pytest:
 
 ```bash
 pytest --external-geovisio-url=http://localhost:5000
 ```
 
+#### Using with an unsecure geovisio API
+
+The CLI parameter `--disable-cert-check` is available to use with an unsecure geovisio API (or when behind proxies messing with ssl). 
+
+There are no automated test for this, but you can run a geovisio with `flask run --cert=adhoc` to manually test this. 
+
 ### Documentation
 
 High-level documentation is handled by [Typer](https://typer.tiangolo.com/). You can update the generated `USAGE.md` file using this command:
 
 ```bash
 make docs
 ```
```

### Comparing `geovisio_cli-0.3.0/USAGE.md` & `geovisio_cli-0.3.1/USAGE.md`

 * *Files 23% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 **Options**:
 
 * `--id TEXT`: Id of the collection
 * `--api-url TEXT`: GeoVisio endpoint URL
 * `--location TEXT`: Full url of the collection
 * `--wait / --no-wait`: wait for all pictures to be ready  [default: no-wait]
+* `--disable-cert-check / --enable-cert-check`: Disable SSL certificates checks while uploading. This should not be used, unless if you -really- know what you are doing.  [default: enable-cert-check]
 * `--help`: Show this message and exit.
 
 ## `geovisio login`
 
 Authenticate into the given instance, and save credentials in a configuration file.
 
 This will generate credentials, and ask the user to visit a page to associate those credentials to the user's account.
@@ -56,14 +57,15 @@
 ```console
 $ geovisio login [OPTIONS]
 ```
 
 **Options**:
 
 * `--api-url TEXT`: GeoVisio endpoint URL  [required]
+* `--disable-cert-check / --enable-cert-check`: Disable SSL certificates checks while uploading. This should not be used, unless if you -really- know what you are doing.  [default: enable-cert-check]
 * `--help`: Show this message and exit.
 
 ## `geovisio test-process`
 
 (For testing) Generates a TOML file with metadata used for upload
 
 **Usage**:
@@ -107,8 +109,10 @@
 * `--token TEXT`: GeoVisio token if the geovisio instance needs it.
 
 If none is provided and the geovisio instance requires it, the token will be asked during run.
 Note: is is advised to wait for prompt without using this variable.
 * `--sort-method [filename-asc|filename-desc|time-asc|time-desc]`: Strategy used for sorting your pictures. Either by filename or EXIF time, in ascending or descending order.  [default: time-asc]
 * `--split-distance INTEGER`: Maximum distance between two pictures to be considered in the same sequence (in meters).  [default: 100]
 * `--split-time INTEGER`: Maximum time interval between two pictures to be considered in the same sequence (in seconds).  [default: 60]
+* `--picture-upload-timeout FLOAT`: Timeout time to receive the first byte of the response for each picture upload (in seconds)  [default: 60.0]
+* `--disable-cert-check / --enable-cert-check`: Disable SSL certificates checks while uploading. This should not be used, unless if you -really- know what you are doing.  [default: enable-cert-check]
 * `--help`: Show this message and exit.
```

### Comparing `geovisio_cli-0.3.0/geovisio_cli/auth.py` & `geovisio_cli-0.3.1/geovisio_cli/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 
 
 def _login_with_stored_credentials(s: Session, geovisio: Geovisio):
     creds = _read_existing_credentials(geovisio)
 
     instance_cred = creds.get_instance_credentials(geovisio.url)
     if not instance_cred:
-        _generate_and_update_credentials(creds, geovisio)
+        _generate_and_update_credentials(s, creds, geovisio)
         return False
 
-    account_name = _check_if_associated(geovisio, instance_cred)
+    account_name = _check_if_associated(s, geovisio, instance_cred)
     if not account_name:
         claim_url = f"{geovisio.url}/api/auth/tokens/{instance_cred.token_id}/claim"
         print(
             f"🔐 We're waiting for you to link your user account with generated API token. To finalize authentication, please either go to the URL below, or scan the QR code below."
         )
         print(f"[green]{claim_url}[/green]")
         _display_qr_code(claim_url)
@@ -78,42 +78,47 @@
             ]
         }
 
     def get_instance_credentials(self, instance_url: str):
         return next((c for c in self.instances if c.url == instance_url), None)
 
 
-def create_auth_credentials(geovisio: Geovisio) -> InstanceCredential:
+def create_auth_credentials(
+    geovisio: Geovisio, disable_cert_check: bool = False
+) -> InstanceCredential:
     """
     Login to geovisio and store auth cookie in session
     """
-    utils.test_geovisio_url(geovisio.url)
-    creds = _read_existing_credentials(geovisio)
-
-    instance_cred = creds.get_instance_credentials(geovisio.url)
-    if instance_cred:
-        account_name = _check_if_associated(geovisio, instance_cred)
-        if account_name:
-            print(f"👤 Already logged to instance as [green]{account_name}[/green]")
+    with requests.session() as s:
+        if disable_cert_check:
+            s.verify = False
+        utils.test_geovisio_url(s, geovisio.url)
+        creds = _read_existing_credentials(geovisio)
+
+        instance_cred = creds.get_instance_credentials(geovisio.url)
+        if instance_cred:
+            account_name = _check_if_associated(s, geovisio, instance_cred)
+            if account_name:
+                print(f"👤 Already logged to instance as [green]{account_name}[/green]")
+                return instance_cred
+            claim_url = instance_cred.get_claim_url()
+            print(
+                f"🔐 We're waiting for you to link your user account with generated API token. To finalize authentication, please either go to the URL below, or scan the QR code below."
+            )
+            print(f"[green]{claim_url}[/green]")
+            _display_qr_code(claim_url)
             return instance_cred
-        claim_url = instance_cred.get_claim_url()
-        print(
-            f"🔐 We're waiting for you to link your user account with generated API token. To finalize authentication, please either go to the URL below, or scan the QR code below."
-        )
-        print(f"[green]{claim_url}[/green]")
-        _display_qr_code(claim_url)
-        return instance_cred
 
-    return _generate_and_update_credentials(creds, geovisio)
+        return _generate_and_update_credentials(s, creds, geovisio)
 
 
 def _generate_and_update_credentials(
-    creds: Credentials, geovisio: Geovisio
+    session: requests.Session, creds: Credentials, geovisio: Geovisio
 ) -> InstanceCredential:
-    i = _generate_new_instance_credentials(geovisio)
+    i = _generate_new_instance_credentials(session, geovisio)
 
     creds.instances.append(i)
 
     _write_credentials(creds)
     return i
 
 
@@ -134,16 +139,18 @@
     with open(get_config_file_path(), "r") as f:
         tomlFileContent = f.read()
         creds.from_toml(toml.loads(tomlFileContent))
         f.close()
     return creds
 
 
-def _generate_new_instance_credentials(geovisio: Geovisio) -> InstanceCredential:
-    token_response = requests.post(f"{geovisio.url}/api/auth/tokens/generate")
+def _generate_new_instance_credentials(
+    session: requests.Session, geovisio: Geovisio
+) -> InstanceCredential:
+    token_response = session.post(f"{geovisio.url}/api/auth/tokens/generate")
     raise_for_status(token_response, "Impossible to generate a GeoVisio token")
 
     token = token_response.json()
     jwt_token = token["jwt_token"]
     id = token["id"]
 
     claim_url = next(l["href"] for l in token["links"] if l["rel"] == "claim")
@@ -160,17 +167,17 @@
     os.makedirs(os.path.dirname(config_file_path), exist_ok=True)
     with open(config_file_path, "w") as f:
         f.write(toml.dumps(creds.toml()))
         f.close()
 
 
 def _check_if_associated(
-    geovisio: Geovisio, creds: InstanceCredential
+    session: requests.Session, geovisio: Geovisio, creds: InstanceCredential
 ) -> Optional[str]:
-    token_response = requests.get(
+    token_response = session.get(
         f"{geovisio.url}/api/users/me",
         headers={"Authorization": f"Bearer {creds.jwt_token}"},
     )
     if token_response.status_code == 403 or token_response.status_code == 401:
         return None
     raise_for_status(token_response, "Impossible to get token status")
```

### Comparing `geovisio_cli-0.3.0/geovisio_cli/main.py` & `geovisio_cli-0.3.1/geovisio_cli/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import typer
 from typing_extensions import Annotated
 from pathlib import Path
-from geovisio_cli import sequence, exception, model, auth, utils, __version__
+from geovisio_cli import exception, model, auth, utils, __version__
 from rich import print
 from rich.panel import Panel
 from typing import Optional
 import os
+import geovisio_cli.sequences.process.standard
+import requests
+
+import geovisio_cli.sequences.status
+import geovisio_cli.sequences.upload
 
 
 app = typer.Typer()
 
 
 def version_callback(value: bool):
     if value:
@@ -68,59 +73,72 @@
         default=None,
         help="""GeoVisio token if the geovisio instance needs it.
 
 If none is provided and the geovisio instance requires it, the token will be asked during run.
 Note: is is advised to wait for prompt without using this variable.
 """,
     ),
-    sort_method: Optional[sequence.SortMethod] = typer.Option(
+    sort_method: Optional[model.SortMethod] = typer.Option(
         default="time-asc",
         help="Strategy used for sorting your pictures. Either by filename or EXIF time, in ascending or descending order.",
     ),
     split_distance: Optional[int] = typer.Option(
         default=100,
         help="Maximum distance between two pictures to be considered in the same sequence (in meters).",
     ),
     split_time: Optional[int] = typer.Option(
         default=60,
         help="Maximum time interval between two pictures to be considered in the same sequence (in seconds).",
     ),
+    picture_upload_timeout: float = typer.Option(
+        default=60.0,
+        help="Timeout time to receive the first byte of the response for each picture upload (in seconds)",
+    ),
+    disable_cert_check: Annotated[
+        bool,
+        typer.Option(
+            "--disable-cert-check/--enable-cert-check",
+            help="Disable SSL certificates checks while uploading. This should not be used, unless if you -really- know what you are doing.",
+        ),
+    ] = False,
 ):
     """Processes and sends a given sequence on your GeoVisio API"""
 
     def cmd():
         if user or password:
             raise exception.CliException(
                 "user/password authentication have been deprecated, use a token or `geovisio login` instead"
             )
         geovisio = model.Geovisio(url=api_url, token=token)
-        sequence.upload(
+        geovisio_cli.sequences.upload.upload(
             path,
             geovisio,
             wait=wait,
             alreadyBlurred=isBlurred,
             title=title,
             sortMethod=sort_method,
-            splitParams=sequence.SplitParams(
+            splitParams=geovisio_cli.sequences.process.standard.SplitParams(
                 maxDistance=split_distance,
                 maxTime=split_time,
             ),
+            pictureUploadTimeout=picture_upload_timeout,
+            disableCertCheck=disable_cert_check,
         )
 
     _run_command(cmd, "importing collection")
 
 
 @app.command()
 def test_process(
     path: Path = typer.Argument(..., help="Local path to your sequence folder"),
     title: Optional[str] = typer.Option(
         default=None,
         help="Collection title. If not provided, the title will be the directory name.",
     ),
-    sort_method: Optional[sequence.SortMethod] = typer.Option(
+    sort_method: Optional[model.SortMethod] = typer.Option(
         default="time-asc",
         help="Strategy used for sorting your pictures. Either by filename or EXIF time, in ascending or descending order.",
     ),
     split_distance: Optional[int] = typer.Option(
         default=100,
         help="Maximum distance between two pictures to be considered in the same sequence (in meters).",
     ),
@@ -128,24 +146,24 @@
         default=60,
         help="Maximum time interval between two pictures to be considered in the same sequence (in seconds).",
     ),
 ):
     """(For testing) Generates a TOML file with metadata used for upload"""
 
     def cmd():
-        sequence.process(
+        geovisio_cli.sequences.process.standard.process(
             path,
             title,
             sortMethod=sort_method,
-            splitParams=sequence.SplitParams(
+            splitParams=geovisio_cli.sequences.process.standard.SplitParams(
                 maxDistance=split_distance,
                 maxTime=split_time,
             ),
         )
-        outputFile = os.path.join(path, sequence.SEQUENCE_TOML_FILE)
+        outputFile = os.path.join(path, model.SEQUENCE_TOML_FILE)
         print(
             "\n✅ [green]Metadata file saved to: [bold]" + outputFile + "[/bold][/green]"
         )
 
     _run_command(cmd, "processing collection")
 
 
@@ -153,14 +171,21 @@
 def collection_status(
     id: Optional[str] = typer.Option(default=None, help="Id of the collection"),
     api_url: Optional[str] = typer.Option(default=None, help="GeoVisio endpoint URL"),
     location: Optional[str] = typer.Option(
         default=None, help="Full url of the collection"
     ),
     wait: bool = typer.Option(default=False, help="wait for all pictures to be ready"),
+    disable_cert_check: Annotated[
+        bool,
+        typer.Option(
+            "--disable-cert-check/--enable-cert-check",
+            help="Disable SSL certificates checks while uploading. This should not be used, unless if you -really- know what you are doing.",
+        ),
+    ] = False,
 ):
     """
     Print the status of a collection.\n
     Either a --location should be provided, with the full location url of the collection
     or only the --id combined with the --api-url
     """
 
@@ -170,19 +195,22 @@
                 raise exception.CliException(
                     "The way to identify the collection should be either with --location or with --id combined with --api-url"
                 )
             l = f"{api_url}/api/collections/{id}"
         else:
             l = location
 
-        mySequence = sequence.Sequence(id=id, location=l)
-        sequence.display_sequence_status(mySequence)
+        mySequence = model.Sequence(id=id, location=l)
+        with requests.session() as s:
+            if disable_cert_check:
+                s.verify = False
+            geovisio_cli.sequences.status.display_sequence_status(s, mySequence)
 
-        if wait:
-            sequence.wait_for_sequence(mySequence)
+            if wait:
+                geovisio_cli.sequences.status.wait_for_sequence(s, mySequence)
 
     _run_command(cmd, "getting collection status")
 
 
 @app.command(
     help=f"""
     Authenticate into the given instance, and save credentials in a configuration file.
@@ -190,17 +218,26 @@
     This will generate credentials, and ask the user to visit a page to associate those credentials to the user's account.
 
     The credentials will be stored in {auth.get_config_file_path()}
     """
 )
 def login(
     api_url: str = typer.Option(..., help="GeoVisio endpoint URL"),
+    disable_cert_check: Annotated[
+        bool,
+        typer.Option(
+            "--disable-cert-check/--enable-cert-check",
+            help="Disable SSL certificates checks while uploading. This should not be used, unless if you -really- know what you are doing.",
+        ),
+    ] = False,
 ):
     return _run_command(
-        lambda: auth.create_auth_credentials(model.Geovisio(url=api_url)),
+        lambda: auth.create_auth_credentials(
+            model.Geovisio(url=api_url), disable_cert_check
+        ),
         "authenticating",
     )
 
 
 def _run_command(command, command_name_for_error):
     try:
         utils.check_if_lastest_version()
```

### Comparing `geovisio_cli-0.3.0/geovisio_cli/utils.py` & `geovisio_cli-0.3.1/geovisio_cli/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from geovisio_cli.exception import CliException
 from rich import print
 import requests
 
-REQUESTS_TIMEOUT = 30
+REQUESTS_CNX_TIMEOUT = 6.1  # max number of seconds to wait for the connection to establish, cf https://requests.readthedocs.io/en/latest/user/advanced/#timeouts
+REQUESTS_TIMEOUT = (REQUESTS_CNX_TIMEOUT, 30)
 
 
-def test_geovisio_url(geovisio: str):
+def test_geovisio_url(session: requests.Session, geovisio: str):
     full_url = f"{geovisio}/api"
     try:
-        r = requests.get(full_url, timeout=REQUESTS_TIMEOUT)
+        r = session.get(full_url, timeout=REQUESTS_TIMEOUT)
     except (
         requests.Timeout,
         requests.ConnectionError,
         requests.ConnectTimeout,
         requests.TooManyRedirects,
     ) as e:
         raise CliException(
```

### Comparing `geovisio_cli-0.3.0/pyproject.toml` & `geovisio_cli-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/tests/fixtures/e1.jpg` & `geovisio_cli-0.3.1/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/tests/fixtures/e2.jpg` & `geovisio_cli-0.3.1/tests/fixtures/e2.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/tests/fixtures/e3.jpg` & `geovisio_cli-0.3.1/tests/fixtures/e3.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/tests/integration/conftest.py` & `geovisio_cli-0.3.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/tests/integration/docker-compose-geovisio.yml` & `geovisio_cli-0.3.1/tests/integration/docker-compose-geovisio.yml`

 * *Files 0% similar despite different names*

```diff
@@ -71,12 +71,11 @@
       - ./keycloak-realm.json:/opt/keycloak/data/import/geovisio_realm.json
 
     networks:
       keycloak:
         aliases:
           - keycloak.localtest.me
 
-
 networks:
   db: {}
   keycloak: {}
-  geovisio: {}
+  geovisio: {}
```

### Comparing `geovisio_cli-0.3.0/tests/integration/docker-compose-gitlab-override.yml` & `geovisio_cli-0.3.1/tests/integration/docker-compose-gitlab-override.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/tests/integration/keycloak-realm.json` & `geovisio_cli-0.3.1/tests/integration/keycloak-realm.json`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/tests/integration/test_auth.py` & `geovisio_cli-0.3.1/tests/integration/test_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-from geovisio_cli import auth, sequence, exception, model
+from geovisio_cli.sequences import upload
+from geovisio_cli import auth, exception, model
 import os
 import pytest
 from pathlib import Path
 from ..conftest import FIXTURE_DIR
 from .conftest import _login
 import requests
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
     os.path.join(FIXTURE_DIR, "e2.jpg"),
     os.path.join(FIXTURE_DIR, "e3.jpg"),
 )
 def test_auth_with_token(geovisio_with_token, datafiles):
-    reports = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio_with_token, title="some title"
+    reports = upload.upload(
+        path=Path(datafiles),
+        geovisio=geovisio_with_token,
+        title="some title",
+        pictureUploadTimeout=20,
     )
 
     assert len(reports) == 1
     assert len(reports[0].uploaded_pictures) == 3
     assert len(reports[0].errors) == 0
 
 
@@ -39,16 +43,19 @@
         assert (
             claim.text == "You are now logged in the CLI, you can upload your pictures"
         )
 
     assert os.path.exists(tmp_path / "geovisio" / "config.toml")
 
     # doing a geovisio upload should work without crendentials now
-    uploadReports = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio, title="some title"
+    uploadReports = upload.upload(
+        path=Path(datafiles),
+        geovisio=geovisio,
+        title="some title",
+        pictureUploadTimeout=20,
     )
     assert len(uploadReports) == 1
     assert len(uploadReports[0].uploaded_pictures) == 3
     assert len(uploadReports[0].errors) == 0
 
 
 @pytest.mark.datafiles(
@@ -65,15 +72,20 @@
     assert os.path.exists(tmp_path / "geovisio" / "config.toml")
 
     # doing a geovisio upload should not work as the token is not usable yet
     with pytest.raises(
         exception.CliException,
         match="🔁 Computer not authenticated yet, impossible to upload pictures, but you can try again the same upload command after finalizing the login",
     ):
-        sequence.upload(path=Path(datafiles), geovisio=geovisio, title="some title")
+        upload.upload(
+            path=Path(datafiles),
+            geovisio=geovisio,
+            title="some title",
+            pictureUploadTimeout=20,
+        )
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
 )
 def test_login_on_invalid_url_path(geovisio_with_token, datafiles):
     with pytest.raises(exception.CliException) as e:
```

### Comparing `geovisio_cli-0.3.0/tests/integration/test_upload.py` & `geovisio_cli-0.3.1/tests/integration/test_upload.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 import os
 import pytest
+
+import geovisio_cli.sequences.status
+import geovisio_cli.sequences.upload
 from ..conftest import FIXTURE_DIR
 from pathlib import Path
 import requests
-from geovisio_cli import sequence, exception, model
+from geovisio_cli import exception, model
 from datetime import timedelta
 import toml
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
     os.path.join(FIXTURE_DIR, "e2.jpg"),
     os.path.join(FIXTURE_DIR, "e3.jpg"),
 )
 def test_valid_upload(geovisio_with_token, datafiles):
-    uploadReports = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio_with_token, title="some title"
+    uploadReports = geovisio_cli.sequences.upload.upload(
+        path=Path(datafiles),
+        geovisio=geovisio_with_token,
+        title="some title",
+        pictureUploadTimeout=20,
     )
     assert len(uploadReports) == 1
     assert len(uploadReports[0].uploaded_pictures) == 3
     assert len(uploadReports[0].errors) == 0
 
-    collection = sequence.Sequence(location=uploadReports[0].location)
-    sequence.wait_for_sequence(collection, timeout=timedelta(minutes=1))
-    status = sequence.status(collection)
-    sequence_info = sequence.info(collection)
+    collection = model.Sequence(location=uploadReports[0].location)
+    with requests.session() as s:
+        geovisio_cli.sequences.status.wait_for_sequence(
+            s, collection, timeout=timedelta(minutes=1)
+        )
+        status = geovisio_cli.sequences.status.get_status(s, collection)
+        sequence_info = geovisio_cli.sequences.status.info(s, collection)
     # 3 pictures should have been uploaded
     assert len(status.pictures) == 3
 
     for i in status.pictures:
         assert i.status == "ready"
 
     # the collection should also have 3 items
@@ -36,21 +45,19 @@
     collection.raise_for_status()
 
     features = collection.json()["features"]
     assert len(features) == 3
 
     assert sequence_info.title == "some title"
     assert sequence_info.interior_orientation == [
-        sequence.InteriorOrientation(
-            make="SONY", model="FDR-X1000V", field_of_view=None
-        )
+        model.InteriorOrientation(make="SONY", model="FDR-X1000V", field_of_view=None)
     ]
 
     # Check generated TOML file
-    tomlFile = datafiles / sequence.SEQUENCE_TOML_FILE
+    tomlFile = datafiles / model.SEQUENCE_TOML_FILE
     with open(tomlFile, "r") as f:
         tomlFileContent = f.read()
         seqToml = toml.loads(tomlFileContent)
         assert seqToml["1"]["sequence"]["id"] == sequence_info.id
         assert seqToml["1"]["pictures"]["e1.jpg"]["id"] == features[0]["id"]
         assert seqToml["1"]["pictures"]["e2.jpg"]["id"] == features[1]["id"]
         assert seqToml["1"]["pictures"]["e3.jpg"]["id"] == features[2]["id"]
@@ -67,44 +74,46 @@
     picE2bak = datafiles / "e2.bak"
     os.rename(picE2, picE2bak)
     with open(picE2, "w") as picE2file:
         picE2file.write("")
         picE2file.close()
 
     # Start upload -> 2 uploaded pics + 1 failure
-    uploadReports = sequence.upload(
+    uploadReports = geovisio_cli.sequences.upload.upload(
         path=Path(datafiles),
         geovisio=geovisio_with_token,
         title="some title",
-        sortMethod=sequence.SortMethod.filename_asc,
+        sortMethod=model.SortMethod.filename_asc,
+        pictureUploadTimeout=20,
     )
     assert len(uploadReports) == 1
     assert len(uploadReports[0].uploaded_pictures) == 2
     assert len(uploadReports[0].errors) == 1
     assert uploadReports[0].errors[0].position == 2
 
     # Check TOML file -> e2 has no ID but broken status
-    tomlFile = datafiles / sequence.SEQUENCE_TOML_FILE
+    tomlFile = datafiles / model.SEQUENCE_TOML_FILE
     with open(tomlFile, "r") as f:
         tomlFileContent = f.read()
         f.close()
         seqToml = toml.loads(tomlFileContent)
         assert seqToml["1"]["pictures"]["e2.jpg"].get("id") is None
         assert seqToml["1"]["pictures"]["e2.jpg"]["status"] == "broken"
 
     # Make e2 valid
     os.remove(picE2)
     os.rename(picE2bak, picE2)
 
     # Launch again upload : 1 uploaded pic + 0 failure
-    uploadReports2 = sequence.upload(
+    uploadReports2 = geovisio_cli.sequences.upload.upload(
         path=Path(datafiles),
         geovisio=geovisio_with_token,
         title="some title",
-        sortMethod=sequence.SortMethod.filename_asc,
+        sortMethod=model.SortMethod.filename_asc,
+        pictureUploadTimeout=20,
     )
     assert uploadReports2[0].location == uploadReports[0].location
     assert len(uploadReports2[0].uploaded_pictures) == 1
     assert len(uploadReports2[0].errors) == 0
 
     # Check TOML file -> everything has ID and looks like a charm
     with open(tomlFile, "r") as f:
@@ -128,40 +137,47 @@
     os.path.join(FIXTURE_DIR, "e1.jpg"),
     os.path.join(FIXTURE_DIR, "e2.jpg"),
     os.path.join(FIXTURE_DIR, "e3.jpg"),
 )
 def test_upload_twice(geovisio_with_token, datafiles):
     """Uploading twice the same sequence, should result of nothing done in the second upload"""
     # Start upload -> 2 uploaded pics + 1 failure
-    uploadReports = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio_with_token, title="some title"
+    uploadReports = geovisio_cli.sequences.upload.upload(
+        path=Path(datafiles),
+        geovisio=geovisio_with_token,
+        title="some title",
+        pictureUploadTimeout=20,
     )
     assert len(uploadReports) == 1
     assert len(uploadReports[0].uploaded_pictures) == 3
     assert len(uploadReports[0].errors) == 0
 
     # Launch again upload : 1 uploaded pic + 0 failure
-    uploadReports2 = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio_with_token, title="some title"
+    uploadReports2 = geovisio_cli.sequences.upload.upload(
+        path=Path(datafiles),
+        geovisio=geovisio_with_token,
+        title="some title",
+        pictureUploadTimeout=20,
     )
     assert len(uploadReports2) == 1
     assert uploadReports2[0].location == uploadReports[0].location
     assert len(uploadReports2[0].uploaded_pictures) == 0
     assert len(uploadReports2[0].errors) == 0
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
 )
 def test_upload_on_invalid_url_host(datafiles):
     with pytest.raises(exception.CliException) as e:
-        sequence.upload(
+        geovisio_cli.sequences.upload.upload(
             path=Path(datafiles),
             geovisio=model.Geovisio(url="http://some_invalid_url"),
             title="some title",
+            pictureUploadTimeout=20,
         )
     msg = str(e.value)
     assert msg.startswith(
         """The API is not reachable. Please check error and used URL below, and retry later if the URL is correct.
 
 [bold]Used URL:[/bold] http://some_invalid_url/api
 [bold]Error:[/bold]"""
@@ -170,20 +186,21 @@
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
 )
 def test_upload_on_invalid_url_path(geovisio_with_token, datafiles):
     with pytest.raises(exception.CliException) as e:
-        sequence.upload(
+        geovisio_cli.sequences.upload.upload(
             path=Path(datafiles),
             geovisio=model.Geovisio(
                 url=geovisio_with_token.url + "/some_additional_path"
             ),
             title=None,
+            pictureUploadTimeout=20,
         )
     msg = str(e.value)
     assert msg.startswith(
         f"""The API URL is not valid.
 
 Note that your URL should be the API root (something like https://geovisio.fr, https://panoramax.ign.fr or any other geovisio instance).
 Please make sure you gave the correct URL and retry.
@@ -194,18 +211,19 @@
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
 )
 def test_upload_on_invalid_url_schema(datafiles):
     with pytest.raises(exception.CliException) as e:
-        sequence.upload(
+        geovisio_cli.sequences.upload.upload(
             path=Path(datafiles),
             geovisio=model.Geovisio(url="a non valid url at all"),
             title=None,
+            pictureUploadTimeout=20,
         )
     assert str(e.value).startswith(
         """Error while connecting to the API. Please check error and used URL below
 
 [bold]Used URL:[/bold] a non valid url at all/api
 [bold]Error:[/bold]"""
     )
```

### Comparing `geovisio_cli-0.3.0/tests/test_process.py` & `geovisio_cli-0.3.1/tests/test_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pytest
 import os
-from geovisio_cli import sequence
+from geovisio_cli.sequences.process import standard
 from .conftest import FIXTURE_DIR
 from pathlib import Path, PurePath
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
     os.path.join(FIXTURE_DIR, "e2.jpg"),
     os.path.join(FIXTURE_DIR, "e3.jpg"),
     os.path.join(FIXTURE_DIR, "not_a_pic.md"),
 )
 def test_upload_with_invalid_file(datafiles):
-    ms = sequence.process(path=Path(datafiles), title=None)
+    ms = standard.process(path=Path(datafiles), title=None)
 
     assert len(ms.sequences) == 1
     s = ms.sequences[0]
     assert len(s.pictures) == 3
     assert [PurePath(p.path).stem for p in s.pictures] == ["e1", "e2", "e3"]
     assert s.title == Path(datafiles).name
```

### Comparing `geovisio_cli-0.3.0/tests/test_utils.py` & `geovisio_cli-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.0/PKG-INFO` & `geovisio_cli-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geovisio_cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: Geovio client cli tool
 Author-email: Antoine Desbordes <antoine.desbordes@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests ~= 2.28.0
 Requires-Dist: typer ~= 0.9.0
@@ -197,14 +197,20 @@
 
 If you don't have Docker Compose, or want to use an existing GeoVisio test instance (to speed up tests), you can pass the `--external-geovisio-url` option to pytest:
 
 ```bash
 pytest --external-geovisio-url=http://localhost:5000
 ```
 
+#### Using with an unsecure geovisio API
+
+The CLI parameter `--disable-cert-check` is available to use with an unsecure geovisio API (or when behind proxies messing with ssl). 
+
+There are no automated test for this, but you can run a geovisio with `flask run --cert=adhoc` to manually test this. 
+
 ### Documentation
 
 High-level documentation is handled by [Typer](https://typer.tiangolo.com/). You can update the generated `USAGE.md` file using this command:
 
 ```bash
 make docs
 ```
```

