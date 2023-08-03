# Comparing `tmp/cmdcomp-2.0.6.tar.gz` & `tmp/cmdcomp-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-2.0.6.tar", max compression
+gzip compressed data, was "cmdcomp-2.1.0.tar", max compression
```

## Comparing `cmdcomp-2.0.6.tar` & `cmdcomp-2.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2425 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/README.md
--rw-r--r--   0        0        0       79 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2289 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/app.py
--rw-r--r--   0        0        0      573 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/completion.py
--rw-r--r--   0        0        0      734 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/config.py
--rw-r--r--   0        0        0      444 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/exception.py
--rw-r--r--   0        0        0      115 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/main.py
--rw-r--r--   0        0        0      115 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/model.py
--rw-r--r--   0        0        0      131 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/shell.py
--rw-r--r--   0        0        0        0 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/__init__.py
--rw-r--r--   0        0        0      535 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/app_info.py
--rw-r--r--   0        0        0      261 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/cmdcomp_info.py
--rw-r--r--   0        0        0     3358 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/command/__init__.py
--rw-r--r--   0        0        0      338 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/command/option/__init__.py
--rw-r--r--   0        0        0      331 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/command/option/command_option.py
--rw-r--r--   0        0        0      373 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/command/option/file_option.py
--rw-r--r--   0        0        0     2164 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/completion.py
--rw-r--r--   0        0        0      377 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/config.py
--rw-r--r--   0        0        0     1888 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v1/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1469 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v1/templates/zsh.sh.jinja
--rw-r--r--   0        0        0        0 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/__init__.py
--rw-r--r--   0        0        0      535 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/app_info.py
--rw-r--r--   0        0        0      261 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/cmdcomp_info.py
--rw-r--r--   0        0        0     6844 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/__init__.py
--rw-r--r--   0        0        0      371 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/argument/__init__.py
--rw-r--r--   0        0        0      789 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/argument/command_argument.py
--rw-r--r--   0        0        0      744 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/argument/file_argument.py
--rw-r--r--   0        0        0      601 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/argument/flag_argument.py
--rw-r--r--   0        0        0     1668 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/argument/values_argument.py
--rw-r--r--   0        0        0      888 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/completion.py
--rw-r--r--   0        0        0      380 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/config.py
--rw-r--r--   0        0        0     4338 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/templates/bash.sh.jinja
--rw-r--r--   0        0        0     2949 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1696 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 cmdcomp-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2425 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/README.md
+-rw-r--r--   0        0        0       79 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2289 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/app.py
+-rw-r--r--   0        0        0      573 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/completion.py
+-rw-r--r--   0        0        0      734 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/config.py
+-rw-r--r--   0        0        0      444 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/exception.py
+-rw-r--r--   0        0        0      115 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/main.py
+-rw-r--r--   0        0        0      115 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/model.py
+-rw-r--r--   0        0        0      131 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/shell.py
+-rw-r--r--   0        0        0        0 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/v1/__init__.py
+-rw-r--r--   0        0        0      535 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/v1/app_info.py
+-rw-r--r--   0        0        0      261 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/v1/cmdcomp_info.py
+-rw-r--r--   0        0        0     3358 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/v1/command/__init__.py
+-rw-r--r--   0        0        0      338 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/v1/command/option/__init__.py
+-rw-r--r--   0        0        0      331 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/v1/command/option/command_option.py
+-rw-r--r--   0        0        0      373 2023-08-03 15:19:45.691405 cmdcomp-2.1.0/cmdcomp/v1/command/option/file_option.py
+-rw-r--r--   0        0        0     2164 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v1/completion.py
+-rw-r--r--   0        0        0      377 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v1/config.py
+-rw-r--r--   0        0        0     1888 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v1/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1469 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v1/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0        0 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/__init__.py
+-rw-r--r--   0        0        0      535 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/app_info.py
+-rw-r--r--   0        0        0      261 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/cmdcomp_info.py
+-rw-r--r--   0        0        0     6821 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/command/__init__.py
+-rw-r--r--   0        0        0      371 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/command/argument/__init__.py
+-rw-r--r--   0        0        0      789 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/command/argument/command_argument.py
+-rw-r--r--   0        0        0      744 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/command/argument/file_argument.py
+-rw-r--r--   0        0        0      601 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/command/argument/flag_argument.py
+-rw-r--r--   0        0        0     1668 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/command/argument/values_argument.py
+-rw-r--r--   0        0        0      888 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/completion.py
+-rw-r--r--   0        0        0      380 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/config.py
+-rw-r--r--   0        0        0     4338 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     2949 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/cmdcomp/v2/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1696 2023-08-03 15:19:45.695405 cmdcomp-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 cmdcomp-2.1.0/PKG-INFO
```

### Comparing `cmdcomp-2.0.6/README.md` & `cmdcomp-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/app.py` & `cmdcomp-2.1.0/cmdcomp/app.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/completion.py` & `cmdcomp-2.1.0/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/config.py` & `cmdcomp-2.1.0/cmdcomp/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v1/app_info.py` & `cmdcomp-2.1.0/cmdcomp/v1/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v1/command/__init__.py` & `cmdcomp-2.1.0/cmdcomp/v1/command/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v1/completion.py` & `cmdcomp-2.1.0/cmdcomp/v1/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v1/templates/bash.sh.jinja` & `cmdcomp-2.1.0/cmdcomp/v1/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v1/templates/zsh.sh.jinja` & `cmdcomp-2.1.0/cmdcomp/v1/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v2/app_info.py` & `cmdcomp-2.1.0/cmdcomp/v2/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v2/command/__init__.py` & `cmdcomp-2.1.0/cmdcomp/v2/command/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Annotated, Literal, OrderedDict, TypeAlias
 
 from pydantic import ConfigDict, Field
 
 from cmdcomp.model import Model
-from cmdcomp.v2.command.argument.command_argument import V2CommandArgument
-from cmdcomp.v2.command.argument.file_argument import V2FileArgument
 from cmdcomp.v2.command.argument.flag_argument import V2FlagArgument
 from cmdcomp.v2.command.argument.values_argument import (
     V2ValueArgument,
     V2ValuesArgument,
 )
 
 from .argument import V2Argument
@@ -33,29 +31,23 @@
         title="description of the command.",
         default=None,
     )
 
     arguments: Annotated[
         OrderedDict[
             Position | Literal["*"] | Keyword,
-            str
-            | list[str]
-            | V2ValuesArgument
-            | V2FileArgument
-            | V2CommandArgument
-            | V2FlagArgument
-            | None,
+            str | list[str] | V2Argument | None,
         ],
         Field(
             title="arguments of the command.",
             description=(
                 "argment key allow "
-                "positional integer (like `1` , `2`), "
-                'keyword string(like `"--f"`, `"-f"`), '
-                'wildcard string(`"*"`).'
+                "positional integer (like 1, 2), "
+                'keyword string (like "--f", "-f"), '
+                'wildcard string ("*").'
             ),
         ),
     ]
 
     @property
     def aliases(self) -> list[str]:
         if isinstance(self.alias, str):
@@ -134,31 +126,26 @@
             default_factory=list,
         ),
     ]
 
     arguments: Annotated[
         OrderedDict[
             Keyword,
-            str
-            | list[str]
-            | V2ValuesArgument
-            | V2FileArgument
-            | V2CommandArgument
-            | V2FlagArgument
-            | None,
+            str | list[str] | V2Argument | None,
         ],
         Field(
             title="arguments of the command.",
             description='argment key allow keyword string (like "--f", "-f") only.',
             default_factory=OrderedDict,
         ),
     ]
 
-    subcommands: OrderedDict[SubcommandName, "V2Command"] = Field(
+    raw_subcommands: OrderedDict[SubcommandName, "V2Command | None"] = Field(
         title="subcommands of the command.",
+        alias="subcommands",
         default_factory=OrderedDict,
     )
 
     @property
     def aliases(self) -> list[str]:
         if isinstance(self.alias, str):
             return [self.alias]
@@ -180,14 +167,28 @@
                 (k, _convert_argument(v))
                 for k, v in self.arguments.items()
                 if isinstance(k, str)
             ]
         )
 
     @property
+    def subcommands(self) -> OrderedDict[SubcommandName, "V2Command"]:
+        return OrderedDict(
+            [
+                (
+                    name,
+                    V2SubcommandsCommand(alias=[], arguments=OrderedDict())
+                    if subcommand is None
+                    else subcommand,
+                )
+                for name, subcommand in self.raw_subcommands.items()
+            ]
+        )
+
+    @property
     def subcommand_names_with_alias(self) -> list[SubcommandName]:
         return _subcommand_names_with_alias(self)
 
     @property
     def keyword_names_with_alias(self) -> list[Keyword]:
         return _keyword_names_with_alias(self)
 
@@ -208,21 +209,15 @@
         return len(self.keyword_arguments) != 0
 
 
 V2Command = V2PoristionalArgumentsCommand | V2SubcommandsCommand
 
 
 def _convert_argument(
-    value: str
-    | list[str]
-    | V2ValuesArgument
-    | V2FileArgument
-    | V2CommandArgument
-    | V2FlagArgument
-    | None,
+    value: str | list[str] | V2Argument | None,
 ) -> V2Argument:
     match value:
         case str():
             return V2ValuesArgument(type="values", values=[value])
 
         case list():
             return V2ValuesArgument(
```

### Comparing `cmdcomp-2.0.6/cmdcomp/v2/command/argument/command_argument.py` & `cmdcomp-2.1.0/cmdcomp/v2/command/argument/command_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v2/command/argument/file_argument.py` & `cmdcomp-2.1.0/cmdcomp/v2/command/argument/file_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v2/command/argument/flag_argument.py` & `cmdcomp-2.1.0/cmdcomp/v2/command/argument/flag_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v2/command/argument/values_argument.py` & `cmdcomp-2.1.0/cmdcomp/v2/command/argument/values_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v2/completion.py` & `cmdcomp-2.1.0/cmdcomp/v2/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v2/templates/bash.sh.jinja` & `cmdcomp-2.1.0/cmdcomp/v2/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/cmdcomp/v2/templates/zsh.sh.jinja` & `cmdcomp-2.1.0/cmdcomp/v2/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.6/pyproject.toml` & `cmdcomp-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "2.0.6"
+version = "2.1.0"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `cmdcomp-2.0.6/PKG-INFO` & `cmdcomp-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 2.0.6
+Version: 2.1.0
 Summary: cmdcomp is a cli tool completion generator for shell.
 Home-page: https://github.com/yassun4dev/cmdcomp
 License: BSD-3-Clause
 Author: Yasutanium
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmdcomp Version: 2.0.6 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 2.1.0 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
```

