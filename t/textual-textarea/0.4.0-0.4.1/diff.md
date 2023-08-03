# Comparing `tmp/textual_textarea-0.4.0.tar.gz` & `tmp/textual_textarea-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_textarea-0.4.0.tar", max compression
+gzip compressed data, was "textual_textarea-0.4.1.tar", max compression
```

## Comparing `textual_textarea-0.4.0.tar` & `textual_textarea-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1068 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/LICENSE
--rw-r--r--   0        0        0     5062 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/README.md
--rw-r--r--   0        0        0     1555 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      170 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/__init__.py
--rw-r--r--   0        0        0      491 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/__main__.py
--rw-r--r--   0        0        0     1028 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/colors.py
--rw-r--r--   0        0        0     3510 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/comments.py
--rw-r--r--   0        0        0     1091 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/containers.py
--rw-r--r--   0        0        0     2021 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/error_modal.py
--rw-r--r--   0        0        0     3374 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/key_handlers.py
--rw-r--r--   0        0        0      681 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/messages.py
--rw-r--r--   0        0        0     3057 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/path_input.py
--rw-r--r--   0        0        0        0 2023-08-03 17:08:32.543686 textual_textarea-0.4.0/src/textual_textarea/py.typed
--rw-r--r--   0        0        0      450 2023-08-03 17:08:32.547686 textual_textarea-0.4.0/src/textual_textarea/serde.py
--rw-r--r--   0        0        0    31761 2023-08-03 17:08:32.547686 textual_textarea-0.4.0/src/textual_textarea/textarea.py
--rw-r--r--   0        0        0     6019 1970-01-01 00:00:00.000000 textual_textarea-0.4.0/setup.py
--rw-r--r--   0        0        0     5860 1970-01-01 00:00:00.000000 textual_textarea-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-03 18:15:41.757434 textual_textarea-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5062 2023-08-03 18:15:41.757434 textual_textarea-0.4.1/README.md
+-rw-r--r--   0        0        0     1555 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/__init__.py
+-rw-r--r--   0        0        0      491 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/__main__.py
+-rw-r--r--   0        0        0     1028 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/colors.py
+-rw-r--r--   0        0        0     3510 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/comments.py
+-rw-r--r--   0        0        0     1091 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/containers.py
+-rw-r--r--   0        0        0     2021 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/error_modal.py
+-rw-r--r--   0        0        0     3374 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/key_handlers.py
+-rw-r--r--   0        0        0      681 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/messages.py
+-rw-r--r--   0        0        0     3299 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/path_input.py
+-rw-r--r--   0        0        0        0 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/py.typed
+-rw-r--r--   0        0        0      450 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/serde.py
+-rw-r--r--   0        0        0    31775 2023-08-03 18:15:41.761434 textual_textarea-0.4.1/src/textual_textarea/textarea.py
+-rw-r--r--   0        0        0     6019 1970-01-01 00:00:00.000000 textual_textarea-0.4.1/setup.py
+-rw-r--r--   0        0        0     5860 1970-01-01 00:00:00.000000 textual_textarea-0.4.1/PKG-INFO
```

### Comparing `textual_textarea-0.4.0/LICENSE` & `textual_textarea-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.4.0/README.md` & `textual_textarea-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.4.0/pyproject.toml` & `textual_textarea-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textual-textarea"
-version = "0.4.0"
+version = "0.4.1"
 description = "A text area (multi-line input) with syntax highlighting for Textual"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/tconbeer/textual-textarea"
 repository = "https://github.com/tconbeer/textual-textarea"
 readme = "README.md"
 packages = [{ include = "textual_textarea", from = "src" }]
```

### Comparing `textual_textarea-0.4.0/src/textual_textarea/colors.py` & `textual_textarea-0.4.1/src/textual_textarea/colors.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.4.0/src/textual_textarea/comments.py` & `textual_textarea-0.4.1/src/textual_textarea/comments.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.4.0/src/textual_textarea/containers.py` & `textual_textarea-0.4.1/src/textual_textarea/containers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.4.0/src/textual_textarea/error_modal.py` & `textual_textarea-0.4.1/src/textual_textarea/error_modal.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.4.0/src/textual_textarea/key_handlers.py` & `textual_textarea-0.4.1/src/textual_textarea/key_handlers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.4.0/src/textual_textarea/messages.py` & `textual_textarea-0.4.1/src/textual_textarea/messages.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.4.0/src/textual_textarea/path_input.py` & `textual_textarea-0.4.1/src/textual_textarea/path_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,15 +81,17 @@
         name: Union[str, None] = None,
         id: Union[str, None] = None,
         classes: Union[str, None] = None,
         disabled: bool = False,
         dir_okay: bool = True,
         file_okay: bool = True,
         must_exist: bool = False,
+        tab_advances_focus: bool = False,
     ) -> None:
+        self.tab_advances_focus = tab_advances_focus
         super().__init__(
             value,
             placeholder,
             highlighter,
             password,
             suggester=PathSuggester(),
             validators=PathValidator(dir_okay, file_okay, must_exist),
@@ -99,8 +101,11 @@
             disabled=disabled,
         )
 
     def action_cancel(self) -> None:
         self.post_message(CancelPathInput())
 
     def action_complete(self) -> None:
-        self.action_cursor_right()
+        if self._suggestion and self._suggestion != self.value:
+            self.action_cursor_right()
+        elif self.tab_advances_focus:
+            self.app.action_focus_next()
```

### Comparing `textual_textarea-0.4.0/src/textual_textarea/textarea.py` & `textual_textarea-0.4.1/src/textual_textarea/textarea.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,19 +34,14 @@
 class TextInput(Static, can_focus=True):
     DEFAULT_CSS = """
         TextInput {
             height: auto;
             width: auto;
             padding: 0 1;
         }
-        #validation_label {
-            color: red;
-            text-style: italic;
-            margin: 0 0 0 3;
-        }
     """
 
     lines: reactive[List[str]] = reactive(lambda: list(" "))
     cursor: reactive[Cursor] = reactive(Cursor(0, 0))
     selection_anchor: reactive[Union[Cursor, None]] = reactive(None)
     clipboard: List[str] = list()
     cursor_visible: reactive[bool] = reactive(True)
@@ -569,14 +564,22 @@
         language (str): Must be the short name of a Pygments lexer
             (https://pygments.org/docs/lexers/), e.g., "python", "sql", "as3".
         theme (str): Must be name of a Pygments style (https://pygments.org/styles/),
             e.g., "bw", "github-dark", "solarized-light".
         theme_colors (WidgetColors): The colors extracted from the theme.
     """
 
+    DEFAULT_CSS = """
+    #validation_label {
+        color: $error;
+        text-style: italic;
+        margin: 0 0 0 3;
+    }
+    """
+
     BINDINGS = [
         Binding("ctrl+s", "save", "Save Query"),
         Binding("ctrl+o", "load", "Open Query"),
         Binding("ctrl+q", "quit", "Quit"),
     ]
 
     def __init__(
```

### Comparing `textual_textarea-0.4.0/setup.py` & `textual_textarea-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyperclip>=1.8.2,<2.0.0', 'textual>=0.27.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'textual-textarea',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'A text area (multi-line input) with syntax highlighting for Textual',
     'long_description': '# Textual Textarea\n![Textual Textarea Screenshot](textarea.png)\n\n## Installation\n\n```\npip install textual-textarea\n```\n\n## Features\nFull-featured text editor experience with VS-Code-like bindings, in your Textual App:\n- Syntax highlighting and support for themes.\n- Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>Home/End</kbd>).\n- Select text using <kbd>shift</kbd> or click and drag.\n- Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.\n- Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.\n- Comment selections with <kbd>ctrl+/</kbd>.\n- Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.\n- Automatic completions of quotes and brackets.\n- Quit with <kbd>ctrl+q</kbd>.\n\n## Usage\n\n### Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="solarized-dark")\n\n    def on_mount(self) -> None:\n        ta = self.query_one(TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts three additional, optional arguments when initializing the widget:\n\n- language (str): Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to `None`.\n- theme (str): Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n- use_system_clipboard (bool): Set to `False` to make the TextArea\'s copy and paste operations ignore the system clipboard. Defaults to `True`. Some Linux users may need to apt-install `xclip` or `xsel` to enable the system clipboard features.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n### Interacting with the Widget\n\n#### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\nSimilarly, the TextArea exposes a `selected_text` property (read-only):\n```python\nta = self.query_one(TextArea)\nselection = ta.selected_text\n```\n\n#### Getting and Setting The Cursor Position\n\nThe TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):\n\n```python\nta = self.query_one(TextArea)\nold_cursor = ta.cursor\nta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible\ncursor_line_number = ta.cursor.lno\ncursor_x_position = ta.cursor.pos\n```\n\nSimilarly, there is a `selection_anchor` property (`Union[None, Cursor]`):\n\n```python\nta = self.query_one(TextArea)\nanchor = ta.selection_anchor # will be None if no text is selected\nta.selection_anchor = (999, 0)  # the anchor will move as close to line 999, pos 0 as possible\nta.selection_anchor = None # the selection will be cleared\n```\n\n#### Getting and Setting The Language\n\nSyntax highlighting and comment insertion depends on the configured language for the TextArea.\n\nThe TextArea exposes a `language` property that returns `None` or a string that is equal to the short name of the [Pygments lexer](https://pygments.org/docs/lexers/) for the currently configured language:\n\n```python\nta = self.query_one(TextArea)\nold_language = ta.language\nta.language = "python"\n```\n\n#### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\n\n#### Adding Bindings and other Behavior\n\nYou can subclass TextArea to add your own behavior. This snippet adds an action that posts a Submitted message containing the text of the TextArea when the user presses <kbd>ctrl+j</kbd>:\n\n```python\nfrom textual.message import Message\nfrom textual_textarea import TextArea\n\n\nclass CodeEditor(TextArea):\n    BINDINGS = [\n        ("ctrl+j", "submit", "Run Query"),\n    ]\n\n    class Submitted(Message, bubble=True):\n        def __init__(self, text: str) -> None:\n            super().__init__()\n            self.text = text\n\n    async def action_submit(self) -> None:\n        self.post_message(self.Submitted(self.text))\n```\n',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tconbeer/textual-textarea',
```

### Comparing `textual_textarea-0.4.0/PKG-INFO` & `textual_textarea-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-textarea
-Version: 0.4.0
+Version: 0.4.1
 Summary: A text area (multi-line input) with syntax highlighting for Textual
 Home-page: https://github.com/tconbeer/textual-textarea
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

