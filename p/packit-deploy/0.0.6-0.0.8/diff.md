# Comparing `tmp/packit_deploy-0.0.6.tar.gz` & `tmp/packit_deploy-0.0.8.tar.gz`

## Comparing `packit_deploy-0.0.6.tar` & `packit_deploy-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,35 @@
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/.github/workflows/test.yml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/config/basic/packit.yml
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/config/noproxy/packit.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/__about__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/__init__.py
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/cli.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/config.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/docker_helpers.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/packit_constellation.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/tests/test_cli.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/tests/test_config.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/tests/test_integration.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/README.md
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/conftest.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/.github/workflows/build-proxy.yml
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/config/basic/packit.yml
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/config/complete/packit.yml
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/config/nodemo/packit.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/config/noproxy/packit.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/Dockerfile
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/README.md
+-rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/build
+-rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/common
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/nginx.conf
+-rwxr-xr-x   0        0        0      118 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/push
+-rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/bin/dhparams
+-rwxr-xr-x   0        0        0     1293 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/bin/packit-proxy
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/bin/self-signed-certificate
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/ssl/certificate.pem
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/ssl/dhparam.pem
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/proxy/ssl/key.pem
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/src/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/src/packit_deploy/__about__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/src/packit_deploy/__init__.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/src/packit_deploy/cli.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/src/packit_deploy/config.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/src/packit_deploy/docker_helpers.py
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/src/packit_deploy/packit_constellation.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/tests/test_cli.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/tests/test_config.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/tests/test_integration.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/README.md
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 packit_deploy-0.0.8/PKG-INFO
```

### Comparing `packit_deploy-0.0.6/.github/workflows/test.yml` & `packit_deploy-0.0.8/.github/workflows/test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,33 +6,37 @@
       - main
   push:
     branches:
       - main
 
 env:
   CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+  BRANCH_NAME: ${{ github.head_ref || github.ref_name }}
 
 jobs:
-  build:
+  run:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
+      - name: Set up QEMU
+        uses: docker/setup-qemu-action@v2
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install hatch
+          proxy/build
       - name: Lint
         run: |
           hatch run lint:style
       - name: Test
         run: |
           hatch run cov-ci
       - name: Upload to Codecov
```

### Comparing `packit_deploy-0.0.6/config/basic/packit.yml` & `packit_deploy-0.0.8/config/noproxy/packit.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-## The name of the docker network that containers will be attached to.
-## If you want to proxy OrderlyWeb to the host, you will need to
-## arrange a proxy on this network, or use dev_mode in the web section
-## below.
 ## Prefix for container names; we'll use {container_prefix}-(container_name)
 container_prefix: packit
 
 ## Set this flag to true to prevent use of --volumes in the cli to remove
 ## volumes on stop
 protect_data: false
 
@@ -20,17 +16,19 @@
 ## Names of the docker volumes to use:
 ##
 ## outpack: stores the outpack metadata
 ## proxy_logs: stores logs from the reverse proxy (only used if proxy is given)
 ## (More volumes are anticipated as the tool develops)
 volumes:
   outpack: outpack_volume
-  proxy_logs: orderly_web_proxy_logs
+  proxy_logs: packit_proxy_logs
 
 outpack:
+  initial:
+    url: https://github.com/reside-ic/orderly3-example.git
   server:
     name: outpack_server
     tag: main
   migrate:
     name: outpack.orderly
     tag: main
```

### Comparing `packit_deploy-0.0.6/config/noproxy/packit.yml` & `packit_deploy-0.0.8/config/basic/packit.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## The name of the docker network that containers will be attached to.
+## If you want to proxy Packit to the host, you will need to
+## arrange a proxy on this network, or use dev_mode in the web section
+## below.
 ## Prefix for container names; we'll use {container_prefix}-(container_name)
 container_prefix: packit
 
 ## Set this flag to true to prevent use of --volumes in the cli to remove
 ## volumes on stop
 protect_data: false
 
@@ -16,19 +20,19 @@
 ## Names of the docker volumes to use:
 ##
 ## outpack: stores the outpack metadata
 ## proxy_logs: stores logs from the reverse proxy (only used if proxy is given)
 ## (More volumes are anticipated as the tool develops)
 volumes:
   outpack: outpack_volume
-  proxy_logs: orderly_web_proxy_logs
+  proxy_logs: packit_proxy_logs
 
 outpack:
   initial:
-    source: demo
+    url: https://github.com/reside-ic/orderly3-example.git
   server:
     name: outpack_server
     tag: main
   migrate:
     name: outpack.orderly
     tag: main
 
@@ -40,7 +44,19 @@
     name: packit
     tag: main
   db:
     name: packit-db
     tag: main
     user: packituser
     password: changeme
+
+## If running a proxy directly, fill this section in.  Otherwise you
+## are responsible for proxying the application out of the docker
+## network
+proxy:
+  enabled: true
+  hostname: localhost
+  port_http: 80
+  port_https: 443
+  image:
+    name: packit-proxy
+    tag: mrc-4319
```

### Comparing `packit_deploy-0.0.6/src/packit_deploy/cli.py` & `packit_deploy-0.0.8/src/packit_deploy/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from packit_deploy.config import PackitConfig
 from packit_deploy.packit_constellation import PackitConstellation
 
 
 def main(argv=None):
     path, extra, options, args = parse_args(argv)
     if args.version:
-        print(about.__version__)
         return about.__version__
     else:
         cfg = PackitConfig(path, extra, options)
         obj = PackitConstellation(cfg)
         if args.action == "start":
             packit_start(obj, args)
         elif args.action == "status":
```

### Comparing `packit_deploy-0.0.6/src/packit_deploy/config.py` & `packit_deploy-0.0.8/src/packit_deploy/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,34 +4,32 @@
 from packit_deploy.docker_helpers import DockerClient
 
 
 class PackitConfig:
     def __init__(self, path, extra=None, options=None):
         dat = config.read_yaml(f"{path}/packit.yml")
         dat = config.config_build(path, dat, extra, options)
+        self.vault = config.config_vault(dat, ["vault"])
         self.network = config.config_string(dat, ["network"])
         self.protect_data = config.config_boolean(dat, ["protect_data"])
         self.volumes = {"outpack": config.config_string(dat, ["volumes", "outpack"])}
 
         self.container_prefix = config.config_string(dat, ["container_prefix"])
         self.repo = config.config_string(dat, ["repo"])
 
+        if "ssh" in dat:
+            self.ssh_public = config.config_string(dat, ["ssh", "public"])
+            self.ssh_private = config.config_string(dat, ["ssh", "private"])
+            self.ssh = True
+        else:
+            self.ssh = False
+
         if "initial" in dat["outpack"]:
-            source = config.config_string(dat, ["outpack", "initial", "source"])
-            if source == "demo":
-                self.outpack_demo = True
-                self.outpack_source_url = None
-            elif source == "clone":
-                self.outpack_demo = False
-                self.outpack_source_url = config.config_string(dat, ["outpack", "initial", "url"])
-            else:
-                err = "Unknown outpack initial source. Valid values are 'demo' and 'clone'"
-                raise Exception(err)
+            self.outpack_source_url = config.config_string(dat, ["outpack", "initial", "url"])
         else:
-            self.outpack_demo = False
             self.outpack_source_url = None
 
         self.outpack_ref = self.build_ref(dat, "outpack", "server")
         self.packit_api_ref = self.build_ref(dat, "packit", "api")
         self.packit_ref = self.build_ref(dat, "packit", "app")
         self.packit_db_ref = self.build_ref(dat, "packit", "db")
         self.packit_db_user = config.config_string(dat, ["packit", "db", "user"])
@@ -52,14 +50,31 @@
         }
 
         if "proxy" in dat and dat["proxy"]:
             self.proxy_enabled = config.config_boolean(dat, ["proxy", "enabled"], True)
         else:
             self.proxy_enabled = False
 
+        if self.proxy_enabled:
+            self.proxy_hostname = config.config_string(dat, ["proxy", "hostname"])
+            self.proxy_port_http = config.config_integer(dat, ["proxy", "port_http"])
+            self.proxy_port_https = config.config_integer(dat, ["proxy", "port_https"])
+            ssl = config.config_dict(dat, ["proxy", "ssl"], True)
+            self.proxy_ssl_self_signed = ssl is None
+            if not self.proxy_ssl_self_signed:
+                self.proxy_ssl_certificate = config.config_string(dat, ["proxy", "ssl", "certificate"], True)
+                self.proxy_ssl_key = config.config_string(dat, ["proxy", "ssl", "key"], True)
+
+            self.proxy_name = config.config_string(dat, ["proxy", "image", "name"])
+            self.proxy_tag = config.config_string(dat, ["proxy", "image", "tag"])
+            self.proxy_ref = constellation.ImageReference(self.repo, self.proxy_name, self.proxy_tag)
+            self.containers["proxy"] = "proxy"
+            self.images["proxy"] = self.proxy_ref
+            self.volumes["proxy_logs"] = config.config_string(dat, ["volumes", "proxy_logs"])
+
     def build_ref(self, dat, section, subsection):
         name = config.config_string(dat, [section, subsection, "name"])
         tag = config.config_string(dat, [section, subsection, "tag"])
         return constellation.ImageReference(self.repo, name, tag)
 
     def get_container(self, name):
         with DockerClient() as cl:
```

### Comparing `packit_deploy-0.0.6/src/packit_deploy/docker_helpers.py` & `packit_deploy-0.0.8/src/packit_deploy/docker_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # the test log almost impossible to read.
 #
 # https://github.com/kennethreitz/requests/issues/1882#issuecomment-52281285
 # https://github.com/kennethreitz/requests/issues/3912
 #
 # This little helper can be used with python's with statement as
 #
-#      with docker_client() as cl:
+#      with DockerClient() as cl:
 #        cl.containers...
 #
 # and will close *most* unused handles on exit.  It's easier to look
 # at than endless try/finally blocks everywhere.
 import docker
```

### Comparing `packit_deploy-0.0.6/tests/test_cli.py` & `packit_deploy-0.0.8/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,20 +40,17 @@
     assert args.action == "status"
 
     res = cli.parse_args(["--version"])
     args = res[3]
     assert args.version is True
 
 
-def test_prints_version():
-    with mock.patch("builtins.print") as p:
-        cli.main(["--version"])
-
-    assert p.called
-    assert p.call_args[0][0] == "0.0.5"
+def test_version():
+    res = cli.main(["--version"])
+    assert res == "0.0.8"
 
 
 def test_args_passed_to_start():
     with mock.patch("src.packit_deploy.cli.packit_start") as f:
         cli.main(["start", "config/noproxy"])
 
     assert f.called
```

### Comparing `packit_deploy-0.0.6/tests/test_config.py` & `packit_deploy-0.0.8/tests/test_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import pytest
-
 from src.packit_deploy.config import PackitConfig
 
 
 def test_config_no_proxy():
     cfg = PackitConfig("config/noproxy")
     assert cfg.network == "packit-network"
     assert cfg.volumes["outpack"] == "outpack_volume"
@@ -17,36 +15,54 @@
 
     assert len(cfg.images) == 4
     assert str(cfg.images["outpack-server"]) == "mrcide/outpack_server:main"
     assert str(cfg.images["packit"]) == "mrcide/packit:main"
     assert str(cfg.images["packit-db"]) == "mrcide/packit-db:main"
     assert str(cfg.images["packit-api"]) == "mrcide/packit-api:main"
 
-    assert cfg.outpack_demo is True
-    assert cfg.outpack_source_url is None
+    assert cfg.outpack_source_url is not None
     assert cfg.proxy_enabled is False
     assert cfg.protect_data is False
 
     assert cfg.packit_db_user == "packituser"
     assert cfg.packit_db_password == "changeme"
 
 
-def test_config_proxy():
+def test_config_proxy_disabled():
     options = {"proxy": {"enabled": False}}
-    cfg = PackitConfig("config/noproxy", options=options)
+    cfg = PackitConfig("config/basic", options=options)
     assert cfg.proxy_enabled is False
 
 
+def test_config_proxy():
+    cfg = PackitConfig("config/basic")
+    assert cfg.proxy_enabled
+    assert cfg.proxy_ssl_self_signed
+    assert "proxy" in cfg.containers
+    assert str(cfg.images["proxy"]) == "mrcide/packit-proxy:mrc-4319"
+    assert cfg.proxy_hostname == "localhost"
+    assert cfg.proxy_port_http == 80
+    assert cfg.proxy_port_https == 443
+
+    cfg = PackitConfig("config/complete")
+    assert cfg.proxy_enabled
+    assert not cfg.proxy_ssl_self_signed
+    assert cfg.proxy_ssl_certificate == "VAULT:secret/cert:value"
+    assert cfg.proxy_ssl_key == "VAULT:secret/key:value"
+
+
 def test_outpack_initial_source():
-    options = {"outpack": {"initial": {"source": "wrong"}}}
-    with pytest.raises(Exception) as err:
-        PackitConfig("config/noproxy", options=options)
-    assert str(err.value) == "Unknown outpack initial source. Valid values are 'demo' and 'clone'"
-
-    options = {"outpack": {"initial": {"source": "clone", "url": "whatever"}}}
-    cfg = PackitConfig("config/noproxy", options=options)
-    assert cfg.outpack_demo is False
-    assert cfg.outpack_source_url == "whatever"
+    cfg = PackitConfig("config/complete")
+    assert cfg.outpack_source_url == "https://github.com/reside-ic/orderly3-example.git"
 
-    cfg = PackitConfig("config/basic")
-    assert cfg.outpack_demo is False
+    cfg = PackitConfig("config/nodemo")
     assert cfg.outpack_source_url is None
+
+
+def test_ssh():
+    cfg = PackitConfig("config/complete")
+    assert cfg.ssh_public == "VAULT:secret/ssh:public"
+    assert cfg.ssh_private == "VAULT:secret/ssh:private"
+    assert cfg.ssh
+
+    cfg = PackitConfig("config/basic")
+    assert not cfg.ssh
```

### Comparing `packit_deploy-0.0.6/LICENSE.txt` & `packit_deploy-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.6/README.md` & `packit_deploy-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.6/pyproject.toml` & `packit_deploy-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 
 [tool.hatch.envs.default]
 dependencies = [
     "constellation==1.0.0",
     "coverage[toml]>=6.5",
     "docker",
     "docopt",
-    "pytest"
+    "pytest",
+    "vault_dev"
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
     "- coverage combine",
     "coverage report",
```

### Comparing `packit_deploy-0.0.6/PKG-INFO` & `packit_deploy-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packit-deploy
-Version: 0.0.6
+Version: 0.0.8
 Project-URL: Documentation, https://github.com/mrc-ide/packit-deploy#readme
 Project-URL: Issues, https://github.com/mrc-ide/packit-deploy/issues
 Project-URL: Source, https://github.com/mrc-ide/packit-deploy
 Author-email: Alex Hill <alex.hill@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

