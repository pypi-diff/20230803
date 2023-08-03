# Comparing `tmp/sotrans_fastapi_keycloak-0.0.7.tar.gz` & `tmp/sotrans_fastapi_keycloak-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotrans_fastapi_keycloak-0.0.7.tar", last modified: Tue Aug  1 12:29:19 2023, max compression
+gzip compressed data, was "sotrans_fastapi_keycloak-0.0.8.tar", last modified: Thu Aug  3 14:36:56 2023, max compression
```

## Comparing `sotrans_fastapi_keycloak-0.0.7.tar` & `sotrans_fastapi_keycloak-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 12:29:19.517334 sotrans_fastapi_keycloak-0.0.7/
--rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1122 2023-08-01 12:29:19.517334 sotrans_fastapi_keycloak-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.7/README.md
--rw-rw-rw-   0        0        0     1314 2023-08-01 12:29:11.000000 sotrans_fastapi_keycloak-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 12:29:19.517334 sotrans_fastapi_keycloak-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:29:19.498000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/
--rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/__init__.py
--rw-rw-rw-   0        0        0    47787 2023-08-01 12:28:40.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/api.py
--rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/exceptions.py
--rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/model.py
--rw-rw-rw-   0        0        0     2096 2023-08-01 12:28:40.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/sotrans_model.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:29:19.516025 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-08-01 12:29:19.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-08-01 12:29:19.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 12:29:19.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-08-01 12:29:19.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-08-01 12:29:19.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 14:36:56.189527 sotrans_fastapi_keycloak-0.0.8/
+-rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1122 2023-08-03 14:36:56.189527 sotrans_fastapi_keycloak-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1314 2023-08-03 14:36:55.000000 sotrans_fastapi_keycloak-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 14:36:56.189527 sotrans_fastapi_keycloak-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:36:56.157517 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/
+-rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/__init__.py
+-rw-rw-rw-   0        0        0    48510 2023-08-03 13:25:22.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/api.py
+-rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/exceptions.py
+-rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/model.py
+-rw-rw-rw-   0        0        0     1041 2023-08-03 14:04:55.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/role.py
+-rw-rw-rw-   0        0        0     2096 2023-08-01 12:28:40.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/sotrans_model.py
+-rw-rw-rw-   0        0        0      925 2023-08-03 14:04:55.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/sotrans_role.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:36:56.187397 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-08-03 14:36:56.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2023-08-03 14:36:56.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 14:36:56.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-08-03 14:36:56.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-03 14:36:56.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/top_level.txt
```

### Comparing `sotrans_fastapi_keycloak-0.0.7/LICENSE` & `sotrans_fastapi_keycloak-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.7/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans_fastapi_keycloak
-Version: 0.0.7
+Version: 0.0.8
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

### Comparing `sotrans_fastapi_keycloak-0.0.7/pyproject.toml` & `sotrans_fastapi_keycloak-0.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     "pydantic_core==2.4.0",
     "requests==2.31.0",
     "sniffio==1.3.0",
     "starlette==0.27.0",
     "typing_extensions==4.7.1",
     "urllib3==2.0.4"
 ]
-version = "0.0.7"
+version = "0.0.8"
```

### Comparing `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/__init__.py` & `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/api.py` & `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     KeycloakGroupModel,
     KeycloakIdentityProviderModel,
     KeycloakRoleModel,
     KeycloakTokenModel,
     KeycloakUserModel,
     OIDCUserModel,
 )
+from sotrans_fastapi_keycloak.role import Role
 
 
 def is_response_valid(response: Response) -> bool:
     """Check if response status code in valid range function
 
     :param response: response to check
     :return: whether response is valid or not
@@ -163,14 +164,15 @@
             realm: str,
             admin_client_secret: str,
             callback_uri: str,
             admin_client_id: str = "admin-cli",
             timeout: int = 10,
             user_type: type[BaseModel] = KeycloakUserModel,
             oidc_user_type: type[BaseModel] = OIDCUserModel,
+            roles: dict[str, Role] | None = None
     ):
         """FastAPIKeycloak constructor
 
         Args:
             server_url (str): The URL of the Keycloak server, with `/auth` suffix
             client_id (str): The id of the client used for users
             client_secret (str): The client secret
@@ -182,14 +184,16 @@
             timeout (int): Timeout in seconds to wait for the server
             user_type (type): UserModel type, which is used in user management methods
             oidc_user_type (type): OIDCUserModel type, which specifies schema for user info, get from token
         """
         self._user_model = user_type
         self._oidc_user_type = oidc_user_type
 
+        self.roles = roles or {}
+
         self.server_url = server_url
         self.realm = realm
         self.client_id = client_id
         self.client_secret = client_secret
         self.admin_client_id = admin_client_id
         self.admin_client_secret = admin_client_secret
         self.callback_uri = callback_uri
@@ -254,21 +258,21 @@
 
         Returns:
             OAuth2PasswordBearer: Auth scheme for swagger
         """
         return OAuth2PasswordBearer(tokenUrl = self.token_uri)
 
     def get_current_user(
-            self, required_roles: list[str] = None, extra_fields: list[str] = None
+            self, required_role_names: list[str] = None, extra_fields: list[str] = None
     ) -> Callable[[str], BaseModel]:
         """Returns the current user based on an access token in the HTTP-header. Optionally verifies roles are possessed
         by the user
 
         Args:
-            required_roles list[str]: list of role names required for this endpoint
+            required_role_names list[str]: list of role names required for this endpoint
             extra_fields list[str]: The names of the additional fields you need that are encoded in JWT
 
         Returns:
             Callable[[str], OIDCUser]: Dependency method which returns the decoded JWT content
 
         Raises:
             ExpiredSignatureError: If the token is expired (exp > datetime.now())
@@ -292,21 +296,17 @@
                 ExpiredSignatureError: If the token is expired (exp > datetime.now())
                 JWTError: If decoding fails or the signature is invalid
                 JWTClaimsError: If any claim is invalid
                 HTTPException: If any role required is not contained within the roles of the users
             """
             decoded_token = self._decode_token(token = token, audience = "account")
             user = self._oidc_user_type.model_validate(decoded_token)
-            if required_roles:
-                for role in required_roles:
-                    if role not in user.roles:
-                        raise HTTPException(
-                            status_code = status.HTTP_403_FORBIDDEN,
-                            detail = f'Role "{role}" is required to perform this action',
-                        )
+
+            if required_role_names:
+                self._assert_roles(user.roles, required_role_names)
 
             if extra_fields:
                 for field in extra_fields:
                     user.extra_fields[field] = decoded_token.get(field, None)
 
             return user
 
@@ -550,14 +550,29 @@
             KeycloakError: If the resulting response is not a successful HTTP-Code (>299)
         """
         return self._admin_request(
             url = f"{self.roles_uri}/{role_name}",
             method = HTTPMethod.DELETE,
         )
 
+    def _assert_roles(self, available_role_names: list[str], required_role_names: list[str]):
+        # O(n)
+        required_roles = [self.roles.get(role_name, Role()) for role_name in required_role_names]
+        # O(m)
+        user_roles = [self.roles.get(role_name, Role()) for role_name in available_role_names]
+
+        # O(n * m * k), can be slightly optimized using checking firstly LCA of all roles.
+        # but, considering the fact that n, m ~ 1-2 and roles tree is very simple, not needed
+        for role in required_roles:
+            if not any([user_role.check(role) for user_role in user_roles]):
+                raise HTTPException(
+                    status_code = status.HTTP_403_FORBIDDEN,
+                    detail = f'Role "{role}" is required to perform this action',
+                )
+
     @result_or_error(response_model = KeycloakGroupModel, is_list = True)
     def get_all_groups(self, skip: int = 0, limit: int = 20) -> list[KeycloakGroupModel]:
         """Get all base groups of the Keycloak realm
 
         Args:
             skip: paging offset
             limit: maximum results count
```

### Comparing `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/exceptions.py` & `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/model.py` & `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/sotrans_model.py` & `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/sotrans_model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans-fastapi-keycloak
-Version: 0.0.7
+Version: 0.0.8
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

