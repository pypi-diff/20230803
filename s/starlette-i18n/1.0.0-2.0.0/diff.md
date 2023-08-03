# Comparing `tmp/starlette-i18n-1.0.0.tar.gz` & `tmp/starlette-i18n-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette-i18n-1.0.0.tar", last modified: Sun Aug  1 11:27:41 2021, max compression
+gzip compressed data, was "starlette-i18n-2.0.0.tar", last modified: Thu Aug  3 15:05:02 2023, max compression
```

## Comparing `starlette-i18n-1.0.0.tar` & `starlette-i18n-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-01 11:27:41.621701 starlette-i18n-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11466 2021-08-01 11:27:30.000000 starlette-i18n-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-08-01 11:27:30.000000 starlette-i18n-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3501 2021-08-01 11:27:41.621701 starlette-i18n-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2021-08-01 11:27:30.000000 starlette-i18n-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      423 2021-08-01 11:27:30.000000 starlette-i18n-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-01 11:27:41.621701 starlette-i18n-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2021-08-01 11:27:30.000000 starlette-i18n-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-01 11:27:41.621701 starlette-i18n-1.0.0/starlette_i18n/
--rw-r--r--   0 runner    (1001) docker     (121)      632 2021-08-01 11:27:30.000000 starlette-i18n-1.0.0/starlette_i18n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-08-01 11:27:30.000000 starlette-i18n-1.0.0/starlette_i18n/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2021-08-01 11:27:30.000000 starlette-i18n-1.0.0/starlette_i18n/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2021-08-01 11:27:30.000000 starlette-i18n-1.0.0/starlette_i18n/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2021-08-01 11:27:30.000000 starlette-i18n-1.0.0/starlette_i18n/i18n.py
--rw-r--r--   0 runner    (1001) docker     (121)     2496 2021-08-01 11:27:31.000000 starlette-i18n-1.0.0/starlette_i18n/locale.py
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2021-08-01 11:27:31.000000 starlette-i18n-1.0.0/starlette_i18n/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-08-01 11:27:31.000000 starlette-i18n-1.0.0/starlette_i18n/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-01 11:27:41.621701 starlette-i18n-1.0.0/starlette_i18n.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3501 2021-08-01 11:27:41.000000 starlette-i18n-1.0.0/starlette_i18n.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      489 2021-08-01 11:27:41.000000 starlette-i18n-1.0.0/starlette_i18n.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-01 11:27:41.000000 starlette-i18n-1.0.0/starlette_i18n.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-01 11:27:41.000000 starlette-i18n-1.0.0/starlette_i18n.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-08-01 11:27:41.000000 starlette-i18n-1.0.0/starlette_i18n.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-08-01 11:27:41.000000 starlette-i18n-1.0.0/starlette_i18n.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:05:02.767955 starlette-i18n-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-03 15:05:02.767955 starlette-i18n-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:05:02.767955 starlette-i18n-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:05:02.767955 starlette-i18n-2.0.0/starlette_i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/starlette_i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/starlette_i18n/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/starlette_i18n/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/starlette_i18n/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/starlette_i18n/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/starlette_i18n/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/starlette_i18n/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 15:04:51.000000 starlette-i18n-2.0.0/starlette_i18n/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:05:02.767955 starlette-i18n-2.0.0/starlette_i18n.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-03 15:05:02.000000 starlette-i18n-2.0.0/starlette_i18n.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 15:05:02.000000 starlette-i18n-2.0.0/starlette_i18n.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:05:02.000000 starlette-i18n-2.0.0/starlette_i18n.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:05:02.000000 starlette-i18n-2.0.0/starlette_i18n.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-03 15:05:02.000000 starlette-i18n-2.0.0/starlette_i18n.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 15:05:02.000000 starlette-i18n-2.0.0/starlette_i18n.egg-info/top_level.txt
```

### Comparing `starlette-i18n-1.0.0/LICENSE` & `starlette-i18n-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette-i18n-1.0.0/PKG-INFO` & `starlette-i18n-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,97 @@
 Metadata-Version: 2.1
 Name: starlette-i18n
-Version: 1.0.0
+Version: 2.0.0
 Summary: Localisation helper for starlette
 Home-page: https://github.com/bigbag/starlette-i18n
+Download-URL: https://pypi.python.org/pypi/starlette-i18n
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
-Download-URL: https://pypi.python.org/pypi/starlette-i18n
-Description: # starlette-i18n
-        
-        [![CI](https://github.com/bigbag/starlette-i18n/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-i18n/actions?query=workflow%3ACI)
-        [![codecov](https://codecov.io/gh/bigbag/starlette-i18n/branch/main/graph/badge.svg)](https://codecov.io/gh/bigbag/starlette-i18n) 
-        [![pypi](https://img.shields.io/pypi/v/starlette-i18n.svg)](https://pypi.python.org/pypi/starlette-i18n)
-        [![downloads](https://img.shields.io/pypi/dm/starlette-i18n.svg)](https://pypistats.org/packages/starlette-i18n)
-        [![versions](https://img.shields.io/pypi/pyversions/starlette-i18n.svg)](https://github.com/bigbag/starlette-i18n)
-        [![license](https://img.shields.io/github/license/bigbag/starlette-i18n.svg)](https://github.com/bigbag/starlette-i18n/blob/master/LICENSE)
-        
-        
-        **starlette-i18n** is a localisation helper for starlette.
-        
-        
-        ## Installation
-        
-        starlette-i18n is available on PyPI.
-        Use pip to install:
-        
-            $ pip install starlette-i18n
-        
-        ## Basic Usage
-        
-        ```py
-        import uvicorn
-        from starlette.applications import Starlette
-        from starlette.responses import PlainTextResponse
-        
-        from starlette_i18n import (
-            DEFAULT_LOCALE,
-            LANGUAGE_HEADER,
-            LocaleFromHeaderMiddleware,
-            load_gettext_translations,
-        )
-        from starlette_i18n import gettext_lazy as _
-        
-        BABEL_DOMAIN = "messages"
-        BABEL_LOCALES_PATH = "locales"
-        
-        
-        def init_app():
-            load_gettext_translations(directory=BABEL_LOCALES_PATH, domain=BABEL_DOMAIN)
-        
-            app_ = Starlette()
-            app_.add_middleware(
-                LocaleFromHeaderMiddleware, 
-                language_header=LANGUAGE_HEADER, 
-                default_code=DEFAULT_LOCALE
-            )
-        
-            @app_.route("/")
-            def success(request):
-                return PlainTextResponse(_("OK"), status_code=200)
-        
-            return app_
-        
-        
-        app = init_app()
-        
-        if __name__ == "__main__":
-            uvicorn.run(app=app)
-        ```
-        
-        ## License
-        
-        starlette-i18n is developed and distributed under the Apache 2.0 license.
-        
-        ## Reporting a Security Vulnerability
-        
-        See our [security policy](https://github.com/bigbag/starlette-i18n/security/policy).
-        
 Platform: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# starlette-i18n
+
+[![CI](https://github.com/bigbag/starlette-i18n/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-i18n/actions?query=workflow%3ACI)
+[![codecov](https://codecov.io/gh/bigbag/starlette-i18n/branch/main/graph/badge.svg)](https://codecov.io/gh/bigbag/starlette-i18n) 
+[![pypi](https://img.shields.io/pypi/v/starlette-i18n.svg)](https://pypi.python.org/pypi/starlette-i18n)
+[![downloads](https://img.shields.io/pypi/dm/starlette-i18n.svg)](https://pypistats.org/packages/starlette-i18n)
+[![versions](https://img.shields.io/pypi/pyversions/starlette-i18n.svg)](https://github.com/bigbag/starlette-i18n)
+[![license](https://img.shields.io/github/license/bigbag/starlette-i18n.svg)](https://github.com/bigbag/starlette-i18n/blob/master/LICENSE)
+
+
+**starlette-i18n** is a localisation helper for starlette.
+
+
+## Installation
+
+starlette-i18n is available on PyPI.
+Use pip to install:
+
+    $ pip install starlette-i18n
+
+## Basic Usage
+
+```py
+import uvicorn
+from starlette.applications import Starlette
+from starlette.responses import PlainTextResponse
+
+from starlette_i18n import (
+    DEFAULT_LOCALE,
+    LANGUAGE_HEADER,
+    LocaleFromHeaderMiddleware,
+    load_gettext_translations,
+)
+from starlette_i18n import gettext_lazy as _
+
+BABEL_DOMAIN = "messages"
+BABEL_LOCALES_PATH = "locales"
+
+
+def init_app():
+    load_gettext_translations(directory=BABEL_LOCALES_PATH, domain=BABEL_DOMAIN)
+
+    app_ = Starlette()
+    app_.add_middleware(
+        LocaleFromHeaderMiddleware, 
+        language_header=LANGUAGE_HEADER, 
+        default_code=DEFAULT_LOCALE
+    )
+
+    @app_.route("/")
+    def success(request):
+        return PlainTextResponse(_("OK"), status_code=200)
+
+    return app_
+
+
+app = init_app()
+
+if __name__ == "__main__":
+    uvicorn.run(app=app)
+```
+
+## License
+
+starlette-i18n is developed and distributed under the Apache 2.0 license.
+
+## Reporting a Security Vulnerability
+
+See our [security policy](https://github.com/bigbag/starlette-i18n/security/policy).
```

### Comparing `starlette-i18n-1.0.0/README.md` & `starlette-i18n-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `starlette-i18n-1.0.0/setup.py` & `starlette-i18n-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: POSIX",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Environment :: Console",
     "Intended Audience :: Developers",
 ]
```

### Comparing `starlette-i18n-1.0.0/starlette_i18n/__init__.py` & `starlette-i18n-2.0.0/starlette_i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette-i18n-1.0.0/starlette_i18n/helpers.py` & `starlette-i18n-2.0.0/starlette_i18n/helpers.py`

 * *Files identical despite different names*

### Comparing `starlette-i18n-1.0.0/starlette_i18n/i18n.py` & `starlette-i18n-2.0.0/starlette_i18n/i18n.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 def _make_lazy_gettext(lookup_func: t.Callable) -> t.Callable:
     def lazy_gettext(
         string: t.Union[LazyProxy, str],
         *args: t.Any,
         locale: t.Optional[str] = None,
         **kwargs: t.Any,
     ) -> t.Union[LazyProxy, str]:
-
         if isinstance(string, LazyProxy):
             return string
 
         if "enable_cache" not in kwargs:
             kwargs["enable_cache"] = False
 
         return LazyProxy(lookup_func, string, locale=locale, *args, **kwargs)
@@ -61,8 +60,8 @@
 
 def get_locale() -> Locale:
     locale: Locale = _language_ctx.get()
     return locale
 
 
 def get_locale_code() -> str:
-    return str(get_locale())
+    return str(get_locale().language)
```

### Comparing `starlette-i18n-1.0.0/starlette_i18n/locale.py` & `starlette-i18n-2.0.0/starlette_i18n/locale.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from __future__ import annotations
 
 import logging
 import os
 import typing as t
+from dataclasses import dataclass
 
-from babel.core import Locale as _Locale
+from babel.core import Locale as OriginLocale
 from babel.support import NullTranslations, Translations
 
 from . import constants
 
 logger = logging.getLogger(__name__)
 
 
 class _GettextTranslations:
-    _translations: t.Dict[str, t.Union[Translations, NullTranslations]] = {}
+    _translations: t.Dict[str, NullTranslations] = {}
     _default_locale: str = constants.DEFAULT_LOCALE
     _supported_locales: t.Set[str] = set()
 
     @property
-    def translations(
-        self,
-    ) -> t.Dict[str, t.Union[Translations, NullTranslations]]:
+    def translations(self) -> t.Dict[str, NullTranslations]:
         return self._translations
 
     @property
     def supported_locales(self) -> t.Set[str]:
         return self._supported_locales
 
     @property
@@ -35,15 +34,15 @@
         for lang in os.listdir(directory):
             if os.path.isfile(os.path.join(directory, lang)):
                 continue
 
             try:
                 translation = Translations.load(directory, [lang], domain)
                 if lang in self._translations:
-                    self._translations[lang].merge(translation)
+                    self._translations[lang].merge(translation)  # type: ignore
                 else:
                     self._translations[lang] = translation
             except Exception as e:
                 logger.error("Cannot load translation for '%s': %s", lang, str(e))
                 continue
 
         self._supported_locales = set(self._translations.keys())
@@ -51,32 +50,44 @@
 
         logger.info("Supported locales: %s", sorted(self._supported_locales))
 
 
 gettext_translations = _GettextTranslations()
 
 
-class Locale(_Locale):
+@dataclass
+class Locale:
+    language: str
+    translations: NullTranslations
+    territory: t.Optional[str] = None
+    script: t.Optional[str] = None
+    variant: t.Optional[str] = None
+    modifier: t.Optional[str] = None
+
     @classmethod
-    def get(cls, code: str) -> Locale:
+    def get(cls, code: str) -> "Locale":
         if code not in gettext_translations.supported_locales:
             code = gettext_translations.default_locale
 
-        translations = gettext_translations.translations.get(code, NullTranslations())
-        locale: Locale = cls.parse(code)
-        locale.translations = translations
-        return locale
+        locale = OriginLocale.parse(code)
+        return cls(
+            language=locale.language,
+            translations=gettext_translations.translations.get(code, NullTranslations()),
+            territory=locale.territory,
+            script=locale.script,
+            variant=locale.variant,
+            modifier=locale.modifier,
+        )
 
     def translate(
         self,
         message: str,
         plural_message: t.Optional[str] = None,
         count: t.Optional[int] = None,
         **kwargs: str,
     ) -> str:
-
-        if plural_message is not None:
+        if plural_message is not None and count is not None:
             message = self.translations.ungettext(message, plural_message, count)
         else:
             message = self.translations.ugettext(message)
 
         return message.format(**kwargs) if len(kwargs) else message
```

### Comparing `starlette-i18n-1.0.0/starlette_i18n/middleware.py` & `starlette-i18n-2.0.0/starlette_i18n/middleware.py`

 * *Files identical despite different names*

### Comparing `starlette-i18n-1.0.0/starlette_i18n.egg-info/PKG-INFO` & `starlette-i18n-2.0.0/starlette_i18n.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,97 @@
 Metadata-Version: 2.1
 Name: starlette-i18n
-Version: 1.0.0
+Version: 2.0.0
 Summary: Localisation helper for starlette
 Home-page: https://github.com/bigbag/starlette-i18n
+Download-URL: https://pypi.python.org/pypi/starlette-i18n
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
-Download-URL: https://pypi.python.org/pypi/starlette-i18n
-Description: # starlette-i18n
-        
-        [![CI](https://github.com/bigbag/starlette-i18n/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-i18n/actions?query=workflow%3ACI)
-        [![codecov](https://codecov.io/gh/bigbag/starlette-i18n/branch/main/graph/badge.svg)](https://codecov.io/gh/bigbag/starlette-i18n) 
-        [![pypi](https://img.shields.io/pypi/v/starlette-i18n.svg)](https://pypi.python.org/pypi/starlette-i18n)
-        [![downloads](https://img.shields.io/pypi/dm/starlette-i18n.svg)](https://pypistats.org/packages/starlette-i18n)
-        [![versions](https://img.shields.io/pypi/pyversions/starlette-i18n.svg)](https://github.com/bigbag/starlette-i18n)
-        [![license](https://img.shields.io/github/license/bigbag/starlette-i18n.svg)](https://github.com/bigbag/starlette-i18n/blob/master/LICENSE)
-        
-        
-        **starlette-i18n** is a localisation helper for starlette.
-        
-        
-        ## Installation
-        
-        starlette-i18n is available on PyPI.
-        Use pip to install:
-        
-            $ pip install starlette-i18n
-        
-        ## Basic Usage
-        
-        ```py
-        import uvicorn
-        from starlette.applications import Starlette
-        from starlette.responses import PlainTextResponse
-        
-        from starlette_i18n import (
-            DEFAULT_LOCALE,
-            LANGUAGE_HEADER,
-            LocaleFromHeaderMiddleware,
-            load_gettext_translations,
-        )
-        from starlette_i18n import gettext_lazy as _
-        
-        BABEL_DOMAIN = "messages"
-        BABEL_LOCALES_PATH = "locales"
-        
-        
-        def init_app():
-            load_gettext_translations(directory=BABEL_LOCALES_PATH, domain=BABEL_DOMAIN)
-        
-            app_ = Starlette()
-            app_.add_middleware(
-                LocaleFromHeaderMiddleware, 
-                language_header=LANGUAGE_HEADER, 
-                default_code=DEFAULT_LOCALE
-            )
-        
-            @app_.route("/")
-            def success(request):
-                return PlainTextResponse(_("OK"), status_code=200)
-        
-            return app_
-        
-        
-        app = init_app()
-        
-        if __name__ == "__main__":
-            uvicorn.run(app=app)
-        ```
-        
-        ## License
-        
-        starlette-i18n is developed and distributed under the Apache 2.0 license.
-        
-        ## Reporting a Security Vulnerability
-        
-        See our [security policy](https://github.com/bigbag/starlette-i18n/security/policy).
-        
 Platform: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# starlette-i18n
+
+[![CI](https://github.com/bigbag/starlette-i18n/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-i18n/actions?query=workflow%3ACI)
+[![codecov](https://codecov.io/gh/bigbag/starlette-i18n/branch/main/graph/badge.svg)](https://codecov.io/gh/bigbag/starlette-i18n) 
+[![pypi](https://img.shields.io/pypi/v/starlette-i18n.svg)](https://pypi.python.org/pypi/starlette-i18n)
+[![downloads](https://img.shields.io/pypi/dm/starlette-i18n.svg)](https://pypistats.org/packages/starlette-i18n)
+[![versions](https://img.shields.io/pypi/pyversions/starlette-i18n.svg)](https://github.com/bigbag/starlette-i18n)
+[![license](https://img.shields.io/github/license/bigbag/starlette-i18n.svg)](https://github.com/bigbag/starlette-i18n/blob/master/LICENSE)
+
+
+**starlette-i18n** is a localisation helper for starlette.
+
+
+## Installation
+
+starlette-i18n is available on PyPI.
+Use pip to install:
+
+    $ pip install starlette-i18n
+
+## Basic Usage
+
+```py
+import uvicorn
+from starlette.applications import Starlette
+from starlette.responses import PlainTextResponse
+
+from starlette_i18n import (
+    DEFAULT_LOCALE,
+    LANGUAGE_HEADER,
+    LocaleFromHeaderMiddleware,
+    load_gettext_translations,
+)
+from starlette_i18n import gettext_lazy as _
+
+BABEL_DOMAIN = "messages"
+BABEL_LOCALES_PATH = "locales"
+
+
+def init_app():
+    load_gettext_translations(directory=BABEL_LOCALES_PATH, domain=BABEL_DOMAIN)
+
+    app_ = Starlette()
+    app_.add_middleware(
+        LocaleFromHeaderMiddleware, 
+        language_header=LANGUAGE_HEADER, 
+        default_code=DEFAULT_LOCALE
+    )
+
+    @app_.route("/")
+    def success(request):
+        return PlainTextResponse(_("OK"), status_code=200)
+
+    return app_
+
+
+app = init_app()
+
+if __name__ == "__main__":
+    uvicorn.run(app=app)
+```
+
+## License
+
+starlette-i18n is developed and distributed under the Apache 2.0 license.
+
+## Reporting a Security Vulnerability
+
+See our [security policy](https://github.com/bigbag/starlette-i18n/security/policy).
```

