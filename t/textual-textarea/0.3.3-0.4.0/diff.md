# Comparing `tmp/textual_textarea-0.3.3.tar.gz` & `tmp/textual_textarea-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_textarea-0.3.3.tar", max compression
+gzip compressed data, was "textual_textarea-0.4.0.tar", max compression
```

## Comparing `textual_textarea-0.3.3.tar` & `textual_textarea-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1068 2023-07-28 21:27:04.660127 textual_textarea-0.3.3/LICENSE
--rw-r--r--   0        0        0     4575 2023-07-28 21:27:04.660127 textual_textarea-0.3.3/README.md
--rw-r--r--   0        0        0     1555 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       71 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/__init__.py
--rw-r--r--   0        0        0      491 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/__main__.py
--rw-r--r--   0        0        0      175 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/cancellable_input.py
--rw-r--r--   0        0        0     1028 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/colors.py
--rw-r--r--   0        0        0     3510 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/comments.py
--rw-r--r--   0        0        0     1091 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/containers.py
--rw-r--r--   0        0        0     2021 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/error_modal.py
--rw-r--r--   0        0        0     3374 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/key_handlers.py
--rw-r--r--   0        0        0      681 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/messages.py
--rw-r--r--   0        0        0        0 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/py.typed
--rw-r--r--   0        0        0      450 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/serde.py
--rw-r--r--   0        0        0    28729 2023-07-28 21:27:04.664127 textual_textarea-0.3.3/src/textual_textarea/textarea.py
--rw-r--r--   0        0        0     5518 1970-01-01 00:00:00.000000 textual_textarea-0.3.3/setup.py
--rw-r--r--   0        0        0     5373 1970-01-01 00:00:00.000000 textual_textarea-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5062 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/README.md
+-rw-r--r--   0        0        0     1555 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/__init__.py
+-rw-r--r--   0        0        0      491 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/__main__.py
+-rw-r--r--   0        0        0     1028 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/colors.py
+-rw-r--r--   0        0        0     3510 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/comments.py
+-rw-r--r--   0        0        0     1091 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/containers.py
+-rw-r--r--   0        0        0     2021 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/error_modal.py
+-rw-r--r--   0        0        0     3374 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/key_handlers.py
+-rw-r--r--   0        0        0      681 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/messages.py
+-rw-r--r--   0        0        0     3057 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/path_input.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/py.typed
+-rw-r--r--   0        0        0      450 2023-08-03 17:08:32.547686 textual_textarea-0.4.0/src/textual_textarea/serde.py
+-rw-r--r--   0        0        0    31761 2023-08-03 17:08:32.547686 textual_textarea-0.4.0/src/textual_textarea/textarea.py
+-rw-r--r--   0        0        0     6019 1970-01-01 00:00:00.000000 textual_textarea-0.4.0/setup.py
+-rw-r--r--   0        0        0     5860 1970-01-01 00:00:00.000000 textual_textarea-0.4.0/PKG-INFO
```

### Comparing `textual_textarea-0.3.3/LICENSE` & `textual_textarea-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.3/README.md` & `textual_textarea-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -59,27 +59,41 @@
 
 ```python
 ta = self.query_one(TextArea)
 old_text = ta.text
 ta.text = "New Text!\n\nMany Lines!"
 ```
 
+Similarly, the TextArea exposes a `selected_text` property (read-only):
+```python
+ta = self.query_one(TextArea)
+selection = ta.selected_text
+```
 
 #### Getting and Setting The Cursor Position
 
 The TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):
 
 ```python
 ta = self.query_one(TextArea)
 old_cursor = ta.cursor
 ta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible
 cursor_line_number = ta.cursor.lno
 cursor_x_position = ta.cursor.pos
 ```
 
+Similarly, there is a `selection_anchor` property (`Union[None, Cursor]`):
+
+```python
+ta = self.query_one(TextArea)
+anchor = ta.selection_anchor # will be None if no text is selected
+ta.selection_anchor = (999, 0)  # the anchor will move as close to line 999, pos 0 as possible
+ta.selection_anchor = None # the selection will be cleared
+```
+
 #### Getting and Setting The Language
 
 Syntax highlighting and comment insertion depends on the configured language for the TextArea.
 
 The TextArea exposes a `language` property that returns `None` or a string that is equal to the short name of the [Pygments lexer](https://pygments.org/docs/lexers/) for the currently configured language:
 
 ```python
```

### Comparing `textual_textarea-0.3.3/pyproject.toml` & `textual_textarea-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "textual-textarea"
-version = "0.3.3"
+version = "0.4.0"
 description = "A text area (multi-line input) with syntax highlighting for Textual"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/tconbeer/textual-textarea"
 repository = "https://github.com/tconbeer/textual-textarea"
 readme = "README.md"
 packages = [{ include = "textual_textarea", from = "src" }]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-textual = ">=0.21.0, <1.0.0"
+textual = ">=0.27.0, <1.0.0"
 pyperclip = "^1.8.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
-textual = {version="0.21.0", extras=["dev"]}
+textual = {version="0.27.0", extras=["dev"]}
 
 [tool.poetry.group.static.dependencies]
 black = "^23.3.0"
-ruff = ">=0.0.264,<0.0.281"
+ruff = ">=0.0.264,<0.0.283"
 mypy = "^1.2.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 
 [tool.ruff]
```

### Comparing `textual_textarea-0.3.3/src/textual_textarea/colors.py` & `textual_textarea-0.4.0/src/textual_textarea/colors.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.3/src/textual_textarea/comments.py` & `textual_textarea-0.4.0/src/textual_textarea/comments.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.3/src/textual_textarea/containers.py` & `textual_textarea-0.4.0/src/textual_textarea/containers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.3/src/textual_textarea/error_modal.py` & `textual_textarea-0.4.0/src/textual_textarea/error_modal.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.3/src/textual_textarea/key_handlers.py` & `textual_textarea-0.4.0/src/textual_textarea/key_handlers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.3/src/textual_textarea/messages.py` & `textual_textarea-0.4.0/src/textual_textarea/messages.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.3/src/textual_textarea/textarea.py` & `textual_textarea-0.4.0/src/textual_textarea/textarea.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 from rich.style import Style
 from rich.syntax import Syntax
 from textual import events
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.reactive import reactive
 from textual.widget import Widget
-from textual.widgets import Input, Static
+from textual.widgets import Input, Label, Static
 
-from textual_textarea.cancellable_input import CancellableInput
 from textual_textarea.colors import WidgetColors
 from textual_textarea.comments import INLINE_MARKERS
 from textual_textarea.containers import FooterContainer, TextContainer
 from textual_textarea.error_modal import ErrorModal
 from textual_textarea.key_handlers import Cursor, handle_arrow
 from textual_textarea.messages import TextAreaCursorMoved, TextAreaScrollOne
+from textual_textarea.path_input import PathInput
 from textual_textarea.serde import deserialize_lines, serialize_lines
 
 BRACKETS = {
     "(": ")",
     "[": "]",
     "{": "}",
 }
@@ -34,14 +34,19 @@
 class TextInput(Static, can_focus=True):
     DEFAULT_CSS = """
         TextInput {
             height: auto;
             width: auto;
             padding: 0 1;
         }
+        #validation_label {
+            color: red;
+            text-style: italic;
+            margin: 0 0 0 3;
+        }
     """
 
     lines: reactive[List[str]] = reactive(lambda: list(" "))
     cursor: reactive[Cursor] = reactive(Cursor(0, 0))
     selection_anchor: reactive[Union[Cursor, None]] = reactive(None)
     clipboard: List[str] = list()
     cursor_visible: reactive[bool] = reactive(True)
@@ -532,19 +537,30 @@
     def _get_character_before_cursor(self, cursor: Cursor) -> Union[str, None]:
         if self.cursor.pos == 0:
             return None
         else:
             return self.lines[cursor.lno][cursor.pos - 1]
 
     def move_cursor(self, x: int, y: int) -> None:
+        self.cursor = self._get_valid_cursor(x, y)
+        self.update(self._content)
+
+    def move_selection_anchor(self, x: int, y: int) -> None:
+        self.selection_anchor = self._get_valid_cursor(x, y)
+        self.update(self._content)
+
+    def _get_valid_cursor(self, x: int, y: int) -> Cursor:
         max_y = len(self.lines) - 1
         safe_y = max(0, min(max_y, y))
         max_x = len(self.lines[safe_y]) - 1
         safe_x = max(0, min(max_x, x))
-        self.cursor = Cursor(lno=safe_y, pos=safe_x)
+        return Cursor(lno=safe_y, pos=safe_x)
+
+    def clear_selection_anchor(self) -> None:
+        self.selection_anchor = None
         self.update(self._content)
 
 
 class TextArea(Widget, can_focus=True, can_focus_children=False):
     """
     A Widget that presents a feature-rich, multiline text editor interface.
 
@@ -607,14 +623,31 @@
             contents (str): A string (optionally containing newlines) to
                 set the contents of the TextArea equal to.
         """
         self.text_input.move_cursor(0, 0)
         self.text_input.lines = deserialize_lines(contents)
 
     @property
+    def selected_text(self) -> str:
+        """
+        Returns:
+            str: The contents of the TextArea between the selection
+            anchor and the cursor. Returns an empty string if the
+            selection anchor is not set.
+        """
+        anchor = self.text_input.selection_anchor
+        if anchor is None:
+            return ""
+        else:
+            lines, first, last = self.text_input._get_selected_lines(anchor)
+            lines[-1] = lines[-1][: last.pos]
+            lines[0] = lines[0][first.pos :]
+            return serialize_lines(lines)
+
+    @property
     def cursor(self) -> Cursor:
         """
         Returns
             Cursor: The location of the cursor in the TextInput
         """
         return self.text_input.cursor
 
@@ -624,14 +657,35 @@
         Args:
             cursor (Union[Cursor, Tuple[int, int]]): The position (line number, pos)
             to move the cursor to
         """
         self.text_input.move_cursor(cursor[1], cursor[0])
 
     @property
+    def selection_anchor(self) -> Union[Cursor, None]:
+        """
+        Returns
+            Cursor: The location of the selection anchor in the TextInput
+        """
+        return self.text_input.selection_anchor
+
+    @selection_anchor.setter
+    def selection_anchor(self, cursor: Union[Cursor, Tuple[int, int], None]) -> None:
+        """
+        Args:
+            cursor (Union[Cursor, Tuple[int, int], None]): The position
+            (line number, pos) to move the selection anchor to, or None
+            to clear the selection.
+        """
+        if cursor is None:
+            self.text_input.clear_selection_anchor()
+        else:
+            self.text_input.move_selection_anchor(cursor[1], cursor[0])
+
+    @property
     def language(self) -> Union[str, None]:
         """
         Returns
             str | None: The Pygments short name of the active language
         """
         return self.text_input.language
 
@@ -646,35 +700,62 @@
     def compose(self) -> ComposeResult:
         with TextContainer():
             yield TextInput(
                 language=self._language,
                 theme=self.theme,
                 theme_colors=self.theme_colors,
             )
-        yield FooterContainer(theme_colors=self.theme_colors)
+        with FooterContainer(theme_colors=self.theme_colors):
+            yield Label("", id="validation_label")
 
     def on_mount(self) -> None:
         self.styles.background = self.theme_colors.bgcolor
         self.text_container = self.query_one(TextContainer)
         self.text_input = self.query_one(TextInput)
         self.footer = self.query_one(FooterContainer)
 
     def on_focus(self) -> None:
         self.text_input.focus()
 
+    def on_click(self) -> None:
+        self.text_input.focus()
+
     def action_save(self) -> None:
+        self._clear_footer_input()
         self._mount_footer_input("save")
 
     def action_load(self) -> None:
+        self._clear_footer_input()
         self._mount_footer_input("open")
 
+    def _clear_footer_input(self) -> None:
+        try:
+            self.footer.query_one(PathInput).remove()
+        except Exception:
+            pass
+        try:
+            self.footer.query_one(Label).update("")
+        except Exception:
+            pass
+
+    def on_cancel_path_input(self) -> None:
+        self._clear_footer_input()
+
     def _mount_footer_input(self, name: str) -> None:
-        input = CancellableInput(
+        if name == "open":
+            file_okay, dir_okay, must_exist = True, False, True
+        else:
+            file_okay, dir_okay, must_exist = True, False, False
+
+        input = PathInput(
             id=f"textarea__{name}_input",
             placeholder=f"{name.capitalize()}: Enter file path OR press ESC to cancel",
+            file_okay=file_okay,
+            dir_okay=dir_okay,
+            must_exist=must_exist,
         )
         input.styles.background = self.theme_colors.bgcolor
         input.styles.border = "round", self.theme_colors.contrast_text_color
         input.styles.color = self.theme_colors.contrast_text_color
         self.footer.mount(input)
         input.focus()
 
@@ -712,14 +793,22 @@
         event.stop()
         offset = 1 if event.direction == "down" else -1
         self.text_container.scroll_to(
             self.text_container.window_region.x,
             self.text_container.window_region.y + offset,
         )
 
+    def on_input_changed(self, message: Input.Changed) -> None:
+        if message.input.id in ("textarea__save_input", "textarea__open_input"):
+            label = self.footer.query_one(Label)
+            if message.validation_result and not message.validation_result.is_valid:
+                label.update(";".join(message.validation_result.failure_descriptions))
+            else:
+                label.update("")
+
     def on_input_submitted(self, message: Input.Submitted) -> None:
         """
         Handle the submit event for the Save and Open modals.
         """
         expanded_path = expanduser(message.input.value)
         if message.input.id == "textarea__save_input":
             try:
@@ -747,10 +836,10 @@
                             "There was an error when attempting to open your file:"
                         ),
                         error=e,
                     )
                 )
             else:
                 self.text = contents
-        message.input.remove()
+        self._clear_footer_input()
         self.text_input.update(self.text_input._content)
         self.text_input.focus()
```

### Comparing `textual_textarea-0.3.3/setup.py` & `textual_textarea-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 packages = \
 ['textual_textarea']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pyperclip>=1.8.2,<2.0.0', 'textual>=0.21.0,<1.0.0']
+['pyperclip>=1.8.2,<2.0.0', 'textual>=0.27.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'textual-textarea',
-    'version': '0.3.3',
+    'version': '0.4.0',
     'description': 'A text area (multi-line input) with syntax highlighting for Textual',
-    'long_description': '# Textual Textarea\n![Textual Textarea Screenshot](textarea.png)\n\n## Installation\n\n```\npip install textual-textarea\n```\n\n## Features\nFull-featured text editor experience with VS-Code-like bindings, in your Textual App:\n- Syntax highlighting and support for themes.\n- Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>Home/End</kbd>).\n- Select text using <kbd>shift</kbd> or click and drag.\n- Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.\n- Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.\n- Comment selections with <kbd>ctrl+/</kbd>.\n- Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.\n- Automatic completions of quotes and brackets.\n- Quit with <kbd>ctrl+q</kbd>.\n\n## Usage\n\n### Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="solarized-dark")\n\n    def on_mount(self) -> None:\n        ta = self.query_one(TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts three additional, optional arguments when initializing the widget:\n\n- language (str): Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to `None`.\n- theme (str): Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n- use_system_clipboard (bool): Set to `False` to make the TextArea\'s copy and paste operations ignore the system clipboard. Defaults to `True`. Some Linux users may need to apt-install `xclip` or `xsel` to enable the system clipboard features.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n### Interacting with the Widget\n\n#### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\n\n#### Getting and Setting The Cursor Position\n\nThe TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):\n\n```python\nta = self.query_one(TextArea)\nold_cursor = ta.cursor\nta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible\ncursor_line_number = ta.cursor.lno\ncursor_x_position = ta.cursor.pos\n```\n\n#### Getting and Setting The Language\n\nSyntax highlighting and comment insertion depends on the configured language for the TextArea.\n\nThe TextArea exposes a `language` property that returns `None` or a string that is equal to the short name of the [Pygments lexer](https://pygments.org/docs/lexers/) for the currently configured language:\n\n```python\nta = self.query_one(TextArea)\nold_language = ta.language\nta.language = "python"\n```\n\n#### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\n\n#### Adding Bindings and other Behavior\n\nYou can subclass TextArea to add your own behavior. This snippet adds an action that posts a Submitted message containing the text of the TextArea when the user presses <kbd>ctrl+j</kbd>:\n\n```python\nfrom textual.message import Message\nfrom textual_textarea import TextArea\n\n\nclass CodeEditor(TextArea):\n    BINDINGS = [\n        ("ctrl+j", "submit", "Run Query"),\n    ]\n\n    class Submitted(Message, bubble=True):\n        def __init__(self, text: str) -> None:\n            super().__init__()\n            self.text = text\n\n    async def action_submit(self) -> None:\n        self.post_message(self.Submitted(self.text))\n```\n',
+    'long_description': '# Textual Textarea\n![Textual Textarea Screenshot](textarea.png)\n\n## Installation\n\n```\npip install textual-textarea\n```\n\n## Features\nFull-featured text editor experience with VS-Code-like bindings, in your Textual App:\n- Syntax highlighting and support for themes.\n- Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>Home/End</kbd>).\n- Select text using <kbd>shift</kbd> or click and drag.\n- Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.\n- Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.\n- Comment selections with <kbd>ctrl+/</kbd>.\n- Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.\n- Automatic completions of quotes and brackets.\n- Quit with <kbd>ctrl+q</kbd>.\n\n## Usage\n\n### Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="solarized-dark")\n\n    def on_mount(self) -> None:\n        ta = self.query_one(TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts three additional, optional arguments when initializing the widget:\n\n- language (str): Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to `None`.\n- theme (str): Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n- use_system_clipboard (bool): Set to `False` to make the TextArea\'s copy and paste operations ignore the system clipboard. Defaults to `True`. Some Linux users may need to apt-install `xclip` or `xsel` to enable the system clipboard features.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n### Interacting with the Widget\n\n#### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\nSimilarly, the TextArea exposes a `selected_text` property (read-only):\n```python\nta = self.query_one(TextArea)\nselection = ta.selected_text\n```\n\n#### Getting and Setting The Cursor Position\n\nThe TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):\n\n```python\nta = self.query_one(TextArea)\nold_cursor = ta.cursor\nta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible\ncursor_line_number = ta.cursor.lno\ncursor_x_position = ta.cursor.pos\n```\n\nSimilarly, there is a `selection_anchor` property (`Union[None, Cursor]`):\n\n```python\nta = self.query_one(TextArea)\nanchor = ta.selection_anchor # will be None if no text is selected\nta.selection_anchor = (999, 0)  # the anchor will move as close to line 999, pos 0 as possible\nta.selection_anchor = None # the selection will be cleared\n```\n\n#### Getting and Setting The Language\n\nSyntax highlighting and comment insertion depends on the configured language for the TextArea.\n\nThe TextArea exposes a `language` property that returns `None` or a string that is equal to the short name of the [Pygments lexer](https://pygments.org/docs/lexers/) for the currently configured language:\n\n```python\nta = self.query_one(TextArea)\nold_language = ta.language\nta.language = "python"\n```\n\n#### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\n\n#### Adding Bindings and other Behavior\n\nYou can subclass TextArea to add your own behavior. This snippet adds an action that posts a Submitted message containing the text of the TextArea when the user presses <kbd>ctrl+j</kbd>:\n\n```python\nfrom textual.message import Message\nfrom textual_textarea import TextArea\n\n\nclass CodeEditor(TextArea):\n    BINDINGS = [\n        ("ctrl+j", "submit", "Run Query"),\n    ]\n\n    class Submitted(Message, bubble=True):\n        def __init__(self, text: str) -> None:\n            super().__init__()\n            self.text = text\n\n    async def action_submit(self) -> None:\n        self.post_message(self.Submitted(self.text))\n```\n',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tconbeer/textual-textarea',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `textual_textarea-0.3.3/PKG-INFO` & `textual_textarea-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: textual-textarea
-Version: 0.3.3
+Version: 0.4.0
 Summary: A text area (multi-line input) with syntax highlighting for Textual
 Home-page: https://github.com/tconbeer/textual-textarea
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
-Requires-Dist: textual (>=0.21.0,<1.0.0)
+Requires-Dist: textual (>=0.27.0,<1.0.0)
 Project-URL: Repository, https://github.com/tconbeer/textual-textarea
 Description-Content-Type: text/markdown
 
 # Textual Textarea
 ![Textual Textarea Screenshot](textarea.png)
 
 ## Installation
@@ -79,27 +79,41 @@
 
 ```python
 ta = self.query_one(TextArea)
 old_text = ta.text
 ta.text = "New Text!\n\nMany Lines!"
 ```
 
+Similarly, the TextArea exposes a `selected_text` property (read-only):
+```python
+ta = self.query_one(TextArea)
+selection = ta.selected_text
+```
 
 #### Getting and Setting The Cursor Position
 
 The TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):
 
 ```python
 ta = self.query_one(TextArea)
 old_cursor = ta.cursor
 ta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible
 cursor_line_number = ta.cursor.lno
 cursor_x_position = ta.cursor.pos
 ```
 
+Similarly, there is a `selection_anchor` property (`Union[None, Cursor]`):
+
+```python
+ta = self.query_one(TextArea)
+anchor = ta.selection_anchor # will be None if no text is selected
+ta.selection_anchor = (999, 0)  # the anchor will move as close to line 999, pos 0 as possible
+ta.selection_anchor = None # the selection will be cleared
+```
+
 #### Getting and Setting The Language
 
 Syntax highlighting and comment insertion depends on the configured language for the TextArea.
 
 The TextArea exposes a `language` property that returns `None` or a string that is equal to the short name of the [Pygments lexer](https://pygments.org/docs/lexers/) for the currently configured language:
 
 ```python
```

