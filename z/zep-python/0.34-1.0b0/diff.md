# Comparing `tmp/zep_python-0.34.tar.gz` & `tmp/zep_python-1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.34.tar", max compression
+gzip compressed data, was "zep_python-1.0b0.tar", max compression
```

## Comparing `zep_python-0.34.tar` & `zep_python-1.0b0.tar`

### file list

```diff
@@ -1,9 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-08-02 23:15:07.689601 zep_python-0.34/LICENSE
--rw-r--r--   0        0        0     2402 2023-08-02 23:15:07.689601 zep_python-0.34/README.md
--rw-r--r--   0        0        0      872 2023-08-02 23:15:07.693601 zep_python-0.34/pyproject.toml
--rw-r--r--   0        0        0      417 2023-08-02 23:15:07.693601 zep_python-0.34/zep_python/__init__.py
--rw-r--r--   0        0        0     2234 2023-08-02 23:15:07.693601 zep_python-0.34/zep_python/exceptions.py
--rw-r--r--   0        0        0     5855 2023-08-02 23:15:07.693601 zep_python-0.34/zep_python/models.py
--rw-r--r--   0        0        0        0 2023-08-02 23:15:07.693601 zep_python-0.34/zep_python/py.typed
--rw-r--r--   0        0        0    19426 2023-08-02 23:15:07.693601 zep_python-0.34/zep_python/zep_client.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 zep_python-0.34/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 23:20:19.775943 zep_python-1.0b0/LICENSE
+-rw-r--r--   0        0        0      877 2023-08-02 23:20:19.775943 zep_python-1.0b0/README.md
+-rw-r--r--   0        0        0     1074 2023-08-02 23:20:19.779943 zep_python-1.0b0/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/__init__.py
+-rw-r--r--   0        0        0      168 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/document/__init__.py
+-rw-r--r--   0        0        0    13320 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/document/client.py
+-rw-r--r--   0        0        0    18469 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/document/collections.py
+-rw-r--r--   0        0        0     3764 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/document/models.py
+-rw-r--r--   0        0        0     2608 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/experimental/__init__.py
+-rw-r--r--   0        0        0       74 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/experimental/langchain/__init__.py
+-rw-r--r--   0        0        0    20276 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/experimental/langchain/zep_vectorstore.py
+-rw-r--r--   0        0        0      268 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/memory/__init__.py
+-rw-r--r--   0        0        0    17816 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/memory/client.py
+-rw-r--r--   0        0        0     5883 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/memory/models.py
+-rw-r--r--   0        0        0        0 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/py.typed
+-rw-r--r--   0        0        0      375 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/utils.py
+-rw-r--r--   0        0        0     8486 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/zep_client.py
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 zep_python-1.0b0/PKG-INFO
```

### Comparing `zep_python-0.34/LICENSE` & `zep_python-1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.34/pyproject.toml` & `zep_python-1.0b0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "zep-python"
-version = "0.34"
+version = "1.0b0"
 description = "Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.9.0,<4"
 httpx = "^0.24.0"
 pydantic = "^1.10.7"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-httpx = "^0.22.0"
 pytest-asyncio = "^0.21.0"
@@ -21,13 +21,23 @@
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.265"
 mypy = "^1.2.0"
 pre-commit = "^3.3.1"
 mkdocs = "^1.4.3"
 mkdocstrings = {version = "0.21.2", extras = ["python"]}
-python-dotenv = "^1.0.0"
 mkdocs-material = "^9.1.13"
+pytest-httpx = "^0.22.0"
+faker = "^19.2.0"
+python-dotenv = "^1.0.0"
+
+
+[tool.poetry.group.experimental.dependencies]
+langchain = "^0.0.247"
+numpy = "^1.25.1"
+openai = "^0.27.8"
+tiktoken = "^0.4.0"
+llama-index = "^0.7.16"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `zep_python-0.34/zep_python/exceptions.py` & `zep_python-1.0b0/zep_python/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,7 +82,21 @@
     Raised when the API response contains no results.
 
     Inherits from ZepClientError.
     """
 
     def __init__(self, message: str) -> None:
         super().__init__(message)
+
+
+def handle_response(
+    response: httpx.Response, missing_doc: Optional[str] = None
+) -> None:
+    missing_doc = missing_doc or "No query results found"
+    if response.status_code == 404:
+        raise NotFoundError(missing_doc)
+
+    if response.status_code == 401:
+        raise AuthError(response)
+
+    if response.status_code != 200:
+        raise APIError(response)
```

### Comparing `zep_python-0.34/zep_python/models.py` & `zep_python-1.0b0/zep_python/memory/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,18 +26,18 @@
         Generated by the server.
     session_id : str
         The unique identifier of the session.
     metadata : Dict[str, Any]
         The metadata associated with the session.
     """
 
-    uuid: Optional[str]
-    created_at: Optional[str]
-    updated_at: Optional[str]
-    deleted_at: Optional[str]
+    uuid: Optional[str] = None
+    created_at: Optional[str] = None
+    updated_at: Optional[str] = None
+    deleted_at: Optional[str] = None
     session_id: str
     metadata: Dict[str, Any]
 
 
 class Summary(BaseModel):
     """
     Represents a summary of a conversation.
```

### Comparing `zep_python-0.34/zep_python/zep_client.py` & `zep_python-1.0b0/zep_python/memory/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,120 +1,97 @@
 from __future__ import annotations
 
-from types import TracebackType
-from typing import Any, Dict, List, Optional, Type
-from urllib.parse import urljoin
+from typing import Any, Dict, List, Optional
 
 import httpx
 
-from zep_python.exceptions import APIError, AuthError, NotFoundError
-from zep_python.models import (
+from zep_python.exceptions import APIError, handle_response
+from zep_python.memory.models import (
     Memory,
     MemorySearchPayload,
     MemorySearchResult,
     Message,
     Session,
     Summary,
 )
 
-API_BASE_PATH = "/api/v1"
-API_TIMEOUT = 10
 
-
-class ZepClient:
+class MemoryClient:
     """
-    ZepClient class implementation.
+    memory_client class implementation for memory APIs.
 
     Attributes
     ----------
-    base_url : str
-        The base URL of the API.
-    client : httpx.AsyncClient
-        The HTTP client used for making API requests.
+    aclient : httpx.AsyncClient
+        The async client used for making API requests.
+    client : httpx.Client
+        The client used for making API requests.
 
     Methods
     -------
-    get_memory(session_id: str, lastn: Optional[int] = None) -> List[Memory]:
-        Retrieve memory for the specified session.
-    add_memory(session_id: str, memory_messages: Memory) -> str:
-        Add memory to the specified session.
-    delete_memory(session_id: str) -> str:
-        Delete memory for the specified session.
-    search_memory(session_id: str, search_payload: SearchPayload,
-                  limit: Optional[int] = None) -> List[SearchResult]:
-        Search memory for the specified session.
-    close() -> None:
-        Close the HTTP client.
-    """
+    ___init___(aclient: httpx.AsyncClient, client: httpx.Client) -> None:
+        Initialize the zep_memory_api.
 
-    def __init__(self, base_url: str, api_key: Optional[str] = None) -> None:
-        """
-        Initialize the ZepClient with the specified base URL.
+    handle_response(response: httpx.Response,
+                    missing_message:
+                    Optional[str] = None) -> None:
+        Handle the response from the API.
 
-        Parameters
-        ----------
-        base_url : str
-            The base URL of the API.
+    parse_get_memory_response(response_data: Any) -> Memory:
+        Parse the response from the get_memory API call.
 
-        api_key : Optional[str]
-            The API key to use for authentication. (optional)
-        """
+    gen_get_params(lastn: Optional[int] = None) -> Dict[str, Any]:
+        Generate the parameters for the get_memory API call.
+
+    get_session(session_id: str) -> Session:
+        Retrieve the session with the specified ID.
 
-        headers: Dict[str, str] = {}
-        if api_key is not None:
-            headers["Authorization"] = f"Bearer {api_key}"
+    aget_session(session_id: str) -> Session:
+        Asynchronously retrieve the session with the specified ID.
 
-        self.base_url = concat_url(base_url, API_BASE_PATH)
-        self.aclient = httpx.AsyncClient(
-            base_url=self.base_url, headers=headers, timeout=API_TIMEOUT
-        )
-        self.client = httpx.Client(
-            base_url=self.base_url, headers=headers, timeout=API_TIMEOUT
-        )
+    add_session(session: Session) -> str:
+        Add or update the specified session.
 
-        self._healthcheck(base_url)
+    aaadd_session(session: Session) -> str:
+        Asynchronously add or update the specified session.
 
-    async def __aenter__(self) -> "ZepClient":
-        """Asynchronous context manager entry point"""
-        return self
+    get_memory(session_id: str, lastn: Optional[int] = None) -> Memory:
+        Retrieve memory for the specified session.
 
-    async def __aexit__(
-        self,
-        exc_type: Type[Exception],
-        exc_val: Exception,
-        exc_tb: TracebackType,
-    ) -> None:
-        """Asynchronous context manager exit point"""
-        await self.aclose()
-
-    def __enter__(self) -> "ZepClient":
-        """Sync context manager entry point"""
-        return self
+    aget_memory(session_id: str, lastn: Optional[int] = None) -> Memory:
+        Asynchronously retrieve memory for the specified session.
 
-    def __exit__(
-        self,
-        exc_type: Type[Exception],
-        exc_val: Exception,
-        exc_tb: TracebackType,
-    ) -> None:
-        """Sync context manager exit point"""
-        self.close()
-
-    def _handle_response(
-        self, response: httpx.Response, missing_message: Optional[str] = None
-    ) -> None:
-        missing_message = missing_message or "No query results found"
-        if response.status_code == 404:
-            raise NotFoundError(missing_message)
+    add_memory(session_id: str, memory_messages: Memory) -> str:
+        Add memory to the specified session.
 
-        if response.status_code == 401:
-            raise AuthError(response)
+    aadd_memory(session_id: str, memory_messages: Memory) -> str:
+        Asynchronously add memory to the specified session.
 
-        if response.status_code != 200:
-            raise APIError(response)
+    delete_memory(session_id: str) -> str:
+        Delete memory for the specified session.
+
+    adelete_memory(session_id: str) -> str:
+        Asynchronously delete memory for the specified session.
+
+    search_memory(session_id: str, search_payload: MemorySearchPayload,
+                    limit: Optional[int] = None) -> List[MemorySearchResult]:
+        Search memory for the specified session.
+
+    asearch_memory(session_id: str, search_payload: MemorySearchPayload,
+                    limit: Optional[int] = None) -> List[MemorySearchResult]:
+        Asynchronously search memory for the specified session.
+
+    """
+
+    aclient: httpx.AsyncClient
+    client: httpx.Client
+
+    def __init__(self, aclient: httpx.AsyncClient, client: httpx.Client) -> None:
+        self.aclient = aclient
+        self.client = client
 
     def _parse_get_memory_response(self, response_data: Any) -> Memory:
         """Parse the response from the get_memory API call."""
         messages: List[Message]
         try:
             messages = [
                 Message.parse_obj(m) for m in response_data.get("messages", None)
@@ -139,42 +116,15 @@
 
     def _gen_get_params(self, lastn: Optional[int] = None) -> Dict[str, Any]:
         params = {}
         if lastn is not None:
             params["lastn"] = lastn
         return params
 
-    def _healthcheck(self, base_url: str) -> None:
-        """
-        Check that the Zep server is running and the API URL is correct.
-
-        Raises
-        ------
-        ConnectionError
-            If the server is not running or the API URL is incorrect.
-        """
-
-        url = concat_url(base_url, "/healthz")
-
-        error_msg = """Failed to connect to Zep server. Please check that:
-         - the server is running 
-         - the API URL is correct
-         - No other process is using the same port"""
-
-        try:
-            response = httpx.get(url)
-
-            self._handle_response(response, error_msg)
-
-            if response.status_code == 200 and response.text != ".":
-                raise APIError(response, error_msg)
-
-        except (httpx.ConnectError, httpx.NetworkError, httpx.TimeoutException) as e:
-            raise APIError(None, error_msg) from e
-
+    # Memory APIs : Get a Session
     def get_session(self, session_id: str) -> Session:
         """
         Retrieve the session with the specified ID.
 
         Parameters
         ----------
         session_id : str
@@ -198,20 +148,21 @@
         url = f"/sessions/{session_id}"
 
         try:
             response = self.client.get(url)
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
-        self._handle_response(response, f"No session found for session {session_id}")
+        handle_response(response, f"No session found for session {session_id}")
 
         response_data = response.json()
 
         return Session.parse_obj(response_data)
 
+    # Memory APIs : Get a Session Asynchronously
     async def aget_session(self, session_id: str) -> Session:
         """
         Asynchronously retrieve the session with the specified ID.
 
         Parameters
         ----------
         session_id : str
@@ -235,20 +186,21 @@
         url = f"/sessions/{session_id}"
 
         try:
             response = await self.aclient.get(url)
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
-        self._handle_response(response, f"No session found for session {session_id}")
+        handle_response(response, f"No session found for session {session_id}")
 
         response_data = response.json()
 
         return Session.parse_obj(response_data)
 
+    # Memory APIs : Add a Session
     def add_session(self, session: Session) -> str:
         """
         Add or update the specified session.
 
         Parameters
         ----------
         session : Session
@@ -274,18 +226,19 @@
         url = f"/sessions/{session.session_id}"
 
         try:
             response = self.client.post(url, json=session.dict(exclude_none=True))
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
-        self._handle_response(response, f"Failed to add session {session.session_id}")
+        handle_response(response, f"Failed to add session {session.session_id}")
 
         return response.text
 
+    # Memory APIs : Add a Session Asynchronously
     async def aadd_session(self, session: Session) -> str:
         """
         Asynchronously add or update the specified session.
 
         Parameters
         ----------
         session : Session
@@ -313,18 +266,19 @@
         try:
             response = await self.aclient.post(
                 url, json=session.dict(exclude_none=True)
             )
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
-        self._handle_response(response, f"Failed to add session {session.session_id}")
+        handle_response(response, f"Failed to add session {session.session_id}")
 
         return response.text
 
+    # Memory APIs : Get Memory
     def get_memory(self, session_id: str, lastn: Optional[int] = None) -> Memory:
         """
         Retrieve memory for the specified session.
 
         Parameters
         ----------
         session_id : str
@@ -349,20 +303,21 @@
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         url = f"/sessions/{session_id}/memory"
         params = self._gen_get_params(lastn)
         response = self.client.get(url, params=params)
 
-        self._handle_response(response, f"No memory found for session {session_id}")
+        handle_response(response, f"No memory found for session {session_id}")
 
         response_data = response.json()
 
         return self._parse_get_memory_response(response_data)
 
+    # Memory APIs : Get Memory Asynchronously
     async def aget_memory(self, session_id: str, lastn: Optional[int] = None) -> Memory:
         """
         Asynchronously retrieve memory for the specified session.
 
         Parameters
         ----------
         session_id : str
@@ -386,20 +341,21 @@
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         url = f"/sessions/{session_id}/memory"
         params = self._gen_get_params(lastn)
         response = await self.aclient.get(url, params=params)
 
-        self._handle_response(response, f"No memory found for session {session_id}")
+        handle_response(response, f"No memory found for session {session_id}")
 
         response_data = response.json()
 
         return self._parse_get_memory_response(response_data)
 
+    # Memory APIs : Add Memory
     def add_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
         Add memory to the specified session.
 
         Parameters
         ----------
         session_id : str
@@ -423,18 +379,19 @@
             raise ValueError("session_id must be provided")
 
         response = self.client.post(
             f"/sessions/{session_id}/memory",
             json=memory_messages.dict(exclude_none=True),
         )
 
-        self._handle_response(response)
+        handle_response(response)
 
         return response.text
 
+    # Memory APIs : Add Memory Asynchronously
     async def aadd_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
         Asynchronously add memory to the specified session.
 
         Parameters
         ----------
         session_id : str
@@ -458,18 +415,19 @@
             raise ValueError("session_id must be provided")
 
         response = await self.aclient.post(
             f"/sessions/{session_id}/memory",
             json=memory_messages.dict(exclude_none=True),
         )
 
-        self._handle_response(response)
+        handle_response(response)
 
         return response.text
 
+    # Memory APIs : Delete Memory
     def delete_memory(self, session_id: str) -> str:
         """
         Delete memory for the specified session.
 
         Parameters
         ----------
         session_id : str
@@ -487,17 +445,18 @@
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         response = self.client.delete(f"/sessions/{session_id}/memory")
-        self._handle_response(response)
+        handle_response(response)
         return response.text
 
+    # Memory APIs : Delete Memory Asynchronously
     async def adelete_memory(self, session_id: str) -> str:
         """
         Asynchronously delete memory for the specified session.
 
         Parameters
         ----------
         session_id : str
@@ -515,17 +474,18 @@
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         response = await self.aclient.delete(f"/sessions/{session_id}/memory")
-        self._handle_response(response)
+        handle_response(response)
         return response.text
 
+    # Memory APIs : Search Memory
     def search_memory(
         self,
         session_id: str,
         search_payload: MemorySearchPayload,
         limit: Optional[int] = None,
     ) -> List[MemorySearchResult]:
         """
@@ -560,19 +520,20 @@
 
         params = {"limit": limit} if limit is not None else {}
         response = self.client.post(
             f"/sessions/{session_id}/search",
             json=search_payload.dict(),
             params=params,
         )
-        self._handle_response(response)
+        handle_response(response)
         return [
             MemorySearchResult(**search_result) for search_result in response.json()
         ]
 
+    # Memory APIs : Search Memory Asynchronously
     async def asearch_memory(
         self,
         session_id: str,
         search_payload: MemorySearchPayload,
         limit: Optional[int] = None,
     ) -> List[MemorySearchResult]:
         """
@@ -607,48 +568,11 @@
 
         params = {"limit": limit} if limit is not None else {}
         response = await self.aclient.post(
             f"/sessions/{session_id}/search",
             json=search_payload.dict(),
             params=params,
         )
-        self._handle_response(response)
+        handle_response(response)
         return [
             MemorySearchResult(**search_result) for search_result in response.json()
         ]
-
-    async def aclose(self) -> None:
-        """
-        Asynchronously close the HTTP client.
-
-        [Optional] This method may be called when the ZepClient is no longer needed to
-        release resources.
-        """
-        await self.aclient.aclose()
-
-    def close(self) -> None:
-        """
-        Close the HTTP client.
-
-        [Optional] This method may be called when the ZepClient is no longer needed to
-        release resources.
-        """
-        self.client.close()
-
-
-def concat_url(base_url: str, path: str) -> str:
-    """
-    Join the specified base URL and path.
-
-    Parameters
-    ----------
-    base_url : str
-        The base URL to join.
-    path : str
-        The path to join.
-
-    Returns
-    -------
-    str
-        The joined URL.
-    """
-    return urljoin(base_url + "/", path.lstrip("/"))
```

