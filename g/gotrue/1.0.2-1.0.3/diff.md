# Comparing `tmp/gotrue-1.0.2.tar.gz` & `tmp/gotrue-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotrue-1.0.2.tar", max compression
+gzip compressed data, was "gotrue-1.0.3.tar", max compression
```

## Comparing `gotrue-1.0.2.tar` & `gotrue-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2022-11-05 22:33:59.239689 gotrue-1.0.2/LICENSE
--rw-r--r--   0        0        0     5041 2023-06-01 10:45:55.707482 gotrue-1.0.2/README.md
--rw-r--r--   0        0        0      751 2023-06-01 05:34:22.268497 gotrue-1.0.2/gotrue/__init__.py
--rw-r--r--   0        0        0       35 2022-11-05 22:33:59.240564 gotrue-1.0.2/gotrue/_async/__init__.py
--rw-r--r--   0        0        0    19223 2023-01-29 06:28:16.626281 gotrue-1.0.2/gotrue/_async/api.py
--rw-r--r--   0        0        0    22648 2023-02-05 13:49:37.789911 gotrue-1.0.2/gotrue/_async/client.py
--rw-r--r--   0        0        0     5182 2023-01-29 14:15:19.161481 gotrue-1.0.2/gotrue/_async/gotrue_admin_api.py
--rw-r--r--   0        0        0      947 2023-01-29 14:15:19.161743 gotrue-1.0.2/gotrue/_async/gotrue_admin_mfa_api.py
--rw-r--r--   0        0        0     3718 2023-01-29 14:15:19.161955 gotrue-1.0.2/gotrue/_async/gotrue_base_api.py
--rw-r--r--   0        0        0    30677 2023-06-01 05:34:22.269640 gotrue-1.0.2/gotrue/_async/gotrue_client.py
--rw-r--r--   0        0        0     3956 2023-02-05 13:49:31.139486 gotrue-1.0.2/gotrue/_async/gotrue_mfa_api.py
--rw-r--r--   0        0        0      925 2022-11-05 22:33:59.240887 gotrue-1.0.2/gotrue/_async/storage.py
--rw-r--r--   0        0        0       35 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/__init__.py
--rw-r--r--   0        0        0    18964 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/api.py
--rw-r--r--   0        0        0    22135 2023-06-01 10:47:25.880339 gotrue-1.0.2/gotrue/_sync/client.py
--rw-r--r--   0        0        0     5054 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/gotrue_admin_api.py
--rw-r--r--   0        0        0      934 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/gotrue_admin_mfa_api.py
--rw-r--r--   0        0        0     3652 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/gotrue_base_api.py
--rw-r--r--   0        0        0    30067 2023-06-01 10:47:26.012486 gotrue-1.0.2/gotrue/_sync/gotrue_client.py
--rw-r--r--   0        0        0     3913 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/gotrue_mfa_api.py
--rw-r--r--   0        0        0      886 2023-06-01 10:46:14.000000 gotrue-1.0.2/gotrue/_sync/storage.py
--rw-r--r--   0        0        0      329 2023-01-29 14:15:19.164045 gotrue-1.0.2/gotrue/constants.py
--rw-r--r--   0        0        0     2893 2023-01-29 14:15:19.164103 gotrue-1.0.2/gotrue/errors.py
--rw-r--r--   0        0        0     3035 2023-06-01 05:34:22.270484 gotrue-1.0.2/gotrue/helpers.py
--rw-r--r--   0        0        0      202 2022-11-05 22:33:59.241561 gotrue-1.0.2/gotrue/http_clients.py
--rw-r--r--   0        0        0     1366 2023-01-29 14:15:19.164263 gotrue-1.0.2/gotrue/timer.py
--rw-r--r--   0        0        0    15550 2023-06-01 05:34:22.270717 gotrue-1.0.2/gotrue/types.py
--rw-r--r--   0        0        0     1551 2023-06-01 05:34:34.007395 gotrue-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5946 1970-01-01 00:00:00.000000 gotrue-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-11-05 22:33:59.239689 gotrue-1.0.3/LICENSE
+-rw-r--r--   0        0        0     5041 2023-07-01 18:07:56.273487 gotrue-1.0.3/README.md
+-rw-r--r--   0        0        0      751 2023-08-03 07:16:49.388333 gotrue-1.0.3/gotrue/__init__.py
+-rw-r--r--   0        0        0       35 2022-11-05 22:33:59.240564 gotrue-1.0.3/gotrue/_async/__init__.py
+-rw-r--r--   0        0        0    19237 2023-08-03 07:05:28.458958 gotrue-1.0.3/gotrue/_async/api.py
+-rw-r--r--   0        0        0    22659 2023-08-03 07:05:28.459726 gotrue-1.0.3/gotrue/_async/client.py
+-rw-r--r--   0        0        0     5197 2023-08-03 07:05:28.460226 gotrue-1.0.3/gotrue/_async/gotrue_admin_api.py
+-rw-r--r--   0        0        0      947 2023-01-29 14:15:19.161743 gotrue-1.0.3/gotrue/_async/gotrue_admin_mfa_api.py
+-rw-r--r--   0        0        0     3724 2023-08-03 07:05:28.460390 gotrue-1.0.3/gotrue/_async/gotrue_base_api.py
+-rw-r--r--   0        0        0    30724 2023-08-03 07:05:28.461485 gotrue-1.0.3/gotrue/_async/gotrue_client.py
+-rw-r--r--   0        0        0     3956 2023-02-05 13:49:31.139486 gotrue-1.0.3/gotrue/_async/gotrue_mfa_api.py
+-rw-r--r--   0        0        0      925 2022-11-05 22:33:59.240887 gotrue-1.0.3/gotrue/_async/storage.py
+-rw-r--r--   0        0        0       35 2023-06-01 10:46:14.000000 gotrue-1.0.3/gotrue/_sync/__init__.py
+-rw-r--r--   0        0        0    18978 2023-08-03 07:05:28.462309 gotrue-1.0.3/gotrue/_sync/api.py
+-rw-r--r--   0        0        0    22146 2023-08-03 07:05:28.462839 gotrue-1.0.3/gotrue/_sync/client.py
+-rw-r--r--   0        0        0     5069 2023-08-03 07:05:28.463175 gotrue-1.0.3/gotrue/_sync/gotrue_admin_api.py
+-rw-r--r--   0        0        0      934 2023-06-01 10:46:14.000000 gotrue-1.0.3/gotrue/_sync/gotrue_admin_mfa_api.py
+-rw-r--r--   0        0        0     3658 2023-08-03 07:05:28.463397 gotrue-1.0.3/gotrue/_sync/gotrue_base_api.py
+-rw-r--r--   0        0        0    30103 2023-08-03 07:05:28.463668 gotrue-1.0.3/gotrue/_sync/gotrue_client.py
+-rw-r--r--   0        0        0     3913 2023-06-01 10:46:14.000000 gotrue-1.0.3/gotrue/_sync/gotrue_mfa_api.py
+-rw-r--r--   0        0        0      886 2023-06-01 10:46:14.000000 gotrue-1.0.3/gotrue/_sync/storage.py
+-rw-r--r--   0        0        0      329 2023-01-29 14:15:19.164045 gotrue-1.0.3/gotrue/constants.py
+-rw-r--r--   0        0        0     2893 2023-01-29 14:15:19.164103 gotrue-1.0.3/gotrue/errors.py
+-rw-r--r--   0        0        0     3075 2023-08-03 07:05:28.463921 gotrue-1.0.3/gotrue/helpers.py
+-rw-r--r--   0        0        0      202 2022-11-05 22:33:59.241561 gotrue-1.0.3/gotrue/http_clients.py
+-rw-r--r--   0        0        0     1366 2023-01-29 14:15:19.164263 gotrue-1.0.3/gotrue/timer.py
+-rw-r--r--   0        0        0    15453 2023-08-03 07:05:28.464148 gotrue-1.0.3/gotrue/types.py
+-rw-r--r--   0        0        0     1548 2023-08-03 07:32:01.812944 gotrue-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5893 1970-01-01 00:00:00.000000 gotrue-1.0.3/PKG-INFO
```

### Comparing `gotrue-1.0.2/LICENSE` & `gotrue-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.2/README.md` & `gotrue-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.2/gotrue/__init__.py` & `gotrue-1.0.3/gotrue/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "1.0.1"
+__version__ = "1.0.3"
 
 from ._async.gotrue_admin_api import AsyncGoTrueAdminAPI  # type: ignore # noqa: F401
 from ._async.gotrue_client import AsyncGoTrueClient  # type: ignore # noqa: F401
 from ._async.storage import AsyncMemoryStorage  # type: ignore # noqa: F401
 from ._async.storage import AsyncSupportedStorage  # type: ignore # noqa: F401
 from ._sync.gotrue_admin_api import SyncGoTrueAdminAPI  # type: ignore # noqa: F401
 from ._sync.gotrue_client import SyncGoTrueClient  # type: ignore # noqa: F401
```

### Comparing `gotrue-1.0.2/gotrue/_async/api.py` & `gotrue-1.0.3/gotrue/_async/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import parse_obj_as
+from pydantic import TypeAdapter
 
 from ..exceptions import APIError
 from ..helpers import check_response, encode_uri_component
 from ..http_clients import AsyncClient
 from ..types import (
     CookieOptions,
     LinkType,
@@ -90,15 +90,15 @@
         response = await self.http_client.get(url, headers=headers)
         check_response(response)
         users = response.json().get("users")
         if users is None:
             raise APIError("No users found in response", 400)
         if not isinstance(users, list):
             raise APIError("Expected a list of users", 400)
-        return parse_obj_as(List[User], users)
+        return TypeAdapter(List[User]).validate_python(users)
 
     async def sign_up_with_email(
         self,
         *,
         email: str,
         password: str,
         redirect_to: Optional[str] = None,
```

### Comparing `gotrue-1.0.2/gotrue/_async/client.py` & `gotrue-1.0.3/gotrue/_async/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,15 +556,15 @@
         expires_at_raw = data.get("expires_at")
         if (
             expires_at_raw
             and isinstance(expires_at_raw, int)
             and session_raw
             and isinstance(session_raw, dict)
         ):
-            session = Session.parse_obj(session_raw)
+            session = Session.model_validate(session_raw)
             expires_at = int(expires_at_raw)
             time_now = round(time())
             return session, expires_at, time_now
 
     async def _recover_session(self) -> None:
         """Attempts to get the session from LocalStorage"""
         result = await self._recover_common()
@@ -624,15 +624,15 @@
             self._start_auto_refresh_token(
                 value=(expire_in - refresh_duration_before_expires)
             )
         if self.persist_session and session.expires_at:
             await self._persist_session(session=session)
 
     async def _persist_session(self, *, session: Session) -> None:
-        data = {"session": session.dict(), "expires_at": session.expires_at}
+        data = {"session": session.model_dump(), "expires_at": session.expires_at}
         await self.local_storage.set_item(STORAGE_KEY, dumps(data, default=str))
 
     async def _remove_session(self) -> None:
         """Remove the session."""
         self.current_session = None
         self.current_user = None
         if self.refresh_token_timer:
```

### Comparing `gotrue-1.0.2/gotrue/_async/gotrue_admin_api.py` & `gotrue-1.0.3/gotrue/_async/gotrue_admin_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         This function should only be called on a server.
         Never expose your `service_role` key in the browser.
         """
         return await self._request(
             "GET",
             "admin/users",
-            xform=lambda data: [User.parse_obj(user) for user in data["users"]]
+            xform=lambda data: [User.model_validate(user) for user in data["users"]]
             if "users" in data
             else [],
         )
 
     async def get_user_by_id(self, uid: str) -> UserResponse:
         """
         Get user by id.
@@ -157,19 +157,19 @@
     async def _list_factors(
         self,
         params: AuthMFAAdminListFactorsParams,
     ) -> AuthMFAAdminListFactorsResponse:
         return await self._request(
             "GET",
             f"admin/users/{params.get('user_id')}/factors",
-            xform=AuthMFAAdminListFactorsResponse.parse_obj,
+            xform=AuthMFAAdminListFactorsResponse.model_validate,
         )
 
     async def _delete_factor(
         self,
         params: AuthMFAAdminDeleteFactorParams,
     ) -> AuthMFAAdminDeleteFactorResponse:
         return await self._request(
             "DELETE",
             f"admin/users/{params.get('user_id')}/factors/{params.get('factor_id')}",
-            xform=AuthMFAAdminDeleteFactorResponse.parse_obj,
+            xform=AuthMFAAdminDeleteFactorResponse.model_validate,
         )
```

### Comparing `gotrue-1.0.2/gotrue/_async/gotrue_admin_mfa_api.py` & `gotrue-1.0.3/gotrue/_async/gotrue_admin_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.2/gotrue/_async/gotrue_base_api.py` & `gotrue-1.0.3/gotrue/_async/gotrue_base_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             query["redirect_to"] = redirect_to
         try:
             response = await self._http_client.request(
                 method,
                 url,
                 headers=headers,
                 params=query,
-                json=body.dict() if isinstance(body, BaseModel) else body,
+                json=body.model_dump() if isinstance(body, BaseModel) else body,
             )
             response.raise_for_status()
             result = response if no_resolve_json else response.json()
             if xform:
                 return xform(result)
         except Exception as e:
             raise handle_exception(e)
```

### Comparing `gotrue-1.0.2/gotrue/_async/gotrue_client.py` & `gotrue-1.0.3/gotrue/_async/gotrue_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -527,29 +527,29 @@
         if not session:
             raise AuthSessionMissingError()
         response = await self._request(
             "POST",
             "factors",
             body=params,
             jwt=session.access_token,
-            xform=AuthMFAEnrollResponse.parse_obj,
+            xform=AuthMFAEnrollResponse.model_validate,
         )
         if response.totp.qr_code:
             response.totp.qr_code = f"data:image/svg+xml;utf-8,{response.totp.qr_code}"
         return response
 
     async def _challenge(self, params: MFAChallengeParams) -> AuthMFAChallengeResponse:
         session = await self.get_session()
         if not session:
             raise AuthSessionMissingError()
         return await self._request(
             "POST",
             f"factors/{params.get('factor_id')}/challenge",
             jwt=session.access_token,
-            xform=AuthMFAChallengeResponse.parse_obj,
+            xform=AuthMFAChallengeResponse.model_validate,
         )
 
     async def _challenge_and_verify(
         self,
         params: MFAChallengeAndVerifyParams,
     ) -> AuthMFAVerifyResponse:
         response = await self._challenge(
@@ -570,30 +570,30 @@
         if not session:
             raise AuthSessionMissingError()
         response = await self._request(
             "POST",
             f"factors/{params.get('factor_id')}/verify",
             body=params,
             jwt=session.access_token,
-            xform=AuthMFAVerifyResponse.parse_obj,
+            xform=AuthMFAVerifyResponse.model_validate,
         )
-        session = Session.parse_obj(response.dict())
+        session = Session.model_validate(response.model_dump())
         await self._save_session(session)
         self._notify_all_subscribers("MFA_CHALLENGE_VERIFIED", session)
         return response
 
     async def _unenroll(self, params: MFAUnenrollParams) -> AuthMFAUnenrollResponse:
         session = await self.get_session()
         if not session:
             raise AuthSessionMissingError()
         return await self._request(
             "DELETE",
             f"factors/{params.get('factor_id')}",
             jwt=session.access_token,
-            xform=AuthMFAUnenrollResponse.parse_obj,
+            xform=AuthMFAUnenrollResponse.model_validate,
         )
 
     async def _list_factors(self) -> AuthMFAListFactorsResponse:
         response = await self.get_user()
         all = response.user.factors or []
         totp = [f for f in all if f.factor_type == "totp" and f.status == "verified"]
         return AuthMFAListFactorsResponse(all=all, totp=totp)
@@ -747,15 +747,15 @@
             expire_in = expire_at - time_now
             refresh_duration_before_expires = (
                 EXPIRY_MARGIN if expire_in > EXPIRY_MARGIN else 0.5
             )
             value = (expire_in - refresh_duration_before_expires) * 1000
             await self._start_auto_refresh_token(value)
         if self._persist_session and session.expires_at:
-            await self._storage.set_item(self._storage_key, session.json())
+            await self._storage.set_item(self._storage_key, session.model_dump_json())
 
     async def _start_auto_refresh_token(self, value: float) -> None:
         if self._refresh_token_timer:
             self._refresh_token_timer.cancel()
             self._refresh_token_timer = None
         if value <= 0 or not self._auto_refresh_token:
             return
@@ -804,15 +804,15 @@
             return None
         try:
             expires_at = int(data["expires_at"])
             data["expires_at"] = expires_at
         except ValueError:
             return None
         try:
-            return Session.parse_obj(data)
+            return Session.model_validate(data)
         except Exception:
             return None
 
     def _get_param(
         self,
         query_params: Dict[str, List[str]],
         name: str,
```

### Comparing `gotrue-1.0.2/gotrue/_async/gotrue_mfa_api.py` & `gotrue-1.0.3/gotrue/_async/gotrue_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.2/gotrue/_async/storage.py` & `gotrue-1.0.3/gotrue/_async/storage.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.2/gotrue/_sync/api.py` & `gotrue-1.0.3/gotrue/_sync/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import parse_obj_as
+from pydantic import TypeAdapter
 
 from ..exceptions import APIError
 from ..helpers import check_response, encode_uri_component
 from ..http_clients import SyncClient
 from ..types import (
     CookieOptions,
     LinkType,
@@ -90,15 +90,15 @@
         response = self.http_client.get(url, headers=headers)
         check_response(response)
         users = response.json().get("users")
         if users is None:
             raise APIError("No users found in response", 400)
         if not isinstance(users, list):
             raise APIError("Expected a list of users", 400)
-        return parse_obj_as(List[User], users)
+        return TypeAdapter(List[User]).validate_python(users)
 
     def sign_up_with_email(
         self,
         *,
         email: str,
         password: str,
         redirect_to: Optional[str] = None,
```

### Comparing `gotrue-1.0.2/gotrue/_sync/client.py` & `gotrue-1.0.3/gotrue/_sync/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,15 +552,15 @@
         expires_at_raw = data.get("expires_at")
         if (
             expires_at_raw
             and isinstance(expires_at_raw, int)
             and session_raw
             and isinstance(session_raw, dict)
         ):
-            session = Session.parse_obj(session_raw)
+            session = Session.model_validate(session_raw)
             expires_at = int(expires_at_raw)
             time_now = round(time())
             return session, expires_at, time_now
 
     def _recover_session(self) -> None:
         """Attempts to get the session from LocalStorage"""
         result = self._recover_common()
@@ -616,15 +616,15 @@
             self._start_auto_refresh_token(
                 value=(expire_in - refresh_duration_before_expires)
             )
         if self.persist_session and session.expires_at:
             self._persist_session(session=session)
 
     def _persist_session(self, *, session: Session) -> None:
-        data = {"session": session.dict(), "expires_at": session.expires_at}
+        data = {"session": session.model_dump(), "expires_at": session.expires_at}
         self.local_storage.set_item(STORAGE_KEY, dumps(data, default=str))
 
     def _remove_session(self) -> None:
         """Remove the session."""
         self.current_session = None
         self.current_user = None
         if self.refresh_token_timer:
```

### Comparing `gotrue-1.0.2/gotrue/_sync/gotrue_admin_api.py` & `gotrue-1.0.3/gotrue/_sync/gotrue_admin_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         This function should only be called on a server.
         Never expose your `service_role` key in the browser.
         """
         return self._request(
             "GET",
             "admin/users",
-            xform=lambda data: [User.parse_obj(user) for user in data["users"]]
+            xform=lambda data: [User.model_validate(user) for user in data["users"]]
             if "users" in data
             else [],
         )
 
     def get_user_by_id(self, uid: str) -> UserResponse:
         """
         Get user by id.
@@ -157,19 +157,19 @@
     def _list_factors(
         self,
         params: AuthMFAAdminListFactorsParams,
     ) -> AuthMFAAdminListFactorsResponse:
         return self._request(
             "GET",
             f"admin/users/{params.get('user_id')}/factors",
-            xform=AuthMFAAdminListFactorsResponse.parse_obj,
+            xform=AuthMFAAdminListFactorsResponse.model_validate,
         )
 
     def _delete_factor(
         self,
         params: AuthMFAAdminDeleteFactorParams,
     ) -> AuthMFAAdminDeleteFactorResponse:
         return self._request(
             "DELETE",
             f"admin/users/{params.get('user_id')}/factors/{params.get('factor_id')}",
-            xform=AuthMFAAdminDeleteFactorResponse.parse_obj,
+            xform=AuthMFAAdminDeleteFactorResponse.model_validate,
         )
```

### Comparing `gotrue-1.0.2/gotrue/_sync/gotrue_admin_mfa_api.py` & `gotrue-1.0.3/gotrue/_sync/gotrue_admin_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.2/gotrue/_sync/gotrue_base_api.py` & `gotrue-1.0.3/gotrue/_sync/gotrue_base_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             query["redirect_to"] = redirect_to
         try:
             response = self._http_client.request(
                 method,
                 url,
                 headers=headers,
                 params=query,
-                json=body.dict() if isinstance(body, BaseModel) else body,
+                json=body.model_dump() if isinstance(body, BaseModel) else body,
             )
             response.raise_for_status()
             result = response if no_resolve_json else response.json()
             if xform:
                 return xform(result)
         except Exception as e:
             raise handle_exception(e)
```

### Comparing `gotrue-1.0.2/gotrue/_sync/gotrue_client.py` & `gotrue-1.0.3/gotrue/_sync/gotrue_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -525,29 +525,29 @@
         if not session:
             raise AuthSessionMissingError()
         response = self._request(
             "POST",
             "factors",
             body=params,
             jwt=session.access_token,
-            xform=AuthMFAEnrollResponse.parse_obj,
+            xform=AuthMFAEnrollResponse.model_validate,
         )
         if response.totp.qr_code:
             response.totp.qr_code = f"data:image/svg+xml;utf-8,{response.totp.qr_code}"
         return response
 
     def _challenge(self, params: MFAChallengeParams) -> AuthMFAChallengeResponse:
         session = self.get_session()
         if not session:
             raise AuthSessionMissingError()
         return self._request(
             "POST",
             f"factors/{params.get('factor_id')}/challenge",
             jwt=session.access_token,
-            xform=AuthMFAChallengeResponse.parse_obj,
+            xform=AuthMFAChallengeResponse.model_validate,
         )
 
     def _challenge_and_verify(
         self,
         params: MFAChallengeAndVerifyParams,
     ) -> AuthMFAVerifyResponse:
         response = self._challenge(
@@ -568,30 +568,30 @@
         if not session:
             raise AuthSessionMissingError()
         response = self._request(
             "POST",
             f"factors/{params.get('factor_id')}/verify",
             body=params,
             jwt=session.access_token,
-            xform=AuthMFAVerifyResponse.parse_obj,
+            xform=AuthMFAVerifyResponse.model_validate,
         )
-        session = Session.parse_obj(response.dict())
+        session = Session.model_validate(response.model_dump())
         self._save_session(session)
         self._notify_all_subscribers("MFA_CHALLENGE_VERIFIED", session)
         return response
 
     def _unenroll(self, params: MFAUnenrollParams) -> AuthMFAUnenrollResponse:
         session = self.get_session()
         if not session:
             raise AuthSessionMissingError()
         return self._request(
             "DELETE",
             f"factors/{params.get('factor_id')}",
             jwt=session.access_token,
-            xform=AuthMFAUnenrollResponse.parse_obj,
+            xform=AuthMFAUnenrollResponse.model_validate,
         )
 
     def _list_factors(self) -> AuthMFAListFactorsResponse:
         response = self.get_user()
         all = response.user.factors or []
         totp = [f for f in all if f.factor_type == "totp" and f.status == "verified"]
         return AuthMFAListFactorsResponse(all=all, totp=totp)
@@ -802,15 +802,15 @@
             return None
         try:
             expires_at = int(data["expires_at"])
             data["expires_at"] = expires_at
         except ValueError:
             return None
         try:
-            return Session.parse_obj(data)
+            return Session.model_validate(data)
         except Exception:
             return None
 
     def _get_param(
         self,
         query_params: Dict[str, List[str]],
         name: str,
```

### Comparing `gotrue-1.0.2/gotrue/_sync/gotrue_mfa_api.py` & `gotrue-1.0.3/gotrue/_sync/gotrue_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.2/gotrue/_sync/storage.py` & `gotrue-1.0.3/gotrue/_sync/storage.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.2/gotrue/errors.py` & `gotrue-1.0.3/gotrue/errors.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.2/gotrue/helpers.py` & `gotrue-1.0.3/gotrue/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,36 +23,38 @@
         "access_token" in data
         and "refresh_token" in data
         and "expires_in" in data
         and data["access_token"]
         and data["refresh_token"]
         and data["expires_in"]
     ):
-        session = Session.parse_obj(data)
+        session = Session.model_validate(data)
     user_data = data.get("user", data)
-    user = User.parse_obj(user_data) if user_data else None
+    user = User.model_validate(user_data) if user_data else None
     return AuthResponse(session=session, user=user)
 
 
 def parse_link_response(data: Any) -> GenerateLinkResponse:
     properties = GenerateLinkProperties(
         action_link=data.get("action_link"),
         email_otp=data.get("email_otp"),
         hashed_token=data.get("hashed_token"),
         redirect_to=data.get("redirect_to"),
         verification_type=data.get("verification_type"),
     )
-    user = User.parse_obj({k: v for k, v in data.items() if k not in properties.dict()})
+    user = User.model_validate(
+        {k: v for k, v in data.items() if k not in properties.model_dump()}
+    )
     return GenerateLinkResponse(properties=properties, user=user)
 
 
 def parse_user_response(data: Any) -> UserResponse:
     if "user" not in data:
         data = {"user": data}
-    return UserResponse.parse_obj(data)
+    return UserResponse.model_validate(data)
 
 
 def get_error_message(error: Any) -> str:
     props = ["msg", "message", "error_description", "error"]
     filter = (
         lambda prop: prop in error if isinstance(error, dict) else hasattr(error, prop)
     )
```

### Comparing `gotrue-1.0.2/gotrue/timer.py` & `gotrue-1.0.3/gotrue/timer.py`

 * *Files identical despite different names*

### Comparing `gotrue-1.0.2/gotrue/types.py` & `gotrue-1.0.3/gotrue/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from datetime import datetime
 from time import time
 from typing import Any, Callable, Dict, List, Union
 
-from pydantic import BaseModel, root_validator
+from pydantic import BaseModel, model_validator
 from typing_extensions import Literal, NotRequired, TypedDict
 
 Provider = Literal[
     "apple",
     "azure",
     "bitbucket",
     "discord",
@@ -102,15 +102,15 @@
     expires_at: Union[int, None] = None
     """
     A timestamp of when the token will expire. Returned when a login is confirmed.
     """
     token_type: str
     user: User
 
-    @root_validator
+    @model_validator(mode="before")
     def validator(cls, values: dict) -> dict:
         expires_in = values.get("expires_in")
         if expires_in and not values.get("expires_at"):
             values["expires_at"] = round(time()) + expires_in
         return values
 
 
@@ -611,26 +611,26 @@
 
 class DecodedJWTDict(TypedDict):
     exp: NotRequired[int]
     aal: NotRequired[Union[AuthenticatorAssuranceLevels, None]]
     amr: NotRequired[Union[List[AMREntry], None]]
 
 
-AMREntry.update_forward_refs()
-AuthResponse.update_forward_refs()
-OAuthResponse.update_forward_refs()
-UserResponse.update_forward_refs()
-Session.update_forward_refs()
-UserIdentity.update_forward_refs()
-Factor.update_forward_refs()
-User.update_forward_refs()
-Subscription.update_forward_refs()
-AuthMFAVerifyResponse.update_forward_refs()
-AuthMFAEnrollResponseTotp.update_forward_refs()
-AuthMFAEnrollResponse.update_forward_refs()
-AuthMFAUnenrollResponse.update_forward_refs()
-AuthMFAChallengeResponse.update_forward_refs()
-AuthMFAListFactorsResponse.update_forward_refs()
-AuthMFAGetAuthenticatorAssuranceLevelResponse.update_forward_refs()
-AuthMFAAdminDeleteFactorResponse.update_forward_refs()
-AuthMFAAdminListFactorsResponse.update_forward_refs()
-GenerateLinkProperties.update_forward_refs()
+AMREntry.model_rebuild()
+AuthResponse.model_rebuild()
+OAuthResponse.model_rebuild()
+UserResponse.model_rebuild()
+Session.model_rebuild()
+UserIdentity.model_rebuild()
+Factor.model_rebuild()
+User.model_rebuild()
+Subscription.model_rebuild()
+AuthMFAVerifyResponse.model_rebuild()
+AuthMFAEnrollResponseTotp.model_rebuild()
+AuthMFAEnrollResponse.model_rebuild()
+AuthMFAUnenrollResponse.model_rebuild()
+AuthMFAChallengeResponse.model_rebuild()
+AuthMFAListFactorsResponse.model_rebuild()
+AuthMFAGetAuthenticatorAssuranceLevelResponse.model_rebuild()
+AuthMFAAdminDeleteFactorResponse.model_rebuild()
+AuthMFAAdminListFactorsResponse.model_rebuild()
+GenerateLinkProperties.model_rebuild()
```

### Comparing `gotrue-1.0.2/pyproject.toml` & `gotrue-1.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gotrue"
-version = "1.0.2"
+version = "1.0.3"
 description = "Python Client Library for GoTrue"
 authors = ["Joel Lee <joel@joellee.org>"]
 homepage = "https://github.com/supabase-community/gotrue-py"
 repository = "https://github.com/supabase-community/gotrue-py"
 documentation = "https://github.com/supabase-community/gotrue-py"
 readme = "README.md"
 license = "MIT"
@@ -13,28 +13,28 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = ">=0.23,<0.25"
-pydantic = "^1.10.0"
+pydantic = "^2.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 flake8 = "^5.0.4"
-black = "^23.1.0"
+black = "^23.3.0"
 isort = "^5.12.0"
 pre-commit = "^3.2.2"
 pytest-cov = "^4.0.0"
 pytest-depends = "^1.0.1"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = "^0.21.1"
 Faker = "^18.3.1"
 unasync-cli = "^0.0.9"
-python-semantic-release = "^7.33.2"
+python-semantic-release = "^7.34.6"
 
 [tool.poetry.group.dev.dependencies]
 pygithub = "^1.57"
 
 [tool.semantic_release]
 version_variable = "gotrue/__init__.py:__version__"
 version_toml = "pyproject.toml:tool.poetry.version"
```

### Comparing `gotrue-1.0.2/PKG-INFO` & `gotrue-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: gotrue
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Client Library for GoTrue
 Home-page: https://github.com/supabase-community/gotrue-py
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: httpx (>=0.23,<0.25)
-Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: pydantic (>=2.1,<3.0)
 Project-URL: Documentation, https://github.com/supabase-community/gotrue-py
 Project-URL: Repository, https://github.com/supabase-community/gotrue-py
 Description-Content-Type: text/markdown
 
 # gotrue-py
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?label=license)](https://opensource.org/licenses/MIT)
```

