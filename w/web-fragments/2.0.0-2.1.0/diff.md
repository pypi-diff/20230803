# Comparing `tmp/web-fragments-2.0.0.tar.gz` & `tmp/web-fragments-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-fragments-2.0.0.tar", last modified: Mon Dec 13 11:58:01 2021, max compression
+gzip compressed data, was "web-fragments-2.1.0.tar", last modified: Thu Aug  3 11:01:03 2023, max compression
```

## Comparing `web-fragments-2.0.0.tar` & `web-fragments-2.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 11:58:01.580569 web-fragments-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-12-13 11:57:53.000000 web-fragments-2.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-12-13 11:57:53.000000 web-fragments-2.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-12-13 11:57:53.000000 web-fragments-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-12-13 11:57:53.000000 web-fragments-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4769 2021-12-13 11:58:01.580569 web-fragments-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2021-12-13 11:57:53.000000 web-fragments-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      621 2021-12-13 11:58:01.580569 web-fragments-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-12-13 11:57:53.000000 web-fragments-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 11:58:01.576569 web-fragments-2.0.0/web_fragments/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-12-13 11:57:53.000000 web-fragments-2.0.0/web_fragments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-12-13 11:57:53.000000 web-fragments-2.0.0/web_fragments/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 11:58:01.576569 web-fragments-2.0.0/web_fragments/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-13 11:57:53.000000 web-fragments-2.0.0/web_fragments/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-12-13 11:57:53.000000 web-fragments-2.0.0/web_fragments/examples/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      611 2021-12-13 11:57:53.000000 web-fragments-2.0.0/web_fragments/examples/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     9096 2021-12-13 11:57:53.000000 web-fragments-2.0.0/web_fragments/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 11:58:01.576569 web-fragments-2.0.0/web_fragments/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 11:58:01.576569 web-fragments-2.0.0/web_fragments/templates/web_fragments/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-12-13 11:57:53.000000 web-fragments-2.0.0/web_fragments/templates/web_fragments/standalone_fragment.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 11:58:01.580569 web-fragments-2.0.0/web_fragments/test_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      547 2021-12-13 11:57:53.000000 web-fragments-2.0.0/web_fragments/test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 11:58:01.580569 web-fragments-2.0.0/web_fragments/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     7837 2021-12-13 11:57:53.000000 web-fragments-2.0.0/web_fragments/tests/test_fragment.py
--rw-r--r--   0 runner    (1001) docker     (121)     3253 2021-12-13 11:57:53.000000 web-fragments-2.0.0/web_fragments/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2021-12-13 11:57:53.000000 web-fragments-2.0.0/web_fragments/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 11:58:01.576569 web-fragments-2.0.0/web_fragments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4769 2021-12-13 11:58:01.000000 web-fragments-2.0.0/web_fragments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      661 2021-12-13 11:58:01.000000 web-fragments-2.0.0/web_fragments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 11:58:01.000000 web-fragments-2.0.0/web_fragments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 11:58:01.000000 web-fragments-2.0.0/web_fragments.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-12-13 11:58:01.000000 web-fragments-2.0.0/web_fragments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-12-13 11:58:01.000000 web-fragments-2.0.0/web_fragments.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.412799 web-fragments-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-08-03 11:00:57.000000 web-fragments-2.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-08-03 11:00:57.000000 web-fragments-2.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-08-03 11:00:57.000000 web-fragments-2.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-08-03 11:00:57.000000 web-fragments-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-08-03 11:01:03.412799 web-fragments-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3013 2023-08-03 11:00:57.000000 web-fragments-2.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-08-03 11:01:03.412799 web-fragments-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-08-03 11:00:57.000000 web-fragments-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.408799 web-fragments-2.1.0/web_fragments/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.412799 web-fragments-2.1.0/web_fragments/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/examples/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/examples/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9010 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.408799 web-fragments-2.1.0/web_fragments/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.412799 web-fragments-2.1.0/web_fragments/templates/web_fragments/
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/templates/web_fragments/standalone_fragment.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.412799 web-fragments-2.1.0/web_fragments/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.412799 web-fragments-2.1.0/web_fragments/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     7837 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/tests/test_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.408799 web-fragments-2.1.0/web_fragments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/top_level.txt
```

### Comparing `web-fragments-2.0.0/LICENSE.txt` & `web-fragments-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `web-fragments-2.0.0/README.rst` & `web-fragments-2.1.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 web-fragments
 =============
 
 .. image:: https://img.shields.io/pypi/v/web-fragments.svg
     :target: https://pypi.python.org/pypi/web-fragments/
     :alt: PyPI
 
-.. image:: https://github.com/edx/web-fragments/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/web-fragments/actions?query=workflow%3A%22Python+CI%22
+.. image:: https://github.com/openedx/web-fragments/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/web-fragments/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. image:: http://codecov.io/github/edx/web-fragments/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/web-fragments?branch=master
     :alt: Codecov
 
 .. image:: http://web-fragments.readthedocs.io/en/latest/?badge=latest
@@ -18,15 +18,15 @@
     :alt: Documentation
 
 .. image:: https://img.shields.io/pypi/pyversions/web-fragments.svg
     :target: https://pypi.python.org/pypi/web-fragments/
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/github/license/edx/web-fragments.svg
-    :target: https://github.com/edx/web-fragments/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/web-fragments/blob/master/LICENSE.txt
     :alt: License
 
 Overview
 --------
 
 The web fragments library provides a Python and Django implementation for
 managing fragments of web pages. In particular, this library refactors the
@@ -62,20 +62,17 @@
 noted.
 
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
-Contributions are very welcome. Please read `Contributing to edX`_ for details.
+Contributions are very welcome. Please read `the Open edX Contributing Guide`_ for details.
 
-Note: Even though these guidelines were written with ``edx-platform`` in mind,
-they should be followed for Open edX code in general.
-
-.. _Contributing to edX: https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst
+.. _the Open edX Contributing Guide: https://github.com/openedx/.github/blob/master/CONTRIBUTING.md
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
```

### Comparing `web-fragments-2.0.0/setup.py` & `web-fragments-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 setup(
     name='web-fragments',
     version=VERSION,
     description="""Web fragments""",
     long_description=README + '\n\n' + CHANGELOG,
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/web-fragments',
+    url='https://github.com/openedx/web-fragments',
     packages=[
         'web_fragments',
     ],
     include_package_data=True,
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Django edx',
```

### Comparing `web-fragments-2.0.0/web_fragments/examples/views.py` & `web-fragments-2.1.0/web_fragments/examples/views.py`

 * *Files identical despite different names*

### Comparing `web-fragments-2.0.0/web_fragments/fragment.py` & `web-fragments-2.1.0/web_fragments/fragment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Python representation of a web fragment.
 """
 
 from collections import namedtuple
 
-FragmentResource = namedtuple("FragmentResource", "kind, data, mimetype, placement")  # pylint: disable=C0103
+FragmentResource = namedtuple("FragmentResource", "kind, data, mimetype, placement")
 
 JS_API_VERSION = 1
 
 
 class Fragment:
     """
     A fragment of a web page to be included on another page.
@@ -49,28 +49,28 @@
 
     def to_dict(self):
         """
         Returns the fragment in a dictionary representation.
         """
         return {
             'content': self.content,
-            'resources': [r._asdict() for r in self.resources],  # pylint: disable=W0212
+            'resources': [r._asdict() for r in self.resources],
             'js_init_fn': self.js_init_fn,
             'js_init_version': self.js_init_version,
             'json_init_args': self.json_init_args
         }
 
     @classmethod
     def from_dict(cls, pods):
         """
         Returns a new Fragment from a dictionary representation.
         """
         frag = cls()
         frag.content = pods['content']
-        frag._resources = [FragmentResource(**d) for d in pods['resources']]  # pylint: disable=protected-access
+        frag._resources = [FragmentResource(**d) for d in pods['resources']]
         frag.js_init_fn = pods['js_init_fn']
         frag.js_init_version = pods['js_init_version']
         frag.json_init_args = pods['json_init_args']
         return frag
 
     def add_content(self, content):
         """
```

### Comparing `web-fragments-2.0.0/web_fragments/test_utils/__init__.py` & `web-fragments-2.1.0/web_fragments/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `web-fragments-2.0.0/web_fragments/tests/test_fragment.py` & `web-fragments-2.1.0/web_fragments/tests/test_fragment.py`

 * *Files identical despite different names*

### Comparing `web-fragments-2.0.0/web_fragments/tests/test_views.py` & `web-fragments-2.1.0/web_fragments/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `web-fragments-2.0.0/web_fragments/views.py` & `web-fragments-2.1.0/web_fragments/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,46 +12,46 @@
 
 
 class FragmentView(View, metaclass=ABCMeta):
     """
     Base class for Django web fragment views.
     """
 
-    def get(self, request, *args, **kwargs):  # pylint: disable=unused-argument
+    def get(self, request, *args, **kwargs):
         """
         Render a fragment to HTML or return JSON describing it, based on the request.
         """
         fragment = self.render_to_fragment(request, **kwargs)
         response_format = request.GET.get('format') or request.POST.get('format') or 'html'
         if response_format == 'json' or WEB_FRAGMENT_RESPONSE_TYPE in request.META.get('HTTP_ACCEPT', 'text/html'):
             return JsonResponse(fragment.to_dict())
 
         return self.render_standalone_response(request, fragment, **kwargs)
 
-    def render_standalone_response(self, request, fragment, **kwargs):  # pylint: disable=unused-argument
+    def render_standalone_response(self, request, fragment, **kwargs):
         """
         Renders a standalone page as a response for the specified fragment.
         """
         if fragment is None:
             return HttpResponse(status=204)
 
         html = self.render_to_standalone_html(request, fragment, **kwargs)
         return HttpResponse(html)
 
-    def render_to_standalone_html(self, request, fragment, **kwargs):  # pylint: disable=unused-argument
+    def render_to_standalone_html(self, request, fragment, **kwargs):
         """
         Render the specified fragment to HTML for a standalone page.
         """
         template = get_template(STANDALONE_TEMPLATE_NAME)
         context = {
             'head_html': fragment.head_html(),
             'body_html': fragment.body_html(),
             'foot_html': fragment.foot_html(),
         }
         return template.render(context)
 
     @abstractmethod
-    def render_to_fragment(self, request, **kwargs):  # pylint: disable=unused-argument
+    def render_to_fragment(self, request, **kwargs):
         """
         Render this view to a fragment.
         """
         raise NotImplementedError()
```

### Comparing `web-fragments-2.0.0/web_fragments.egg-info/SOURCES.txt` & `web-fragments-2.1.0/web_fragments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

