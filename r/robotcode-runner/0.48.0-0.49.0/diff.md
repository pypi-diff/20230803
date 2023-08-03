# Comparing `tmp/robotcode_runner-0.48.0.tar.gz` & `tmp/robotcode_runner-0.49.0.tar.gz`

## Comparing `robotcode_runner-0.48.0.tar` & `robotcode_runner-0.49.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    24078 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    25481 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/PKG-INFO
```

### Comparing `robotcode_runner-0.48.0/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.49.0/src/robotcode/runner/cli/libdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.48.0/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.49.0/src/robotcode/runner/cli/rebot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.48.0/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.49.0/src/robotcode/runner/cli/robot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.48.0/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.49.0/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.48.0/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.49.0/src/robotcode/runner/cli/discover/discover.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,24 @@
 from robot.conf import RobotSettings
 from robot.errors import DATA_ERROR, INFO_PRINTED, DataError, Information
 from robot.model import ModelModifier, TestCase, TestSuite
 from robot.model.visitor import SuiteVisitor
 from robot.output import LOGGER, Message
 from robot.running.builder import TestSuiteBuilder
 from robot.running.builder.builders import SuiteStructureParser
+from robot.utils import NormalizedDict
 from robot.utils.filereader import FileReader
 from robotcode.core.dataclasses import from_json
-from robotcode.core.lsp.types import Diagnostic, DiagnosticSeverity, DocumentUri, Position, Range
+from robotcode.core.lsp.types import (
+    Diagnostic,
+    DiagnosticSeverity,
+    DocumentUri,
+    Position,
+    Range,
+)
 from robotcode.core.uri import Uri
 from robotcode.plugin import Application, OutputFormat, UnknownError, pass_application
 from robotcode.plugin.click_helper.types import add_options
 from robotcode.robot.utils import get_robot_version
 
 from ..robot import ROBOT_OPTIONS, RobotFrameworkEx, handle_robot_options
 
@@ -43,17 +50,21 @@
     global __patched
     if __patched:
         return
     __patched = True
 
     if get_robot_version() <= (6, 1):
         if get_robot_version() > (5, 0) and get_robot_version() < (6, 0) or get_robot_version() < (5, 0):
-            from robot.running.builder.testsettings import TestDefaults  # pyright: ignore[reportMissingImports]
+            from robot.running.builder.testsettings import (
+                TestDefaults,
+            )
         else:
-            from robot.running.builder.settings import Defaults as TestDefaults  # pyright: ignore[reportMissingImports]
+            from robot.running.builder.settings import (
+                Defaults as TestDefaults,
+            )
 
         old_validate_test_counts = TestSuiteBuilder._validate_test_counts
 
         def _validate_test_counts(self: Any, suite: TestSuite, multisource: bool = False) -> None:
             # we don't need this
             try:
                 old_validate_test_counts(self, suite, multisource)
@@ -70,19 +81,23 @@
             except DataError as e:
                 LOGGER.error(str(e))
                 parent_defaults = self._stack[-1][-1] if self._stack else None
                 if get_robot_version() < (6, 1):
                     from robot.running.builder.parsers import format_name
 
                     return ErroneousTestSuite(
-                        error_message=str(e), name=format_name(structure.source), source=structure.source
+                        error_message=str(e),
+                        name=format_name(structure.source),
+                        source=structure.source,
                     ), TestDefaults(parent_defaults)
 
                 return ErroneousTestSuite(
-                    error_message=str(e), name=TestSuite.name_from_source(structure.source), source=structure.source
+                    error_message=str(e),
+                    name=TestSuite.name_from_source(structure.source),
+                    source=structure.source,
                 ), TestDefaults(parent_defaults)
 
         SuiteStructureParser._build_suite = build_suite
 
         old_validate_execution_mode = SuiteStructureParser._validate_execution_mode
 
         def _validate_execution_mode(self: SuiteStructureParser, suite: TestSuite) -> None:
@@ -91,15 +106,17 @@
             except DataError as e:
                 LOGGER.error(f"Parsing '{suite.source}' failed: {e.message}")
 
         SuiteStructureParser._validate_execution_mode = _validate_execution_mode
 
     elif get_robot_version() >= (6, 1):
         from robot.parsing.suitestructure import SuiteDirectory, SuiteFile
-        from robot.running.builder.settings import TestDefaults  # pyright: ignore[reportMissingImports]
+        from robot.running.builder.settings import (
+            TestDefaults,
+        )
 
         old_validate_not_empty = TestSuiteBuilder._validate_not_empty
 
         def _validate_not_empty(self: Any, suite: TestSuite, multi_source: bool = False) -> None:
             try:
                 old_validate_not_empty(self, suite, multi_source)
             except DataError as e:
@@ -111,30 +128,34 @@
 
         def build_suite_file(self: SuiteStructureParser, structure: SuiteFile) -> TestSuite:
             try:
                 return old_build_suite_file(self, structure)
             except DataError as e:
                 LOGGER.error(str(e))
                 return ErroneousTestSuite(
-                    error_message=str(e), name=TestSuite.name_from_source(structure.source), source=structure.source
+                    error_message=str(e),
+                    name=TestSuite.name_from_source(structure.source),
+                    source=structure.source,
                 )
 
         SuiteStructureParser._build_suite_file = build_suite_file
 
         old_build_suite_directory = SuiteStructureParser._build_suite_directory
 
         def build_suite_directory(
             self: SuiteStructureParser, structure: SuiteDirectory
         ) -> Tuple[TestSuite, TestDefaults]:
             try:
                 return old_build_suite_directory(self, structure)  # type: ignore
             except DataError as e:
                 LOGGER.error(str(e))
                 return ErroneousTestSuite(
-                    error_message=str(e), name=TestSuite.name_from_source(structure.source), source=structure.source
+                    error_message=str(e),
+                    name=TestSuite.name_from_source(structure.source),
+                    source=structure.source,
                 ), TestDefaults(self.parent_defaults)
 
         SuiteStructureParser._build_suite_directory = build_suite_directory
 
         if get_robot_version() < (6, 1, 1):
             old_validate_execution_mode = SuiteStructureParser._validate_execution_mode
 
@@ -210,16 +231,30 @@
             needs_parse_include=get_robot_version() >= (6, 1),
         )
         self._current = self.all
         self.suites: List[TestItem] = []
         self.tests: List[TestItem] = []
         self.tags: Dict[str, List[TestItem]] = defaultdict(list)
         self.statistics = Statistics()
+        self._collected = [NormalizedDict(ignore="_")]
 
     def visit_suite(self, suite: TestSuite) -> None:
+        if suite.name in self._collected[-1] and suite.parent.source:
+            LOGGER.warn(
+                (
+                    f"Warning in {'file' if Path(suite.parent.source).is_file() else 'folder'} "
+                    f"'{suite.parent.source}': "
+                    if suite.source and Path(suite.parent.source).exists()
+                    else ""
+                )
+                + f"Multiple suites with name '{suite.name}' in suite '{suite.parent.longname}'."
+            )
+
+        self._collected[-1][suite.name] = True
+        self._collected.append(NormalizedDict(ignore="_"))
         try:
             item = TestItem(
                 type="suite",
                 id=f"{Path(suite.source).resolve() if suite.source is not None else ''};{suite.longname}",
                 name=suite.name,
                 longname=suite.longname,
                 uri=str(Uri.from_path(Path(suite.source).resolve())) if suite.source else None,
@@ -249,15 +284,26 @@
         finally:
             self._current = old_current
 
         self.statistics.suites += 1
         if suite.tests:
             self.statistics.suites_with_tests += 1
 
+    def end_suite(self, _suite: TestSuite) -> None:
+        self._collected.pop()
+
     def visit_test(self, test: TestCase) -> None:
+        if test.name in self._collected[-1]:
+            LOGGER.warn(
+                f"Warning in file '{test.source}' on line {test.lineno}: "
+                f"Multiple {'task' if test.parent.rpa else 'test'}s with name '{test.name}' in suite "
+                f"'{test.parent.longname}'."
+            )
+        self._collected[-1][test.name] = True
+
         if self._current.children is None:
             self._current.children = []
         try:
             item = TestItem(
                 type="test",
                 id=f"{Path(test.source).resolve() if test.source is not None else ''};{test.longname};{test.lineno}",
                 name=test.name,
@@ -280,15 +326,18 @@
         self._current.children.append(item)
 
         self.statistics.tests += 1
 
 
 @click.group(invoke_without_command=False)
 @click.option(
-    "--read-from-stdin", is_flag=True, help="Read file contents from stdin. This is an internal option.", hidden=True
+    "--read-from-stdin",
+    is_flag=True,
+    help="Read file contents from stdin. This is an internal option.",
+    hidden=True,
 )
 @pass_application
 def discover(app: Application, read_from_stdin: bool) -> None:
     """\
     Commands to discover informations about the current project.
 
     \b
@@ -300,15 +349,17 @@
     """
     if read_from_stdin:
         global _stdin_data
         _stdin_data = from_json(sys.stdin.buffer.read(), Dict[str, str], strict=True)
         app.verbose(f"Read data from stdin: {_stdin_data!r}")
 
 
-RE_IN_FILE_LINE_MATCHER = re.compile(r".+\sin\sfile\s'(?P<file>.*)'\son\sline\s(?P<line>\d+):(?P<message>.*)")
+RE_IN_FILE_LINE_MATCHER = re.compile(
+    r".+\sin\s(file|folder)\s'(?P<file>.*)'(\son\sline\s(?P<line>\d+))?:(?P<message>.*)"
+)
 RE_PARSING_FAILED_MATCHER = re.compile(r"Parsing\s'(?P<file>.*)'\sfailed:(?P<message>.*)")
 
 
 class DiagnosticsLogger:
     def __init__(self) -> None:
         self.messages: List[Message] = []
 
@@ -317,15 +368,18 @@
             self.messages.append(msg)
 
 
 def build_diagnostics(messages: List[Message]) -> Dict[str, List[Diagnostic]]:
     result: Dict[str, List[Diagnostic]] = {}
 
     def add_diagnostic(
-        message: Message, source_uri: Optional[str] = None, line: Optional[int] = None, text: Optional[str] = None
+        message: Message,
+        source_uri: Optional[str] = None,
+        line: Optional[int] = None,
+        text: Optional[str] = None,
     ) -> None:
         source_uri = str(Uri.from_path(Path(source_uri).resolve() if source_uri else Path.cwd()))
 
         if source_uri not in result:
             result[source_uri] = []
 
         result[source_uri].append(
@@ -339,29 +393,34 @@
                 source="robotcode.discover",
                 code="discover",
             )
         )
 
     for message in messages:
         if match := RE_IN_FILE_LINE_MATCHER.match(message.message):
-            add_diagnostic(message, match.group("file"), int(match.group("line")), text=match.group("message").strip())
+            add_diagnostic(
+                message,
+                match.group("file"),
+                int(match.group("line")) if match.group("line") is not None else None,
+                text=match.group("message").strip(),
+            )
         elif match := RE_PARSING_FAILED_MATCHER.match(message.message):
             add_diagnostic(message, match.group("file"), text=match.group("message").strip())
         else:
             add_diagnostic(message)
 
     return result
 
 
 def handle_options(
     app: Application,
     by_longname: Tuple[str, ...],
     exclude_by_longname: Tuple[str, ...],
     robot_options_and_args: Tuple[str, ...],
-) -> Tuple[TestSuite, Optional[Dict[str, List[Diagnostic]]]]:
+) -> Tuple[TestSuite, Collector, Optional[Dict[str, List[Diagnostic]]]]:
     root_folder, profile, cmd_options = handle_robot_options(
         app, by_longname, exclude_by_longname, robot_options_and_args
     )
 
     try:
         _patch()
 
@@ -414,15 +473,18 @@
 
         suite = builder.build(*arguments)
         settings.rpa = suite.rpa
         if settings.pre_run_modifiers:
             suite.visit(ModelModifier(settings.pre_run_modifiers, settings.run_empty_suite, LOGGER))
         suite.configure(**settings.suite_config)
 
-        return suite, build_diagnostics(diagnostics_logger.messages)
+        collector = Collector()
+        suite.visit(collector)
+
+        return suite, collector, build_diagnostics(diagnostics_logger.messages)
 
     except Information as err:
         app.echo(str(err))
         app.exit(INFO_PRINTED)
     except DataError as err:
         LOGGER.error(err)
         app.exit(DATA_ERROR)
@@ -454,26 +516,24 @@
     Examples:
     ```
     robotcode discover all
     robotcode --profile regression discover all
     ```
     """
 
-    suite, diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
-
-    collector = Collector()
-    suite.visit(collector)
+    suite, collector, diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
 
     if collector.all.children:
         if app.config.output_format is None or app.config.output_format == OutputFormat.TEXT:
             tests_or_tasks = "Task" if suite.rpa else "Test"
 
             def print(item: TestItem, indent: int = 0) -> Iterable[str]:
                 type = click.style(
-                    item.type.capitalize() if item.type == "suite" else tests_or_tasks.capitalize(), fg="green"
+                    item.type.capitalize() if item.type == "suite" else tests_or_tasks.capitalize(),
+                    fg="green",
                 )
 
                 if item.type == "test":
                     yield f"    {type}: {item.longname}{os.linesep}"
                 else:
                     yield f"{type}: {item.longname}{os.linesep}"
 
@@ -525,18 +585,15 @@
     Examples:
     ```
     robotcode discover tests
     robotcode --profile regression discover tests
     ```
     """
 
-    suite, diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
-
-    collector = Collector()
-    suite.visit(collector)
+    suite, collector, diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
 
     if collector.all.children:
         if app.config.output_format is None or app.config.output_format == OutputFormat.TEXT:
 
             def print(items: List[TestItem]) -> Iterable[str]:
                 for item in items:
                     yield f"{item.longname}{os.linesep}"
@@ -572,18 +629,15 @@
     Examples:
     ```
     robotcode discover suites
     robotcode --profile regression discover suites
     ```
     """
 
-    suite, diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
-
-    collector = Collector()
-    suite.visit(collector)
+    suite, collector, diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
 
     if collector.all.children:
         if app.config.output_format is None or app.config.output_format == OutputFormat.TEXT:
 
             def print(items: List[TestItem]) -> Iterable[str]:
                 for item in items:
                     yield f"{item.longname}{os.linesep}"
@@ -626,18 +680,15 @@
     robotcode discover tags
     robotcode --profile regression discover tags
 
     robotcode --profile regression discover tags -i wip
     ```
     """
 
-    suite, _diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
-
-    collector = Collector()
-    suite.visit(collector)
+    _suite, collector, _diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
 
     if collector.all.children:
         if app.config.output_format is None or app.config.output_format == OutputFormat.TEXT:
 
             def print(tags: Dict[str, List[TestItem]]) -> Iterable[str]:
                 for tag, items in tags.items():
                     yield f"{tag}{os.linesep}"
```

### Comparing `robotcode_runner-0.48.0/.gitignore` & `robotcode_runner-0.49.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.48.0/LICENSE.txt` & `robotcode_runner-0.49.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.48.0/README.md` & `robotcode_runner-0.49.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.48.0/pyproject.toml` & `robotcode_runner-0.49.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,17 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.48.0",
-  "robotcode-modifiers==0.48.0",
-  "robotcode==0.48.0",
+  "robotcode-robot==0.49.0",
+  "robotcode-modifiers==0.49.0",
+  "robotcode==0.49.0",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.48.0/PKG-INFO` & `robotcode_runner-0.49.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.48.0
+Version: 0.49.0
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.48.0
-Requires-Dist: robotcode-robot==0.48.0
-Requires-Dist: robotcode==0.48.0
+Requires-Dist: robotcode-modifiers==0.49.0
+Requires-Dist: robotcode-robot==0.49.0
+Requires-Dist: robotcode==0.49.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

