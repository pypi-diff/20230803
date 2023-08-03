# Comparing `tmp/significantdigits-0.1.2.tar.gz` & `tmp/significantdigits-0.1.3.tar.gz`

## Comparing `significantdigits-0.1.2.tar` & `significantdigits-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/__init__.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/__main__.py
--rw-r--r--   0        0        0    29800 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/_significantdigits.py
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/args.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/conftest.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/export/__init__.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/export/generic.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/export/numpy.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/export/stdin.py
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/scripts/significantdigits
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/src/Makefile
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/src/float_const.h
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/src/float_struct.h
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/src/truncation.c
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/src/truncation.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/stats/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/stats/dense.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/stats/dispatch.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/stats/sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/test/__init__.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/test/test_args.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/test/test_cramer.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/test/test_higham.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/test/test_parker.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 significantdigits-0.1.2/significantdigits/test/utils.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 significantdigits-0.1.2/.gitignore
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 significantdigits-0.1.2/LICENSE
--rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 significantdigits-0.1.2/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 significantdigits-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10981 2020-02-02 00:00:00.000000 significantdigits-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/__init__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/__main__.py
+-rw-r--r--   0        0        0    29867 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/_significantdigits.py
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/args.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/conftest.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/export/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/export/generic.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/export/numpy.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/export/stdin.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/src/Makefile
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/src/float_const.h
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/src/float_struct.h
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/src/truncation.c
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/src/truncation.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/stats/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/stats/dense.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/stats/dispatch.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/stats/sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/test/__init__.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/test/test_args.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/test/test_cramer.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/test/test_higham.py
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/test/test_parker.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/test/test_scalar.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 significantdigits-0.1.3/significantdigits/test/utils.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 significantdigits-0.1.3/.gitignore
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 significantdigits-0.1.3/LICENSE
+-rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 significantdigits-0.1.3/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 significantdigits-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 significantdigits-0.1.3/PKG-INFO
```

### Comparing `significantdigits-0.1.2/significantdigits/__main__.py` & `significantdigits-0.1.3/significantdigits/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/python3
 
 import sys
 
 
 from significantdigits import export
-from significantdigits import (
-    significant_digits, contributing_digits, Metric)
+from significantdigits import significant_digits, contributing_digits, Metric
 from significantdigits import args as argparse
 from significantdigits import stats
 
 
 def main():
     args = argparse.parse_args()
     Parser = export.input_formats[args.input_format]
@@ -24,33 +23,39 @@
 
     if args.reference:
         reference = parser.parse(args.reference, dtype=dtype)
     else:
         reference = stats.mean(inputs, axis=args.axis, dtype=dtype)
 
     if args.metric == Metric.Significant:
-        s = significant_digits(array=inputs,
-                               reference=reference,
-                               axis=args.axis,
-                               base=args.base,
-                               error=args.error,
-                               method=args.method,
-                               probability=args.probability,
-                               confidence=args.confidence)
+        s = significant_digits(
+            array=inputs,
+            reference=reference,
+            axis=args.axis,
+            base=args.base,
+            error=args.error,
+            method=args.method,
+            probability=args.probability,
+            confidence=args.confidence,
+            dtype=dtype,
+        )
     elif args.metric == Metric.Contributing:
-        s = contributing_digits(array=inputs,
-                                reference=reference,
-                                axis=args.axis,
-                                base=args.base,
-                                error=args.error,
-                                method=args.method,
-                                probability=args.probability,
-                                confidence=args.confidence)
+        s = contributing_digits(
+            array=inputs,
+            reference=reference,
+            axis=args.axis,
+            base=args.base,
+            error=args.error,
+            method=args.method,
+            probability=args.probability,
+            confidence=args.confidence,
+            dtype=dtype,
+        )
     else:
-        print(f'Error: unkown metric {args.metric}')
+        print(f"Error: unkown metric {args.metric}")
         sys.exit(1)
 
     exporter.export(s)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `significantdigits-0.1.2/significantdigits/_significantdigits.py` & `significantdigits-0.1.3/significantdigits/_significantdigits.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-
-from typing import TypeVar
-from typing import Tuple, Union
-import math
 import warnings
 from enum import Enum, auto
-from typing import Optional
+from typing import Optional, Tuple, TypeVar, Union
 
 import numpy as np
 import scipy
 import scipy.stats
 
 
 class AutoName(Enum):
@@ -17,14 +13,15 @@
 
 
 class Metric(AutoName):
     """
     Significant: Compute the number of significant digits
     Contributing: Compute the number of contributing digits
     """
+
     Significant = auto()
     Contributing = auto()
 
     @classmethod
     def is_significant(cls, error):
         if isinstance(error, cls):
             return error == cls.Significant
@@ -42,14 +39,15 @@
 class Method(AutoName):
     """
     CNH: Centered Normality Hypothesis
          X follows a Gaussian law centered around the reference or
          Z follows a Gaussian law centered around 0
     General: No assumption about the distribution of X or Z
     """
+
     CNH = auto()
     General = auto()
 
     @classmethod
     def is_cnh(cls, error):
         if isinstance(error, cls):
             return error == cls.CNH
@@ -69,14 +67,15 @@
     ----------+-------------+-------------
               | Reference x | Reference Y
     ----------+-------------+-------------
     Absolute  | Z = X - x   | Z = X - Y
     Relative  | Z = X/x - 1 | Z = X/Y - 1
     ----------+-------------+-------------
     """
+
     Absolute = auto()
     Relative = auto()
 
     @classmethod
     def is_absolute(cls, error):
         if isinstance(error, cls):
             return error == cls.Absolute
@@ -94,146 +93,148 @@
 def _lower_map(x):
     if isinstance(x, list):
         return list(map(str.lower, x))
     if isinstance(x, dict):
         return {k.lower(): v for k, v in x.items()}
 
 
-Metric.names = _lower_map(vars(Metric)['_member_names_'])
-Metric.map = _lower_map(vars(Metric)['_value2member_map_'])
+Metric.names = _lower_map(vars(Metric)["_member_names_"])
+Metric.map = _lower_map(vars(Metric)["_value2member_map_"])
 
-Method.names = _lower_map(vars(Method)['_member_names_'])
-Method.map = _lower_map(vars(Method)['_value2member_map_'])
+Method.names = _lower_map(vars(Method)["_member_names_"])
+Method.map = _lower_map(vars(Method)["_value2member_map_"])
 
-Error.names = _lower_map(vars(Error)['_member_names_'])
-Error.map = _lower_map(vars(Error)['_value2member_map_'])
+Error.names = _lower_map(vars(Error)["_member_names_"])
+Error.map = _lower_map(vars(Error)["_value2member_map_"])
 
 internal_dtype = np.dtype(np.float64)
-default_probability = {Metric.Significant: 0.95,
-                       Metric.Contributing: 0.51}
-default_confidence = {Metric.Significant: 0.95,
-                      Metric.Contributing: 0.95}
+default_probability = {Metric.Significant: 0.95, Metric.Contributing: 0.51}
+default_confidence = {Metric.Significant: 0.95, Metric.Contributing: 0.95}
 
-InputType = TypeVar('InputType', np.ndarray, tuple, list)
-r'''Valid random variable inputs type (np.ndarray, tuple, list)
+InputType = TypeVar("InputType", np.ndarray, tuple, list)
+r"""Valid random variable inputs type (np.ndarray, tuple, list)
 
 Types allowing for `array` in significant_digits and contributing_digits functions
 
-'''
+"""
 
-ReferenceType = TypeVar('ReferenceType', np.ndarray, tuple, list, float, int)
-r'''Valid reference inputs type (np.ndarray, tuple, list, float, int)
+ReferenceType = TypeVar(
+    "ReferenceType", np.ndarray, tuple, list, float, int, np.floating
+)
+r"""Valid reference inputs type (np.ndarray, tuple, list, float, int)
 
 Types allowing for `reference` in significant_digits and contributing_digits functions
 
-'''
+"""
 
 
 def get_input_type():
-    r''' Returns InputType subtypes'''
+    r"""Returns InputType subtypes"""
     return InputType.__constraints__
 
 
 def get_reference_type():
-    r'''Returns ReferenceType subtypes'''
+    r"""Returns ReferenceType subtypes"""
     return ReferenceType.__constraints__
 
 
 def assert_is_valid_metric(metric: Union[Metric, str]) -> None:
     if Metric.is_significant(metric) or Metric.is_contributing(metric):
         return
 
-    raise TypeError(f"provided invalid metric {metric}: "
-                    f"must be one of {list(Metric)}")
+    raise TypeError(
+        f"provided invalid metric {metric}: " f"must be one of {list(Metric)}"
+    )
 
 
 def assert_is_valid_method(method: Union[Method, str]) -> None:
     if Method.is_cnh(method) or Method.is_general(method):
         return
 
-    raise TypeError(f"provided invalid method {method}: "
-                    f"must be one of {list(Method)}")
+    raise TypeError(
+        f"provided invalid method {method}: " f"must be one of {list(Method)}"
+    )
 
 
 def assert_is_valid_error(error: Union[Error, str]) -> None:
     if Error.is_absolute(error) or Error.is_relative(error):
         return
 
-    raise TypeError(f"provided invalid error {error}: "
-                    f"must be one of {list(Error)}")
+    raise TypeError(f"provided invalid error {error}: " f"must be one of {list(Error)}")
 
 
 def assert_is_probability(probability: float) -> None:
     if probability < 0 or probability > 1:
         raise TypeError("probability must be between 0 and 1")
 
 
 def assert_is_confidence(confidence: float) -> None:
     if confidence < 0 or confidence > 1:
         raise TypeError("confidence must be between 0 and 1")
 
 
-def change_base(array: InputType, base: int) -> InputType:
-    '''Changes basis from binary to `base` representation
+def change_basis(array: InputType, base: int) -> InputType:
+    """Changes basis from binary to `base` representation
 
     Parameters
     ----------
     array : np.ndarray
         array_like containing significant or contributing bits
     basis : int
         output basis
 
     Returns
     -------
     np.ndarray
         Array convert to base `base`
-    '''
-    sig_power2 = np.power(2, array)
-
-    def to_base(x):
-        return math.log(x, base)
-    np_to_base = np.frompyfunc(to_base, 1, 1)
-    x = np_to_base(sig_power2)
-    return x
-
+    """
+    pow2 = np.power(2, array, dtype=np.float64)
+    array_masked = np.ma.array(pow2, mask=array <= 0)
+    return np.emath.logn(base, array_masked).astype(np.int8)
 
-def preprocess_inputs(array: Union[np.ndarray, tuple, list],
-                      reference: Union[np.ndarray, tuple, list]
-                      ) -> Tuple[np.ndarray, np.ndarray]:
 
+def preprocess_inputs(
+    array: Union[np.ndarray, tuple, list], reference: Union[np.ndarray, tuple, list]
+) -> Tuple[np.ndarray, np.ndarray]:
     if scipy.sparse.issparse(array[0]):
         array = np.asanyarray([i.toarray() for i in array])
 
     if not isinstance(array, InputType.__constraints__):
-        raise TypeError(f'Input array must be '
-                        f'one of the following types '
-                        f'{InputType.__constraints__}')
+        raise TypeError(
+            f"Input array must be "
+            f"one of the following types "
+            f"{InputType.__constraints__}"
+        )
 
     if not isinstance(array, np.ndarray):
         array = np.array(array)
 
     if reference is not None:
         if scipy.sparse.issparse(reference):
             reference = reference.toarray()
         if not isinstance(reference, ReferenceType.__constraints__):
-            raise TypeError(f'Reference must be '
-                            f'one of the following types '
-                            f'{ReferenceType.__constraints__}')
+            raise TypeError(
+                f"Reference must be "
+                f"one of the following types "
+                f"{ReferenceType.__constraints__}"
+            )
 
         if not isinstance(reference, np.ndarray):
             reference = np.array(reference)
 
     return (array, reference)
 
 
-def compute_z(array: InputType,
-              reference: Optional[ReferenceType],
-              error: Union[Error, str],
-              axis: int,
-              shuffle_samples: bool = False) -> InputType:
+def compute_z(
+    array: InputType,
+    reference: Optional[ReferenceType],
+    error: Union[Error, str],
+    axis: int,
+    shuffle_samples: bool = False,
+) -> InputType:
     r"""Compute Z, the distance between the random variable and the reference
 
     Compute Z, the distance between the random variable and the reference
     with three cases depending on the dimensions of array and reference:
 
     X = array
     Y = reference
@@ -272,16 +273,15 @@
 
 
     """
     nb_samples = array.shape[axis]
 
     if reference is None:
         if nb_samples % 2 != 0:
-            error_msg = ("Number of samples must be ",
-                         "a multiple of 2")
+            error_msg = ("Number of samples must be ", "a multiple of 2")
             raise Exception(error_msg)
         nb_samples /= 2
         if shuffle_samples:
             np.random.shuffle(array)
         x, y = np.split(array, 2, axis=axis)
     elif reference.ndim == array.ndim:
         x = array
@@ -294,36 +294,40 @@
         y = reference
     elif reference.ndim == 0:
         x = array
         y = reference
     else:
         raise TypeError("No comparison found for X and reference:")
 
+    x = np.array(x)
+    y = np.array(y)
+
     if Error.is_absolute(error):
         z = x - y
     elif Error.is_relative(error):
         if np.any(y[y == 0]):
-            warn_msg = ('error is set to relative and the reference '
-                        '0 leading to NaN')
+            warn_msg = "error is set to relative and the reference " "0 leading to NaN"
             warnings.warn(warn_msg)
         z = x / y - 1
     else:
         raise Exception(f"Unknown error {error}")
-
     return z
 
 
-def significant_digits_cnh(array: InputType,
-                           reference: Optional[ReferenceType],
-                           axis: int,
-                           error: Union[Error, str],
-                           probability: float,
-                           confidence: float,
-                           shuffle_samples: bool = False) -> InputType:
-    r'''Compute significant digits for Centered Normality Hypothesis (CNH)
+def significant_digits_cnh(
+    array: InputType,
+    reference: Optional[ReferenceType],
+    axis: int,
+    error: Union[Error, str],
+    probability: float,
+    confidence: float,
+    shuffle_samples: bool = False,
+    dtype: Optional[np.dtype] = None,
+) -> InputType:
+    r"""Compute significant digits for Centered Normality Hypothesis (CNH)
 
     Parameters
     ----------
     array: InputType
         Element to compute
     reference: Optional[ReferenceType]
         Reference for comparing the array
@@ -335,14 +339,17 @@
         Probability for the significant digits result
     confidence : float
         Confidence level for the significant digits result
     shuffle_samples : bool, default=False
         If reference is None, the array is split in two and
         comparison is done between both pieces.
         If shuffle_samples is True, it shuffles pieces.
+    dtype : np.dtype, default=None
+        Numerical type used for computing contributing digits
+        Widest format between array and reference is taken if no supplied.
 
     Returns
     -------
     ndarray
         array_like containing contributing digits
 
     See Also
@@ -357,37 +364,39 @@
     .. [1] Sohier, D., Castro, P. D. O., Févotte, F.,
     Lathuilière, B., Petit, E., & Jamond, O. (2021).
     Confidence intervals for stochastic arithmetic.
     ACM Transactions on Mathematical Software (TOMS), 47(2), 1-33.
 
     .. math::
         s >= -log_2(std) - [\frac{1}{2} log_2( \frac{n-1}{ Chi^2_{1-\frac{\alpha}{2}} }) ) + log_2(F^{-1}(\frac{p+1}{2})]
-    '''
-    z = compute_z(array, reference, error, axis=axis,
-                  shuffle_samples=shuffle_samples)
+    """
+    z = compute_z(array, reference, error, axis=axis, shuffle_samples=shuffle_samples)
     nb_samples = z.shape[axis]
     std = np.std(z, axis=axis, dtype=internal_dtype)
-    std0 = np.ma.masked_array(std == 0)
+    std0 = np.ma.array(std, mask=std == 0)
     chi2 = scipy.stats.chi2.interval(confidence, nb_samples - 1)[0]
     inorm = scipy.stats.norm.ppf((probability + 1) / 2)
     delta_chn = 0.5 * np.log2((nb_samples - 1) / chi2) + np.log2(inorm)
-    significant = -np.log2(std) - delta_chn
-    if significant.ndim != 0:
-        significant[std0] = np.finfo(z.dtype).nmant - delta_chn
-    elif std0:
-        significant = np.finfo(z.dtype).nmant - delta_chn
+    significant = -1 * (np.ma.log2(std0) + delta_chn)
+    max_bits = np.finfo(dtype if dtype else z.dtype).nmant
+    if significant.ndim == 0:
+        significant = np.ma.array(significant, mask=std0.mask)
+    significant = significant.filled(fill_value=max_bits - delta_chn)
     return significant
 
 
-def significant_digits_general(array: InputType,
-                               reference: Optional[ReferenceType],
-                               axis: int,
-                               error: Union[Error, str],
-                               shuffle_samples: bool = False) -> InputType:
-    r'''Compute significant digits for unknown underlying distribution
+def significant_digits_general(
+    array: InputType,
+    reference: Optional[ReferenceType],
+    axis: int,
+    error: Union[Error, str],
+    shuffle_samples: bool = False,
+    dtype: Optional[np.dtype] = None,
+) -> InputType:
+    r"""Compute significant digits for unknown underlying distribution
 
     For the general case, the probability is not parametrizable but
     can be estimated by the sample size. By setting `return_probability` to
     True, the function returns a tuple with the estimated probability
     lower bound for the given `confidence`.
 
     Parameters
@@ -400,14 +409,17 @@
         Axis or axes along which the significant digits are computed
     error : Error | str
         The error function to use to compute error between array and reference.
     shuffle_samples : bool, optional=False
         If reference is None, the array is split in two and
         comparison is done between both pieces.
         If shuffle_samples is True, it shuffles pieces.
+    dtype : np.dtype, default=None
+        Numerical type used for computing contributing digits
+        Widest format between array and reference is taken if no supplied.
 
     Returns
     -------
     out : ndarray
         array_like containing contributing digits
 
     See Also
@@ -422,49 +434,53 @@
     .. [1] Sohier, D., Castro, P. D. O., Févotte, F.,
     Lathuilière, B., Petit, E., & Jamond, O. (2021).
     Confidence intervals for stochastic arithmetic.
     ACM Transactions on Mathematical Software (TOMS), 47(2), 1-33.
 
     .. math::
         s = max{k \in [1,mant], st \forall i \in [1,n], |Z_i| <= 2^{-k}}
-    '''
-    z = compute_z(array, reference, error, axis=axis,
-                  shuffle_samples=shuffle_samples)
+    """
+    z = compute_z(array, reference, error, axis=axis, shuffle_samples=shuffle_samples)
 
     sample_shape = tuple(dim for i, dim in enumerate(z.shape) if i != axis)
-    max_bits = np.finfo(z.dtype).nmant
-    significant = np.full(sample_shape, max_bits, dtype=np.float64)
-    z_mask = np.full(sample_shape, False)
-    for k in range(max_bits, -1, -1):
-        pow2minusk = np.power(2, -np.float64(k))
-        successess = np.abs(z) <= pow2minusk
-        _z = np.all(successess, axis=axis)
-        if z.ndim == 0 and _z:
-            significant = k
+    max_bits = np.finfo(dtype if dtype else z.dtype).nmant
+    significant = np.ma.MaskedArray(
+        data=np.full(shape=sample_shape, fill_value=0, dtype=np.int8), mask=False
+    )
+    zz = np.ma.array(np.abs(z), mask=np.abs(z) <= 0, fill_value=max_bits)
+    if np.all(zz.mask):
+        return zz.filled()
+
+    z2 = np.ma.log2(zz)
+
+    # Compute successes
+    for k in range(0, max_bits + 1):
+        # min(bool) <=> logical and
+        successes = np.ma.min(z2 <= -k, axis=axis)
+        significant.mask |= np.ma.logical_not(successes)
+        significant[np.logical_not(significant.mask)] = k
+        if np.all(significant.mask):
             break
 
-        z_mask = np.ma.masked_array(data=_z, mask=_z)
-        if np.all(_z):
-            break
-
-        significant[~z_mask] = k
+    return significant.data
 
-    return significant
 
-
-def significant_digits(array: InputType,
-                       reference: Optional[ReferenceType] = None,
-                       axis: int = 0,
-                       base: int = 2,
-                       error: Union[str, Error] = Error.Relative,
-                       method: Union[str, Method] = Method.CNH,
-                       probability: float = default_probability[Metric.Significant],
-                       confidence: float = default_confidence[Metric.Significant],
-                       shuffle_samples: bool = False) -> InputType:
-    r'''Compute significant digits
+def significant_digits(
+    array: InputType,
+    reference: Optional[ReferenceType] = None,
+    axis: int = 0,
+    base: int = 2,
+    error: Union[str, Error] = Error.Relative,
+    method: Union[str, Method] = Method.CNH,
+    probability: float = default_probability[Metric.Significant],
+    confidence: float = default_confidence[Metric.Significant],
+    shuffle_samples: bool = False,
+    dtype: Optional[np.dtype] = None,
+) -> InputType:
+    r"""Compute significant digits
 
     Parameters
     ----------
     array: InputType
         Element to compute
     reference: Optional[ReferenceType], optional=None
         Reference for comparing the array
@@ -480,14 +496,17 @@
         Probability for the significant digits result
     confidence : float, default=0.95
         Confidence level for the significant digits result
     shuffle_samples : bool, optional=False
         If reference is None, the array is split in two and \
         comparison is done between both pieces. \
         If shuffle_samples is True, it shuffles pieces.
+    dtype : np.dtype, default=None
+        Numerical type used for computing contributing digits
+        Widest format between array and reference is taken if no supplied.
 
     Returns
     -------
     ndarray
         array_like containing contributing digits
 
     See Also
@@ -500,54 +519,63 @@
     Notes
     -----
     .. [1] Sohier, D., Castro, P. D. O., Févotte, F.,
     Lathuilière, B., Petit, E., & Jamond, O. (2021).
     Confidence intervals for stochastic arithmetic.
     ACM Transactions on Mathematical Software (TOMS), 47(2), 1-33.
 
-    '''
+    """
     assert_is_probability(probability)
     assert_is_confidence(confidence)
     assert_is_valid_method(method)
     assert_is_valid_error(error)
 
     significant = None
 
     array, reference = preprocess_inputs(array, reference)
 
     if method == Method.CNH:
-        significant = significant_digits_cnh(array=array,
-                                             reference=reference,
-                                             error=error,
-                                             probability=probability,
-                                             confidence=confidence,
-                                             axis=axis,
-                                             shuffle_samples=shuffle_samples)
+        significant = significant_digits_cnh(
+            array=array,
+            reference=reference,
+            error=error,
+            probability=probability,
+            confidence=confidence,
+            axis=axis,
+            shuffle_samples=shuffle_samples,
+            dtype=dtype,
+        )
 
     elif method == Method.General:
-        significant = significant_digits_general(array=array,
-                                                 reference=reference,
-                                                 error=error,
-                                                 axis=axis,
-                                                 shuffle_samples=shuffle_samples)
+        significant = significant_digits_general(
+            array=array,
+            reference=reference,
+            error=error,
+            axis=axis,
+            shuffle_samples=shuffle_samples,
+            dtype=dtype,
+        )
 
     if base != 2:
-        significant = change_base(significant, base)
+        significant = change_basis(significant, base)
 
     return significant
 
 
-def contributing_digits_cnh(array: InputType,
-                            reference: Optional[ReferenceType],
-                            axis: int,
-                            error: Union[Error, str],
-                            probability: float,
-                            confidence: float,
-                            shuffle_samples: bool = False) -> InputType:
-    r'''Compute contributing digits for Centered Hypothesis Normality
+def contributing_digits_cnh(
+    array: InputType,
+    reference: Optional[ReferenceType],
+    axis: int,
+    error: Union[Error, str],
+    probability: float,
+    confidence: float,
+    shuffle_samples: bool = False,
+    dtype: Optional[np.dtype] = None,
+) -> InputType:
+    r"""Compute contributing digits for Centered Hypothesis Normality
 
     Parameters
     ----------
     array: InputType
         Element to compute
     reference: Optional[ReferenceType]
         Reference for comparing the array
@@ -559,14 +587,17 @@
         Probability for the contributing digits result
     confidence : float
         Confidence level for the contributing digits result
     shuffle_samples : bool, default=False
         If reference is None, the array is split in two and
         comparison is done between both pieces.
         If shuffle_samples is True, it shuffles pieces.
+    dtype : np.dtype, default=None
+        Numerical type used for computing contributing digits
+        Widest format between array and reference is taken if no supplied.
 
     Returns
     -------
     ndarray
         array_like containing contributing digits
 
     See Also
@@ -581,39 +612,41 @@
     .. [1] Sohier, D., Castro, P. D. O., Févotte, F.,
     Lathuilière, B., Petit, E., & Jamond, O. (2021).
     Confidence intervals for stochastic arithmetic.
     ACM Transactions on Mathematical Software (TOMS), 47(2), 1-33.
 
     .. math::
         c >= -log_2(std) - [\frac{1}{2} log_2( \frac{n-1} / \frac{ Chi^2_{1-\frac{alpha}{2}} }) ) + log_2(p+\frac{1}{2}) + log_2(2\sqrt{2\pi})]
-    '''
-    z = compute_z(array, reference, error, axis=axis,
-                  shuffle_samples=shuffle_samples)
+    """
+    z = compute_z(array, reference, error, axis=axis, shuffle_samples=shuffle_samples)
     nb_samples = z.shape[axis]
     std = np.std(z, axis=axis, dtype=internal_dtype)
-    std0 = np.ma.masked_array(std == 0)
+    std0 = np.ma.masked_array(std, mask=std == 0)
     chi2 = scipy.stats.chi2.interval(confidence, nb_samples - 1)[0]
-    delta_chn = 0.5 * np.log2((nb_samples - 1)/chi2) + \
-        np.log2(probability - 0.5) + np.log2(2 * np.sqrt(2 * np.pi))
-    contributing = -np.log2(std) - delta_chn
-    if contributing.ndim != 0:
-        contributing[std0] = np.finfo(z.dtype).nmant - delta_chn
-    elif std0:
-        contributing = np.finfo(z.dtype).nmant - delta_chn
-
+    delta_chn = (
+        0.5 * np.log2((nb_samples - 1) / chi2)
+        + np.log2(probability - 0.5)
+        + np.log2(2 * np.sqrt(2 * np.pi))
+    )
+    contributing = -np.ma.log2(std0) - delta_chn
+    max_bits = np.finfo(dtype if dtype else z.dtype).nmant
+    contributing = contributing.filled(fill_value=max_bits - delta_chn)
     return contributing
 
 
-def contributing_digits_general(array: InputType,
-                                reference: Optional[ReferenceType],
-                                axis: int,
-                                error: Union[Error, str],
-                                probability: float,
-                                shuffle_samples: bool = False) -> InputType:
-    r'''Computes contributing digits for unknown underlying distribution
+def contributing_digits_general(
+    array: InputType,
+    reference: Optional[ReferenceType],
+    axis: int,
+    error: Union[Error, str],
+    probability: float,
+    shuffle_samples: bool = False,
+    dtype: Optional[np.dtype] = None,
+) -> InputType:
+    r"""Computes contributing digits for unknown underlying distribution
 
     This function computes with a certain probability the number of bits
     of the mantissa that will round the result towards the correct reference
     value[1]_
 
     Parameters
     ----------
@@ -627,15 +660,17 @@
         The error function to use to compute error between array and reference.
     probability : float
         Probability for the contributing digits result
     shuffle_samples : bool, default=False
         If reference is None, the array is split in two and
         comparison is done between both pieces.
         If shuffle_samples is True, it shuffles pieces.
-
+    dtype : np.dtype, default=None
+        Numerical type used for computing contributing digits
+        Widest format between array and reference is taken if no supplied.
     Returns
     -------
     ndarray
         array_like containing contributing digits
 
     See Also
     --------
@@ -650,46 +685,55 @@
     Lathuilière, B., Petit, E., & Jamond, O. (2021).
     Confidence intervals for stochastic arithmetic.
     ACM Transactions on Mathematical Software (TOMS), 47(2), 1-33.
 
     .. math::
         C^{i_k} = "\lfloor 2^k|Z_i|  \rfloor is even"
         c = (\frac{#success}{#trials} > p)
-    '''
+    """
 
-    z = compute_z(array, reference, error, axis=axis,
-                  shuffle_samples=shuffle_samples)
-    nb_samples = z.shape[axis]
+    z = compute_z(array, reference, error, axis=axis, shuffle_samples=shuffle_samples)
     sample_shape = tuple(dim for i, dim in enumerate(z.shape) if i != axis)
-    contributing = np.zeros(sample_shape)
-    contributing = np.zeros(
-        [dim for i, dim in enumerate(z.shape) if i != axis])
-    max_bits = np.finfo(z.dtype).nmant
-    z_mask = np.full(sample_shape, fill_value=True)
+    max_bits = np.finfo(dtype if dtype else z.dtype).nmant
+    contributing = np.ma.MaskedArray(
+        data=np.full(shape=sample_shape, fill_value=1, dtype=np.int8), mask=False
+    )
 
     for k in range(1, max_bits + 1):
-        pow2k = np.power(2, k)
-        successes = np.floor(pow2k * np.abs(z)) % 2 == 0
-        _z = np.sum(successes, axis=axis) / nb_samples
-        z_mask = z_mask & (_z > probability)
-        contributing[z_mask] = k
+        # scale = ldexp(x,n) = x * 2^n
+        # floor(scale) & 1 : returns 1 if scale is even
+        # taking the max to check if at least one result is even
+        # Get the negation to have success as boolean
+        successes = np.logical_not(
+            np.max(
+                np.bitwise_and(np.floor(np.abs(np.ldexp(z, k))).astype(np.int64), 1),
+                axis=axis,
+            )
+        )
+        contributing.mask |= np.ma.logical_not(successes)
+        contributing[np.logical_not(contributing.mask)] = k
+        if np.all(contributing.mask):
+            break
 
-    return contributing
+    return contributing.data
 
 
-def contributing_digits(array: InputType,
-                        reference: Optional[ReferenceType] = None,
-                        axis: int = 0,
-                        base: int = 2,
-                        error: Union[str, Error] = Error.Relative,
-                        method: Union[str, Method] = Method.CNH,
-                        probability: float = default_probability[Metric.Contributing],
-                        confidence: float = default_confidence[Metric.Contributing],
-                        shuffle_samples: bool = False) -> InputType:
-    r'''Compute contributing digits
+def contributing_digits(
+    array: InputType,
+    reference: Optional[ReferenceType] = None,
+    axis: int = 0,
+    base: int = 2,
+    error: Union[str, Error] = Error.Relative,
+    method: Union[str, Method] = Method.CNH,
+    probability: float = default_probability[Metric.Contributing],
+    confidence: float = default_confidence[Metric.Contributing],
+    shuffle_samples: bool = False,
+    dtype: Optional[np.dtype] = None,
+) -> InputType:
+    r"""Compute contributing digits
 
 
     This function computes with a certain probability the number of bits
     of the mantissa that will round the result towards the correct reference
     value[1]_
 
     Parameters
@@ -709,15 +753,17 @@
         Probability for the contributing digits result
     confidence : float, default=0.95
         Confidence level for the contributing digits result
     shuffle_samples : bool, default=False
         If reference is None, the array is split in two and
         comparison is done between both pieces.
         If shuffle_samples is True, it shuffles pieces.
-
+    dtype : np.dtype, default=None
+        Numerical type used for computing contributing digits
+        Widest format between array and reference is taken if no supplied.
     Returns
     -------
     ndarray
         array_like containing contributing digits
 
     See Also
     --------
@@ -729,52 +775,58 @@
     Notes
     -----
     .. [1] Sohier, D., Castro, P. D. O., Févotte, F.,
     Lathuilière, B., Petit, E., & Jamond, O. (2021).
     Confidence intervals for stochastic arithmetic.
     ACM Transactions on Mathematical Software (TOMS), 47(2), 1-33.
 
-    '''
+    """
 
     assert_is_probability(probability)
     assert_is_confidence(confidence)
     assert_is_valid_method(method)
     assert_is_valid_error(error)
 
     contributing = None
 
     array, reference = preprocess_inputs(array, reference)
 
     if method == Method.CNH:
-        contributing = contributing_digits_cnh(array=array,
-                                               reference=reference,
-                                               error=error,
-                                               axis=axis,
-                                               probability=probability,
-                                               confidence=confidence,
-                                               shuffle_samples=shuffle_samples)
+        contributing = contributing_digits_cnh(
+            array=array,
+            reference=reference,
+            error=error,
+            axis=axis,
+            probability=probability,
+            confidence=confidence,
+            shuffle_samples=shuffle_samples,
+            dtype=dtype,
+        )
 
     elif method == Method.General:
-        contributing = contributing_digits_general(array=array,
-                                                   reference=reference,
-                                                   error=error,
-                                                   axis=axis,
-                                                   probability=probability,
-                                                   shuffle_samples=shuffle_samples)
+        contributing = contributing_digits_general(
+            array=array,
+            reference=reference,
+            error=error,
+            axis=axis,
+            probability=probability,
+            shuffle_samples=shuffle_samples,
+            dtype=dtype,
+        )
 
     if base != 2:
-        contributing = change_base(contributing, base)
+        contributing = change_basis(contributing, base)
 
     return contributing
 
 
-def probability_estimation_bernoulli(success: int,
-                                     trials: int,
-                                     confidence: float) -> float:
-    r'''Computes probability lower bound for Bernoulli process
+def probability_estimation_bernoulli(
+    success: int, trials: int, confidence: float
+) -> float:
+    r"""Computes probability lower bound for Bernoulli process
 
     This function computes the probability associated with metrics
     computed in the general case (without assumption on the underlying
     distribution). Indeed, in that case the probability is given by the
     sample size with a certain confidence level.
 
     Parameters
@@ -785,44 +837,46 @@
         Number of trials for a Bernoulli experiment
     confidence : float
         Confidence level for the probability lower bound estimation
 
     Returns
     -------
     float
-        The lower bound probability with `confidence` level to have `success` successes for `trials` trials
+        The lower bound probability with `confidence` level to have `success`
+        successes for `trials` trials
 
 
     Notes
     -----
     .. [1] Sohier, D., Castro, P. D. O., Févotte, F.,
     Lathuilière, B., Petit, E., & Jamond, O. (2021).
     Confidence intervals for stochastic arithmetic.
     ACM Transactions on Mathematical Software (TOMS), 47(2), 1-33.
 
     .. math::
         p = 1 + \frac{\log{ 1 - \alpha }}{n} if success=sample\_size
         p = \frac{s+2}{s+4} - F^{-1}(\frac{p+1}{2}) \sqrt{ \frac{(s+2)(n-s+2)}{n+4}^3  } else
-    '''
+    """
     s = success
     n = trials
     coef = scipy.stats.norm.ppf(confidence)
 
     if s == n:
         # Special case when having only successes
         probability = 1 + np.log(1 - confidence) / n
     else:
-        probability = (s + 2) / (n + 4) - coef * \
-            np.sqrt((s + 2) * (n - s + 2) / (n + 4)**3)
+        probability = (s + 2) / (n + 4) - coef * np.sqrt(
+            (s + 2) * (n - s + 2) / (n + 4) ** 3
+        )
 
     return probability
 
 
 def minimum_number_of_trials(probability: float, confidence: float) -> int:
-    r'''Computes the minimum number of trials to have probability and confidence
+    r"""Computes the minimum number of trials to have probability and confidence
 
     This function computes the minimal sample size required to have
     metrics with a certain probability and confidence for the general case
     (without assumption on the underlying distribution).
 
     For example, if one wants significant digits with proabability p = 99%
     and confidence (1 - alpha) = 95%, it requires at least 299 observations.
@@ -845,11 +899,11 @@
     Lathuilière, B., Petit, E., & Jamond, O. (2021).
     Confidence intervals for stochastic arithmetic.
     ACM Transactions on Mathematical Software (TOMS), 47(2), 1-33.
 
     .. math::
         n = \lceil \frac{\ln{\alpha}}{\ln{p}}
 
-    '''
+    """
     alpha = 1 - confidence
     n = np.log(alpha) / np.log(probability)
     return int(np.ceil(n))
```

### Comparing `significantdigits-0.1.2/significantdigits/args.py` & `significantdigits-0.1.3/significantdigits/args.py`

 * *Files identical despite different names*

### Comparing `significantdigits-0.1.2/significantdigits/conftest.py` & `significantdigits-0.1.3/significantdigits/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,99 +4,104 @@
 import sys
 
 import numpy as np
 import pytest
 
 import significantdigits
 import significantdigits.args
+from significantdigits.test.utils import Setup
 
 
 class Save:
+    def __init__(self):
+        self.setup = Setup()
 
     def save(self, outputs, samples):
-        np.save(outputs, samples)
-        assert(os.path.isfile(outputs))
+        filename = self.setup.get_numpy_data_path(outputs)
+        np.save(filename, samples)
+        assert os.path.isfile(filename)
 
 
 class Load:
+    def __init__(self):
+        self.setup = Setup()
 
     def load(self, inputs):
-        assert(os.path.isfile(inputs))
-        return np.load(inputs)
+        filename = self.setup.get_numpy_data_path(inputs)
+        assert os.path.isfile(filename)
+        return np.load(filename)
 
 
 class RunFuzzyTest:
-
-    def run(self, nsamples, function, *args, **kwargs):
-        return [function(*args, **kwargs) for _ in range(nsamples)]
+    def run(self, samples, function, *args, **kwargs):
+        return [function(*args, **kwargs) for _ in range(samples)]
 
 
 class RunMetricDigitsTest:
-
-    available_metrics = ['significant', 'contributing']
+    available_metrics = ["significant", "contributing"]
 
     def __init__(self, metric):
+        self.setup = Setup()
         self.metric = self.check_metric(metric)
         self.bases = [2, 10]
         self.methods = significantdigits.Method
         self.errors = significantdigits.Error
+        self.writer = None
 
     def check_metric(self, metric):
         if metric in self.available_metrics:
             return metric
         else:
-            print((f'Unknown metric {metric}.'
-                   f' Must be one of {self.available_metrics}'))
+            print(
+                (
+                    f"Unknown metric {metric}."
+                    f" Must be one of {self.available_metrics}"
+                )
+            )
             sys.exit(1)
 
     def compute_significant_digits(self, x, ref, error, method, base):
         return significantdigits.significant_digits(
-            x, ref, error=error, method=method, base=base)
+            x, ref, error=error, method=method, base=base
+        )
 
     def compute_contributing_digits(self, x, ref, error, method, base):
         return significantdigits.contributing_digits(
-            x, ref, error=error, method=method, base=base)
+            x, ref, error=error, method=method, base=base
+        )
 
     def compute_metric(self, *args, **kwargs):
-        if self.metric == 'significant':
+        if self.metric == "significant":
             return self.compute_significant_digits(*args, **kwargs)
         else:
             return self.compute_contributing_digits(*args, **kwargs)
 
     def save_result(self, metric, error, method, base):
-        result = dict(Method=method,
-                      Error=error,
-                      Base=base,
-                      Metric=metric)
+        result = {"Method": method, "Error": error, "Base": base, "Metric": metric}
         self.writer.writerow(result.values())
 
     def run(self, output, x, ref):
-        header = ['Method', 'Error', 'Base', self.metric.capitalize()]
-        with open(output, 'w') as fo:
+        header = ["Method", "Error", "Base", self.metric.capitalize()]
+        filename = self.setup.get_report_path(output)
+        with open(filename, "a", encoding="utf-8") as fo:
             self.writer = csv.writer(fo)
             self.writer.writerow(header)
-            configurations = itertools.product(self.bases,
-                                               self.methods,
-                                               self.errors)
-            for (base, method, error) in configurations:
-                metric = self.compute_metric(x,
-                                             ref,
-                                             error,
-                                             method,
-                                             base)
-                self.save_result(metric,
-                                 error,
-                                 method,
-                                 base)
+            configurations = itertools.product(self.bases, self.methods, self.errors)
+            for base, method, error in configurations:
+                metric = self.compute_metric(x, ref, error, method, base)
+                self.save_result(metric, error, method, base)
 
 
 def pytest_addoption(parser):
     parser.addoption(
-        "--nsamples", action="store", type=int, default=3,
-        help="Number of samples to run"
+        "--nsamples",
+        action="store",
+        type=int,
+        default=3,
+        help="Number of samples to run",
     )
 
 
 @pytest.fixture
 def nsamples(request):
     return request.config.getoption("--nsamples")
 
@@ -104,20 +109,20 @@
 @pytest.fixture
 def run_fuzzy(request):
     return RunFuzzyTest()
 
 
 @pytest.fixture
 def run_significant_digits(request):
-    return RunMetricDigitsTest('significant')
+    return RunMetricDigitsTest("significant")
 
 
 @pytest.fixture
 def run_contributing_digits(request):
-    return RunMetricDigitsTest('contributing')
+    return RunMetricDigitsTest("contributing")
 
 
 @pytest.fixture
 def save(request):
     return Save()
```

### Comparing `significantdigits-0.1.2/significantdigits/export/numpy.py` & `significantdigits-0.1.3/significantdigits/export/numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from significantdigits.export.generic import Exporter, Parser
 
 import numpy as np
 
 
 class NumpyParser(Parser):
-
     def parse(self, *args, **kwargs):
-        filename = kwargs.get('filename', args[0])
+        filename = kwargs.get("filename", args[0])
         return np.load(filename, allow_pickle=True)
 
 
 class NumpyExporter(Exporter):
-
     def __init__(self, *args, **kwargs):
-        filename = kwargs.get('filename', args[0])
+        filename = kwargs.get("filename", args[0])
         self.filename = filename
 
     def export(self, *args, **kwargs):
-        values = kwargs.get('values', args)
+        values = kwargs.get("values", args)
         np.save(self.filename, values)
```

### Comparing `significantdigits-0.1.2/significantdigits/export/stdin.py` & `significantdigits-0.1.3/significantdigits/export/stdin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from significantdigits.export.generic import Exporter, Parser
 
 import numpy as np
 
 
 class StdinParser(Parser):
-
     def parse(self, *args, **kwargs):
-        values = kwargs.get('values', *args)
-        dtype = kwargs.get('dtype', np.float64)
+        values = kwargs.get("values", *args)
+        dtype = kwargs.get("dtype", np.float64)
         return np.asarray(values, dtype=dtype)
 
 
 class StdinExporter(Exporter):
-
     def __init__(self, *args, **kwargs):
-        filename = kwargs.get('filename', args[0])
+        filename = kwargs.get("filename", args[0])
         self.filename = filename
 
     def export(self, *args, **kwargs):
-        values = kwargs.get('values', args)
+        values = kwargs.get("values", args)
         print(values)
```

### Comparing `significantdigits-0.1.2/significantdigits/src/float_const.h` & `significantdigits-0.1.3/significantdigits/src/float_const.h`

 * *Files identical despite different names*

### Comparing `significantdigits-0.1.2/significantdigits/src/float_struct.h` & `significantdigits-0.1.3/significantdigits/src/float_struct.h`

 * *Files identical despite different names*

### Comparing `significantdigits-0.1.2/significantdigits/src/truncation.c` & `significantdigits-0.1.3/significantdigits/src/truncation.c`

 * *Files identical despite different names*

### Comparing `significantdigits-0.1.2/significantdigits/src/truncation.py` & `significantdigits-0.1.3/significantdigits/src/truncation.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,15 @@
         fp_f64 = ctypes.c_double(x)
         fp_trunc = truncation_clib.truncate_binary64(fp_f64, n)
     else:
         raise TypeError(type(x))
     return fp_trunc
 
 
-if __name__ == '__main__':
-
+if __name__ == "__main__":
     x16 = np.float16(0.9995)
     print("Truncation for float16:", x16)
     for i in range(11):
         print(i, f"{truncate(x16, i):.4f}")
 
     x32 = np.float32(0.99999994)
     print("Truncation for float32:", x32)
```

### Comparing `significantdigits-0.1.2/significantdigits/stats/__init__.py` & `significantdigits-0.1.3/significantdigits/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `significantdigits-0.1.2/significantdigits/stats/dense.py` & `significantdigits-0.1.3/significantdigits/stats/dense.py`

 * *Files identical despite different names*

### Comparing `significantdigits-0.1.2/significantdigits/stats/sparse.py` & `significantdigits-0.1.3/significantdigits/stats/sparse.py`

 * *Files identical despite different names*

### Comparing `significantdigits-0.1.2/significantdigits/test/test_cramer.py` & `significantdigits-0.1.3/significantdigits/test/test_cramer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 #!/usr/bin/python3
 
 import numpy as np
-from significantdigits.test.utils import (
-    get_numpy_data_path, get_report_data_path)
 
 
 class TestCramer:
-    '''Solving 2x2 system a.x=b with Cramer's rule'''
+    """Solving 2x2 system a.x=b with Cramer's rule"""
 
-    filename_npy = get_numpy_data_path('cramer.npy')
-    filename_csv = get_report_data_path('cramer.csv')
+    filename = "cramer"
     a = np.array([[0.2161, 0.1441], [1.2969, 0.8648]])
     b = np.array([0.1440, 0.8642])
     args = (a, b)
 
     def cramer(self, a, b):
         det = a[0, 0] * a[1, 1] - a[1, 0] * a[0, 1]
         det0 = b[0] * a[1, 1] - b[1] * a[0, 1]
         det1 = a[0, 0] * b[1] - a[1, 0] * b[0]
         return np.array([det0 / det, det1 / det])
 
     def test_fuzzy(self, run_fuzzy, nsamples, save):
         samples = run_fuzzy.run(nsamples, self.cramer, *self.args)
-        save.save(self.filename_npy, samples)
+        save.save(self.filename, samples)
 
     def test_significant_digits(self, load, run_significant_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = np.array([2, -2])
-        run_significant_digits.run(self.filename_csv, x, ref)
+        run_significant_digits.run(self.filename, x, ref)
 
     def test_contributing_digits(self, load, run_contributing_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = np.array([2, -2])
-        run_contributing_digits.run(self.filename_csv, x, ref)
+        run_contributing_digits.run(self.filename, x, ref)
```

### Comparing `significantdigits-0.1.2/significantdigits/test/test_higham.py` & `significantdigits-0.1.3/significantdigits/test/test_higham.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 #!/usr/bin/python3
 
 import numpy as np
-from significantdigits.test.utils import (
-    get_numpy_data_path, get_report_data_path)
+from significantdigits.test.utils import Setup
 
+setup = Setup()
 
-class TestDotProduct:
 
-    filename_csv = get_numpy_data_path('higham_dot_product.csv')
-    filename_npy = get_report_data_path('higham_dot_product.npy')
+class TestDotProduct:
+    filename = "higham_dot_product"
     args = [10**i for i in range(2, 6)]
 
     def dot_product(self, sizes):
         results = []
         for size in sizes:
-            x = np.random.random_sample(size)
-            y = np.random.random_sample(size)
+            x = setup.rng.random_sample(size)
+            y = setup.rng.random_sample(size)
             z = np.dot(x, y)
             results.append(z)
         return results
 
     def test_fuzzy(self, run_fuzzy, nsamples, save):
         samples = run_fuzzy.run(nsamples, self.dot_product, self.args)
-        save.save(self.filename_npy, samples)
+        save.save(self.filename, samples)
 
     def test_significant_digits(self, load, run_significant_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = np.mean(x, axis=0)
-        run_significant_digits.run(self.filename_csv, x, ref)
+        run_significant_digits.run(self.filename, x, ref)
 
     def test_contributing_digits(self, load, run_contributing_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = np.mean(x, axis=0)
-        run_contributing_digits.run(self.filename_csv, x, ref)
+        run_contributing_digits.run(self.filename, x, ref)
```

### Comparing `significantdigits-0.1.2/significantdigits/test/test_parker.py` & `significantdigits-0.1.3/significantdigits/test/test_parker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,82 @@
 #!/usr/bin/python3
 
 import math
 
 import numpy as np
 import scipy.linalg
-from significantdigits.test.utils import (
-    get_numpy_data_path, get_report_data_path)
 
 # Set of tests taken from:
 # Parker, Douglas Stott, Brad Pierce, and Paul R. Eggert.
 # "Monte Carlo arithmetic: how to gamble with floating point and win."
 # Computing in Science & Engineering 2.4 (2000): 58-68.
 
 
 class TestDiscriminant:
-    '''Solving quadratic equation using discriminant
-        due to W. Kahan
-    '''
-    filename_npy = get_numpy_data_path('parker_descriminant.npy')
-    filename_csv = get_report_data_path('parker_descriminant.csv')
+    """Solving quadratic equation using discriminant
+    due to W. Kahan
+    """
+
+    filename = "parker_descriminant"
     args = (7, -8686, 2)
 
     def discriminant(self, a, b, c):
         return (-b - math.sqrt(b * b - 4 * a * c)) / (2 * a)
 
     def test_fuzzy(self, run_fuzzy, nsamples, save):
         samples = run_fuzzy.run(nsamples, self.discriminant, *self.args)
-        save.save(self.filename_npy, samples)
+        save.save(self.filename, samples)
 
     def test_significant_digits(self, load, run_significant_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = np.mean(x, axis=0)
-        run_significant_digits.run(self.filename_csv, x, ref)
+        run_significant_digits.run(self.filename, x, ref)
 
     def test_contributing_digits(self, load, run_contributing_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = np.mean(x, axis=0)
-        run_contributing_digits.run(self.filename_csv, x, ref)
+        run_contributing_digits.run(self.filename, x, ref)
 
 
 class TestCancellation:
-    '''Simple example illustrating catastrophic cancellation
+    """Simple example illustrating catastrophic cancellation
     due to non-associativity.
-    '''
+    """
 
-    filename_npy = get_numpy_data_path('parker_cancellation.npy')
-    filename_csv = get_report_data_path('parker_cancellation.csv')
+    filename = "parker_cancellation"
 
     def cancellation(self):
         x = (11111113 - 11111111) + 7.5111111
         y = 11111113 + (-11111111 + 7.5111111)
         return np.array([x, y])
 
     def test_fuzzy(self, run_fuzzy, nsamples, save):
         samples = run_fuzzy.run(nsamples, self.cancellation)
-        save.save(self.filename_npy, samples)
+        save.save(self.filename, samples)
 
     def test_significant_digits(self, load, run_significant_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = [9.5111111, 9.5111111]
-        run_significant_digits.run(self.filename_csv, x, ref)
+        run_significant_digits.run(self.filename, x, ref)
 
     def test_contributing_digits(self, load, run_contributing_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = [9.5111111, 9.5111111]
-        run_contributing_digits.run(self.filename_csv, x, ref)
+        run_contributing_digits.run(self.filename, x, ref)
 
 
 class TestMuller:
-
-    filename_npy = get_numpy_data_path('parker_muller.npy')
-    filename_csv = get_report_data_path('parker_muller.csv')
+    filename = "parker_muller"
 
     args = (1.510005072139, 30)
 
     def muller(self, x0, n):
-
         def sequence(x_k):
-            num = (3 * x_k ** 4 - 20 * x_k ** 3 + 35 * x_k ** 2 - 24)
-            den = (4 * x_k ** 3 - 30 * x_k ** 2 + 70 * x_k - 50)
+            num = 3 * x_k**4 - 20 * x_k**3 + 35 * x_k**2 - 24
+            den = 4 * x_k**3 - 30 * x_k**2 + 70 * x_k - 50
             return num / den
 
         x_k0 = x0
         x_k1 = x_k0
 
         results = []
 
@@ -90,81 +84,125 @@
             results.append(x_k1)
             x_k1, x_k0 = sequence(x_k0), x_k1
 
         return results
 
     def test_fuzzy(self, run_fuzzy, nsamples, save):
         samples = run_fuzzy.run(nsamples, self.muller, *self.args)
-        save.save(self.filename_npy, samples)
+        save.save(self.filename, samples)
 
     def test_significant_digits(self, load, run_significant_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = np.mean(x, axis=0)
-        run_significant_digits.run(self.filename_csv, x, ref)
+        run_significant_digits.run(self.filename, x, ref)
 
     def test_contributing_digits(self, load, run_contributing_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = np.mean(x, axis=0)
-        run_contributing_digits.run(self.filename_csv, x, ref)
+        run_contributing_digits.run(self.filename, x, ref)
 
 
 class TestTchebycheff:
-
-    filename_npy = get_numpy_data_path('parker_tchebycheff.npy')
-    filename_csv = get_numpy_data_path('parker_tchebycheff.csv')
+    filename = "parker_tchebycheff"
     args = np.linspace(0, 1, 100)
 
     def tchebycheff(self, z):
-        coeffs = np.array([524288, -2621440, 5570560, -6553600,
-                           4659200, -2050048, 549120, -84480, 6600, -200, 1])
+        coeffs = np.array(
+            [
+                524288,
+                -2621440,
+                5570560,
+                -6553600,
+                4659200,
+                -2050048,
+                549120,
+                -84480,
+                6600,
+                -200,
+                1,
+            ]
+        )
         power = np.array([20, 18, 16, 14, 12, 10, 8, 6, 4, 2, 0])
-        def t_20(x): return np.sum(coeffs * x ** power)
+
+        def t_20(x):
+            return np.sum(coeffs * x**power)
+
         return np.array(list(map(t_20, z)))
 
     def test_fuzzy(self, run_fuzzy, nsamples, save):
         samples = run_fuzzy.run(nsamples, self.tchebycheff, self.args)
-        save.save(self.filename_npy, samples)
+        save.save(self.filename, samples)
 
     def test_significant_digits(self, load, run_significant_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = np.cos(20 * np.arccos(self.args))
-        run_significant_digits.run(self.filename_csv, x, ref)
+        run_significant_digits.run(self.filename, x, ref)
 
     def test_contributing_digits(self, load, run_contributing_digits):
         args = self.args
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = np.cos(20 * np.arccos(args))
-        run_contributing_digits.run(self.filename_csv, x, ref)
+        run_contributing_digits.run(self.filename, x, ref)
 
 
 class TestGaussian:
-
-    filename_npy = get_numpy_data_path('parker_gaussian.npy')
-    filename_csv = get_numpy_data_path('parker_gaussian.csv')
+    filename = "parker_gaussian"
     args = 24
 
     def turing_matrix(self, n):
-        T = np.eye(n)
-        T[:, -1] = np.array([2**i for i in range(n)])
-        return T
+        t = np.eye(n)
+        t[:, -1] = np.array([2**i for i in range(n)])
+        return t
+
+    def reference(self, n):
+        return np.array([2**-i for i in range(n)])
+
+    def gaussian(self, n):
+        a = self.turing_matrix(n)
+        b = np.full(n, 1)
+        return scipy.linalg.solve(a, b)
+
+    def test_fuzzy(self, run_fuzzy, nsamples, save):
+        samples = run_fuzzy.run(nsamples, self.gaussian, self.args)
+        save.save(self.filename, samples)
+
+    def test_significant_digits(self, load, run_significant_digits):
+        x = load.load(self.filename)
+        ref = self.reference(self.args)
+        run_significant_digits.run(self.filename, x, ref)
+
+    def test_contributing_digits(self, load, run_contributing_digits):
+        x = load.load(self.filename)
+        ref = self.reference(self.args)
+        run_contributing_digits.run(self.filename, x, ref)
+
+
+class TestGaussianLarge:
+    filename = "parker_gaussian"
+    args = 1000
+
+    def turing_matrix(self, n):
+        t = np.eye(n)
+        t[:, -1] = np.array([2**i for i in range(n)])
+        return t
 
     def reference(self, n):
-        return np.array([2**-i for i in range(self.args)])
+        return np.array([2**-i for i in range(n)])
 
     def gaussian(self, n):
-        A = self.turing_matrix(n)
+        a = self.turing_matrix(n)
         b = np.full(n, 1)
-        return scipy.linalg.solve(A, b)
+        return scipy.linalg.solve(a, b)
 
     def test_fuzzy(self, run_fuzzy, nsamples, save):
         samples = run_fuzzy.run(nsamples, self.gaussian, self.args)
-        save.save(self.filename_npy, samples)
+        save.save(self.filename, samples)
 
     def test_significant_digits(self, load, run_significant_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = self.reference(self.args)
-        run_significant_digits.run(self.filename_csv, x, ref)
+        run_significant_digits.run(self.filename, x, ref)
 
     def test_contributing_digits(self, load, run_contributing_digits):
-        x = load.load(self.filename_npy)
+        x = load.load(self.filename)
         ref = self.reference(self.args)
-        run_contributing_digits.run(self.filename_csv, x, ref)
+        run_contributing_digits.run(self.filename, x, ref)
```

### Comparing `significantdigits-0.1.2/.gitignore` & `significantdigits-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `significantdigits-0.1.2/LICENSE` & `significantdigits-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `significantdigits-0.1.2/README.md` & `significantdigits-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# significantdigits package - v0.1.2
+# significantdigits package - v0.1.3
 
 Compute the number of significant digits based on the paper [Confidence Intervals for Stochastic Arithmetic](https://arxiv.org/abs/1807.09655).
-This package is also inspired from the [Jupyter notebook](https://github.com/interflop/stochastic-confidence-intervals/blob/master/Intervals.ipynb) included with the publication.
+This package is also inspired by the [Jupyter Notebook](https://github.com/interflop/stochastic-confidence-intervals/blob/master/Intervals.ipynb) included with the publication.
 
 ## Getting started
 
 This synthetic example illustrates how to compute significant digits
 of a results sample with a given known reference:
 
 ```python
@@ -35,40 +35,35 @@
 ```
 ## Installation
 
 ```bash
     python3 -m pip install -U significantdigits
 ```
 
-or if you want the lastest version of the code, you can install from
-the repository directly
+or if you want the latest version of the code, you can install it **from** the repository directly
 
 ```bash
     python3 -m pip install -U git+https://github.com/verificarlo/significantdigits.git
     # or if you don't have 'git' installed
     python3 -m pip install -U https://github.com/verificarlo/significantdigits/zipball/master
 ```
 
 ## Advanced Usage
 
 ### Inputs types
 
-Functions accept the following types for the inputs:
+Functions accept the following types of inputs:
 ```python
     InputType: np.ndarray | tuple | list
 ```
 Those types are accessible with the `get_input_type` function.
 
 ### Z computation
-
-Metric are computed using Z, the distance
-between the samples and the reference.
-They are four possible cases depending on the
-distance and the nature of the reference that are
-summarized in this table:
+Metrics are computed using Z, the distance between the samples and the reference.
+They are four possible cases depending on the distance and the nature of the reference that is summarized in this table:
 
 |                    | constant reference (x) | random variable reference (Y) |
 | ------------------ | ---------------------- | ----------------------------- |
 | Absolute precision | Z = X - x              | Z = X - Y                     |
 | Relative precision | Z = X/x - 1            | Z = X/Y - 1                   |
 
 
@@ -108,16 +103,15 @@
     -------
     array : numpy.ndarray
         The result of Z following the error method choose
 ```
 
 ### Methods
 
-Two methods exist for computing both significant and contributing digits
-depending on wether the sample follow a Centered Normal distribution or not.
+Two methods exist for computing both significant and contributing digits depending on whether the sample follows a Centered Normal distribution or not.
 You can pass the method to the function by using the `Method` enum provided by the package. 
 The functions also accept the name as a string
 `"cnh"` for `Method.CNH` and `"general"` for `Method.General`.
 
 ```python
 class Method(AutoName):
     """
@@ -162,14 +156,17 @@
         Probability for the significant digits result
     confidence : float, default=0.95
         Confidence level for the significant digits result
     shuffle_samples : bool, optional=False
         If reference is None, the array is split in two and \
         comparison is done between both pieces. \
         If shuffle_samples is True, it shuffles pieces.
+    dtype : np.dtype, default=None
+        Numerical type used for computing contributing digits
+        Widest format between array and reference is taken if no supplied.
 
     Returns
     -------
     ndarray
         array_like containing contributing digits
 
 ```
@@ -202,31 +199,34 @@
         Probability for the contributing digits result
     confidence : float, default=0.95
         Confidence level for the contributing digits result
     shuffle_samples : bool, default=False
         If reference is None, the array is split in two and
         comparison is done between both pieces.
         If shuffle_samples is True, it shuffles pieces.
+    dtype : np.dtype, default=None
+        Numerical type used for computing contributing digits
+        Widest format between array and reference is taken if no supplied.
 
     Returns
     -------
     ndarray
         array_like containing contributing digits
 
 ```
-### Utils functions
+### Utils function
 
 These are utility functions for the general case.
 
 `probability_estimation_general`
 allows having an estimation
 on the lower bound probability given the sample size.
 
 `minimum_number_of_trials` gives the minimal sample size
-required to reach requested `probability` and `confidence`.
+required to reach the requested `probability` and `confidence`.
 
 ```python
 probability_estimation_general(success: int, trials: int, confidence: float) -> float
     Computes probability lower bound for Bernouilli process
 
     This function computes the probability associated with metrics
     computed in the general case (without assumption on the underlying
@@ -277,9 +277,9 @@
 ### License
 
 This file is part of the Verificarlo project,
 under the Apache License v2.0 with LLVM Exceptions.
 SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception.
 See https://llvm.org/LICENSE.txt for license information.
 
-Copyright (c) 2020-2022 Verificarlo Contributors
+Copyright (c) 2020-2023 Verificarlo Contributors
```

### Comparing `significantdigits-0.1.2/pyproject.toml` & `significantdigits-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pathspec"]
 build-backend = "hatchling.build"
 
 [project]
 name = "significantdigits"
-version = "0.1.2"
+version = "0.1.3"
 description = "Solid stochastic statistic analysis of Stochastic Arithmetic"
 authors = [
     { name = "Verificarlo contributors", email = "verificarlo@googlegroups.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `significantdigits-0.1.2/PKG-INFO` & `significantdigits-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: significantdigits
-Version: 0.1.2
+Version: 0.1.3
 Summary: Solid stochastic statistic analysis of Stochastic Arithmetic
 Project-URL: Bug Tracker, https://github.com/verificarlo/significantdigits/issues
 Author-email: Verificarlo contributors <verificarlo@googlegroups.com>
 License: Copyright 2022 Verificarlo project
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
@@ -33,18 +33,18 @@
 Requires-Dist: py>=1.10.0
 Requires-Dist: pyparsing>=2.4.7
 Requires-Dist: pytest>=6.2.5
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: toml>=0.10.2
 Description-Content-Type: text/markdown
 
-# significantdigits package - v0.1.2
+# significantdigits package - v0.1.3
 
 Compute the number of significant digits based on the paper [Confidence Intervals for Stochastic Arithmetic](https://arxiv.org/abs/1807.09655).
-This package is also inspired from the [Jupyter notebook](https://github.com/interflop/stochastic-confidence-intervals/blob/master/Intervals.ipynb) included with the publication.
+This package is also inspired by the [Jupyter Notebook](https://github.com/interflop/stochastic-confidence-intervals/blob/master/Intervals.ipynb) included with the publication.
 
 ## Getting started
 
 This synthetic example illustrates how to compute significant digits
 of a results sample with a given known reference:
 
 ```python
@@ -74,40 +74,35 @@
 ```
 ## Installation
 
 ```bash
     python3 -m pip install -U significantdigits
 ```
 
-or if you want the lastest version of the code, you can install from
-the repository directly
+or if you want the latest version of the code, you can install it **from** the repository directly
 
 ```bash
     python3 -m pip install -U git+https://github.com/verificarlo/significantdigits.git
     # or if you don't have 'git' installed
     python3 -m pip install -U https://github.com/verificarlo/significantdigits/zipball/master
 ```
 
 ## Advanced Usage
 
 ### Inputs types
 
-Functions accept the following types for the inputs:
+Functions accept the following types of inputs:
 ```python
     InputType: np.ndarray | tuple | list
 ```
 Those types are accessible with the `get_input_type` function.
 
 ### Z computation
-
-Metric are computed using Z, the distance
-between the samples and the reference.
-They are four possible cases depending on the
-distance and the nature of the reference that are
-summarized in this table:
+Metrics are computed using Z, the distance between the samples and the reference.
+They are four possible cases depending on the distance and the nature of the reference that is summarized in this table:
 
 |                    | constant reference (x) | random variable reference (Y) |
 | ------------------ | ---------------------- | ----------------------------- |
 | Absolute precision | Z = X - x              | Z = X - Y                     |
 | Relative precision | Z = X/x - 1            | Z = X/Y - 1                   |
 
 
@@ -147,16 +142,15 @@
     -------
     array : numpy.ndarray
         The result of Z following the error method choose
 ```
 
 ### Methods
 
-Two methods exist for computing both significant and contributing digits
-depending on wether the sample follow a Centered Normal distribution or not.
+Two methods exist for computing both significant and contributing digits depending on whether the sample follows a Centered Normal distribution or not.
 You can pass the method to the function by using the `Method` enum provided by the package. 
 The functions also accept the name as a string
 `"cnh"` for `Method.CNH` and `"general"` for `Method.General`.
 
 ```python
 class Method(AutoName):
     """
@@ -201,14 +195,17 @@
         Probability for the significant digits result
     confidence : float, default=0.95
         Confidence level for the significant digits result
     shuffle_samples : bool, optional=False
         If reference is None, the array is split in two and \
         comparison is done between both pieces. \
         If shuffle_samples is True, it shuffles pieces.
+    dtype : np.dtype, default=None
+        Numerical type used for computing contributing digits
+        Widest format between array and reference is taken if no supplied.
 
     Returns
     -------
     ndarray
         array_like containing contributing digits
 
 ```
@@ -241,31 +238,34 @@
         Probability for the contributing digits result
     confidence : float, default=0.95
         Confidence level for the contributing digits result
     shuffle_samples : bool, default=False
         If reference is None, the array is split in two and
         comparison is done between both pieces.
         If shuffle_samples is True, it shuffles pieces.
+    dtype : np.dtype, default=None
+        Numerical type used for computing contributing digits
+        Widest format between array and reference is taken if no supplied.
 
     Returns
     -------
     ndarray
         array_like containing contributing digits
 
 ```
-### Utils functions
+### Utils function
 
 These are utility functions for the general case.
 
 `probability_estimation_general`
 allows having an estimation
 on the lower bound probability given the sample size.
 
 `minimum_number_of_trials` gives the minimal sample size
-required to reach requested `probability` and `confidence`.
+required to reach the requested `probability` and `confidence`.
 
 ```python
 probability_estimation_general(success: int, trials: int, confidence: float) -> float
     Computes probability lower bound for Bernouilli process
 
     This function computes the probability associated with metrics
     computed in the general case (without assumption on the underlying
@@ -316,9 +316,9 @@
 ### License
 
 This file is part of the Verificarlo project,
 under the Apache License v2.0 with LLVM Exceptions.
 SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception.
 See https://llvm.org/LICENSE.txt for license information.
 
-Copyright (c) 2020-2022 Verificarlo Contributors
+Copyright (c) 2020-2023 Verificarlo Contributors
```

