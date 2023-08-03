# Comparing `tmp/syntaxlight-0.1.0.tar.gz` & `tmp/syntaxlight-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.1.0.tar", max compression
+gzip compressed data, was "syntaxlight-0.1.1.tar", max compression
```

## Comparing `syntaxlight-0.1.0.tar` & `syntaxlight-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.0/LICENSE
--rw-r--r--   0        0        0      463 2023-08-03 06:35:22.027696 syntaxlight-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.0/README.md
--rw-r--r--   0        0        0      225 2023-07-29 15:28:20.515491 syntaxlight-0.1.0/syntaxlight/__init__.py
--rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.0/syntaxlight/ast.py
--rw-r--r--   0        0        0     2244 2023-07-30 03:01:17.999345 syntaxlight-0.1.0/syntaxlight/css/all.css
--rw-r--r--   0        0        0      535 2023-08-01 01:05:24.164690 syntaxlight-0.1.0/syntaxlight/css/asm.css
--rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.0/syntaxlight/css/bnf.css
--rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.0/syntaxlight/css/c.css
--rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.0/syntaxlight/css/css.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.0/syntaxlight/css/index.css
--rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.0/syntaxlight/css/json.css
--rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.0/syntaxlight/css/lua.css
--rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.0/syntaxlight/css/makefile.css
--rw-r--r--   0        0        0      876 2023-08-01 01:05:24.169127 syntaxlight-0.1.0/syntaxlight/css/shell.css
--rw-r--r--   0        0        0     2907 2023-08-02 06:45:18.634086 syntaxlight-0.1.0/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.0/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.0/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.0/syntaxlight/error.py
--rw-r--r--   0        0        0     1947 2023-07-29 15:01:42.303917 syntaxlight-0.1.0/syntaxlight/example.py
--rw-r--r--   0        0        0     1926 2023-07-30 02:57:51.649503 syntaxlight-0.1.0/syntaxlight/export.py
--rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.0/syntaxlight/gdt.py
--rw-r--r--   0        0        0     2189 2023-08-01 09:07:20.794987 syntaxlight-0.1.0/syntaxlight/language.py
--rw-r--r--   0        0        0      567 2023-08-02 08:37:35.901602 syntaxlight-0.1.0/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0     2645 2023-07-31 03:00:16.388119 syntaxlight-0.1.0/syntaxlight/lexers/asm_lexer.py
--rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.0/syntaxlight/lexers/bnf_lexer.py
--rw-r--r--   0        0        0    12853 2023-07-31 01:57:07.230431 syntaxlight-0.1.0/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.0/syntaxlight/lexers/css_lexer.py
--rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.0/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    24348 2023-08-02 05:55:13.541695 syntaxlight-0.1.0/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.0/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.0/syntaxlight/lexers/makefile_lexer.py
--rw-r--r--   0        0        0     4457 2023-08-02 08:39:10.819146 syntaxlight-0.1.0/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.0/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.0/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      405 2023-08-01 12:25:00.965587 syntaxlight-0.1.0/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0     1099 2023-07-31 01:38:18.589025 syntaxlight-0.1.0/syntaxlight/parsers/asm_parser.py
--rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.0/syntaxlight/parsers/bnf_parser.py
--rw-r--r--   0        0        0   103618 2023-07-30 12:40:07.793171 syntaxlight-0.1.0/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.0/syntaxlight/parsers/css_parser.py
--rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.0/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.0/syntaxlight/parsers/lua_parser.py
--rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.0/syntaxlight/parsers/makefile_parser.py
--rw-r--r--   0        0        0    13420 2023-08-02 07:49:45.535569 syntaxlight-0.1.0/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0     4619 2023-08-02 08:26:36.227646 syntaxlight-0.1.0/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.0/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.0/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.0/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.0/syntaxlight/template.html
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.1/LICENSE
+-rw-r--r--   0        0        0      463 2023-08-03 08:45:58.550937 syntaxlight-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.1/README.md
+-rw-r--r--   0        0        0      225 2023-07-29 15:28:20.515491 syntaxlight-0.1.1/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.1/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2244 2023-07-30 03:01:17.999345 syntaxlight-0.1.1/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      535 2023-08-01 01:05:24.164690 syntaxlight-0.1.1/syntaxlight/css/asm.css
+-rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.1/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.1/syntaxlight/css/c.css
+-rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.1/syntaxlight/css/css.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.1/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.1/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.1/syntaxlight/css/lua.css
+-rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.1/syntaxlight/css/makefile.css
+-rw-r--r--   0        0        0      876 2023-08-01 01:05:24.169127 syntaxlight-0.1.1/syntaxlight/css/shell.css
+-rw-r--r--   0        0        0     2907 2023-08-02 06:45:18.634086 syntaxlight-0.1.1/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.1/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.1/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.1/syntaxlight/error.py
+-rw-r--r--   0        0        0     1947 2023-07-29 15:01:42.303917 syntaxlight-0.1.1/syntaxlight/example.py
+-rw-r--r--   0        0        0     1926 2023-07-30 02:57:51.649503 syntaxlight-0.1.1/syntaxlight/export.py
+-rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.1/syntaxlight/gdt.py
+-rw-r--r--   0        0        0     2189 2023-08-01 09:07:20.794987 syntaxlight-0.1.1/syntaxlight/language.py
+-rw-r--r--   0        0        0      567 2023-08-02 08:37:35.901602 syntaxlight-0.1.1/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     2645 2023-07-31 03:00:16.388119 syntaxlight-0.1.1/syntaxlight/lexers/asm_lexer.py
+-rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.1/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12853 2023-07-31 01:57:07.230431 syntaxlight-0.1.1/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.1/syntaxlight/lexers/css_lexer.py
+-rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.1/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    24348 2023-08-02 05:55:13.541695 syntaxlight-0.1.1/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.1/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.1/syntaxlight/lexers/makefile_lexer.py
+-rw-r--r--   0        0        0     4457 2023-08-02 08:39:10.819146 syntaxlight-0.1.1/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.1/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.1/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      405 2023-08-01 12:25:00.965587 syntaxlight-0.1.1/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     1099 2023-07-31 01:38:18.589025 syntaxlight-0.1.1/syntaxlight/parsers/asm_parser.py
+-rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.1/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0   104736 2023-08-03 08:45:00.482967 syntaxlight-0.1.1/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.1/syntaxlight/parsers/css_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.1/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.1/syntaxlight/parsers/lua_parser.py
+-rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.1/syntaxlight/parsers/makefile_parser.py
+-rw-r--r--   0        0        0    13420 2023-08-02 07:49:45.535569 syntaxlight-0.1.1/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0     4619 2023-08-02 08:26:36.227646 syntaxlight-0.1.1/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.1/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.1/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.1/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.1/syntaxlight/template.html
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.1/PKG-INFO
```

### Comparing `syntaxlight-0.1.0/LICENSE` & `syntaxlight-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/README.md` & `syntaxlight-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/ast.py` & `syntaxlight-0.1.1/syntaxlight/ast.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/all.css` & `syntaxlight-0.1.1/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/asm.css` & `syntaxlight-0.1.1/syntaxlight/css/asm.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/bnf.css` & `syntaxlight-0.1.1/syntaxlight/css/bnf.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/c.css` & `syntaxlight-0.1.1/syntaxlight/css/c.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/css.css` & `syntaxlight-0.1.1/syntaxlight/css/css.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/index.css` & `syntaxlight-0.1.1/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/json.css` & `syntaxlight-0.1.1/syntaxlight/css/json.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/lua.css` & `syntaxlight-0.1.1/syntaxlight/css/lua.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/makefile.css` & `syntaxlight-0.1.1/syntaxlight/css/makefile.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/shell.css` & `syntaxlight-0.1.1/syntaxlight/css/shell.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/themes.json` & `syntaxlight-0.1.1/syntaxlight/css/themes.json`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/css/toml.css` & `syntaxlight-0.1.1/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/error.py` & `syntaxlight-0.1.1/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/example.py` & `syntaxlight-0.1.1/syntaxlight/example.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/export.py` & `syntaxlight-0.1.1/syntaxlight/export.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/gdt.py` & `syntaxlight-0.1.1/syntaxlight/gdt.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/language.py` & `syntaxlight-0.1.1/syntaxlight/language.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/__init__.py` & `syntaxlight-0.1.1/syntaxlight/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/asm_lexer.py` & `syntaxlight-0.1.1/syntaxlight/lexers/asm_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/bnf_lexer.py` & `syntaxlight-0.1.1/syntaxlight/lexers/bnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.1.1/syntaxlight/lexers/c_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/css_lexer.py` & `syntaxlight-0.1.1/syntaxlight/lexers/css_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.1.1/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/lexer.py` & `syntaxlight-0.1.1/syntaxlight/lexers/lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.1.1/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/makefile_lexer.py` & `syntaxlight-0.1.1/syntaxlight/lexers/makefile_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.1.1/syntaxlight/lexers/shell_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.1.1/syntaxlight/lexers/toml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.1.1/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/parsers/asm_parser.py` & `syntaxlight-0.1.1/syntaxlight/parsers/asm_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/parsers/bnf_parser.py` & `syntaxlight-0.1.1/syntaxlight/parsers/bnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.1.1/syntaxlight/parsers/c_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -740,19 +740,25 @@
             )
 
         return node
 
     def _unknown_typedef_id_guess(self):
         """
         @扩展文法
-        对于 static clock_t ticks = 10; 判定双 ID 则将前一个 clock_t 置为 TYPEDEF_ID
+
+        对于未知符号, 判断下一个 token 类型, 更正为 TYPEDEF_ID
+
+        - static clock_t ticks = 10;                  ID
+        - static clock_t *ticks = 10;                 *
+        - static uint64 (*syscalls[])(void)           (
         """
         if self.current_token.type == TokenType.ID and self.peek_next_token().type in (
             TokenType.ID,
             TokenType.MUL,
+            TokenType.LPAREN
         ):
             self.current_token.type = CTokenType.TYPEDEF_ID
             GDT.register_id(self.current_token.value, CSS.TYPEDEF)
 
     def storage_class_specifier(self):
         """
         <storage-class-specifier> ::= 'auto'
@@ -1956,15 +1962,31 @@
         <designation> ::= <designator>+ "="
         """
         node = Designation()
         designators = [self.designator()]
         while self.current_token.type in self.cfirst_set.designator:
             designators.append(self.designator())
         node.update(designators=designators)
-        node.register_token(self.eat(TokenType.ASSIGN))
+
+        # @扩展文法
+        # 此处为 GNU C 扩展, 正常来说赋值应该为
+        # struct x[] = {
+        #    [0] = 1
+        # }
+        # GNU C 扩展了此处可以不使用等号直接赋值
+        # static uint64 (*syscalls[])(void) = {
+        #     [SYS_fork] sys_fork,   [SYS_exit] sys_exit,     [SYS_wait] sys_wait,     [SYS_pipe] sys_pipe,
+        #     [SYS_read] sys_read,   [SYS_kill] sys_kill,     [SYS_exec] sys_exec,     [SYS_fstat] sys_fstat,
+        #     [SYS_chdir] sys_chdir, [SYS_dup] sys_dup,       [SYS_getpid] sys_getpid, [SYS_sbrk] sys_sbrk,
+        #     [SYS_sleep] sys_sleep, [SYS_uptime] sys_uptime, [SYS_open] sys_open,     [SYS_write] sys_write,
+        #     [SYS_mknod] sys_mknod, [SYS_unlink] sys_unlink, [SYS_link] sys_link,     [SYS_mkdir] sys_mkdir,
+        #     [SYS_close] sys_close,
+        # };
+        if self.current_token.type == TokenType.ASSIGN:
+            node.register_token(self.eat(TokenType.ASSIGN))
         return node
 
     def designator(self):
         """
         <designator> ::= "[" <constant-expression> "]"
                        | "." <identifier>
         """
```

### Comparing `syntaxlight-0.1.0/syntaxlight/parsers/css_parser.py` & `syntaxlight-0.1.1/syntaxlight/parsers/css_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.1.1/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/parsers/lua_parser.py` & `syntaxlight-0.1.1/syntaxlight/parsers/lua_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/parsers/makefile_parser.py` & `syntaxlight-0.1.1/syntaxlight/parsers/makefile_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/parsers/parser.py` & `syntaxlight-0.1.1/syntaxlight/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/parsers/shell_parser.py` & `syntaxlight-0.1.1/syntaxlight/parsers/shell_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.1.1/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.1.1/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/syntaxlight/syntax_parse.py` & `syntaxlight-0.1.1/syntaxlight/syntax_parse.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.0/PKG-INFO` & `syntaxlight-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.1.0
+Version: 0.1.1
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

