# Comparing `tmp/syntaxlight-0.0.9.tar.gz` & `tmp/syntaxlight-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.0.9.tar", max compression
+gzip compressed data, was "syntaxlight-0.1.0.tar", max compression
```

## Comparing `syntaxlight-0.0.9.tar` & `syntaxlight-0.1.0.tar`

### file list

```diff
@@ -1,41 +1,50 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.9/LICENSE
--rw-r--r--   0        0        0      464 2023-07-29 15:18:30.018496 syntaxlight-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2183 2023-07-22 12:55:46.842043 syntaxlight-0.0.9/README.md
--rw-r--r--   0        0        0      187 2023-07-29 14:31:45.643282 syntaxlight-0.0.9/syntaxlight/__init__.py
--rw-r--r--   0        0        0    15173 2023-07-29 13:02:30.287941 syntaxlight-0.0.9/syntaxlight/ast.py
--rw-r--r--   0        0        0     2223 2023-07-29 13:42:32.821896 syntaxlight-0.0.9/syntaxlight/css/all.css
--rw-r--r--   0        0        0      665 2023-07-22 15:03:22.184483 syntaxlight-0.0.9/syntaxlight/css/bnf.css
--rw-r--r--   0        0        0     2118 2023-07-23 15:21:29.646891 syntaxlight-0.0.9/syntaxlight/css/c.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.9/syntaxlight/css/index.css
--rw-r--r--   0        0        0      529 2023-07-21 12:50:35.868013 syntaxlight-0.0.9/syntaxlight/css/json.css
--rw-r--r--   0        0        0     1101 2023-07-26 09:05:41.943038 syntaxlight-0.0.9/syntaxlight/css/lua.css
--rw-r--r--   0        0        0      744 2023-07-29 14:18:59.090972 syntaxlight-0.0.9/syntaxlight/css/shell.css
--rw-r--r--   0        0        0     2812 2023-07-29 14:20:16.175242 syntaxlight-0.0.9/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.9/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.9/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2428 2023-07-26 07:25:50.581952 syntaxlight-0.0.9/syntaxlight/error.py
--rw-r--r--   0        0        0     1947 2023-07-29 15:01:42.303917 syntaxlight-0.0.9/syntaxlight/example.py
--rw-r--r--   0        0        0     1676 2023-07-29 15:00:43.690651 syntaxlight-0.0.9/syntaxlight/export.py
--rw-r--r--   0        0        0     2781 2023-07-29 13:56:47.817032 syntaxlight-0.0.9/syntaxlight/gdt.py
--rw-r--r--   0        0        0     1882 2023-07-29 15:16:31.592870 syntaxlight-0.0.9/syntaxlight/language.py
--rw-r--r--   0        0        0      401 2023-07-24 09:03:19.313778 syntaxlight-0.0.9/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.0.9/syntaxlight/lexers/bnf_lexer.py
--rw-r--r--   0        0        0    12514 2023-07-29 03:41:26.897980 syntaxlight-0.0.9/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.0.9/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    22638 2023-07-29 13:36:11.005583 syntaxlight-0.0.9/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     8150 2023-07-26 08:57:37.822371 syntaxlight-0.0.9/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     4077 2023-07-29 14:16:38.127889 syntaxlight-0.0.9/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3002 2023-07-26 02:47:58.836633 syntaxlight-0.0.9/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.0.9/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      275 2023-07-25 01:05:05.983118 syntaxlight-0.0.9/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.0.9/syntaxlight/parsers/bnf_parser.py
--rw-r--r--   0        0        0    99058 2023-07-29 03:43:10.405548 syntaxlight-0.0.9/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.0.9/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0    35078 2023-07-26 09:03:07.504849 syntaxlight-0.0.9/syntaxlight/parsers/lua_parser.py
--rw-r--r--   0        0        0    12778 2023-07-29 14:00:12.143979 syntaxlight-0.0.9/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0     2344 2023-07-29 14:21:32.659521 syntaxlight-0.0.9/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.0.9/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.0.9/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     2842 2023-07-29 15:18:08.408506 syntaxlight-0.0.9/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.0.9/syntaxlight/template.html
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 syntaxlight-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.0/LICENSE
+-rw-r--r--   0        0        0      463 2023-08-03 06:35:22.027696 syntaxlight-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.0/README.md
+-rw-r--r--   0        0        0      225 2023-07-29 15:28:20.515491 syntaxlight-0.1.0/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.0/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2244 2023-07-30 03:01:17.999345 syntaxlight-0.1.0/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      535 2023-08-01 01:05:24.164690 syntaxlight-0.1.0/syntaxlight/css/asm.css
+-rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.0/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.0/syntaxlight/css/c.css
+-rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.0/syntaxlight/css/css.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.0/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.0/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.0/syntaxlight/css/lua.css
+-rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.0/syntaxlight/css/makefile.css
+-rw-r--r--   0        0        0      876 2023-08-01 01:05:24.169127 syntaxlight-0.1.0/syntaxlight/css/shell.css
+-rw-r--r--   0        0        0     2907 2023-08-02 06:45:18.634086 syntaxlight-0.1.0/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.0/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.0/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.0/syntaxlight/error.py
+-rw-r--r--   0        0        0     1947 2023-07-29 15:01:42.303917 syntaxlight-0.1.0/syntaxlight/example.py
+-rw-r--r--   0        0        0     1926 2023-07-30 02:57:51.649503 syntaxlight-0.1.0/syntaxlight/export.py
+-rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.0/syntaxlight/gdt.py
+-rw-r--r--   0        0        0     2189 2023-08-01 09:07:20.794987 syntaxlight-0.1.0/syntaxlight/language.py
+-rw-r--r--   0        0        0      567 2023-08-02 08:37:35.901602 syntaxlight-0.1.0/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     2645 2023-07-31 03:00:16.388119 syntaxlight-0.1.0/syntaxlight/lexers/asm_lexer.py
+-rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.0/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12853 2023-07-31 01:57:07.230431 syntaxlight-0.1.0/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.0/syntaxlight/lexers/css_lexer.py
+-rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.0/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    24348 2023-08-02 05:55:13.541695 syntaxlight-0.1.0/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.0/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.0/syntaxlight/lexers/makefile_lexer.py
+-rw-r--r--   0        0        0     4457 2023-08-02 08:39:10.819146 syntaxlight-0.1.0/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.0/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.0/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      405 2023-08-01 12:25:00.965587 syntaxlight-0.1.0/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     1099 2023-07-31 01:38:18.589025 syntaxlight-0.1.0/syntaxlight/parsers/asm_parser.py
+-rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.0/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0   103618 2023-07-30 12:40:07.793171 syntaxlight-0.1.0/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.0/syntaxlight/parsers/css_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.0/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.0/syntaxlight/parsers/lua_parser.py
+-rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.0/syntaxlight/parsers/makefile_parser.py
+-rw-r--r--   0        0        0    13420 2023-08-02 07:49:45.535569 syntaxlight-0.1.0/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0     4619 2023-08-02 08:26:36.227646 syntaxlight-0.1.0/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.0/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.0/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.0/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.0/syntaxlight/template.html
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.0/PKG-INFO
```

### Comparing `syntaxlight-0.0.9/LICENSE` & `syntaxlight-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.9/README.md` & `syntaxlight-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # syntaxlight
 
 > 本项目仍在开发中, 尚不可用...
 
-syntaxlight 是一个基于 BNF 的语法高亮的 python 库, 您可以 [在线浏览]() 文法高亮结果
+syntaxlight 是一个基于 BNF 的语法高亮的 python 库, 您可以 [在线浏览](https://luzhixing12345.github.io/syntaxlight/articles/全部文法高亮/C/) 文法高亮结果
 
 目前支持 C/Python 等主流编程语言和 json xml 等主流标记语言的文法解析, 支持多种高亮主题以及自定义颜色(默认使用 Vscode 风格), 您可在此查看[全部文法支持和高亮支持](https://luzhixing12345.github.io/syntaxlight/articles/%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C/%E5%85%A8%E9%83%A8%E6%96%87%E6%B3%95%E6%94%AF%E6%8C%81/)
 
 ## 安装
 
 ```bash
 pip install syntaxlight
```

### Comparing `syntaxlight-0.0.9/syntaxlight/ast.py` & `syntaxlight-0.1.0/syntaxlight/ast.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,16 +214,24 @@
     def __init__(self, constant) -> None:
         super().__init__()
         self.constant = constant
         self.is_leaf_ast = True
         self.node_info += f"\\n{self.constant}"
 
 
+class WrapString(AST):
+    def __init__(self) -> None:
+        super().__init__()
+        self.strings = None
+    def visit(self, node_visitor: "NodeVisitor" = None):
+        node_visitor.link(self, self.strings)
+        return super().visit(node_visitor)
+
 class String(AST):
-    def __init__(self, string) -> None:
+    def __init__(self, string = None) -> None:
         super().__init__()
         self.string: str = string
         self.is_leaf_ast = True
 
         string_info = self.string.replace("\\", "\\\\").replace('"', '\\"')
         self.node_info += f"\\n{string_info}"
```

### Comparing `syntaxlight-0.0.9/syntaxlight/css/all.css` & `syntaxlight-0.1.0/syntaxlight/css/all.css`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     color: #DCDCAA; /* @--function int func() */
     color: #4EC9B0; /* @--struct class */
     color: #D7BA6E; /* @--controlchar \n\t */
     color: #4FC1FF; /* @--enum type */
     color: #88D6FE; /* @--format type */
     color: #9EB2BF; /* @--punctuator . ; :  */
     color: #D4D4D4; /* @--operator +-*=  */
+    color: #969696;
 }
 
 .one-dark-pro {
     color: #23272E; /* @--background */
     color: #DA4D3E; /* @--variant a */
     color: #C678DD; /* @--type int */
     color: #C678DD; /* @--define include */
```

### Comparing `syntaxlight-0.0.9/syntaxlight/css/bnf.css` & `syntaxlight-0.1.0/syntaxlight/css/bnf.css`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-pre[class*="language-"] {
+pre[class*="language-bnf"] {
     background: --background;
 }
 
 .Token {
     color: --punctuator;
 }
 
-.Token.brace-depth-0 {
+.Token.BraceDepth-0 {
     color: --brace1;
 }
 
-.Token.brace-depth-1 {
+.Token.BraceDepth-1 {
     color: --brace2;
 }
 
-.Token.brace-depth-2 {
+.Token.BraceDepth-2 {
     color: --brace3;
 }
 
 .Token.RuleName {
     color: --struct;
 }
 
@@ -42,10 +42,11 @@
     color: --define;
 }
 
 .Token.BuiltinSymbol {
     color: --variant;
 }
 
-.Token.RANGLE_BRACE, .Token.LANGLE_BRACE {
+.Token.RANGLE_BRACE,
+.Token.LANGLE_BRACE {
     color: --punctuator;
 }
```

### Comparing `syntaxlight-0.0.9/syntaxlight/css/c.css` & `syntaxlight-0.1.0/syntaxlight/css/c.css`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-pre[class*="language-"] {
+pre[class*="language-c"] {
     background: --background;
 }
 
 .Token {
     color: --punctuator;
 }
 
-.Token.brace-depth-0 {
+.Token.BraceDepth-0 {
     color: --brace1;
 }
 
-.Token.brace-depth-1 {
+.Token.BraceDepth-1 {
     color: --brace2;
 }
 
-.Token.brace-depth-2 {
+.Token.BraceDepth-2 {
     color: --brace3;
 }
 
 .Token.VOID,
 .Token.CHAR,
 .Token.SHORT,
 .Token.INT,
@@ -36,15 +36,16 @@
 .Token.EXTERN,
 .Token.TYPEDEF,
 .Token.CONST,
 .Token.VOLATITLE,
 .Token.RESTRICT,
 .Token._ATOMIC,
 .Token._STATIC_ASSERT,
-.Token._GENERIC {
+.Token._GENERIC,
+.Token.GNU-C-Extension {
     color: --type;
 }
 
 .Token.ID {
     color: --variant;
 }
 
@@ -78,14 +79,15 @@
     color: --define;
 }
 
 .Token.IF,
 .Token.ELSE,
 .Token.FOR,
 .Token.WHILE,
+.Token.DO,
 .Token.SWITCH,
 .Token.CASE,
 .Token.DEFAULT {
     color: --define;
 }
 
 
@@ -97,16 +99,19 @@
 
 .Token.HeaderName {
     color: --string;
     border-bottom: 1px solid --string;
 }
 
 .Token.StorageType,
+.Token.FunctionType,
 .Token.QualifyType,
 .Token.StructureType,
+.Token.STRUCT,
+.Token.UNION,
 .Token.EnumSpecifier {
     color: --type;
 }
 
 .Token.FunctionName.ID,
 .Token.FunctionCall.ID {
     color: --function;
@@ -143,15 +148,19 @@
     color: --operator;
 }
 
 .Token.Control {
     color: --controlchar;
 }
 
-.Token.COMMA, .Token.COLON, .Token.DOT, .Token.SEMI, .Token.GotoLabel {
+.Token.COMMA,
+.Token.COLON,
+.Token.DOT,
+.Token.SEMI,
+.Token.GotoLabel {
     color: --punctuator;
 }
 
 
 .Token.COMMENT {
     color: --comment;
 }
```

### Comparing `syntaxlight-0.0.9/syntaxlight/css/index.css` & `syntaxlight-0.1.0/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.9/syntaxlight/css/json.css` & `syntaxlight-0.1.0/syntaxlight/css/toml.css`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-pre[class*="language-"] {
+pre[class*="language-toml"] {
     background: --background;
 }
 
 .Token {
     color: --punctuator;
 }
 
-.Token.brace-depth-0 {
+.Token.String {
+    color: --string;
+}
+
+.Token.BraceDepth-0 {
     color: --brace1;
 }
 
-.Token.brace-depth-1 {
+.Token.BraceDepth-1 {
     color: --brace2;
 }
 
-.Token.brace-depth-2 {
+.Token.BraceDepth-2 {
     color: --brace3;
 }
 
-.Token.Pair.Key {
-    color: --variant;
+.Token.NUMBER {
+    color: --number;
 }
 
-.Token.COMMA, .Token.COLON {
-    color: --punctuator;
+
+.Token.Path {
+    color: --type;
 }
 
-.Token.UnaryOp,
-.Token.Keyword,
-.Token.NUMBER {
-    color: --number;
+.Token.TableArrayHeader.Path,
+.Token.TableHeader.Path {
+    color: --variant;
 }
 
-.Token.STRING {
-    color: --string;
+.Token.Date {
+    color: --number;
 }
 
 .Token.COMMENT {
     color: --comment;
 }
```

### Comparing `syntaxlight-0.0.9/syntaxlight/css/lua.css` & `syntaxlight-0.1.0/syntaxlight/css/json.css`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,42 @@
-pre[class*="language-"] {
+pre[class*="language-json"] {
     background: --background;
 }
 
 .Token {
     color: --punctuator;
 }
 
-.Token.brace-depth-0 {
+.Token.BraceDepth-0 {
     color: --brace1;
 }
 
-.Token.brace-depth-1 {
+.Token.BraceDepth-1 {
     color: --brace2;
 }
 
-.Token.brace-depth-2 {
+.Token.BraceDepth-2 {
     color: --brace3;
 }
 
-.Token.STR {
-    color: --string;
-}
-
-.Token.STR.Format {
-    color: --format;
-}
-
-.Token.AttributeType.ID {
-    color: --string;
-}
-
-.Token.Attribute.LANGLE_BRACE, .Token.Attribute.RANGLE_BRACE {
-    color: --punctuator;
-}
-
-
-.Token.Control {
-    color: --controlchar;
-}
-
-.Token.Keyword {
-    color: --define;
-}
-
-.Token.LOCAL {
-    color: --type;
-}
-
-.Token.ID {
+.Token.Pair.Key {
     color: --variant;
 }
 
-.Token.FunctionName.ID,
-.Token.FunctionCall.ID {
-    color: --function;
-}
-
-.Token.Field.ID, .Token.TableKey {
-    color: --struct;
-}
-
-.Token.TRUE, .Token.FALSE, .Token.NIL {
-    color: --type;
+.Token.COMMA,
+.Token.COLON {
+    color: --punctuator;
 }
 
-.Token.AND, .Token.NOT, .Token.OR {
-    color: --punctuator;
+.Token.UnaryOp,
+.Token.Keyword,
+.Token.NUMBER {
+    color: --number;
 }
 
-.Token.COLON, .Token.DOUBLE_COLON {
-    color: --type;
+.Token.STRING {
+    color: --string;
 }
 
 .Token.COMMENT {
     color: --comment;
-}
-
-.Token.NUMBER {
-    color: --number;
-}
+}
```

### Comparing `syntaxlight-0.0.9/syntaxlight/css/shell.css` & `syntaxlight-0.1.0/syntaxlight/css/css.css`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,52 @@
-pre[class*="language-"] {
+pre[class*="language-css"] {
     background: --background;
 }
 
 .Token {
     color: --punctuator;
 }
 
-.Token.brace-depth-0 {
+.Token.ID {
+    color: --string;
+}
+
+.Token.BraceDepth-0 {
     color: --brace1;
 }
 
-.Token.brace-depth-1 {
+.Token.BraceDepth-1 {
     color: --brace2;
 }
 
-.Token.brace-depth-2 {
+.Token.BraceDepth-2 {
     color: --brace3;
 }
 
+.Token.NUMBER {
+    color: --number;
+}
 
-.Token.PATH {
+.Token.KEY {
     color: --variant;
 }
 
-.Token.Program, .Token.Function {
+.Token.CLASS_NAME,
+.Token.HASH_ID {
     color: --function;
 }
 
-
-.Token.STR {
-    color: --string;
-}
-
-.Token.NUMBER {
-    color:  --number;
-}
-
 .Token.COMMENT {
     color: --comment;
 }
 
-.Token.Keyword {
-    color: --define;
-}
-
-
-.Token.GlobalVariant {
-    color: --type;
-}
-
-.Token.Variant, .Token.VARIANT {
-    color: --variant;
+.Token.FUNCTION {
+    color: --function;
 }
 
-.Token.Format {
-    color: --format;
+.Token.COLOR {
+    color: --string;
 }
 
-.Token.Control {
-    color: --control;
+.Token.STRING {
+    color: --string;
 }
```

### Comparing `syntaxlight-0.0.9/syntaxlight/css/themes.json` & `syntaxlight-0.1.0/syntaxlight/css/themes.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985532407407408%*

 * *Differences: {"'vscode'": "{'extension': {'shell': {'.Token.OPTION': 'color: #b3b2b2;'}, 'makefile': "*

 * *             "OrderedDict([('.Token.OPTION', 'color: #b3b2b2;')])}}"}*

```diff
@@ -75,16 +75,19 @@
         "--struct": "#4EC9B0",
         "--type": "#569cd6",
         "--variant": "#88D6FE",
         "extension": {
             "json": {
                 ".Token.Keyword": "color: #327ED0;"
             },
+            "makefile": {
+                ".Token.OPTION": "color: #b3b2b2;"
+            },
             "shell": {
-                ".Token.OPTION": "color: #ABABAB;"
+                ".Token.OPTION": "color: #b3b2b2;"
             },
             "toml": {
                 ".Token.Keyword": "color: #327ED0;"
             }
         }
     }
 }
```

### Comparing `syntaxlight-0.0.9/syntaxlight/css/toml.css` & `syntaxlight-0.1.0/syntaxlight/css/shell.css`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,71 @@
-pre[class*="language-"] {
+pre[class*="language-shell"] {
     background: --background;
 }
 
 .Token {
     color: --punctuator;
 }
 
-.Token.String {
-    color: --string;
-}
-
-.Token.brace-depth-0 {
+.Token.BraceDepth-0 {
     color: --brace1;
 }
 
-.Token.brace-depth-1 {
+.Token.BraceDepth-1 {
     color: --brace2;
 }
 
-.Token.brace-depth-2 {
+.Token.BraceDepth-2 {
     color: --brace3;
 }
 
+.Token.Program,
+.Token.Function,
+.Token.BACK_SLASH {
+    color: --function;
+}
+
+
+.Token.STRING {
+    color: --string;
+}
+
 .Token.NUMBER {
     color: --number;
 }
 
+.Token.COMMENT {
+    color: --comment;
+}
 
-.Token.Path {
-    color: --type;
+.Token.Keyword {
+    color: --define;
 }
 
-.Token.TableArrayHeader.Path,
-.Token.TableHeader.Path {
+/* .Token.OPTION {
+    color: --type;
+} */
+
+.Token.Variant,
+.Token.VARIANT {
     color: --variant;
 }
 
-.Token.Date {
-    color: --number;
+.Token.Format {
+    color: --format;
 }
 
-.Token.COMMENT {
-    color: --comment;
+.Token.Control {
+    color: --control;
+}
+
+.Token.Url {
+    border-bottom: 1px solid --punctuator;
+}
+
+.Token.HOST_NAME {
+    color: --struct;
+}
+
+.Token.DIR_PATH {
+    color: --type;
 }
```

### Comparing `syntaxlight-0.0.9/syntaxlight/error.py` & `syntaxlight-0.1.0/syntaxlight/error.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     UNTERMINATED_STRING = 'unterminated string'
     MULTICHARACTER_CONSTANT = 'Multi-character character constant'
 
     # parser error code
     UNEXPECTED_TOKEN = "Unexpected token"
     MISS_EXPECTED_TOKEN = "Miss expected token"
     TRAILING_COMMA = "Trailing comma not allowed"
+    BRACE_MISS_MATCH = 'brace number miss match'
 
 
 class Error(Exception):
     def __init__(
         self,
         error_code=None,
         token=None,
```

### Comparing `syntaxlight-0.0.9/syntaxlight/example.py` & `syntaxlight-0.1.0/syntaxlight/example.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.9/syntaxlight/export.py` & `syntaxlight-0.1.0/syntaxlight/export.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import os
 from typing import Dict, List
 import json
-
+from .language import clean_language
 
 def export_css(languages: List[str], export_dir: str = ".", style: str = "vscode"):
     syntaxlight_path = os.path.dirname(__file__)
     json_file_path = os.path.join(syntaxlight_path, "css", "themes.json")
     with open(json_file_path, "r", encoding="utf-8") as f:
         themes: Dict[str, Dict[str, str]] = json.load(f)
 
     EXTENSION_NAME = "extension"
 
     if style in themes:
         theme = themes[style]
         for language in languages:
+            language = clean_language(language)
             origin_css_file = os.path.join(syntaxlight_path, "css", f"{language}.css")
             if not os.path.exists(origin_css_file):
                 print(f"no {language} css file")
                 exit(1)
             with open(origin_css_file, "r", encoding="utf-8") as f:
                 css_content = f.read()
-
+            
             # 应用扩展, 完善 CSS
             if EXTENSION_NAME in theme:
                 if language in theme[EXTENSION_NAME]:
                     for class_name, css in theme[EXTENSION_NAME][language].items():
                         css_content += "\n" + class_name + " {\n    " + css + "\n}"
 
             # 使用主题颜色替换 css 文件中的对应类型
             for type_name, color in theme.items():
                 if type_name == EXTENSION_NAME:
                     continue
 
                 css_content = css_content.replace(type_name, color)
-
+            
+            # 添加对应的作用域
+            css_content = css_content.replace('.Token',f'pre[class*="language-{language}"] .Token')
             with open(f'{export_dir}/{language}.css', "w", encoding="utf-8") as f:
                 f.write(css_content)
     else:
         print(f"unknown style {style}")
         print(f"supported style: {list(themes.keys())}")
         exit(1)
```

### Comparing `syntaxlight-0.0.9/syntaxlight/gdt.py` & `syntaxlight-0.1.0/syntaxlight/gdt.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,7 +85,11 @@
     def __getitem__(self, name) -> Enum:
         if name not in self._descriptors:
             return None
         return self._descriptors[name]["type"]
 
     def __contains__(self, item):
         return item in self._descriptors
+
+    def __repr__(self) -> str:
+        
+        return str(list(self._descriptors.keys()))
```

### Comparing `syntaxlight-0.0.9/syntaxlight/language.py` & `syntaxlight-0.1.0/syntaxlight/language.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from .lexers import *
 from .parsers import *
+import re
 from typing import List, TypedDict
 
 class SyntaxDict(TypedDict):
     lexer: Lexer
     parser: Parser
     suffix: List[str]
 
@@ -12,24 +13,28 @@
     "json": SyntaxDict(lexer=JsonLexer, parser=JsonParser, suffix=['json']),
     "c": SyntaxDict(lexer=CLexer, parser=CParser, suffix=["c", "h"]),
     "lua": SyntaxDict(lexer=LuaLexer, parser=LuaParser, suffix=['lua']),
     "bnf": SyntaxDict(lexer=BNFLexer, parser=BNFParser, suffix=['bnf']),
     "toml": SyntaxDict(lexer=TomlLexer, parser=TomlParser, suffix=['toml']),
     "xml": SyntaxDict(lexer=XmlLexer, parser=XmlParser, suffix=['xml']),
     "shell": SyntaxDict(lexer=ShellLexer, parser=ShellParser, suffix=['sh']),
+    "asm": SyntaxDict(lexer=AssemblyLexer, parser=AssemblyParser, suffix=['asm']),
+    "css": SyntaxDict(lexer=CSSLexer,parser=CSSParser, suffix=['css']),
+    "makefile": SyntaxDict(lexer=MakefileLexer,parser=MakefileParser, suffix=['mk','mak'])
 }
 
 def clean_language(language:str):
     
     language = language.lower()
     rename_languages = {
-        'bash': 'shell'
+        r'^bash$': 'shell',
+        r'.*?asm.*?': 'asm'
     }
     for r_language in rename_languages:
-        if language == r_language:
+        if bool(re.match(r_language, language)):
             return rename_languages[r_language]
         
     return language
 
 def guess_language(file_path: str) -> str:
     """
     通过文件名猜测文法类型
```

### Comparing `syntaxlight-0.0.9/syntaxlight/lexers/bnf_lexer.py` & `syntaxlight-0.1.0/syntaxlight/lexers/bnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.9/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.1.0/syntaxlight/lexers/c_lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     TRUE = "true"  # C23
     TYPEDEF = "typedef"
     TYPEOF = "typeof"  # C23
     TYPEOF_UNQUAL = "typeof_unqual"  # C23
     UNION = "union"
     UNSIGNED = "unsigned"
     VOID = "void"
-    VOLATITLE = "volatile"
+    VOLATILE = "volatile"
     WHILE = "while"
     _ALIGNAS = "_Alignas"  # C23 => ALIGNAS
     ALIGNAS = "alignas"
     _ATOMIC = "_Atomic"
     _BITINT = "_BitInt"
     _BOOL = "_Bool"  # C23 => BOOL
     _COMPLEX = "_Complex"
@@ -60,14 +60,18 @@
     _DECIMAL64 = "_Decimal64"  # C23
     _GENERIC = "_Generic"
     _IMAGINARY = "_Imaginary"
     _NORETURN = "_Noreturn"
     _STATIC_ASSERT = "_Static_assert"  # C23 => STATIC_ASSERT
     _THREAD_LOCAL = "_Thread_local"  # C23 => THREAD_LOCAL
 
+    # GNU C extension
+    _ASM = "__asm__"
+    _ATTRIBUTE = "__attribute__"
+
     RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
     # start - end 之间为对应语言的保留关键字
     # -----------------------------------------------
 
     POINTER = "POINTER"
     STAR = "STAR"
     TYPEDEF_ID = "typedef-id"
@@ -145,15 +149,20 @@
 
             if self.current_char == "/" and self.peek() == "/":
                 return self.get_comment("//", "\n")
             if self.current_char == "/" and self.peek() == "*":
                 return self.get_comment("/*", "*/")
 
             if self.current_char.isdigit():
-                return self.get_number(accept_hex=True, accept_bit=True,accept_p=True)
+                return self.get_number(
+                    accept_hex=True,
+                    accept_bit=True,
+                    accept_p=True,
+                    end_chars=["f", "F", "l", "L", "U", "u"],
+                )
 
             if self.current_char.isalpha() or self.current_char == TokenType.UNDERLINE.value:
                 return self.get_id()
 
             if self.current_char == '"':
                 return self.get_string()
 
@@ -208,15 +217,15 @@
             CTokenType.BOOL,
             self.atomic_type_specifier,
             self.struct_or_union_specifier,
             self.enum_specifier,
             self.typedef_name,
         )
         self.type_qualifier = TokenSet(
-            CTokenType.CONST, CTokenType.VOLATITLE, CTokenType.RESTRICT, CTokenType._ATOMIC
+            CTokenType.CONST, CTokenType.VOLATILE, CTokenType.RESTRICT, CTokenType._ATOMIC
         )
         self.function_speficier = TokenSet(CTokenType.INLINE, CTokenType._NORETURN)
         self.alignment_specifier = TokenSet(CTokenType._ALIGNAS)
         self.declaration_specifier = TokenSet(
             self.storage_class_specifier,
             self.type_specifier,
             self.type_qualifier,
@@ -305,21 +314,23 @@
         self.expression_statement = TokenSet(self.expression, TokenType.SEMI)
         self.compound_statement = TokenSet(TokenType.LCURLY_BRACE)
         self.selection_statement = TokenSet(CTokenType.IF, CTokenType.SWITCH)
         self.iteration_statement = TokenSet(CTokenType.WHILE, CTokenType.DO, CTokenType.FOR)
         self.jump_statement = TokenSet(
             CTokenType.GOTO, CTokenType.CONTINUE, CTokenType.BREAK, CTokenType.RETURN
         )
+        self.gnu_c_statement_extension = TokenSet(CTokenType._ASM)
         self.statement = TokenSet(
             self.labeled_statement,
             self.expression_statement,
             self.compound_statement,
             self.selection_statement,
             self.iteration_statement,
             self.jump_statement,
+            self.gnu_c_statement_extension,
         )
         self.external_declaration = TokenSet(
             self.function_definition, self.declaration, self.group_part, self.statement
         )
         self.block_item = TokenSet(self.declaration, self.statement, self.group)
         self.init_declarator_list = TokenSet(self.declarator)
         self.identifier_list = TokenSet(TokenType.ID)
```

### Comparing `syntaxlight-0.0.9/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.1.0/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.9/syntaxlight/lexers/lexer.py` & `syntaxlight-0.1.0/syntaxlight/lexers/lexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from ..error import ErrorCode, LexerError
 from typing import Dict, List, Tuple
 import re
 
+
 GLOBAL_TOKEN_ID = 0
 
 # class NewTokenType(Enum):
 #     RESERVED_KEYWORD_START = "RESERVED_KEYWORD_START"
 #     RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
 
 
@@ -57,14 +58,15 @@
     ID = "ID"
     STRING = "STRING"  # STRING 表示严格意义上的字符串, 即 "" 两个双引号包裹的
     CHARACTER = "CHARACTER"  # CHARACTER 表示单个字符, 即 'a'
     STR = "STR"  # STR 表示 "" | '' 包裹的字符串
     NUMBER = "NUMBER"  # 整数 | 小数 | 科学计数法
     INT = "INT"  # 整数
     FLOAT = "FLOAT"  # 小数
+    TEXT = "TEXT"  # 未知的字符
     COMMENT = "COMMENT"
     SHL = "<<"
     SHR = ">>"
     EQ = "=="
     STRICT_EQ = "==="
     NE = "!="
     NORE = "~="
@@ -106,15 +108,15 @@
     CYAN = 96
     WHITE = 97
 
 
 class Token:
     def __init__(self, type: Enum, value, line=None, column=None):
         self.type: Enum = type
-        self.value:str = value
+        self.value: str = value
         self.line: int = line
         self.column: int = column
         self.ast: None
         self.class_list = set()  # parser 语法分析阶段赋给 token
         self.class_list.add("Token")
         global GLOBAL_TOKEN_ID
         self._id = GLOBAL_TOKEN_ID
@@ -138,17 +140,18 @@
         return "Token[{ID}]({type}, {value}, position={lineno}:{column})".format(
             ID=self._id,
             type=self.type,
             value=repr(self.value),
             lineno=self.line,
             column=self.column,
         )
-    
+
     def add_css(self, CSS: Enum):
-        self.class_list.add(CSS.value)
+        if CSS is not None:
+            self.class_list.add(CSS.value)
 
     def __repr__(self):
         return self.__str__()
 
 
 class Lexer:
     """
@@ -168,19 +171,22 @@
         self.LanguageTokenType: Enum = LanguageTokenType
         self.context_bias = 10  # 发生错误时 token 的前后文行数
         self.file_path = None  # 手动修改文件路径, 用于后期错误处理的输出
         self._status_stack = []  # 状态栈
 
         # 获取 RESERVED_KEYWORD_START - RESERVED_KEYWORD_END 之间的保留关键字
         tt_list = list(LanguageTokenType)
-        start_index = tt_list.index(LanguageTokenType.RESERVED_KEYWORD_START)
-        end_index = tt_list.index(LanguageTokenType.RESERVED_KEYWORD_END)
-        self.reserved_keywords = {
-            token_type.value: token_type for token_type in tt_list[start_index + 1 : end_index]
-        }
+        try:
+            start_index = tt_list.index(LanguageTokenType.RESERVED_KEYWORD_START)
+            end_index = tt_list.index(LanguageTokenType.RESERVED_KEYWORD_END)
+            self.reserved_keywords = {
+                token_type.value: token_type for token_type in tt_list[start_index + 1 : end_index]
+            }
+        except:
+            self.reserved_keywords = {}
         # 不可见字符, 一般情况下直接忽略即可, 这里考虑到为了不破坏原本的代码格式所以进行保留
         # \n \t \v \r \f \b
         self.invisible_characters = [
             TokenType.LF.value,
             TokenType.TAB.value,
             TokenType.VERTICAL_TAB.value,
             TokenType.CR.value,
@@ -349,56 +355,62 @@
         """
         peek_pos = self.pos + n
         if peek_pos > len(self.text) - 1:
             return None
         else:
             return self.text[self.pos + 1 : peek_pos + 1]
 
-    def get_number(self, accept_float = True, accept_hex = False, accept_bit = False, accept_p = False) -> Token:
+    def get_number(
+        self,
+        accept_float=True,
+        accept_hex=False,
+        accept_bit=False,
+        accept_p=False,
+        end_chars: List[str] = [],
+    ) -> Token:
         """
          <digit> ::= [0-9]
         <digits> ::= <digit>*
         <number> ::= <digits>(.<digits>)?(E|e[+-]?<digits>)?
 
         @accept_float: 允许小数和科学计数法
         @accept_hex  : 允许16进制表示 0xfff
         @accept_bit  : 允许二进制表示 0b111
         @accept_p    : 允许后面跟 P/p
         """
         bit_matching_status = False
         hex_matching_status = False
-        def is_match_char(char:str) -> bool:
-            
+
+        def is_match_char(char: str) -> bool:
             if hex_matching_status:
-                return bool(re.match(r'[0-9a-fA-F]',char))
+                return bool(re.match(r"[0-9a-fA-F]", char))
             if bit_matching_status:
-                return bool(re.match(r'[01]',char))
+                return bool(re.match(r"[01]", char))
             return char.isdigit()
 
         result = ""
 
         if accept_hex:
-            if self.current_char == '0' and self.peek() in ('x', 'X'):
+            if self.current_char == "0" and self.peek() in ("x", "X"):
                 result = self.current_char
                 self.advance()
                 result += self.current_char
                 self.advance()
                 hex_matching_status = True
 
         if accept_bit:
-            if self.current_char == '0' and self.peek() in ('b', 'B'):
+            if self.current_char == "0" and self.peek() in ("b", "B"):
                 result = self.current_char
                 self.advance()
                 result += self.current_char
                 self.advance()
-                # 如果此时已经处于 hex_matching_status 状态了则忽略 
+                # 如果此时已经处于 hex_matching_status 状态了则忽略
                 if not hex_matching_status:
                     bit_matching_status = True
 
-
         # <digits>
         while self.current_char is not None and is_match_char(self.current_char):
             result += self.current_char
             self.advance()
 
         if accept_float:
             # (.<digits>)?
@@ -415,26 +427,29 @@
                 self.advance()
                 if self.current_char in (TokenType.MINUS.value, TokenType.PLUS.value):
                     result += self.current_char
                     self.advance()
                 while self.current_char is not None and is_match_char(self.current_char):
                     result += self.current_char
                     self.advance()
-        
+
         if accept_p:
-            if self.current_char in ('P','p'):
+            if self.current_char in ("P", "p"):
                 result += self.current_char
                 self.advance()
                 if self.current_char in (TokenType.MINUS.value, TokenType.PLUS.value):
                     result += self.current_char
                     self.advance()
                 while self.current_char is not None and is_match_char(self.current_char):
                     result += self.current_char
                     self.advance()
 
+        while self.current_char in end_chars:
+            result += self.current_char
+            self.advance()
         # column - 1, 因为判断结束需要跳出 number
         return Token(TokenType.NUMBER, result, self.line, self.column - 1)
 
     def get_string(self):
         """
         严格双引号 ""
         """
@@ -469,23 +484,27 @@
             token = Token(TokenType.STRING, result, self.line, self.column)
             self.advance()
             self.error(ErrorCode.UNEXPECTED_TOKEN, token)
         end_character = self.current_char  # 结束标志一定是和开始标志相同的
         self.advance()
 
         while self.current_char is not None and self.current_char != end_character:
-            result += self.current_char
             if self.current_char == "\\":
+                result += self.current_char
                 self.advance()
                 if self.current_char is None:
                     self.error(
                         ErrorCode.UNEXPECTED_TOKEN,
                         Token(TokenType.STRING, result, self.line, self.column - 1),
                     )
-                result += self.current_char
+                # 对于 '\' 和 "\" 直接结束
+                # print(self.current_char)
+                if self.current_char == end_character and self.peek() in (" ", "\n"):
+                    break
+            result += self.current_char
             self.advance()
 
         result += end_character
         token = Token(TokenType.STR, result, self.line, self.column)
         self.advance()
         return token
 
@@ -593,15 +612,16 @@
             self.advance()
 
         # 除单行注释外抛异常
         if self.current_char is None and end_symbol != "\n":
             token = Token(TokenType.COMMENT, result, self.line, self.column - 1)
             self.error(ErrorCode.UNTERMINATED_COMMENT, token)
 
-        if end_symbol == "\n":
+        # 对于单行注释以 \n 为终止符的, 将最后一个 \n 去掉
+        if end_symbol == "\n" and result[-1] == "\n":
             result = result[:-1]
             token = Token(TokenType.COMMENT, result, self.line, self.column - 1)
         else:
             token = Token(TokenType.COMMENT, result, self.line, self.column)
             self.advance()
         return token
 
@@ -613,27 +633,55 @@
         assert self.current_char in self.long_op_dict
         token_type = TokenType(self.current_char)
         result = self.current_char
 
         for long_op in self.long_op_dict[self.current_char]:
             if self.peek(len(long_op)) == long_op:
                 result = self.current_char + long_op
-                token_type = TokenType(result)
+                try:
+                    token_type = TokenType(result)
+                except:
+                    token_type = self.LanguageTokenType(result)
                 for _ in range(len(long_op)):
                     self.advance()
                 break
 
         token = Token(token_type, result, self.line, self.column)
         self.advance()
         return token
 
     def get_next_token(self) -> Token:
         """
         while self.current_char is not None:
-            # do something
+            if self.current_char == TokenType.SPACE.value:
+                return self.skip_whitespace()
+
+            if self.current_char in self.invisible_characters:
+                return self.skip_invisiable_character()
+
+            # your code
+
+            try:
+                token_type = TokenType(self.current_char)
+            except ValueError:  # pragma: no cover
+                token = Token(TokenType.TEXT, self.current_char, self.line, self.column)
+                self.advance()
+                return token
+            else:
+                token = Token(
+                    type=token_type,
+                    value=token_type.value,  # e.g. ';', '.', etc
+                    line=self.line,
+                    column=self.column,
+                )
+                self.advance()
+                return token
+
+        # End of File
+        return Token(type=TokenType.EOF, value="EOF", line=self.line, column=self.column)
         """
         raise NotImplementedError
 
 
 class TokenSet:
     def __init__(self, *args) -> None:
         self._token_set = set()
```

### Comparing `syntaxlight-0.0.9/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.1.0/syntaxlight/lexers/lua_lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
     RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
     # start - end 之间为对应语言的保留关键字
     # -----------------------------------------------
 
 
 class LuaLexer(Lexer):
-    def __init__(self, text: str, TokenType: TokenType = LuaTokenType):
-        super().__init__(text, TokenType)
+    def __init__(self, text: str, LanguageTokenType: Enum = LuaTokenType):
+        super().__init__(text, LanguageTokenType)
         self.build_long_op_dict(["//", ">>", "<<", "..", "...", "<=", ">=", "==", "~=", "::"])
 
     def get_literal_str(self):
         """
         [[ ... ]]
         [====[ ]====]
         数量相等的匹配长换行字符串
```

### Comparing `syntaxlight-0.0.9/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.1.0/syntaxlight/lexers/xml_lexer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,103 @@
-from .lexer import Lexer, Token, TokenType, ErrorCode
+from .lexer import Lexer, Token, TokenType, TokenSet, ErrorCode
 from enum import Enum
 
 
-class ShellTokenType(Enum):
+class XmlTokenType(Enum):
     RESERVED_KEYWORD_START = "RESERVED_KEYWORD_START"
-    IF = "if"
-    ELIF = "elif"
-    ELSE = "else"
-    THEN = "then"
-    FI = "fi"
-    FOR = "for"
-    DO = "do"
-    IN = "in"
-    DONE = "done"
-    WHILE = "while"
-    BREAK = "break"
-
     RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
 
-    OPTION = "option"
-    PATH = "path"
-    VARIANT = "variant"
-    REDIRECT_TO = ">"
-    REDIRECT_FROM = "<"
+    PROLOG_START = "<?xml"
+    PROLOG_END = "?>"
+    TAG_START_BEGIN = "<"
+    TAG_END = ">"
+    TAG_COMPLETE_BEGIN = '</'
+    TAG_SELF_END = "/>"
+    NAME = "NAME"
+    CONTENT = "CONTENT"
 
 
-class ShellLexer(Lexer):
-    def __init__(self, text: str, LanguageTokenType: Enum = ShellTokenType):
+class XmlLexer(Lexer):
+    def __init__(self, text: str, LanguageTokenType: Enum = XmlTokenType):
         super().__init__(text, LanguageTokenType)
-
-    def get_option(self):
-        """
-        长短选项
-        -s --options
-        """
-        result = ""
-        while self.current_char is not None:
-            if self.current_char.isalnum() or self.current_char in ("-", "_"):
-                result += self.current_char
-                self.advance()
-            else:
-                break
-
-        return Token(ShellTokenType.OPTION, result, self.line, self.column - 1)
-
-    def get_path(self):
-        """
-        /proc/xxx
-        /usr/lib/...
-        """
-        result = ""
-        while self.current_char is not None:
-            if self.current_char.isalnum() or self.current_char in ("/", "-", "_", "."):
-                result += self.current_char
-                self.advance()
-            else:
-                break
-        return Token(ShellTokenType.PATH, result, self.line, self.column - 1)
-
-    def shell_variant(self):
-        """
-        $i
-        $mysh
-        """
-        result = "$"
-        self.advance()
-        while self.current_char is not None:
-            if self.current_char.isalnum() or self.current_char in ("-", "_"):
-                result += self.current_char
-                self.advance()
-            else:
-                break
-        return Token(ShellTokenType.VARIANT, result, self.line, self.column - 1)
+        self.content_matching = False
 
     def get_next_token(self) -> Token:
         while self.current_char is not None:
+            if self.content_matching:
+                result = ""
+                while self.current_char is not None and self.current_char != "<":
+                    result += self.current_char
+                    self.advance()
+                self.content_matching = False
+                return Token(XmlTokenType.CONTENT, result, self.line, self.column - 1)
+
             if self.current_char == TokenType.SPACE.value:
                 return self.skip_whitespace()
 
             if self.current_char in self.invisible_characters:
                 return self.skip_invisiable_character()
 
+            if self.current_char == "<":
+                if self.peek(4) == "?xml":
+                    result = "<?xml"
+                    self.advance()
+                    self.advance()
+                    self.advance()
+                    self.advance()
+                    token = Token(XmlTokenType.PROLOG_START, result, self.line, self.column)
+                    self.advance()
+                    return token
+                elif self.peek(3) == "!--":
+                    return self.get_comment("<!--", "-->")
+                elif self.peek() == "/":
+                    self.advance()
+                    token = Token(XmlTokenType.TAG_COMPLETE_BEGIN, "</", self.line, self.column)
+                    self.advance()
+                    return token
+                else:
+                    token = Token(
+                        XmlTokenType.TAG_START_BEGIN, self.current_char, self.line, self.column
+                    )
+                    self.advance()
+                    return token
+            if self.current_char == "/" and self.peek() == ">":
+                self.advance()
+                token = Token(XmlTokenType.TAG_SELF_END, "/>", self.line, self.column)
+                self.advance()
+                return token
+            if self.current_char == ">":
+                token = Token(XmlTokenType.TAG_END, self.current_char, self.line, self.column)
+                self.content_matching = True
+                self.advance()
+                return token
+            if self.current_char == "?" and self.peek() == ">":
+                self.advance()
+                token = Token(XmlTokenType.PROLOG_END, "?>", self.line, self.column)
+                self.advance()
+                return token
+            
             if self.current_char.isdigit():
-                return self.get_number(accept_bit=True, accept_hex=True)
+                return self.get_number()
 
-            if self.current_char.isalnum() or self.current_char == "_":
-                return self.get_id(extend_chars=["_", "-", "."])
+            if self.current_char.isalpha() or self.current_char in ("_", ":"):
+                result = ""
+                # <Name> ::= (Letter | '_' | ':') (<NameChar>)*
+                # <NameChar> ::= <Letter> | <Digit> | '.' | '-' | '_' | ':'
+                while self.current_char is not None and (
+                    self.current_char.isalnum() or self.current_char in ("_", ":", ".", "-")
+                ):
+                    result += self.current_char
+                    self.advance()
+
+                return Token(XmlTokenType.NAME, result, self.line, self.column - 1)
 
             if self.current_char in ('"', "'"):
                 return self.get_str()
 
-            if self.current_char == "-":
-                return self.get_option()
-
-            if self.current_char == "#":
-                return self.get_comment()
-
-            if self.current_char in ("/", "."):
-                return self.get_path()
-
-            if self.current_char == "$" and self.peek() != '(':
-                return self.shell_variant()
-
-            if self.current_char in ("<", ">"):
-                
-                token = Token(
-                    ShellTokenType(self.current_char), self.current_char, self.line, self.column
-                )
-                self.advance()
-                return token
-
             try:
                 token_type = TokenType(self.current_char)
             except ValueError:  # pragma: no cover
                 token = Token(None, self.current_char, self.line, self.column)
                 self.error(ErrorCode.UNKNOWN_CHARACTER, token)
             else:
                 token = Token(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `syntaxlight-0.0.9/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.1.0/syntaxlight/lexers/toml_lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                         result += self.current_char
                         self.advance()
                     return Token(TomlTokenType.DATE, result, self.line, self.column - 1)
                 else:
                     return token
 
             if self.current_char.isalpha():
-                return self.get_id(extend_chars=["_"])
+                return self.get_id(extend_chars=["_",'-'])
 
             try:
                 token_type = TokenType(self.current_char)
             except ValueError:  # pragma: no cover
                 token = Token(None, self.current_char, self.line, self.column)
                 self.error(ErrorCode.UNKNOWN_CHARACTER, token)
             else:
```

### Comparing `syntaxlight-0.0.9/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.1.0/syntaxlight/lexers/shell_lexer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,127 @@
-from .lexer import Lexer, Token, TokenType, TokenSet, ErrorCode
+from .lexer import Lexer, Token, TokenType, ErrorCode
 from enum import Enum
+import re
 
-
-class XmlTokenType(Enum):
+class ShellTokenType(Enum):
     RESERVED_KEYWORD_START = "RESERVED_KEYWORD_START"
+    IF = "if"
+    ELIF = "elif"
+    ELSE = "else"
+    THEN = "then"
+    FI = "fi"
+    FOR = "for"
+    DO = "do"
+    IN = "in"
+    DONE = "done"
+    WHILE = "while"
+    BREAK = "break"
+    CD = 'cd'
+    EXPORT = 'export'
+
     RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
 
-    PROLOG_START = "<?xml"
-    PROLOG_END = "?>"
-    TAG_START_BEGIN = "<"
-    TAG_END = ">"
-    TAG_COMPLETE_BEGIN = '</'
-    TAG_SELF_END = "/>"
-    NAME = "NAME"
-    CONTENT = "CONTENT"
+    OPTION = "option"
+    PATH = "path"
+    VARIANT = "variant"
+    REDIRECT_TO = ">"
+    REDIRECT_FROM = "<"
+    LINUX_USER_PATH = 'root@kamilu'
+    HOST_NAME = 'HostName'
+    DIR_PATH = 'DirPath'
+    TAG = 'Tag'
 
 
-class XmlLexer(Lexer):
-    def __init__(self, text: str, LanguageTokenType: Enum = XmlTokenType):
+class ShellLexer(Lexer):
+    def __init__(self, text: str, LanguageTokenType: Enum = ShellTokenType):
         super().__init__(text, LanguageTokenType)
-        self.content_matching = False
+        self.build_long_op_dict(['&&','>>','<<'])
 
-    def get_next_token(self) -> Token:
+    def get_option(self):
+        """
+        长短选项
+        -s --options
+        """
+        result = ""
+        while self.current_char is not None:
+            if self.current_char.isalnum() or self.current_char in ("-", "_"):
+                result += self.current_char
+                self.advance()
+            else:
+                break
+
+        return Token(ShellTokenType.OPTION, result, self.line, self.column - 1)
+
+    def shell_variant(self):
+        """
+        $i
+        $mysh
+        """
+        result = "$"
+        self.advance()
         while self.current_char is not None:
-            if self.content_matching:
-                result = ""
-                while self.current_char is not None and self.current_char != "<":
-                    result += self.current_char
-                    self.advance()
-                self.content_matching = False
-                return Token(XmlTokenType.CONTENT, result, self.line, self.column - 1)
+            if self.current_char.isalnum() or self.current_char in ("-", "_"):
+                result += self.current_char
+                self.advance()
+            else:
+                break
+        return Token(ShellTokenType.VARIANT, result, self.line, self.column - 1)
 
+    def get_next_token(self) -> Token:
+        while self.current_char is not None:
             if self.current_char == TokenType.SPACE.value:
                 return self.skip_whitespace()
 
             if self.current_char in self.invisible_characters:
                 return self.skip_invisiable_character()
 
-            if self.current_char == "<":
-                if self.peek(4) == "?xml":
-                    result = "<?xml"
-                    self.advance()
-                    self.advance()
-                    self.advance()
-                    self.advance()
-                    token = Token(XmlTokenType.PROLOG_START, result, self.line, self.column)
-                    self.advance()
-                    return token
-                elif self.peek(3) == "!--":
-                    return self.get_comment("<!--", "-->")
-                elif self.peek() == "/":
-                    self.advance()
-                    token = Token(XmlTokenType.TAG_COMPLETE_BEGIN, "</", self.line, self.column)
-                    self.advance()
-                    return token
-                else:
-                    token = Token(
-                        XmlTokenType.TAG_START_BEGIN, self.current_char, self.line, self.column
-                    )
-                    self.advance()
-                    return token
-            if self.current_char == "/" and self.peek() == ">":
-                self.advance()
-                token = Token(XmlTokenType.TAG_SELF_END, "/>", self.line, self.column)
-                self.advance()
-                return token
-            if self.current_char == ">":
-                token = Token(XmlTokenType.TAG_END, self.current_char, self.line, self.column)
-                self.content_matching = True
-                self.advance()
-                return token
-            if self.current_char == "?" and self.peek() == ">":
-                self.advance()
-                token = Token(XmlTokenType.PROLOG_END, "?>", self.line, self.column)
-                self.advance()
-                return token
-            
             if self.current_char.isdigit():
-                return self.get_number()
+                return self.get_number(accept_bit=True, accept_hex=True)
+
+            if self.current_char.isalnum() or self.current_char in ('_','.','/'):
+                token = self.get_id(extend_chars=["_", "-", ".",'/',':','+','-','@','~'])
+                if bool(re.match(r'^\w+@[\w.-]+:[~\w/]+', token.value)):
+                    if self.current_char in ('#', '$'):
+                        token.value += self.current_char
+                        token.column += 1
+                        self.advance()
+                    token.type = ShellTokenType.LINUX_USER_PATH
+
+                return token
+
+            # 只接受双引号, 因为无法判断 can't ... 这种
+            if self.current_char == '"':
+                return self.get_string()
 
-            if self.current_char.isalpha() or self.current_char in ("_", ":"):
-                result = ""
-                # <Name> ::= (Letter | '_' | ':') (<NameChar>)*
-                # <NameChar> ::= <Letter> | <Digit> | '.' | '-' | '_' | ':'
-                while self.current_char is not None and (
-                    self.current_char.isalnum() or self.current_char in ("_", ":", ".", "-")
-                ):
-                    result += self.current_char
-                    self.advance()
+            if self.current_char == "-" and (self.peek().isalpha() or self.peek() == '-'):
+                return self.get_option()
 
-                return Token(XmlTokenType.NAME, result, self.line, self.column - 1)
+            if self.current_char == "#":
+                return self.get_comment()
 
-            if self.current_char in ('"', "'"):
-                return self.get_str()
+            if self.current_char == "$" and self.peek() != '(':
+                return self.shell_variant()
+
+            if self.current_char in ("<", ">") and self.peek() != self.current_char:
+                token = Token(
+                    ShellTokenType(self.current_char), self.current_char, self.line, self.column
+                )
+                self.advance()
+                return token
+
+            if self.current_char in self.long_op_dict:
+                return self.get_long_op()
 
             try:
                 token_type = TokenType(self.current_char)
             except ValueError:  # pragma: no cover
-                token = Token(None, self.current_char, self.line, self.column)
-                self.error(ErrorCode.UNKNOWN_CHARACTER, token)
+                # 考虑一些特殊的情况: test\shell\11.sh
+                token = Token(TokenType.TEXT, self.current_char, self.line, self.column)
+                self.advance()
+                return token
             else:
                 token = Token(
                     type=token_type,
                     value=token_type.value,  # e.g. ';', '.', etc
                     line=self.line,
                     column=self.column,
                 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `syntaxlight-0.0.9/syntaxlight/parsers/bnf_parser.py` & `syntaxlight-0.1.0/syntaxlight/parsers/bnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.9/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.1.0/syntaxlight/parsers/c_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     STRUCTURE_TYPE = "StructureType"
     QUALIFY_TYPE = "QualifyType"
     HEADER_NAME = "HeaderName"
     ALIGN_SPECIFIER = "AlignSpecifier"
     ATOMAIC_TYPE_SPECIFIER = "AtomicTypeSpecifier"
     STRUCTURE_CLASS = "StructureClass"
     GOTO_LABEL = "GotoLabel"
+    GNU_C_EXTENSION = "GNU-C-Extension"
 
 
 class TranslationUnit(AST):
     def __init__(self, declarations) -> None:
         super().__init__()
         self.declarations = declarations
 
@@ -646,14 +647,19 @@
         super().__init__()
         self.value: str = value
         self.is_leaf_ast = True
         value = self.value.replace("\\", "\\\\").replace('"', '\\"')
         self.node_info += f"\\n{value}"
 
 
+class GNU_C_Assembly(AST):
+    def __init__(self) -> None:
+        super().__init__()
+
+
 class CParser(Parser):
     def __init__(self, lexer, skip_invisible_characters=True, skip_space=True):
         super().__init__(lexer, skip_invisible_characters, skip_space)
         self.cfirst_set = CTokenSet()
         self.in_preprocessing = False  # 进入预处理阶段, 影响 after_eat
         self.preprocessing_keywords = [
             "ifdef",
@@ -837,15 +843,15 @@
         <struct-or-union-specifier> ::= <struct-or-union> <identifier> ("{" {<struct-declaration>}* "}")?
                                       | <struct-or-union>              "{" {<struct-declaration>}* "}"
         """
         if self.current_token.type not in self.cfirst_set.struct_or_union_specifier:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be struct or union")
 
         node = Structure()
-        
+
         node.update(structure_type=self.struct_or_union())
 
         # 对于如下情况
         # typedef struct State State;
         # struct State {
         #     int c;
         #     State *out;
@@ -1390,14 +1396,24 @@
             node.register_token(self.eat(TokenType.RPAREN))
             node.register_token(self.eat(TokenType.LCURLY_BRACE))
             node.update(initializer_list=self.initializer_list())
             if self.current_token.type == TokenType.COMMA:
                 node.register_token(self.eat())
             node.register_token(self.eat(TokenType.RCURLY_BRACE))
 
+        # 检查是不是宏定义
+        if node.primary_expr is not None:
+            if isinstance(node.primary_expr.sub_node, Identifier):
+                if node.primary_expr.sub_node.id in GDT or bool(
+                    re.match(r"^[A-Z_][0-9A-Z_]+$", node.primary_expr.sub_node.id)
+                ):
+                    if self.current_token.type == TokenType.LPAREN:
+                        # 宏函数匹配
+                        self._match_macro_function(node.primary_expr.sub_node.id)
+
         sub_nodes = []
         while self.current_token.type in self.cfirst_set.postfix_expression_inside:
             if self.current_token.type == TokenType.LSQUAR_PAREN:
                 node.register_token(self.eat(TokenType.LSQUAR_PAREN))
                 sub_nodes.append(self.expression())
                 node.register_token(self.eat(TokenType.RSQUAR_PAREN))
             elif self.current_token.type == TokenType.LPAREN:
@@ -1442,22 +1458,30 @@
                                | <char>
                                | "(" <expression> ")"
                                | <generic-selection>
         """
         node = PrimaryExpression()
         if self.current_token.type == TokenType.ID:
             sub_node = self.identifier()
+            # 多个 STRING 可以拼接在一起
+            # printk(KERN_INFO "%s\n")
+            while self.current_token.type == TokenType.STRING:
+                self.string_inside_format()
         elif self.current_token.type in self.cfirst_set.constant:
             # @扩展文法
             # Constant 包含了 true, false
             # 该关键字由 C23 引入, 但非常常用, 一般会 define 为 1 和 0, 所以这里引入为 Constant
             sub_node = Constant(self.current_token.value)
             sub_node.register_token(self.eat(self.current_token.type))
         elif self.current_token.type == TokenType.STRING:
             sub_node = self.string()
+            # 多个 STRING 可以拼接在一起
+            # printk(KERN_INFO "%s\n")
+            while self.current_token.type == TokenType.STRING:
+                self.string_inside_format()
         elif self.current_token.type == TokenType.CHARACTER:
             sub_node = Char(self.current_token.value)
             sub_node.register_token(self.eat(self.current_token.type))
         elif self.current_token.type == TokenType.LPAREN:
             node.register_token(self.eat(TokenType.LPAREN))
             sub_node = self.expression()
             node.register_token(self.eat(TokenType.RPAREN))
@@ -1503,14 +1527,47 @@
             node.update(type_name=self.type_name())
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be default or type-name")
         node.register_token(self.eat(TokenType.COLON))
         node.update(assignment_expr=self.assignment_expression())
         return node
 
+    def _match_macro_function(self, macro_name:str):
+        """
+        匹配不符合 C 文法的宏定义函数
+
+        1. 对于全大写 ID 的会被认为是宏函数
+
+           XBOX_ARG_BOOLEAN(NULL, [-h][--help][help = "show help information"])
+
+        2. 对于前面定义过的宏函数会被匹配
+
+           #define container_of()
+
+           struct ipc_namespace *ns = container_of(table->data, struct ipc_namespace, shm_rmid_forced);
+        """
+        
+        assert self.current_token.type == TokenType.LPAREN
+        self.eat(TokenType.LPAREN)
+        brace_number = 1
+
+        while self.current_token.type != TokenType.EOF:
+            if self.current_token.type == TokenType.RPAREN:
+                brace_number -= 1
+                if brace_number == 0:
+                    self.eat()
+                    return
+            elif self.current_token.type == TokenType.LPAREN:
+                brace_number += 1
+            self.pp_token()
+
+        self.error(ErrorCode.BRACE_MISS_MATCH, f'in macro define function {macro_name}')
+
+
+
     def expression(self):
         """
         <expression> ::= <assignment-expression> ("," <assignment-expression>)*
         """
         node = Expression()
         exprs = [self.assignment_expression()]
         while self.current_token.type == TokenType.COMMA:
@@ -1729,18 +1786,18 @@
 
         <function-definition> ::= <declaration-specifier>* <declarator> <declaration>* <compound-statement>
         """
         node = Declaration()
         if self.current_token.type in self.cfirst_set.static_assert_declaration:
             node.update(static_assert=self.static_assert_declaration())
             return node
-        
+
         declaration_specifiers: List[AST] = [self.declaration_sepcifier()]
         self._unknown_typedef_id_guess()
-        
+
         while self.current_token.type in self.cfirst_set.declaration_specifier:
             declaration_specifiers.append(self.declaration_sepcifier())
             self._unknown_typedef_id_guess()
 
         if self.current_token.type in self.cfirst_set.init_declarator_list:
             init_declarator_list = self.init_declarator_list()
             if self.current_token.type == TokenType.SEMI:
@@ -1948,14 +2005,15 @@
         """
         <statement> ::= <labeled-statement>
                       | <expression-statement>
                       | <compound-statement>
                       | <selection-statement>
                       | <iteration-statement>
                       | <jump-statement>
+                      | <gnu-c-statement-extension>
         """
         if (
             self.current_token.type == TokenType.ID
             and self.peek_next_token().type == TokenType.COLON
         ):
             # goto id;
             # id: ...
@@ -1971,14 +2029,16 @@
             return self.compound_statement()
         elif self.current_token.type in self.cfirst_set.selection_statement:
             return self.selection_statement()
         elif self.current_token.type in self.cfirst_set.iteration_statement:
             return self.iteration_statement()
         elif self.current_token.type in self.cfirst_set.jump_statement:
             return self.jump_statement()
+        elif self.current_token.type in self.cfirst_set.gnu_c_statement_extension:
+            return self.gnu_c_statement_extension()
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be a statement")
 
     def labeled_statement(self):
         """
         <labeled-statement> ::= <identifier> ":" <statement>
                               | case <constant-expression> ":" <statement>
@@ -2106,14 +2166,54 @@
             else:
                 node.update(keyword=self.get_keyword())
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be goto continue break return")
         node.register_token(self.eat(TokenType.SEMI))
         return node
 
+    def gnu_c_statement_extension(self):
+        """
+        https://gcc.gnu.org/onlinedocs/gcc/Extended-Asm.html
+
+        <gnu-c-statement-extension> ::= __asm__ <asm-qualifiers> "(" <STRING>+ <OutputOperands >* ")"
+
+        <asm-qualifiers> ::= volatile
+                           | inline
+                           | goto
+
+        <OutputOperands> ::= ":" <STRING>? ( "(" <constant_expression> ")" ) ("," <STRING>? ( "(" <constant_expression> ")" ))*
+        """
+        node = GNU_C_Assembly()
+        node.update(keyword=self.get_keyword(CTokenType._ASM, css_type=C_CSS.GNU_C_EXTENSION))
+        if self.current_token.type in (CTokenType.VOLATILE, CTokenType.INLINE, CTokenType.GOTO):
+            node.update(asm_qualifier=self.get_keyword(css_type=C_CSS.GNU_C_EXTENSION))
+        node.register_token(self.eat(TokenType.LPAREN))
+
+        while self.current_token.type == TokenType.STRING:
+            self.string_inside_format()
+
+        while self.current_token.type == TokenType.COLON:
+            node.register_token(self.eat(TokenType.COLON))
+            if self.current_token.type == TokenType.STRING:
+                node.register_token(self.eat(TokenType.STRING))
+            if self.current_token.type == TokenType.LPAREN:
+                node.register_token(self.eat(TokenType.LPAREN))
+                self.constant_expression()
+                node.register_token(self.eat(TokenType.RPAREN))
+                while self.current_token.type == TokenType.COMMA:
+                    node.register_token(self.eat())
+                    if self.current_token.type == TokenType.STRING:
+                        node.register_token(self.eat(TokenType.STRING))
+                    if self.current_token.type == TokenType.LPAREN:
+                        node.register_token(self.eat(TokenType.LPAREN))
+                        self.constant_expression()
+                        node.register_token(self.eat(TokenType.RPAREN))
+
+        node.register_token(self.eat(TokenType.RPAREN))
+
     def identifier(self):
         """
         <ID>
         """
         node = Identifier(self.current_token.value)
         token_value = self.current_token.value
         node.register_token(self.eat(TokenType.ID))
@@ -2375,14 +2475,18 @@
         elif self.current_token.type == TokenType.RANGLE_BRACE:
             self.current_token.type = TokenType.GT
 
         if self.current_token.type == TokenType.ID:
             return self.identifier()
         elif self.current_token.type == TokenType.STRING:
             return self.string()
+        elif self.current_token.value in self.lexer.reserved_keywords:
+            return self.get_keyword()
+        elif self.current_token.type in self.cfirst_set.struct_or_union:
+            return self.struct_or_union()
         else:
             node = PPtoken(self.current_token.value)
             node.register_token(self.eat())
             return node
 
     def header_name(self):
         """
```

### Comparing `syntaxlight-0.0.9/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.1.0/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.9/syntaxlight/parsers/lua_parser.py` & `syntaxlight-0.1.0/syntaxlight/parsers/lua_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.9/syntaxlight/parsers/parser.py` & `syntaxlight-0.1.0/syntaxlight/parsers/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,33 @@
 from ..lexers.lexer import Lexer, Token, TokenType, TTYColor
 from ..error import ParserError, ErrorCode
 from enum import Enum
-from ..ast import AST, Keyword, add_ast_type, Identifier, Punctuator, String
+from ..ast import AST, Keyword, add_ast_type, Identifier, Punctuator, WrapString, Number, String
 from typing import List
 import sys
 import html
 import traceback
 import re
 from ..gdt import CSS
 
 
 DEBUG = False
-DEBUG = True
+# DEBUG = True
 
 
 class Parser:
     def __init__(
         self, lexer, skip_invisible_characters=True, skip_space=True, display_warning=True
     ):
         self.lexer: Lexer = lexer
         # set current token to the first token taken from the input
         self.skip_invisible_characters = skip_invisible_characters
         self.skip_space = skip_space
         self.display_warning = display_warning
         self._token_list: List[Token] = []  # lexer 解析后经过 parser 确定类型后的 tokens
-        self.brace_list: List[TokenType] = [
-            TokenType.LPAREN,
-            TokenType.RPAREN,
-            TokenType.LSQUAR_PAREN,
-            TokenType.RSQUAR_PAREN,
-            TokenType.LCURLY_BRACE,
-            TokenType.RCURLY_BRACE,
-            TokenType.LANGLE_BRACE,
-            TokenType.RANGLE_BRACE,
-        ]
-        self.brace_max_depth = 3  # 深度循环轮次
         self.root: AST = None  # 主根节点
         self.sub_roots: List[AST] = []  # 其他根节点, 例如预处理命令
         self._status_stack = []  # 状态栈
         self.current_token: Token = self.lexer.get_next_token()
         self._skip()
 
     def error(
@@ -214,25 +203,26 @@
         if self.current_token.type == TokenType.CR:
             self.eat(self.current_token.type)
         if self.current_token.type == TokenType.EOF:
             return
         self.eat(TokenType.LF)
         self.skip_crlf()
 
-    def peek_next_token(self) -> Token:
+    def peek_next_token(self, n = 1) -> Token:
         """
         查看下一个 token 的类型
         """
         # 保存程序状态
         self.lexer._record()
         token_list_length = len(self._token_list)
         sub_roots_length = len(self.sub_roots)
         current_token = self.current_token
 
-        self.eat()
+        for _ in range(n):
+            self.eat()
         next_token = self.current_token
 
         self.lexer._reset()
         self._token_list = self._token_list[:token_list_length]
         self.sub_roots = self.sub_roots[:sub_roots_length]
         self.current_token = current_token
         return next_token
@@ -249,40 +239,58 @@
         self._token_list.append(token)
 
     def to_html(self):
         """
         将一个解析完成的 AST node 输出其 token 流的 HTML 格式
         """
         html_str = ""
-        # 对于 ([{<>}]) 计算括号深度
+        self.brace_matching()
+        for token in self._token_list:
+            html_str += f'<span class="{token.get_css_class()}">{html.escape(token.value)}</span>'
+        return html_str
+
+    def brace_matching(self):
+        '''
+        对于 ([{<>}]) 计算括号深度
+        '''
+        brace_max_depth = 3  # 括号深度循环轮次
+        brace_list: List[TokenType] = [
+            TokenType.LPAREN,
+            TokenType.RPAREN,
+            TokenType.LSQUAR_PAREN,
+            TokenType.RSQUAR_PAREN,
+            TokenType.LCURLY_BRACE,
+            TokenType.RCURLY_BRACE,
+            TokenType.LANGLE_BRACE,
+            TokenType.RANGLE_BRACE,
+        ]
+
         brace_depth = 0
         brace_stack: List[TokenType] = []
         for token in self._token_list:
-            # print(self.brace_list)
-            if token.type in self.brace_list:
+            # print(brace_list)
+            if token.type in brace_list:
                 if len(brace_stack) == 0:
                     brace_stack.append(token.type)
-                    token.class_list.add(f"brace-depth-{brace_depth%self.brace_max_depth}")
+                    token.class_list.add(f"BraceDepth-{brace_depth%brace_max_depth}")
                     brace_depth += 1
                 else:
                     # 括号匹配
-                    if self.brace_list.index(brace_stack[-1]) + 1 == self.brace_list.index(
+                    if brace_list.index(brace_stack[-1]) + 1 == brace_list.index(
                         token.type
                     ):
                         brace_stack.pop()
                         brace_depth -= 1
-                        token.class_list.add(f"brace-depth-{brace_depth%self.brace_max_depth}")
+                        token.class_list.add(f"BraceDepth-{brace_depth%brace_max_depth}")
                     else:
                         # 加入 brace_stack
                         brace_stack.append(token.type)
-                        token.class_list.add(f"brace-depth-{brace_depth%self.brace_max_depth}")
+                        token.class_list.add(f"BraceDepth-{brace_depth%brace_max_depth}")
                         brace_depth += 1
 
-            html_str += f'<span class="{token.get_css_class()}">{html.escape(token.value)}</span>'
-        return html_str
 
     def parse(self):
         raise NotImplementedError(self.__class__.__name__ + " must override the parse function")
 
     def get_keyword(self, token_type: Enum = None, css_type: Enum = None) -> Keyword:
         """
         keyword
@@ -314,34 +322,51 @@
         node = Punctuator(self.current_token.value)
         if token_type is None:
             node.register_token(self.eat())
         else:
             node.register_token(self.eat(token_type))
         return node
 
-    def string_inside_format(self, token: Token) -> List[String]:
+    def string(self):
+        node = WrapString()
+        node.update(strings = self.string_inside_format())
+        return node
+
+    def string_inside_format(self, token: Token = None) -> List[String]:
         """
         取出其中格式化字符(如 %d %x \n) 并新建 token
         """
-        pattern = r"(%[0-9ldiufFeEgGxXoscpaAnYyMmHhSs]+|(?:\\\\|\\n|\\t|\\v|\\f))"
+        if token is None:
+            token = self.current_token
+        pattern = r"(%[#0-9ldiufFeEgGxXoscpaAnYyMmHhSsLl]+|(?:\\\\|\\n|\\t|\\v|\\f))"
         sub_strings = re.split(pattern, token.value)
         new_asts = []
         line = token.line
         column = token.column - len(token.value)
         token_type = token.type
         for sub_string in sub_strings:
             if len(sub_string) == 0:
                 continue
             column += len(sub_string)
             token = Token(token_type, sub_string, line, column)
-            if bool(re.match(r"%[0-9ldiufFeEgGxXoscpaAnYyMmHhSs]+", sub_string)):
+            if bool(re.match(r"%[#0-9ldiufFeEgGxXoscpaAnYyMmHhSsLl]+", sub_string)):
                 token.add_css(CSS.FORMAT)
             elif sub_string in ["\\n", "\\t", "\\f", "\\v", "\\a", "\\b", "\\\\"]:
                 token.add_css(CSS.CONTROL)
 
             self.manual_register_token(token)
             node = String(token.value)
             node.register_token([token])
             new_asts.append(node)
 
         self.manual_get_next_token()
         return new_asts
+
+    def punctuator(self):
+        node = Punctuator(self.current_token.value)
+        node.register_token(self.eat())
+        return node
+
+    def number(self):
+        node = Number(self.current_token.value)
+        node.register_token(self.eat())
+        return node
```

### Comparing `syntaxlight-0.0.9/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.1.0/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.9/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.1.0/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.9/syntaxlight/syntax_parse.py` & `syntaxlight-0.1.0/syntaxlight/syntax_parse.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 def parse(
     text: str, language=None, file_path=None, show_error_context=True, save_ast_tree=False
 ) -> str:
     if len(text) == 0:
         return ""
     language = clean_language(language)
-    parser = get_parser(text, language)
-    parser.lexer.file_path = file_path
-
+    
     try:
+        parser = get_parser(text, language)
+        parser.lexer.file_path = file_path
         parser.parse()
     except Error as e:
         sys.stderr.write(e.message)
         if show_error_context:
             sys.stderr.write(e.context)
     else:
         display_ast(parser.root, parser.sub_roots, save_ast_tree=save_ast_tree)
@@ -58,39 +58,23 @@
             tokens.append(token)
         except Error as e:
             print(e.message)
             print(e.context)
     return tokens
 
 
-def get_lexer(code_or_path: str, language: str = None) -> Lexer:
+def get_lexer(text: str, language: str = None) -> Lexer:
     """
     @code_or_path: 代码或者文件的路径
     @lanaguge: 选择的语言, 如果第一个参数为文件路径则不需要传入 language
     """
-    code, language = _preprocess(code_or_path, language)
     if language not in SUPPORTED_SYNTAX:
         print("lexer not support")
         show_help_info()
         exit(1)
-    return SUPPORTED_SYNTAX[language]["lexer"](code)
+    return SUPPORTED_SYNTAX[language]["lexer"](text)
 
 
-def get_parser(code_or_path: str, language: str = None) -> Parser:
-    code, language = _preprocess(code_or_path, language)
-    lexer = get_lexer(code, language)
+def get_parser(text: str, language: str = None) -> Parser:
+    lexer = get_lexer(text, language)
     parser = SUPPORTED_SYNTAX[language]["parser"](lexer)
     return parser
-
-
-def _preprocess(code_or_path: str, language: str = None):
-    if os.path.exists(code_or_path):
-        with open(code_or_path, "r", encoding="utf-8") as f:
-            code = f.read()
-
-        if language is None:
-            language = guess_language(code_or_path)
-    else:
-        code = code_or_path
-
-    language = clean_language(language)
-    return code, language
```

### Comparing `syntaxlight-0.0.9/PKG-INFO` & `syntaxlight-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.0.9
+Version: 0.1.0
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Documentation, https://luzhixing12345.github.io/syntaxlight/
 Project-URL: Repository, https://github.com/luzhixing12345/syntaxlight
 Description-Content-Type: text/markdown
 
 # syntaxlight
 
 > 本项目仍在开发中, 尚不可用...
 
-syntaxlight 是一个基于 BNF 的语法高亮的 python 库, 您可以 [在线浏览]() 文法高亮结果
+syntaxlight 是一个基于 BNF 的语法高亮的 python 库, 您可以 [在线浏览](https://luzhixing12345.github.io/syntaxlight/articles/全部文法高亮/C/) 文法高亮结果
 
 目前支持 C/Python 等主流编程语言和 json xml 等主流标记语言的文法解析, 支持多种高亮主题以及自定义颜色(默认使用 Vscode 风格), 您可在此查看[全部文法支持和高亮支持](https://luzhixing12345.github.io/syntaxlight/articles/%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C/%E5%85%A8%E9%83%A8%E6%96%87%E6%B3%95%E6%94%AF%E6%8C%81/)
 
 ## 安装
 
 ```bash
 pip install syntaxlight
```

