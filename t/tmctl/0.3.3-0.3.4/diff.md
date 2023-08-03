# Comparing `tmp/tmctl-0.3.3.tar.gz` & `tmp/tmctl-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmctl-0.3.3.tar", last modified: Thu Jul 20 05:20:04 2023, max compression
+gzip compressed data, was "tmctl-0.3.4.tar", last modified: Thu Aug  3 09:03:49 2023, max compression
```

## Comparing `tmctl-0.3.3.tar` & `tmctl-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:20:04.792816 tmctl-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 05:20:04.792816 tmctl-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 05:20:04.792816 tmctl-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-20 05:19:54.000000 tmctl-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:20:04.788816 tmctl-0.3.3/tmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-20 05:19:54.000000 tmctl-0.3.3/tmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35341 2023-07-20 05:19:54.000000 tmctl-0.3.3/tmctl/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-20 05:19:54.000000 tmctl-0.3.3/tmctl/tmctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:20:04.788816 tmctl-0.3.3/tmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 05:20:04.000000 tmctl-0.3.3/tmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-20 05:20:04.000000 tmctl-0.3.3/tmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 05:20:04.000000 tmctl-0.3.3/tmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 05:20:04.000000 tmctl-0.3.3/tmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 05:20:04.000000 tmctl-0.3.3/tmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 05:20:04.000000 tmctl-0.3.3/tmctl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:49.710645 tmctl-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 09:03:49.710645 tmctl-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 09:03:49.710645 tmctl-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-03 09:03:38.000000 tmctl-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:49.710645 tmctl-0.3.4/tmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 09:03:38.000000 tmctl-0.3.4/tmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35575 2023-08-03 09:03:38.000000 tmctl-0.3.4/tmctl/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-08-03 09:03:38.000000 tmctl-0.3.4/tmctl/tmctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:49.710645 tmctl-0.3.4/tmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 09:03:49.000000 tmctl-0.3.4/tmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-03 09:03:49.000000 tmctl-0.3.4/tmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:03:49.000000 tmctl-0.3.4/tmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-03 09:03:49.000000 tmctl-0.3.4/tmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 09:03:49.000000 tmctl-0.3.4/tmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 09:03:49.000000 tmctl-0.3.4/tmctl.egg-info/top_level.txt
```

### Comparing `tmctl-0.3.3/tmctl/controller.py` & `tmctl-0.3.4/tmctl/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import requests
 import yaml
 
 
 @dataclass
 class CommonOption:
     admin_url: str
+    session: requests.Session = None
     output: str = "json"
     indent: int = 4
     username: str = None
     password: str = None
 
 
 @dataclass
@@ -26,40 +27,22 @@
 
 
 class AdminClient(object):
     def __init__(
         self,
         common_option: CommonOption,
         base_url: str = None,
-        session: requests.session = None,
     ):
         self._common_option = common_option
         self._admin_url = self._common_option.admin_url
         self._output = self._common_option.output
         self._indent = self._common_option.indent
 
         self._base_url = base_url
-        self._session = session or requests.session()
-        self._try_login()
-
-    def _try_login(self) -> None:
-        try:
-            response = self._session.post(
-                f"{self._admin_url}/v1/auth/login",
-                data={
-                    "username": self._common_option.username,
-                    "password": self._common_option.password,
-                },
-            )
-
-            if response.status_code in [401, 422]:
-                raise Exception("Invalid username or password")
-        except Exception as e:
-            logging.warning(e)
-            exit(1)
+        self._session = common_option.session or requests.session()
 
     def _response_to_object(self, response: dict) -> CommonResponse:
         return CommonResponse(
             status=response.get("status", None) or None,
             message=response.get("message", None) or {},
             data=response.get("data", None) or {},
         )
@@ -151,18 +134,20 @@
         if response.ok:
             return response.content
         else:
             message = response.json()["message"]
             print(f"[ERROR] reason : {message}")
             exit(1)
 
-    def _send_post(self, url, json_data: dict = None, form_data: dict = None):
+    def _send_post(
+        self, url, json_data: dict = None, form_data: dict = None, params: dict = None
+    ):
         json_data = json_data or {}
         response = self._session.post(
-            self._admin_url + url, data=form_data, json=json_data
+            self._admin_url + url, data=form_data, json=json_data, params=params
         )
 
         if response.ok:
             return self._response_to_object(response.json())
         else:
             message = response.json()["message"]
             print(f"[ERROR] reason : {message}")
@@ -463,45 +448,45 @@
     usage:
         ex) tmctl <group> <command> <yaml file>
         ex) tmctl cluster <ls(list), rm(delete), submit get> <manual.yaml>
         ex) tmctl cluster ls
         ex) tmctl cluster submit test.yaml
     """
 
-    def __init__(self, url):
-        super(Cluster, self).__init__(url, "/v1/clusters")
+    def __init__(self, common_option: CommonOption):
+        super(Cluster, self).__init__(common_option, "/v1/clusters")
 
     def add_catalog(self, cluster_name, catalog_name, direct_on=False):
-        response = self._send_get("/v1/client/clusters", params={"name": cluster_name})
+        response = self._send_get("/v2/client/clusters", params={"name": cluster_name})
         cluster = response.data[0]
 
         response = self._send_get("/v1/catalogs", params={"name": catalog_name})
         catalog = response.data[0]
 
         cluster["catalog_list"].append(catalog["id"])
 
         response = self._send_put(
-            "/v1/client/clusters",
+            "/v2/client/clusters",
             json_data=cluster,
             params={"name": cluster_name, "direct_on": direct_on},
         )
         self._print(response.data)
 
     def remove_catalog(self, cluster_name, catalog_name, direct_on=False):
-        response = self._send_get("/v1/client/clusters", params={"name": cluster_name})
+        response = self._send_get("/v2/client/clusters", params={"name": cluster_name})
         cluster = response.data[0]
 
         response = self._send_get("/v1/catalogs", params={"name": catalog_name})
         catalog = response.data[0]
 
         if catalog["id"] in cluster["catalog_list"]:
             cluster["catalog_list"].remove(catalog["id"])
 
         response = self._send_put(
-            "/v1/client/clusters",
+            "/v2/client/clusters",
             json_data=cluster,
             params={"name": cluster_name, "direct_on": direct_on},
         )
         self._print(response.data)
 
     def rm_catalog(self, cluster_name, catalog_name, direct_on=False):
         return self.remove_catalog(
@@ -511,40 +496,41 @@
     def create(self, name, **kwargs):
         """
         cluster create command\n
         e.g) tmctl cluster create cluster_name
         e.g) tmctl cluster create cluster_name -direct_on=False
         """
         parameters = {**{"name": name, "direct_on": True}, **kwargs}
-        response = self._send_post("/v1/client/clusters", parameters)
+        response = self._send_post("/v2/client/clusters", parameters)
         self._print(response.data)
 
-    def delete(self, name, force=False, refresh=1, timeout=120):
+    def delete(self, name, force=False):
         """
         cluster delete(rm) command\n
         """
-        response = self._send_get("/v1/clusters", {"name": name})
+        response = self._send_get("/v2/client/clusters", {"name": name})
 
         clusters = response.data
 
         if clusters:
             cluster = clusters[0]
             health_check = self._health_check_status(cluster["id"]).data
 
             if health_check:
                 if force:
-                    self.off(name=name, refresh=refresh, timeout=timeout)
+                    self._send_delete(
+                        f"""/v2/client/clusters/{cluster["id"]}""",
+                        params={"force_remove": True},
+                    )
                 else:
                     print("Cluster is on. please off the cluster first.")
                     logging.warning("Cluster is on. please off the cluster first.")
                     exit(1)
 
-        response = self._send_delete(
-            "/v1/client/clusters", {"name": name, "force_remove": force}
-        )
+        response = self._send_delete(f"""/v2/client/clusters/{cluster["id"]}""")
         self._print(response.data)
 
     def _health_check_status(self, cluster_id):
         response = self._send_health_check_status_get(
             f"/v1/clusters/{cluster_id}/gateway/health"
         )
         return response
@@ -657,15 +643,15 @@
         """
         self.list()
 
     def get(self, name):
         """
         cluster info(ON/OFF) get\n
         """
-        response = self._send_get("/v1/clusters", {"name": name})
+        response = self._send_get("/v2/client/clusters", {"name": name})
 
         clusters = response.data
 
         if clusters:
             cluster = clusters[0]
 
             cluster["status"] = (
@@ -676,15 +662,15 @@
 
     def status(self, name, refresh=1, timeout=120):
         """
         cluster status get\n
         """
         cluster = None
 
-        response = self._send_get("/v1/clusters", params={"name": name})
+        response = self._send_get("/v2/client/clusters", params={"name": name})
 
         clusters = response.data
 
         if clusters:
             cluster = clusters[0]
 
         if not cluster:
@@ -733,18 +719,17 @@
         for each in yamls:
             version = each.get("version", None)
             action_type = each.get("type", None)
 
             if version in ["v1/cluster"]:
                 cluster_config = each.get("cluster", None) or {}
                 name = cluster_config.get("name", None)
-
                 direct_on = cluster_config.get("direct_on", True)
-
                 chart_name = cluster_config.get("chart", None)
+                cluster_view_data = cluster_config.get("cluster_view_data", None) or {}
 
                 params = {"name": chart_name}
 
                 response = self._send_get("/v1/charts", params=params)
 
                 chart_id = None
                 charts = response.data
@@ -786,97 +771,111 @@
 
                 if not chart_id:
                     print("invalid chart id or chart_name", chart_id, chart_name)
                     exit(1)
 
                 if action_type == "create":
                     response = self._send_post(
-                        "/v1/clusters",
+                        "/v2/client/clusters",
                         json_data={
                             "name": name,
                             "chart_id": chart_id,
                             "catalog_list": catalog_list,
                             "file_list": file_list,
                             "settings": settings,
+                            "cluster_view_data": cluster_view_data,
                         },
+                        params={"direct_on": direct_on},
                     )
 
                     clusters = response.data
 
                     if clusters:
-                        cluster = clusters[0]
-                        self._print(cluster)
-                        if direct_on:
-                            self.on(cluster_id=cluster["id"], is_update=False)
+                        self._print(clusters)
 
                 elif action_type == "update":
                     cluster_id = cluster_config.get("id", None)
 
                     if cluster_id:
-                        response = self._send_post(
-                            f"/v1/clusters/{cluster_id}",
+                        response = self._send_put(
+                            f"/v2/client/clusters/{cluster_id}",
                             json_data={
                                 "name": name,
                                 "chart_id": chart_id,
                                 "catalog_list": catalog_list,
                                 "file_list": file_list,
                                 "settings": settings,
+                                "cluster_view_data": cluster_view_data,
                             },
+                            params={"direct_on": direct_on},
                         )
 
                         clusters = response.data
 
                         if clusters:
-                            cluster = clusters[0]
-                            self._print(cluster)
-                            if direct_on:
-                                self.on(cluster_id=cluster_id, is_update=True)
+                            self._print(clusters)
                     else:
                         message = "cluster_id is None"
                         # logging.warning("cluster id is unknown.")
                         print(f"[ERROR] reason : {message}")
                         exit(1)
                 else:
                     message = "invalid action type"
                     print(f"[ERROR] reason : {message}")
                     exit(1)
 
     def on(self, name):
         """
         cluster on command
         """
-        response = self._send_put(f"/v1/client/clusters/{name}/on")
-        self._print(response.data)
+        response = self._send_get("/v2/client/clusters", {"name": name})
 
-        logging.info(response)
+        clusters = response.data
+
+        if clusters:
+            cluster = clusters[0]
+            response = self._send_put(f"""/v2/client/clusters/{cluster["id"]}/on""")
+            self._print(response.data)
+
+            logging.info(response)
+        else:
+            logging.info(f"Cannot find cluster name: {name}")
 
     def off(self, name):
         """
         cluster off command(not delete)
         """
-        response = self._send_put(f"/v1/client/clusters/{name}/off")
-        self._print(response.data)
+        response = self._send_get("/v2/client/clusters", {"name": name})
 
-        logging.info(response)
+        clusters = response.data
+
+        if clusters:
+            cluster = clusters[0]
+            response = self._send_put(f"""/v2/client/clusters/{cluster["id"]}/off""")
+            self._print(response.data)
+
+            logging.info(response)
+        else:
+            logging.info(f"Cannot find cluster name: {name}")
 
 
 class HelmChart(AdminClient):
     """
     helm_chart setting\n
     preparation file
         setting helm_chart yaml file
     usage:
         ex) tmctl <group> <command> <yaml file>
         ex) tmctl helm_chart <ls(list), rm(delete), submit get> <manual.yaml>
         ex) tmctl helm_chart ls
         ex) tmctl helm_chart submit test.yaml
     """
 
-    def __init__(self, url):
-        super(HelmChart, self).__init__(url, "/v1/charts")
+    def __init__(self, common_option: CommonOption):
+        super(HelmChart, self).__init__(common_option, "/v1/charts")
 
     def ls(self):
         """
         helm_chart list check\n
         """
         self.list()
 
@@ -960,16 +959,16 @@
     usage:
         ex) tmctl <group> <command> <yaml file>
         ex) tmctl mount <ls(list), rm(delete), submit get> <manual.yaml>
         ex) tmctl mount ls
         ex) tmctl mount submit test.yaml
     """
 
-    def __init__(self, url):
-        super(MountFile, self).__init__(url, "/v1/mounts")
+    def __init__(self, common_option: CommonOption):
+        super(MountFile, self).__init__(common_option, "/v1/mounts")
 
     def get(self, mount_path):
         """
         mount file info get\n
         """
         response = self._send_get(f"{self._base_url}", {"mount_path": mount_path})
         for each in response.data:
```

### Comparing `tmctl-0.3.3/tmctl/tmctl.py` & `tmctl-0.3.4/tmctl/tmctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,27 +35,28 @@
 
         admin_url = url or self._config["admin"]["url"]
         output = output or "json"
         indent = indent or 4
         username = username or self._config["admin"].get("username", None)
         password = password or self._config["admin"].get("password", None)
 
+        session = requests.session()
+        self._try_login(
+            session, admin_url=admin_url, username=username, password=password
+        )
+
         common_option = CommonOption(
             admin_url=admin_url,
+            session=session,
             output=output,
             indent=indent,
             username=username,
             password=password,
         )
 
-        session = requests.session()
-        self._try_login(
-            session, admin_url=admin_url, username=username, password=password
-        )
-
         self.catalog = Catalog(common_option)
         self.cluster = Cluster(common_option)
         self.helm_chart = HelmChart(common_option)
         self.file = File(common_option)
         self.mount = MountFile(common_option)
 
         log_config = self._config.get("logging", None) or {}
@@ -119,15 +120,15 @@
     ) -> None:
         try:
             response = session.post(
                 f"{admin_url}/v1/auth/login",
                 data={"username": username, "password": password},
             )
 
-            if response.status_code == 401:
+            if response.status_code in [401, 422]:
                 raise Exception("Invalid username or password")
             elif response.status_code == 404:
                 logging.warning("Server authentication is not enabled")
         except Exception as e:
             logging.warning(e)
             exit(1)
```

