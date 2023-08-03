# Comparing `tmp/qctrl_client-7.2.2.tar.gz` & `tmp/qctrl_client-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_client-7.2.2.tar", max compression
+gzip compressed data, was "qctrl_client-8.0.0.tar", max compression
```

## Comparing `qctrl_client-7.2.2.tar` & `qctrl_client-8.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    36653 2023-07-31 05:53:32.003609 qctrl_client-7.2.2/LICENSE
--rw-r--r--   0        0        0      214 2023-07-31 05:53:32.003609 qctrl_client-7.2.2/README.md
--rw-r--r--   0        0        0     2614 2023-07-31 05:53:55.327645 qctrl_client-7.2.2/pyproject.toml
--rw-r--r--   0        0        0      747 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/__init__.py
--rw-r--r--   0        0        0      686 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/auth/__init__.py
--rw-r--r--   0        0        0     1831 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/auth/base.py
--rw-r--r--   0        0        0     4969 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/auth/cli.py
--rw-r--r--   0        0        0      972 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/auth/helpers.py
--rw-r--r--   0        0        0     1042 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/auth/keycloak.py
--rw-r--r--   0        0        0     4316 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/auth/oidc.py
--rw-r--r--   0        0        0     1801 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/auth/password.py
--rw-r--r--   0        0        0     3096 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/auth/redirect_listener.py
--rw-r--r--   0        0        0     1516 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/auth/service_account.py
--rw-r--r--   0        0        0     7742 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/client.py
--rw-r--r--   0        0        0      809 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/core/__init__.py
--rw-r--r--   0        0        0     2999 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/core/functions.py
--rw-r--r--   0        0        0      995 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/core/products.py
--rw-r--r--   0        0        0      638 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/core/router/__init__.py
--rw-r--r--   0        0        0    12547 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/core/router/api.py
--rw-r--r--   0        0        0     1189 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/core/router/base.py
--rw-r--r--   0        0        0     1197 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/core/router/local.py
--rw-r--r--   0        0        0     2677 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/core/settings.py
--rw-r--r--   0        0        0     1179 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/core/utils.py
--rw-r--r--   0        0        0     1329 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/defaults.py
--rw-r--r--   0        0        0     2172 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/exceptions.py
--rw-r--r--   0        0        0     1357 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/globals.py
--rw-r--r--   0        0        0     1424 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/pytest_plugin.py
--rw-r--r--   0        0        0      601 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/transports/__init__.py
--rw-r--r--   0        0        0     4625 2023-07-31 05:53:32.007609 qctrl_client-7.2.2/qctrlclient/transports/requests_transport.py
--rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 qctrl_client-7.2.2/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/LICENSE
+-rw-r--r--   0        0        0      214 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/README.md
+-rw-r--r--   0        0        0     2614 2023-08-03 02:28:10.068607 qctrl_client-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0      747 2023-08-03 02:28:10.080607 qctrl_client-8.0.0/qctrlclient/__init__.py
+-rw-r--r--   0        0        0      686 2023-08-03 02:28:10.076607 qctrl_client-8.0.0/qctrlclient/auth/__init__.py
+-rw-r--r--   0        0        0     1831 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/auth/base.py
+-rw-r--r--   0        0        0     4969 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/auth/cli.py
+-rw-r--r--   0        0        0      972 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/auth/helpers.py
+-rw-r--r--   0        0        0     1042 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/auth/keycloak.py
+-rw-r--r--   0        0        0     4316 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/auth/oidc.py
+-rw-r--r--   0        0        0     1801 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/auth/password.py
+-rw-r--r--   0        0        0     3096 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/auth/redirect_listener.py
+-rw-r--r--   0        0        0     1516 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/auth/service_account.py
+-rw-r--r--   0        0        0     7742 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/client.py
+-rw-r--r--   0        0        0      786 2023-08-03 02:28:10.076607 qctrl_client-8.0.0/qctrlclient/core/__init__.py
+-rw-r--r--   0        0        0     2633 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/core/functions.py
+-rw-r--r--   0        0        0      995 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/core/products.py
+-rw-r--r--   0        0        0      638 2023-08-03 02:28:10.072607 qctrl_client-8.0.0/qctrlclient/core/router/__init__.py
+-rw-r--r--   0        0        0    13607 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/core/router/api.py
+-rw-r--r--   0        0        0     1189 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/core/router/base.py
+-rw-r--r--   0        0        0     1197 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/core/router/local.py
+-rw-r--r--   0        0        0     2677 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/core/settings.py
+-rw-r--r--   0        0        0     1179 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/core/utils.py
+-rw-r--r--   0        0        0     1329 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/defaults.py
+-rw-r--r--   0        0        0     2172 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/exceptions.py
+-rw-r--r--   0        0        0     1357 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/globals.py
+-rw-r--r--   0        0        0     1424 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/pytest_plugin.py
+-rw-r--r--   0        0        0      601 2023-08-03 02:28:10.080607 qctrl_client-8.0.0/qctrlclient/transports/__init__.py
+-rw-r--r--   0        0        0     4625 2023-08-03 02:27:51.076168 qctrl_client-8.0.0/qctrlclient/transports/requests_transport.py
+-rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 qctrl_client-8.0.0/PKG-INFO
```

### Comparing `qctrl_client-7.2.2/LICENSE` & `qctrl_client-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/pyproject.toml` & `qctrl_client-8.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-client"
-version = "7.2.2"
+version = "8.0.0"
 description = "Q-CTRL Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
```

### Comparing `qctrl_client-7.2.2/qctrlclient/__init__.py` & `qctrl_client-8.0.0/qctrlclient/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/auth/__init__.py` & `qctrl_client-8.0.0/qctrlclient/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/auth/base.py` & `qctrl_client-8.0.0/qctrlclient/auth/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/auth/cli.py` & `qctrl_client-8.0.0/qctrlclient/auth/cli.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/auth/helpers.py` & `qctrl_client-8.0.0/qctrlclient/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/auth/keycloak.py` & `qctrl_client-8.0.0/qctrlclient/auth/keycloak.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/auth/oidc.py` & `qctrl_client-8.0.0/qctrlclient/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/auth/password.py` & `qctrl_client-8.0.0/qctrlclient/auth/password.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/auth/redirect_listener.py` & `qctrl_client-8.0.0/qctrlclient/auth/redirect_listener.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/auth/service_account.py` & `qctrl_client-8.0.0/qctrlclient/auth/service_account.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/client.py` & `qctrl_client-8.0.0/qctrlclient/client.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/core/__init__.py` & `qctrl_client-8.0.0/qctrlclient/core/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 from .functions import (
     core_workflow,
     print_warnings,
-    run_core_workflow,
 )
 from .products import (
     Product,
     ProductInfo,
 )
 from .router import (
     ApiRouter,
```

### Comparing `qctrl_client-7.2.2/qctrlclient/core/functions.py` & `qctrl_client-8.0.0/qctrlclient/core/functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,33 +17,14 @@
     Callable,
     Dict,
     Optional,
 )
 from warnings import warn
 
 
-def run_core_workflow(get_config: Callable, workflow: str, data: Any):
-    """Runs the core workflow using the configured router.
-
-    Parameters
-    ----------
-    get_config : Callable
-        Returns a `CoreClientSettings` instance. The configured
-        router will be used to execute the workflow.
-    workflow : str
-        The registered name of the workflow to be executed.
-    data : Any
-        The required input data for the workflow.
-    """
-    config = get_config()
-    router = config.get_router()
-    result = router(workflow, data)
-    return result
-
-
 def core_workflow(
     get_config: Callable, workflow: str, formatter: Optional[Callable] = None
 ):
     """Decorator for a function which will execute a workflow.
     The decorated function should return the data to be used
     during workflow execution. When being used in a client
     package, it is recommended to use a partial to provide
@@ -70,16 +51,22 @@
         which is the raw result fo the workflow. If used, the
         decorated function will return the result of this callable.
     """
 
     def decorator(func: Callable):
         @wraps(func)
         def customized_decorator(*args, **kwargs):
+
+            # router is instantiated before function is called
+            # so any alteration to settings is visible within
+            # the function
+            config = get_config()
+            router = config.get_router()
             data = func(*args, **kwargs)
-            result = run_core_workflow(get_config, workflow, data)
+            result = router(workflow, data)
 
             if formatter:
                 result = formatter(result)
 
             return result
 
         return customized_decorator
```

### Comparing `qctrl_client-7.2.2/qctrlclient/core/products.py` & `qctrl_client-8.0.0/qctrlclient/core/products.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/core/router/__init__.py` & `qctrl_client-8.0.0/qctrlclient/core/router/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/core/router/api.py` & `qctrl_client-8.0.0/qctrlclient/core/router/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -166,80 +166,62 @@
 
     def _validate(self):
         """Performs validation checks on the settings."""
 
         if not self._settings.product:
             raise GraphQLClientError("`product` must be configured in settings")
 
-        self._check_has_organizations()
-        self._check_must_set_organization()
-        self._check_organization_permission()
+        self._check_organization_config()
 
-    def _check_must_set_organization(self):
-        if self._settings.organization:
-            return
-
-        if len(self._organizations) > 1:
-            error_message = "You are assigned to multiple organizations. "
-            error_message += "Please configure an organization:\n\n"
-
-            for organization in self._organizations:
-                error_message += f"- {organization.slug}\n"
-
-            show_error_message(error_message)
-
-    def _check_has_organizations(self):
-        # if no organizations found
-        if not self._organizations:
-            show_error_message("No organizations found")
+    def _check_organization_config(self):
+        """Validates the `organization` configuration. After this
+        function finishes, the following will be true:
+
+        - The slug of the organization that the workflow will run
+          under will be configured in `settings.organization`.
+        - The user is a member of the configured organization.
 
-    def _check_organization_permission(self):
-        """Checks that the user is assigned to the configured
-        organization. Requires that the `organization` setting
-        is configured.
-
-        Parameters
-        ----------
-        organizations : List[Organization]
-            List of organizations that the user is assigned to which provide
-            access to the corresponding product.
-        """
-
-        assigned = False
-
-        if not self._settings.organization:
-            return
-
-        for organization in self._organizations:
-            if organization.slug == self._settings.organization:
-                assigned = True
-                break
-
-        if not assigned:
-            show_error_message(
-                f"Configured organization not found: `{self._settings.organization}`"
-            )
-
-    @property
-    def _organization(self) -> Organization:
-        """Returns the organization that the user is assigned to
-        which provides access to the configured product.
+        If the above rules cannot be guaranteed, an error message
+        will be displayed.
         """
 
+        # organization configured by user
         if self._settings.organization:
+            found = False
+
             for organization in self._organizations:
                 if organization.slug == self._settings.organization:
-                    return organization
+                    found = True
+                    break
 
-        if len(self._organizations) == 1:
-            return self._organizations[0]
+            if not found:
+                show_error_message(
+                    f"Configured organization not found: `{self._settings.organization}`"
+                )
 
-        raise GraphQLClientError(
-            f"Configured organization not found: `{self._settings.organization}`"
-        )
+        # organization not configured by user
+        else:
+
+            # user is not a member of any organization
+            if not self._organizations:
+                show_error_message("No organizations found")
+
+            # user is a member of multiple organizations
+            elif len(self._organizations) > 1:
+                error_message = "You are assigned to multiple organizations. "
+                error_message += "Please configure an organization:\n\n"
+
+                for organization in self._organizations:
+                    error_message += f"- {organization.slug}\n"
+
+                show_error_message(error_message)
+
+            # user is a member of one organization
+            else:
+                self._settings.organization = self._organizations[0].slug
 
     @cached_property
     def _organizations(self) -> List[Organization]:
         """Returns the list of organizations that the user is
         assigned to which provide access to the configured product.
         """
 
@@ -358,18 +340,28 @@
         package_versions = {}
 
         for package in self._TRACKED_PACKAGES:
             package_versions[package] = get_installed_version(package)
 
         return {
             "package_versions": package_versions,
-            "organization_slug": self._organization.slug,
-            "organization": self._organization.to_dict(),
+            "organization_slug": self._settings.organization,
+            "organization": self._get_configured_organization().to_dict(),
         }
 
+    def _get_configured_organization(self) -> Organization:
+        """Returns the corresponding `Organization` object for
+        the `organization` configured in settings.
+        """
+        for organization in self._organizations:
+            if organization.slug == self._settings.organization:
+                return organization
+
+        raise RuntimeError(f"Organization not found: {self._settings.organization}")
+
     @staticmethod
     def _handle_warnings(warnings_data: List[Dict[str, Any]]):
         """Handles warnings returned when starting a workflow."""
 
         for warning_data in warnings_data:
             message = warning_data["message"]
             warn(Warning(message))
@@ -413,16 +405,50 @@
         """Returns the result of the action. If the action
         has not finished, the API will be polled until it has.
         If the action has failed, a `RuntimeError` will be
         raised.
         """
 
         if not action.is_finished():
-            action = self._poll_for_completion(action)
+            try:
+                action = self._poll_for_completion(action)
+            except KeyboardInterrupt:
+                self._revoke_action(action)
+                action = self._poll_for_completion(action)
 
         if action.is_failed():
             raise RuntimeError(action.errors)
 
         if action.is_revoked():
-            raise RuntimeError("The action was cancelled")
+            raise RuntimeError(
+                f'Your task (action_id="{action.action_id}") has been cancelled.'
+            )
 
         return action.result
+
+    def _revoke_action(self, action: Action) -> Action:
+        """
+        Updates the status of the Action to REVOKED.
+        """
+
+        _query = gql.gql(
+            """
+            mutation updateActionMutation($modelId: String!, $status: ActionStatusEnum ) {
+                updateAction(input: {modelId: $modelId , status: $status}) {
+                    action {
+                        modelId
+                        status
+                        name
+                        progress
+                    }
+                    errors {
+                        fields
+                        message
+                    }
+                }
+            }
+        """
+        )
+
+        self._client.execute(
+            _query, {"modelId": action.action_id, "status": ActionStatus.REVOKED.value}
+        )
```

### Comparing `qctrl_client-7.2.2/qctrlclient/core/router/base.py` & `qctrl_client-8.0.0/qctrlclient/core/router/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/core/router/local.py` & `qctrl_client-8.0.0/qctrlclient/core/router/local.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/core/settings.py` & `qctrl_client-8.0.0/qctrlclient/core/settings.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/core/utils.py` & `qctrl_client-8.0.0/qctrlclient/core/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/defaults.py` & `qctrl_client-8.0.0/qctrlclient/defaults.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/exceptions.py` & `qctrl_client-8.0.0/qctrlclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/globals.py` & `qctrl_client-8.0.0/qctrlclient/globals.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/pytest_plugin.py` & `qctrl_client-8.0.0/qctrlclient/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/transports/__init__.py` & `qctrl_client-8.0.0/qctrlclient/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/qctrlclient/transports/requests_transport.py` & `qctrl_client-8.0.0/qctrlclient/transports/requests_transport.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.2/PKG-INFO` & `qctrl_client-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-client
-Version: 7.2.2
+Version: 8.0.0
 Summary: Q-CTRL Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

