# Comparing `tmp/multiHGtest-0.0.3.tar.gz` & `tmp/multiHGtest-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiHGtest-0.0.3.tar", last modified: Wed Aug  2 10:26:14 2023, max compression
+gzip compressed data, was "multiHGtest-0.0.4.tar", last modified: Thu Aug  3 07:33:39 2023, max compression
```

## Comparing `multiHGtest-0.0.3.tar` & `multiHGtest-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-02 10:26:14.124726 multiHGtest-0.0.3/
--rw-r--r--   0 kipnisal   (503) staff       (20)     1073 2022-02-20 07:18:17.000000 multiHGtest-0.0.3/LICENSE
--rw-r--r--   0 kipnisal   (503) staff       (20)     1134 2023-08-02 10:26:14.124782 multiHGtest-0.0.3/PKG-INFO
--rw-r--r--   0 kipnisal   (503) staff       (20)      588 2023-08-02 10:16:59.000000 multiHGtest-0.0.3/README.md
--rw-r--r--   0 kipnisal   (503) staff       (20)      103 2023-03-15 07:51:05.000000 multiHGtest-0.0.3/pyproject.toml
--rw-r--r--   0 kipnisal   (503) staff       (20)      749 2023-08-02 10:26:14.125042 multiHGtest-0.0.3/setup.cfg
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-02 10:26:14.122543 multiHGtest-0.0.3/src/
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-02 10:26:14.123739 multiHGtest-0.0.3/src/multiHGtest/
--rw-r--r--   0 kipnisal   (503) staff       (20)       82 2023-03-22 12:05:06.000000 multiHGtest-0.0.3/src/multiHGtest/__init__.py
--rw-r--r--   0 kipnisal   (503) staff       (20)     6087 2023-08-02 10:24:06.000000 multiHGtest-0.0.3/src/multiHGtest/multiHGtest.py
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-02 10:26:14.124409 multiHGtest-0.0.3/src/multiHGtest.egg-info/
--rw-r--r--   0 kipnisal   (503) staff       (20)     1134 2023-08-02 10:26:14.000000 multiHGtest-0.0.3/src/multiHGtest.egg-info/PKG-INFO
--rw-r--r--   0 kipnisal   (503) staff       (20)      321 2023-08-02 10:26:14.000000 multiHGtest-0.0.3/src/multiHGtest.egg-info/SOURCES.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)        1 2023-08-02 10:26:14.000000 multiHGtest-0.0.3/src/multiHGtest.egg-info/dependency_links.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)       39 2023-08-02 10:26:14.000000 multiHGtest-0.0.3/src/multiHGtest.egg-info/requires.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)       12 2023-08-02 10:26:14.000000 multiHGtest-0.0.3/src/multiHGtest.egg-info/top_level.txt
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-02 10:26:14.124542 multiHGtest-0.0.3/tests/
--rw-r--r--   0 kipnisal   (503) staff       (20)     3661 2023-03-22 12:40:10.000000 multiHGtest-0.0.3/tests/test_multiHGtest.py
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-03 07:33:39.138353 multiHGtest-0.0.4/
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1073 2022-02-20 07:18:17.000000 multiHGtest-0.0.4/LICENSE
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1134 2023-08-03 07:33:39.138433 multiHGtest-0.0.4/PKG-INFO
+-rw-r--r--   0 kipnisal   (503) staff       (20)      588 2023-08-02 10:16:59.000000 multiHGtest-0.0.4/README.md
+-rw-r--r--   0 kipnisal   (503) staff       (20)      103 2023-03-15 07:51:05.000000 multiHGtest-0.0.4/pyproject.toml
+-rw-r--r--   0 kipnisal   (503) staff       (20)      749 2023-08-03 07:33:39.138749 multiHGtest-0.0.4/setup.cfg
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-03 07:33:39.133763 multiHGtest-0.0.4/src/
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-03 07:33:39.135411 multiHGtest-0.0.4/src/multiHGtest/
+-rw-r--r--   0 kipnisal   (503) staff       (20)       82 2023-03-22 12:05:06.000000 multiHGtest-0.0.4/src/multiHGtest/__init__.py
+-rw-r--r--   0 kipnisal   (503) staff       (20)     6276 2023-08-03 07:32:56.000000 multiHGtest-0.0.4/src/multiHGtest/multiHGtest.py
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-03 07:33:39.137570 multiHGtest-0.0.4/src/multiHGtest.egg-info/
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1134 2023-08-03 07:33:39.000000 multiHGtest-0.0.4/src/multiHGtest.egg-info/PKG-INFO
+-rw-r--r--   0 kipnisal   (503) staff       (20)      354 2023-08-03 07:33:39.000000 multiHGtest-0.0.4/src/multiHGtest.egg-info/SOURCES.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)        1 2023-08-03 07:33:39.000000 multiHGtest-0.0.4/src/multiHGtest.egg-info/dependency_links.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)       39 2023-08-03 07:33:39.000000 multiHGtest-0.0.4/src/multiHGtest.egg-info/requires.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)       12 2023-08-03 07:33:39.000000 multiHGtest-0.0.4/src/multiHGtest.egg-info/top_level.txt
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-03 07:33:39.138005 multiHGtest-0.0.4/tests/
+-rw-r--r--   0 kipnisal   (503) staff       (20)     3663 2023-08-03 06:30:49.000000 multiHGtest-0.0.4/tests/test_multiHGtest.py
+-rw-r--r--   0 kipnisal   (503) staff       (20)     2889 2023-08-03 06:58:43.000000 multiHGtest-0.0.4/tests/test_uniformity_pvalues.py
```

### Comparing `multiHGtest-0.0.3/LICENSE` & `multiHGtest-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multiHGtest-0.0.3/PKG-INFO` & `multiHGtest-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiHGtest
-Version: 0.0.3
+Version: 0.0.4
 Summary: Testing for differences in survival using hypergeometric P-values
 Home-page: https://github.com/alonkipnis/higher-criticism-test
 Download-URL: https://github.com/alonkipnis/higher-criticism-test
 Author: Alon Kipnis
 Author-email: alonkipnis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multiHGtest-0.0.3/README.md` & `multiHGtest-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `multiHGtest-0.0.3/setup.cfg` & `multiHGtest-0.0.4/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multiHGtest
-version = 0.0.03
+version = 0.0.04
 author = Alon Kipnis
 author_email = alonkipnis@gmail.com
 description = Testing for differences in survival using hypergeometric P-values
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/alonkipnis/higher-criticism-test
 download_url = https://github.com/alonkipnis/higher-criticism-test
```

### Comparing `multiHGtest-0.0.3/src/multiHGtest/multiHGtest.py` & `multiHGtest-0.0.4/src/multiHGtest/multiHGtest.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,38 +14,40 @@
         M:    total number of object
         n:    total number of Type I objects
         N:    number of draws
         randomize:   whether to do a randomized test
         alternative: type of alternative to consider. Options are:
                   'greater', 'less', 'two-sided'
 
+        NOTE: For 'two-sided', the function only returns approximated P-values what is accurate for extreme values
+        but less accurate for typical values.
+
     Returns:
         Test's P-value
     """
 
     if randomize:
-        U = uniform.rvs(size=len(k))
+        U1, U2 = uniform.rvs(size=(2, len(k)))
     else:
-        U = 0
+        U1 = U2 = 0
 
     if alternative == 'greater':
-        return hypergeom.sf(k - 1, M, n, N) - U * hypergeom.pmf(k, M, n, N)  # sf is 1-cdf+Pk, so Pr(X >= k) = Pr(X>k-1)
+        return hypergeom.sf(k - 1, M, n, N) - U1 * hypergeom.pmf(k, M, n, N)  # sf is 1-cdf+Pk, so Pr(X >= k) = Pr(X>k-1)
 
     if alternative == 'less':
-        return hypergeom.cdf(k, M, n, N) - U * hypergeom.pmf(k, M, n, N)
+        return hypergeom.cdf(k, M, n, N) - U1 * hypergeom.pmf(k, M, n, N)
 
     if alternative == 'two-sided':
         l1 = hypergeom.cdf(k, M, n, N)
         l2 = hypergeom.cdf(N - k, M, n, N)
 
         r1 = hypergeom.sf(k - 1, M, n, N)
         r2 = hypergeom.sf(N - k + 1, M, n, N)
-
-        l = np.minimum(l1, l2) - U * ((l1 < l2) * hypergeom.pmf(k, M, n, N) + (l1 > l2) * hypergeom.pmf(N - k, M, n, N))
-        r = np.minimum(r1, r2) - U * ((r1 < r2) * hypergeom.pmf(k, M, n, N) + (r1 > r2) * hypergeom.pmf(N - k, M, n, N))
+        l = np.minimum(l1, l2) - U1 * ((l1 < l2) * hypergeom.pmf(k, M, n, N) + (l1 > l2) * hypergeom.pmf(N - k, M, n, N)) / 2
+        r = np.minimum(r1, r2) - U2 * ((r1 < r2) * hypergeom.pmf(k, M, n, N) + (r1 > r2) * hypergeom.pmf(N - k, M, n, N)) / 2
         return l + r
 
     raise ValueError("'alternative' must be one of 'grater', 'less', or 'two-sided'")
 
 
 def _MultiTest(Nt1: list, Nt2: list, Ot1: list = None, Ot2: list = None, **kwargs):
     """
```

### Comparing `multiHGtest-0.0.3/src/multiHGtest.egg-info/PKG-INFO` & `multiHGtest-0.0.4/src/multiHGtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiHGtest
-Version: 0.0.3
+Version: 0.0.4
 Summary: Testing for differences in survival using hypergeometric P-values
 Home-page: https://github.com/alonkipnis/higher-criticism-test
 Download-URL: https://github.com/alonkipnis/higher-criticism-test
 Author: Alon Kipnis
 Author-email: alonkipnis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multiHGtest-0.0.3/tests/test_multiHGtest.py` & `multiHGtest-0.0.4/tests/test_multiHGtest.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,16 @@
         O2 = poisson.rvs(Nt2[t] * lam2 * (Nt2[t] > 0))
 
         Nt1[t + 1] = np.maximum(Nt1[t] - O1, 0)
         Nt2[t + 1] = np.maximum(Nt2[t] - O2, 0)
     return Nt1, Nt2
 
 
+
+
 def main():
     T = 1000
     N1 = 5000
     N2 = 5000
 
     beta = .6
     r = 2
```

