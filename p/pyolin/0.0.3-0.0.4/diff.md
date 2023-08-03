# Comparing `tmp/pyolin-0.0.3.tar.gz` & `tmp/pyolin-0.0.4.tar.gz`

## Comparing `pyolin-0.0.3.tar` & `pyolin-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,38 @@
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 pyolin-0.0.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pyolin-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/__init__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/__main__.py
--rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/field.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/header_detector.py
--rw-r--r--   0        0        0    16373 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/ioformat.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/parser.py
--rw-r--r--   0        0        0     7752 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/pyolin.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/record.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/util.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/__init__.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_addresses.csv
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_addresses_unix.csv
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_addresses_with_header.csv
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_amazon_reviews.tsv
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_colors.json
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_files.txt
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_files_with_header.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_formatting.txt
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_grades_simple_csv.csv
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_grades_with_header.csv
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_nba.txt
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_news_decline.csv
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_news_decline.tsv
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_onerow.csv
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_pickle
--rw-r--r--   0        0        0    64009 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/test_pyolin.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/utils.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pyolin-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyolin-0.0.3/LICENSE
--rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 pyolin-0.0.3/README.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 pyolin-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 pyolin-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 pyolin-0.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyolin-0.0.4/.vscode/launch.json
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pyolin-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/__main__.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/field.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/header_detector.py
+-rw-r--r--   0        0        0    28593 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/ioformat.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/json_encoder.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/parser.py
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/pyolin.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/record.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/util.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/__init__.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_addresses.csv
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_addresses_unix.csv
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_addresses_with_header.csv
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_amazon_reviews.tsv
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_colors.json
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_files.txt
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_files_with_header.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_formatting.txt
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_grades_simple_csv.csv
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_grades_with_header.csv
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_json_example.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_nba.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_news_decline.csv
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_news_decline.tsv
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_onerow.csv
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/data_pickle
+-rw-r--r--   0        0        0    79776 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/test_pyolin.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyolin/test/utils.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pyolin-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyolin-0.0.4/LICENSE
+-rw-r--r--   0        0        0     8861 2020-02-02 00:00:00.000000 pyolin-0.0.4/README.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 pyolin-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 pyolin-0.0.4/PKG-INFO
```

### Comparing `pyolin-0.0.3/.github/workflows/python-package.yml` & `pyolin-0.0.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.3/pyolin/field.py` & `pyolin-0.0.4/pyolin/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Iterable, Optional, Tuple, Union
 
 
 Number = Union[int, float]
 Boolean = bool
 
-class Field(str):
 
+class Field(str):
     def __new__(cls, content, *, header: Optional[Iterable[str]]):
         return super().__new__(cls, content)
 
     def __init__(self, content, *, header: Optional[Iterable[str]]):
         self.header = header
 
     def _isnumber(self):
@@ -22,46 +22,47 @@
     def _coerce_to_number(self) -> Number:
         try:
             try:
                 return int(self)
             except ValueError:
                 return float(self)
         except ValueError:
+            # pylint:disable=raise-missing-from
             raise ValueError(f'Cannot convert "{self}" to int or float')
 
     def _coerce_with_type_check(self, other: Any) -> Tuple[Union[Number, str], Any]:
-        '''
+        """
         Perform numeric type coercion via type check. If we can coerce to the
         "other" type, perform the coercion. Otherwise use the super
         implementation.
-        '''
+        """
         if isinstance(other, Field) and self._isnumber() and other._isnumber():
             return self._coerce_to_number(), other._coerce_to_number()
         elif isinstance(other, (int, float)):
             return self._coerce_to_number(), other
         else:
             return super(), other
 
     def _coerce_with_fallback(self, other: Any) -> Tuple[Union[Number, str], Any]:
-        '''
+        """
         Perform numeric type coercion by converting self to a numeric value
         (without checking the `other` type). Falls back to the super
         implementation if the coercion failed.
-        '''
+        """
         try:
             return self._coerce_assuming_numeric(other)
         except ValueError:
             return super(), other
 
     def _coerce_assuming_numeric(self, other):
-        '''
+        """
         Perform numeric type coercion assuming both self and other can be
         successfully converted to numeric types. An exception will be thrown
         if the coercion failed.
-        '''
+        """
         if isinstance(other, Field):
             other = other._coerce_to_number()
         return self._coerce_to_number(), other
 
     def __gt__(self, other):
         modified_self, modified_other = self._coerce_with_type_check(other)
         return modified_self.__gt__(modified_other)
@@ -95,18 +96,18 @@
         return modified_self.__sub__(modified_other)  # type: ignore
 
     def __rsub__(self, other):
         modified_self, modified_other = self._coerce_assuming_numeric(other)
         return modified_self.__rsub__(modified_other)  # type: ignore
 
     def __mul__(self, other):
-        '''
+        """
         Multiplication is one special case where the numeric operation takes
         precendence over the string operation, since the former is more common.
-        '''
+        """
         modified_self, modified_other = self._coerce_with_fallback(other)
         return modified_self.__mul__(modified_other)
 
     def __matmul__(self, other):
         modified_self, modified_other = self._coerce_assuming_numeric(other)
         # pylint: disable=no-member
         return modified_self.__matmul__(modified_other)  # type: ignore
@@ -209,21 +210,24 @@
     def __floor__(self):
         return self._coerce_to_number().__floor__()
 
     def __ceil__(self):
         return self._coerce_to_number().__ceil__()
 
     def __bytes__(self):
-        return self.encode('utf-8')
+        return self.encode("utf-8")
+
+    def __hash__(self):
+        return hash(str(self))
 
     @property
     def bool(self) -> bool:
-        if self.lower() in ('true', 't', 'y', 'yes', '1', 'on'):
+        if self.lower() in ("true", "t", "y", "yes", "1", "on"):
             return True
-        elif self.lower() in ('false', 'f', 'n', 'no', '0', 'off'):
+        elif self.lower() in ("false", "f", "n", "no", "0", "off"):
             return False
         else:
             raise ValueError(f'Cannot convert "{self}" to bool')
 
     @property
     def int(self) -> int:
         return int(self)
```

### Comparing `pyolin-0.0.3/pyolin/header_detector.py` & `pyolin-0.0.4/pyolin/header_detector.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,29 +38,29 @@
 
             if thisType != columnTypes[col]:
                 if columnTypes[col] is None:  # add new column type
                     columnTypes[col] = thisType
                 else:
                     # type is inconsistent, remove column from
                     # consideration
-                    columnTypes[col] = 'Disqualified'
+                    columnTypes[col] = "Disqualified"
 
-    debug('column types', columnTypes)
+    debug("column types", columnTypes)
     # finally, compare results against first row and "vote"
     # on whether it's a header
     hasHeader = 0
     for col, colType in enumerate(columnTypes):
         if isinstance(colType, int):  # it's a length
             if len(header[col]) != colType:
                 hasHeader += 1
             else:
                 hasHeader -= 1
-        elif colType != 'Disqualified' and colType is not None:  # attempt typecast
+        elif colType != "Disqualified" and colType is not None:  # attempt typecast
             try:
                 colType(header[col])
             except (ValueError, TypeError):
                 hasHeader += 1
             else:
                 hasHeader -= 1
-    debug('hasHeader', hasHeader)
+    debug("hasHeader", hasHeader)
 
     return hasHeader > 0
```

### Comparing `pyolin-0.0.3/pyolin/parser.py` & `pyolin-0.0.4/pyolin/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,153 +1,174 @@
+"""Implementation of the Python code parsing logic in Pyolin."""
 import ast
 import io
 import textwrap
 import token
 import tokenize
 import traceback
 from types import CodeType
-from typing import Any, Dict, Iterable, List, Sequence, Tuple
+from typing import Any, Dict, Iterable, List, Tuple
 
 from .util import debug, NoMoreRecords
 
 
-def _split_last_statement(tokens: Iterable[tokenize.TokenInfo], prog: str) -> Tuple[int, int]:
+def _split_last_statement(
+    tokens: Iterable[tokenize.TokenInfo], prog: str
+) -> Tuple[int, int]:
     def _line_pos_to_pos(linepos):
         line, pos = linepos
         offset = 0
         for _ in range(1, line):
-            offset = prog.index('\n', offset) + 1
+            offset = prog.index("\n", offset) + 1
         return pos + offset
 
     started = False
     for tok in reversed(list(tokens)):
         if tok.exact_type in (token.SEMI, token.NEWLINE):
             if started:
                 return _line_pos_to_pos(tok.start), _line_pos_to_pos(tok.end)
         elif tok.type not in (token.ENDMARKER, token.COMMENT, token.NL):
             started = True
     return 0, 0
 
 
-def _replace_double_semicolons(tokens: Iterable[tokenize.TokenInfo]) -> Iterable[tokenize.TokenInfo]:
+def _replace_double_semicolons(
+    tokens: Iterable[tokenize.TokenInfo],
+) -> Iterable[tokenize.TokenInfo]:
     double_semis = []
     last_semi = False
     tokens = list(tokens)
     for i, tok in enumerate(tokens):
-        if tok.string == ';':
+        if tok.string == ";":
             if last_semi:
-                double_semis.append(i-1)
+                double_semis.append(i - 1)
             else:
                 last_semi = True
         else:
             last_semi = False
     for i in reversed(double_semis):
         del tokens[i + 1]
         _replace_with_newline(tokens, i)
-    debug('tokens', list(tokens), double_semis)
+    debug("tokens", list(tokens), double_semis)
     return tokens
 
 
 def _replace_with_newline(tokens: List[tokenize.TokenInfo], pos: int) -> None:
     tok = tokens[pos]
-    tokens[pos] = tokenize.TokenInfo(
-        token.NEWLINE,
-        '\n',
-        tok.start,
-        tok.end,
-        tok.line)
+    tokens[pos] = tokenize.TokenInfo(token.NEWLINE, "\n", tok.start, tok.end, tok.line)
     line_offset = 0
-    for i, tok2 in enumerate(tokens[pos + 1:]):
+    for i, tok2 in enumerate(tokens[pos + 1 :]):
         if i == 0:
             line_offset = tok2.start[1]
         if tok2.start[0] != tok.start[0]:
             line_offset = 0
         tokens[i + pos + 1] = tokenize.TokenInfo(
-            tok2.type, tok2.string,
+            tok2.type,
+            tok2.string,
             start=(tok2.start[0] + 1, tok2.start[1] - line_offset),
             end=(tok2.end[0] + 1, tok2.end[1] - line_offset),
-            line=tok2.line)
+            line=tok2.line,
+        )
 
 
-def _parse(prog: str) -> Tuple[ast.AST, ast.AST]:
-    '''
-    Parse the given pyolin program into the exec statements and eval statements that can be evaluated
-    directly, applying the necessary syntax transformations as necessary.
-    '''
+def _parse(prog: str) -> Tuple[ast.Module, ast.Expression]:
+    """
+    Parse the given pyolin program into the exec statements and eval statements that can be
+    evaluated directly, applying the necessary syntax transformations as necessary.
+    """
     prog_io = io.StringIO(prog)
     tokens = tokenize.generate_tokens(prog_io.readline)
     tokens = _replace_double_semicolons(tokens)
     prog = tokenize.untokenize(tokens)
-    debug(f'newprog=\n{prog}')
+    debug(f"newprog=\n{prog}")
     split_start, split_end = _split_last_statement(tokens, prog)
     prog_stmts = prog[:split_start]
     prog_expr = prog[split_end:]
-    debug(f'stmt={prog_stmts} expr={prog_expr}')
+    debug(f"stmt={prog_stmts} expr={prog_expr}")
     try:
-        exec_statements = ast.parse(prog_stmts, mode='exec')
-    except SyntaxError as e:
-        raise RuntimeError(textwrap.dedent(
-            f'''\
-            Invalid syntax:
-              {prog_stmts}
-              {" "*(e.offset-1)}^'''))
+        exec_statements = ast.parse(prog_stmts, mode="exec")
+    except SyntaxError as exc:
+        assert exc.offset
+        raise RuntimeError(
+            textwrap.dedent(
+                f"""\
+                Invalid syntax:
+                  {prog_stmts}
+                  {" "*(exc.offset-1)}^"""
+            )
+        ) from None
     try:
         # Try to parse as generator expression (the common case)
-        eval_expr = ast.parse(f'({prog_expr})', mode='eval')
-    except SyntaxError as e:
+        eval_expr = ast.parse(f"({prog_expr})", mode="eval")
+    except SyntaxError as exc:
         # Try to parse as <expr> if <condition>
         try:
-            eval_expr = ast.parse(f'({prog_expr} else _UNDEFINED_)', mode='eval')
+            eval_expr = ast.parse(f"({prog_expr} else _UNDEFINED_)", mode="eval")
         except SyntaxError:
             try:
-                ast.parse(f'{prog_expr}', mode='exec')
+                # Check if it's executable to provide better error message
+                ast.parse(f"{prog_expr}", mode="exec")
             except SyntaxError:
-                raise RuntimeError(textwrap.dedent(
-                    f'''\
+                assert exc.offset
+                raise RuntimeError(
+                    textwrap.dedent(
+                        f"""\
                     Invalid syntax:
                       {prog_expr}
-                      {" "*(e.offset-2)}^'''))
+                      {" "*(exc.offset-2)}^"""
+                    )
+                ) from None
             else:
-                raise RuntimeError(textwrap.dedent(f'''\
+                raise RuntimeError(
+                    textwrap.dedent(
+                        f"""\
                     Cannot evaluate value from statement:
-                      {prog_expr}'''))
+                      {prog_expr}"""
+                    )
+                ) from None
     debug(ast.dump(eval_expr))
     return exec_statements, eval_expr
 
 
 class UserError(RuntimeError):
+    """An error in the user-provided Pyolin program."""
 
     def formatted_tb(self):
+        """Formats the traceback of this error, hiding any Pyolin internals from
+        the stack trace."""
         cause = self.__cause__
         assert isinstance(cause, BaseException)
+        exception_traceback = cause.__traceback__  # pylint: disable=no-member
+        assert exception_traceback
         return traceback.format_exception(
-            cause.__class__,
-            cause,
-            cause.__traceback__.tb_next)  # pylint: disable=no-member
+            cause.__class__, cause, exception_traceback.tb_next
+        )
 
     def __str__(self):
-        return ''.join(self.formatted_tb()).rstrip('\n')
+        return "".join(self.formatted_tb()).rstrip("\n")
 
 
 class Prog:
+    """The intermediate representation of the user-provided Pyolin program."""
 
     _exec: CodeType
     _eval: CodeType
 
     def __init__(self, prog: Any):
-        if hasattr(prog, '__code__'):
-            self._exec = compile('', filename='pyolin_user_prog.py', mode='exec')
+        if hasattr(prog, "__code__"):
+            self._exec = compile("", filename="pyolin_user_prog.py", mode="exec")
             self._eval = prog.__code__
         else:
             exec_code, eval_code = _parse(prog)
-            debug('Resulting AST', ast.dump(exec_code), ast.dump(eval_code))
-            self._exec = compile(exec_code, filename='pyolin_user_prog.py', mode='exec')
-            self._eval = compile(eval_code, filename='pyolin_user_prog.py', mode='eval')
+            debug("Resulting AST", ast.dump(exec_code), ast.dump(eval_code))
+            self._exec = compile(exec_code, filename="pyolin_user_prog.py", mode="exec")
+            self._eval = compile(eval_code, filename="pyolin_user_prog.py", mode="eval")
 
-    def exec(self, globals: Dict[str, Any]) -> Any:
+    def exec(self, global_dict: Dict[str, Any]) -> Any:
+        """Executes the user-provided Pyolin program and returns the result."""
         try:
-            exec(self._exec, globals)
-            return eval(self._eval, globals)
+            exec(self._exec, global_dict)  # pylint: disable=exec-used
+            return eval(self._eval, global_dict)  # pylint: disable=eval-used
         except NoMoreRecords:
             raise
-        except Exception as e:
-            raise UserError() from e
+        except Exception as exc:
+            raise UserError() from exc
```

### Comparing `pyolin-0.0.3/pyolin/pyolin.py` & `pyolin-0.0.4/pyolin/pyolin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,182 +1,224 @@
 import argparse
-import collections
 import importlib
 import itertools
 import re
 import sys
+import json
 
 from contextlib import contextmanager
+from typing import (
+    IO,
+    Any,
+    Callable,
+    Generator,
+    Generic,
+    Iterable,
+    Optional,
+    TypeVar,
+    Union,
+)
 from hashbang import command, Argument
 
-from .util import (BoxedItem, LazyItem, Item, ItemDict, StreamingSequence, _UNDEFINED_, NoMoreRecords)
+from .util import (
+    BoxedItem,
+    LazyItem,
+    Item,
+    ItemDict,
+    StreamingSequence,
+    _UNDEFINED_,
+    NoMoreRecords,
+)
 from .ioformat import *
 from .record import RecordSequence
 from .parser import Prog
 
 
 @contextmanager
-def get_io(input_file, *, binary=False):
+def get_io(input_file: Optional[str]) -> Generator[IO[Any], None, None]:
     if input_file:
-        mode = 'rb' if binary else 'r'
+        mode = "rb"
         with open(input_file, mode) as f:
             yield f
     else:
-        yield sys.stdin.buffer if binary else sys.stdin
+        yield sys.stdin.buffer
 
 
-class RecordScoped(LazyItem):
-    def __init__(self, generator, *, on_accessed):
+I = TypeVar("I")
+
+
+class RecordScoped(LazyItem, Generic[I]):
+    _on_accessed: Callable[[], None]
+
+    def __init__(self, generator: RecordSequence, *, on_accessed: Callable[[], None]):
         super().__init__(self._get_first_time, on_accessed=on_accessed)
         self._iter = iter(generator)
 
     def _get_first_time(self):
         self._on_accessed()
         next(self)
         return self._val
 
     def __iter__(self):
         return self
 
     def __next__(self):
-        '''
+        """
         Advances to the next record in the generator. This is done manually so
         that the value can be accessed multiple times within the same
         iteration.
-        '''
+        """
         try:
             self._val = next(self._iter)
             return self._val
-        except StopIteration as e:
-            raise NoMoreRecords() from e
+        except StopIteration as exc:
+            raise NoMoreRecords() from exc
 
 
-def _execute_internal(prog, *args,
-            input=None,
-            field_separator=None,
-            record_separator='\n',
-            input_format='awk',
-            output_format='auto'):
+def _execute_internal(
+    prog,
+    *args,
+    input_: Optional[str] = None,
+    field_separator=None,
+    record_separator="\n",
+    input_format="auto",
+    output_format="auto",
+):
     prog = Prog(prog)
-    new_parser = lambda input_format: create_parser(input_format, record_separator, field_separator)
+
+    def new_parser(input_format):
+        return create_parser(input_format, record_separator, field_separator)
+
     parser_box = BoxedItem(lambda: new_parser(input_format))
 
-    def gen_records():
+    def gen_records(input_file: Optional[str]):
         parser_box.frozen = True
         parser = parser_box()
-        with get_io(input, binary=parser.binary) as f:
-            for record in parser.records(f):
+        with get_io(input_file) as io_stream:
+            for i, record in enumerate(parser.records(io_stream)):
+                record.set_num(i)
                 yield record
 
-    def get_contents(input):
+    def get_contents(input_file: Optional[str]) -> Union[str, bytes]:
         parser_box.frozen = True
-        parser = parser_box()
-        with get_io(input, binary=parser.binary) as f:
-            return f.read()
+        with get_io(input_file) as io_stream:
+            contents = io_stream.read()
+            try:
+                return contents.decode("utf-8")
+            except Exception:
+                return contents
 
-    record_seq = RecordSequence(gen_records())
+    record_seq = RecordSequence(gen_records(input_))
 
     def get_dataframe():
         import pandas as pd
+
         header = [f.str for f in record_seq.header] if record_seq.header else None
         df = pd.DataFrame(record_seq, columns=header)
-        return df.apply(pd.to_numeric, errors='ignore')  # type: ignore
+        return df.apply(pd.to_numeric, errors="ignore")  # type: ignore
 
-    scope = 'undecided'
+    scope = "undecided"
 
     def set_scope(newscope):
         nonlocal scope
-        if scope != newscope and scope != 'undecided':
-            raise RuntimeError('Cannot access both record scoped and table scoped variables')
+        if scope != newscope and scope != "undecided":
+            raise RuntimeError(
+                "Cannot access both record scoped and table scoped variables"
+            )
         scope = newscope
 
     def table_scoped(func):
-        return LazyItem(func, on_accessed=lambda: set_scope('table'))
+        return LazyItem(func, on_accessed=lambda: set_scope("table"))
 
-    record_var = RecordScoped(record_seq, on_accessed=lambda: set_scope('record'))
+    record_var = RecordScoped(record_seq, on_accessed=lambda: set_scope("record"))
     try:
         printer = new_printer(output_format)
     except KeyError:
+        # pylint:disable=raise-missing-from
         raise ValueError(f'Unrecognized output format "{output_format}"')
-    global_dict = ItemDict({
-        # Record scoped
-        'record': record_var,
-        'fields': record_var,
-        'line': Item(lambda: record_var().str),
-
-        # Table scoped
-        'lines': table_scoped(lambda: StreamingSequence(r.str for r in record_seq)),
-        'records': table_scoped(lambda: record_seq),
-        'file': table_scoped(lambda: get_contents(input)),
-        'contents': table_scoped(lambda: get_contents(input)),
-        'df': table_scoped(get_dataframe),
-
-        # Other
-        'filename': input,
-        '_UNDEFINED_': _UNDEFINED_,
-        'new_printer': new_printer,
-        'new_parser': new_parser,
-        'BEGIN': True,
-
-        # Modules
-        're': re,
-        'pd': Item(lambda: importlib.import_module('pandas')),
-        'np': Item(lambda: importlib.import_module('numpy')),
-        'csv': Item(lambda: importlib.import_module('csv')),
-        'pyolin': Item(lambda: importlib.import_module('pyolin')),
-
-        # Writeable
-        'printer': printer,
-        'parser': parser_box,
-        'header': None,
-    })
+    global_dict = ItemDict(
+        {
+            # Record scoped
+            "record": record_var,
+            "fields": record_var,
+            "line": Item(lambda: record_var().str),
+            # Table scoped
+            "lines": table_scoped(lambda: StreamingSequence(r.str for r in record_seq)),
+            "records": table_scoped(lambda: record_seq),
+            "file": table_scoped(lambda: get_contents(input_)),
+            "contents": table_scoped(lambda: get_contents(input_)),
+            "df": table_scoped(get_dataframe),
+            "jsonobj": table_scoped(lambda: json.loads(get_contents(input_))),
+            # Other
+            "filename": input_,
+            "_UNDEFINED_": _UNDEFINED_,
+            "new_printer": new_printer,
+            "new_parser": new_parser,
+            # Modules
+            "re": re,
+            "pd": Item(lambda: importlib.import_module("pandas")),
+            "np": Item(lambda: importlib.import_module("numpy")),
+            "csv": Item(lambda: importlib.import_module("csv")),
+            "pyolin": Item(lambda: importlib.import_module("pyolin")),
+            # Writeable
+            "printer": printer,
+            "parser": parser_box,
+            "header": None,
+        }
+    )
 
     # Shift argv results
-    sys.argv = ['pyolin', *args]
+    sys.argv = ["pyolin", *args]
 
     try:
         result = prog.exec(global_dict)
     except NoMoreRecords:
         return _UNDEFINED_, global_dict
-    else:
-        if scope == 'record':
-            global_dict['BEGIN'] = False
-            result = itertools.chain((result,), (prog.exec(global_dict) for _ in record_var))
 
-        return result, global_dict
+    if scope == "record":
+        result = itertools.chain(
+            (result,), (prog.exec(global_dict) for _ in record_var)
+        )
+
+    return result, global_dict
+
 
 def run(*args, **kwargs):
-    '''
-    Run pyolin from another Python script. This is designed to ease the transition from the one-liner
-    to a more full-fledged script file. By running pyolin in Python, you get the results in Python
-    list or objects, while still keeping the input parsing and output formatting capabilities of
-    pyolin. Serious scripts should migrate away from those as well, perhaps outputting json and then
-    using pyolin as a data-formatting pass-through.
-    '''
+    """
+    Run pyolin from another Python script. This is designed to ease the transition from
+    the one-liner to a more full-fledged script file. By running pyolin in Python, you get the
+    results in Python list or objects, while still keeping the input parsing and output formatting
+    capabilities of pyolin. Serious scripts should migrate away from those as well, perhaps
+    outputting json and then using pyolin as a data-formatting pass-through.
+    """
     result, _ = _execute_internal(*args, **kwargs)
     if isinstance(result, (str, bytes)):
         return result
-    if isinstance(result, collections.abc.Iterable):
+    if isinstance(result, Iterable):
         return list(result)
     else:
         return result
 
 
 @command(
-    Argument('field_separator', aliases='F'),
-    Argument('input_format', choices=list(PARSERS)),
-    Argument('output_format', choices=list(PRINTERS)),
-    formatter_class=argparse.RawDescriptionHelpFormatter)
-def _command_line(prog, *_REMAINDER_,
-        input=None,
-        field_separator=None,
-        record_separator='\n',
-        input_format='awk',
-        output_format='auto'):
-    '''
+    Argument("field_separator", aliases="F"),
+    Argument("input_format", choices=list(PARSERS)),
+    Argument("output_format", choices=list(PRINTERS)),
+    formatter_class=argparse.RawDescriptionHelpFormatter,
+)
+def _command_line(
+    prog,
+    *_REMAINDER_,
+    input_=None,
+    field_separator=None,
+    record_separator="\n",
+    input_format="auto",
+    output_format="auto",
+):
+    """
     pyolin - Python one liners to easily parse and process data in Python.
 
     Pyolin processes text information from stdin or a given file and evaluates
     the given input `prog` and prints the result.
 
     Example:
         pyolin 'record[0] + record[1] if record[2] > 50'
@@ -206,16 +248,23 @@
         df – Contents of the entire file as a pandas.DataFrame. (Available
             only if pandas is installed).
       - General:
         filename – The name of the file being processed, possibly None if
             reading from stdin.
         re – The regex module.
         pd – The pandas module, if installed.
-    '''
-    result, global_dict = _execute_internal(prog, *_REMAINDER_, input=input,
-            field_separator=field_separator, record_separator=record_separator,
-            input_format=input_format, output_format=output_format)
-    printer = global_dict['printer']
+    """
+    result, global_dict = _execute_internal(
+        prog,
+        *_REMAINDER_,
+        input_=input_,
+        field_separator=field_separator,
+        record_separator=record_separator,
+        input_format=input_format,
+        output_format=output_format,
+    )
+    printer = global_dict["printer"]
     if not isinstance(printer, Printer):
         raise RuntimeError(
-            f'printer must be an instance of Printer. Found "{printer!r}" instead')
-    global_dict['printer'].print_result(result, header=global_dict.get('header'))
+            f'printer must be an instance of Printer. Found "{printer!r}" instead'
+        )
+    global_dict["printer"].print_result(result, header=global_dict.get("header"))
```

### Comparing `pyolin-0.0.3/pyolin/test/data_amazon_reviews.tsv` & `pyolin-0.0.4/pyolin/test/data_amazon_reviews.tsv`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.3/pyolin/test/data_grades_with_header.csv` & `pyolin-0.0.4/pyolin/test/data_grades_with_header.csv`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.3/pyolin/test/test_pyolin.py` & `pyolin-0.0.4/pyolin/test/test_pyolin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,916 +1,1050 @@
+# pylint: disable=missing-function-docstring
+# pylint: disable=missing-module-docstring
+# pylint: disable=missing-class-docstring
+# pylint: disable=too-many-lines
+
 import contextlib
 import os
-from pyolin.parser import UserError
-from pyolin import pyolin
-from pyolin.util import _UNDEFINED_
+import traceback
+from typing import Any, Callable, Sequence, Union
 from pprint import pformat
 import subprocess
 import sys
 import textwrap
 import unittest
 from unittest import mock
 
+from pyolin.parser import UserError
+from pyolin import pyolin
+from pyolin.util import _UNDEFINED_
+
 from .utils import ErrorWithStderr, run_capturing_output, timeout
 
 
 def _test_file(file):
     return os.path.join(os.path.dirname(__file__), file)
 
 
-def run_cli(prog, *, input='data_nba.txt', extra_args=(), **kwargs):
-    with run_capturing_output(errmsg=f'Prog: {prog}') as output:
-        pyolin._command_line(prog, *extra_args, input=_test_file(input), **kwargs)
+def run_cli(prog, *, input_file="data_nba.txt", extra_args=(), **kwargs):
+    with run_capturing_output(errmsg=f"Prog: {prog}") as output:
+        pyolin._command_line(prog, *extra_args, input_=_test_file(input_file), **kwargs)
         return output
 
 
-def run_pyolin(prog, *, input='data_nba.txt', **kwargs):
-    return pyolin.run(prog, input=_test_file(input), **kwargs)
+def run_pyolin(prog, *, input_file="data_nba.txt", **kwargs):
+    return pyolin.run(prog, input_=_test_file(input_file), **kwargs)
 
 
 @contextlib.contextmanager
-def pyolinPopen(prog, extra_args=(), universal_newlines=True, **kwargs):
+def pyolin_popen(prog, extra_args=(), universal_newlines=True, **kwargs):
     with subprocess.Popen(
-        [sys.executable, '.', prog] + extra_args,
-        stdin=kwargs.get('stdin', subprocess.PIPE),
-        stdout=kwargs.get('stdout', subprocess.PIPE),
-        stderr=kwargs.get('stderr', subprocess.PIPE),
+        [sys.executable, "-m", "pyolin", prog] + extra_args,
+        stdin=kwargs.get("stdin", subprocess.PIPE),
+        stdout=kwargs.get("stdout", subprocess.PIPE),
+        stderr=kwargs.get("stderr", subprocess.PIPE),
         universal_newlines=universal_newlines,
-        **kwargs
+        **kwargs,
     ) as proc:
         yield proc
 
 
 class PyolinTest(unittest.TestCase):
-
     maxDiff = None
     longMessage = True
 
     def _myassert(self, actual, expected, prog, data):
         if isinstance(expected, str):
             expected = textwrap.dedent(expected)
             self.assertEqual(
                 actual,
                 expected,
-                msg=f'''\
+                msg=f"""\
 Prog: pyolin \'{prog}\' {_test_file(data)}
 Expected:
 {textwrap.indent(expected, '    ')}
 ---
 
 Actual:
 {textwrap.indent(actual, '    ')}
 ---
-''')
+""",
+            )
         else:
             self.assertEqual(
                 actual,
                 expected,
-                msg=f'''\
+                msg=f"""\
 Prog: pyolin \'{prog}\' {_test_file(data)}
 Expected:
     {expected!r}
 ---
 
 Actual:
     {actual!r}
 ---
-''')
+""",
+            )
 
-    def assertRunPyolin(self, prog, expected, *, input='data_nba.txt', **kwargs):
-        actual = run_pyolin(prog, input=input, **kwargs)
+    def assert_run_pyolin(
+        self,
+        prog: Union[str, Callable[[], Any]],
+        expected: Any,
+        *,
+        input_file: str = "data_nba.txt",
+        **kwargs,
+    ):
+        actual = run_pyolin(prog, input_file=input_file, **kwargs)
         self.assertEqual(actual, expected)
 
-    def assertPyolin(self, prog, expected, *, input='data_nba.txt', extra_args=[], **kwargs):
-        actual = run_cli(prog, input=input, extra_args=extra_args, **kwargs)
+    def assert_pyolin(
+        self,
+        prog: Union[str, Callable[[], Any]],
+        expected: Union[str, bytes],
+        *,
+        input_file: str = "data_nba.txt",
+        extra_args: Sequence[str] = (),
+        **kwargs,
+    ):
+        actual = run_cli(prog, input_file=input_file, extra_args=extra_args, **kwargs)
         if isinstance(expected, str):
-            self._myassert(actual.getvalue(), expected, prog, input)
+            self._myassert(actual.getvalue(), expected, prog, input_file)
         else:
-            self._myassert(actual.getbytes(), expected, prog, input)
+            self._myassert(actual.getbytes(), expected, prog, input_file)
 
-    def testLines(self):
-        self.assertPyolin(
-            'line for line in lines',
-            '''\
+    def test_lines(self):
+        self.assert_pyolin(
+            "line for line in lines",
+            """\
             | value                          |
             | ------------------------------ |
             | Bucks Milwaukee    60 22 0.732 |
             | Raptors Toronto    58 24 0.707 |
             | 76ers Philadelphia 51 31 0.622 |
             | Celtics Boston     49 33 0.598 |
             | Pacers Indiana     48 34 0.585 |
-            ''')
+            """,
+        )
 
-    def testLine(self):
-        self.assertPyolin(
-            'line',
-            '''\
+    def test_line(self):
+        self.assert_pyolin(
+            "line",
+            """\
             | value                          |
             | ------------------------------ |
             | Bucks Milwaukee    60 22 0.732 |
             | Raptors Toronto    58 24 0.707 |
             | 76ers Philadelphia 51 31 0.622 |
             | Celtics Boston     49 33 0.598 |
             | Pacers Indiana     48 34 0.585 |
-            ''')
+            """,
+        )
 
-    def testFields(self):
-        self.assertPyolin(
-            'fields',
-            '''\
+    def test_fields(self):
+        self.assert_pyolin(
+            "fields",
+            """\
             | 0       | 1            | 2  | 3  | 4     |
             | ------- | ------------ | -- | -- | ----- |
             | Bucks   | Milwaukee    | 60 | 22 | 0.732 |
             | Raptors | Toronto      | 58 | 24 | 0.707 |
             | 76ers   | Philadelphia | 51 | 31 | 0.622 |
             | Celtics | Boston       | 49 | 33 | 0.598 |
             | Pacers  | Indiana      | 48 | 34 | 0.585 |
-            ''')
+            """,
+        )
 
-    def testAwkOutputFormat(self):
-        self.assertPyolin(
-            'fields',
-            '''\
+    def test_awk_output_format(self):
+        self.assert_pyolin(
+            "fields",
+            """\
             Bucks Milwaukee 60 22 0.732
             Raptors Toronto 58 24 0.707
             76ers Philadelphia 51 31 0.622
             Celtics Boston 49 33 0.598
             Pacers Indiana 48 34 0.585
-            ''',
-            output_format='awk')
+            """,
+            output_format="awk",
+        )
 
-    def testAwkOutputFormatFieldSeparator(self):
-        self.assertPyolin(
+    def test_awk_output_format_field_separator(self):
+        self.assert_pyolin(
             'printer.field_separator = ","; fields',
-            '''\
+            """\
             Bucks,Milwaukee,60,22,0.732
             Raptors,Toronto,58,24,0.707
             76ers,Philadelphia,51,31,0.622
             Celtics,Boston,49,33,0.598
             Pacers,Indiana,48,34,0.585
-            ''',
-            output_format='awk')
+            """,
+            output_format="awk",
+        )
 
-    def testAwkOutputFormatRecordSeparator(self):
-        self.assertPyolin(
+    def test_awk_output_format_record_separator(self):
+        self.assert_pyolin(
             'printer.record_separator = ";\\n"; fields',
-            '''\
+            """\
             Bucks Milwaukee 60 22 0.732;
             Raptors Toronto 58 24 0.707;
             76ers Philadelphia 51 31 0.622;
             Celtics Boston 49 33 0.598;
             Pacers Indiana 48 34 0.585;
-            ''',
-            output_format='awk')
+            """,
+            output_format="awk",
+        )
 
-    def testReorderFields(self):
-        self.assertPyolin(
-            'fields[1], fields[0]',
-            '''\
+    def test_reorder_fields(self):
+        self.assert_pyolin(
+            "fields[1], fields[0]",
+            """\
             | 0            | 1       |
             | ------------ | ------- |
             | Milwaukee    | Bucks   |
             | Toronto      | Raptors |
             | Philadelphia | 76ers   |
             | Boston       | Celtics |
             | Indiana      | Pacers  |
-            ''')
+            """,
+        )
 
-    def testConditional(self):
-        self.assertPyolin(
+    def test_conditional(self):
+        self.assert_pyolin(
             'record for record in records if record[1] == "Boston"',
-            '''\
+            """\
             | 0       | 1      | 2  | 3  | 4     |
             | ------- | ------ | -- | -- | ----- |
             | Celtics | Boston | 49 | 33 | 0.598 |
-            ''')
+            """,
+        )
 
-    def testNumberConversion(self):
-        self.assertPyolin(
-            'record.str for record in records if record[2] > 50',
-            '''\
+    def test_number_conversion(self):
+        self.assert_pyolin(
+            "record.str for record in records if record[2] > 50",
+            """\
             | value                          |
             | ------------------------------ |
             | Bucks Milwaukee    60 22 0.732 |
             | Raptors Toronto    58 24 0.707 |
             | 76ers Philadelphia 51 31 0.622 |
-            ''')
+            """,
+        )
 
-    def testExpressionRecord(self):
-        self.assertPyolin(
-            'len(records)',
-            '''\
+    def test_expression_record(self):
+        self.assert_pyolin(
+            "len(records)",
+            """\
             5
-            ''')
+            """,
+        )
 
-    def testIfExpression(self):
-        self.assertPyolin(
-            'fields[0] if fields[3] > 30',
-            '''\
+    def test_if_expression(self):
+        self.assert_pyolin(
+            "fields[0] if fields[3] > 30",
+            """\
             | value   |
             | ------- |
             | 76ers   |
             | Celtics |
             | Pacers  |
-            ''')
+            """,
+        )
 
-    def testTernaryExplicit(self):
-        self.assertPyolin(
+    def test_ternary_explicit(self):
+        self.assert_pyolin(
             'r[1] if len(r[1]) > 8 else "Name too short" for r in records',
-            '''\
+            """\
             | value          |
             | -------------- |
             | Milwaukee      |
             | Name too short |
             | Philadelphia   |
             | Name too short |
             | Name too short |
-            ''')
+            """,
+        )
 
-    def testTernaryImplicit(self):
-        self.assertPyolin(
+    def test_ternary_implicit(self):
+        self.assert_pyolin(
             'fields[1] if fields[2] > 50 else "Score too low"',
-            '''\
+            """\
             | value         |
             | ------------- |
             | Milwaukee     |
             | Toronto       |
             | Philadelphia  |
             | Score too low |
             | Score too low |
-            ''')
+            """,
+        )
 
-    def testCountCondition(self):
-        self.assertPyolin(
-            'len([r for r in records if r[2] > 50])',
-            '''\
+    def test_count_condition(self):
+        self.assert_pyolin(
+            "len([r for r in records if r[2] > 50])",
+            """\
             3
-            ''')
+            """,
+        )
 
-    def testEnumerate(self):
-        self.assertPyolin(
-            '(i, line) for i, line in enumerate(lines)',
-            '''\
+    def test_enumerate(self):
+        self.assert_pyolin(
+            "(i, line) for i, line in enumerate(lines)",
+            """\
             | 0 | 1                              |
             | - | ------------------------------ |
             | 0 | Bucks Milwaukee    60 22 0.732 |
             | 1 | Raptors Toronto    58 24 0.707 |
             | 2 | 76ers Philadelphia 51 31 0.622 |
             | 3 | Celtics Boston     49 33 0.598 |
             | 4 | Pacers Indiana     48 34 0.585 |
-            ''')
+            """,
+        )
 
-    def testSkipNone(self):
-        self.assertPyolin(
-            '[None, 1, 2, 3]',
-            '''\
+    def test_skip_none(self):
+        self.assert_pyolin(
+            "[None, 1, 2, 3]",
+            """\
             | value |
             | ----- |
             | None  |
             | 1     |
             | 2     |
             | 3     |
-            ''')
+            """,
+        )
 
-    def testSingletonNone(self):
+    def test_singleton_none(self):
         """
         Just a singleton None, not in a sequence, should be printed (maybe?)
         """
-        self.assertPyolin(
-            'None',
-            '''\
+        self.assert_pyolin(
+            "None",
+            """\
             None
-            ''')
+            """,
+        )
 
-    def testRegex(self):
-        self.assertPyolin(
+    def test_regex(self):
+        self.assert_pyolin(
             r'fields if re.match(r"^\d.*", fields[0])',
-            '''\
+            """\
             | 0     | 1            | 2  | 3  | 4     |
             | ----- | ------------ | -- | -- | ----- |
             | 76ers | Philadelphia | 51 | 31 | 0.622 |
-            ''')
+            """,
+        )
 
-    def testAddition(self):
-        self.assertPyolin(
-            'fields[2] + 100',
-            '''\
+    def test_addition(self):
+        self.assert_pyolin(
+            "fields[2] + 100",
+            """\
             | value |
             | ----- |
             | 160   |
             | 158   |
             | 151   |
             | 149   |
             | 148   |
-            ''')
+            """,
+        )
 
-    def testRadd(self):
-        self.assertPyolin(
-            '100 + fields[2]',
-            '''\
+    def test_radd(self):
+        self.assert_pyolin(
+            "100 + fields[2]",
+            """\
             | value |
             | ----- |
             | 160   |
             | 158   |
             | 151   |
             | 149   |
             | 148   |
-            ''')
+            """,
+        )
 
-    def testFieldAddition(self):
-        self.assertPyolin(
-            'fields[2] + fields[3]',
-            '''\
+    def test_field_addition(self):
+        self.assert_pyolin(
+            "fields[2] + fields[3]",
+            """\
             | value |
             | ----- |
             | 82    |
             | 82    |
             | 82    |
             | 82    |
             | 82    |
-            ''')
+            """,
+        )
 
-    def testFieldConcat(self):
-        self.assertPyolin(
-            'fields[2] + fields[0]',
-            '''\
+    def test_field_concat(self):
+        self.assert_pyolin(
+            "fields[2] + fields[0]",
+            """\
             | value     |
             | --------- |
             | 60Bucks   |
             | 58Raptors |
             | 5176ers   |
             | 49Celtics |
             | 48Pacers  |
-            ''')
+            """,
+        )
 
-    def testFieldConcatReversed(self):
-        self.assertPyolin(
-            'fields[0] + fields[2]',
-            '''\
+    def test_field_concat_reversed(self):
+        self.assert_pyolin(
+            "fields[0] + fields[2]",
+            """\
             | value     |
             | --------- |
             | Bucks60   |
             | Raptors58 |
             | 76ers51   |
             | Celtics49 |
             | Pacers48  |
-            ''')
+            """,
+        )
 
-    def testStringConcat(self):
-        self.assertPyolin(
+    def test_string_concat(self):
+        self.assert_pyolin(
             'fields[0] + "++"',
-            '''\
+            """\
             | value     |
             | --------- |
             | Bucks++   |
             | Raptors++ |
             | 76ers++   |
             | Celtics++ |
             | Pacers++  |
-            ''')
+            """,
+        )
 
-    def testLt(self):
-        self.assertPyolin(
-            'fields[0] if fields[2] < 51',
-            '''\
+    def test_lt(self):
+        self.assert_pyolin(
+            "fields[0] if fields[2] < 51",
+            """\
             | value   |
             | ------- |
             | Celtics |
             | Pacers  |
-            ''')
+            """,
+        )
 
-    def testLe(self):
-        self.assertPyolin(
-            'fields[0] if fields[2] <= 51',
-            '''\
+    def test_le(self):
+        self.assert_pyolin(
+            "fields[0] if fields[2] <= 51",
+            """\
             | value   |
             | ------- |
             | 76ers   |
             | Celtics |
             | Pacers  |
-            ''')
+            """,
+        )
 
-    def testSubtraction(self):
-        self.assertPyolin(
-            'fields[2] - 50',
-            '''\
+    def test_subtraction(self):
+        self.assert_pyolin(
+            "fields[2] - 50",
+            """\
             | value |
             | ----- |
             | 10    |
             | 8     |
             | 1     |
             | -1    |
             | -2    |
-            ''')
+            """,
+        )
 
-    def testRsub(self):
-        self.assertPyolin(
-            '50 - fields[2]',
-            '''\
+    def test_rsub(self):
+        self.assert_pyolin(
+            "50 - fields[2]",
+            """\
             | value |
             | ----- |
             | -10   |
             | -8    |
             | -1    |
             | 1     |
             | 2     |
-            ''')
+            """,
+        )
 
-    def testLeftShift(self):
-        self.assertPyolin(
-            'fields[2] << 2',
-            '''\
+    def test_left_shift(self):
+        self.assert_pyolin(
+            "fields[2] << 2",
+            """\
             | value |
             | ----- |
             | 240   |
             | 232   |
             | 204   |
             | 196   |
             | 192   |
-            ''')
+            """,
+        )
 
-    def testNeg(self):
-        self.assertPyolin(
-            '(-fields[2])',
-            '''\
+    def test_neg(self):
+        self.assert_pyolin(
+            "(-fields[2])",
+            """\
             | value |
             | ----- |
             | -60   |
             | -58   |
             | -51   |
             | -49   |
             | -48   |
-            ''')
+            """,
+        )
 
-    def testRound(self):
-        self.assertPyolin(
-            'round(fields[2], -2)',
-            '''\
+    def test_round(self):
+        self.assert_pyolin(
+            "round(fields[2], -2)",
+            """\
             | value |
             | ----- |
             | 100   |
             | 100   |
             | 100   |
             | 0     |
             | 0     |
-            ''')
+            """,
+        )
 
-    def testSkipFirstLine(self):
-        self.assertPyolin(
-            'l for l in lines[1:]',
-            '''\
+    def test_skip_first_line(self):
+        self.assert_pyolin(
+            "l for l in lines[1:]",
+            """\
             | value                          |
             | ------------------------------ |
             | Raptors Toronto    58 24 0.707 |
             | 76ers Philadelphia 51 31 0.622 |
             | Celtics Boston     49 33 0.598 |
             | Pacers Indiana     48 34 0.585 |
-            ''')
+            """,
+        )
 
-    def testAnd(self):
-        self.assertPyolin(
-            'record if fields[2] > 50 and fields[3] > 30',
-            '''\
+    def test_and(self):
+        self.assert_pyolin(
+            "record if fields[2] > 50 and fields[3] > 30",
+            """\
             | 0     | 1            | 2  | 3  | 4     |
             | ----- | ------------ | -- | -- | ----- |
             | 76ers | Philadelphia | 51 | 31 | 0.622 |
-            ''')
+            """,
+        )
 
-    def testAddHeader(self):
-        self.assertPyolin(
+    def test_add_header(self):
+        self.assert_pyolin(
             'header = ("Team", "City", "Win", "Loss", "Winrate"); records',
-            '''\
+            """\
             | Team    | City         | Win | Loss | Winrate |
             | ------- | ------------ | --- | ---- | ------- |
             | Bucks   | Milwaukee    | 60  | 22   | 0.732   |
             | Raptors | Toronto      | 58  | 24   | 0.707   |
             | 76ers   | Philadelphia | 51  | 31   | 0.622   |
             | Celtics | Boston       | 49  | 33   | 0.598   |
             | Pacers  | Indiana      | 48  | 34   | 0.585   |
-            ''')
+            """,
+        )
 
-    def testCountDots(self):
-        self.assertPyolin(
+    def test_count_dots(self):
+        self.assert_pyolin(
             'sum(line.count("0") for line in lines)',
-            '''\
+            """\
             7
-            ''')
+            """,
+        )
 
-    def testMaxScore(self):
-        self.assertPyolin(
-            'max(r[2] for r in records)',
-            '''\
+    def test_max_score(self):
+        self.assert_pyolin(
+            "max(r[2] for r in records)",
+            """\
             60
-            ''')
+            """,
+        )
 
-    def testContents(self):
-        self.assertPyolin(
-            'len(contents)',
-            '''\
+    def test_contents(self):
+        self.assert_pyolin(
+            "len(contents)",
+            """\
             154
-            ''')
+            """,
+        )
 
-    def testEmptyList(self):
-        self.assertPyolin(
-            '[]',
-            '''\
-            ''')
+    def test_empty_list(self):
+        self.assert_pyolin(
+            "[]",
+            """\
+            """,
+        )
 
-    def testStreamingStdin(self):
-        with pyolinPopen('parser.has_header = False; line', extra_args=['--output_format=awk']) as proc:
-            proc.stdin.write('Raptors Toronto    58 24 0.707\n')
+    def test_streaming_stdin(self):
+        with pyolin_popen(
+            "parser.has_header = False; line",
+            extra_args=["--input_format=awk", "--output_format=awk"],
+        ) as proc:
+            assert proc.stdin and proc.stdout
+            proc.stdin.write("Raptors Toronto    58 24 0.707\n")
             proc.stdin.flush()
             with timeout(2):
                 self.assertEqual(
-                    proc.stdout.readline(),
-                    'Raptors Toronto    58 24 0.707\n')
-            proc.stdin.write('Celtics Boston     49 33 0.598\n')
+                    proc.stdout.readline(), "Raptors Toronto    58 24 0.707\n"
+                )
+            proc.stdin.write("Celtics Boston     49 33 0.598\n")
             proc.stdin.flush()
             with timeout(2):
                 self.assertEqual(
-                    proc.stdout.readline(),
-                    'Celtics Boston     49 33 0.598\n')
+                    proc.stdout.readline(), "Celtics Boston     49 33 0.598\n"
+                )
 
-    def testClosedStdout(self):
-        with pyolinPopen('parser.has_header = False; line', extra_args=['--output_format=awk']) as proc:
-            proc.stdin.write('Raptors Toronto    58 24 0.707\n')
+    def test_closed_stdout(self):
+        with pyolin_popen(
+            "parser.has_header = False; line",
+            extra_args=["--input_format=awk", "--output_format=awk"],
+        ) as proc:
+            assert proc.stdin and proc.stdout and proc.stderr
+            proc.stdin.write("Raptors Toronto    58 24 0.707\n")
             proc.stdin.flush()
             with timeout(2):
-                self.assertEqual(proc.stdout.readline(), 'Raptors Toronto    58 24 0.707\n')
+                self.assertEqual(
+                    proc.stdout.readline(), "Raptors Toronto    58 24 0.707\n"
+                )
             # Command line tools like `head` will close the pipe when it is done getting the data
             # it needs. Make sure this doesn't crash
             proc.stdout.close()
-            proc.stdin.write('Celtics Boston     49 33 0.598\n')
+            proc.stdin.write("Celtics Boston     49 33 0.598\n")
             proc.stdin.close()
             # proc.stdin.flush()
             errmsg = proc.stderr.read()
-            self.assertEqual(errmsg, '', errmsg)
+            self.assertEqual(errmsg, "", errmsg)
 
-    def testStreamingStdinBinary(self):
-        with pyolinPopen(
-                'file[:2]',
-                extra_args=['--input_format=binary', '--output_format=binary'],
-                universal_newlines=False) as proc:
-            stdout, _ = proc.communicate(b'\x30\x62\x43\x00')  # type: ignore
-            self.assertEqual(stdout, b'\x30\x62')
-
-    def testStreamingSlice(self):
-        with pyolinPopen(
-                'parser.has_header = False; records[:2]', extra_args=['--output_format=awk']) as proc:
-            proc.stdin.write('Raptors Toronto    58 24 0.707\n')
-            proc.stdin.write('Celtics Boston     49 33 0.598\n')
+    def test_streaming_stdin_binary(self):
+        with pyolin_popen(
+            "file[:2]",
+            extra_args=["--output_format=binary"],
+            universal_newlines=False,
+        ) as proc:
+            stdout, _ = proc.communicate(b"\x30\x62\x43\x00")  # type: ignore
+            self.assertEqual(stdout, b"\x30\x62")
+
+    def test_streaming_slice(self):
+        with pyolin_popen(
+            "parser.has_header = False; records[:2]",
+            extra_args=["--input_format=awk", "--output_format=awk"],
+        ) as proc:
+            assert proc.stdin and proc.stdout
+            proc.stdin.write("Raptors Toronto    58 24 0.707\n")
+            proc.stdin.write("Celtics Boston     49 33 0.598\n")
             proc.stdin.flush()
             with timeout(2):
                 self.assertEqual(
-                    proc.stdout.readline(),
-                    'Raptors Toronto 58 24 0.707\n')
+                    proc.stdout.readline(), "Raptors Toronto 58 24 0.707\n"
+                )
+                self.assertEqual(proc.stdout.readline(), "Celtics Boston 49 33 0.598\n")
+            proc.stdin.write("Write more stuff...\n")
+
+    def test_streaming_index(self):
+        with pyolin_popen(
+            "parser.has_header = False; records[1].str",
+            extra_args=["--input_format=awk", "--output_format=awk"],
+        ) as proc:
+            assert proc.stdin and proc.stdout
+            proc.stdin.write("Raptors Toronto    58 24 0.707\n")
+            proc.stdin.write("Celtics Boston     49 33 0.598\n")
+            proc.stdin.flush()
+            with timeout(2):
                 self.assertEqual(
-                    proc.stdout.readline(),
-                    'Celtics Boston 49 33 0.598\n')
-            proc.stdin.write('Write more stuff...\n')
-
-    def testStreamingIndex(self):
-        with pyolinPopen(
-                'parser.has_header = False; records[1].str',
-                extra_args=['--output_format=awk']) as proc:
-            proc.stdin.write('Raptors Toronto    58 24 0.707\n')
-            proc.stdin.write('Celtics Boston     49 33 0.598\n')
+                    proc.stdout.readline(), "Celtics Boston     49 33 0.598\n"
+                )
+            proc.stdin.write("Write more stuff...\n")
+
+    def test_streaming_index_with_auto_parser(self):
+        with pyolin_popen(
+            "parser.has_header = False; records[1].str",
+            extra_args=["--output_format=awk"],
+        ) as proc:
+            assert proc.stdin and proc.stdout
+            proc.stdin.write("Raptors Toronto    58 24 0.707\n")
+            proc.stdin.write("Celtics Boston     49 33 0.598\n")
+            proc.stdin.write("Warriors GS        49 33 0.598\n")
+            proc.stdin.write("Lakers LA          49 33 0.598\n")
+            proc.stdin.write("Bucks Milwaukee    49 33 0.598\n")
+            proc.stdin.write("76ers Philly       49 33 0.598\n")
             proc.stdin.flush()
             with timeout(2):
                 self.assertEqual(
-                    proc.stdout.readline(),
-                    'Celtics Boston     49 33 0.598\n')
-            proc.stdin.write('Write more stuff...\n')
-
-    def testRecordsIndex(self):
-        self.assertPyolin(
-            'records[1]',
-            '''\
+                    proc.stdout.readline(), "Celtics Boston     49 33 0.598\n"
+                )
+            proc.stdin.write("Write more stuff...\n")
+
+    def test_records_index(self):
+        self.assert_pyolin(
+            "records[1]",
+            """\
             Raptors Toronto 58 24 0.707
-            ''')
+            """,
+        )
 
-    def testDestructuring(self):
-        self.assertPyolin(
-            'city for team, city, _, _, _ in records',
-            '''\
+    def test_destructuring(self):
+        self.assert_pyolin(
+            "city for team, city, _, _, _ in records",
+            """\
             | value        |
             | ------------ |
             | Milwaukee    |
             | Toronto      |
             | Philadelphia |
             | Boston       |
             | Indiana      |
-            ''')
+            """,
+        )
 
-    def testPercentage(self):
-        self.assertPyolin(
-            '(r[0], round(r[3] / sum(r[3] for r in records), 2)) '
-            'for r in records',
-            '''\
+    def test_percentage(self):
+        self.assert_pyolin(
+            "(r[0], round(r[3] / sum(r[3] for r in records), 2)) " "for r in records",
+            """\
             | 0       | 1    |
             | ------- | ---- |
             | Bucks   | 0.15 |
             | Raptors | 0.17 |
             | 76ers   | 0.22 |
             | Celtics | 0.23 |
             | Pacers  | 0.24 |
-            ''')
+            """,
+        )
 
-    def testSingletonTuple(self):
+    def test_singleton_tuple(self):
         """
         Tuples are treated as fields in a single record, whereas other iterable
         types are treated as multiple records.
         """
-        self.assertPyolin(
-            'sum(r[3] for r in records), max(r[3] for r in records)',
-            '''\
+        self.assert_pyolin(
+            "sum(r[3] for r in records), max(r[3] for r in records)",
+            """\
             144 34
-            ''')
+            """,
+        )
 
-    def testModuleImport(self):
-        self.assertPyolin(
+    def test_module_import(self):
+        self.assert_pyolin(
             'record[0] if fnmatch.fnmatch(record[0], "*.txt")',
-            '''\
+            """\
             | value                  |
             | ---------------------- |
             | dir/file.txt           |
             | dir/file1.txt          |
             | dir/fileb.txt          |
             | dir/subdir/subfile.txt |
-            ''',
-            input='data_files.txt')
+            """,
+            input_file="data_files.txt",
+        )
 
-    def testRecordVariables(self):
-        self.assertPyolin(
-            'type(record).__name__, type(line).__name__, '
-            'type(fields).__name__',
-            '''\
+    def test_record_variables(self):
+        self.assert_pyolin(
+            "type(record).__name__, type(line).__name__, type(fields).__name__",
+            """\
             | 0      | 1   | 2      |
             | ------ | --- | ------ |
             | Record | str | Record |
             | Record | str | Record |
             | Record | str | Record |
             | Record | str | Record |
             | Record | str | Record |
-            ''')
+            """,
+        )
 
-    def testFileVariables(self):
-        self.assertPyolin(
-            'type(lines).__name__, type(records).__name__, '
-            'type(file).__name__, type(contents).__name__',
-            '''\
+    def test_file_variables(self):
+        self.assert_pyolin(
+            "type(lines).__name__, type(records).__name__, "
+            "type(file).__name__, type(contents).__name__",
+            """\
             StreamingSequence RecordSequence str str
-            ''')
+            """,
+        )
 
-    def testBoolean(self):
-        self.assertPyolin(
-            'record if record[1].bool',
-            '''\
+    def test_boolean(self):
+        self.assert_pyolin(
+            "record if record[1].bool",
+            """\
             | 0          | 1    | 2  | 3    |
             | ---------- | ---- | -- | ---- |
             | dir        | True | 30 | 40.0 |
             | dir/subdir | True | 12 | 42.0 |
-            ''',
-            input='data_files.txt')
+            """,
+            input_file="data_files.txt",
+        )
 
-    def testAwkHeaderDetection(self):
-        self.assertPyolin(
-            'record if record[1].bool',
-            '''\
+    def test_awk_header_detection(self):
+        self.assert_pyolin(
+            "record if record[1].bool",
+            """\
             | Path       | IsDir | Size | Score |
             | ---------- | ----- | ---- | ----- |
             | dir        | True  | 30   | 40.0  |
             | dir/subdir | True  | 12   | 42.0  |
-            ''',
-            input='data_files_with_header.txt')
+            """,
+            input_file="data_files_with_header.txt",
+        )
 
-    def testFilename(self):
-        self.assertPyolin(
-            'filename',
-            f'''\
+    def test_awk_output_with_header(self):
+        self.assert_pyolin(
+            "record if record[1].bool",
+            """\
+            Path IsDir Size Score
+            dir True 30 40.0
+            dir/subdir True 12 42.0
+            """,
+            input_file="data_files_with_header.txt",
+            output_format="awk",
+        )
+
+    def test_filename(self):
+        self.assert_pyolin(
+            "filename",
+            f"""\
             {os.path.dirname(__file__)}/data_files.txt
-            ''',
-            input='data_files.txt')
+            """,
+            input_file="data_files.txt",
+        )
 
-    def testBytes(self):
-        self.assertPyolin(
+    def test_bytes(self):
+        self.assert_pyolin(
             'b"hello"',
-            '''\
+            """\
             hello
-            ''')
+            """,
+        )
 
-    def testReversed(self):
-        self.assertPyolin(
-            'reversed(lines)',
-            '''\
+    def test_reversed(self):
+        self.assert_pyolin(
+            "reversed(lines)",
+            """\
             | value                          |
             | ------------------------------ |
             | Pacers Indiana     48 34 0.585 |
             | Celtics Boston     49 33 0.598 |
             | 76ers Philadelphia 51 31 0.622 |
             | Raptors Toronto    58 24 0.707 |
             | Bucks Milwaukee    60 22 0.732 |
-            ''')
+            """,
+        )
 
-    def testInOperator(self):
-        self.assertPyolin(
+    def test_in_operator(self):
+        self.assert_pyolin(
             '"Raptors Toronto    58 24 0.707" in lines',
-            '''\
+            """\
             True
-            ''')
+            """,
+        )
 
-    def testBase64(self):
-        self.assertPyolin(
-            'base64.b64encode(fields[0].bytes)',
-            '''\
+    def test_base64(self):
+        self.assert_pyolin(
+            "base64.b64encode(fields[0].bytes)",
+            """\
             | value        |
             | ------------ |
             | QnVja3M=     |
             | UmFwdG9ycw== |
             | NzZlcnM=     |
             | Q2VsdGljcw== |
             | UGFjZXJz     |
-            ''')
+            """,
+        )
 
-    def testUrlQuote(self):
-        self.assertPyolin(
-            'urllib.parse.quote(line)',
-            '''\
+    def test_url_quote(self):
+        self.assert_pyolin(
+            "urllib.parse.quote(line)",
+            """\
             | value                                          |
             | ---------------------------------------------- |
             | Bucks%20Milwaukee%20%20%20%2060%2022%200.732   |
             | Raptors%20Toronto%20%20%20%2058%2024%200.707   |
             | 76ers%20Philadelphia%2051%2031%200.622         |
             | Celtics%20Boston%20%20%20%20%2049%2033%200.598 |
             | Pacers%20Indiana%20%20%20%20%2048%2034%200.585 |
-            ''')
+            """,
+        )
 
-    def testFieldsEqual(self):
-        self.assertPyolin(
-            'fields[2], fields[3], fields[2] == fields[3]',
-            '''\
+    def test_fields_equal(self):
+        self.assert_pyolin(
+            "fields[2], fields[3], fields[2] == fields[3]",
+            """\
             | 0  | 1    | 2     |
             | -- | ---- | ----- |
             | 30 | 40.0 | False |
             | 40 | 32.0 | False |
             | 23 | 56.0 | False |
             | 15 | 85.0 | False |
             | 31 | 31.0 | True  |
             | 44 | 16.0 | False |
             | 12 | 42.0 | False |
             | 11 | 53.0 | False |
-            ''',
-            input='data_files.txt')
+            """,
+            input_file="data_files.txt",
+        )
 
-    def testFieldsComparison(self):
-        self.assertPyolin(
-            'fields[2], fields[3], fields[2] >= fields[3]',
-            '''\
+    def test_fields_comparison(self):
+        self.assert_pyolin(
+            "fields[2], fields[3], fields[2] >= fields[3]",
+            """\
             | 0  | 1    | 2     |
             | -- | ---- | ----- |
             | 30 | 40.0 | False |
             | 40 | 32.0 | True  |
             | 23 | 56.0 | False |
             | 15 | 85.0 | False |
             | 31 | 31.0 | True  |
             | 44 | 16.0 | True  |
             | 12 | 42.0 | False |
             | 11 | 53.0 | False |
-            ''',
-            input='data_files.txt')
+            """,
+            input_file="data_files.txt",
+        )
 
-    def testMultiplication(self):
-        self.assertPyolin(
-            'fields[3] * 10',
-            '''\
+    def test_multiplication(self):
+        self.assert_pyolin(
+            "fields[3] * 10",
+            """\
             | value |
             | ----- |
             | 220   |
             | 240   |
             | 310   |
             | 330   |
             | 340   |
-            ''')
+            """,
+        )
 
-    def testFieldsMultiplication(self):
-        self.assertPyolin(
-            'fields[3] * fields[2]',
-            '''\
+    def test_fields_multiplication(self):
+        self.assert_pyolin(
+            "fields[3] * fields[2]",
+            """\
             | value |
             | ----- |
             | 1320  |
             | 1392  |
             | 1581  |
             | 1617  |
             | 1632  |
-            ''')
+            """,
+        )
 
-    def testStringMultiplication(self):
-        self.assertPyolin(
-            'fields[0] * 2',
-            '''\
+    def test_string_multiplication(self):
+        self.assert_pyolin(
+            "fields[0] * 2",
+            """\
             | value          |
             | -------------- |
             | BucksBucks     |
             | RaptorsRaptors |
             | 76ers76ers     |
             | CelticsCeltics |
             | PacersPacers   |
-            ''')
+            """,
+        )
 
-    def testPandasDataframe(self):
-        self.assertPyolin(
-            'df',
-            '''\
+    def test_pandas_dataframe(self):
+        self.assert_pyolin(
+            "df",
+            """\
             | 0       | 1            | 2  | 3  | 4     |
             | ------- | ------------ | -- | -- | ----- |
             | Bucks   | Milwaukee    | 60 | 22 | 0.732 |
             | Raptors | Toronto      | 58 | 24 | 0.707 |
             | 76ers   | Philadelphia | 51 | 31 | 0.622 |
             | Celtics | Boston       | 49 | 33 | 0.598 |
             | Pacers  | Indiana      | 48 | 34 | 0.585 |
-            ''')
+            """,
+        )
 
-    def testPandasDtypes(self):
-        self.assertPyolin(
-            'df.dtypes',
-            '''\
+    def test_pandas_dtypes(self):
+        self.assert_pyolin(
+            "df.dtypes",
+            """\
             | value   |
             | ------- |
             | object  |
             | object  |
             | int64   |
             | int64   |
             | float64 |
-            ''')
+            """,
+        )
 
-    def testPandaNumericOperations(self):
-        self.assertPyolin(
-            'df[2] * 2',
-            '''\
+    def test_panda_numeric_operations(self):
+        self.assert_pyolin(
+            "df[2] * 2",
+            """\
             | value |
             | ----- |
             | 120   |
             | 116   |
             | 102   |
             | 98    |
             | 96    |
-            ''')
+            """,
+        )
 
-    def testNumpyNumericOperations(self):
-        self.assertPyolin(
-            'np.power(df[2], 2)',
-            '''\
+    def test_numpy_numeric_operations(self):
+        self.assert_pyolin(
+            "np.power(df[2], 2)",
+            """\
             | value |
             | ----- |
             | 3600  |
             | 3364  |
             | 2601  |
             | 2401  |
             | 2304  |
-            ''')
+            """,
+        )
 
-    def testFieldSeparator(self):
-        self.assertPyolin(
-            'record',
-            '''\
+    def test_field_separator(self):
+        self.assert_pyolin(
+            "record",
+            """\
             | 0         | 1          | 2           | 3    | 4    | 5     | 6    | 7    | 8  |
             | --------- | ---------- | ----------- | ---- | ---- | ----- | ---- | ---- | -- |
             | Alfalfa   | Aloysius   | 123-45-6789 | 40.0 | 90.0 | 100.0 | 83.0 | 49.0 | D- |
             | Alfred    | University | 123-12-1234 | 41.0 | 97.0 | 96.0  | 97.0 | 48.0 | D+ |
             | Gerty     | Gramma     | 567-89-0123 | 41.0 | 80.0 | 60.0  | 40.0 | 44.0 | C  |
             | Android   | Electric   | 087-65-4321 | 42.0 | 23.0 | 36.0  | 45.0 | 47.0 | B- |
             | Franklin  | Benny      | 234-56-2890 | 50.0 | 1.0  | 90.0  | 80.0 | 90.0 | B- |
             | George    | Boy        | 345-67-3901 | 40.0 | 1.0  | 11.0  | -1.0 | 4.0  | B  |
             | Heffalump | Harvey     | 632-79-9439 | 30.0 | 1.0  | 20.0  | 30.0 | 40.0 | C  |
-            ''',
-            input='data_grades_simple_csv.csv',
-            field_separator=r',')
+            """,
+            input_file="data_grades_simple_csv.csv",
+            field_separator=r",",
+        )
 
-    def testFieldSeparatorRegex(self):
-        self.assertPyolin(
-            'record',
-            '''\
-    | 0         | 1          | 2           | 3  | 4 | 5  | 6 | 7   | 8 | 9  | 10 | 11 | 12 | 13 |
-    | --------- | ---------- | ----------- | -- | - | -- | - | --- | - | -- | -- | -- | -- | -- |
-    | Alfalfa   | Aloysius   | 123-45-6789 | 40 | 0 | 90 | 0 | 100 | 0 | 83 | 0  | 49 | 0  | D- |
-    | Alfred    | University | 123-12-1234 | 41 | 0 | 97 | 0 | 96  | 0 | 97 | 0  | 48 | 0  | D+ |
-    | Gerty     | Gramma     | 567-89-0123 | 41 | 0 | 80 | 0 | 60  | 0 | 40 | 0  | 44 | 0  | C  |
-    | Android   | Electric   | 087-65-4321 | 42 | 0 | 23 | 0 | 36  | 0 | 45 | 0  | 47 | 0  | B- |
-    | Franklin  | Benny      | 234-56-2890 | 50 | 0 | 1  | 0 | 90  | 0 | 80 | 0  | 90 | 0  | B- |
-    | George    | Boy        | 345-67-3901 | 40 | 0 | 1  | 0 | 11  | 0 | -1 | 0  | 4  | 0  | B  |
-    | Heffalump | Harvey     | 632-79-9439 | 30 | 0 | 1  | 0 | 20  | 0 | 30 | 0  | 40 | 0  | C  |
-    ''',
-            input='data_grades_simple_csv.csv',
-            field_separator=r'[\.,]')
-
-    def testRecordSeparator(self):
-        self.assertPyolin(
-            'record',
-            '''\
+    def test_field_separator_regex(self):
+        self.assert_pyolin(
+            "record",
+            # pylint:disable=line-too-long
+            """\
+            | 0         | 1          | 2           | 3  | 4 | 5  | 6 | 7   | 8 | 9  | 10 | 11 | 12 | 13 |
+            | --------- | ---------- | ----------- | -- | - | -- | - | --- | - | -- | -- | -- | -- | -- |
+            | Alfalfa   | Aloysius   | 123-45-6789 | 40 | 0 | 90 | 0 | 100 | 0 | 83 | 0  | 49 | 0  | D- |
+            | Alfred    | University | 123-12-1234 | 41 | 0 | 97 | 0 | 96  | 0 | 97 | 0  | 48 | 0  | D+ |
+            | Gerty     | Gramma     | 567-89-0123 | 41 | 0 | 80 | 0 | 60  | 0 | 40 | 0  | 44 | 0  | C  |
+            | Android   | Electric   | 087-65-4321 | 42 | 0 | 23 | 0 | 36  | 0 | 45 | 0  | 47 | 0  | B- |
+            | Franklin  | Benny      | 234-56-2890 | 50 | 0 | 1  | 0 | 90  | 0 | 80 | 0  | 90 | 0  | B- |
+            | George    | Boy        | 345-67-3901 | 40 | 0 | 1  | 0 | 11  | 0 | -1 | 0  | 4  | 0  | B  |
+            | Heffalump | Harvey     | 632-79-9439 | 30 | 0 | 1  | 0 | 20  | 0 | 30 | 0  | 40 | 0  | C  |
+            """,
+            # pylint:enable=line-too-long
+            input_file="data_grades_simple_csv.csv",
+            field_separator=r"[\.,]",
+            input_format="awk",
+        )
+
+    def test_record_separator(self):
+        self.assert_pyolin(
+            "record",
+            """\
             | value     |
             | --------- |
             | JET       |
             | 20031201  |
             | 20001006  |
             | 53521     |
             | 1.000E+01 |
@@ -919,37 +1053,39 @@
             | TRANS     |
             | 2.000E+00 |
             | 1.000E+00 |
             | 2         |
             | 1         |
             | 0         |
             | 0         |
-            ''',
-            input='data_onerow.csv',
-            record_separator=r',')
+            """,
+            input_file="data_onerow.csv",
+            record_separator=r",",
+        )
 
-    def testRecordSeparatorMultipleChars(self):
-        self.assertPyolin(
-            'parser.has_header=False; record',
-            '''\
-            | value                                    |
-            | ---------------------------------------- |
-            | JET                                      |
-            | 0031201                                  |
-            | 0001006,53521,1.000E+01,NBIC,HSELM,TRANS |
-            | .000E+00,1.000E+00                       |
-            | ,1,0,0                                   |
-            ''',
-            input='data_onerow.csv',
-            record_separator=r',2')
+    def test_record_separator_multiple_chars(self):
+        self.assert_pyolin(
+            "parser.has_header=False; record",
+            """\
+            | value    |
+            | -------- |
+            | JET      |
+            | 0031201  |
+            | 0001006  | 53521 | 1.000E+01 | NBIC | HSELM | TRANS |
+            | .000E+00 | 1.000E+00 |
+            |          | 1 | 0 | 0 |
+            """,
+            input_file="data_onerow.csv",
+            record_separator=r",2",
+        )
 
-    def testRecordSeparatorRegex(self):
-        self.assertPyolin(
-            'record',
-            '''\
+    def test_record_separator_regex(self):
+        self.assert_pyolin(
+            "record",
+            """\
             | value    |
             | -------- |
             | JET      |
             | 20031201 |
             | 20001006 |
             | 53521    |
             | 1        |
@@ -961,522 +1097,559 @@
             | 000E+00  |
             | 1        |
             | 000E+00  |
             | 2        |
             | 1        |
             | 0        |
             | 0        |
-            ''',
-            input='data_onerow.csv',
-            record_separator=r'[,.]')
+            """,
+            input_file="data_onerow.csv",
+            record_separator=r"[,.]",
+        )
 
-    def testSimpleCsv(self):
-        self.assertPyolin(
-            'df[[0, 1, 2]]',
-            '''\
+    def test_simple_csv(self):
+        self.assert_pyolin(
+            "df[[0, 1, 2]]",
+            """\
             | 0         | 1          | 2           |
             | --------- | ---------- | ----------- |
             | Alfalfa   | Aloysius   | 123-45-6789 |
             | Alfred    | University | 123-12-1234 |
             | Gerty     | Gramma     | 567-89-0123 |
             | Android   | Electric   | 087-65-4321 |
             | Franklin  | Benny      | 234-56-2890 |
             | George    | Boy        | 345-67-3901 |
             | Heffalump | Harvey     | 632-79-9439 |
-            ''',
-            input='data_grades_simple_csv.csv',
-            input_format='csv')
+            """,
+            input_file="data_grades_simple_csv.csv",
+            input_format="csv",
+        )
 
-    def testQuotedCsv(self):
-        self.assertPyolin(
-            'record[0]',
-            '''\
+    def test_quoted_csv(self):
+        self.assert_pyolin(
+            "record[0]",
+            """\
             | value            |
             | ---------------- |
             | 60 Minutes       |
             | 48 Hours Mystery |
             | 20/20            |
             | Nightline        |
             | Dateline Friday  |
             | Dateline Sunday  |
-            ''',
-            input='data_news_decline.csv',
-            input_format='csv')
+            """,
+            input_file="data_news_decline.csv",
+            input_format="csv",
+        )
 
-    def testQuotedCsvStr(self):
-        self.assertPyolin(
-            'record.str',
-            '''\
+    def test_quoted_csv_str(self):
+        self.assert_pyolin(
+            "record.str",
+            """\
             | value                             |
             | --------------------------------- |
             | "60 Minutes",       7.6, 7.4, 7.3 |
             | "48 Hours Mystery", 4.1, 3.9, 3.6 |
             | "20/20",            4.1, 3.7, 3.3 |
             | "Nightline",        2.7, 2.6, 2.7 |
             | "Dateline Friday",  4.1, 4.1, 3.9 |
             | "Dateline Sunday",  3.5, 3.2, 3.1 |
-            ''',
-            input='data_news_decline.csv',
-            input_format='csv')
+            """,
+            input_file="data_news_decline.csv",
+            input_format="csv",
+        )
 
-    def testAutoCsv(self):
-        self.assertPyolin(
-            'df[[0,1,2]]',
-            '''\
+    def test_auto_csv(self):
+        self.assert_pyolin(
+            "df[[0,1,2]]",
+            """\
             | 0                     | 1        | 2                                |
             | --------------------- | -------- | -------------------------------- |
             | John                  | Doe      | 120 jefferson st.                |
             | Jack                  | McGinnis | 220 hobo Av.                     |
             | John "Da Man"         | Repici   | 120 Jefferson St.                |
             | Stephen               | Tyler    | 7452 Terrace "At the Plaza" road |
             |                       | Blankman |                                  |
             | Joan "the bone", Anne | Jet      | 9th, at Terrace plc              |
-            ''',
-            input='data_addresses.csv',
-            input_format='csv')
+            """,
+            input_file="data_addresses.csv",
+            input_format="csv",
+        )
 
-    def testCsvExcel(self):
-        self.assertPyolin(
-            'df[[0,1,2]]',
-            '''\
+    def test_csv_excel(self):
+        self.assert_pyolin(
+            "df[[0,1,2]]",
+            """\
             | 0                     | 1        | 2                                |
             | --------------------- | -------- | -------------------------------- |
             | John                  | Doe      | 120 jefferson st.                |
             | Jack                  | McGinnis | 220 hobo Av.                     |
             | John "Da Man"         | Repici   | 120 Jefferson St.                |
             | Stephen               | Tyler    | 7452 Terrace "At the Plaza" road |
             |                       | Blankman |                                  |
             | Joan "the bone", Anne | Jet      | 9th, at Terrace plc              |
-            ''',
-            input='data_addresses.csv',
-            input_format='csv_excel')
+            """,
+            input_file="data_addresses.csv",
+            input_format="csv_excel",
+        )
 
-    def testCsvUnix(self):
-        self.assertPyolin(
+    def test_csv_unix(self):
+        self.assert_pyolin(
             '"|".join((record[0], record[1], record[2]))',
-            '''\
+            """\
             | value                                          |
             | ---------------------------------------------- |
             | John|Doe|120 jefferson st.                     |
             | Jack|McGinnis|220 hobo Av.                     |
             | John "Da Man"|Repici|120 Jefferson St.         |
             | Stephen|Tyler|7452 Terrace "At the Plaza" road |
             | |Blankman|                                     |
             | Joan "the bone", Anne|Jet|9th, at Terrace plc  |
-            ''',
-            input='data_addresses_unix.csv',
-            input_format='csv')
+            """,
+            input_file="data_addresses_unix.csv",
+            input_format="csv",
+        )
 
-    def testQuotedTsv(self):
-        self.assertPyolin(
-            'record[0], record[2]',
-            '''\
+    def test_quoted_tsv(self):
+        self.assert_pyolin(
+            "record[0], record[2]",
+            """\
             | 0                | 1   |
             | ---------------- | --- |
             | 60 Minutes       | 7.4 |
             | 48 Hours Mystery | 3.9 |
             | 20/20            | 3.7 |
             | Nightline        | 2.6 |
             | Dateline Friday  | 4.1 |
             | Dateline Sunday  | 3.2 |
-            ''',
-            input='data_news_decline.tsv',
-            input_format='csv',
-            field_separator='\t')
-
-    def testStatement(self):
-        self.assertPyolin(
-            'a = record[2]; b = 1; a + b',
-            '''\
+            """,
+            input_file="data_news_decline.tsv",
+            input_format="csv",
+            field_separator="\t",
+        )
+
+    def test_statement(self):
+        self.assert_pyolin(
+            "a = record[2]; b = 1; a + b",
+            """\
             | value |
             | ----- |
             | 61    |
             | 59    |
             | 52    |
             | 50    |
             | 49    |
-            ''')
+            """,
+        )
 
-    def testStatementTable(self):
-        self.assertPyolin(
-            'a = len(records); b = 2; a * b',
-            '''\
+    def test_statement_table(self):
+        self.assert_pyolin(
+            "a = len(records); b = 2; a * b",
+            """\
             10
-            ''')
+            """,
+        )
 
-    def testSyntaxError(self):
+    def test_syntax_error(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('a..x')
+            run_cli("a..x")
         self.assertEqual(
-            textwrap.dedent('''\
+            textwrap.dedent(
+                """\
                 Invalid syntax:
                   a..x
-                    ^'''),
-            str(context.exception.__cause__))
+                    ^"""
+            ),
+            str(context.exception.__cause__),
+        )
 
-    def testSyntaxErrorInStatement(self):
+    def test_syntax_error_in_statement(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('a..x; a+1')
+            run_cli("a..x; a+1")
         self.assertEqual(
-            textwrap.dedent('''\
+            textwrap.dedent(
+                """\
                 Invalid syntax:
                   a..x
-                    ^'''),
-            str(context.exception.__cause__))
+                    ^"""
+            ),
+            str(context.exception.__cause__),
+        )
 
-    def testHeaderDetection(self):
-        self.assertPyolin(
+    def test_header_detection(self):
+        self.assert_pyolin(
             'df[["Last name", "SSN", "Final"]]',
-            '''\
+            """\
             | Last name | SSN         | Final |
             | --------- | ----------- | ----- |
             | Alfalfa   | 123-45-6789 | 49    |
             | Alfred    | 123-12-1234 | 48    |
             | Gerty     | 567-89-0123 | 44    |
             | Android   | 087-65-4321 | 47    |
             | Franklin  | 234-56-2890 | 90    |
             | George    | 345-67-3901 | 4     |
             | Heffalump | 632-79-9439 | 40    |
-            ''',
-            input='data_grades_with_header.csv',
-            input_format='csv')
+            """,
+            input_file="data_grades_with_header.csv",
+            input_format="csv",
+        )
 
-    def testForceHasHeader(self):
-        self.assertPyolin(
-            'parser.has_header = True; (r[0], r[2], r[7]) for r in records',
-            '''\
+    def test_force_has_header(self):
+        self.assert_pyolin(
+            "parser.has_header = True; (r[0], r[2], r[7]) for r in records",
+            """\
             | Alfalfa   | 123-45-6789 | 49.0 |
             | --------- | ----------- | ---- |
             | Alfred    | 123-12-1234 | 48.0 |
             | Gerty     | 567-89-0123 | 44.0 |
             | Android   | 087-65-4321 | 47.0 |
             | Franklin  | 234-56-2890 | 90.0 |
             | George    | 345-67-3901 | 4.0  |
             | Heffalump | 632-79-9439 | 40.0 |
-            ''',
-            input='data_grades_simple_csv.csv',
-            input_format='csv')
+            """,
+            input_file="data_grades_simple_csv.csv",
+            input_format="csv",
+        )
 
-    def testHeaderDetectionCsvExcel(self):
-        self.assertPyolin(
+    def test_header_detection_csv_excel(self):
+        self.assert_pyolin(
             'df[["Last Name", "Address"]]',
-            '''\
+            """\
             | Last Name             | Address                          |
             | --------------------- | -------------------------------- |
             | John                  | 120 jefferson st.                |
             | Jack                  | 220 hobo Av.                     |
             | John "Da Man"         | 120 Jefferson St.                |
             | Stephen               | 7452 Terrace "At the Plaza" road |
             | Joan "the bone", Anne | 9th, at Terrace plc              |
-            ''',
-            input='data_addresses_with_header.csv',
-            input_format='csv_excel')
+            """,
+            input_file="data_addresses_with_header.csv",
+            input_format="csv_excel",
+        )
 
-    def testPrintDataframeHeader(self):
-        self.assertPyolin(
-            'list(df.columns.values)',
-            '''\
+    def test_print_dataframe_header(self):
+        self.assert_pyolin(
+            "list(df.columns.values)",
+            """\
             | value      |
             | ---------- |
             | Last name  |
             | First name |
             | SSN        |
             | Test1      |
             | Test2      |
             | Test3      |
             | Test4      |
             | Final      |
             | Grade      |
-            ''',
-            input='data_grades_with_header.csv',
-            input_format='csv')
+            """,
+            input_file="data_grades_with_header.csv",
+            input_format="csv",
+        )
 
-    def testAssignToRecord(self):
-        '''
+    def test_assign_to_record(self):
+        """
         Try to confuse the parser by writing to a field called record
-        '''
-        self.assertPyolin(
-            'record=1; record+1',
-            '''\
+        """
+        self.assert_pyolin(
+            "record=1; record+1",
+            """\
             2
-            ''')
+            """,
+        )
 
-    def testAccessRecordAndTable(self):
+    def test_access_record_and_table(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('a = record[0]; b = records; b')
+            run_cli("a = record[0]; b = records; b")
         self.assertEqual(
-            'Cannot access both record scoped and table scoped variables',
-            str(context.exception.__cause__.__cause__))
+            "Cannot access both record scoped and table scoped variables",
+            str(context.exception.__cause__.__cause__),
+        )
 
-    def testAccessTableAndRecord(self):
+    def test_access_table_and_record(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('a = records; b = record[0]; b')
+            run_cli("a = records; b = record[0]; b")
         self.assertEqual(
-            'Cannot access both record scoped and table scoped variables',
-            str(context.exception.__cause__.__cause__))
+            "Cannot access both record scoped and table scoped variables",
+            str(context.exception.__cause__.__cause__),
+        )
 
-    def testEmptyRecordScoped(self):
-        self.assertPyolin(
-            'record[0]',
-            '',
-            input=os.devnull)
-
-    def testEmptyTableScoped(self):
-        self.assertPyolin(
-            'record for record in records',
-            '',
-            input=os.devnull)
-
-    def testSemicolonInString(self):
-        self.assertPyolin(
-            '"hello; world"',
-            'hello; world\n')
+    def test_empty_record_scoped(self):
+        self.assert_pyolin("record[0]", "", input_file=os.devnull)
 
-    def testStackTraceCleaning(self):
+    def test_empty_table_scoped(self):
+        self.assert_pyolin("record for record in records", "", input_file=os.devnull)
+
+    def test_semicolon_in_string(self):
+        self.assert_pyolin('"hello; world"', "hello; world\n")
+
+    def test_stack_trace_cleaning(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('urllib.parse.quote(12345)')
+            run_cli("urllib.parse.quote(12345)")
         assert isinstance(context.exception.__cause__, UserError)
         formatted = context.exception.__cause__.formatted_tb()
         self.assertEqual(5, len(formatted), pformat(formatted))
-        self.assertIn('Traceback (most recent call last)', formatted[0])
-        self.assertIn('pyolin_user_prog.py', formatted[1])
-        self.assertIn('return quote_from_bytes', formatted[2])
+        self.assertIn("Traceback (most recent call last)", formatted[0])
+        self.assertIn("pyolin_user_prog.py", formatted[1])
+        self.assertIn("return quote_from_bytes", formatted[2])
         self.assertIn('"quote_from_bytes() expected bytes"', formatted[3])
-        self.assertIn('quote_from_bytes() expected bytes', formatted[4])
+        self.assertIn("quote_from_bytes() expected bytes", formatted[4])
 
-    def testInvalidOutputFormat(self):
+    def test_invalid_output_format(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('1+1', output_format='invalid')
+            run_cli("1+1", output_format="invalid")
         self.assertEqual(
-            'Unrecognized output format "invalid"',
-            str(context.exception.__cause__))
+            'Unrecognized output format "invalid"', str(context.exception.__cause__)
+        )
 
-    def testCsvOutputFormat(self):
-        self.assertPyolin(
-            'records',
-            '''\
+    def test_csv_output_format(self):
+        self.assert_pyolin(
+            "records",
+            """\
             Bucks,Milwaukee,60,22,0.732\r
             Raptors,Toronto,58,24,0.707\r
             76ers,Philadelphia,51,31,0.622\r
             Celtics,Boston,49,33,0.598\r
             Pacers,Indiana,48,34,0.585\r
-            ''',
-            output_format='csv')
+            """,
+            output_format="csv",
+        )
 
-    def testCsvOutputFormatUnix(self):
-        self.assertPyolin(
-            'printer.dialect = csv.unix_dialect; records',
-            '''\
+    def test_csv_output_format_unix(self):
+        self.assert_pyolin(
+            "printer.dialect = csv.unix_dialect; records",
+            """\
             "Bucks","Milwaukee","60","22","0.732"
             "Raptors","Toronto","58","24","0.707"
             "76ers","Philadelphia","51","31","0.622"
             "Celtics","Boston","49","33","0.598"
             "Pacers","Indiana","48","34","0.585"
-            ''',
-            output_format='csv')
+            """,
+            output_format="csv",
+        )
 
-    def testCsvOutputInvalidDialect(self):
+    def test_csv_output_invalid_dialect(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('printer.dialect = "invalid"; records', output_format='csv')
-        self.assertEqual(
-            'Unknown dialect "invalid"',
-            str(context.exception.__cause__))
+            run_cli('printer.dialect = "invalid"; records', output_format="csv")
+        self.assertEqual('Unknown dialect "invalid"', str(context.exception.__cause__))
 
-    def testCsvOutputFormatDelimiter(self):
-        self.assertPyolin(
+    def test_csv_output_format_delimiter(self):
+        self.assert_pyolin(
             'printer.delimiter = "^"; records',
-            '''\
+            """\
             Bucks^Milwaukee^60^22^0.732\r
             Raptors^Toronto^58^24^0.707\r
             76ers^Philadelphia^51^31^0.622\r
             Celtics^Boston^49^33^0.598\r
             Pacers^Indiana^48^34^0.585\r
-            ''',
-            output_format='csv')
+            """,
+            output_format="csv",
+        )
 
-    def testCsvOutputNonTuple(self):
-        self.assertPyolin(
-            'record[2]',
-            '''\
+    def test_csv_output_non_tuple(self):
+        self.assert_pyolin(
+            "record[2]",
+            """\
             60\r
             58\r
             51\r
             49\r
             48\r
-            ''',
-            output_format='csv')
+            """,
+            output_format="csv",
+        )
 
-    def testCsvOutputQuoting(self):
-        self.assertPyolin(
-            'records',
+    def test_csv_output_quoting(self):
+        self.assert_pyolin(
+            "records",
             '''\
             John,Doe,120 jefferson st.,Riverside, NJ, 08075\r
             Jack,McGinnis,220 hobo Av.,Phila, PA,09119\r
             "John ""Da Man""",Repici,120 Jefferson St.,Riverside, NJ,08075\r
             Stephen,Tyler,"7452 Terrace ""At the Plaza"" road",SomeTown,SD, 91234\r
             ,Blankman,,SomeTown, SD, 00298\r
             "Joan ""the bone"", Anne",Jet,"9th, at Terrace plc",Desert City,CO,00123\r
             ''',
-            input_format='csv',
-            output_format='csv',
-            input='data_addresses.csv')
+            input_format="csv",
+            output_format="csv",
+            input_file="data_addresses.csv",
+        )
 
-    def testCsvOutputWithHeader(self):
-        self.assertPyolin(
+    def test_csv_output_with_header(self):
+        self.assert_pyolin(
             'printer.print_header = True; df[["Last name", "SSN", "Final"]]',
-            '''\
+            """\
             Last name,SSN,Final\r
             Alfalfa,123-45-6789,49\r
             Alfred,123-12-1234,48\r
             Gerty,567-89-0123,44\r
             Android,087-65-4321,47\r
             Franklin,234-56-2890,90\r
             George,345-67-3901,4\r
             Heffalump,632-79-9439,40\r
-            ''',
-            input='data_grades_with_header.csv',
-            input_format='csv',
-            output_format='csv')
+            """,
+            input_file="data_grades_with_header.csv",
+            input_format="csv",
+            output_format="csv",
+        )
 
-    def testCsvOutputWithHeaderFunction(self):
+    def test_csv_output_with_header_function(self):
         def func():
             # pylint: disable=undefined-variable
             printer.print_header = True  # type: ignore
             return df[["Last name", "SSN", "Final"]]  # type: ignore
             # pylint: enable=undefined-variable
 
-        self.assertPyolin(
+        self.assert_pyolin(
             func,
-            '''\
+            """\
             Last name,SSN,Final\r
             Alfalfa,123-45-6789,49\r
             Alfred,123-12-1234,48\r
             Gerty,567-89-0123,44\r
             Android,087-65-4321,47\r
             Franklin,234-56-2890,90\r
             George,345-67-3901,4\r
             Heffalump,632-79-9439,40\r
-            ''',
-            input='data_grades_with_header.csv',
-            input_format='csv',
-            output_format='csv')
-
-    def testStreamingStdinCsv(self):
-        with pyolinPopen('parser.has_header = False; record', ['--output_format', 'csv']) as proc:
-            proc.stdin.write('Raptors Toronto    58 24 0.707\n')
+            """,
+            input_file="data_grades_with_header.csv",
+            input_format="csv",
+            output_format="csv",
+        )
+
+    def test_streaming_stdin_csv(self):
+        with pyolin_popen(
+            "parser.has_header = False; record",
+            ["--output_format", "csv", "--input_format", "awk"],
+        ) as proc:
+            assert proc.stdin and proc.stdout
+            proc.stdin.write("Raptors Toronto    58 24 0.707\n")
             proc.stdin.flush()
             with timeout(2):
                 self.assertEqual(
-                    proc.stdout.readline(),
-                    'Raptors,Toronto,58,24,0.707\n')
-            proc.stdin.write('Celtics Boston     49 33 0.598\n')
+                    proc.stdout.readline(), "Raptors,Toronto,58,24,0.707\n"
+                )
+            proc.stdin.write("Celtics Boston     49 33 0.598\n")
             proc.stdin.flush()
             with timeout(2):
-                self.assertEqual(
-                    proc.stdout.readline(),
-                    'Celtics,Boston,49,33,0.598\n')
+                self.assertEqual(proc.stdout.readline(), "Celtics,Boston,49,33,0.598\n")
 
-    def testNumericHeader(self):
-        self.assertPyolin(
-            'printer.print_header = True; record[0],record[2],record[7]',
-            '''\
+    def test_numeric_header(self):
+        self.assert_pyolin(
+            "printer.print_header = True; record[0],record[2],record[7]",
+            """\
             0,1,2\r
             Alfalfa,123-45-6789,49.0\r
             Alfred,123-12-1234,48.0\r
             Gerty,567-89-0123,44.0\r
             Android,087-65-4321,47.0\r
             Franklin,234-56-2890,90.0\r
             George,345-67-3901,4.0\r
             Heffalump,632-79-9439,40.0\r
-            ''',
-            input='data_grades_simple_csv.csv',
-            input_format='csv',
-            output_format='csv')
+            """,
+            input_file="data_grades_simple_csv.csv",
+            input_format="csv",
+            output_format="csv",
+        )
 
-    def testMarkdownOutput(self):
-        self.assertPyolin(
+    def test_markdown_output(self):
+        self.assert_pyolin(
             'df[["Last name", "SSN", "Final"]]',
-            '''\
+            """\
             | Last name | SSN         | Final |
             | --------- | ----------- | ----- |
             | Alfalfa   | 123-45-6789 | 49    |
             | Alfred    | 123-12-1234 | 48    |
             | Gerty     | 567-89-0123 | 44    |
             | Android   | 087-65-4321 | 47    |
             | Franklin  | 234-56-2890 | 90    |
             | George    | 345-67-3901 | 4     |
             | Heffalump | 632-79-9439 | 40    |
-            ''',
-            input='data_grades_with_header.csv',
-            input_format='csv',
-            output_format='markdown')
-
-    def testTsvOutput(self):
-        self.assertPyolin(
-            'records',
-            '''\
+            """,
+            input_file="data_grades_with_header.csv",
+            input_format="csv",
+            output_format="markdown",
+        )
+
+    def test_tsv_output(self):
+        self.assert_pyolin(
+            "records",
+            """\
             Bucks	Milwaukee	60	22	0.732\r
             Raptors	Toronto	58	24	0.707\r
             76ers	Philadelphia	51	31	0.622\r
             Celtics	Boston	49	33	0.598\r
             Pacers	Indiana	48	34	0.585\r
-            ''',
-            output_format='tsv')
+            """,
+            output_format="tsv",
+        )
 
-    def testMultilineInput(self):
-        self.assertPyolin(
-            textwrap.dedent('''\
+    def test_multiline_input(self):
+        self.assert_pyolin(
+            textwrap.dedent(
+                """\
             record = 1
             record + 1\
-            '''),
-            '''\
+            """
+            ),
+            """\
             2
-            ''')
+            """,
+        )
 
-    def testMultilineMixedInput(self):
-        self.assertPyolin(
-            textwrap.dedent('''\
-            record = 1; record += 1
-            record += 1; record + 1
-            '''),
-            '''\
+    def test_multiline_mixed_input(self):
+        self.assert_pyolin(
+            textwrap.dedent(
+                """\
+                record = 1; record += 1
+                record += 1; record + 1
+                """
+            ),
+            """\
             4
-            ''')
+            """,
+        )
 
-    def testLastStatement(self):
+    def test_last_statement(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('1+1;pass')
+            run_cli("1+1;pass")
         self.assertEqual(
-            textwrap.dedent('''\
-            Cannot evaluate value from statement:
-              pass'''),
-            str(context.exception.__cause__))
-
-    def testMultilinePythonProgram(self):
-        self.assertPyolin(
-            textwrap.dedent('''\
-            result = []
-            for i in range(5):
-                result.append(range(i + 1))
-            result
-            '''),
-            '''\
+            textwrap.dedent(
+                """\
+                Cannot evaluate value from statement:
+                  pass"""
+            ),
+            str(context.exception.__cause__),
+        )
+
+    def test_multiline_python_program(self):
+        self.assert_pyolin(
+            textwrap.dedent(
+                """\
+                result = []
+                for i in range(5):
+                    result.append(range(i + 1))
+                result
+                """
+            ),
+            """\
             0
             0 1
             0 1 2
             0 1 2 3
             0 1 2 3 4
-            ''',
-            output_format='awk')
+            """,
+            output_format="awk",
+        )
 
-    def testMarkdownWrapping(self):
-        with mock.patch.dict(os.environ, {'PYOLIN_TABLE_WIDTH': '80'}):
-            self.assertPyolin(
+    def test_markdown_wrapping(self):
+        with mock.patch.dict(os.environ, {"PYOLIN_TABLE_WIDTH": "80"}):
+            self.assert_pyolin(
                 'df[["marketplace", "review_body", "star_rating"]]',
-                '''\
+                """\
                 | marketplace | review_body                                      | star_rating |
                 | ----------- | ------------------------------------------------ | ----------- |
                 | US          | Absolutely love this watch! Get compliments      | 5           |
                 :             : almost every time I wear it. Dainty.             :             :
                 | US          | I love this watch it keeps time wonderfully.     | 5           |
                 | US          | Scratches                                        | 2           |
                 | US          | It works well on me. However, I found cheaper    | 5           |
@@ -1490,263 +1663,391 @@
                 :             :  folded because it is well polished and brushed  :             :
                 :             : and the folds are pretty tight for the most      :             :
                 :             : part.<br /><br />I love the new member of my     :             :
                 :             : collection and it looks great.  I've had it for  :             :
                 :             : about a week and so far it has kept good time    :             :
                 :             : despite day 1 which is typical of a new          :             :
                 :             : mechanical watch                                 :             :
-                ''',
-                input='data_amazon_reviews.tsv',
-                input_format='tsv',
-                output_format='markdown')
-
-    def testMarkdownWrapping2(self):
-        with mock.patch.dict(os.environ, {'PYOLIN_TABLE_WIDTH': '80'}):
-            self.assertPyolin(
-                'records',
-                '''\
+                """,
+                input_file="data_amazon_reviews.tsv",
+                input_format="tsv",
+                output_format="markdown",
+            )
+
+    def test_markdown_wrapping2(self):
+        with mock.patch.dict(os.environ, {"PYOLIN_TABLE_WIDTH": "80"}):
+            self.assert_pyolin(
+                "records",
+                """\
                 | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11    | 12           | 13  | 14 |
                 | - | - | - | - | - | - | - | - | - | - | -- | ----- | ------------ | --- | -- |
                 | a | b | c | d | e | f | g | h | i | j | k  | lmnop | qrstuv123456 | wxy | z  |
                 :   :   :   :   :   :   :   :   :   :   :    :       : 789123456789 :     :    :
                 :   :   :   :   :   :   :   :   :   :   :    :       : 123456789    :     :    :
-                ''',
-                input='data_formatting.txt',
-                output_format='markdown')
-
-    def testJsonOutput(self):
-        self.assertPyolin(
-            'records',
-            '''\
+                """,
+                input_file="data_formatting.txt",
+                output_format="markdown",
+            )
+
+    def test_json_output(self):
+        self.assert_pyolin(
+            "records[0]",
+            """\
             [
-            {"0": "Bucks", "1": "Milwaukee", "2": 60, "3": 22, "4": 0.732},
-            {"0": "Raptors", "1": "Toronto", "2": 58, "3": 24, "4": 0.707},
-            {"0": "76ers", "1": "Philadelphia", "2": 51, "3": 31, "4": 0.622},
-            {"0": "Celtics", "1": "Boston", "2": 49, "3": 33, "4": 0.598},
-            {"0": "Pacers", "1": "Indiana", "2": 48, "3": 34, "4": 0.585}
+                "Bucks",
+                "Milwaukee",
+                60,
+                22,
+                0.732
             ]
-            ''',
-            output_format='json')
+            """,
+            output_format="json",
+        )
 
-    def testJsonInput(self):
-        self.assertPyolin(
-            'df',
-            '''\
+    def test_json_output_with_manual_header(self):
+        self.assert_pyolin(
+            "header = ['team', 'city', 'wins', 'loss', 'Win rate']; records[0]",
+            """\
+            {
+                "team": "Bucks",
+                "city": "Milwaukee",
+                "wins": 60,
+                "loss": 22,
+                "Win rate": 0.732
+            }
+            """,
+            output_format="json",
+        )
+
+    def test_json_output_with_header(self):
+        self.assert_pyolin(
+            "records",
+            """\
+            [
+                {"Path": "dir", "IsDir": "True", "Size": 30, "Score": 40.0},
+                {"Path": "dir/file.txt", "IsDir": "False", "Size": 40, "Score": 32.0},
+                {"Path": "dir/file1.txt", "IsDir": "False", "Size": 23, "Score": 56.0},
+                {"Path": "dir/file2.mp4", "IsDir": "False", "Size": 15, "Score": 85.0},
+                {"Path": "dir/filea.png", "IsDir": "False", "Size": 31, "Score": 31.0},
+                {"Path": "dir/fileb.txt", "IsDir": "False", "Size": 44, "Score": 16.0},
+                {"Path": "dir/subdir", "IsDir": "True", "Size": 12, "Score": 42.0},
+                {"Path": "dir/subdir/subfile.txt", "IsDir": "False", "Size": 11, "Score": 53.0}
+            ]
+            """,
+            input_file="data_files_with_header.txt",
+            output_format="json",
+        )
+
+    def test_json_input(self):
+        self.assert_pyolin(
+            "df",
+            """\
             | color   | value |
             | ------- | ----- |
             | red     | #f00  |
             | green   | #0f0  |
             | blue    | #00f  |
             | cyan    | #0ff  |
             | magenta | #f0f  |
             | yellow  | #ff0  |
             | black   | #000  |
-            ''',
-            input='data_colors.json',
-            input_format='json',
-            output_format='markdown')
+            """,
+            input_file="data_colors.json",
+            input_format="json",
+            output_format="markdown",
+        )
 
-    def testContains(self):
-        self.assertPyolin(
+    def test_contains(self):
+        self.assert_pyolin(
             '("green", "#0f0") in records',
-            '''\
+            """\
             True
-            ''',
-            input='data_colors.json',
-            input_format='json')
+            """,
+            input_file="data_colors.json",
+            input_format="json",
+        )
 
-    def testSingleValueOutput(self):
-        self.assertPyolin(
-            'len(records)',
-            '''\
-            | value |
-            | ----- |
-            | 7     |
-            ''',
-            input='data_colors.json',
-            input_format='json',
-            output_format='markdown')
-
-    def testRecordOutput(self):
-        self.assertPyolin(
-            'records[0]',
-            '''\
-            | color | value |
-            | ----- | ----- |
-            | red   | #f00  |
-            ''',
-            input='data_colors.json',
-            input_format='json',
-            output_format='markdown')
-
-    def testRecordsWithHeader(self):
-        self.assertPyolin(
-            'records',
-            '''\
-            | color   | value |
-            | ------- | ----- |
-            | red     | #f00  |
-            | green   | #0f0  |
-            | blue    | #00f  |
-            | cyan    | #0ff  |
-            | magenta | #f0f  |
-            | yellow  | #ff0  |
-            | black   | #000  |
-            ''',
-            input='data_colors.json',
-            input_format='json',
-            output_format='markdown')
-
-    def testLinesWithHeader(self):
-        self.assertPyolin(
-            'lines',
-            '''\
-            | value                                 |
-            | ------------------------------------- |
-            | {"color": "red", "value": "#f00"}     |
-            | {"color": "green", "value": "#0f0"}   |
-            | {"color": "blue", "value": "#00f"}    |
-            | {"color": "cyan", "value": "#0ff"}    |
-            | {"color": "magenta", "value": "#f0f"} |
-            | {"color": "yellow", "value": "#ff0"}  |
-            | {"color": "black", "value": "#000"}   |
-            ''',
-            input='data_colors.json',
-            input_format='json',
-            output_format='markdown')
-
-    def testMarkdownNonUniformColumnCount(self):
-        self.assertPyolin(
-            'range(i) for i in range(1, 5)',
-            '''\
+    def test_markdown_output_format(self):
+        for prog, expected in [
+            (
+                "len(records)",
+                """\
+                | value |
+                | ----- |
+                | 7     |
+                """,
+            ),
+            (
+                "records[0]",
+                """\
+                | color | value |
+                | ----- | ----- |
+                | red   | #f00  |
+                """,
+            ),
+            (
+                "records",
+                """\
+                | color   | value |
+                | ------- | ----- |
+                | red     | #f00  |
+                | green   | #0f0  |
+                | blue    | #00f  |
+                | cyan    | #0ff  |
+                | magenta | #f0f  |
+                | yellow  | #ff0  |
+                | black   | #000  |
+                """,
+            ),
+            (
+                "lines",
+                """\
+                | value                                 |
+                | ------------------------------------- |
+                | {"color": "red", "value": "#f00"}     |
+                | {"color": "green", "value": "#0f0"}   |
+                | {"color": "blue", "value": "#00f"}    |
+                | {"color": "cyan", "value": "#0ff"}    |
+                | {"color": "magenta", "value": "#f0f"} |
+                | {"color": "yellow", "value": "#ff0"}  |
+                | {"color": "black", "value": "#000"}   |
+                """,
+            ),
+        ]:
+            with self.subTest(prog):
+                self.assert_pyolin(
+                    prog,
+                    expected,
+                    input_file="data_colors.json",
+                    input_format="json",
+                    output_format="markdown",
+                )
+
+    def test_markdown_non_uniform_column_count(self):
+        self.assert_pyolin(
+            "range(i) for i in range(1, 5)",
+            """\
             | value |
             | ----- |
             | 0     |
             | 0     | 1 |
             | 0     | 1 | 2 |
             | 0     | 1 | 2 | 3 |
-            ''',
-            output_format='markdown')
+            """,
+            output_format="markdown",
+        )
 
-    def testReprPrinter(self):
-        self.assertPyolin(
-            'range(10)',
-            '''\
+    def test_repr_printer(self):
+        self.assert_pyolin(
+            "range(10)",
+            """\
             range(0, 10)
-            ''',
-            output_format='repr')
+            """,
+            output_format="repr",
+        )
 
-    def testReprPrinterTable(self):
-        self.assertPyolin(
-            'records',
-            '''\
+    def test_repr_printer_table(self):
+        self.assert_pyolin(
+            "records",
+            """\
             [('Bucks', 'Milwaukee', '60', '22', '0.732'), ('Raptors', 'Toronto', '58', '24', '0.707'), ('76ers', 'Philadelphia', '51', '31', '0.622'), ('Celtics', 'Boston', '49', '33', '0.598'), ('Pacers', 'Indiana', '48', '34', '0.585')]
-            ''',
-            output_format='repr')
+            """,
+            output_format="repr",
+        )
 
-    def testReprPrinterRecords(self):
-        self.assertPyolin(
+    def test_repr_printer_records(self):
+        self.assert_pyolin(
             '"aloha\u2011\u2011\u2011"',
-            '''\
+            """\
             'aloha\u2011\u2011\u2011'
-            ''',
-            output_format='repr')
+            """,
+            output_format="repr",
+        )
 
-    def testStrPrinterRecords(self):
-        self.assertPyolin(
+    def test_str_printer_records(self):
+        self.assert_pyolin(
             '"aloha\u2011\u2011\u2011"',
-            '''\
+            """\
             aloha\u2011\u2011\u2011
-            ''',
-            output_format='str')
+            """,
+            output_format="str",
+        )
 
-    def testStrPrinterTable(self):
-        self.assertPyolin(
-            'records',
-            '''\
-            [('Bucks', 'Milwaukee', '60', '22', '0.732'), ('Raptors', 'Toronto', '58', '24', '0.707'), ('76ers', 'Philadelphia', '51', '31', '0.622'), ('Celtics', 'Boston', '49', '33', '0.598'), ('Pacers', 'Indiana', '48', '34', '0.585')]
-            ''',
-            output_format='str')
+    def test_str_printer_table(self):
+        self.assert_pyolin(
+            "records",
+            (
+                "[('Bucks', 'Milwaukee', '60', '22', '0.732'), "
+                "('Raptors', 'Toronto', '58', '24', '0.707'), "
+                "('76ers', 'Philadelphia', '51', '31', '0.622'), "
+                "('Celtics', 'Boston', '49', '33', '0.598'), "
+                "('Pacers', 'Indiana', '48', '34', '0.585')]\n"
+            ),
+            output_format="str",
+        )
 
-    def testSetPrinter(self):
-        self.assertPyolin(
+    def test_set_printer(self):
+        self.assert_pyolin(
             'printer = new_printer("repr"); range(10)',
-            '''\
+            """\
             range(0, 10)
-            ''')
+            """,
+        )
 
-    def testPrinterNone(self):
+    def test_printer_none(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('printer = None; 123')
+            run_cli("printer = None; 123")
         self.assertEqual(
             'printer must be an instance of Printer. Found "None" instead',
-            str(context.exception.__cause__))
+            str(context.exception.__cause__),
+        )
 
-    def testRaiseStopIteration(self):
+    def test_raise_stop_iteration(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('raise StopIteration(); None')
+            run_cli("raise StopIteration(); None")
         assert isinstance(context.exception.__cause__, UserError)
         formatted = context.exception.__cause__.formatted_tb()
         self.assertEqual(3, len(formatted), pformat(formatted))
-        self.assertIn('Traceback (most recent call last)', formatted[0])
-        self.assertIn('pyolin_user_prog.py', formatted[1])
-        self.assertIn('StopIteration', formatted[2])
-
-    def testBinaryInputLen(self):
-        self.assertPyolin(
-            'len(file)',
-            '''\
+        self.assertIn("Traceback (most recent call last)", formatted[0])
+        self.assertIn("pyolin_user_prog.py", formatted[1])
+        self.assertIn("StopIteration", formatted[2])
+
+    def test_binary_input_len(self):
+        self.assert_pyolin(
+            "len(file)",
+            """\
             21
-            ''',
-            input_format='binary',
-            input='data_pickle')
+            """,
+            input_file="data_pickle",
+        )
 
-    def testBinaryInputPickle(self):
-        self.assertPyolin(
-            'pickle.loads(file)',
-            '''\
+    def test_binary_input_can_be_accessed(self):
+        self.assert_pyolin(
+            "type(file).__name__",
+            """\
+            bytes
+            """,
+            input_file="data_pickle",
+        )
+
+    def test_binary_input_pickle(self):
+        self.assert_pyolin(
+            "pickle.loads(file)",
+            """\
             hello world
-            ''',
-            input_format='binary',
-            input='data_pickle')
+            """,
+            input_file="data_pickle",
+        )
 
-    def testBinaryPrinter(self):
-        self.assertPyolin(
+    def test_binary_printer(self):
+        self.assert_pyolin(
             'b"\\x30\\x62\\x43\\x00"',
-            b'\x30\x62\x43\x00',
-            input_format='binary',
-            output_format='binary')
+            b"\x30\x62\x43\x00",
+            output_format="binary",
+        )
 
-    def testBinaryInputAccessRecords(self):
+    def test_auto_parser(self):
+        for input_file, expected_output in [
+            ("data_nba.txt", ("Bucks", "Milwaukee", "60", "22", "0.732")),
+            ("data_files.txt", ("dir", "True", "30", "40.0")),
+            ("data_colors.json", ("red", "#f00")),
+            (
+                "data_addresses_with_header.csv",
+                ("John", "Doe", "120 jefferson st.", "Riverside", " NJ", " 08075"),
+            ),
+            (
+                "data_addresses_unix.csv",
+                ("John", "Doe", "120 jefferson st.", "Riverside", " NJ", " 08075"),
+            ),
+            (
+                "data_grades_with_header.csv",
+                (
+                    "Alfalfa",
+                    "Aloysius",
+                    "123-45-6789",
+                    "40.0",
+                    "90.0",
+                    "100.0",
+                    "83.0",
+                    "49.0",
+                    "D-",
+                ),
+            ),
+            (
+                "data_amazon_reviews.tsv",
+                (
+                    "US",
+                    "3653882",
+                    "R3O9SGZBVQBV76",
+                    "B00FALQ1ZC",
+                    "937001370",
+                    (
+                        'Invicta Women\'s 15150 "Angel" 18k Yellow Gold Ion-Plated Stainless Steel '
+                        "and Brown Leather Watch"
+                    ),
+                    "Watches",
+                    "5",
+                    "0",
+                    "0",
+                    "N",
+                    "Y",
+                    "Five Stars",
+                    (
+                        "Absolutely love this watch! Get compliments almost every time I wear it. "
+                        "Dainty."
+                    ),
+                    "2015-08-31",
+                ),
+            ),
+        ]:
+            with self.subTest(input_file):
+                self.assert_pyolin(
+                    "records[0]",
+                    repr(expected_output) + "\n",
+                    input_file=input_file,
+                    output_format="repr",
+                )
+
+    def test_binary_input_access_records(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('records', input_format='binary', input='data_pickle')
+            run_cli("records", input_file="data_pickle")
+
+        def format_exception_only(exc):
+            if sys.version_info >= (3, 10):
+                return traceback.format_exception_only(exc)  # type: ignore
+            else:
+                return traceback.format_exception_only(type(exc), exc)  # type: ignore
+
         self.assertEqual(
-            'Record based attributes are not supported in binary input mode',
-            str(context.exception.__cause__))
+            "`record`-based attributes are not supported for binary inputs",
+            str(context.exception.__cause__),
+            msg="".join(format_exception_only(context.exception.__cause__)),
+        )
 
-    def testSetFieldSeparator(self):
-        self.assertPyolin(
+    def test_set_field_separator(self):
+        self.assert_pyolin(
             'parser.field_separator = ","; record',
-            '''\
+            """\
             | 0         | 1          | 2           | 3    | 4    | 5     | 6    | 7    | 8  |
             | --------- | ---------- | ----------- | ---- | ---- | ----- | ---- | ---- | -- |
             | Alfalfa   | Aloysius   | 123-45-6789 | 40.0 | 90.0 | 100.0 | 83.0 | 49.0 | D- |
             | Alfred    | University | 123-12-1234 | 41.0 | 97.0 | 96.0  | 97.0 | 48.0 | D+ |
             | Gerty     | Gramma     | 567-89-0123 | 41.0 | 80.0 | 60.0  | 40.0 | 44.0 | C  |
             | Android   | Electric   | 087-65-4321 | 42.0 | 23.0 | 36.0  | 45.0 | 47.0 | B- |
             | Franklin  | Benny      | 234-56-2890 | 50.0 | 1.0  | 90.0  | 80.0 | 90.0 | B- |
             | George    | Boy        | 345-67-3901 | 40.0 | 1.0  | 11.0  | -1.0 | 4.0  | B  |
             | Heffalump | Harvey     | 632-79-9439 | 30.0 | 1.0  | 20.0  | 30.0 | 40.0 | C  |
-            ''',
-            input='data_grades_simple_csv.csv')
+            """,
+            input_file="data_grades_simple_csv.csv",
+        )
 
-    def testSetRecordSeparator(self):
-        self.assertPyolin(
+    def test_set_record_separator(self):
+        self.assert_pyolin(
             'parser.record_separator = ","; record',
-            '''\
+            """\
             | value     |
             | --------- |
             | JET       |
             | 20031201  |
             | 20001006  |
             | 53521     |
             | 1.000E+01 |
@@ -1755,178 +2056,419 @@
             | TRANS     |
             | 2.000E+00 |
             | 1.000E+00 |
             | 2         |
             | 1         |
             | 0         |
             | 0         |
-            ''',
-            input='data_onerow.csv')
+            """,
+            input_file="data_onerow.csv",
+        )
 
-    def testSetParser(self):
-        self.assertPyolin(
+    def test_set_parser(self):
+        self.assert_pyolin(
             'parser = new_parser("json"); df',
-            '''\
+            """\
             | color   | value |
             | ------- | ----- |
             | red     | #f00  |
             | green   | #0f0  |
             | blue    | #00f  |
             | cyan    | #0ff  |
             | magenta | #f0f  |
             | yellow  | #ff0  |
             | black   | #000  |
-            ''',
-            input='data_colors.json')
+            """,
+            input_file="data_colors.json",
+        )
 
-    def testSetParserRecord(self):
+    def test_set_parser_record(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('a = records[0]; parser = 123; 123')
+            run_cli("a = records[0]; parser = 123; 123")
         self.assertEqual(
-            'Cannot set parser after it has been used',
-            str(context.exception.__cause__.__cause__))
+            "Cannot set parser after it has been used",
+            str(context.exception.__cause__.__cause__),
+        )
 
-    def testRecordsIfUndefined(self):
-        self.assertPyolin(
-            'records if False',
-            '''\
-            ''')
+    def test_records_if_undefined(self):
+        self.assert_pyolin(
+            "records if False",
+            """\
+            """,
+        )
 
-    def testGenRecordsIfUndefined(self):
-        self.assertRunPyolin(
-            'records if False',
-            _UNDEFINED_)
-
-    def testUndefinedRepr(self):
-        self.assertPyolin(
-            '_UNDEFINED_',
-            '''\
-            Undefined()
-            ''',
-            output_format='repr')
+    def test_gen_records_if_undefined(self):
+        self.assert_run_pyolin("records if False", _UNDEFINED_)
 
-    def testUndefinedStr(self):
-        self.assertPyolin(
-            '_UNDEFINED_',
-            '''\
-            ''',
-            output_format='str')
+    def test_undefined(self):
+        for output_format, expected in {
+            "repr": "Undefined()\n",
+            "str": "",
+            "json": "",
+            "awk": "",
+            "auto": "",
+            "binary": "",
+            "csv": "",
+        }.items():
+            with self.subTest(output_format):
+                self.assert_pyolin(
+                    "_UNDEFINED_",
+                    expected,
+                    output_format=output_format,
+                )
 
-    def testNameError(self):
+    def test_name_error(self):
         with self.assertRaises(ErrorWithStderr) as context:
-            run_cli('idontknowwhatisthis + 1')
+            run_cli("idontknowwhatisthis + 1")
         self.assertEqual(
             "name 'idontknowwhatisthis' is not defined",
-            str(context.exception.__cause__.__cause__))
+            str(context.exception.__cause__.__cause__),
+        )
 
-    def testBegin(self):
-        self.assertPyolin(
-            'if BEGIN: mysum = 0; header = ("sum", "value")\n'
-            'mysum += record[2]\n'
-            'mysum, record[2]',
-            '''\
+    def test_record_first(self):
+        self.assert_pyolin(
+            'if record.first: mysum = 0; header = ("sum", "value")\n'
+            "mysum += record[2]\n"
+            "mysum, record[2]",
+            """\
             | sum | value |
             | --- | ----- |
             | 60  | 60    |
             | 118 | 58    |
             | 169 | 51    |
             | 218 | 49    |
             | 266 | 48    |
-            ''')
+            """,
+        )
 
-    def testTrailingNewline(self):
-        self.assertPyolin(
-            'records\n',
-            '''\
+    def test_record_num(self):
+        self.assert_pyolin(
+            'record.num',
+            """\
+            | value |
+            | ----- |
+            | 0     |
+            | 1     |
+            | 2     |
+            | 3     |
+            | 4     |
+            """,
+        )
+
+    def test_trailing_newline(self):
+        self.assert_pyolin(
+            "records\n",
+            """\
             | 0       | 1            | 2  | 3  | 4     |
             | ------- | ------------ | -- | -- | ----- |
             | Bucks   | Milwaukee    | 60 | 22 | 0.732 |
             | Raptors | Toronto      | 58 | 24 | 0.707 |
             | 76ers   | Philadelphia | 51 | 31 | 0.622 |
             | Celtics | Boston       | 49 | 33 | 0.598 |
             | Pacers  | Indiana      | 48 | 34 | 0.585 |
-            ''')
+            """,
+        )
 
-    def testExecuteFunction(self):
+    def test_execute_function(self):
         def get_records():
             # pylint: disable=undefined-variable
             return records  # type: ignore
             # pylint: enable=undefined-variable
-        self.assertRunPyolin(
+
+        self.assert_run_pyolin(
             get_records,
             [
-                ('Bucks', 'Milwaukee', 60, 22, 0.732),
-                ('Raptors', 'Toronto', 58, 24, 0.707),
-                ('76ers', 'Philadelphia', 51, 31, 0.622),
-                ('Celtics', 'Boston', 49, 33, 0.598),
-                ('Pacers', 'Indiana', 48, 34, 0.585),
-            ])
+                ("Bucks", "Milwaukee", 60, 22, 0.732),
+                ("Raptors", "Toronto", 58, 24, 0.707),
+                ("76ers", "Philadelphia", 51, 31, 0.622),
+                ("Celtics", "Boston", 49, 33, 0.598),
+                ("Pacers", "Indiana", 48, 34, 0.585),
+            ],
+        )
 
-    def testExecuteFunctionRecordScoped(self):
+    def test_execute_function_record_scoped(self):
         def get_records():
             # pylint: disable=undefined-variable
             return record[0]  # type: ignore
             # pylint: enable=undefined-variable
-        self.assertRunPyolin(
-            get_records,
-            ['Bucks', 'Raptors', '76ers', 'Celtics', 'Pacers'])
 
-    def testDoubleSemiColon(self):
-        self.assertPyolin(
-            'record = 1; record += 1;; record += 1; record + 1',
-            '''\
+        self.assert_run_pyolin(
+            get_records, ["Bucks", "Raptors", "76ers", "Celtics", "Pacers"]
+        )
+
+    def test_double_semi_colon(self):
+        self.assert_pyolin(
+            "record = 1; record += 1;; record += 1; record + 1",
+            """\
             4
-            ''')
+            """,
+        )
 
-    def testIfBeginDoubleSemiColon(self):
-        '''
+    def test_if_record_first_double_semi_colon(self):
+        """
         Double semi-colon is treated as a newline
-        '''
-        self.assertPyolin(
-            'if BEGIN: sum = 0;; sum += record[2]; sum, record[2]',
-            '''\
+        """
+        self.assert_pyolin(
+            "if record.first: sum = 0;; sum += record[2]; sum, record[2]",
+            """\
             | 0   | 1  |
             | --- | -- |
             | 60  | 60 |
             | 118 | 58 |
             | 169 | 51 |
             | 218 | 49 |
             | 266 | 48 |
-            ''')
+            """,
+        )
 
-    def testUndefinedIsFalse(self):
-        self.assertRunPyolin('bool(_UNDEFINED_)', False)
+    def test_undefined_is_false(self):
+        self.assert_run_pyolin("bool(_UNDEFINED_)", False)
 
-    def testEndWithDoubleSemiColon(self):
-        self.assertPyolin(
-            'record[2];;',
-            '''\
+    def test_end_with_double_semi_colon(self):
+        self.assert_pyolin(
+            "record[2];;",
+            """\
             | value |
             | ----- |
             | 60    |
             | 58    |
             | 51    |
             | 49    |
             | 48    |
-            ''')
+            """,
+        )
 
-    def testSysArgv(self):
-        '''
+    def test_sys_argv(self):
+        """
         sys.argv should be shifted, so sys.argv[1] should be the first one after the pyolin prog
-        '''
-        self.assertPyolin(
-            'sys.argv',
-            '''\
+        """
+        self.assert_pyolin(
+            "sys.argv",
+            """\
             | value   |
             | ------- |
             | pyolin  |
             | testing |
             | 1       |
             | 2       |
             | 3       |
-            ''',
-            extra_args=['testing', '1', '2', '3']
+            """,
+            extra_args=["testing", "1", "2", "3"],
+        )
+
+    def test_manual_load_json_record(self):
+        for output_format, expected in {
+            "awk": """\
+                   color red
+                   value #f00
+                   """,
+            "json": """\
+                    {
+                        "color": "red",
+                        "value": "#f00"
+                    }
+                    """,
+        }.items():
+            with self.subTest(output_format):
+                self.assert_pyolin(
+                    "json.loads(file)[0]",
+                    expected,
+                    input_file="data_colors.json",
+                    output_format=output_format,
+                )
+
+    def test_manual_load_json_output(self):
+        for output_format, expected in {
+            "awk": """\
+                    ('color', 'red') ('value', '#f00')
+                    ('color', 'green') ('value', '#0f0')
+                    ('color', 'blue') ('value', '#00f')
+                    ('color', 'cyan') ('value', '#0ff')
+                    ('color', 'magenta') ('value', '#f0f')
+                    ('color', 'yellow') ('value', '#ff0')
+                    ('color', 'black') ('value', '#000')
+                    """,
+            "json": """\
+                    [
+                        {
+                            "color": "red",
+                            "value": "#f00"
+                        },
+                        {
+                            "color": "green",
+                            "value": "#0f0"
+                        },
+                        {
+                            "color": "blue",
+                            "value": "#00f"
+                        },
+                        {
+                            "color": "cyan",
+                            "value": "#0ff"
+                        },
+                        {
+                            "color": "magenta",
+                            "value": "#f0f"
+                        },
+                        {
+                            "color": "yellow",
+                            "value": "#ff0"
+                        },
+                        {
+                            "color": "black",
+                            "value": "#000"
+                        }
+                    ]
+                    """,
+        }.items():
+            with self.subTest(output_format):
+                self.assert_pyolin(
+                    "json.loads(file)",
+                    expected,
+                    input_file="data_colors.json",
+                    output_format=output_format,
+                )
+
+    def test_manual_load_csv(self):
+        self.assert_pyolin(
+            "csv.reader(io.StringIO(file))",
+            # pylint:disable=line-too-long
+            """\
+            | 0                     | 1        | 2                                | 3           | 4   | 5      |
+            | --------------------- | -------- | -------------------------------- | ----------- | --- | ------ |
+            | John                  | Doe      | 120 jefferson st.                | Riverside   |  NJ |  08075 |
+            | Jack                  | McGinnis | 220 hobo Av.                     | Phila       |  PA | 09119  |
+            | John "Da Man"         | Repici   | 120 Jefferson St.                | Riverside   |  NJ | 08075  |
+            | Stephen               | Tyler    | 7452 Terrace "At the Plaza" road | SomeTown    | SD  |  91234 |
+            |                       | Blankman |                                  | SomeTown    |  SD |  00298 |
+            | Joan "the bone", Anne | Jet      | 9th, at Terrace plc              | Desert City | CO  | 00123  |
+            """,
+            # pylint:enable=line-too-long
+            input_file="data_addresses.csv",
+        )
+
+    def test_non_table_json(self):
+        with self.assertRaises(ErrorWithStderr) as context:
+            run_cli("records", input_file="data_json_example.json")
+            self.assertEqual(
+                "TypeError: Input is not an array of objects",
+                str(context.exception.__cause__),
+            )
+
+    def test_jsonobj_string_output(self):
+        self.assert_pyolin(
+            "jsonobj['glossary']['title']",
+            "example glossary\n",
+            input_file="data_json_example.json",
+        )
+
+    def test_jsonobj_obj_output(self):
+        self.assert_pyolin(
+            "jsonobj['glossary']['GlossDiv']['GlossList']['GlossEntry']['GlossDef']",
+            """\
+            {
+                "para": "A meta-markup language, used to create markup languages such as DocBook.",
+                "GlossSeeAlso": [
+                    "GML",
+                    "XML"
+                ]
+            }
+            """,
+            input_file="data_json_example.json",
+        )
+
+    def test_3d_table(self):
+        self.assert_pyolin(
+            "[['foo', ['a', 'b']], ['bar', ['c', 'd']]]",
+            """\
+            [
+                [
+                    "foo",
+                    "['a', 'b']"
+                ],
+                [
+                    "bar",
+                    "['c', 'd']"
+                ]
+            ]
+            """,
+            input_file="data_json_example.json",
+        )
+
+    def test_multiline_json_prog(self):
+        self.assert_pyolin(
+            textwrap.dedent("""\
+            [
+                ['foo', ['a', 'b']], ['bar', ['c', 'd']]
+            ]"""),
+            """\
+            [
+                [
+                    "foo",
+                    "['a', 'b']"
+                ],
+                [
+                    "bar",
+                    "['c', 'd']"
+                ]
+            ]
+            """,
+            input_file="data_json_example.json",
+        )
+
+    def test_json_with_undefined(self):
+        self.assert_pyolin(
+            "[_UNDEFINED_, 'foo']",
+            """\
+            [
+                "foo"
+            ]
+            """,
+            input_file="data_json_example.json",
+            output_format="json"
+        )
+
+    def test_records_negative_index(self):
+        self.assert_pyolin(
+            "records[-1]",
+            """\
+            Pacers Indiana 48 34 0.585
+            """,
         )
 
+    def test_records_negative_slice_start(self):
+        self.assert_pyolin(
+            "records[-1:]",
+            """\
+            | 0      | 1       | 2  | 3  | 4     |
+            | ------ | ------- | -- | -- | ----- |
+            | Pacers | Indiana | 48 | 34 | 0.585 |
+            """,
+        )
+
+    def test_records_negative_slice_stop(self):
+        self.assert_pyolin(
+            "records[:-3]",
+            """\
+            | 0       | 1         | 2  | 3  | 4     |
+            | ------- | --------- | -- | -- | ----- |
+            | Bucks   | Milwaukee | 60 | 22 | 0.732 |
+            | Raptors | Toronto   | 58 | 24 | 0.707 |
+            """,
+        )
+
+    def test_records_negative_slice_step(self):
+        self.assert_pyolin(
+            "records[::-1]",
+            """\
+            | 0       | 1            | 2  | 3  | 4     |
+            | ------- | ------------ | -- | -- | ----- |
+            | Pacers  | Indiana      | 48 | 34 | 0.585 |
+            | Celtics | Boston       | 49 | 33 | 0.598 |
+            | 76ers   | Philadelphia | 51 | 31 | 0.622 |
+            | Raptors | Toronto      | 58 | 24 | 0.707 |
+            | Bucks   | Milwaukee    | 60 | 22 | 0.732 |
+            """,
+        )
 
     # TODOs:
     # Bash / Zsh autocomplete integration
```

### Comparing `pyolin-0.0.3/pyolin/test/utils.py` & `pyolin-0.0.4/pyolin/test/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import contextlib
 import io
 import signal
-from unittest import mock
+from typing import Optional
 
 
 class ErrorWithStderr(Exception):
-
     def __init__(self, stderr, *, errmsg=None):
         self.stderr = stderr
         self.errmsg = errmsg
 
     def __str__(self):
-        result = ['', self.errmsg]
+        result = ["", self.errmsg]
         if self.stderr:
-            result += [
-                '',
-                '===== STDERR =====',
-                str(self.stderr),
-                '=================='
-            ]
+            result += ["", "===== STDERR =====", str(self.stderr), "=================="]
         if self.__cause__:
             result += [
-                '',
-                '===== ERROR =====',
+                "",
+                "===== ERROR =====",
                 str(self.__cause__),
-                '================='
+                "=================",
             ]
-        return '\n'.join(result)
+        return "\n".join(result)
 
 
 class timeout:
-    def __init__(self, seconds, error_message='Timeout'):
+    def __init__(self, seconds, error_message="Timeout"):
         self.seconds = seconds
         self.error_message = error_message
 
     def handle_timeout(self, signum, frame):
         raise TimeoutError(self.error_message)
 
     def __enter__(self):
@@ -47,22 +41,22 @@
 
 class TextIO(io.TextIOWrapper):
     def __init__(self, **kwargs):
         self._io = io.BytesIO()
         super().__init__(self._io, write_through=True, **kwargs)
 
     def getvalue(self):
-        return self._io.getvalue().decode('utf-8')
+        return self._io.getvalue().decode("utf-8")
 
     def getbytes(self):
         return self._io.getvalue()
 
 
 @contextlib.contextmanager
-def run_capturing_output(*, errmsg=None):
+def run_capturing_output(*, errmsg: Optional[str] = None):
     out = TextIO()
     err = TextIO()
     with contextlib.redirect_stdout(out):
         with contextlib.redirect_stderr(err):
             try:
                 yield out
             except BaseException as e:
```

### Comparing `pyolin-0.0.3/LICENSE` & `pyolin-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.3/README.md` & `pyolin-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
 Treats the input file as binary. The input file will be read in binary mode. `records`, `lines`, `df`, and other variables derived from these are not available when using this parser.
 
 ## Printers
 
 ### `auto`
 
-Automatically detect the suitable output format for best human-readability depending on the result data type. If the result datatype is a list, this will be printed in a markdown table. Otherwise, this will be printed in the "Awk" format.
+Automatically detect the suitable output format for best human-readability depending on the result data type. If the result datatype is table-like, this will be printed in a markdown table. Otherwise, if result is a complex dict or list, it will be printed in JSON. Otherwise, this will be printed in the "Awk" format.
 
 ### `awk`
 alias: `unix`
 
 A printer that mimics the behavior of Awk. By default it prints each record in a new line, where each field within a record is separated by a space. The separators can be modified by setting the corresponding fields of the printer. e.g. `printer.field_separator = ","` or `printer.record_separator = "\r\n"`
 
 ### `csv`
```

### Comparing `pyolin-0.0.3/pyproject.toml` & `pyolin-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyolin"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Maurice Lam", email="mauriceprograms@gmail.com" },
 ]
 description = "Tool to easily write Python one-liners"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "hashbang >= 0.1.14",
 ]
+optional-dependencies.dev = [
+    "pandas"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/mauricelam/pyolin"
 "Bug Tracker" = "https://github.com/mauricelam/pyolin/issues"
```

### Comparing `pyolin-0.0.3/PKG-INFO` & `pyolin-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: pyolin
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool to easily write Python one-liners
 Project-URL: Homepage, https://github.com/mauricelam/pyolin
 Project-URL: Bug Tracker, https://github.com/mauricelam/pyolin/issues
 Author-email: Maurice Lam <mauriceprograms@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: hashbang>=0.1.14
+Provides-Extra: dev
+Requires-Dist: pandas; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Pyolin
 
 ![CI](https://github.com/mauricelam/pyolin/actions/workflows/python-package.yml/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/pyolin.svg?color=%230073b7)](https://pypi.org/project/pyolin/)
 
@@ -150,15 +152,15 @@
 
 Treats the input file as binary. The input file will be read in binary mode. `records`, `lines`, `df`, and other variables derived from these are not available when using this parser.
 
 ## Printers
 
 ### `auto`
 
-Automatically detect the suitable output format for best human-readability depending on the result data type. If the result datatype is a list, this will be printed in a markdown table. Otherwise, this will be printed in the "Awk" format.
+Automatically detect the suitable output format for best human-readability depending on the result data type. If the result datatype is table-like, this will be printed in a markdown table. Otherwise, if result is a complex dict or list, it will be printed in JSON. Otherwise, this will be printed in the "Awk" format.
 
 ### `awk`
 alias: `unix`
 
 A printer that mimics the behavior of Awk. By default it prints each record in a new line, where each field within a record is separated by a space. The separators can be modified by setting the corresponding fields of the printer. e.g. `printer.field_separator = ","` or `printer.record_separator = "\r\n"`
 
 ### `csv`
```

