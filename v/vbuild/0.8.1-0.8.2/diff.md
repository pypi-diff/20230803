# Comparing `tmp/vbuild-0.8.1.tar.gz` & `tmp/vbuild-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbuild-0.8.1.tar", last modified: Sat Aug 24 10:55:24 2019, max compression
+gzip compressed data, was "vbuild-0.8.2.tar", max compression
```

## Comparing `vbuild-0.8.1.tar` & `vbuild-0.8.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1065 2018-09-21 16:26:15.017863 vbuild-0.8.1/LICENSE
--rw-r--r--   0        0        0     3689 2018-10-22 15:48:07.564878 vbuild-0.8.1/README.md
--rw-r--r--   0        0        0     1100 2019-08-24 10:55:15.769932 vbuild-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    18708 2019-08-24 10:54:21.616670 vbuild-0.8.1/vbuild/__init__.py
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 vbuild-0.8.1/setup.py
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 vbuild-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-03 09:26:18.134218 vbuild-0.8.2/LICENSE
+-rw-r--r--   0        0        0     3689 2023-08-03 09:26:18.134218 vbuild-0.8.2/README.md
+-rw-r--r--   0        0        0     1115 2023-08-03 09:26:18.930227 vbuild-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    18703 2023-08-03 09:26:18.930227 vbuild-0.8.2/vbuild/__init__.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 vbuild-0.8.2/PKG-INFO
```

### Comparing `vbuild-0.8.1/LICENSE` & `vbuild-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vbuild-0.8.1/README.md` & `vbuild-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `vbuild-0.8.1/pyproject.toml` & `vbuild-0.8.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vbuild"
-version = "0.8.1"
+version = "0.8.2" # auto-updated
 description = "A simple module to extract html/script/style from a vuejs '.vue' file (can minimize/es2015 compliant js) ... just py2 or py3, NO nodejs !"
 authors = ["manatlan <manatlan@gmail.com>"]
 #include = ["LICENSE"]
 readme = 'README.md'
 keywords=['vuejs', 'vue', 'html', 'javascript', 'style', 'minimize', 'es2015']
 homepage = "https://github.com/manatlan/vbuild"
 repository = "https://github.com/manatlan/vbuild"
```

### Comparing `vbuild-0.8.1/vbuild/__init__.py` & `vbuild-0.8.2/vbuild/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # #############################################################################
 #    Copyright (C) 2018 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/vbuild
 # #############################################################################
-__version__ = "0.8.1"  # py2.7 & py3.5 !!!!
+__version__ = "0.8.2" # auto-updated
 
 import re, os, json, glob, itertools, traceback, subprocess, pkgutil
 
 try:
     from HTMLParser import HTMLParser
     import urllib2 as urlrequest
     import urllib as urlparse
@@ -223,16 +223,16 @@
         block = css[p1:p2]
         mediadef = block[: block.find("{")].strip()
         mediacss = block[block.find("{") + 1 : block.rfind("}")].strip()
         css = css.replace(block, "")
         medias.append((mediadef, mkPrefixCss(mediacss, prefix)))
 
     lines = []
-    css = re.sub(re.compile("/\*.*?\*/", re.DOTALL), "", css)
-    css = re.sub(re.compile("[ \t\n]+", re.DOTALL), " ", css)
+    css = re.sub(re.compile(r"/\*.*?\*/", re.DOTALL), "", css)
+    css = re.sub(re.compile(r"[ \t\n]+", re.DOTALL), " ", css)
     for rule in re.findall(r"[^}]+{[^}]+}", css):
         sels, decs = rule.split("{", 1)
         if prefix:
             l = [
                 (prefix + " " + i.replace(":scope", "").strip()).strip()
                 for i in sels.split(",")
             ]
```

### Comparing `vbuild-0.8.1/setup.py` & `vbuild-0.8.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,111 @@
-# -*- coding: utf-8 -*-
-from distutils.core import setup
+Metadata-Version: 2.1
+Name: vbuild
+Version: 0.8.2
+Summary: A simple module to extract html/script/style from a vuejs '.vue' file (can minimize/es2015 compliant js) ... just py2 or py3, NO nodejs !
+Home-page: https://github.com/manatlan/vbuild
+License: MIT
+Keywords: vuejs,vue,html,javascript,style,minimize,es2015
+Author: manatlan
+Author-email: manatlan@gmail.com
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: pscript (>=0.7.0,<0.8.0)
+Project-URL: Documentation, https://github.com/manatlan/vbuild
+Project-URL: Repository, https://github.com/manatlan/vbuild
+Description-Content-Type: text/markdown
 
-packages = \
-['vbuild']
+# vbuild
 
-package_data = \
-{'': ['*']}
+"Compile" your [VueJS](https://vuejs.org/) components (*.vue) to standalone html/js/css ... python only, **no need of nodejs**. And you can use [python components](https://github.com/manatlan/vbuild/blob/master/doc/PyComponent.md) with **vbuild**, in your vue/sfc files !!!
 
-install_requires = \
-['pscript>=0.7.0,<0.8.0']
-
-setup_kwargs = {
-    'name': 'vbuild',
-    'version': '0.8.1',
-    'description': "A simple module to extract html/script/style from a vuejs '.vue' file (can minimize/es2015 compliant js) ... just py2 or py3, NO nodejs !",
-    'long_description': '# vbuild\n\n"Compile" your [VueJS](https://vuejs.org/) components (*.vue) to standalone html/js/css ... python only, **no need of nodejs**. And you can use [python components](https://github.com/manatlan/vbuild/blob/master/doc/PyComponent.md) with **vbuild**, in your vue/sfc files !!!\n\nIt\'s just an utility to [generate](https://github.com/manatlan/vbuild/blob/master/doc/generate.md) HTML(template), SCRIPT and STYLE from a [VUE/SFC component]((https://fr.vuejs.org/v2/guide/single-file-components.html)) (*.vue). It won\'t replace webpack/nodejs/vue-cli, it fills the _"Sometimes you have to work with the tools you have, not the ones you want."_ gap.\n\n[DEMO](https://manatlan.alwaysdata.net/vbuild/)\n\n[Available on pypi](https://pypi.org/project/vbuild/)\n\n[Changelog](https://github.com/manatlan/vbuild/blob/master/changelog.md)\n\n## Features\n\n * **NO node-js stack**, only pure python (py2 or py3 compliant)\n * Ability to use [python components](https://github.com/manatlan/vbuild/blob/master/doc/PyComponent.md)\n * Components can be styled with [SASS or LESS ccs-pre-processors](https://github.com/manatlan/vbuild/blob/master/doc/CssPreProcess.md) !\n * Provide a [JS-minifier (ES5 compliant JS, via closure)](https://github.com/manatlan/vbuild/blob/master/doc/minimize.md)\n * Ability to [post process stuff](https://github.com/manatlan/vbuild/blob/master/doc/PostProcess.md), with your own processors\n * Respect [VueJs specs](https://vue-loader.vuejs.org/spec.html) (at least one template tag, many style (scoped or not) tags)\n * `templates` are converted to a `<script type="text/x-template" id="XXX"></script>` (not converted to JS)\n * Unittested (coverage 100%)\n * no import/from ! \n \n\n```python\nimport vbuild\n\nc=vbuild.render("mycompo.vue")\n#c=vbuild.render("vues/*.vue")\n#c=vbuild.render( "c1.vue", "c2.vue" )\n#c=vbuild.render( "c1.vue", "vues/*.vue" )\n\nprint( c.html )\nprint( c.script )\nprint( c.style )\n\n#or \n\nprint( c ) # all stuff in html tags\n\n```\n\n## Main Goal\n\nIts main purpose is to let you use components (.vue files) in your vuejs app, without a full nodejs stack. It\'s up to you to create your generator, to extract the things, and create your "index.html" file. It\'s a 4 lines of python code; example:\n\n```python\nimport vbuild\nbuf=readYourTemplate("index.tpl") # should contains a tag "<!-- HERE -->" that would be substituted\nbuf=buf.replace("<!-- HERE -->",str( vbuild.render( "vues/*.vue" ) ) )\nwriteYourTemplate("index.html",buf)\n```\n\n([a real example](https://github.com/manatlan/wuy/tree/master/examples/vueapp) of rendering vue/sfc components, using **vbuild** and the marvelous [wuy](https://github.com/manatlan/wuy))\n\n\n## Vue/sfc component compatibility\n\nAll classical JS vue/sfc components are compatibles. But now, you can use [python component](https://github.com/manatlan/vbuild/blob/master/doc/PyComponent.md) too. \n\nHere is, side by side, the same component (in js, and in python):\n\n<image src="https://raw.githubusercontent.com/manatlan/vbuild/master/doc/vs.png"/>\n\n## To use the full features of vbuild\n\nIf you want to use the full features, you\'ll need to install the optionnal\'s libs.\n\n```\nsudo pip install pyscss lesscpy closure\n```\n\nAll theses libs works with py2 and/or py3, and you could use the [css-pre-processors SASS and LESS](https://github.com/manatlan/vbuild/blob/master/doc/CssPreProcess.md), and [closure to minify js](https://github.com/manatlan/vbuild/blob/master/doc/minimize.md).\n\n## TODO\n\n * more utilities\n * more rock solid version\n * and docs !\n * add pyscss lesscpy closure to pip setup.py (optionnal\'s modules)\n * see the [TODO list for python components too](https://github.com/manatlan/vbuild/blob/master/doc/PyComponent.md)\n\n',
-    'author': 'manatlan',
-    'author_email': 'manatlan@gmail.com',
-    'url': 'https://github.com/manatlan/vbuild',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
-}
+It's just an utility to [generate](https://github.com/manatlan/vbuild/blob/master/doc/generate.md) HTML(template), SCRIPT and STYLE from a [VUE/SFC component]((https://fr.vuejs.org/v2/guide/single-file-components.html)) (*.vue). It won't replace webpack/nodejs/vue-cli, it fills the _"Sometimes you have to work with the tools you have, not the ones you want."_ gap.
+
+[DEMO](https://manatlan.alwaysdata.net/vbuild/)
+
+[Available on pypi](https://pypi.org/project/vbuild/)
+
+[Changelog](https://github.com/manatlan/vbuild/blob/master/changelog.md)
+
+## Features
+
+ * **NO node-js stack**, only pure python (py2 or py3 compliant)
+ * Ability to use [python components](https://github.com/manatlan/vbuild/blob/master/doc/PyComponent.md)
+ * Components can be styled with [SASS or LESS ccs-pre-processors](https://github.com/manatlan/vbuild/blob/master/doc/CssPreProcess.md) !
+ * Provide a [JS-minifier (ES5 compliant JS, via closure)](https://github.com/manatlan/vbuild/blob/master/doc/minimize.md)
+ * Ability to [post process stuff](https://github.com/manatlan/vbuild/blob/master/doc/PostProcess.md), with your own processors
+ * Respect [VueJs specs](https://vue-loader.vuejs.org/spec.html) (at least one template tag, many style (scoped or not) tags)
+ * `templates` are converted to a `<script type="text/x-template" id="XXX"></script>` (not converted to JS)
+ * Unittested (coverage 100%)
+ * no import/from ! 
+ 
+
+```python
+import vbuild
+
+c=vbuild.render("mycompo.vue")
+#c=vbuild.render("vues/*.vue")
+#c=vbuild.render( "c1.vue", "c2.vue" )
+#c=vbuild.render( "c1.vue", "vues/*.vue" )
+
+print( c.html )
+print( c.script )
+print( c.style )
+
+#or 
+
+print( c ) # all stuff in html tags
+
+```
+
+## Main Goal
+
+Its main purpose is to let you use components (.vue files) in your vuejs app, without a full nodejs stack. It's up to you to create your generator, to extract the things, and create your "index.html" file. It's a 4 lines of python code; example:
+
+```python
+import vbuild
+buf=readYourTemplate("index.tpl") # should contains a tag "<!-- HERE -->" that would be substituted
+buf=buf.replace("<!-- HERE -->",str( vbuild.render( "vues/*.vue" ) ) )
+writeYourTemplate("index.html",buf)
+```
+
+([a real example](https://github.com/manatlan/wuy/tree/master/examples/vueapp) of rendering vue/sfc components, using **vbuild** and the marvelous [wuy](https://github.com/manatlan/wuy))
+
+
+## Vue/sfc component compatibility
+
+All classical JS vue/sfc components are compatibles. But now, you can use [python component](https://github.com/manatlan/vbuild/blob/master/doc/PyComponent.md) too. 
+
+Here is, side by side, the same component (in js, and in python):
+
+<image src="https://raw.githubusercontent.com/manatlan/vbuild/master/doc/vs.png"/>
+
+## To use the full features of vbuild
+
+If you want to use the full features, you'll need to install the optionnal's libs.
+
+```
+sudo pip install pyscss lesscpy closure
+```
+
+All theses libs works with py2 and/or py3, and you could use the [css-pre-processors SASS and LESS](https://github.com/manatlan/vbuild/blob/master/doc/CssPreProcess.md), and [closure to minify js](https://github.com/manatlan/vbuild/blob/master/doc/minimize.md).
+
+## TODO
+
+ * more utilities
+ * more rock solid version
+ * and docs !
+ * add pyscss lesscpy closure to pip setup.py (optionnal's modules)
+ * see the [TODO list for python components too](https://github.com/manatlan/vbuild/blob/master/doc/PyComponent.md)
 
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,59 +1,64 @@
-# -*- coding: utf-8 -*- from distutils.core import setup packages = \
-['vbuild'] package_data = \ {'': ['*']} install_requires = \
-['pscript>=0.7.0,<0.8.0'] setup_kwargs = { 'name': 'vbuild', 'version':
-'0.8.1', 'description': "A simple module to extract html/script/style from a
-vuejs '.vue' file (can minimize/es2015 compliant js) ... just py2 or py3, NO
-nodejs !", 'long_description': '# vbuild\n\n"Compile" your [VueJS](https://
-vuejs.org/) components (*.vue) to standalone html/js/css ... python only, **no
-need of nodejs**. And you can use [python components](https://github.com/
-manatlan/vbuild/blob/master/doc/PyComponent.md) with **vbuild**, in your vue/
-sfc files !!!\n\nIt\'s just an utility to [generate](https://github.com/
-manatlan/vbuild/blob/master/doc/generate.md) HTML(template), SCRIPT and STYLE
-from a [VUE/SFC component]((https://fr.vuejs.org/v2/guide/single-file-
-components.html)) (*.vue). It won\'t replace webpack/nodejs/vue-cli, it fills
-the _"Sometimes you have to work with the tools you have, not the ones you
-want."_ gap.\n\n[DEMO](https://manatlan.alwaysdata.net/vbuild/)\n\n[Available
-on pypi](https://pypi.org/project/vbuild/)\n\n[Changelog](https://github.com/
-manatlan/vbuild/blob/master/changelog.md)\n\n## Features\n\n * **NO node-js
-stack**, only pure python (py2 or py3 compliant)\n * Ability to use [python
-components](https://github.com/manatlan/vbuild/blob/master/doc/
-PyComponent.md)\n * Components can be styled with [SASS or LESS ccs-pre-
-processors](https://github.com/manatlan/vbuild/blob/master/doc/
-CssPreProcess.md) !\n * Provide a [JS-minifier (ES5 compliant JS, via closure)]
-(https://github.com/manatlan/vbuild/blob/master/doc/minimize.md)\n * Ability to
+Metadata-Version: 2.1 Name: vbuild Version: 0.8.2 Summary: A simple module to
+extract html/script/style from a vuejs '.vue' file (can minimize/es2015
+compliant js) ... just py2 or py3, NO nodejs ! Home-page: https://github.com/
+manatlan/vbuild License: MIT Keywords:
+vuejs,vue,html,javascript,style,minimize,es2015 Author: manatlan Author-email:
+manatlan@gmail.com Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*,
+!=3.4.*, !=3.5.* Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 2 Classifier: Programming Language :: Python
+:: 2.7 Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Software Development :: Build Tools Classifier: Topic :: Software Development
+:: Libraries :: Python Modules Requires-Dist: pscript (>=0.7.0,<0.8.0) Project-
+URL: Documentation, https://github.com/manatlan/vbuild Project-URL: Repository,
+https://github.com/manatlan/vbuild Description-Content-Type: text/markdown #
+vbuild "Compile" your [VueJS](https://vuejs.org/) components (*.vue) to
+standalone html/js/css ... python only, **no need of nodejs**. And you can use
+[python components](https://github.com/manatlan/vbuild/blob/master/doc/
+PyComponent.md) with **vbuild**, in your vue/sfc files !!! It's just an utility
+to [generate](https://github.com/manatlan/vbuild/blob/master/doc/generate.md)
+HTML(template), SCRIPT and STYLE from a [VUE/SFC component]((https://
+fr.vuejs.org/v2/guide/single-file-components.html)) (*.vue). It won't replace
+webpack/nodejs/vue-cli, it fills the _"Sometimes you have to work with the
+tools you have, not the ones you want."_ gap. [DEMO](https://
+manatlan.alwaysdata.net/vbuild/) [Available on pypi](https://pypi.org/project/
+vbuild/) [Changelog](https://github.com/manatlan/vbuild/blob/master/
+changelog.md) ## Features * **NO node-js stack**, only pure python (py2 or py3
+compliant) * Ability to use [python components](https://github.com/manatlan/
+vbuild/blob/master/doc/PyComponent.md) * Components can be styled with [SASS or
+LESS ccs-pre-processors](https://github.com/manatlan/vbuild/blob/master/doc/
+CssPreProcess.md) ! * Provide a [JS-minifier (ES5 compliant JS, via closure)]
+(https://github.com/manatlan/vbuild/blob/master/doc/minimize.md) * Ability to
 [post process stuff](https://github.com/manatlan/vbuild/blob/master/doc/
-PostProcess.md), with your own processors\n * Respect [VueJs specs](https://
-vue-loader.vuejs.org/spec.html) (at least one template tag, many style (scoped
-or not) tags)\n * `templates` are converted to a `
-` (not converted to JS)\n * Unittested (coverage 100%)\n * no import/from ! \n
-\n\n```python\nimport vbuild\n\nc=vbuild.render
-("mycompo.vue")\n#c=vbuild.render("vues/*.vue")\n#c=vbuild.render( "c1.vue",
-"c2.vue" )\n#c=vbuild.render( "c1.vue", "vues/*.vue" )\n\nprint( c.html
-)\nprint( c.script )\nprint( c.style )\n\n#or \n\nprint( c ) # all stuff in
-html tags\n\n```\n\n## Main Goal\n\nIts main purpose is to let you use
-components (.vue files) in your vuejs app, without a full nodejs stack. It\'s
-up to you to create your generator, to extract the things, and create your
-"index.html" file. It\'s a 4 lines of python code; example:
-\n\n```python\nimport vbuild\nbuf=readYourTemplate("index.tpl") # should
-contains a tag "" that would be substituted\nbuf=buf.replace("",str
-( vbuild.render( "vues/*.vue" ) ) )\nwriteYourTemplate
-("index.html",buf)\n```\n\n([a real example](https://github.com/manatlan/wuy/
-tree/master/examples/vueapp) of rendering vue/sfc components, using **vbuild**
-and the marvelous [wuy](https://github.com/manatlan/wuy))\n\n\n## Vue/sfc
-component compatibility\n\nAll classical JS vue/sfc components are compatibles.
-But now, you can use [python component](https://github.com/manatlan/vbuild/
-blob/master/doc/PyComponent.md) too. \n\nHere is, side by side, the same
-component (in js, and in python):\n\n\n\n## To use the full features of
-vbuild\n\nIf you want to use the full features, you\'ll need to install the
-optionnal\'s libs.\n\n```\nsudo pip install pyscss lesscpy closure\n```\n\nAll
-theses libs works with py2 and/or py3, and you could use the [css-pre-
-processors SASS and LESS](https://github.com/manatlan/vbuild/blob/master/doc/
-CssPreProcess.md), and [closure to minify js](https://github.com/manatlan/
-vbuild/blob/master/doc/minimize.md).\n\n## TODO\n\n * more utilities\n * more
-rock solid version\n * and docs !\n * add pyscss lesscpy closure to pip
-setup.py (optionnal\'s modules)\n * see the [TODO list for python components
-too](https://github.com/manatlan/vbuild/blob/master/doc/PyComponent.md)\n\n',
-'author': 'manatlan', 'author_email': 'manatlan@gmail.com', 'url': 'https://
-github.com/manatlan/vbuild', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'python_requires': '>=2.7,
-!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*', } setup(**setup_kwargs)
+PostProcess.md), with your own processors * Respect [VueJs specs](https://vue-
+loader.vuejs.org/spec.html) (at least one template tag, many style (scoped or
+not) tags) * `templates` are converted to a `
+` (not converted to JS) * Unittested (coverage 100%) * no import/from !
+```python import vbuild c=vbuild.render("mycompo.vue") #c=vbuild.render("vues/
+*.vue") #c=vbuild.render( "c1.vue", "c2.vue" ) #c=vbuild.render( "c1.vue",
+"vues/*.vue" ) print( c.html ) print( c.script ) print( c.style ) #or print( c
+) # all stuff in html tags ``` ## Main Goal Its main purpose is to let you use
+components (.vue files) in your vuejs app, without a full nodejs stack. It's up
+to you to create your generator, to extract the things, and create your
+"index.html" file. It's a 4 lines of python code; example: ```python import
+vbuild buf=readYourTemplate("index.tpl") # should contains a tag "" that would
+be substituted buf=buf.replace("",str( vbuild.render( "vues/*.vue" ) ) )
+writeYourTemplate("index.html",buf) ``` ([a real example](https://github.com/
+manatlan/wuy/tree/master/examples/vueapp) of rendering vue/sfc components,
+using **vbuild** and the marvelous [wuy](https://github.com/manatlan/wuy)) ##
+Vue/sfc component compatibility All classical JS vue/sfc components are
+compatibles. But now, you can use [python component](https://github.com/
+manatlan/vbuild/blob/master/doc/PyComponent.md) too. Here is, side by side, the
+same component (in js, and in python):  ## To use the full features of vbuild
+If you want to use the full features, you'll need to install the optionnal's
+libs. ``` sudo pip install pyscss lesscpy closure ``` All theses libs works
+with py2 and/or py3, and you could use the [css-pre-processors SASS and LESS]
+(https://github.com/manatlan/vbuild/blob/master/doc/CssPreProcess.md), and
+[closure to minify js](https://github.com/manatlan/vbuild/blob/master/doc/
+minimize.md). ## TODO * more utilities * more rock solid version * and docs ! *
+add pyscss lesscpy closure to pip setup.py (optionnal's modules) * see the
+[TODO list for python components too](https://github.com/manatlan/vbuild/blob/
+master/doc/PyComponent.md)
```

