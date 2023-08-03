# Comparing `tmp/sphinx_fasvg-1.0.0.tar.gz` & `tmp/sphinx_fasvg-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_fasvg-1.0.0.tar", last modified: Sun Jun  6 16:49:02 2021, max compression
+gzip compressed data, was "sphinx_fasvg-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_fasvg-1.0.0.tar` & `sphinx_fasvg-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,10 @@
-drwxr-xr-x   0 kujiu     (1000) users      (100)        0 2021-06-06 16:49:02.111714 sphinx_fasvg-1.0.0/
--rw-r--r--   0 kujiu     (1000) users      (100)    13827 2020-05-19 13:35:17.000000 sphinx_fasvg-1.0.0/LICENSE
--rw-r--r--   0 kujiu     (1000) users      (100)    15282 2020-05-19 13:35:17.000000 sphinx_fasvg-1.0.0/LICENSE-de
--rw-r--r--   0 kujiu     (1000) users      (100)    15898 2020-05-19 13:35:17.000000 sphinx_fasvg-1.0.0/LICENSE-fr
--rw-r--r--   0 kujiu     (1000) users      (100)    15887 2020-05-19 13:35:17.000000 sphinx_fasvg-1.0.0/LICENSE-nl
--rw-r--r--   0 kujiu     (1000) users      (100)     2837 2021-06-06 16:49:02.111714 sphinx_fasvg-1.0.0/PKG-INFO
--rw-r--r--   0 kujiu     (1000) users      (100)     1179 2021-06-06 16:17:02.000000 sphinx_fasvg-1.0.0/README.rst
--rw-r--r--   0 kujiu     (1000) users      (100)      142 2021-06-06 16:49:02.111714 sphinx_fasvg-1.0.0/setup.cfg
--rw-r--r--   0 kujiu     (1000) users      (100)     1628 2021-06-06 16:15:36.000000 sphinx_fasvg-1.0.0/setup.py
-drwxr-xr-x   0 kujiu     (1000) users      (100)        0 2021-06-06 16:49:02.111714 sphinx_fasvg-1.0.0/sphinx_fasvg/
--rw-r--r--   0 kujiu     (1000) users      (100)     7963 2021-06-06 16:48:39.000000 sphinx_fasvg-1.0.0/sphinx_fasvg/__init__.py
-drwxr-xr-x   0 kujiu     (1000) users      (100)        0 2021-06-06 16:49:02.111714 sphinx_fasvg-1.0.0/sphinx_fasvg.egg-info/
--rw-r--r--   0 kujiu     (1000) users      (100)     2837 2021-06-06 16:49:02.000000 sphinx_fasvg-1.0.0/sphinx_fasvg.egg-info/PKG-INFO
--rw-r--r--   0 kujiu     (1000) users      (100)      313 2021-06-06 16:49:02.000000 sphinx_fasvg-1.0.0/sphinx_fasvg.egg-info/SOURCES.txt
--rw-r--r--   0 kujiu     (1000) users      (100)        1 2021-06-06 16:49:02.000000 sphinx_fasvg-1.0.0/sphinx_fasvg.egg-info/dependency_links.txt
--rw-r--r--   0 kujiu     (1000) users      (100)       61 2021-06-06 16:49:02.000000 sphinx_fasvg-1.0.0/sphinx_fasvg.egg-info/entry_points.txt
--rw-r--r--   0 kujiu     (1000) users      (100)       14 2021-06-06 16:49:02.000000 sphinx_fasvg-1.0.0/sphinx_fasvg.egg-info/requires.txt
--rw-r--r--   0 kujiu     (1000) users      (100)       13 2021-06-06 16:49:02.000000 sphinx_fasvg-1.0.0/sphinx_fasvg.egg-info/top_level.txt
+-rw-r--r--   0        0        0       59 2020-05-19 13:35:17.895795 sphinx_fasvg-2.0.0/.gitignore
+-rw-r--r--   0        0        0      429 2023-08-01 21:02:05.436288 sphinx_fasvg-2.0.0/CHANGES
+-rw-r--r--   0        0        0    13827 2020-05-19 13:35:17.895795 sphinx_fasvg-2.0.0/LICENSE
+-rw-r--r--   0        0        0    15282 2020-05-19 13:35:17.895795 sphinx_fasvg-2.0.0/LICENSE-de
+-rw-r--r--   0        0        0    15898 2020-05-19 13:35:17.899795 sphinx_fasvg-2.0.0/LICENSE-fr
+-rw-r--r--   0        0        0    15887 2020-05-19 13:35:17.899795 sphinx_fasvg-2.0.0/LICENSE-nl
+-rw-r--r--   0        0        0     1179 2021-06-06 16:17:02.890465 sphinx_fasvg-2.0.0/README.rst
+-rw-r--r--   0        0        0     2358 2023-08-01 21:40:37.012050 sphinx_fasvg-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9729 2023-08-03 13:30:30.370225 sphinx_fasvg-2.0.0/sphinx_fasvg/__init__.py
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 sphinx_fasvg-2.0.0/PKG-INFO
```

### Comparing `sphinx_fasvg-1.0.0/LICENSE` & `sphinx_fasvg-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_fasvg-1.0.0/LICENSE-de` & `sphinx_fasvg-2.0.0/LICENSE-de`

 * *Files identical despite different names*

### Comparing `sphinx_fasvg-1.0.0/LICENSE-fr` & `sphinx_fasvg-2.0.0/LICENSE-fr`

 * *Files identical despite different names*

### Comparing `sphinx_fasvg-1.0.0/LICENSE-nl` & `sphinx_fasvg-2.0.0/LICENSE-nl`

 * *Files identical despite different names*

### Comparing `sphinx_fasvg-1.0.0/README.rst` & `sphinx_fasvg-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_fasvg-1.0.0/sphinx_fasvg/__init__.py` & `sphinx_fasvg-2.0.0/sphinx_fasvg/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+# pylint:disable=invalid-name,unused-argument,too-many-arguments
+
 """
 Use fontawesome icons
 """
 
 import re
 import uuid
 
 from docutils import nodes
 from docutils.parsers.rst import Directive
-import docutils.parsers.rst.directives as directives
+from docutils.parsers.rst import directives
 
 from sphinx.writers.html import HTMLTranslator
 from sphinx.writers.latex import LaTeXTranslator
 from sphinx.writers.texinfo import TexinfoTranslator
 from sphinx.writers.text import TextTranslator
 from sphinx.writers.manpage import ManualPageTranslator
 from sphinx.util.osutil import relative_uri
 
-__version_info__ = (1, 0, 0)
+__version_info__ = (2, 0, 0)
 __version__ = '.'.join([str(val) for val in __version_info__])
 
 
 class fa(nodes.General, nodes.Inline, nodes.Element):
-    pass
+    """Generic node for FontAwesome"""
 
 
 class falink(nodes.General, nodes.Inline, nodes.Element):
-    pass
+    """Generic link node for FontAwesome"""
 
 
 def append_fa_image(self: HTMLTranslator, node: fa or falink) -> None:
+    """Add image to node"""
     path = {
         'brands': self.builder.config.fa_brands_path,
         'regular': self.builder.config.fa_regular_path,
         'solid': self.builder.config.fa_solid_path,
     }[node['iconset']]
 
     path = relative_uri(
@@ -45,171 +48,223 @@
 
     label_uid = uuid.uuid4()
     title = None
     options = 'role="img"'
     options += ' xmlns="http://www.w3.org/2000/svg"'
     options += ' xmlns:xlink="http://www.w3.org/1999/xlink"'
     if node.get('alt', None):
-        options += ' aria-labelledby="fa_%s"' % label_uid
-        title = '<title id="%s">%s</title>' % (label_uid, node['alt'])
+        options += f' aria-labelledby="fa_{label_uid}"'
+        title = f'<title id="{label_uid}">{node["alt"]}</title>'
     else:
         options += ' aria-hidden="true" xlink:title=""'
 
     if node.get('html_id', None):
-        options += ' id="%s"' % node['html_id']
+        options += f' id={node["html_id"]}'
 
-    options += ' class="fasvg %s"' % (node.get('html_class', '') or '')
+    options += f' class="fasvg {node.get("html_class", "") or ""}"'
 
     self.body.append(
-        '<svg %s>' % options
+        f'<svg {options}>'
     )
 
     if title:
         self.body.append(title)
 
     self.body.append(
-        '<use xlink:href="%s#%s"></use></svg>' % (path, node['icon'])
+        f'<use xlink:href="{path}#{node["icon"]}"></use></svg>'
     )
 
 
 def html_visit_fa(self: HTMLTranslator, node: fa) -> None:
+    """Rendering FA node in HTML"""
     append_fa_image(self, node)
     raise nodes.SkipNode
 
 
 def latex_visit_fa(self: LaTeXTranslator, node: fa) -> None:
+    """Rendering FA node in LaTeX"""
     if 'alt' in node.attributes:
-        self.body.append('[%s]' % node['alt'])
+        self.body.append(f'[{node["alt"]}]')
     raise nodes.SkipNode
 
 
 def texinfo_visit_fa(self: TexinfoTranslator, node: fa) -> None:
+    """Rendering FA node in TeXinfo"""
     if 'alt' in node.attributes:
-        self.body.append('[%s]' % node['alt'])
+        self.body.append(f'[{node["alt"]}]')
     raise nodes.SkipNode
 
 
 def text_visit_fa(self: TextTranslator, node: fa) -> None:
+    """Rendering FA node in text"""
     if 'alt' in node.attributes:
-        self.add_text('[%s]' % node['alt'])
+        self.add_text(f'[{node["alt"]}]')
     raise nodes.SkipNode
 
 
 def gemini_visit_fa(self, node: fa) -> None:
+    """Rendering FA node in Gemini"""
     if 'alt' in node.attributes:
-        self.add_text('[%s]' % node['alt'])
+        self.add_text(f'[{node["alt"]}]')
     raise nodes.SkipNode
 
 
 def man_visit_fa(self: ManualPageTranslator, node: fa) -> None:
+    """Rendering FA node in Man file"""
     if 'alt' in node.attributes:
-        self.body.append('[%s]' % node['alt'])
+        self.body.append(f'[{node["alt"]}]')
     raise nodes.SkipNode
 
 
 def create_fa_node(iconset, icon, html_id=None, html_class=None, alt=None):
+    """Create FA node"""
     node = fa()
     node['iconset'] = iconset
     node['icon'] = icon
     node['html_id'] = html_id
     node['html_class'] = html_class
     node['alt'] = alt or ''
     return node
 
 
 def html_visit_falink(self: HTMLTranslator, node: fa) -> None:
+    """Rendering FA link node in HTML"""
     self.body.append(
-        '<a class="fasvglink %s" href="%s">' %
-        (node['icon'], node['url']))
+        f'<a class="fasvglink {node["icon"]}" href="{node["url"]}">'
+    )
     append_fa_image(self, node)
 
-    self.body.append(' %s</a>' % node['text'])
+    self.body.append(f' {node["text"]}</a>')
     raise nodes.SkipNode
 
 
 def latex_visit_falink(self: LaTeXTranslator, node: fa) -> None:
-    self.body.append('\\href{%s}{%s %s}' % (
-        node['url'], node['alt'], node['text']))
+    """Rendering FA link node in LaTeX"""
+    self.body.append(
+        f'\\href{{{node["url"]}}}'
+        f'{{{node["alt"]} {node["text"]}}}'
+    )
     raise nodes.SkipNode
 
 
 def texinfo_visit_falink(self: TexinfoTranslator, node: fa) -> None:
-    self.body.append('\\href{%s}{%s %s}' % (
-        node['url'], node['alt'], node['text']))
+    """Rendering FA link node in TexInfo"""
+    self.body.append(
+        f'\\href{{{node["url"]}}}{{{node["alt"]} {node["text"]}}}'
+    )
     raise nodes.SkipNode
 
 
 def text_visit_falink(self: TextTranslator, node: fa) -> None:
-    self.add_text('%s %s <%s>' % (node['alt'], node['text'], node['url']))
+    """Rendering FA link node in text"""
+    self.add_text(
+        f'{node["alt"]} {node["text"]} <{node["url"]}>'
+    )
     raise nodes.SkipNode
 
 
 def gemini_visit_falink(self, node: fa) -> None:
+    """Rendering FA link node in Gemini"""
     self.end_block()
-    self.add_text('=> %s %s %s' % (node['alt'], node['url'], node['text']))
+    self.add_text(
+        f'=> {node["alt"]} {node["url"]} {node["text"]}'
+    )
     self.end_block()
     raise nodes.SkipNode
 
 
 def man_visit_falink(self: ManualPageTranslator, node: fa) -> None:
-    self.body.append('%s %s <%s>' % (node['text'], node['alt'], node['url']))
+    """Rendering FA link node in Man file"""
+    self.body.append(f'{node["text"]} {node["alt"]} <{node["url"]}>')
     raise nodes.SkipNode
 
 
 def create_falink_node(iconset, text):
+    """Create a new link node depending of text and iconset"""
     node = falink()
     regex = re.compile(
-        r'(?P<icon>[a-zA-Z-_]*):(?P<text>.*)'
-        + r'(?P<alt>\[.*\] *)<(?P<url>.*)>')
+        r'(?P<icon> *[a-zA-Z-_]* *):(?P<text>.*)'
+        + r'(?P<alt>\[.*\] *)?<(?P<url>.*)>')
     parsed = regex.search(text)
     node['iconset'] = iconset
-    node['icon'] = parsed.group('icon')
+    node['icon'] = parsed.group('icon').strip()
     node['url'] = parsed.group('url').strip()
     node['alt'] = (parsed.group('alt') or '').strip().strip('[]')
     node['text'] = parsed.group('text').strip()
     return node
 
 
-def fab(role, rawtext, text, lineno, inliner, options={}, content=[]):
-    regex = re.compile(r'(?P<icon>[a-zA-Z-_]*)(?P<alt>\[.*\] *)')
+def fab(role, rawtext, text, lineno, inliner, options=None, content=None):
+    """Node for FontAwesome brand icon"""
+    if not options:
+        options = {}
+    if not content:
+        content = []
+    regex = re.compile(r'(?P<icon>[a-zA-Z-_]*)(?P<alt>\[.*\] *)?')
     parsed = regex.search(text)
     alt = (parsed.group('alt') or '').strip().strip('[]')
     icon = parsed.group('icon').strip()
     return [create_fa_node('brands', icon, alt=alt)], []
 
 
-def far(role, rawtext, text, lineno, inliner, options={}, content=[]):
-    regex = re.compile(r'(?P<icon>[a-zA-Z-_]*)(?P<alt>\[.*\] *)')
+def far(role, rawtext, text, lineno, inliner, options=None, content=None):
+    """Node for FontAwesome regular icon"""
+    if not options:
+        options = {}
+    if not content:
+        content = []
+    regex = re.compile(r'(?P<icon>[a-zA-Z-_]*)(?P<alt>\[.*\] *)?')
     parsed = regex.search(text)
     alt = (parsed.group('alt') or '').strip().strip('[]')
     icon = parsed.group('icon').strip()
     return [create_fa_node('regular', icon, alt=alt)], []
 
 
-def fas(role, rawtext, text, lineno, inliner, options={}, content=[]):
-    regex = re.compile(r'(?P<icon>[a-zA-Z-_]*)(?P<alt>\[.*\] *)')
+def fas(role, rawtext, text, lineno, inliner, options=None, content=None):
+    """Node for FontAwesome solid icon"""
+    if not options:
+        options = {}
+    if not content:
+        content = []
+    regex = re.compile(r'(?P<icon>[a-zA-Z-_]*)(?P<alt>\[.*\] *)?')
     parsed = regex.search(text)
     alt = (parsed.group('alt') or '').strip().strip('[]')
     icon = parsed.group('icon').strip()
     return [create_fa_node('solid', icon, alt=alt)], []
 
 
-def fablink(role, rawtext, text, lineno, inliner, options={}, content=[]):
+def fablink(role, rawtext, text, lineno, inliner, options=None, content=None):
+    """Node for link with FontAwesome brands iconset"""
+    if not options:
+        options = {}
+    if not content:
+        content = []
     return [create_falink_node('brands', text)], []
 
 
-def farlink(role, rawtext, text, lineno, inliner, options={}, content=[]):
+def farlink(role, rawtext, text, lineno, inliner, options=None, content=None):
+    """Node for link with FontAwesome regular iconset"""
+    if not options:
+        options = {}
+    if not content:
+        content = []
     return [create_falink_node('regular', text)], []
 
 
-def faslink(role, rawtext, text, lineno, inliner, options={}, content=[]):
+def faslink(role, rawtext, text, lineno, inliner, options=None, content=None):
+    """Node for link with FontAwesome solid iconset"""
+    if not options:
+        options = {}
+    if not content:
+        content = []
     return [create_falink_node('solid', text)], []
 
 
 class FaDirective(Directive):
+    """ Main directive for FontAwesome icons """
 
     has_content = False
     required_arguments = 1
     final_argument_whitespace = True
     option_spec = {
         "class": directives.unchanged,
         "id": directives.unchanged,
@@ -225,26 +280,32 @@
             self.options['class'],
             self.options['alt']
         )
         return [node]
 
 
 class Fab(FaDirective):
+    """ Directive for FontAwesome brands iconset """
     iconset = 'brands'
 
 
 class Far(FaDirective):
+    """ Directive for FontAwesome regular iconset """
     iconset = 'regular'
 
 
 class Fas(FaDirective):
+    """ Directive for FontAwesome solid iconset """
     iconset = 'solid'
 
 
 def setup(app):
+    """
+    Setup Sphinx app
+    """
     app.add_node(
         fa,
         html=(html_visit_fa, None),
         epub=(html_visit_fa, None),
         latex=(latex_visit_fa, None),
         texinfo=(texinfo_visit_fa, None),
         text=(text_visit_fa, None),
```

