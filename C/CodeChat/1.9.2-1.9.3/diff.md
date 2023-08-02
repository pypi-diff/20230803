# Comparing `tmp/CodeChat-1.9.2.tar.gz` & `tmp/CodeChat-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodeChat-1.9.2.tar", last modified: Sat Jun 11 03:19:19 2022, max compression
+gzip compressed data, was "CodeChat-1.9.3.tar", last modified: Wed Aug  2 22:12:57 2023, max compression
```

## Comparing `CodeChat-1.9.2.tar` & `CodeChat-1.9.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-06-11 03:19:19.349760 CodeChat-1.9.2/
-drwxrwxrwx   0        0        0        0 2022-06-11 03:19:19.314902 CodeChat-1.9.2/CodeChat/
--rw-rw-rw-   0        0        0     7083 2022-06-11 02:57:17.000000 CodeChat-1.9.2/CodeChat/CodeToMarkdown.py
--rw-rw-rw-   0        0        0     7409 2022-06-11 02:57:27.000000 CodeChat-1.9.2/CodeChat/CodeToPretext.py
--rw-rw-rw-   0        0        0    44026 2022-06-11 02:57:41.000000 CodeChat-1.9.2/CodeChat/CodeToRest.py
--rw-rw-rw-   0        0        0    17345 2022-06-11 02:57:42.000000 CodeChat-1.9.2/CodeChat/CodeToRestSphinx.py
--rw-rw-rw-   0        0        0    10664 2022-06-11 02:57:45.000000 CodeChat-1.9.2/CodeChat/CommentDelimiterInfo.py
--rw-rw-rw-   0        0        0    35998 2020-08-10 17:02:31.000000 CodeChat-1.9.2/CodeChat/LICENSE.rst
--rw-rw-rw-   0        0        0    26399 2022-06-11 02:57:46.000000 CodeChat-1.9.2/CodeChat/RestToCode.py
--rw-rw-rw-   0        0        0    42601 2022-06-11 02:57:46.000000 CodeChat-1.9.2/CodeChat/SourceClassifier.py
--rw-rw-rw-   0        0        0     1373 2022-06-11 03:03:44.000000 CodeChat-1.9.2/CodeChat/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-11 03:19:19.345800 CodeChat-1.9.2/CodeChat/css/
--rw-rw-rw-   0        0        0     2632 2022-06-11 02:57:57.000000 CodeChat-1.9.2/CodeChat/css/CodeChat.css
--rw-rw-rw-   0        0        0     1393 2022-06-11 02:57:54.000000 CodeChat-1.9.2/CodeChat/css/CodeChat_sphinx_rtd_theme.css
--rw-rw-rw-   0        0        0     4454 2022-02-11 13:33:28.000000 CodeChat-1.9.2/CodeChat/css/docutils.css
--rw-rw-rw-   0        0        0     4685 2021-10-25 14:42:38.000000 CodeChat-1.9.2/CodeChat/mdbook_CodeChat.py
-drwxrwxrwx   0        0        0        0 2022-06-11 03:19:19.335763 CodeChat-1.9.2/CodeChat.egg-info/
--rw-rw-rw-   0        0        0     4666 2022-06-11 03:19:18.000000 CodeChat-1.9.2/CodeChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      605 2022-06-11 03:19:19.000000 CodeChat-1.9.2/CodeChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-11 03:19:18.000000 CodeChat-1.9.2/CodeChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2022-06-11 03:19:18.000000 CodeChat-1.9.2/CodeChat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2022-06-11 03:19:19.000000 CodeChat-1.9.2/CodeChat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-06-11 03:19:19.000000 CodeChat-1.9.2/CodeChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2022-06-11 02:57:13.000000 CodeChat-1.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4666 2022-06-11 03:19:19.349760 CodeChat-1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     3899 2022-06-11 02:57:14.000000 CodeChat-1.9.2/README.rst
--rw-rw-rw-   0        0        0      615 2021-07-27 12:52:18.000000 CodeChat-1.9.2/pyproject.toml
--rw-rw-rw-   0        0        0      366 2022-06-11 03:19:19.351223 CodeChat-1.9.2/setup.cfg
--rw-rw-rw-   0        0        0     7860 2022-06-11 02:57:15.000000 CodeChat-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:12:57.750446 CodeChat-1.9.3/
+drwxrwxrwx   0        0        0        0 2023-08-02 22:12:57.663093 CodeChat-1.9.3/CodeChat/
+-rw-rw-rw-   0        0        0     7075 2023-08-02 21:52:24.000000 CodeChat-1.9.3/CodeChat/CodeToMarkdown.py
+-rw-rw-rw-   0        0        0     7401 2023-08-02 21:52:24.000000 CodeChat-1.9.3/CodeChat/CodeToPretext.py
+-rw-rw-rw-   0        0        0    45986 2023-08-02 21:52:43.000000 CodeChat-1.9.3/CodeChat/CodeToRest.py
+-rw-rw-rw-   0        0        0    17486 2023-08-02 21:52:24.000000 CodeChat-1.9.3/CodeChat/CodeToRestSphinx.py
+-rw-rw-rw-   0        0        0    10664 2022-06-11 02:57:45.000000 CodeChat-1.9.3/CodeChat/CommentDelimiterInfo.py
+-rw-rw-rw-   0        0        0    35998 2020-08-10 17:02:31.000000 CodeChat-1.9.3/CodeChat/LICENSE.rst
+-rw-rw-rw-   0        0        0    26391 2023-08-02 21:52:24.000000 CodeChat-1.9.3/CodeChat/RestToCode.py
+-rw-rw-rw-   0        0        0    42575 2023-08-02 21:52:24.000000 CodeChat-1.9.3/CodeChat/SourceClassifier.py
+-rw-rw-rw-   0        0        0     1373 2023-08-02 21:52:43.000000 CodeChat-1.9.3/CodeChat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:12:57.743306 CodeChat-1.9.3/CodeChat/css/
+-rw-rw-rw-   0        0        0     2632 2022-09-23 17:18:26.000000 CodeChat-1.9.3/CodeChat/css/CodeChat.css
+-rw-rw-rw-   0        0        0     1393 2022-09-23 17:18:26.000000 CodeChat-1.9.3/CodeChat/css/CodeChat_sphinx_rtd_theme.css
+-rw-rw-rw-   0        0        0      983 2023-08-02 21:52:35.000000 CodeChat-1.9.3/CodeChat/css/__init__.py
+-rw-rw-rw-   0        0        0     4454 2022-09-23 17:18:26.000000 CodeChat-1.9.3/CodeChat/css/docutils.css
+-rw-rw-rw-   0        0        0     4685 2021-10-25 14:42:38.000000 CodeChat-1.9.3/CodeChat/mdbook_CodeChat.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:12:57.712247 CodeChat-1.9.3/CodeChat.egg-info/
+-rw-rw-rw-   0        0        0     4666 2023-08-02 22:12:57.000000 CodeChat-1.9.3/CodeChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-08-02 22:12:57.000000 CodeChat-1.9.3/CodeChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 22:12:57.000000 CodeChat-1.9.3/CodeChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-08-02 22:12:57.000000 CodeChat-1.9.3/CodeChat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      118 2023-08-02 22:12:57.000000 CodeChat-1.9.3/CodeChat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 22:12:57.000000 CodeChat-1.9.3/CodeChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2022-06-11 02:57:13.000000 CodeChat-1.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4666 2023-08-02 22:12:57.751023 CodeChat-1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3899 2022-06-11 02:57:14.000000 CodeChat-1.9.3/README.rst
+-rw-rw-rw-   0        0        0      615 2021-07-27 12:52:18.000000 CodeChat-1.9.3/pyproject.toml
+-rw-rw-rw-   0        0        0      367 2023-08-02 22:12:57.756497 CodeChat-1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     7864 2023-08-02 21:52:35.000000 CodeChat-1.9.3/setup.py
```

### Comparing `CodeChat-1.9.2/CodeChat/CodeToMarkdown.py` & `CodeChat-1.9.3/CodeChat/CodeToMarkdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 # This function converts a string containing source code to Markdown, preserving all indentations of both source code and comments. To do so, the comment characters are stripped from CodeChat-formatted comments and all code is placed inside fenced code blocks.
 def code_to_markdown_string(
     # _`code_str`: the code to translate to markdown.
     code_str,
     # See `options <options>`.
     **options
 ):
-
     # Use a StringIO to capture writes into a string.
     output_md = StringIO()
     # Include a header containing some `CodeChat style`.
     output_md.write(codechat_style + "\n\n")
     ast_syntax_error, classified_lines = source_lexer(
         code_str, get_lexer(code=code_str, **options)
     )
@@ -104,15 +103,14 @@
     # .. _output_encoding:
     #
     # Encoding to use for the output file.
     output_encoding="utf-8",
     # See `options <options>`.
     **options
 ):
-
     # Provide a default ``rst_path``.
     if not md_path:
         md_path = source_path + ".md"
     with open(source_path, encoding=input_encoding) as fi:
         code_str = fi.read()
     # If not already present, provide the filename of the source to help in identifying a lexer.
     options.setdefault("filename", source_path)
@@ -137,15 +135,14 @@
     # An iterable of (type, string) pairs, one per line.
     classified_lines,
     # .. _out_file:
     #
     # A file-like output to which the markdown text is written.
     out_file,
 ):
-
     # Keep track of the current type. Begin with neither comment nor code.
     current_type = -2
 
     # Keep track of the current line number.
     line = 1
 
     for type_, string in classified_lines:
@@ -188,15 +185,14 @@
 # Output text produced when exiting a state. Supports `_generate_markdown`_.
 def _exit_state(
     # The type (classification) of the last line.
     type_,
     # See out_file_.
     out_file,
 ):
-
     # Code state: emit an ending fence.
     if type_ == -1:
         out_file.write(_fence + "\n")
     # Comment state: emit a closing indent.
     elif type_ > 0:
         out_file.write("\n</div>\n\n")
     # Initial state or non-indented comment. Nothing needed.
```

### Comparing `CodeChat-1.9.2/CodeChat/CodeToPretext.py` & `CodeChat-1.9.3/CodeChat/CodeToPretext.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 # This function converts a string containing source code to PreTeXt, preserving all indentations of both source code and comments. To do so, the comment characters are stripped from CodeChat-formatted comments and all code is placed inside fenced code blocks.
 def code_to_pretext_string(
     # _`code_str`: the code to translate to PreTeXt.
     code_str,
     # See `options <options>`.
     **options,
 ):
-
     # Use a StringIO to capture writes into a string.
     output_ptx = StringIO()
     ast_syntax_error, classified_lines = source_lexer(
         code_str, get_lexer(code=code_str, **options)
     )
     # Remove the newline from a syntax error, so that source line numbers match exactly with the lines output by this function.
     if ast_syntax_error:
@@ -96,15 +95,14 @@
     # .. _output_encoding:
     #
     # Encoding to use for the output file.
     output_encoding="utf-8",
     # See `options <options>`.
     **options,
 ):
-
     # Provide a default ``rst_path``.
     if not pt_path:
         pt_path = source_path + ".ptx"
     with open(source_path, encoding=input_encoding) as fi:
         code_str = fi.read()
     # If not already present, provide the filename of the source to help in identifying a lexer.
     options.setdefault("filename", source_path)
@@ -127,15 +125,14 @@
     # An iterable of (type, string) pairs, one per line.
     classified_lines,
     # .. _out_file:
     #
     # A file-like output to which the pretext source is written.
     out_file,
 ):
-
     # Determine the number of characters produced when a newline is written.
     newline_chars = out_file.write("\n")
     # Undo this write.
     out_file.seek(out_file.tell() - newline_chars, 0)
 
     # Keep track of the current type. Begin with neither comment nor code.
     current_type = -2
@@ -187,15 +184,14 @@
     # One line from the program being translated.
     string,
     # See out_file_.
     out_file,
     # The number of character written by a newline.
     newline_chars,
 ):
-
     # Code state: do nothing.
     if type_ == -1:
         pass
     # Comment state: emit a closing ``</p>`` tag if it wasn't provided.
     elif type_ >= 0:
         if not re.search(xml_closing_tag_regex, string):
             # Append it to the end of the string by backing up one character (the existing newline at the end of the current line).
```

### Comparing `CodeChat-1.9.2/CodeChat/CodeToRest.py` & `CodeChat-1.9.3/CodeChat/CodeToRest.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,29 +29,27 @@
 # =======
 # These are listed in the order prescribed by `PEP 8
 # <http://www.python.org/dev/peps/pep-0008/#imports>`_.
 #
 # Standard library
 # ----------------
 import html
+import importlib.resources
 from io import StringIO
-import os.path
 from pathlib import Path
 import re
 
 # Third-party imports
 # -------------------
 from docutils import io, core, nodes
 from docutils.parsers.rst.directives.body import CodeBlock
 from docutils.parsers.rst import directives, Directive, roles
 from docutils.writers.html4css1 import Writer
 from docutils.parsers.rst import states
 from docutils import statemachine, utils
-from docutils.utils.error_reporting import SafeString, ErrorString
-import pkg_resources
 
 # Local application imports
 # -------------------------
 from .SourceClassifier import source_lexer, get_lexer, _debug_print, codechat_style
 
 
 # API
@@ -65,17 +63,16 @@
 # code_to_rest_string
 # -------------------
 # This function converts a string containing source code to reST, preserving all indentations of both source code and comments. To do so, the comment characters are stripped from reST-formatted comments and all code is placed inside code blocks.
 def code_to_rest_string(
     # _`code_str`: the code to translate to reST.
     code_str,
     # See `options <options>`.
-    **options
+    **options,
 ):
-
     lexer = get_lexer(code=code_str, **options)
     if not lexer:
         raise ValueError("Unable to determine a lexer for this string.")
 
     # Use a StringIO to capture writes into a string.
     output_rst = StringIO()
     # Include a header containing some `CodeChat style`. Don't put this in a separate ``.js`` file, since docutils doesn't have an easy way to include it.
@@ -106,17 +103,16 @@
     # encoding of the input file.
     input_encoding=None,
     # .. _output_encoding:
     #
     # Encoding to use for the output file.
     output_encoding="utf-8",
     # See `options <options>`.
-    **options
+    **options,
 ):
-
     # Provide a default ``rst_path``.
     if not rst_path:
         rst_path = source_path + ".rst"
     # Use docutil's I/O classes to better handle and sniff encodings.
     #
     # Note: both these classes automatically close themselves after a
     # read or write.
@@ -138,17 +134,16 @@
 def code_to_html_string(
     # See code_str_.
     code_str,
     # A file-like object where warnings and errors will be written, or None to
     # send them to stderr.
     warning_stream=None,
     # See `options <options>`.
-    **options
+    **options,
 ):
-
     rest = code_to_rest_string(code_str, **options)
     # `docutils
     # <http://docutils.sourceforge.net/docs/user/tools.html#rst2html-py>`_
     # converts reST to HTML.
     html = core.publish_string(
         rest,
         writer_name="html",
@@ -181,15 +176,14 @@
     # overwritten. If not supplied, ``source_path.html`` will be assumed.
     html_path=None,
     # See input_encoding_.
     input_encoding=None,
     # See output_encoding_.
     output_encoding="utf-8",
 ):
-
     html_path = html_path or source_path + ".html"
     fi = io.FileInput(source_path=source_path, encoding=input_encoding)
     fo = io.FileOutput(destination_path=html_path, encoding=output_encoding)
 
     code_str = fi.read()
     lexer = get_lexer(filename=source_path, code=code_str)
     html = code_to_html_string(code_str, lexer=lexer)
@@ -197,16 +191,17 @@
     fo.write(html)
 
 
 # Styling
 # --------
 # Provide a programmatic way to get a list of paths to static files needed by CodeChat. When using Sphinx, this should be assigned or appended to `html_static_path <http://sphinx-doc.org/config.html#confval-html_static_path>`_.
 def html_static_path():
-    # There's only one path needed -- ``css/``, relative to this directory.
-    return [pkg_resources.resource_filename("CodeChat", "css")]
+    # There's only one path needed -- ``css/``, relative to this directory. TODO: this won't correctly handle resources that get placed in temp files, such as a zip file.
+    with importlib.resources.as_file(importlib.resources.files("CodeChat.css")) as p:
+        return [str(p)]
 
 
 # Provide correct formatting of CodeChat-produced documents in reST based on the `CodeChat style`.
 rest_codechat_style = ".. raw:: html\n\n " + codechat_style + "\n\n"
 
 
 # .. _Converting_classified_code_to_reST:
@@ -352,14 +347,15 @@
 # |                          |  Three space indent     |                                   |
 # |                          |                         |                                   |
 # |                          |  .. raw:: html          |                                   |
 # |                          |                         |                                   |
 # |                          |   </div>                |                                   |
 # +--------------------------+-------------------------+-----------------------------------+
 
+
 # Following either a fenced code block or a raw block, care must be taken to
 # separate these blocks' content from indented comments which follow them. For
 # example, the following code:
 #
 # +--------------------------+-------------------------+-----------------------------------+
 # + Python source            + Translated to reST      | Translated to (simplified) HTML   |
 # +==========================+=========================+===================================+
@@ -428,15 +424,14 @@
     # An iterable of (type, string) pairs, one per line.
     classified_lines,
     # .. _out_file:
     #
     # A file-like output to which the reST text is written.
     out_file,
 ):
-
     # Keep track of the current type. Begin with a 0-indent comment.
     current_type = -2
 
     # Keep track of the current line number.
     line = 1
 
     for type_, string in classified_lines:
@@ -495,15 +490,14 @@
 # Output text produced when exiting a state. Supports `_generate_rest`_.
 def _exit_state(
     # The type (classification) of the last line.
     type_,
     # See out_file_.
     out_file,
 ):
-
     # Code state: emit an ending fence.
     if type_ == -1:
         out_file.write(" Ending fence\n\n..\n\n")
     # Comment state: emit a closing indent.
     elif type_ > 0:
         out_file.write("\n.. raw:: html\n\n </div>\n\n..\n\n")
     # Initial state. Nothing needed.
@@ -603,15 +597,14 @@
 #
 # _SetLine
 # ^^^^^^^^
 # This directive allows changing the line number at which errors will be
 # reported. ``.. set-line:: 10`` makes the current line report as line 10,
 # regardless of its actual location in the file.
 class _SetLine(Directive):
-
     required_arguments = 1
     optional_arguments = 0
     final_argument_whitespace = False
     option_spec = {}
     has_content = False
 
     def run(self):
@@ -676,15 +669,14 @@
     # The ``docutils.parsers.rst.states.Inliner`` object that called this function. It contains the several attributes useful for error reporting and document tree access.
     inliner,
     # A dictionary of directive options for customization (from the "role" directive), to be interpreted by this function. Used for additional attributes for the generated elements and other functionality.
     options={},
     # A list of strings, the directive content for customization (from the "role" directive). To be interpreted by the role function.
     content=[],
 ):
-
     # See https://doughellmann.com/blog/2010/05/09/defining-custom-roles-in-sphinx/.
     env = inliner.document.settings.env
     try:
         # Invoke
         p = Path(env.docname)
         # Return p.<text> using `getattr <https://docs.python.org/3/library/functions.html#getattr>`_.
         path_component = str(getattr(p, text, p))
@@ -706,15 +698,14 @@
 # This function returns the ``source``; it also prepends a Sphinx `highlight directive <http://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#directive-highlight>`_ if possible.
 def add_highlight_language(
     # The source reST to potentially prepend a `highlight directive`_ to.
     source,
     # The lexer which was used to produce this source.
     lexer,
 ):
-
     # If there's `file-wide metadata <http://www.sphinx-doc.org/en/stable/markup/misc.html#file-wide-metadata>`_, then it's hard to know where the `highlight directive`_ can be safely placed:
     #
     # - Putting it before file-wide metadata demotes it to not being metadata.
     # - Finding the right place to put the ``.. highlight`` directive after the metadata is difficult to know.
     if not re.search("^:(tocdepth|nocomments|orphan):", source, re.MULTILINE):
         # There's no file-wide metadata. Add the `highlight directive`_.
         return ".. highlight:: {}\n\n{}".format(lexer.aliases[0], source)
@@ -725,15 +716,15 @@
 
 # .. _`_CodeInclude`:
 #
 # _CodeInclude
 # ^^^^^^^^^^^^
 # Provide a way to include source code to be processed by CodeChat. It is a slight modification of the `docutils include directive <https://docutils.sourceforge.io/docs/ref/rst/directives.html#including-an-external-document-fragment>`_ and supports all the same options; it also supports the `class <https://docutils.sourceforge.io/docs/ref/rst/directives.html#id22>`_ option.
 #
-# Implementation note: this is mostly copied directly from ``docutils.parsers.rst.directives.misc.Include``, version 0.16.
+# Implementation note: this is mostly copied directly from ``docutils.parsers.rst.directives.misc.Include``, version 0.21.
 class _CodeInclude(Directive):
 
     """
     Include content read from a separate source file.
 
     Content will be lexed based on the provided lexer then parsed by the
     parser. The encoding of the included file can be specified. Only
@@ -753,64 +744,69 @@
         "start-line": int,
         "end-line": int,
         "start-after": directives.unchanged_required,
         "end-before": directives.unchanged_required,
         "class": directives.class_option,
     }
 
-    standard_include_path = os.path.join(os.path.dirname(states.__file__), "include")
+    standard_include_path = Path(states.__file__).parent / "include"
 
     def run(self):
-        """Include a file as part of the content of this reST file."""
+        """Include a file as part of the content of this reST file.
+
+        Depending on the options, the file (or a clipping) is
+        converted to nodes and returned or inserted into the input stream.
+        """
         if not self.state.document.settings.file_insertion_enabled:
             raise self.warning('"%s" directive disabled.' % self.name)
-        source = self.state_machine.input_lines.source(
-            self.lineno - self.state_machine.input_offset - 1
-        )
-        source_dir = os.path.dirname(os.path.abspath(source))
+        current_source = self.state.document.current_source
         path = directives.path(self.arguments[0])
         if path.startswith("<") and path.endswith(">"):
-            path = os.path.join(self.standard_include_path, path[1:-1])
-        path = os.path.normpath(os.path.join(source_dir, path))
-        path = utils.relative_path(None, path)
-        path = nodes.reprunicode(path)
+            _base = self.standard_include_path
+            path = path[1:-1]
+        else:
+            _base = Path(current_source).parent
+        path = utils.relative_path(None, _base / path)
         encoding = self.options.get(
             "encoding", self.state.document.settings.input_encoding
         )
         e_handler = self.state.document.settings.input_encoding_error_handler
         tab_width = self.options.get(
             "tab-width", self.state.document.settings.tab_width
         )
         try:
-            self.state.document.settings.record_dependencies.add(path)
             include_file = io.FileInput(
                 source_path=path, encoding=encoding, error_handler=e_handler
             )
         except UnicodeEncodeError:
             raise self.severe(
-                'Problems with "%s" directive path:\n'
-                'Cannot encode input file path "%s" '
-                "(wrong locale?)." % (self.name, SafeString(path))
+                f'Problems with "{self.name}" directive path:\n'
+                f'Cannot encode input file path "{path}" '
+                "(wrong locale?)."
             )
-        except IOError as error:
+        except OSError as error:
             raise self.severe(
-                'Problems with "%s" directive path:\n%s.'
-                % (self.name, ErrorString(error))
+                f'Problems with "{self.name}" directive '
+                f"path:\n{io.error_string(error)}."
             )
+        else:
+            self.state.document.settings.record_dependencies.add(path)
+
+        # Get to-be-included content
         startline = self.options.get("start-line", None)
         endline = self.options.get("end-line", None)
         try:
             if startline or (endline is not None):
                 lines = include_file.readlines()
                 rawtext = "".join(lines[startline:endline])
             else:
                 rawtext = include_file.read()
         except UnicodeError as error:
             raise self.severe(
-                'Problem with "%s" directive:\n%s' % (self.name, ErrorString(error))
+                f'Problem with "{self.name}" directive:\n' + io.error_string(error)
             )
         # start-after/end-before: no restrictions on newlines in match-text,
         # and no restrictions on matching inside lines vs. line boundaries
         after_text = self.options.get("start-after", None)
         if after_text:
             # skip content in rawtext before *and incl.* a matching text
             after_index = rawtext.find(after_text)
@@ -870,16 +866,55 @@
             rawtext = add_highlight_language(rawtext, lexer)
         ##------------
         # ... to here.
 
         include_lines = statemachine.string2lines(
             rawtext, tab_width, convert_whitespace=True
         )
+        for i, line in enumerate(include_lines):
+            if len(line) > self.state.document.settings.line_length_limit:
+                raise self.warning(
+                    '"%s": line %d exceeds the' " line-length-limit." % (path, i + 1)
+                )
+
         # **Deleted code**: Options for ``literal`` and ``code`` don't apply.
+        # Prevent circular inclusion:
+        clip_options = (startline, endline, before_text, after_text)
+        include_log = self.state.document.include_log
+        # log entries are tuples (<source>, <clip-options>)
+        if not include_log:  # new document, initialize with document source
+            include_log.append(
+                (utils.relative_path(None, current_source), (None, None, None, None))
+            )
+        if (path, clip_options) in include_log:
+            master_paths = (pth for (pth, opt) in reversed(include_log))
+            inclusion_chain = "\n> ".join((path, *master_paths))
+            raise self.warning(
+                'circular inclusion in "%s" directive:\n%s'
+                % (self.name, inclusion_chain)
+            )
+
+        if "parser" in self.options:
+            # parse into a dummy document and return created nodes
+            document = utils.new_document(path, self.state.document.settings)
+            document.include_log = include_log + [(path, clip_options)]
+            parser = self.options["parser"]()
+            parser.parse("\n".join(include_lines), document)
+            # clean up doctree and complete parsing
+            document.transformer.populate_from_components((parser,))
+            document.transformer.apply_transforms()
+            return document.children
+
+        # Include as rST source:
+        #
+        # mark end (cf. parsers.rst.states.Body.comment())
+        include_lines += ["", '.. end of inclusion from "%s"' % path]
         self.state_machine.insert_input(include_lines, path)
+        # update include-log
+        include_log.append((path, clip_options))
         return []
 
 
 # Register the new directives and role with docutils.
 directives.register_directive("fenced-code", _FencedCodeBlock)
 directives.register_directive("set-line", _SetLine)
 # Imitate Sphinx's naming convention of `literalinclude <http://www.sphinx-doc.org/en/stable/markup/code.html#directive-literalinclude>`_.
```

### Comparing `CodeChat-1.9.2/CodeChat/CodeToRestSphinx.py` & `CodeChat-1.9.3/CodeChat/CodeToRestSphinx.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,23 @@
 # -------------------
 import sphinx
 from sphinx.application import Sphinx
 from sphinx.config import Config
 import sphinx.io
 import sphinx.project
 import sphinx.util
-from sphinx.util import path_stabilize
+
+# This was deprecated_ in Sphinx v5.1.0.
+if sphinx.version_info[:3] >= (5, 1, 0):
+    from sphinx.util.osutil import path_stabilize
+else:
+    from sphinx.util import path_stabilize
 from sphinx.util.osutil import SEP, relpath
 
-# The exception ``FiletypeNotFoundError`` was `deprecated in Sphinx v2.4.0 <https://www.sphinx-doc.org/en/master/extdev/deprecated.html>`_ by moving it from ``sphinx.io`` to ``sphinx.errors``.
+# The exception ``FiletypeNotFoundError`` was `deprecated <https://www.sphinx-doc.org/en/master/extdev/deprecated.html>`_  in Sphinx v2.4.0 by moving it from ``sphinx.io`` to ``sphinx.errors``.
 if sphinx.version_info[:3] >= (2, 4, 0):
     from sphinx.errors import FiletypeNotFoundError
 else:
     from sphinx.io import FiletypeNotFoundError
 import pygments.util
 
 # Local application imports
@@ -115,15 +120,14 @@
     app,
     # _`docname`: The name of the document that was read. It contains a path
     # relative to the project directory and (typically) no extension.
     docname,
     # A list whose single element is the contents of the source file.
     source,
 ):
-
     if is_source_code(app.env, docname):
         # See if it's an extension we should process.
         try:
             # See if ``source_file`` matches any of the globs.
             lexer = None
             lfg = app.config.CodeChat_lexer_for_glob
             path_docname = Path(docname)
@@ -158,15 +162,14 @@
 # Return True if the supplied ``docname`` is source code.
 def is_source_code(
     # The `Sphinx build environment <http://www.sphinx-doc.org/en/1.5.1/extdev/envapi.html>`_.
     env,
     # See docname_.
     docname,
 ):
-
     # If the docname's extension doesn't change when asking for its full path,
     # then it's source code. Normally, the docname of ``foo.rst`` is ``foo``;
     # only for source code is the docname of ``foo.c`` also ``foo.c``. Look up
     # the name and extension using `doc2path
     # <http://sphinx-doc.org/extdev/envapi.html#sphinx.environment.BuildEnvironment.doc2path>`_.
     docname_ext = env.doc2path(docname, None)
     return Path(docname_ext) == Path(docname)
@@ -302,25 +305,26 @@
         # This was the existing code.
         raise FiletypeNotFoundError
 
 
 # Per the `where to patch <https://docs.python.org/3/library/unittest.mock.html#where-to-patch>`_ docs, patch this where the ``get_filetype`` function is used, not where it's defined:
 SPHINX_VERSION = sphinx.version_info[:3]
 if SPHINX_VERSION >= (2, 4, 0) and SPHINX_VERSION < (4, 0, 0):
-    # The function ``sphinx.io.get_filetype`` was `deprecated in Sphinx v2.4.0`_; it was renamed to ``sphinx.util.get_filetype`` instead. Sphinx uses ``sphinx.deprecation._ModuleWrapper`` to perform deprecation. Since ``get_filetype`` is used in ``sphinx.io``, we need to monkeypatch inside it, hence the ``_module`` (a member of the ``_ModuleWrapper``).
+    # The function ``sphinx.io.get_filetype`` was deprecated_ in Sphinx v2.4.0; it was renamed to ``sphinx.util.get_filetype`` instead. Sphinx uses ``sphinx.deprecation._ModuleWrapper`` to perform deprecation. Since ``get_filetype`` is used in ``sphinx.io``, we need to monkeypatch inside it, hence the ``_module`` (a member of the ``_ModuleWrapper``).
     sphinx.io._module.get_filetype = _get_filetype
 elif SPHINX_VERSION >= (4, 0, 0) and SPHINX_VERSION < (5, 0, 0):
     # In these versions, ``get_filetype`` is used in ``sphinx.io``. It's no longer deprecated, but removed; therefore, a direct monkeypatch works.
     sphinx.io.get_filetype = _get_filetype
 else:
     # In current Sphinx, ``get_filetype`` is used in several places:
     sphinx.builders.get_filetype = _get_filetype
     sphinx.io.get_filetype = _get_filetype
     sphinx.transforms.i18n.get_filetype = _get_filetype
 
+
 # Correct naming for the "show source" option
 # ===========================================
 # The following function corrects the extension of source files in the
 # "source" link. By default, Sphinx (in ``sphinx.builders.html.StandaloneHTMLBuilder.get_doc_context``)
 # creates a sourcename by appending a file's extension to the value returned by
 # ``doc2path``. For non-source files, ``doc2path``'s return value contains no
 # extension, so this works fine. However, for source files, ``doc2path``'s
@@ -338,15 +342,14 @@
     # A dictionary of values that are given to the template engine to render the
     # page and can be modified to include custom values. Keys must be strings.
     context,
     # A doctree when the page is created from a reST documents; None when the
     # page is created from an HTML template alone.
     doctree,
 ):
-
     sourcename = context.get("sourcename")
     ext = Path(pagename).suffix
     # The extension Sphinx uses optionally includes the `html_sourcelink_suffix <http://www.sphinx-doc.org/en/stable/config.html#confval-html_sourcelink_suffix>`_.
     sphinx_ext = ext + (
         ""
         if ext == app.config.html_sourcelink_suffix
         else app.config.html_sourcelink_suffix
@@ -363,15 +366,14 @@
 # This routine defines the `entry point
 # <http://sphinx-doc.org/extdev/appapi.html>`_ called by Sphinx to initialize
 # this extension.
 def setup(
     # See app_.
     app,
 ):
-
     # Ensure we're using a new enough Sphinx using `require_sphinx
     # <http://sphinx-doc.org/extdev/appapi.html#sphinx.application.Sphinx.require_sphinx>`_.
     app.require_sphinx("2.0")
 
     # Use the `source-read <http://sphinx-doc.org/extdev/appapi.html#event-source-read>`_
     # event hook to transform source code to reST before Sphinx processes it.
     app.connect("source-read", _source_read)
```

### Comparing `CodeChat-1.9.2/CodeChat/CommentDelimiterInfo.py` & `CodeChat-1.9.3/CodeChat/CommentDelimiterInfo.py`

 * *Files identical despite different names*

### Comparing `CodeChat-1.9.2/CodeChat/LICENSE.rst` & `CodeChat-1.9.3/CodeChat/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `CodeChat-1.9.2/CodeChat/RestToCode.py` & `CodeChat-1.9.3/CodeChat/RestToCode.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,14 @@
     # See comment_delimiters_.
     comment_delimiters,
     # See position_.
     position,
     # See line_counter_.
     line_counter,
 ):
-
     # This covers the case that the language does not support inline comments.
     # It places block comment delimiters around a single line to give an inline effect
     # There is no added space between the end of the comment and the end delimiter because this
     # space is not taken out in the Code to reST translation. If a space is added, it is no
     # longer round trip stable. (It adds a space every time it is translated.)
     if line_counter is None:
         f = "{} {}{}\n".format(comment_delimiters[1], line, comment_delimiters[2])
@@ -186,15 +185,14 @@
     out_path=None,
     # _`input_encoding`: Encoding to use for the input file. The default of None detects the encoding
     # of the input file.
     input_encoding=None,
     # _`output_encoding`: Encoding to use for the output file.
     output_encoding="utf-8",
 ):
-
     if out_path is None:
         # Find the file extension of the given language.
         file_ext = find_file_ext(lang)
         # Obtain the file path without the ``.rst`` extension.
         file_name_list = source_rst_path.rsplit(".", 1)
         file_name = file_name_list[0]
         # Place the file extension on the file path.
@@ -438,15 +436,14 @@
     # but with the correct file extension for the given lang_
     out_path=None,
     # See input_encoding_
     input_encoding=None,
     # See output_encoding_
     output_encoding="utf-8",
 ):
-
     if out_path is None:
         # Find the file extension of the given language.
         file_ext = find_file_ext(lang)
         # Obtain the file path without the ``.rst`` extension.
         file_name_list = source_html_path.rsplit(".", 1)
         file_name = file_name_list[0]
         # Place the file extension on the file path.
@@ -473,15 +470,14 @@
 def html_to_code_string(
     # _`html_str`: The string of HTML that will get converted into code.
     # This string is generally multiple lines. The program separates and processes all the lines it is given.
     html_str,
     # See lang_.
     lang,
 ):
-
     string_out = "\n.. set-line:: -3\n\n..\n\n"
 
     def traverse_etree(element):
         nonlocal string_out
         if isinstance(element.tag, str):
             tag = element.tag
             if tag == "p":
```

### Comparing `CodeChat-1.9.2/CodeChat/SourceClassifier.py` & `CodeChat-1.9.3/CodeChat/SourceClassifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     # The MIME type of the source file to lex.
     mimetype=None,
     # The code to be highlighted, used to guess a lexer.
     code=None,
     # _`options`: Specify the lexer (see `get_lexer` arguments), and provide it any other needed options.
     **options
 ):
-
     # This sets the default tabsize to 4 spaces in
     # `Pygments' lexer <http://pygments.org/docs/api/#pygments.lexer.Lexer>`_,
     # and this link is a list  of
     # `all available lexers <http://pygments.org/docs/lexers/#available-lexers>`_
     options.setdefault("tabsize", 4)
 
     if lexer:
@@ -121,15 +120,14 @@
 # **This routine is the heart of the algorithm.**
 def source_lexer(
     # _`code_str`: the code to classify.
     code_str,
     # _`lexer`: The lexer used to analyze the code.
     lexer,
 ):
-
     _debug_print("Lexer: {}\n".format(lexer.name))
     # Gather some additional information, based on the lexer, which is needed
     # to correctly process comments:
     cdi = COMMENT_DELIMITER_INFO[lexer.name]
     # * If there's no multi-line start info, then classify generic comments as
     #   inline. The exception is HTML, which (currently, as of Pygments v.10.0) classifies as generic comments, but also supports in-line JavaScript comments.
     comment_is_inline = False if lexer.name == "HTML" else not cdi[1]
@@ -260,15 +258,14 @@
 # -----------------------
 def _pygments_lexer(
     # See code_str_.
     code_str,
     # See lexer_.
     lexer,
 ):
-
     # Pygments does some cleanup on the code given to it before lexing it. If
     # this is Python code, we want to run AST on that cleaned-up version, so
     # that AST results can be correlated with Pygments results. However,
     # Pygments doesn't offer a way to do this; so, add that ability in to the
     # detected lexer.
     preprocessed_code_str = _pygments_get_tokens_preprocess(lexer, code_str)
     # Note: though Pygments does support a `String.Doc token type <http://pygments.org/docs/tokens/#literals>`_,
@@ -461,15 +458,14 @@
     # .. _comment_is_block:
     #
     # When true, classify generic comment as block comments.
     comment_is_block,
     # Docstring dict found from AST scanning.
     ast_docstring,
 ):
-
     # Keep track of the current group, string, and line no.
     current_string = ""
     current_group = None
     token_lineno = 1
     # Walk through tokens.
     for tokentype, string in iter_token:
         _debug_print("tokentype = {}, string = {}\n".format(tokentype, [string]))
@@ -532,15 +528,14 @@
     # The tokentype to place into a group.
     tokentype,
     # See comment_is_inline_.
     comment_is_inline,
     # See comment_is_block_.
     comment_is_block,
 ):
-
     # The list of Pygments `tokens <http://pygments.org/docs/tokens/>`_ lists
     # ``Token.Text`` (how a newline is classified) and ``Token.Whitespace``.
     # Consider either as whitespace.
     if tokentype in Token.Text or tokentype in Token.Whitespace:
         return _GROUP.whitespace
     # There is a Token.Comment, but this can refer to inline or block comments.
     # Therefore, use info from CommentDelimiterInfo as a tiebreaker.
@@ -574,15 +569,14 @@
     # ``group_lexer_tokens``.
     iter_grouped,
     # .. _comment_delim_info:
     #
     # An element of COMMENT_DELIMITER_INFO for the language being classified.
     comment_delim_info,
 ):
-
     # Keep a list of (group, string) tuples we're accumulating.
     _list = []
 
     # Keep track of the length of whitespace at the beginning of the body and
     # end portions of a block comment.
     ws_len = 0
 
@@ -756,15 +750,14 @@
     # same parameters as is_delim_indented_line_.
     delim,
     # True if this is the last line of a multi-line comment.
     is_last,
     # See comment_delim_info_.
     comment_delim_info,
 ):
-
     # A line containing only whitespace is always considered valid.
     if line.isspace():
         return True
     # A line beginning with ws_len spaces has the expected indent.
     if len(line) > indent_len and line[:indent_len].isspace():
         return True
 
@@ -827,15 +820,14 @@
     # Delimiter expected near the end of an indent (one character).
     delim,
     # True if this is the last line of a multi-line comment.
     is_last,
     # See comment_delim_info_.
     comment_delim_info,
 ):
-
     # A line the correct number of spaces, followed by a delimiter then either
     # a space or a newline is correctly indented.
     if (
         len(line) >= indent_len
         and line[: indent_len - 2].isspace()
         and line[indent_len - 2] == delim
         and line[indent_len - 1] in "\n "
@@ -878,24 +870,22 @@
     # ``gather_groups_on_newlines``.
     iter_gathered_groups,
     # See comment_delim_info_.
     comment_delim_info,
     # See lexer_.
     lexer,
 ):
-
     # Keep track of block comment state.
     is_block_rest_comment = False
 
     # Walk through groups.
     for _list in iter_gathered_groups:
         _debug_print("[(group, ws_len, string), ...] = {}\n".format(_list))
 
         if _is_rest_comment(_list, is_block_rest_comment, comment_delim_info, lexer):
-
             first_group, first_ws_len, first_string = _list[0]
             # The type = # of leading whitespace characters, or 0 if none.
             if first_group == _GROUP.whitespace:
                 # Encode this whitespace in the type, then drop it.
                 type_ = len(first_string)
                 _list.pop(0)
                 first_group, first_ws_len, first_string = _list[0]
@@ -957,15 +947,14 @@
     # The string corresponding to this group.
     string,
     # See comment_delim_info_.
     comment_delim_info,
     # See lexer_.
     lexer,
 ):
-
     # Number of characters in an opening block comment.
     len_opening_block_comment_delim = len(comment_delim_info[1])
     # Number of characters in an closing block comment.
     len_closing_block_comment_delim = len(comment_delim_info[2])
 
     if group == _GROUP.inline_comment:
         # .. _COBOL special case:
@@ -1000,15 +989,14 @@
 def _remove_beginning_comment_delim(
     # Either the number of characters in the beginning delimiter, or a tuple of
     # strings which give all valid beginning comment delimiters.
     beginning_comment_delim_seq,
     # The string which start with the delimiter to be removed.
     string,
 ):
-
     # Loop through all delimiters.
     for bcd in beginning_comment_delim_seq:
         # If we find one at the beginning of the string, strip it off.
         if string.startswith(bcd):
             return string[len(bcd) :]
 
     # Not found -- panic.
@@ -1024,15 +1012,14 @@
     # that will be interpreted by reST.
     is_block_rest_comment,
     # See comment_delim_info_.
     comment_delim_info,
     # See lexer_.
     lexer,
 ):
-
     # See if there is any _GROUP.other in this line. If so, it's not a reST
     # comment.
     group_tuple, ws_len_tuple, string_tuple = list(zip(*line_list))
     if _GROUP.other in group_tuple:
         return False
     # If there's no comments (meaning the entire line is whitespace), it's not a
     # reST comment.
```

### Comparing `CodeChat-1.9.2/CodeChat/__init__.py` & `CodeChat-1.9.3/CodeChat/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 #   "ReST" -> "HTML" [label="docutils.publish_string\lSphinx\l"]
 #   "HTML" -> "ReST" [label="html_to_rest"]
 #
 #
 # Give the version number, which is read by `../setup.py` during packaging.
 # This is chosen following the `version convention
 # <http://packaging.python.org/en/latest/tutorial.html#version>`_.
-__version__ = "1.9.2"
+__version__ = "1.9.3"
```

### Comparing `CodeChat-1.9.2/CodeChat/css/CodeChat.css` & `CodeChat-1.9.3/CodeChat/css/CodeChat.css`

 * *Files identical despite different names*

### Comparing `CodeChat-1.9.2/CodeChat/css/CodeChat_sphinx_rtd_theme.css` & `CodeChat-1.9.3/CodeChat/css/CodeChat_sphinx_rtd_theme.css`

 * *Files identical despite different names*

### Comparing `CodeChat-1.9.2/CodeChat/css/docutils.css` & `CodeChat-1.9.3/CodeChat/css/docutils.css`

 * *Files identical despite different names*

### Comparing `CodeChat-1.9.2/CodeChat/mdbook_CodeChat.py` & `CodeChat-1.9.3/CodeChat/mdbook_CodeChat.py`

 * *Files identical despite different names*

### Comparing `CodeChat-1.9.2/CodeChat.egg-info/PKG-INFO` & `CodeChat-1.9.3/CodeChat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeChat
-Version: 1.9.2
+Version: 1.9.3
 Summary: The CodeChat System for software documentation
 Home-page: http://codechat.readthedocs.io/en/latest/
 Author: Bryan A. Jones
 Author-email: bjones@ece.msstate.edu
 License: GPLv3+
 Keywords: literate programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `CodeChat-1.9.2/CodeChat.egg-info/SOURCES.txt` & `CodeChat-1.9.3/CodeChat.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 CodeChat.egg-info/SOURCES.txt
 CodeChat.egg-info/dependency_links.txt
 CodeChat.egg-info/entry_points.txt
 CodeChat.egg-info/requires.txt
 CodeChat.egg-info/top_level.txt
 CodeChat/css/CodeChat.css
 CodeChat/css/CodeChat_sphinx_rtd_theme.css
+CodeChat/css/__init__.py
 CodeChat/css/docutils.css
```

### Comparing `CodeChat-1.9.2/MANIFEST.in` & `CodeChat-1.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `CodeChat-1.9.2/PKG-INFO` & `CodeChat-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeChat
-Version: 1.9.2
+Version: 1.9.3
 Summary: The CodeChat System for software documentation
 Home-page: http://codechat.readthedocs.io/en/latest/
 Author: Bryan A. Jones
 Author-email: bjones@ece.msstate.edu
 License: GPLv3+
 Keywords: literate programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `CodeChat-1.9.2/README.rst` & `CodeChat-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `CodeChat-1.9.2/pyproject.toml` & `CodeChat-1.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CodeChat-1.9.2/setup.py` & `CodeChat-1.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 # ==========
 # Create a source distribution, a built distribution, then upload both to
 # `CodeChat at PyPI <https://pypi.python.org/pypi/CodeChat>`_:
 #
 # .. code-block:: console
 #   :linenos:
 #
-#   python -m pip install -U pip setuptools wheel twine
-#   python setup.py sdist bdist_wheel
+#   python -m pip install -U pip setuptools wheel twine build
+#   python -m build
 #   python -m twine upload dist/*
 #
 # To create an RPM, first manually edit the ``name=`` setting to add a ``python3-`` prefix and lowercase the name (e.g. ``name=python3-codechat``, not ``name=python3-CodeChat``). Then, use (on an RPM-based Linux distribution):
 #
 # .. code-block:: console
 #   :linenos:
 #
@@ -158,15 +158,15 @@
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Topic :: Software Development :: Documentation",
         "Topic :: Text Processing :: Markup",
     ],
     keywords="literate programming",
-    packages=["CodeChat"],
+    packages=["CodeChat", "CodeChat.css"],
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=(
         [
             # Note: I don't include Sphinx in this list: while :doc:`CodeToRest.py
```

