# Comparing `tmp/robotcode_language_server-0.48.0.tar.gz` & `tmp/robotcode_language_server-0.49.0.tar.gz`

## Comparing `robotcode_language_server-0.48.0.tar` & `robotcode_language_server-0.49.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21103 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    19239 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    40988 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    58866 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    71453 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83910 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    90141 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    42889 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/pyproject.toml
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.48.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21103 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    19239 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    40988 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    58866 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    71453 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83910 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    91023 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24170 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    42889 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/pyproject.toml
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/server.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,30 +28,32 @@
 from .model_helper import ModelHelperMixin
 from .protocol_part import RobotLanguageServerProtocolPart
 
 if TYPE_CHECKING:
     from robotcode.language_server.robotframework.protocol import RobotLanguageServerProtocol  # pragma: no cover
 
 
-CODEACTIONKINDS_QUICKFIX_CREATEKEYWORD = f"{CodeActionKind.QUICK_FIX.value}.createKeyword"
+CODEACTIONKIND_QUICKFIX_CREATEKEYWORD = f"{CodeActionKind.QUICK_FIX.value}.createKeyword"
 
 
 KEYWORD_WITH_ARGS_TEMPLATE = Template(
     """\
 ${name}
     [Arguments]    ${args}
-    Fail
+    # TODO: implement keyword "${name}".
+    Fail    Not Implemented
 
 """
 )
 
 KEYWORD_TEMPLATE = Template(
     """\
 ${name}
-    Fail
+    # TODO: implement keyword "${name}".
+    Fail    Not Implemented
 
 """
 )
 
 
 class FindKeywordSectionVisitor(AsyncVisitor):
     def __init__(self) -> None:
@@ -76,15 +78,15 @@
         parent.code_action.collect.add(self.collect)
 
         self.parent.commands.register_all(self)
 
     @language_id("robotframework")
     @code_action_kinds(
         [
-            CODEACTIONKINDS_QUICKFIX_CREATEKEYWORD,
+            CODEACTIONKIND_QUICKFIX_CREATEKEYWORD,
         ]
     )
     @_logger.call
     async def collect(
         self, sender: Any, document: TextDocument, range: Range, context: CodeActionContext
     ) -> Optional[List[Union[Command, CodeAction]]]:
         kw_not_found_in_diagnostics = next((d for d in context.diagnostics if d.code == "KeywordNotFoundError"), None)
@@ -126,22 +128,29 @@
 
         namespace = await self.parent.documents_cache.get_namespace(document)
 
         model = await self.parent.documents_cache.get_model(document, False)
         node = await get_node_at_position(model, range.start)
 
         if isinstance(node, (KeywordCall, Fixture, TestTemplate, Template)):
-            keyword = (
-                node.value
-                if isinstance(node, (TestTemplate, Template))
-                else node.keyword
-                if isinstance(node, KeywordCall)
-                else node.name
+            keyword_token = (
+                node.get_token(RobotToken.NAME)
+                if isinstance(node, (TestTemplate, Template, Fixture))
+                else node.get_token(RobotToken.KEYWORD)
             )
 
+            if keyword_token is None:
+                return
+
+            bdd_token, token = self.split_bdd_prefix(namespace, keyword_token)
+            if bdd_token is not None and token is not None:
+                keyword = token.value
+            else:
+                keyword = keyword_token.value
+
             arguments = []
 
             for t in node.get_tokens(RobotToken.ARGUMENT):
                 name, value = split_from_equals(cast(Token, t).value)
                 if value is not None and not contains_variable(name, "$@&%"):
                     arguments.append(f"${{{name}}}")
                 else:
```

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,28 +574,32 @@
                 sort_text=f"070_{setting}",
                 insert_text_format=InsertTextFormat.PLAIN_TEXT,
                 text_edit=TextEdit(range=range, new_text=f"[{setting}]") if range is not None else None,
             )
             for setting in settings
         ]
 
-    async def create_bdd_prefix_completion_items(self, range: Optional[Range]) -> List[CompletionItem]:
+    async def create_bdd_prefix_completion_items(
+        self, range: Optional[Range], at_top: bool = False, with_space: bool = True
+    ) -> List[CompletionItem]:
         prefixes = {"Given", "When", "Then", "And", "But"}
 
         if self.namespace.languages is not None:
             prefixes.update(self.namespace.languages.bdd_prefixes)
 
         return [
             CompletionItem(
                 label=prefix,
                 kind=CompletionItemKind.UNIT,
                 detail="BDD Prefix",
-                sort_text=f"080_{prefix}",
+                sort_text=f"000_{prefix}" if at_top else f"080_{prefix}",
                 insert_text_format=InsertTextFormat.PLAIN_TEXT,
-                text_edit=TextEdit(range=range, new_text=f"{prefix} ") if range is not None else None,
+                text_edit=TextEdit(range=range, new_text=prefix + (" " if with_space else ""))
+                if range is not None
+                else None,
             )
             for prefix in prefixes
         ]
 
     async def create_keyword_settings_completion_items(self, range: Optional[Range]) -> List[CompletionItem]:
         from robot.parsing.lexer.settings import KeywordSettings
 
@@ -670,26 +674,37 @@
     ) -> List[CompletionItem]:
         result: List[CompletionItem] = []
 
         r: Optional[Range] = None
 
         has_bdd = False
         bdd_token = None
+        only_bdd = False
 
         if token is not None:
             old_token = token
             bdd_token, token = self.split_bdd_prefix(self.namespace, token)
 
+            if (
+                bdd_token is None
+                and token is not None
+                and self.is_bdd_token(self.namespace, token)
+                and position.character > range_from_token(token).end.character
+            ):
+                bdd_token = token
+                token = None
+                only_bdd = True
+
             if token is not None and token.value == "":
                 token = None
 
             if bdd_token is not None and position.character > range_from_token(bdd_token).end.character:
                 has_bdd = True
 
-            if not has_bdd and token is None:
+            if not has_bdd and token is not None:
                 token = old_token
 
         if token is not None:
             r = range_from_token(token)
 
             if r is not None and "." in token.value:
 
@@ -873,20 +888,28 @@
                     kind=CompletionItemKind.KEYWORD,
                     sort_text="998_NONE",
                     insert_text_format=InsertTextFormat.PLAIN_TEXT,
                     text_edit=TextEdit(range=r, new_text="NONE"),
                 )
             )
 
-        if add_bdd_prefixes and not has_bdd:
-            result += await self.create_bdd_prefix_completion_items(
-                range_from_token(token) if token is not None else None
-            )
+        if add_bdd_prefixes and not (has_bdd or only_bdd):
+            bdd_range = r
+            at_top = False
+            with_space = True
+            if bdd_token is not None and (
+                position in range_from_token(bdd_token) or position == range_from_token(bdd_token).end.character
+            ):
+                at_top = True
+                with_space = False
+                bdd_range = range_from_token(bdd_token)
+
+            result += await self.create_bdd_prefix_completion_items(bdd_range, at_top, with_space)
 
-        if add_reserverd:
+        if add_reserverd and not (has_bdd or only_bdd):
             for k in get_reserved_keywords():
                 result.append(
                     CompletionItem(
                         label=k,
                         kind=CompletionItemKind.KEYWORD,
                         sort_text=f"999_{k}",
                         insert_text_format=InsertTextFormat.PLAIN_TEXT,
```

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,19 +609,17 @@
     @classmethod
     def is_bdd_token(cls, namespace: Namespace, token: Token) -> bool:
         if get_robot_version() < (6, 0):
             bdd_match = cls.BDD_TOKEN.match(token.value)
             return bool(bdd_match)
 
         parts = token.value.split()
-        if len(parts) < 2:
-            return False
 
-        for index in range(1, len(parts)):
-            prefix = " ".join(parts[:index]).title()
+        for index in range(0, len(parts)):
+            prefix = " ".join(parts[: index + 1]).title()
 
             if prefix.title() in (
                 namespace.languages.bdd_prefixes if namespace.languages is not None else DEFAULT_BDD_PREFIXES
             ):
                 return True
 
         return False
```

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/.gitignore` & `robotcode_language_server-0.49.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/LICENSE.txt` & `robotcode_language_server-0.49.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/README.md` & `robotcode_language_server-0.49.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.48.0/pyproject.toml` & `robotcode_language_server-0.49.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.48.0",
-  "robotcode==0.48.0",
+  "robotcode-jsonrpc2==0.49.0",
+  "robotcode==0.49.0",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 langserver = "robotcode.language_server.hooks"
 
 [project.urls]
```

### Comparing `robotcode_language_server-0.48.0/PKG-INFO` & `robotcode_language_server-0.49.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.48.0
+Version: 0.49.0
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.48.0
-Requires-Dist: robotcode==0.48.0
+Requires-Dist: robotcode-jsonrpc2==0.49.0
+Requires-Dist: robotcode==0.49.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

