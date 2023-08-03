# Comparing `tmp/montagu_deploy-0.0.2.tar.gz` & `tmp/montagu_deploy-0.0.3.tar.gz`

## Comparing `montagu_deploy-0.0.2.tar` & `montagu_deploy-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,19 @@
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/basic/diagnostic-reports.yml
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/basic/montagu.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/ci/diagnostic-reports.yml
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/ci/montagu.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/complete/diagnostic-reports.yml
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/complete/montagu.yml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/__about__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/admin.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/cli.py
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/config.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/database.py
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/montagu_constellation.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/orderly-web.yml
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/test_cli.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/test_config.py
--rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/test_constellation.py
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/test_integration.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/utils.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/README.md
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/config/basic/montagu.yml
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/config/complete/montagu.yml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/src/montagu_deploy/__about__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/src/montagu_deploy/__init__.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/src/montagu_deploy/cli.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/src/montagu_deploy/config.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/src/montagu_deploy/database.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/src/montagu_deploy/montagu_constellation.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/tests/test_cli.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/tests/test_config.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/tests/test_constellation.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/tests/test_integration.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/README.md
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 montagu_deploy-0.0.3/PKG-INFO
```

### Comparing `montagu_deploy-0.0.2/.github/workflows/test.yml` & `montagu_deploy-0.0.3/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -31,16 +31,13 @@
         run: |
           python -m pip install --upgrade pip
           pip install hatch
       - name: Lint
         run: |
           hatch run lint:style
       - name: Test
-        env:
-          VAULT_TOKEN: ${{ secrets.VAULT_TOKEN }}
-          YOUTRACK_TOKEN: ${{ secrets.YOUTRACK_TOKEN }}
         run: |
           hatch run cov-ci
       - name: Upload to Codecov
         uses: codecov/codecov-action@v3
         with:
           fail_ci_if_error: true
```

### Comparing `montagu_deploy-0.0.2/config/basic/montagu.yml` & `montagu_deploy-0.0.3/config/basic/montagu.yml`

 * *Files 27% similar despite different names*

```diff
@@ -21,22 +21,18 @@
   db: db_volume
   burden_estimates: burden_estimate_files
   emails: emails
   templates: template_volume
   guidance: guidance_volume
   static: static_volume
   static_logs: static_logs
-  mq: mq
 
 api:
   name: montagu-api
   tag: master
-  admin:
-    name: montagu-cli
-    tag: master
 db:
   name: montagu-db
   tag: master
   root_user: vimc
   migrate:
     name: montagu-migrate
     tag: master
@@ -67,53 +63,22 @@
     - role
     - role_permission
 proxy:
   name: montagu-reverse-proxy
   tag: vimc-7152
   port_http: 80
   port_https: 443
+  metrics:
+    repo: nginx
+    name: nginx-prometheus-exporter
+    tag: 0.10.0
 contrib:
   name: montagu-contrib-portal
   tag: master
 admin:
   name: montagu-admin-portal
   tag: master
 static:
   name: montagu-static
   tag: master
-mq:
-  repo: docker.io
-  name: redis
-  tag: latest
-  port: 6379
-flower:
-  repo: mher
-  name: flower
-  tag: 0.9.5
-  port: 5555
-task_queue:
-  name: task-queue-worker
-  tag: master
-  tasks:
-    diagnostic_reports:
-      use_additional_recipients: false
-      poll_seconds: 5
-    archive_folder_contents:
-      min_file_age_seconds: 3600
-  servers:
-    youtrack:
-      token: faketoken
-    orderlyweb:
-      url: http://orderly-web-web:8888
-    montagu:
-      user: montagu-task@imperial.ac.uk
-      password: password
-    smtp:
-      from: montagu-notifications@imperial.ac.uk
-# If fake_smtp_server config is provided, the task_queue will use this as its smtp server
-# Note this will override other config provided in the task_queue section above
-fake_smtp_server:
-  repo: reachfive
-  name: fake-smtp-server
-  tag: latest
 
-orderly_web_api_url: https://localhost/reports/api/v2
+orderly_web_api_url: http://montagu_orderly_web:8888/api/v2
```

### Comparing `montagu_deploy-0.0.2/config/ci/montagu.yml` & `montagu_deploy-0.0.3/config/complete/montagu.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-vault:
-  ## Address of the vault server.  This should be a string if it is
-  ## present.
-  addr: ~
-  auth:
-    ## Authentication type - must be either "token" or the name of a
-    ## supported authentication method.  These seem to be poorly
-    ## documented in the hvac, but include "github" for github
-    ## authentication.
-    ##
-    ## On a vault client object, see auth.implemented_class_names for
-    ## a list, which is currently
-    ##
-    ##     azure, github, gcp, kubernetes, ldap, mfa, okta
-    method: github
-
 ## Prefix for container names; we'll use {container_prefix}-(container_name)
 container_prefix: montagu
 
 ## Set this flag to true to prevent use of --volumes in the cli to remove
 ## volumes on stop
 protect_data: false
 
@@ -37,27 +21,26 @@
   db: db_volume
   burden_estimates: burden_estimate_files
   emails: emails
   templates: template_volume
   guidance: guidance_volume
   static: static_volume
   static_logs: static_logs
-  mq: mq
 
 api:
   name: montagu-api
   tag: master
-  admin:
-    name: montagu-cli
-    tag: master
+  email:
+    password: "changeme"
+    flow_url: "fakeurl"
 db:
   name: montagu-db
   tag: master
   root_user: vimc
-  root_password: changeme
+  root_password: "changeme"
   migrate:
     name: montagu-migrate
     tag: master
   users:
     api:
       password: "apipassword"
       permissions: all
@@ -66,14 +49,20 @@
       permissions: all
     orderly:
       password: "orderlypassword"
       permissions: all
     readonly:
       password: "readonlypassword"
       permissions: readonly
+    barman:
+      password: "barmanpassword"
+      option: superuser
+    streaming_barman:
+      password: "streamingpassword"
+      option: replication
   protected_tables:
     - gavi_support_level
     - activity_type
     - burden_outcome
     - gender
     - responsibility_set_status
     - impact_outcome
@@ -81,55 +70,37 @@
     - support_type
     - touchstone_status
     - permission
     - role
     - role_permission
 proxy:
   name: montagu-reverse-proxy
-  tag: vimc-7152
+  tag: master
   port_http: 80
   port_https: 443
+  metrics:
+    repo: nginx
+    name: nginx-prometheus-exporter
+    tag: 0.4.1
+  ## This section describes how to get the certificate in.  We
+  ## support two sources:
+  ##
+  ## 1. self signed certificates - just leave this section blank
+  ##
+  ## 2. certificates from strings - include the strings directly in
+  ##    the keys here, or more likely use a VAULT:<path>:<key>
+  ##    string to extract them from the vault.
+  ssl:
+    key: "k3y"
+    certificate: "cert"
+    dhparam: "param"
 contrib:
   name: montagu-contrib-portal
   tag: master
 admin:
   name: montagu-admin-portal
   tag: master
 static:
   name: montagu-static
   tag: master
-mq:
-  repo: docker.io
-  name: redis
-  tag: latest
-  port: 6379
-flower:
-  repo: mher
-  name: flower
-  tag: 0.9.5
-  port: 5555
-task_queue:
-  name: task-queue-worker
-  tag: master
-  tasks:
-    diagnostic_reports:
-      use_additional_recipients: false
-      poll_seconds: 5
-    archive_folder_contents:
-      min_file_age_seconds: 3600
-  servers:
-    ## To use value from the vault, use the format VAULT:<path>:<key>
-    youtrack:
-      token: VAULT:secret/youtrack/token:value
-    orderlyweb:
-      url: http://orderly-web-web:8888
-    montagu:
-      user: montagu-task@imperial.ac.uk
-      password: password
-    smtp:
-      from: montagu-notifications@imperial.ac.uk
-fake_smtp_server:
-  repo: reachfive
-  name: fake-smtp-server
-  tag: latest
 
-orderly_web_api_url: https://localhost/reports/api/v2
+orderly_web_api_url: http://montagu_orderly_web:8888/api/v2
```

### Comparing `montagu_deploy-0.0.2/src/montagu_deploy/cli.py` & `montagu_deploy-0.0.3/src/montagu_deploy/cli.py`

 * *Files identical despite different names*

### Comparing `montagu_deploy-0.0.2/src/montagu_deploy/database.py` & `montagu_deploy-0.0.3/src/montagu_deploy/database.py`

 * *Files identical despite different names*

### Comparing `montagu_deploy-0.0.2/src/montagu_deploy/montagu_constellation.py` & `montagu_deploy-0.0.3/src/montagu_deploy/montagu_constellation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from os.path import join
 
 import constellation
 import docker
-import yaml
 from constellation import docker_util
 from psycopg2 import connect
 
 from montagu_deploy import database
 
 
 class MontaguConstellation:
     def __init__(self, cfg):
         api = api_container(cfg)
         db = db_container(cfg)
         admin = admin_container(cfg)
         contrib = contrib_container(cfg)
         static = static_container(cfg)
         proxy = proxy_container(cfg)
-        mq = mq_container(cfg)
-        flower = flower_container(cfg)
-        task_queue = task_queue_container(cfg)
-
-        containers = [api, db, admin, contrib, static, proxy, mq, flower, task_queue]
-
-        if cfg.fake_smtp_ref:
-            fake_smtp = fake_smtp_container(cfg)
-            containers.append(fake_smtp)
+
+        containers = [api, db, admin, contrib, static, proxy]
 
         self.cfg = cfg
         self.obj = constellation.Constellation(
             "montagu", cfg.container_prefix, containers, cfg.network, cfg.volumes, data=cfg, vault_config=cfg.vault
         )
 
     def start(self, **kwargs):
         self.obj.start(**kwargs)
+        # The proxy metrics container cannot be started via constellation, because
+        # it has to belong to the same network as the proxy as soon as it is started
+        # and constellation starts containers on the 'none' network. So we provide
+        # start/stop/status methods for the metrics container that mimic the
+        # constellation behaviour
+        start_proxy_metrics(self.cfg)
 
     def stop(self, **kwargs):
+        stop_proxy_metrics(self.cfg)
         self.obj.stop(**kwargs)
 
     def status(self):
         self.obj.status()
+        status_proxy_metrics(self.cfg)
 
 
 def admin_container(cfg):
     name = cfg.containers["admin"]
     return constellation.ConstellationContainer(name, cfg.admin_ref)
 
 
@@ -61,60 +61,14 @@
     mounts = [
         constellation.ConstellationMount("static", "/www"),
         constellation.ConstellationMount("static_logs", "/var/log/caddy"),
     ]
     return constellation.ConstellationContainer(name, cfg.static_ref, mounts=mounts)
 
 
-def mq_container(cfg):
-    name = cfg.containers["mq"]
-    mounts = [
-        constellation.ConstellationMount("mq", "/data"),
-    ]
-    return constellation.ConstellationContainer(name, cfg.mq_ref, mounts=mounts, ports=[cfg.mq_port])
-
-
-def flower_container(cfg):
-    name = cfg.containers["flower"]
-    mq = cfg.containers["mq"]
-    env = {
-        "CELERY_BROKEN_URL": f"redis://{mq}//",
-        "CELERY_RESULT_BACKEND": f"redis://{mq}/0",
-        "FLOWER_PORT": cfg.flower_port,
-    }
-    return constellation.ConstellationContainer(name, cfg.flower_ref, ports=[cfg.flower_port], environment=env)
-
-
-def task_queue_container(cfg):
-    name = cfg.containers["task_queue"]
-    mounts = [
-        constellation.ConstellationMount("burden_estimates", "/home/worker/burden_estimate_files"),
-    ]
-    return constellation.ConstellationContainer(name, cfg.task_queue_ref, configure=task_queue_configure, mounts=mounts)
-
-
-def task_queue_configure(container, cfg):
-    print("[task-queue] Configuring task-queue container")
-    task_queue_config = {"host": cfg.containers["mq"], "servers": cfg.task_queue_servers, "tasks": cfg.task_queue_tasks}
-    task_queue_config["servers"]["montagu"]["url"] = f"http://{cfg.containers['api']}:8080"
-    if cfg.fake_smtp_ref:
-        task_queue_config["servers"]["smtp"]["host"] = cfg.containers["fake_smtp"]
-        task_queue_config["servers"]["smtp"]["port"] = 1025
-    reports_cfg_filename = join(cfg.path, "diagnostic-reports.yml")
-    with open(reports_cfg_filename) as ymlfile:
-        diag_reports = yaml.safe_load(ymlfile)
-    task_queue_config["tasks"]["diagnostic_reports"]["reports"] = diag_reports
-    docker_util.string_into_container(yaml.dump(task_queue_config), container, "home/worker/config/config.yml")
-
-
-def fake_smtp_container(cfg):
-    name = cfg.containers["fake_smtp"]
-    return constellation.ConstellationContainer(name, cfg.fake_smtp_ref, ports=[1025, 1080])
-
-
 def db_container(cfg):
     name = cfg.containers["db"]
     mounts = [constellation.ConstellationMount("db", "/pgdata")]
     return constellation.ConstellationContainer(name, cfg.db_ref, mounts=mounts, ports=[5432], configure=db_configure)
 
 
 def db_configure(container, cfg):
@@ -245,7 +199,46 @@
         docker_util.exec_safely(container, ["self-signed-certificate", ssl_path])
     else:
         print("[proxy] Copying ssl certificate and key into proxy")
         docker_util.exec_safely(container, f"mkdir -p {ssl_path}")
         docker_util.string_into_container(cfg.ssl_certificate, container, join(ssl_path, "certificate.pem"))
         docker_util.string_into_container(cfg.ssl_key, container, join(ssl_path, "ssl_key.pem"))
         docker_util.string_into_container(cfg.dhparam, container, join(ssl_path, "dhparam.pem"))
+
+
+def start_proxy_metrics(cfg):
+    name = "{}-{}".format(cfg.container_prefix, cfg.containers["metrics"])
+    proxy_name = cfg.containers["proxy"]
+    image = str(cfg.proxy_metrics_ref)
+    print("Starting {} ({})".format(cfg.containers["metrics"], image))
+    docker.from_env().containers.run(
+        image,
+        restart_policy={"Name": "always"},
+        ports={"9113/tcp": 9113},
+        command=f'-nginx.scrape-uri "http://{proxy_name}/basic_status"',
+        network=cfg.network,
+        name=name,
+        detach=True,
+    )
+
+
+def stop_proxy_metrics(cfg):
+    name = "{}-{}".format(cfg.container_prefix, cfg.containers["metrics"])
+    container = get_container(name)
+    if container:
+        print(f"Killing '{name}'")
+        container.remove(force=True)
+
+
+def status_proxy_metrics(cfg):
+    name = "{}-{}".format(cfg.container_prefix, cfg.containers["metrics"])
+    container = get_container(name)
+    status = container.status if container else "missing"
+    print("    - {} ({}): {}".format(cfg.containers["metrics"], name, status))
+
+
+def get_container(name):
+    client = docker.client.from_env()
+    try:
+        return client.containers.get(name)
+    except docker.errors.NotFound:
+        return None
```

### Comparing `montagu_deploy-0.0.2/tests/test_cli.py` & `montagu_deploy-0.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `montagu_deploy-0.0.2/tests/test_config.py` & `montagu_deploy-0.0.3/tests/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,44 +9,35 @@
     assert cfg.volumes["db"] == "db_volume"
     assert cfg.volumes["emails"] == "emails"
     assert cfg.volumes["burden_estimates"] == "burden_estimate_files"
     assert cfg.volumes["guidance"] == "guidance_volume"
     assert cfg.volumes["templates"] == "template_volume"
     assert cfg.volumes["static"] == "static_volume"
     assert cfg.volumes["static_logs"] == "static_logs"
-    assert cfg.volumes["mq"] == "mq"
     assert cfg.container_prefix == "montagu"
 
-    assert len(cfg.containers) == 10
+    assert len(cfg.containers) == 7
     assert cfg.containers["api"] == "api"
     assert cfg.containers["db"] == "db"
     assert cfg.containers["admin"] == "admin"
     assert cfg.containers["contrib"] == "contrib"
     assert cfg.containers["static"] == "static"
     assert cfg.containers["proxy"] == "proxy"
-    assert cfg.containers["mq"] == "mq"
-    assert cfg.containers["flower"] == "flower"
-    assert cfg.containers["task_queue"] == "task-queue"
-
-    assert len(cfg.images) == 12
+    assert cfg.containers["metrics"] == "proxy-metrics"
 
+    assert len(cfg.images) == 8
     assert str(cfg.images["db"]) == "vimc/montagu-db:master"
     assert str(cfg.images["api"]) == "vimc/montagu-api:master"
     assert str(cfg.images["admin"]) == "vimc/montagu-admin-portal:master"
     assert str(cfg.images["contrib"]) == "vimc/montagu-contrib-portal:master"
     assert str(cfg.images["static"]) == "vimc/montagu-static:master"
     assert str(cfg.images["proxy"]) == "vimc/montagu-reverse-proxy:vimc-7152"
-    assert str(cfg.images["mq"]) == "docker.io/redis:latest"
-    assert str(cfg.images["flower"]) == "mher/flower:0.9.5"
-    assert str(cfg.images["task_queue"]) == "vimc/task-queue-worker:master"
+    assert str(cfg.images["metrics"]) == "nginx/nginx-prometheus-exporter:0.10.0"
     assert str(cfg.images["db_migrate"]) == "vimc/montagu-migrate:master"
 
-    assert cfg.mq_port == 6379
-    assert cfg.flower_port == 5555
-
     assert cfg.protect_data is False
     assert cfg.proxy_ssl_self_signed is True
 
     assert cfg.db_root_user == "vimc"
     assert len(cfg.db_root_password) == 50
     assert cfg.db_users == {
         "api": {"password": "apipassword", "permissions": "all"},
```

### Comparing `montagu_deploy-0.0.2/tests/test_constellation.py` & `montagu_deploy-0.0.3/tests/test_constellation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,40 @@
+import ssl
+import time
+import urllib
+
 import docker
 from constellation import docker_util
 
 from src.montagu_deploy.config import MontaguConfig
 from src.montagu_deploy.montagu_constellation import MontaguConstellation
-from tests.utils import http_get
 
 
 def test_start_and_stop():
     cfg = MontaguConfig("config/basic")
     obj = MontaguConstellation(cfg)
 
     obj.start()
 
     cl = docker.client.from_env()
+    containers = cl.containers.list()
+    assert len(containers) == 7
 
     assert docker_util.network_exists(cfg.network)
     assert docker_util.volume_exists(cfg.volumes["db"])
     assert docker_util.volume_exists(cfg.volumes["burden_estimates"])
-    assert docker_util.volume_exists(cfg.volumes["emails"])
-    assert docker_util.volume_exists(cfg.volumes["static"])
-    assert docker_util.volume_exists(cfg.volumes["static_logs"])
-    assert docker_util.volume_exists(cfg.volumes["mq"])
-    assert docker_util.volume_exists(cfg.volumes["templates"])
-    assert docker_util.volume_exists(cfg.volumes["guidance"])
 
     assert docker_util.container_exists("montagu-api")
     assert docker_util.container_exists("montagu-db")
     assert docker_util.container_exists("montagu-proxy")
+    assert docker_util.container_exists("montagu-proxy-metrics")
     assert docker_util.container_exists("montagu-admin")
     assert docker_util.container_exists("montagu-contrib")
-    assert docker_util.container_exists("montagu-static")
-    assert docker_util.container_exists("montagu-mq")
-    assert docker_util.container_exists("montagu-flower")
-    assert docker_util.container_exists("montagu-task-queue")
-    assert docker_util.container_exists("montagu-fake-smtp")
-
-    containers = cl.containers.list()
-    print([c.name for c in containers])
-    print(get_container(cfg, "task_queue").logs())
-    assert len(containers) == 10
 
-    obj.stop(kill=True, remove_volumes=True)
+    obj.stop(kill=True)
 
 
 def test_api_configured():
     cfg = MontaguConfig("config/basic")
     obj = MontaguConstellation(cfg)
 
     obj.start()
@@ -59,27 +49,27 @@
     assert "allow.localhost=False" in api_config
     assert "upload.dir=/upload_dir" in api_config
     assert "email.mode=real" not in api_config
 
     res = http_get("https://localhost/api/v1")
     assert '"status": "success"' in res
 
-    obj.stop(kill=True, remove_volumes=True)
+    obj.stop(kill=True)
 
     cfg = MontaguConfig("config/complete")
     obj = MontaguConstellation(cfg)
 
     obj.start()
     api = get_container(cfg, "api")
     api_config = docker_util.string_from_container(api, "/etc/montagu/api/config.properties").split("\n")
     assert "email.mode=real" in api_config
     assert "email.password=changeme" in api_config
     assert "flow.url=fakeurl" in api_config
 
-    obj.stop(kill=True, remove_volumes=True)
+    obj.stop(kill=True)
 
 
 def test_proxy_configured_self_signed():
     cfg = MontaguConfig("config/basic")
     obj = MontaguConstellation(cfg)
 
     obj.start()
@@ -91,15 +81,15 @@
     assert cert is not None
     assert key is not None
     assert param is not None
 
     res = http_get("https://localhost")
     assert "Montagu" in res
 
-    obj.stop(kill=True, remove_volumes=True)
+    obj.stop(kill=True)
 
 
 def test_db_configured():
     cfg = MontaguConfig("config/complete")
     obj = MontaguConstellation(cfg)
 
     obj.start()
@@ -113,15 +103,15 @@
 
     query = "SELECT * FROM pg_replication_slots WHERE slot_name = 'barman'"
     res = docker_util.exec_safely(db, f'psql -U {cfg.db_root_user} -d postgres -c "{query}"')
     res = res.output.decode("UTF-8")
 
     assert "barman" in res
 
-    obj.stop(kill=True, remove_volumes=True)
+    obj.stop(kill=True)
 
 
 def test_proxy_configured_ssl():
     cfg = MontaguConfig("config/complete")
     obj = MontaguConstellation(cfg)
 
     obj.start()
@@ -130,13 +120,40 @@
     cert = docker_util.string_from_container(api, "/etc/montagu/proxy/certificate.pem")
     key = docker_util.string_from_container(api, "/etc/montagu/proxy/ssl_key.pem")
     param = docker_util.string_from_container(api, "/etc/montagu/proxy/dhparam.pem")
     assert cert == "cert"
     assert key == "k3y"
     assert param == "param"
 
-    obj.stop(kill=True, remove_volumes=True)
+    obj.stop(kill=True)
+
+
+def test_metrics():
+    cfg = MontaguConfig("config/basic")
+    obj = MontaguConstellation(cfg)
+
+    obj.start()
+    http_get("http://localhost:9113/metrics")
+
+    obj.stop(kill=True)
 
 
 def get_container(cfg, name):
     cl = docker.client.from_env()
     return cl.containers.get(f"{cfg.container_prefix}-{cfg.containers[name]}")
+
+
+# Because we wait for a go signal to come up, we might not be able to
+# make the request right away:
+def http_get(url, retries=5, poll=0.5):
+    ctx = ssl.create_default_context()
+    ctx.check_hostname = False
+    ctx.verify_mode = ssl.CERT_NONE
+    for _i in range(retries):
+        try:
+            r = urllib.request.urlopen(url, context=ctx)  # noqa
+            return r.read().decode("UTF-8")
+        except (urllib.error.URLError, ConnectionResetError) as e:
+            print("sleeping...")
+            time.sleep(poll)
+            error = e
+    raise error
```

### Comparing `montagu_deploy-0.0.2/LICENSE.txt` & `montagu_deploy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `montagu_deploy-0.0.2/README.md` & `montagu_deploy-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -45,18 +45,14 @@
 ## Dev requirements
 
 1. [Python3](https://www.python.org/downloads/) (>= 3.7)
 2. [Hatch](https://hatch.pypa.io/latest/install/)
 
 ## Test and lint
 
-For all integration tests to pass, you will need 2 environment variables:
-1. `YOUTRACK_TOKEN` - a token for accessing the YT API
-2. `VAULT_TOKEN` - a github PAT for a user in the vimc robots team.
-
 1. `hatch run test`
 2. `hatch run lint:fmt`
 
 To get coverage reported locally in the console, use `hatch run cov`. 
 On CI, use `hatch run cov-ci` to generate an xml report.
 
 ## Build
```

### Comparing `montagu_deploy-0.0.2/pyproject.toml` & `montagu_deploy-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "constellation>=1.1.2",
+  "constellation>=1.0.3",
   "docopt",
   "psycopg2"
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/montagu-deploy#readme"
 Issues = "https://github.com/unknown/montagu-deploy/issues"
@@ -39,21 +39,16 @@
 montagu = "montagu_deploy.cli:main"
 
 [tool.hatch.version]
 path = "src/montagu_deploy/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
-  "celery",
   "coverage[toml]>=6.5",
-  "orderly_web",
-  "pytest",
-  "redis",
-  "vault_dev",
-  "YTClient"
+  "pytest"
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `montagu_deploy-0.0.2/PKG-INFO` & `montagu_deploy-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: montagu-deploy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Deploy tool for the Montagu web app
 Project-URL: Documentation, https://github.com/unknown/montagu-deploy#readme
 Project-URL: Issues, https://github.com/unknown/montagu-deploy/issues
 Project-URL: Source, https://github.com/unknown/montagu-deploy
 Author-email: Alex <alex.hill@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: constellation>=1.1.2
+Requires-Dist: constellation>=1.0.3
 Requires-Dist: docopt
 Requires-Dist: psycopg2
 Description-Content-Type: text/markdown
 
 # montagu-deploy
 
 [![PyPI - Version](https://img.shields.io/pypi/v/montagu-deploy.svg)](https://pypi.org/project/montagu-deploy)
@@ -70,18 +70,14 @@
 ## Dev requirements
 
 1. [Python3](https://www.python.org/downloads/) (>= 3.7)
 2. [Hatch](https://hatch.pypa.io/latest/install/)
 
 ## Test and lint
 
-For all integration tests to pass, you will need 2 environment variables:
-1. `YOUTRACK_TOKEN` - a token for accessing the YT API
-2. `VAULT_TOKEN` - a github PAT for a user in the vimc robots team.
-
 1. `hatch run test`
 2. `hatch run lint:fmt`
 
 To get coverage reported locally in the console, use `hatch run cov`. 
 On CI, use `hatch run cov-ci` to generate an xml report.
 
 ## Build
```

