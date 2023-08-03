# Comparing `tmp/tokenstream-1.6.0.tar.gz` & `tmp/tokenstream-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenstream-1.6.0.tar", max compression
+gzip compressed data, was "tokenstream-1.7.0.tar", max compression
```

## Comparing `tokenstream-1.6.0.tar` & `tokenstream-1.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-08-02 18:51:55.545993 tokenstream-1.6.0/LICENSE
--rw-r--r--   0        0        0     7512 2023-08-02 18:51:55.545993 tokenstream-1.6.0/README.md
--rw-r--r--   0        0        0     1542 2023-08-02 18:52:44.786665 tokenstream-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      334 2023-08-02 18:52:44.762665 tokenstream-1.6.0/tokenstream/__init__.py
--rw-r--r--   0        0        0     3916 2023-08-02 18:51:55.549993 tokenstream-1.6.0/tokenstream/error.py
--rw-r--r--   0        0        0     3398 2023-08-02 18:51:55.549993 tokenstream-1.6.0/tokenstream/location.py
--rw-r--r--   0        0        0        0 2023-08-02 18:51:55.549993 tokenstream-1.6.0/tokenstream/py.typed
--rw-r--r--   0        0        0    37644 2023-08-02 18:51:55.549993 tokenstream-1.6.0/tokenstream/stream.py
--rw-r--r--   0        0        0     2729 2023-08-02 18:51:55.549993 tokenstream-1.6.0/tokenstream/token.py
--rw-r--r--   0        0        0     8225 1970-01-01 00:00:00.000000 tokenstream-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-03 00:20:29.943721 tokenstream-1.7.0/LICENSE
+-rw-r--r--   0        0        0     7512 2023-08-03 00:20:29.943721 tokenstream-1.7.0/README.md
+-rw-r--r--   0        0        0     1542 2023-08-03 00:20:50.971631 tokenstream-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-08-03 00:20:50.943632 tokenstream-1.7.0/tokenstream/__init__.py
+-rw-r--r--   0        0        0     3920 2023-08-03 00:20:29.947721 tokenstream-1.7.0/tokenstream/error.py
+-rw-r--r--   0        0        0     5967 2023-08-03 00:20:29.947721 tokenstream-1.7.0/tokenstream/location.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:20:29.947721 tokenstream-1.7.0/tokenstream/py.typed
+-rw-r--r--   0        0        0    38741 2023-08-03 00:20:29.947721 tokenstream-1.7.0/tokenstream/stream.py
+-rw-r--r--   0        0        0     2729 2023-08-03 00:20:29.947721 tokenstream-1.7.0/tokenstream/token.py
+-rw-r--r--   0        0        0     8225 1970-01-01 00:00:00.000000 tokenstream-1.7.0/PKG-INFO
```

### Comparing `tokenstream-1.6.0/LICENSE` & `tokenstream-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenstream-1.6.0/README.md` & `tokenstream-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tokenstream-1.6.0/pyproject.toml` & `tokenstream-1.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tokenstream"
-version = "1.6.0"
+version = "1.7.0"
 description = "A versatile token stream for handwritten parsers"
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/vberlier/tokenstream"
 repository = "https://github.com/vberlier/tokenstream"
 documentation = "https://github.com/vberlier/tokenstream"
```

### Comparing `tokenstream-1.6.0/tokenstream/error.py` & `tokenstream-1.7.0/tokenstream/error.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = [
     "InvalidSyntax",
     "UnexpectedEOF",
     "UnexpectedToken",
 ]
 
 
-from .location import SourceLocation
+from .location import INITIAL_LOCATION, SourceLocation
 from .token import Token, TokenPattern, explain_patterns
 
 
 class InvalidSyntax(Exception):
     """Raised when the input contains invalid syntax.
 
     Attributes
@@ -27,16 +27,16 @@
     location: SourceLocation
     end_location: SourceLocation
     alternatives: "dict[type[InvalidSyntax], list[InvalidSyntax]]"
     notes: list[str]
 
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-        self.location = SourceLocation(0, 1, 1)
-        self.end_location = SourceLocation(0, 1, 1)
+        self.location = INITIAL_LOCATION
+        self.end_location = INITIAL_LOCATION
         self.alternatives = {}
         self.notes = []
 
     def format(self, filename: str) -> str:
         """Return a string representing the error and its location in a given file.
 
         >>> try:
```

### Comparing `tokenstream-1.6.0/tokenstream/stream.py` & `tokenstream-1.7.0/tokenstream/stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 __all__ = [
     "TokenStream",
     "SyntaxRules",
+    "Preprocessor",
     "CheckpointCommit",
     "BAKED_REGEX_CACHE",
 ]
 
 import re
 from contextlib import contextmanager
 from dataclasses import dataclass, field
-from typing import Any, Callable, ContextManager, Iterable, Iterator, TypeVar, overload
+from typing import (
+    Any,
+    Callable,
+    ContextManager,
+    Iterable,
+    Iterator,
+    Sequence,
+    TypeVar,
+    overload,
+)
 
 from .error import InvalidSyntax, UnexpectedEOF, UnexpectedToken
-from .location import SourceLocation, set_location
+from .location import INITIAL_LOCATION, SourceLocation, set_location
 from .token import Token, TokenPattern
 
 T = TypeVar("T")
 
 
 SyntaxRules = tuple[tuple[str, str], ...]
 
+Preprocessor = Callable[
+    [str], tuple[str, Sequence[SourceLocation], Sequence[SourceLocation]]
+]
+
 
 def extra_field(**kwargs: Any) -> Any:
     return field(repr=False, init=False, hash=False, compare=False, **kwargs)
 
 
 @dataclass
 class CheckpointCommit:
@@ -64,16 +78,16 @@
     source
         The input string.
 
         >>> stream = TokenStream("hello world")
         >>> stream.source
         'hello world'
 
-    token_handler
-        A callback for modifying tokens before they're emitted.
+    preprocessor
+        A preprocessor that will emit source location mappings for the transformed input.
 
     syntax_rules
         A tuple of ``(token_type, pattern)`` pairs that define the recognizable tokens.
 
         >>> stream = TokenStream("hello world")
         >>> with stream.syntax(word=r"[a-z]+"):
         ...     print(stream.syntax_rules)
@@ -83,21 +97,14 @@
         The compiled regular expression generated from the syntax rules.
 
         >>> stream = TokenStream("hello world")
         >>> with stream.syntax(word=r"[a-z]+"):
         ...     print(stream.regex.pattern)
         (?P<word>[a-z]+)|(?P<newline>\r?\n)|(?P<whitespace>[ \t]+)|(?P<invalid>.+)
 
-    location
-        Tracks the position of the next token to extract in the input string.
-
-        Generally you'll probably want to use ``stream.current.location`` instead
-        because the :attr:`location` attribute doesn't roll back with checkpoints
-        and when the stream resets to a previous token.
-
     index
         The index of the current token in the list of extracted tokens.
 
         You can technically mutate this attribute directly if you want to
         reset the stream back to a specific token, but you should probably
         use the higher-level :meth:`checkpoint` method for this.
 
@@ -139,35 +146,47 @@
 
     regex_cache
         A cache that keeps a reference to the compiled regular expression associated
         to each set of syntax rules.
     """
 
     source: str
-    token_handler: Callable[[Token], Token] | None = extra_field(default=None)
     syntax_rules: SyntaxRules = extra_field(default=())
     regex: re.Pattern[str] = extra_field()
 
-    location: SourceLocation = extra_field()
+    preprocessor: Preprocessor | None = field(default=None)
+    preprocessed_source: str = extra_field()
+    source_mappings: Sequence[SourceLocation] = extra_field(default_factory=list)
+    preprocessed_mappings: Sequence[SourceLocation] = extra_field(default_factory=list)
+
+    preprocessed_pos: int = extra_field(default=0)
+    preprocessed_lineno: int = extra_field(default=1)
+    preprocessed_colno: int = extra_field(default=1)
+    preprocessed_locations: list[SourceLocation] = extra_field(default_factory=list)
 
     index: int = extra_field(default=-1)
     tokens: list[Token] = extra_field(default_factory=list)
     indentation: list[int] = extra_field(default_factory=list)
     indentation_skip: set[str] = extra_field(default_factory=set)
 
     generator: Iterator[Token] = extra_field()
     ignored_tokens: set[str] = extra_field()
 
     data: dict[str, Any] = extra_field(default_factory=dict)
 
-    regex_module: Any = field(default_factory=lambda: re, repr=False)
+    regex_module: Any = field(default=re, repr=False)
     regex_cache: dict[SyntaxRules, re.Pattern[str]] = extra_field()
 
     def __post_init__(self) -> None:
-        self.location = SourceLocation(pos=0, lineno=1, colno=1)
+        if self.preprocessor:
+            self.preprocessed_source, *mappings = self.preprocessor(self.source)
+            self.source_mappings, self.preprocessed_mappings = mappings
+        else:
+            self.preprocessed_source = self.source
+
         self.generator = self.generate_tokens()
         self.ignored_tokens = {"whitespace", "newline", "eof"}
         self.regex_cache = BAKED_REGEX_CACHE.setdefault(self.regex_module, {})
         self.bake_regex()
 
     def bake_regex(self) -> None:
         """Compile the syntax rules.
@@ -208,18 +227,17 @@
         world
         hello
 
         Mostly used to ensure consistency in some of the provided context managers.
         Should be considered internal.
         """
         del self.tokens[self.index + 1 :]
-        self.location = (
-            self.current.end_location
-            if self.index >= 0
-            else SourceLocation(pos=0, lineno=1, colno=1)
+        del self.preprocessed_locations[self.index + 1 :]
+        self.preprocessed_pos, self.preprocessed_lineno, self.preprocessed_colno = (
+            self.preprocessed_locations[self.index] if self.index >= 0 else (0, 1, 1)
         )
 
     @contextmanager
     def syntax(self, **kwargs: str | None) -> Iterator[None]:
         """Extend token syntax using regular expressions.
 
         The keyword arguments associate regular expression patterns to token types. The method returns a context manager during which the specified tokens will be recognized.
@@ -467,33 +485,38 @@
         return value.partition("\n")[0]
 
     def emit_token(self, token_type: str, value: str = "") -> Token:
         """Generate a token in the token stream.
 
         Should be considered internal. Used by the :meth:`generate_tokens` method.
         """
-        end_pos = self.location.pos + len(value)
-        end_lineno = self.location.lineno + value.count("\n")
+        location = SourceLocation(
+            self.preprocessed_pos,
+            self.preprocessed_lineno,
+            self.preprocessed_colno,
+        )
 
-        if (line_start := value.rfind("\n")) == -1:
-            end_colno = self.location.colno + len(value)
-        else:
-            end_colno = len(value) - line_start
+        end_location = location.skip_over(value)
+
+        (
+            self.preprocessed_pos,
+            self.preprocessed_lineno,
+            self.preprocessed_colno,
+        ) = end_location
 
         token = Token(
             type=token_type,
             value=value,
-            location=self.location,
-            end_location=SourceLocation(end_pos, end_lineno, end_colno),
+            location=location.map(self.preprocessed_mappings, self.source_mappings),
+            end_location=end_location.map(
+                self.preprocessed_mappings, self.source_mappings
+            ),
         )
 
-        if self.token_handler:
-            token = self.token_handler(token)
-
-        self.location = token.end_location
+        self.preprocessed_locations.append(end_location)
         self.tokens.append(token)
 
         self.index = len(self.tokens) - 1
 
         return token
 
     def emit_error(self, exc: T) -> T:
@@ -508,15 +531,15 @@
         'hello'
         >>> exc = stream.emit_error(InvalidSyntax("foo"))
         >>> exc.location
         SourceLocation(pos=5, lineno=1, colno=6)
         """
         return set_location(
             exc,
-            self.current.end_location if self.index >= 0 else SourceLocation(0, 1, 1),
+            self.current.end_location if self.index >= 0 else INITIAL_LOCATION,
         )
 
     def generate_tokens(self) -> Iterator[Token]:
         """Extract tokens from the input string.
 
         Should be considered internal. This is the underlying generator being driven
         by the stream.
@@ -524,16 +547,16 @@
 
         def emit_dedent(level: int = 0) -> Iterator[Token]:
             while self.indentation and level < self.indentation[-1]:
                 self.emit_token("dedent")
                 self.indentation.pop()
                 yield self.current
 
-        while self.location.pos < len(self.source):
-            match = self.regex.match(self.source, self.location.pos)
+        while self.preprocessed_pos < len(self.preprocessed_source):
+            match = self.regex.match(self.preprocessed_source, self.preprocessed_pos)
 
             assert match
             assert match.lastgroup
 
             if self.tokens and self.indentation:
                 if (
                     self.current.type == "whitespace"
@@ -1107,15 +1130,23 @@
         ['w', 'o', 'r', 'l', 'd']
         """
         copy = TokenStream(self.source, regex_module=self.regex_module)
 
         copy.syntax_rules = self.syntax_rules
         copy.regex = self.regex
 
-        copy.location = self.location
+        copy.preprocessor = self.preprocessor
+        copy.preprocessed_source = self.preprocessed_source
+        copy.source_mappings = self.source_mappings
+        copy.preprocessed_mappings = self.preprocessed_mappings
+
+        copy.preprocessed_pos = self.preprocessed_pos
+        copy.preprocessed_lineno = self.preprocessed_lineno
+        copy.preprocessed_colno = self.preprocessed_colno
+        copy.preprocessed_locations = list(self.preprocessed_locations)
 
         copy.index = self.index
         copy.tokens = list(self.tokens)
         copy.indentation = list(self.indentation)
         copy.indentation_skip = set(self.indentation_skip)
 
         copy.ignored_tokens = set(self.ignored_tokens)
```

### Comparing `tokenstream-1.6.0/tokenstream/token.py` & `tokenstream-1.7.0/tokenstream/token.py`

 * *Files identical despite different names*

### Comparing `tokenstream-1.6.0/PKG-INFO` & `tokenstream-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenstream
-Version: 1.6.0
+Version: 1.7.0
 Summary: A versatile token stream for handwritten parsers
 Home-page: https://github.com/vberlier/tokenstream
 License: MIT
 Keywords: parsing,tokenizer,lexer,recursive-descent-parser,token-stream
 Author: Valentin Berlier
 Author-email: berlier.v@gmail.com
 Requires-Python: >=3.10,<4.0
```

