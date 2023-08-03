# Comparing `tmp/aiogram_widgets-1.1.0.tar.gz` & `tmp/aiogram_widgets-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram_widgets-1.1.0.tar", max compression
+gzip compressed data, was "aiogram_widgets-1.2.2.tar", max compression
```

## Comparing `aiogram_widgets-1.1.0.tar` & `aiogram_widgets-1.2.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      121 2023-08-02 15:14:30.238658 aiogram_widgets-1.1.0/aiogram_widgets/enums.py
--rw-r--r--   0        0        0       74 2023-08-02 11:45:02.390573 aiogram_widgets-1.1.0/aiogram_widgets/pagination/__init__.py
--rw-r--r--   0        0        0     4161 2023-08-02 14:50:17.801041 aiogram_widgets-1.1.0/aiogram_widgets/pagination/_base.py
--rw-r--r--   0        0        0     3091 2023-08-02 15:03:15.234777 aiogram_widgets-1.1.0/aiogram_widgets/pagination/keyboard.py
--rw-r--r--   0        0        0     3255 2023-08-02 15:03:21.200356 aiogram_widgets-1.1.0/aiogram_widgets/pagination/text.py
--rw-r--r--   0        0        0      547 2023-08-02 12:13:20.064283 aiogram_widgets-1.1.0/aiogram_widgets/types.py
--rw-r--r--   0        0        0     1088 2023-08-02 14:37:27.882686 aiogram_widgets-1.1.0/LICENSE
--rw-r--r--   0        0        0      622 2023-08-02 15:16:24.944769 aiogram_widgets-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4337 2023-08-02 14:29:45.816378 aiogram_widgets-1.1.0/README.md
--rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 aiogram_widgets-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-08-03 19:27:06.733984 aiogram_widgets-1.2.2/aiogram_widgets/__meta__.py
+-rw-r--r--   0        0        0      121 2023-08-03 20:33:55.339887 aiogram_widgets-1.2.2/aiogram_widgets/enums.py
+-rw-r--r--   0        0        0       74 2023-08-02 11:45:02.390573 aiogram_widgets-1.2.2/aiogram_widgets/pagination/__init__.py
+-rw-r--r--   0        0        0     5241 2023-08-03 20:37:59.869446 aiogram_widgets-1.2.2/aiogram_widgets/pagination/_base.py
+-rw-r--r--   0        0        0     3034 2023-08-03 20:37:38.346686 aiogram_widgets-1.2.2/aiogram_widgets/pagination/keyboard.py
+-rw-r--r--   0        0        0     3404 2023-08-03 20:33:59.637681 aiogram_widgets-1.2.2/aiogram_widgets/pagination/text.py
+-rw-r--r--   0        0        0      872 2023-08-03 20:34:01.039311 aiogram_widgets-1.2.2/aiogram_widgets/types.py
+-rw-r--r--   0        0        0     1088 2023-08-02 14:37:27.882686 aiogram_widgets-1.2.2/LICENSE
+-rw-r--r--   0        0        0      810 2023-08-03 20:40:30.095755 aiogram_widgets-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4731 2023-08-03 19:27:06.732988 aiogram_widgets-1.2.2/README.md
+-rw-r--r--   0        0        0     5206 1970-01-01 00:00:00.000000 aiogram_widgets-1.2.2/PKG-INFO
```

### Comparing `aiogram_widgets-1.1.0/aiogram_widgets/pagination/_base.py` & `aiogram_widgets-1.2.2/aiogram_widgets/pagination/_base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 from abc import ABC, abstractmethod
 from math import ceil
 from typing import Any, Dict, List
 
-from aiogram import Dispatcher, Router
-from aiogram.types import InlineKeyboardButton, InlineKeyboardMarkup
+import aiogram
+from aiogram import F, Router
+from aiogram.filters.state import StateFilter
+from aiogram.types import CallbackQuery, InlineKeyboardButton, InlineKeyboardMarkup
 from aiogram.utils.keyboard import InlineKeyboardBuilder
 
-from aiogram_widgets.types import Additional_buttons_type
+if aiogram.__version__ >= "3.0.0b8":
+    from pydantic.v1 import validate_arguments
+else:
+    from pydantic import validate_arguments
+
+from aiogram_widgets.types import AdditionalButtonsType, PaginationButtonsType
 
 
 class BasePaginator(ABC):
+    @validate_arguments(config=dict(arbitrary_types_allowed=True))
     def __init__(
         self,
         data: List[Any],
         per_page: int,
+        router: Router,
         pagination_key: str,
-        router: Dispatcher | Router,
-        additional_buttons: Additional_buttons_type | None = None,
+        pagination_buttons: PaginationButtonsType = ["⏪", "⬅️", "➡️", "⏩"],
+        additional_buttons: AdditionalButtonsType | None = None,
     ):
         """Base paginator class, which implements basic methods"""
         self.data = data
         self.builder = InlineKeyboardBuilder()
         self.pagination_key = pagination_key
         self.router = router
         self.additional_buttons = additional_buttons
 
         self.per_page = per_page
         self.first_page_index = 1
         self.current_page_index = self.first_page_index
         self.last_page_index = self._last_page_index
+        self.pagination_buttons = pagination_buttons
 
         self.paginator_exists: bool = self.last_page_index - self.first_page_index > 0
         self._build()
         if self.paginator_exists:
             self._register_handler()
 
     def as_builder(self) -> InlineKeyboardBuilder:
@@ -43,73 +53,87 @@
 
     @abstractmethod
     def _build(self):
         """Build a keyboard using InlineKeyboardBuilder"""
         ...
 
     @abstractmethod
-    def _register_handler(self):
-        """Register a handler for managing pagination"""
+    async def _callback_handler(self, call: CallbackQuery):
+        """Handler for pagination updates"""
         ...
 
-    @property
-    def _current_data_chunk(self) -> List[Any]:
-        start_index = (self.current_page_index - 1) * self.per_page
-        end_index = start_index + self.per_page
-        current_data_chunk = self.data[start_index:end_index]
-
-        return current_data_chunk
+    def _register_handler(self):
+        """"""
 
-    def _format_button(
-        self, button: InlineKeyboardButton | Dict[str, Any]
-    ) -> InlineKeyboardButton:
-        """Register a handler for managing pagination"""
-        return (
-            button
-            if isinstance(button, InlineKeyboardButton)
-            else InlineKeyboardButton(**button)
+        self.router.callback_query.register(
+            self._callback_handler,
+            F.data.startswith(self.pagination_key),
+            StateFilter("*"),
         )
 
     def _build_pagination_buttons(self, builder: InlineKeyboardBuilder):
         if self.paginator_exists:
             pagination_buttons: List[InlineKeyboardButton] = []
             if self.current_page_index > self.first_page_index:
-                pagination_buttons.append(
-                    InlineKeyboardButton(
-                        text="⏪",
-                        callback_data=f"{self.pagination_key}|{self.first_page_index}",
-                    ),
+                self._add_pagination_button_if_exists(
+                    button_index=0,
+                    callback_data=f"{self.pagination_key}|{self.first_page_index}",
+                    pagination_buttons=pagination_buttons,
                 )
-                pagination_buttons.append(
-                    InlineKeyboardButton(
-                        text="⬅️",
-                        callback_data=f"{self.pagination_key}|{self.current_page_index - 1}",
-                    ),
+                self._add_pagination_button_if_exists(
+                    button_index=1,
+                    callback_data=f"{self.pagination_key}|{self.current_page_index - 1}",
+                    pagination_buttons=pagination_buttons,
                 )
-
             pagination_buttons.append(
                 InlineKeyboardButton(
-                    text=str(self.current_page_index),
+                    text=f"{self.current_page_index}/{self.last_page_index}",
                     callback_data="pass",
                 )
             )
             if self.current_page_index < self.last_page_index:
-                pagination_buttons.append(
-                    InlineKeyboardButton(
-                        text="➡️",
-                        callback_data=f"{self.pagination_key}|{self.current_page_index + 1}",
-                    ),
+                self._add_pagination_button_if_exists(
+                    button_index=2,
+                    callback_data=f"{self.pagination_key}|{self.current_page_index + 1}",
+                    pagination_buttons=pagination_buttons,
                 )
-                pagination_buttons.append(
-                    InlineKeyboardButton(
-                        text="⏩",
-                        callback_data=f"{self.pagination_key}|{self.last_page_index}",
-                    ),
+                self._add_pagination_button_if_exists(
+                    button_index=3,
+                    callback_data=f"{self.pagination_key}|{self.last_page_index}",
+                    pagination_buttons=pagination_buttons,
                 )
             builder.row(*pagination_buttons)
         if self.additional_buttons:
             for button_row in self.additional_buttons:
                 builder.row(*[self._format_button(button) for button in button_row])
 
+    def _format_button(
+        self, button: InlineKeyboardButton | Dict[str, Any]
+    ) -> InlineKeyboardButton:
+        """Format button to InlineKeyboardButton"""
+        if isinstance(button, InlineKeyboardButton):
+            return button
+        return InlineKeyboardButton(**button)
+
+    def _add_pagination_button_if_exists(
+        self,
+        button_index: int,
+        callback_data: str,
+        pagination_buttons: List[InlineKeyboardButton],
+    ):
+        button_text = self.pagination_buttons[button_index]
+        if button_text is not None:
+            pagination_buttons.append(
+                InlineKeyboardButton(text=button_text, callback_data=callback_data)
+            )
+
+    @property
+    def _current_data_chunk(self) -> List[Any]:
+        start_index = (self.current_page_index - 1) * self.per_page
+        end_index = start_index + self.per_page
+        current_data_chunk = self.data[start_index:end_index]
+
+        return current_data_chunk
+
     @property
     def _last_page_index(self) -> int:
         return ceil(len(self.data) / self.per_page)
```

### Comparing `aiogram_widgets-1.1.0/aiogram_widgets/pagination/keyboard.py` & `aiogram_widgets-1.2.2/aiogram_widgets/pagination/keyboard.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,85 @@
 from typing import Annotated, List
 
-from aiogram import Dispatcher, F, Router
-from aiogram.filters.state import StateFilter
-from aiogram.types import CallbackQuery, InlineKeyboardButton
+import aiogram
+from aiogram import Router
+from aiogram.types import CallbackQuery
 from aiogram.utils.keyboard import InlineKeyboardBuilder
-from pydantic import Field, validate_arguments
+
+if aiogram.__version__ >= "3.0.0b8":
+    from pydantic.v1 import Field
+else:
+    from pydantic import Field
 
 from aiogram_widgets.pagination._base import BasePaginator
 from aiogram_widgets.types import (
-    Additional_buttons_type,
-    Button_type,
-    Pagination_key,
-    Per_page_type,
-    Per_row_type,
+    AdditionalButtonsType,
+    ButtonType,
+    PaginationButtonsType,
+    PaginationKeyType,
+    PerPageType,
+    PerRowType,
 )
 
 
 class KeyboardPaginator(BasePaginator):
     """Allows to create a new markup with keyboard pagination"""
 
-    @validate_arguments(config=dict(arbitrary_types_allowed=True))
     def __init__(
         self,
-        data: Annotated[List[Button_type], Field(min_items=1)],
-        router: Dispatcher | Router,
-        additional_buttons: Additional_buttons_type | None = None,
-        pagination_key: Pagination_key = "keyboard_paginated",
-        per_row: Per_row_type = 2,
-        per_page: Per_page_type = 10,
+        data: Annotated[List[ButtonType], Field(min_items=1)],
+        router: Router,
+        additional_buttons: AdditionalButtonsType | None = None,
+        pagination_key: PaginationKeyType = "keyboard_paginated",
+        pagination_buttons: PaginationButtonsType = ["⏪", "⬅️", "➡️", "⏩"],
+        per_row: PerRowType = 2,
+        per_page: PerPageType = 10,
     ):
         """
         :param data - buttons data. (`required`)
         >>> data = [
             {
                 "text": "Button name",
                 "callback_data": "callback_data",
             },
-            InlineKeyboardButton(text="Button name 2", callback_data="callback_data_2"),
+            InlineKeyboardButton(
+                text="Button name 2", callback_data="callback_data_2"
+            ),
             {
                 "text": "Button name 999",
                 "callback_data": "callback_data_999",
             },
         ]
 
         :param router: pagination automatization. (`required`)
         :param additional_buttons: provide additional buttons, that will be inserted after pagination panel. `(default=None)`
         :param pagination_key: callback data, which will be attached to the callback of each pagination button `(default="text_paginated")`
+        :param pagination_buttons: list of `four` buttons, where each is a string or None (if you don't want to add this button) `(default=["⏪", "⬅️", "➡️", "⏩"])`
         :param per_row: amount of items per row `(default=2)`
         :param per_page: amount of items per page `(default=10)`
         """
         self.per_row = per_row
-        super().__init__(data, per_page, pagination_key, router, additional_buttons)
+        super().__init__(
+            data=data,
+            router=router,
+            additional_buttons=additional_buttons,
+            pagination_key=pagination_key,
+            pagination_buttons=pagination_buttons,
+            per_page=per_page,
+        )
 
     def _build(self):
         self.builder = InlineKeyboardBuilder()
 
         for button in self._current_data_chunk:
             button = self._format_button(button)
             self.builder.add(button)
 
         self.builder.adjust(self.per_row)
 
         self._build_pagination_buttons(self.builder)
 
-    def _register_handler(self):
-        """"""
+    async def _callback_handler(self, call: CallbackQuery):
+        self.current_page_index = int(call.data.split("|")[-1])
+        self._build()
 
-        async def __callback_handler(call: CallbackQuery):
-            self.current_page_index = int(call.data.split("|")[-1])
-            self._build()
-
-            await call.message.edit_reply_markup(reply_markup=self.as_markup())
-
-        self.router.callback_query.register(
-            __callback_handler,
-            F.data.startswith(self.pagination_key),
-            StateFilter("*"),
-        )
-
-    def _format_button(self, button: Button_type) -> InlineKeyboardButton:
-        return (
-            InlineKeyboardButton(**button)
-            if not isinstance(button, InlineKeyboardButton)
-            else button
-        )
+        await call.message.edit_reply_markup(reply_markup=self.as_markup())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiogram_widgets-1.1.0/aiogram_widgets/pagination/text.py` & `aiogram_widgets-1.2.2/aiogram_widgets/pagination/text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 from typing import Annotated, List
 
-from aiogram import Dispatcher, F, Router
-from aiogram.filters.state import StateFilter
+import aiogram
+from aiogram import Router
 from aiogram.types import CallbackQuery, InlineKeyboardMarkup
 from aiogram.utils.keyboard import InlineKeyboardBuilder
-from pydantic import Field, PositiveInt, validate_arguments
+
+if aiogram.__version__ >= "3.0.0b8":
+    from pydantic.v1 import Field
+else:
+    from pydantic import Field
 
 from aiogram_widgets.pagination._base import BasePaginator
-from aiogram_widgets.types import Additional_buttons_type, Pagination_key
+from aiogram_widgets.types import (
+    AdditionalButtonsType,
+    PaginationButtonsType,
+    PaginationKeyType,
+    PerPageType,
+)
 
 
 class TextPaginator(BasePaginator):
     """Allows to create a new markup with text pagination"""
 
-    @validate_arguments(config=dict(arbitrary_types_allowed=True))
     def __init__(
         self,
         data: Annotated[List[str], Field(min_items=1)],
-        router: Dispatcher | Router,
+        router: Router,
         data_joiner: str = "\n",
-        additional_buttons: Additional_buttons_type | None = None,
-        pagination_key: Pagination_key = "text_paginated",
-        per_page: PositiveInt = 10,
+        additional_buttons: AdditionalButtonsType | None = None,
+        pagination_key: PaginationKeyType = "text_paginated",
+        pagination_buttons: PaginationButtonsType = ["⏪", "⬅️", "➡️", "⏩"],
+        per_page: PerPageType = 10,
     ):
         """
         :param data: list of text chunks (`required`)
         >>> data = [
             [
                         "Text number 1",
                         "Text number 2",
@@ -35,50 +44,49 @@
             ],
         ]
 
         :param router: pagination automatization. (`required`)
         :param data_joiner: string, which will `join` current text chunk to one text `(default=new string)`
         :param additional_buttons: provide additional buttons, that will be inserted after pagination panel. `(default=None)`
         :param pagination_key: callback data, which will be attached to the callback of each pagination button `(default="text_paginated")`
+        :param pagination_buttons: list of `four` buttons, where each is a string or None (if you don't want to add this button) `(default=["⏪", "⬅️", "➡️", "⏩"])`
         :param per_page: amount of items per page `(default=10)`
         """
-        super().__init__(data, per_page, pagination_key, router, additional_buttons)
+        super().__init__(
+            data=data,
+            router=router,
+            additional_buttons=additional_buttons,
+            pagination_key=pagination_key,
+            pagination_buttons=pagination_buttons,
+            per_page=per_page,
+        )
         self.data_joiner = data_joiner
 
     def _build(self):
         self.builder = InlineKeyboardBuilder()
         self._build_pagination_buttons(self.builder)
 
-    def _register_handler(self):
-        """"""
-
-        async def __callback_handler(call: CallbackQuery):
-            self.current_page_index = int(call.data.split("|")[-1])
-            self._build()
-
-            text, reply_markup = (
-                self._format_data_chunk(),
-                self.as_markup(),
-            )
-            if call.message.caption:
-                await call.message.edit_caption(
-                    caption=text,
-                    reply_markup=reply_markup,
-                    disable_web_page_preview=True,
-                )
-            else:
-                await call.message.edit_text(
-                    text=text, reply_markup=reply_markup, disable_web_page_preview=True
-                )
-
-        self.router.callback_query.register(
-            __callback_handler,
-            F.data.startswith(self.pagination_key),
-            StateFilter("*"),
+    async def _callback_handler(self, call: CallbackQuery):
+        self.current_page_index = int(call.data.split("|")[-1])
+        self._build()
+
+        text, reply_markup = (
+            self._format_data_chunk(),
+            self.as_markup(),
         )
+        if call.message.caption:
+            await call.message.edit_caption(
+                caption=text,
+                reply_markup=reply_markup,
+                disable_web_page_preview=True,
+            )
+        else:
+            await call.message.edit_text(
+                text=text, reply_markup=reply_markup, disable_web_page_preview=True
+            )
 
     @property
     def current_message_data(self) -> tuple[str, InlineKeyboardMarkup]:
         return self._format_data_chunk(), self.as_markup()
 
     def _format_data_chunk(self) -> str:
         return self.data_joiner.join(self._current_data_chunk)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiogram_widgets-1.1.0/LICENSE` & `aiogram_widgets-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-1.1.0/pyproject.toml` & `aiogram_widgets-1.2.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "aiogram-widgets"
-version = "1.1.0"
-description = ""
-authors = ["ggindinson"]
+version = "1.2.2"
 readme = "README.md"
+description = "Create most popular widgets for aiogram 3 in few code lines "
+keywords = ["aiogram", "telegram api", "pagination", "calendar", "checkbox", "multiselect", "templates"]
+authors = ["ggindinson"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 packages = [{include = "aiogram_widgets"}]
 
+
 [project.urls]
 "Homepage" = "https://github.com/ggindinson/aiogram-widgets"
 "PyPI" = "https://pypi.python.org/pypi/aiogram_widgets/"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aiogram = "^3.0.0b6"
-
+aiogram = "3.0.0b7"
+pydantic = ">=1.10.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

