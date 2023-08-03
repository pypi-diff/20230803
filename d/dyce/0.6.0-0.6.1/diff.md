# Comparing `tmp/dyce-0.6.0-py3-none-any.whl.zip` & `tmp/dyce-0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 65400 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1197 b- defN 22-Aug-19 02:34 dyce/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 22-Aug-19 02:35 dyce/_version.py
--rw-r--r--  2.0 unx    33729 b- defN 22-Aug-19 02:34 dyce/evaluation.py
--rw-r--r--  2.0 unx    68940 b- defN 22-Aug-19 02:34 dyce/h.py
--rw-r--r--  2.0 unx     2039 b- defN 22-Aug-19 02:34 dyce/lifecycle.py
--rw-r--r--  2.0 unx    42203 b- defN 22-Aug-19 02:34 dyce/p.py
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-19 02:34 dyce/py.typed
--rw-r--r--  2.0 unx    93866 b- defN 22-Aug-19 02:34 dyce/r.py
--rw-r--r--  2.0 unx     4684 b- defN 22-Aug-19 02:34 dyce/rng.py
--rw-r--r--  2.0 unx     2873 b- defN 22-Aug-19 02:34 dyce/types.py
--rw-r--r--  2.0 unx     2132 b- defN 22-Aug-19 02:35 dyce-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    20482 b- defN 22-Aug-19 02:35 dyce-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-19 02:35 dyce-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 22-Aug-19 02:35 dyce-0.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1071 b- defN 22-Aug-19 02:35 dyce-0.6.0.dist-info/RECORD
-15 files, 273361 bytes uncompressed, 63688 bytes compressed:  76.7%
+Zip file size: 65384 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     1197 b- defN 23-Aug-03 16:02 dyce/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 23-Aug-03 16:03 dyce/_version.py
+-rw-r--r--  2.0 unx    33687 b- defN 23-Aug-03 16:02 dyce/evaluation.py
+-rw-r--r--  2.0 unx    69614 b- defN 23-Aug-03 16:02 dyce/h.py
+-rw-r--r--  2.0 unx     2038 b- defN 23-Aug-03 16:02 dyce/lifecycle.py
+-rw-r--r--  2.0 unx    42284 b- defN 23-Aug-03 16:02 dyce/p.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-03 16:02 dyce/py.typed
+-rw-r--r--  2.0 unx    93666 b- defN 23-Aug-03 16:02 dyce/r.py
+-rw-r--r--  2.0 unx     4684 b- defN 23-Aug-03 16:02 dyce/rng.py
+-rw-r--r--  2.0 unx     2461 b- defN 23-Aug-03 16:02 dyce/types.py
+-rw-r--r--  2.0 unx     2132 b- defN 23-Aug-03 16:03 dyce-0.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    20484 b- defN 23-Aug-03 16:03 dyce-0.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 16:03 dyce-0.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Aug-03 16:03 dyce-0.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1071 b- defN 23-Aug-03 16:03 dyce-0.6.1.dist-info/RECORD
+15 files, 273463 bytes uncompressed, 63672 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: dyce/rng.py
 Comment: 
 
 Filename: dyce/types.py
 Comment: 
 
-Filename: dyce-0.6.0.dist-info/LICENSE
+Filename: dyce-0.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: dyce-0.6.0.dist-info/METADATA
+Filename: dyce-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: dyce-0.6.0.dist-info/WHEEL
+Filename: dyce-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: dyce-0.6.0.dist-info/top_level.txt
+Filename: dyce-0.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dyce-0.6.0.dist-info/RECORD
+Filename: dyce-0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dyce/_version.py

```diff
@@ -1,3 +1,3 @@
-__vers_str__ = "0.6.0"
-__version__ = (0, 6, 0)
+__vers_str__ = "0.6.1"
+__version__ = (0, 6, 1)
```

## dyce/evaluation.py

```diff
@@ -11,15 +11,14 @@
 import sys
 from contextvars import ContextVar
 from fractions import Fraction
 from functools import wraps
 from itertools import chain, product
 from math import prod
 from typing import (
-    TYPE_CHECKING,
     Callable,
     Iterable,
     Iterator,
     List,
     NamedTuple,
     Optional,
     Tuple,
@@ -28,30 +27,27 @@
     Union,
     overload,
 )
 
 from numerary import IntegralLike, RealLike
 from numerary.bt import beartype
 from numerary.types import (
+    CachingProtocolMeta,
+    Protocol,
     RationalLikeMixedT,
     RationalLikeMixedU,
     denominator,
     numerator,
 )
 
 from .h import H, HableT, HOrOutcomeT, _OutcomeCountT, _SourceT
 from .lifecycle import experimental
 from .p import P, RollT
 from .types import _GetItemT, as_int
 
-if TYPE_CHECKING:
-    from typing import Protocol
-else:
-    from numerary.types import Protocol
-
 __all__ = ()
 
 
 # ---- Types ---------------------------------------------------------------------------
 
 
 class HResult(NamedTuple):
@@ -69,15 +65,15 @@
     which: Iterable[_GetItemT] = ()
 
     @property
     def total(self) -> int:
         return self.p.total
 
 
-_LimitT = Union[IntegralLike, RationalLikeMixedU, RealLike]
+LimitT = Union[IntegralLike, RationalLikeMixedU, RealLike]
 _NormalizedLimitT = Union[int, Fraction]
 _ReturnsHOrOutcomeT = Callable[..., HOrOutcomeT]
 _DependentTermT = TypeVar("_DependentTermT", bound=_ReturnsHOrOutcomeT)
 _POrPWithSelectionOrSourceT = Union[P, PWithSelection, _SourceT]
 _PredicateT = Callable[[HResult], bool]
 _HResultCountT = Tuple[HResult, int]
 _PResultCountT = Tuple[PResult, int]
@@ -85,19 +81,19 @@
 
 class _Context(NamedTuple):
     normalized_limit: Optional[_NormalizedLimitT] = None
     contextual_depth: int = 0
     contextual_precision: Fraction = Fraction(1)
 
 
-class _ForEachEvaluatorT(Protocol):
+class _ForEachEvaluatorT(Protocol, metaclass=CachingProtocolMeta):
     def __call__(
         self,
         *args: _POrPWithSelectionOrSourceT,
-        limit: Optional[_LimitT] = None,
+        limit: Optional[LimitT] = None,
         **kw: _POrPWithSelectionOrSourceT,
     ) -> H:
         ...
 
 
 # ---- Data ----------------------------------------------------------------------------
 
@@ -258,17 +254,17 @@
     ```
 
     ``#!python @expandable`` functions can call themselves recursively. They take a
     *limit* keyword argument to control when such recursion should stop. The decorator
     itself takes an optional argument *sentinel*, which defines what is returned once
     *limit* is reached (or a ``#!python RecursionError`` is encountered, whichever comes
     first). The default value for *sentinel* is ``#!python H({0: 1})`` and the value
-    ascribed to *limit* if not provided is ``#!python 1``.
+    ascribed to *limit*, if not provided, is ``#!python 1``.
 
-    If *limit* is an whole number, it defines the maximum recursive evaluation “depth”.
+    If *limit* is a whole number, it defines the maximum recursive evaluation “depth”.
     The way to express no recursion (i.e., merely return *sentinel*) is to set *limit*
     to an integral value of ``#!python 0``. An integral value of ``#!python -1`` is
     equivalent to setting it to ``#!python sys.maxsize``.[^1]
 
     [^1]:
 
         An integral *limit* in the low-to-mid single digits is often more than
@@ -625,15 +621,15 @@
         state.
     """
 
     def _decorator(f):
         @wraps(f)
         def _f(
             *args: _POrPWithSelectionOrSourceT,
-            limit: Optional[_LimitT] = None,
+            limit: Optional[LimitT] = None,
             **kw: _POrPWithSelectionOrSourceT,
         ) -> H:
             try:
                 cur_ctxt = _expandable_ctxt.get()
             except LookupError:
                 cur_ctxt = _Context()
 
@@ -743,17 +739,17 @@
     corresponding count’s weight. In other words, the sum of the counts of the histogram
     retains the same proportion to other outcomes as its corresponding count. This
     becomes clearer when there is no overlap between the histogram and the other
     outcomes.
 
     ``` python
     >>> from dyce.evaluation import aggregate_weighted
-    >>> weighted_sources = ((H(3), 3), (H(-3), 2))
+    >>> weighted_sources = ((H({1: 1}), 1), (H({1: 1, 2: 2}), 2))
     >>> h = aggregate_weighted(weighted_sources).lowest_terms() ; h
-    H({-3: 2, -2: 2, -1: 2, 1: 3, 2: 3, 3: 3})
+    H({1: 5, 2: 4})
 
     ```
 
     !!! note "An important exception"
 
         If a source is the empty histogram (``H({})``), it and its count is omitted from
         the result without scaling.
@@ -789,15 +785,15 @@
 
 
 @experimental
 @beartype
 def foreach(
     callback: _DependentTermT,
     *args: _POrPWithSelectionOrSourceT,
-    limit: Optional[_LimitT] = None,
+    limit: Optional[LimitT] = None,
     sentinel: H = _DEFAULT_SENTINEL,
     **kw: _POrPWithSelectionOrSourceT,
 ) -> H:
     r"""
     !!! warning "Experimental"
 
         This function should be considered experimental and may change or disappear in
@@ -840,15 +836,15 @@
 
 
 @experimental
 @beartype
 def explode(
     source: _SourceT,
     predicate: _PredicateT = lambda result: result.outcome == max(result.h),
-    limit=None,
+    limit: Optional[LimitT] = None,
     inf=float("inf"),
 ) -> H:
     r"""
     !!! warning "Experimental"
 
         This function should be considered experimental and may change or disappear in
         future versions.
@@ -976,15 +972,15 @@
         )
     else:
         raise TypeError(f"unrecognized source type {source}")
 
 
 @beartype
 def _normalize_limit(
-    limit: _LimitT,
+    limit: LimitT,
 ) -> _NormalizedLimitT:
     normalized_limit: _NormalizedLimitT
 
     if isinstance(limit, IntegralLike):
         normalized_limit = as_int(limit)
     elif isinstance(limit, RationalLikeMixedT):
         normalized_limit = Fraction(numerator(limit), denominator(limit))
```

## dyce/h.py

```diff
@@ -52,27 +52,21 @@
     ValuesView,
     cast,
     overload,
 )
 
 from numerary import IntegralLike, RealLike
 from numerary.bt import beartype
-from numerary.types import (
-    CachingProtocolMeta,
-    Protocol,
-    RationalLikeMixedU,
-    SupportsInt,
-    runtime_checkable,
-)
+from numerary.protocol import CachingProtocolMeta
+from numerary.types import Protocol, RationalLikeMixedU, SupportsInt, runtime_checkable
 
 from . import rng
 from .lifecycle import deprecated, experimental
 from .types import (
     _BinaryOperatorT,
-    _RationalInitializerT,
     _UnaryOperatorT,
     as_int,
     is_even,
     is_odd,
     natural_key,
     sorted_outcomes,
 )
@@ -490,14 +484,18 @@
     def __hash__(self) -> int:
         if self._hash is None:
             self._hash = hash(frozenset(self.lowest_terms().items()))
 
         return self._hash
 
     @beartype
+    def __bool__(self) -> int:
+        return bool(self.total)
+
+    @beartype
     def __len__(self) -> int:
         return len(self._h)
 
     @beartype
     def __getitem__(self, key: RealLike) -> int:
         return __getitem__(self._h, key)
 
@@ -1167,15 +1165,15 @@
         H({-1: 1, 0: 1, 1: 1})
 
         ```
         """
         if self._lowest_terms is None:
             counts_gcd = gcd(*self.counts())
 
-            if counts_gcd in (0, 1):
+            if counts_gcd in (0, 1) and 0 not in self.counts():
                 self._lowest_terms = self
             else:
                 self._lowest_terms = type(self)(
                     (outcome, count // counts_gcd)
                     for outcome, count in self.items()
                     if count != 0
                 )
@@ -1225,14 +1223,15 @@
         True
 
         ```
 
         This method caches computing the betas for *n* so they can be reused for varying
         values of *pos* in subsequent calls.
         """
+        # See <https://math.stackexchange.com/q/4173084/226394> for motivation
         n = as_int(n)
         pos = as_int(pos)
 
         if n not in self._order_stat_funcs_by_n:
             self._order_stat_funcs_by_n[n] = self._order_stat_func_for_n(n)
 
         if pos < 0:
@@ -1363,20 +1362,20 @@
             The *max_depth* parameter is similar to an
             [``expandable``][dyce.evaluation.expandable]-decorated function’s limit
             argument when given a whole number. The *precision_limit* parameter is
             similar to an [``expandable``][dyce.evaluation.expandable]-decorated
             function’s limit argument being provided a fractional value. It is an error
             to provide values for both *max_depth* and *precision_limit*.
         """
-        from .evaluation import HResult, _LimitT, expandable
+        from .evaluation import HResult, LimitT, expandable
 
         if max_depth is not None and precision_limit is not None:
             raise ValueError("only one of max_depth and precision_limit is allowed")
 
-        limit: Optional[_LimitT] = (
+        limit: Optional[LimitT] = (
             max_depth if precision_limit is None else precision_limit
         )
 
         @expandable(sentinel=self)
         def _expand(result: HResult) -> HOrOutcomeT:
             res = expand(result.h, result.outcome)
 
@@ -1460,23 +1459,23 @@
         self,
     ) -> Iterator[tuple[RealLike, Fraction]]:
         ...
 
     @overload
     def distribution(
         self,
-        rational_t: _RationalInitializerT[_T],
+        rational_t: Callable[[int, int], _T],
     ) -> Iterator[tuple[RealLike, _T]]:
         ...
 
     @experimental
     @beartype
     def distribution(
         self,
-        rational_t: _RationalInitializerT[_T] = Fraction,
+        rational_t: Optional[Callable[[int, int], _T]] = None,
     ) -> Iterator[tuple[RealLike, _T]]:
         r"""
         Presentation helper function returning an iterator for each outcome/count or
         outcome/probability pair.
 
         ``` python
         >>> h = H((1, 2, 3, 3, 4, 4, 5, 6))
@@ -1542,14 +1541,19 @@
         ``` python
         >>> import sage.rings.rational  # doctest: +SKIP
         >>> [(outcome, sage.rings.rational.Rational(probability)) for outcome, probability in h.distribution()]  # doctest: +SKIP
         [(1, 1/6), (2, 1/6), (3, 1/3), (4, 1/3), (5, 1/6), (6, 1/6)]
 
         ```
         """
+        if rational_t is None:
+            # TODO(posita): See <https://github.com/python/mypy/issues/10854#issuecomment-1663057450>
+            rational_t = Fraction  # type: ignore [assignment]
+            assert rational_t is not None
+
         total = sum(self.values()) or 1
 
         return (
             (outcome, rational_t(self[outcome], total))
             for outcome in sorted_outcomes(self)
         )
 
@@ -1731,18 +1735,22 @@
         """
         mu = mu if mu else self.mean()
         numerator: float
         denominator: float
         numerator = denominator = 0
 
         for outcome, count in self.items():
-            numerator += (outcome - mu) ** 2 * count
+            numerator += outcome**2 * count
             denominator += count
 
-        return numerator / (denominator or 1)
+        # While floating point overflow is impossible to eliminate, we avoid it under
+        # some circumstances by exploiting the equivalence of E[(X - E[X])**2] and the
+        # more efficient E[X**2] - E[X]**2. See
+        # <https://dlsun.github.io/probability/variance.html>.
+        return numerator / (denominator or 1) - mu**2
 
     @beartype
     def roll(self) -> RealLike:
         r"""
         Returns a (weighted) random outcome, sorted.
         """
         return (
@@ -1775,18 +1783,15 @@
         def order_stat_for_n_at_pos(pos: int) -> H:
             return type(self)(_gen_h_items_at_pos(pos))
 
         return order_stat_for_n_at_pos
 
 
 @runtime_checkable
-class HableT(
-    Protocol,
-    metaclass=CachingProtocolMeta,
-):
+class HableT(Protocol, metaclass=CachingProtocolMeta):
     r"""
     A protocol whose implementer can be expressed as (or reduced to) an
     [``H`` object][dyce.h.H] by calling its [``h`` method][dyce.h.HableT.h]. Currently,
     only the [``P`` class][dyce.p.P] implements this protocol, but this affords an
     integration point for ``#!python dyce`` users.
 
     !!! info
```

## dyce/lifecycle.py

```diff
@@ -52,15 +52,14 @@
         f"{f.__qualname__} should be considered experimental and may change or disappear in future versions",
     )
 
 
 def _warn_decr(f: _WrappedT, category: Type[Warning], warning_txt: str) -> _WrappedT:
     @wraps(f)
     def _wrapped(*args, **kw):
-
         warnings.warn(
             warning_txt,
             category=category,
             stacklevel=2,
         )
 
         return f(*args, **kw)
```

## dyce/p.py

```diff
@@ -25,15 +25,15 @@
     overload,
 )
 
 from numerary import RealLike
 from numerary.bt import beartype
 from numerary.types import SupportsIndex, SupportsInt
 
-from .h import H, HableOpsMixin, HableT, _MappingT, _SourceT, sum_h
+from .h import H, HableOpsMixin, HableT, _SourceT, sum_h
 from .lifecycle import deprecated, experimental
 from .types import (
     _BinaryOperatorT,
     _GetItemT,
     _UnaryOperatorT,
     as_int,
     getitems,
@@ -220,27 +220,28 @@
             hs.sort(key=lambda h: tuple(h.items()))
         except TypeError:
             # This is for outcomes that don't support direct comparisons, like symbolic
             # representations
             hs.sort(key=lambda h: str(tuple(h.items())))
 
         self._hs = tuple(hs)
-        self._total: int = prod(h.total for h in self._hs) if self._hs else 0
+        self._total: int = prod(h.total for h in self._hs)
 
     # ---- Properties ------------------------------------------------------------------
 
     @property
     def total(self) -> int:
         r"""
         !!! warning "Experimental"
 
             This method should be considered experimental and may change or disappear in
             future versions.
 
-        Equivalent to ``#!python prod(h.total for h in self) if self else 0``.
+        Equivalent to ``#!python prod(h.total for h in self)``. Note that—consistent
+        with the empty product—this is ``#!python 1`` for an empty pool.
         """
         return self._total
 
     # ---- Overrides -------------------------------------------------------------------
 
     @beartype
     def __repr__(self) -> str:
@@ -291,18 +292,15 @@
         ...
 
     @overload
     def __getitem__(self, key: slice) -> P:
         ...
 
     @beartype
-    # TODO(posita): See <https://github.com/python/mypy/issues/8393>
-    # TODO(posita): See <https://github.com/beartype/beartype/issues/39#issuecomment-871914114> et seq.
-    # TODO(posita): See <https://github.com/beartype/beartype/issues/152>
-    def __getitem__(self, key: _GetItemT) -> Union[H, "P"]:  # type: ignore [override]
+    def __getitem__(self, key: _GetItemT) -> Union[H, "P"]:
         if isinstance(key, slice):
             return P(*self._hs[key])
         else:
             return self._hs[__index__(key)]
 
     @beartype
     def __iter__(self) -> Iterator[H]:
@@ -565,17 +563,17 @@
 
         def _kw_roll_count_tuples(
             pool_name: str,
         ) -> Iterator[tuple[str, RollT, int]]:
             for roll, count in pools_by_kw[pool_name].rolls_with_counts():
                 yield pool_name, roll, count
 
-        def _resolve_dependent_term_for_rolls() -> Iterator[
-            tuple[Union[H, RealLike], int]
-        ]:
+        def _resolve_dependent_term_for_rolls() -> (
+            Iterator[tuple[Union[H, RealLike], int]]
+        ):
             for kw_roll_count_tuples in product(
                 *(_kw_roll_count_tuples(pool_name) for pool_name in pools_by_kw)
             ):
                 combined_count = prod(count for _, _, count in kw_roll_count_tuples)
                 rolls_by_name = {name: roll for name, roll, _ in kw_roll_count_tuples}
                 yield dependent_term(**rolls_by_name), combined_count
 
@@ -745,43 +743,43 @@
         >>> print(yhatzee_on_single_roll.format(width=0))
         {..., 0: 99.92%, 1:  0.08%}
 
         ```
 
         !!! note "In the general case, rolls may appear more than once."
 
-        ``` python
-        >>> sorted(P(H(2), H(3)).rolls_with_counts())
-        [((1, 1), 1), ((1, 2), 1), ((1, 2), 1), ((1, 3), 1), ((2, 2), 1), ((2, 3), 1)]
+            ``` python
+            >>> sorted(P(H(2), H(3)).rolls_with_counts())
+            [((1, 1), 1), ((1, 2), 1), ((1, 2), 1), ((1, 3), 1), ((2, 2), 1), ((2, 3), 1)]
 
-        ```
+            ```
 
-        In the above, ``#!python (1, 2)`` appears a total of two times, each with counts
-        of one.
+            In the above, ``#!python (1, 2)`` appears a total of two times, each with
+            counts of one.
 
-        However, if the pool is homogeneous (meaning it only contains identical
-        histograms), rolls (before selection) are not repeated. (See the note on
-        implementation below.)
+            However, if the pool is homogeneous (meaning it only contains identical
+            histograms), rolls (before selection) are not repeated. (See the note on
+            implementation below.)
 
-        ``` python
-        >>> sorted((2@P(H((-1, 0, 1)))).rolls_with_counts())
-        [((-1, -1), 1), ((-1, 0), 2), ((-1, 1), 2), ((0, 0), 1), ((0, 1), 2), ((1, 1), 1)]
+            ``` python
+            >>> sorted((2@P(H((-1, 0, 1)))).rolls_with_counts())
+            [((-1, -1), 1), ((-1, 0), 2), ((-1, 1), 2), ((0, 0), 1), ((0, 1), 2), ((1, 1), 1)]
 
-        ```
+            ```
 
-        Either way, by summing and counting all rolls, we can confirm identity.
+            Either way, by summing and counting all rolls, we can confirm identity.
 
-        ``` python
-        >>> d6 = H(6)
-        >>> d6avg = H((2, 3, 3, 4, 4, 5))
-        >>> p = 2@P(d6, d6avg)
-        >>> H((sum(roll), count) for roll, count in p.rolls_with_counts()) == p.h() == d6 + d6 + d6avg + d6avg
-        True
+            ``` python
+            >>> d6 = H(6)
+            >>> d6avg = H((2, 3, 3, 4, 4, 5))
+            >>> p = 2@P(d6, d6avg)
+            >>> H((sum(roll), count) for roll, count in p.rolls_with_counts()) == p.h() == d6 + d6 + d6avg + d6avg
+            True
 
-        ```
+            ```
 
         This method does not try to outsmart callers by (mis)interpreting selection
         arguments. It honors selection identifier order and any redundancy.
 
         ``` python
         >>> p_d3_d4 = P(H(3), H(4))
         >>> # Select the second, first, then second (again) elements
@@ -984,16 +982,16 @@
 @beartype
 def _analyze_selection(n: int, which: Iterable[_GetItemT]) -> Optional[int]:
     r"""
     Examines the selection *which* as applied to the values ``#!python range(n)`` and
     returns one of:
 
     * $0$ – *which* selects zero elements in the range
-    * $\{ {i} \mid {i < n} \}$ – *which* favors elements $[0..i)$
-    * $\{ {-i} \mid {i < n} \}$ – *which* favors elements $[i..n)$
+    * $\{ {i} \mid {0 < i < n} \}$ – *which* favors elements $[0..i)$
+    * $\{ {i} \mid {-n < i < 0} \}$ – *which* favors elements $[i..n)$
     * $\{ {k} \mid {k \mod n = 0} \}$ – *which* selects each of $[0..n)$ exactly $k$ times
     * ``#!python None`` – any other selection
     """
     indexes = tuple(range(n))
     counts_by_index: Counter[int] = Counter(getitems(indexes, which))
     found_indexes = set(counts_by_index)
 
@@ -1018,49 +1016,59 @@
         return max_index
     else:
         assert False, "logically impossible (should never be here)"
 
 
 @beartype
 def _rwc_heterogeneous_h_groups(
-    h_groups: Iterable[tuple[_MappingT, int]],
+    h_groups: Iterable[tuple[H, int]],
     k: Optional[int],
 ) -> Iterator[_RollCountT]:
     r"""
     Given an iterable of histogram/count pairs, returns an iterator yielding
     two-tuples (pairs) per [``P.rolls_with_counts``][dyce.p.P.rolls_with_counts].
 
     The use of histogram/count pairs for *h_groups* is acknowledged as awkward, but
     intended, since this implementation leverages homogeneous optimizations (e.g.,
     [``_rwc_homogeneous_n_h_using_partial_selection``][dyce.p._rwc_homogeneous_n_h_using_partial_selection]).
 
     If provided, *k* signals which outcomes are to be selected from the produced rolls.
     This affords an additional optimization where *k* is less than the size of a
     homogeneous subgroup.
     """
-
-    def _choose_rwc_homogeneous_n_h_implementation(n, h) -> Iterator[_RollCountT]:
-        if k and abs(k) < n:
-            return _rwc_homogeneous_n_h_using_partial_selection(n, h, k)
-        else:
-            return _rwc_homogeneous_n_h_using_partial_selection(n, h, n)
+    total_n = sum(n for _, n in h_groups)
 
     for v in product(
-        *(_choose_rwc_homogeneous_n_h_implementation(n, h) for h, n in h_groups)
+        *(
+            _rwc_homogeneous_n_h_using_partial_selection(
+                n, h, k if k and abs(k) < n else n
+            )
+            for h, n in h_groups
+        )
     ):
         # It's possible v is () if h_groups is empty. See
         # <https://stackoverflow.com/questions/3154301/> for a detailed discussion.
         if v:
             rolls_by_group: Iterable[Iterable[RealLike]]
             counts_by_group: Iterable[int]
             rolls_by_group, counts_by_group = zip(*v)
-            sorted_outcomes_for_roll = tuple(sorted(chain(*rolls_by_group)))
             total_count = prod(counts_by_group)
+            sorted_outcomes = tuple(sorted(chain(*rolls_by_group)))
+
+            if k is not None:
+                if k < 0:
+                    sorted_outcomes = (None,) * (
+                        total_n - len(sorted_outcomes)
+                    ) + sorted_outcomes
+                else:
+                    sorted_outcomes = sorted_outcomes + (None,) * (
+                        total_n - len(sorted_outcomes)
+                    )
 
-            yield sorted_outcomes_for_roll, total_count
+            yield sorted_outcomes, total_count
 
 
 @beartype
 def _rwc_homogeneous_n_h_using_partial_selection(
     n: int,
     h: H,
     k: int,
```

## dyce/r.py

```diff
@@ -2836,17 +2836,15 @@
         ...
 
     @overload
     def __getitem__(self, key: slice) -> tuple[RollOutcome, ...]:
         ...
 
     @beartype
-    # TODO(posita): See <https://github.com/python/mypy/issues/8393>
-    # TODO(posita): See <https://github.com/beartype/beartype/issues/39#issuecomment-871914114> et seq.
-    def __getitem__(  # type: ignore [override]
+    def __getitem__(
         self,
         key: _GetItemT,
     ) -> Union[RollOutcome, tuple[RollOutcome, ...]]:
         if isinstance(key, slice):
             return self._roll_outcomes[key]
         else:
             return self._roll_outcomes[__index__(key)]
```

## dyce/types.py

```diff
@@ -5,26 +5,19 @@
 # from its original, then please contact the author before viewing or using this
 # software in any capacity.
 # ======================================================================================
 
 from __future__ import annotations
 
 import re
-from abc import abstractmethod
 from operator import __getitem__, __index__
 from typing import Any, Callable, Iterable, Iterator, Sequence, TypeVar, Union
 
 from numerary.bt import beartype
-from numerary.types import (
-    CachingProtocolMeta,
-    Protocol,
-    SupportsIndex,
-    SupportsInt,
-    runtime_checkable,
-)
+from numerary.types import SupportsIndex, SupportsInt
 
 __all__ = (
     "as_int",
     "is_even",
     "is_odd",
 )
 
@@ -35,27 +28,14 @@
 _T = TypeVar("_T")
 _T_co = TypeVar("_T_co", covariant=True)
 _UnaryOperatorT = Callable[[_T_co], _T_co]
 _BinaryOperatorT = Callable[[_T_co, _T_co], _T_co]
 _GetItemT = Union[SupportsIndex, slice]
 
 
-@runtime_checkable
-class _RationalInitializerT(
-    Protocol[_T_co],
-    metaclass=CachingProtocolMeta,
-):
-    # TODO(posita): See <https://github.com/python/mypy/issues/11013>
-    # __slots__: Any = ()
-
-    @abstractmethod
-    def __call__(self, numerator: int, denominator: int) -> _T_co:
-        pass
-
-
 # ---- Functions -----------------------------------------------------------------------
 
 
 @beartype
 def as_int(val: SupportsInt) -> int:
     r"""
     Helper function to losslessly coerce *val* into an ``#!python int``. Raises
```

## Comparing `dyce-0.6.0.dist-info/LICENSE` & `dyce-0.6.1.dist-info/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # License and credits
 
 ## The MIT License (MIT)
 
-Copyright © 2015-2022 [Matt Bogosian](mailto:matt@bogosian.net?Subject=dyce)
+Copyright © 2015-2023 [Matt Bogosian](mailto:matt@bogosian.net?Subject=dyce)
 ([**@posita**](https://github.com/posita)).
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the “Software”), to deal in the Software
 without restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to the following
```

## Comparing `dyce-0.6.0.dist-info/METADATA` & `dyce-0.6.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyce
-Version: 0.6.0
+Version: 0.6.1
 Summary: Simple Python tools for exploring dice outcomes and other finite discrete probabilities
 Home-page: https://posita.github.io/dyce/
 Author: Matt Bogosian
 Author-email: matt@bogosian.net
 License: MIT License
 Project-URL: Source Repository, https://github.com/posita/dyce/
 Classifier: Topic :: Education
@@ -23,21 +23,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
-Requires-Dist: numerary (>=0.4.0)
+Requires-Dist: numerary (~=0.4.3)
 Provides-Extra: dev
 Requires-Dist: numpy ; extra == 'dev'
 Requires-Dist: pandas ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
-Requires-Dist: sympy (>=1.9) ; extra == 'dev'
-Requires-Dist: tox ; extra == 'dev'
+Requires-Dist: sympy (~=1.9) ; extra == 'dev'
+Requires-Dist: tox (~=4.0) ; extra == 'dev'
 Requires-Dist: versioningit (~=2.0) ; extra == 'dev'
 
 <!---
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !!!!!!!!!!!!!!! IMPORTANT: READ THIS BEFORE EDITING! !!!!!!!!!!!!!!!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   Please keep each sentence on its own unwrapped line.
@@ -51,27 +51,27 @@
 -->
 
 *Copyright and other protections apply.
 Please see the accompanying ``LICENSE`` file for rights and restrictions governing use of this software.
 All rights not expressly waived or licensed are reserved.
 If that file is missing or appears to be modified from its original, then please contact the author before viewing or using this software in any capacity.*
 
-[![Tests](https://github.com/posita/dyce/actions/workflows/unit-tests.yaml/badge.svg)](https://github.com/posita/dyce/actions/workflows/unit-tests.yaml)
-[![Version](https://img.shields.io/pypi/v/dyce/0.6.0.svg)](https://pypi.org/project/dyce/0.6.0/)
-[![Development Stage](https://img.shields.io/pypi/status/dyce/0.6.0.svg)](https://pypi.org/project/dyce/0.6.0/)
-[![License](https://img.shields.io/pypi/l/dyce/0.6.0.svg)](http://opensource.org/licenses/MIT)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dyce/0.6.0.svg)](https://pypi.org/project/dyce/0.6.0/)
-[![Supported Python Implementations](https://img.shields.io/pypi/implementation/dyce/0.6.0.svg)](https://pypi.org/project/dyce/0.6.0/)
+[![Tests](https://github.com/posita/dyce/actions/workflows/on-push.yaml/badge.svg)](https://github.com/posita/dyce/actions/workflows/on-push.yaml)
+[![Version](https://img.shields.io/pypi/v/dyce/0.6.1.svg)](https://pypi.org/project/dyce/0.6.1/)
+[![Development Stage](https://img.shields.io/pypi/status/dyce/0.6.1.svg)](https://pypi.org/project/dyce/0.6.1/)
+[![License](https://img.shields.io/pypi/l/dyce/0.6.1.svg)](http://opensource.org/licenses/MIT)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dyce/0.6.1.svg)](https://pypi.org/project/dyce/0.6.1/)
+[![Supported Python Implementations](https://img.shields.io/pypi/implementation/dyce/0.6.1.svg)](https://pypi.org/project/dyce/0.6.1/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![``numerary``-encumbered](https://raw.githubusercontent.com/posita/numerary/latest/docs/numerary-encumbered.svg)](https://posita.github.io/numerary/)
 [![Bear-ified™](https://raw.githubusercontent.com/beartype/beartype-assets/main/badge/bear-ified.svg)](https://beartype.rtfd.io/)
 
 Now you’re playing with …
 
-<img style="float: right; padding: 0 1.0em 0 1.0em;" src="https://raw.githubusercontent.com/posita/dyce/v0.6.0/docs/dyce.svg" alt="dyce logo">
+<img style="float: right; padding: 0 1.0em 0 1.0em;" src="https://raw.githubusercontent.com/posita/dyce/v0.6.1/docs/dyce.svg" alt="dyce logo">
 
 # ``dyce`` – simple Python tools for exploring dice outcomes and other finite discrete probabilities
 
 **💥 _Now 100% [Bear-ified™](https://beartype.rtfd.io/)!_ 👌🏾🐻**
 ([Details](#requirements) below.)
 
 
@@ -178,25 +178,25 @@
 ```
 
 [``H`` objects](https://posita.github.io/dyce/0.6/dyce/#dyce.h.H) provide a [``distribution`` method](https://posita.github.io/dyce/0.6/dyce/#dyce.h.H.distribution) and a [``distribution_xy`` method](https://posita.github.io/dyce/0.6/dyce/#dyce.h.H.distribution_xy) to ease integration with plotting packages
 [``anydyce``](https://github.com/posita/anydyce/), for example, makes use of these to integrate with [``matplotlib``](https://matplotlib.org/stable/api/index.html).
 
 <!-- Should match any title of the corresponding plot title -->
 <picture>
-  <source srcset="https://raw.githubusercontent.com/posita/dyce/v0.6.0/docs/assets/plot_2d6_lo_hi_dark.png" media="(prefers-color-scheme: dark)">
-  <img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/dyce/v0.6.0/docs/assets/plot_2d6_lo_hi_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/dyce/v0.6.0/docs/assets/plot_2d6_lo_hi_dark.png#gh-dark-mode-only"></span>
+  <source srcset="https://raw.githubusercontent.com/posita/dyce/v0.6.1/docs/assets/plot_2d6_lo_hi_dark.png" media="(prefers-color-scheme: dark)">
+  <img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/dyce/v0.6.1/docs/assets/plot_2d6_lo_hi_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/dyce/v0.6.1/docs/assets/plot_2d6_lo_hi_dark.png#gh-dark-mode-only"></span>
 </picture>
 <!-- The above is a ridiculous work-around for GitHub's braindead, proprietary
 light/dark image rendering dumpster fire. See
 [https://github.community/t/support-theme-context-for-images-in-light-vs-dark-mode/147981/87].
 -->
 
 <details>
 <summary>
-  Source: <a href="https://github.com/posita/dyce/blob/v0.6.0/docs/assets/plot_2d6_lo_hi.py"><code>plot_2d6_lo_hi.py</code></a><br>
+  Source: <a href="https://github.com/posita/dyce/blob/v0.6.1/docs/assets/plot_2d6_lo_hi.py"><code>plot_2d6_lo_hi.py</code></a><br>
   Interactive version: <a href="https://posita.github.io/dyce/0.6/jupyter/lab/?path=2d6_lo_hi.ipynb"><img src="https://jupyterlite.readthedocs.io/en/latest/_static/badge.svg" alt="Try dyce"></a>
 </summary>
 
 ``` python
 --8<-- "docs/assets/plot_2d6_lo_hi.py"
 ```
 </details>
```

## Comparing `dyce-0.6.0.dist-info/RECORD` & `dyce-0.6.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 dyce/__init__.py,sha256=_ahkr-ssHoR40mf3n7bLccG6x-eHdCayCNjfr7F3fBI,1197
-dyce/_version.py,sha256=E5E7ybbUhoxz19raqbYDN8dXF5gsYDbs70bLysMndVA,48
-dyce/evaluation.py,sha256=RUIGDwZuMbcM821DfKQtnAIs1RfHW98ePe3ZY_hEVKo,33729
-dyce/h.py,sha256=79aw3vzdAFhqkpC9NNn0HxxVBfxCkWMMncVxpcqPJo8,68940
-dyce/lifecycle.py,sha256=xnaT6PZexXzuCuFDminKUw-5W0FCIAxkZidzeOgjsGc,2039
-dyce/p.py,sha256=zIUw8PzU1448eF55pac4SgZ5s9-SlxDykwGxqOTa8qU,42203
+dyce/_version.py,sha256=DaDZNz7P-xyE1fISw68FOVWvvsVLiA8lppltVBrrZNU,48
+dyce/evaluation.py,sha256=0aSyj_uSZPU_uygUDLOMFjV3Xvia1OZyNBETsPQiEoA,33687
+dyce/h.py,sha256=tkOdkprxc4dJ1oyGxtvve0yGka2vmDvHlu0cLF5xj8w,69614
+dyce/lifecycle.py,sha256=S4WmEDP7-txObkwJu3foga2G4wsyP-MsDDQVG6RicAk,2038
+dyce/p.py,sha256=Ai5fhz4TF0NAuISyRAw3mGfYjtZRNUtt0C_bYwcXVsg,42284
 dyce/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dyce/r.py,sha256=DO_P5GccbCsxckM8cDy8U_FBE7Zldu95oDjf0Tf-FHY,93866
+dyce/r.py,sha256=EPC5u5UI0stQCaNWI1XZQReZEHoyVVlm8GULsB4w9UU,93666
 dyce/rng.py,sha256=39_0nNSmWCRfk_dzvsQoAN2KgvJdvtIGb3NLQBPjGfo,4684
-dyce/types.py,sha256=jwQ1eOXRamRQYAtChfz77yhbNRlnzakld-caSAcUyqI,2873
-dyce-0.6.0.dist-info/LICENSE,sha256=WmUL-IVfRaesuQ5qOOAEjJpDonVVHmgUD4s-j4VWr60,2132
-dyce-0.6.0.dist-info/METADATA,sha256=9x6GukMMaLt4xPU2B-cRcrJ8u_BxUi4aV0qdGdQkk9s,20482
-dyce-0.6.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dyce-0.6.0.dist-info/top_level.txt,sha256=zp1IGWxuFFhoGaYiMicYyjDwvYArkxZl5iM_XUGZnsE,5
-dyce-0.6.0.dist-info/RECORD,,
+dyce/types.py,sha256=8OnOeHnKYxm4o2o0U5WQwZDCGnrb4T61yPPf1KdgC2E,2461
+dyce-0.6.1.dist-info/LICENSE,sha256=7tXbUY5pmaUxDrpa2zMatzfb6bUAGUOIYHBluMml9tA,2132
+dyce-0.6.1.dist-info/METADATA,sha256=8odYAI_s7J1AR12ER_h7C0FVOqZGr_n5I4fTcfLeZks,20484
+dyce-0.6.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+dyce-0.6.1.dist-info/top_level.txt,sha256=zp1IGWxuFFhoGaYiMicYyjDwvYArkxZl5iM_XUGZnsE,5
+dyce-0.6.1.dist-info/RECORD,,
```

