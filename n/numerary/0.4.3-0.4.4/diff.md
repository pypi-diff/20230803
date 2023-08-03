# Comparing `tmp/numerary-0.4.3-py3-none-any.whl.zip` & `tmp/numerary-0.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 22666 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1051 b- defN 22-Oct-13 21:21 numerary/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 22-Oct-13 21:22 numerary/_version.py
--rw-r--r--  2.0 unx     1795 b- defN 22-Oct-13 21:21 numerary/bt.py
--rw-r--r--  2.0 unx     5673 b- defN 22-Oct-13 21:21 numerary/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-13 21:21 numerary/py.typed
--rw-r--r--  2.0 unx    48632 b- defN 22-Oct-13 21:21 numerary/types.py
--rw-r--r--  2.0 unx     2123 b- defN 22-Oct-13 21:22 numerary-0.4.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    29055 b- defN 22-Oct-13 21:22 numerary-0.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-13 21:22 numerary-0.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Oct-13 21:22 numerary-0.4.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      837 b- defN 22-Oct-13 21:22 numerary-0.4.3.dist-info/RECORD
-11 files, 89315 bytes uncompressed, 21264 bytes compressed:  76.2%
+Zip file size: 22664 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1051 b- defN 23-Aug-03 17:47 numerary/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 23-Aug-03 17:48 numerary/_version.py
+-rw-r--r--  2.0 unx     1795 b- defN 23-Aug-03 17:47 numerary/bt.py
+-rw-r--r--  2.0 unx     5673 b- defN 23-Aug-03 17:47 numerary/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-03 17:47 numerary/py.typed
+-rw-r--r--  2.0 unx    48542 b- defN 23-Aug-03 17:47 numerary/types.py
+-rw-r--r--  2.0 unx     2123 b- defN 23-Aug-03 17:48 numerary-0.4.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    29050 b- defN 23-Aug-03 17:48 numerary-0.4.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 17:48 numerary-0.4.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Aug-03 17:48 numerary-0.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      837 b- defN 23-Aug-03 17:48 numerary-0.4.4.dist-info/RECORD
+11 files, 89220 bytes uncompressed, 21262 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: numerary/py.typed
 Comment: 
 
 Filename: numerary/types.py
 Comment: 
 
-Filename: numerary-0.4.3.dist-info/LICENSE
+Filename: numerary-0.4.4.dist-info/LICENSE
 Comment: 
 
-Filename: numerary-0.4.3.dist-info/METADATA
+Filename: numerary-0.4.4.dist-info/METADATA
 Comment: 
 
-Filename: numerary-0.4.3.dist-info/WHEEL
+Filename: numerary-0.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: numerary-0.4.3.dist-info/top_level.txt
+Filename: numerary-0.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: numerary-0.4.3.dist-info/RECORD
+Filename: numerary-0.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## numerary/_version.py

```diff
@@ -1,3 +1,3 @@
-__vers_str__ = "0.4.3"
-__version__ = (0, 4, 3)
+__vers_str__ = "0.4.4"
+__version__ = (0, 4, 4)
```

## numerary/types.py

```diff
@@ -1309,22 +1309,23 @@
 {RationalLikeMixedU!r}
 """
 RationalLikeMixedT = (RationalLike, RationalLikeMethods)
 rf"""
 {RationalLikeMixedT!r}
 """
 assert RationalLikeMixedU.__args__ == RationalLikeMixedT  # type: ignore [attr-defined]
-assert RationalLikeMethods.__doc__
-RationalLikeMethods.__doc__ += rf"""
 
-    ``` python
-    RationalLikeMixedU = {RationalLikeMixedU!r}
-    RationalLikeMixedT = ({", ".join(cls.__name__ for cls in  RationalLikeMixedT)})
-    ```
-"""
+if RationalLikeMethods.__doc__:
+    RationalLikeMethods.__doc__ += rf"""
+
+        ``` python
+        RationalLikeMixedU = {RationalLikeMixedU!r}
+        RationalLikeMixedT = ({", ".join(cls.__name__ for cls in  RationalLikeMixedT)})
+        ```
+    """
 
 
 @runtime_checkable
 class IntegralLike(
     SupportsAbs[_T_co],
     SupportsFloat,
     SupportsIndex,
@@ -1427,15 +1428,15 @@
     [SupportsRealImagAsMethod][numerary.types.SupportsRealImagAsMethod].
     """
     if callable(getattr(operand, "as_real_imag", None)):
         real_part, _ = operand.as_real_imag()  # type: ignore [union-attr]
 
         return real_part
     elif hasattr(operand, "real"):
-        return operand.real  # type: ignore [union-attr]
+        return operand.real
     else:
         raise TypeError(f"{operand!r} has no real or as_real_imag")
 
 
 @beartype
 def imag(operand: SupportsRealImagMixedU):
     r"""
@@ -1457,15 +1458,15 @@
     [SupportsRealImagAsMethod][numerary.types.SupportsRealImagAsMethod].
     """
     if callable(getattr(operand, "as_real_imag", None)):
         _, imag_part = operand.as_real_imag()  # type: ignore [union-attr]
 
         return imag_part
     elif hasattr(operand, "imag"):
-        return operand.imag  # type: ignore [union-attr]
+        return operand.imag
     else:
         raise TypeError(f"{operand!r} has no real or as_real_imag")
 
 
 # TODO(posita): Are these sufficient? Could these be more specific? See:
 # <https://github.com/python/typeshed/issues/6303#issuecomment-969392257>.
 @overload
@@ -1602,15 +1603,15 @@
     0
     >>> my_floor_float: SupportsFloat = 1.2
     >>> __floor__(my_floor_float)
     1
 
     ```
     """
-    return math.floor(operand)  # type: ignore [arg-type]
+    return math.floor(operand)
 
 
 @beartype
 def __ceil__(operand: Union[SupportsFloat, SupportsFloorCeil]):
     r"""
     Helper function that wraps ``math.ceil``.
 
@@ -1626,15 +1627,15 @@
     1
     >>> my_ceil_float: SupportsFloat = 1.2
     >>> __ceil__(my_ceil_float)
     2
 
     ```
     """
-    return math.ceil(operand)  # type: ignore [arg-type]
+    return math.ceil(operand)
 
 
 @beartype
 def numerator(operand: SupportsNumeratorDenominatorMixedU):
     r"""
     Helper function that extracts the numerator from *operand* including resolving
     non-compliant rational implementations that implement ``numerator`` as a method
```

## Comparing `numerary-0.4.3.dist-info/LICENSE` & `numerary-0.4.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `numerary-0.4.3.dist-info/METADATA` & `numerary-0.4.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerary
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python hacks for type-checking numbers
 Home-page: https://posita.github.io/numerary/
 Author: Matt Bogosian
 Author-email: matt@bogosian.net
 License: MIT License
 Project-URL: Source Repository, https://github.com/posita/numerary/
 Classifier: Topic :: Education
@@ -23,20 +23,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
-Requires-Dist: beartype (==0.*,>=0.10.4)
+Requires-Dist: beartype (~=0.15)
 Provides-Extra: dev
 Requires-Dist: pre-commit ; extra == 'dev'
-Requires-Dist: numpy (~=1.23.2) ; extra == 'dev'
-Requires-Dist: sympy (~=1.10.1) ; extra == 'dev'
-Requires-Dist: tox ; extra == 'dev'
+Requires-Dist: numpy (~=1.25) ; extra == 'dev'
+Requires-Dist: sympy (~=1.9) ; extra == 'dev'
+Requires-Dist: tox (~=4.0) ; extra == 'dev'
 Requires-Dist: versioningit (~=2.0) ; extra == 'dev'
 
 <!---
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !!!!!!!!!!!!!!! IMPORTANT: READ THIS BEFORE EDITING! !!!!!!!!!!!!!!!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   Please keep each sentence on its own unwrapped line.
@@ -51,19 +51,19 @@
 
 *Copyright and other protections apply.
 Please see the accompanying ``LICENSE`` file for rights and restrictions governing use of this software.
 All rights not expressly waived or licensed are reserved.
 If that file is missing or appears to be modified from its original, then please contact the author before viewing or using this software in any capacity.*
 
 [![Tests](https://github.com/posita/numerary/actions/workflows/on-push.yaml/badge.svg)](https://github.com/posita/numerary/actions/workflows/on-push.yaml)
-[![Version](https://img.shields.io/pypi/v/numerary/0.4.3.svg)](https://pypi.org/project/numerary/0.4.3/)
-[![Development Stage](https://img.shields.io/pypi/status/numerary/0.4.3.svg)](https://pypi.org/project/numerary/0.4.3/)
-[![License](https://img.shields.io/pypi/l/numerary/0.4.3.svg)](http://opensource.org/licenses/MIT)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/numerary/0.4.3.svg)](https://pypi.org/project/numerary/0.4.3/)
-[![Supported Python Implementations](https://img.shields.io/pypi/implementation/numerary/0.4.3.svg)](https://pypi.org/project/numerary/0.4.3/)
+[![Version](https://img.shields.io/pypi/v/numerary/0.4.4.svg)](https://pypi.org/project/numerary/0.4.4/)
+[![Development Stage](https://img.shields.io/pypi/status/numerary/0.4.4.svg)](https://pypi.org/project/numerary/0.4.4/)
+[![License](https://img.shields.io/pypi/l/numerary/0.4.4.svg)](http://opensource.org/licenses/MIT)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/numerary/0.4.4.svg)](https://pypi.org/project/numerary/0.4.4/)
+[![Supported Python Implementations](https://img.shields.io/pypi/implementation/numerary/0.4.4.svg)](https://pypi.org/project/numerary/0.4.4/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Bear-ified™](https://raw.githubusercontent.com/beartype/beartype-assets/main/badge/bear-ified.svg)](https://beartype.rtfd.io/)
 
 Are you defining a numeric interface that should work with more than just ``int``s and ``float``s?
 Are you annotating that interface for documentation *and* type-checking?
 Were you excited by [PEP 3141](https://www.python.org/dev/peps/pep-3141/)’s glitz and gloss promising a clean, straightforward number type definition mechanism, only to learn the hard way—after many hours of searching, tweaking, hacking, and testing ever more convoluted code, again and again—that you could’t actually make it work with Python’s type-checking system?
 Do you now wonder whether numbers were something new to computing in general because nothing else would explain such a gaping hole in a programming language so popular with the STEM crowd that has been around since the early 1990s?
@@ -295,15 +295,15 @@
 These offer significant performance improvements, especially where protocols define many methods.
 
 ``` python
 --8<-- "docs/perf_supports_complex.txt"
 ```
 
 <details>
-<summary>Source: <a href="https://github.com/posita/numerary/blob/v0.4.3/docs/perf_supports_complex.ipy"><code>perf_supports_complex.ipy</code></a></summary>
+<summary>Source: <a href="https://github.com/posita/numerary/blob/v0.4.4/docs/perf_supports_complex.ipy"><code>perf_supports_complex.ipy</code></a></summary>
 
 ``` python
 --8<-- "docs/perf_supports_complex.ipy"
 ```
 </details>
 
 ### ``Union``s for inclusion
@@ -554,15 +554,15 @@
 That’s completely off the beaten path and there are probably some gremlins hiding out there.
 
 One subtlety is that the implementation deviates from performing checks in MRO order (and may perform redundant checks).
 This is probably fine as long as runtime comparisons remain limited to crude checks whether attributes merely exist.
 It would likely fail if runtime checking becomes more sophisticated, at which time, this implementation will need to be revisited.
 Hopefully by then, we can just delete ``numerary`` as the aspirationally unnecessary hack it is and move on with our lives.
 
-(See [``beartype.typing``](https://github.com/beartype/beartype/tree/main/beartype/typing) and [``numerary``’s extension](https://github.com/posita/numerary/blob/v0.4.3/numerary/types.py) for details.)
+(See [``beartype.typing``](https://github.com/beartype/beartype/tree/main/beartype/typing) and [``numerary``’s extension](https://github.com/posita/numerary/blob/v0.4.4/numerary/types.py) for details.)
 
 ## License
 
 ``numerary`` is licensed under the [MIT License](https://opensource.org/licenses/MIT).
 See the included [``LICENSE``](https://posita.github.io/numerary/0.4/license/) file for details.
 Source code is [available on GitHub](https://github.com/posita/numerary).
 
@@ -601,15 +601,15 @@
 
 [^4]:
 
     I.E., one of: ``1``, ``on``, ``t``, ``true``, and ``yes``.
 
 See the [hacking quick-start](https://posita.github.io/numerary/0.4/contrib/#hacking-quick-start) for additional development and testing dependencies.
 
-## Customers [![``numerary``-encumbered](https://raw.githubusercontent.com/posita/numerary/v0.4.3/docs/numerary-encumbered.svg)](https://posita.github.io/numerary/)
+## Customers [![``numerary``-encumbered](https://raw.githubusercontent.com/posita/numerary/v0.4.4/docs/numerary-encumbered.svg)](https://posita.github.io/numerary/)
 
 * [``dyce``](https://github.com/posita/dyce/) - a pure-Python library for modeling arbitrarily complex dice mechanics and ~~mother~~ *birthing code base* of ``numerary``!
 * [👻 ``phantom-types``](https://github.com/antonagestam/phantom-types) - predicates and other type constraints without runtime overhead
 * The next one could be _you_! 👋
 
 Do you have a project that suffers problems made slightly less annoying by ``numerary``?
 [Let me know](https://posita.github.io/numerary/0.4/contrib/#starting-discussions-and-filing-issues), and I’ll promote it here!
```

## Comparing `numerary-0.4.3.dist-info/RECORD` & `numerary-0.4.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 numerary/__init__.py,sha256=k6QKh-WuCjm_Dj8gAjOQ1bB_xFAeIUAtScDsfxJYTqo,1051
-numerary/_version.py,sha256=kSXQbq9njMgdVeU0OAkd7--1UhdE2bK5TW8D3_qbV-0,48
+numerary/_version.py,sha256=qa0dN7AELes59gWluANDETnsq__J-HuaOwIEjxNMteU,48
 numerary/bt.py,sha256=ERxq3iXusyZDaBdwMSxdKeDLTjF8HBxCHJBlD_FCzS4,1795
 numerary/protocol.py,sha256=sZhfEHhqNfW09YG8GTamMTJorJpVLGPwua6mBcni01I,5673
 numerary/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-numerary/types.py,sha256=mNwH2ASJ16Sx43MXccubaWUzL-i6FuiVNHPk05nHQM8,48632
-numerary-0.4.3.dist-info/LICENSE,sha256=QzicbGh44z-O64c2KmTpDWqbm9eZlyBqDCeY2SmhnI8,2123
-numerary-0.4.3.dist-info/METADATA,sha256=eGA0GFcF_U3Vceo6Y30C2gTFQUiscmkHvq8tRkp95Vc,29055
-numerary-0.4.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-numerary-0.4.3.dist-info/top_level.txt,sha256=1rtTwz1eyJiLorer_nlqxLIoQryCi9pX71gzGRHhHRo,9
-numerary-0.4.3.dist-info/RECORD,,
+numerary/types.py,sha256=KS--YuHmHnL3NsA4UdetNdmEBwJYQ3exakxw4-i-RaI,48542
+numerary-0.4.4.dist-info/LICENSE,sha256=QzicbGh44z-O64c2KmTpDWqbm9eZlyBqDCeY2SmhnI8,2123
+numerary-0.4.4.dist-info/METADATA,sha256=_QvmWIcou4B7XlyHb0TWHlha0LuM1ZckM55rh1kKp18,29050
+numerary-0.4.4.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+numerary-0.4.4.dist-info/top_level.txt,sha256=1rtTwz1eyJiLorer_nlqxLIoQryCi9pX71gzGRHhHRo,9
+numerary-0.4.4.dist-info/RECORD,,
```

