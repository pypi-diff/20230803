# Comparing `tmp/signal-processing-algorithms-2.0.1.tar.gz` & `tmp/signal_processing_algorithms-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal-processing-algorithms-2.0.1.tar", max compression
+gzip compressed data, was "signal_processing_algorithms-2.1.0.tar", max compression
```

## Comparing `signal-processing-algorithms-2.0.1.tar` & `signal_processing_algorithms-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11342 2022-01-28 15:33:57.406585 signal-processing-algorithms-2.0.1/LICENSE
--rw-r--r--   0        0        0     7925 2022-01-28 15:33:57.406585 signal-processing-algorithms-2.0.1/README.md
--rw-r--r--   0        0        0      581 2022-01-28 15:33:57.406585 signal-processing-algorithms-2.0.1/build.py
--rw-r--r--   0        0        0     1046 2022-01-28 15:33:57.406585 signal-processing-algorithms-2.0.1/pyproject.toml
--rw-r--r--   0        0        0       41 2022-01-28 15:33:57.406585 signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/__init__.py
--rw-r--r--   0        0        0     1089 2022-01-28 15:33:57.406585 signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/determinism.py
--rw-r--r--   0        0        0        0 2022-01-28 15:33:57.406585 signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/energy_statistics/__init__.py
--rw-r--r--   0        0        0     4173 2022-01-28 15:33:57.406585 signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/energy_statistics/cext_calculator.py
--rw-r--r--   0        0        0     4285 2022-01-28 15:33:57.406585 signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/energy_statistics/e_divisive.c
--rw-r--r--   0        0        0    13883 2022-01-28 15:33:57.406585 signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/energy_statistics/energy_statistics.py
--rw-r--r--   0        0        0     6412 2022-01-28 15:33:57.406585 signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/gesd.py
--rw-r--r--   0        0        0     9156 2022-01-28 15:34:45.661126 signal-processing-algorithms-2.0.1/setup.py
--rw-r--r--   0        0        0     8826 2022-01-28 15:34:45.661692 signal-processing-algorithms-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-08-03 17:56:27.429322 signal_processing_algorithms-2.1.0/LICENSE
+-rw-r--r--   0        0        0     7925 2023-08-03 17:56:27.429322 signal_processing_algorithms-2.1.0/README.md
+-rw-r--r--   0        0        0      581 2023-08-03 17:56:27.429322 signal_processing_algorithms-2.1.0/build.py
+-rw-r--r--   0        0        0     1143 2023-08-03 17:56:27.429322 signal_processing_algorithms-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-08-03 17:56:27.429322 signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/__init__.py
+-rw-r--r--   0        0        0     1089 2023-08-03 17:56:27.429322 signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/determinism.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:56:27.429322 signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/energy_statistics/__init__.py
+-rw-r--r--   0        0        0     4173 2023-08-03 17:56:27.429322 signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/energy_statistics/cext_calculator.py
+-rw-r--r--   0        0        0     4285 2023-08-03 17:56:27.429322 signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/energy_statistics/e_divisive.c
+-rw-r--r--   0        0        0    13999 2023-08-03 17:56:27.429322 signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/energy_statistics/energy_statistics.py
+-rw-r--r--   0        0        0     6493 2023-08-03 17:56:27.429322 signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/gesd.py
+-rw-r--r--   0        0        0     9294 1970-01-01 00:00:00.000000 signal_processing_algorithms-2.1.0/setup.py
+-rw-r--r--   0        0        0     9081 1970-01-01 00:00:00.000000 signal_processing_algorithms-2.1.0/PKG-INFO
```

### Comparing `signal-processing-algorithms-2.0.1/LICENSE` & `signal_processing_algorithms-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signal-processing-algorithms-2.0.1/README.md` & `signal_processing_algorithms-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `signal-processing-algorithms-2.0.1/build.py` & `signal_processing_algorithms-2.1.0/build.py`

 * *Files identical despite different names*

### Comparing `signal-processing-algorithms-2.0.1/pyproject.toml` & `signal_processing_algorithms-2.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "signal-processing-algorithms"
-version = "2.0.1"
+version = "2.1.0"
 description = "Signal Processing Algorithms from MongoDB"
 authors = [
     "Alexander Costas <alexander.costas@mongodb.com>",
     "David Bradford <david.bradford@mongodb.com>",
     "David Daly <david.daly@mongodb.com",
     "Henrik Ingo <henrik.ingo@mongodb.com>",
     "Jeff Zambory <jeff.zambory@mongodb.com>",
@@ -15,18 +15,23 @@
 repository="https://github.com/mongodb/signal-processing-algorithms"
 readme = "README.md"
 build = "build.py"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 more-itertools = "^8.2.0"
-numpy = "^1.18.1"
-scipy = "^1.3"
+setuptools = "< 60.0.0"
+numpy = "^1.24.4"
+scipy = "^1.8.1"
 structlog = "^19.1"
-typing-extensions = "^3.7.4"
+typing-extensions = "^4.5.0"
+pyyaml="^6.0.0"
+gevent="^21.12.0"
+greenlet="^1.1.0"
+typed-ast="^1.5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 pytest-black = "^0.3"
 pytest-cov = "^2.8"
 pytest-flake8 = "^1.0"
 pytest-isort = "^1.3"
```

### Comparing `signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/determinism.py` & `signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/determinism.py`

 * *Files identical despite different names*

### Comparing `signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/energy_statistics/cext_calculator.py` & `signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/energy_statistics/cext_calculator.py`

 * *Files identical despite different names*

### Comparing `signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/energy_statistics/e_divisive.c` & `signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/energy_statistics/e_divisive.c`

 * *Files identical despite different names*

### Comparing `signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/energy_statistics/energy_statistics.py` & `signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/energy_statistics/energy_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 
     if series.dtype is not np.float64:
         series = np.array(series, dtype=np.float64)
 
     if len(series.shape) == 1:
         series = np.atleast_2d(series).T
 
+    if not isinstance(series, np.ndarray):
+        raise Exception("Series is not the expected type, np.ndarray.")
+
     return series
 
 
 def _get_valid_input(series: Union[List[float], List[List[float]], np.ndarray]) -> np.ndarray:
     """
     Return valid form of input.
```

### Comparing `signal-processing-algorithms-2.0.1/src/signal_processing_algorithms/gesd.py` & `signal_processing_algorithms-2.1.0/src/signal_processing_algorithms/gesd.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,31 +91,31 @@
     if significance_level <= 0.0 or significance_level >= 1.0:
         raise ValueError(
             "invalid significance_level({significance_level})".format(
                 significance_level=significance_level
             )
         )
 
-    series = ma.array(data)
+    series = ma.array(data)  # type: ignore
     test_statistics = []
     critical_values = []
     potential_outlier_indices = []
 
     # max outliers must be less than length, the standard deviation and mad of a single entry list
     # are 0 so z score would be nan.
     m_outliers = min(max_outliers, length - 1)
 
     indexes = np.arange(m_outliers, dtype=int)
     for i in indexes:
         LOG.debug("iteration", i=i, mad=mad, series=series)
         if mad:
             # sigma in this case is an estimate of .75 quantile * MAD
             # note : 1.4826 == 1 / Q(.75) == 1 / 0.675
-            center = np.ma.median(series)
-            sigma = 1.4826 * np.ma.median(np.fabs(series - center))
+            center = np.ma.median(series)  # type: ignore
+            sigma = 1.4826 * np.ma.median(np.fabs(series - center))  # type: ignore
         else:
             center = series.mean()
             sigma = series.std(ddof=1)
 
         if sigma == 0:
             break
 
@@ -148,15 +148,16 @@
             "iteration complete",
             z_scores=np.array(
                 [
                     np.arange(max_outliers, dtype=int),
                     test_statistics,
                     critical_values,
                     np.greater(test_statistics, critical_values),
-                ]
+                ],
+                dtype="object",
             ).T,
         )
 
         # Mask and exclude the selected value from the next iteration.
         series[max_z_score_index] = ma.masked
 
     LOG.debug("values calculated", max_z_scores=test_statistics, lambda_values=critical_values)
```

### Comparing `signal-processing-algorithms-2.0.1/setup.py` & `signal_processing_algorithms-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,34 @@
 ['signal_processing_algorithms',
  'signal_processing_algorithms.energy_statistics']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['more-itertools>=8.2.0,<9.0.0',
- 'numpy>=1.18.1,<2.0.0',
- 'scipy>=1.3,<2.0',
+['gevent>=21.12.0,<22.0.0',
+ 'greenlet>=1.1.0,<2.0.0',
+ 'more-itertools>=8.2.0,<9.0.0',
+ 'numpy>=1.24.4,<2.0.0',
+ 'pyyaml>=6.0.0,<7.0.0',
+ 'scipy>=1.8.1,<2.0.0',
+ 'setuptools<60.0.0',
  'structlog>=19.1,<20.0',
- 'typing-extensions>=3.7.4,<4.0.0']
+ 'typed-ast>=1.5.0,<2.0.0',
+ 'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'signal-processing-algorithms',
-    'version': '2.0.1',
+    'version': '2.1.0',
     'description': 'Signal Processing Algorithms from MongoDB',
     'long_description': '# Signal Processing Algorithms\n\nA suite of algorithms implementing [Energy\nStatistics](https://en.wikipedia.org/wiki/Energy_distance), [E-Divisive with\nMeans](https://arxiv.org/pdf/1306.4933.pdf) and [Generalized ESD Test for\nOutliers](https://www.itl.nist.gov/div898/handbook/eda/section3/eda35h3.htm) in python. See [The Use\nof Change Point Detection to Identify Software Performance Regressions in a Continuous Integration\nSystem](https://dl.acm.org/doi/abs/10.1145/3358960.3375791) and [Creating a Virtuous Cycle in\nPerformance Testing at MongoDB](https://dl.acm.org/doi/pdf/10.1145/3427921.3450234) for background\non the development and use of this library.\n\n## Getting Started - Users\n```\npip install signal-processing-algorithms\n```\n\n## Getting Started - Developers\n\nGetting the code:\n\n```\n$ git clone git@github.com:mongodb/signal-processing-algorithms.git\n$ cd signal-processing-algorithms\n```\n\nInstallation\n```\n$ pip install poetry\n$ poetry install\n```\nTesting/linting:\n```\n$ poetry run pytest\n```\n\nRunning the slow tests:\n```\n$ poetry run pytest --runslow\n```\n\n**Some of the larger tests can take a significant amount of time (more than 2 hours).**\n\n## Energy statistics\n[Energy Statistics](https://en.wikipedia.org/wiki/Energy_distance) is the statistical concept of Energy Distance \nand can be used to measure how similar/different two distributions are.\n\nFor statistical samples from two random variables X and Y:\nx1, x2, ..., xn and y1, y2, ..., yn\n\nE-Statistic is defined as:\n\n<a href="https://www.codecogs.com/eqnedit.php?latex=E_{n,m}(X,Y):=2A-B-C" target="_blank"><img src="https://latex.codecogs.com/gif.latex?E_{n,m}(X,Y):=2A-B-C" title="E_{n,m}(X,Y):=2A-B-C" /></a>\n\nwhere,\n\n<a href="https://www.codecogs.com/eqnedit.php?latex=A:={\\frac&space;{1}{nm}}\\sum&space;_{i=1}^{n}\\sum&space;_{j=1}^{m}\\|x_{i}-y_{j}\\|,B:={\\frac&space;{1}{n^{2}}}\\sum&space;_{i=1}^{n}\\sum&space;_{j=1}^{n}\\|x_{i}-x_{j}\\|,C:={\\frac&space;{1}{m^{2}}}\\sum&space;_{i=1}^{m}\\sum&space;_{j=1}^{m}\\|y_{i}-y_{j}\\|" target="_blank"><img src="https://latex.codecogs.com/gif.latex?A:={\\frac&space;{1}{nm}}\\sum&space;_{i=1}^{n}\\sum&space;_{j=1}^{m}\\|x_{i}-y_{j}\\|,B:={\\frac&space;{1}{n^{2}}}\\sum&space;_{i=1}^{n}\\sum&space;_{j=1}^{n}\\|x_{i}-x_{j}\\|,C:={\\frac&space;{1}{m^{2}}}\\sum&space;_{i=1}^{m}\\sum&space;_{j=1}^{m}\\|y_{i}-y_{j}\\|" title="A:={\\frac {1}{nm}}\\sum _{i=1}^{n}\\sum _{j=1}^{m}\\|x_{i}-y_{j}\\|,B:={\\frac {1}{n^{2}}}\\sum _{i=1}^{n}\\sum _{j=1}^{n}\\|x_{i}-x_{j}\\|,C:={\\frac {1}{m^{2}}}\\sum _{i=1}^{m}\\sum _{j=1}^{m}\\|y_{i}-y_{j}\\|" /></a>\n\nT-statistic is defined as: \n\n<a href="https://www.codecogs.com/eqnedit.php?latex=T={\\frac&space;{nm}{n&plus;m}}E_{{n,m}}(X,Y)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?T={\\frac&space;{nm}{n&plus;m}}E_{{n,m}}(X,Y)" title="T={\\frac {nm}{n+m}}E_{{n,m}}(X,Y)" /></a>\n\nE-coefficient of inhomogeneity is defined as:\n\n<a href="https://www.codecogs.com/eqnedit.php?latex=H=\\frac{2E||X-Y||&space;-&space;E||X-X\'||&space;-&space;E||Y-Y\'||}{2E||X-Y||}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?H=\\frac{2E||X-Y||&space;-&space;E||X-X\'||&space;-&space;E||Y-Y\'||}{2E||X-Y||}" title="H=\\frac{2E||X-Y|| - E||X-X\'|| - E||Y-Y\'||}{2E||X-Y||}" /></a>\n\n\n```\nfrom signal_processing_algorithms.energy_statistics import energy_statistics\nfrom some_module import series1, series2\n\n# To get Energy Statistics of the distributions.\nes = energy_statistics.get_energy_statistics(series1, series2)\n\n# To get Energy Statistics and permutation test results of the distributions.\nes_with_probabilities = energy_statistics.get_energy_statistics_and_probabilities(series1, series2, permutations=100)\n\n```\n\n## Intro to E-Divisive\n\nDetecting distributional changes in a series of numerical values can be surprisingly difficult. Simple systems based on thresholds or\n mean values can be yield false positives due to outliers in the data, and will fail to detect changes in the noise\n profile of the series you are analyzing.\n \nOne robust way of detecting many of the changes missed by other approaches is to use [E-Divisive with Means](https://arxiv.org/pdf/1306.4933.pdf), an energy\n statistic based approach that compares the expected distance (Euclidean norm) between samples of two portions of the\n series with the expected distance between samples within those portions.\n \nThat is to say, assuming that the two portions can each be modeled as i.i.d. samples drawn from distinct random variables\n (X for the first portion, Y for the second portion), you would expect the E-statistic to be non-zero if there is a\n difference between the two portions: \n \n <a href="https://www.codecogs.com/eqnedit.php?latex=E_{n,m}(X,Y):=2A-B-C" target="_blank"><img src="https://latex.codecogs.com/gif.latex?E_{n,m}(X,Y):=2A-B-C" title="E_{n,m}(X,Y):=2A-B-C" /></a>\n where A, B and C are as defined in the Energy Statistics above.\n\nOne can prove that <a href="https://www.codecogs.com/eqnedit.php?latex={E_{n,m}(X,Y)\\geq&space;0}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?{E_{n,m}(X,Y)\\geq&space;0}" title="{E_{n,m}(X,Y)\\geq 0}" /></a> and that the corresponding population value is zero if and only if X and Y have the same distribution. Under this null hypothesis the test statistic\n\n<a href="https://www.codecogs.com/eqnedit.php?latex=T={\\frac&space;{nm}{n&plus;m}}E_{{n,m}}(X,Y)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?T={\\frac&space;{nm}{n&plus;m}}E_{{n,m}}(X,Y)" title="T={\\frac {nm}{n+m}}E_{{n,m}}(X,Y)" /></a>\n\nconverges in distribution to a quadratic form of independent standard normal random variables. Under the alternative hypothesis T tends to infinity. This makes it possible to construct a consistent statistical test, the energy test for equal distributions\n  \nThus for a series Z of length L,\n\n<a href="https://www.codecogs.com/eqnedit.php?latex=Z&space;=&space;\\{Z_{1},&space;...,&space;Z_{\\tau}&space;,&space;...&space;,&space;Z_{L}\\},&space;X&space;=\\{Z_{1},...,Z_{\\tau}\\},&space;Y=\\{Z_{\\tau&plus;1}\\,...,Z_{L}\\}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?Z&space;=&space;\\{Z_{1},&space;...,&space;Z_{\\tau}&space;,&space;...&space;,&space;Z_{L}\\},&space;X&space;=\\{Z_{1},...,Z_{\\tau}\\},&space;Y=\\{Z_{\\tau&plus;1}\\,...,Z_{L}\\}" title="Z = \\{Z_{1}, ..., Z_{\\tau} , ... , Z_{L}\\}, X =\\{Z_{1},...,Z_{\\tau}\\}, Y=\\{Z_{\\tau+1}\\,...,Z_{L}\\}" /></a>\n\nwe find the most likely change point by solving the following for &tau; such that it has the maximum T statistic value.\n\n### Multiple Change Points\n\nThe algorithm for finding multiple change points is also simple.\n\nAssuming you have some k known change points:\n1. Partition the series into segments between/around these change points.\n2. Find the maximum value of our divergence metric _within_ each partition.\n3. Take the maximum of the maxima we have just found --> this is our k+1th change point.\n4. Return to step 1 and continue until reaching your stopping criterion.\n\n### Stopping Criterion\n\nIn this package we have implemented a permutation based test as a stopping criterion:\n\nAfter step 3 of the multiple change point procedure above, randomly permute all of the data _within_ each cluster, and\n find the most likely change point for this permuted data using the procedure laid out above. \n \nAfter performing this operation z times, count the number of\n permuted change points z\' that have higher divergence metrics than the change point you calculated with un-permuted data.\n The significance level of your change point is thus z\'/(z+1). \n\nWe allow users to configure a permutation tester with `pvalue`\n and `permutations` representing the significance cutoff for algorithm termination and permutations to perform for each\n test, respectively.\n \n### Example\n```\nfrom signal_processing_algorithms.energy_statistics import energy_statistics\nfrom some_module import series\n\nchange_points = energy_statistics.e_divisive(series, pvalue=0.01, permutations=100)\n```\n\n',
     'author': 'Alexander Costas',
     'author_email': 'alexander.costas@mongodb.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/mongodb/signal-processing-algorithms',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

#### html2text {}

```diff
@@ -1,49 +1,51 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['signal_processing_algorithms',
 'signal_processing_algorithms.energy_statistics'] package_data = \ {'': ['*']}
-install_requires = \ ['more-itertools>=8.2.0,<9.0.0', 'numpy>=1.18.1,<2.0.0',
-'scipy>=1.3,<2.0', 'structlog>=19.1,<20.0', 'typing-extensions>=3.7.4,<4.0.0']
-setup_kwargs = { 'name': 'signal-processing-algorithms', 'version': '2.0.1',
-'description': 'Signal Processing Algorithms from MongoDB', 'long_description':
-'# Signal Processing Algorithms\n\nA suite of algorithms implementing
-[Energy\nStatistics](https://en.wikipedia.org/wiki/Energy_distance), [E-
-Divisive with\nMeans](https://arxiv.org/pdf/1306.4933.pdf) and [Generalized ESD
-Test for\nOutliers](https://www.itl.nist.gov/div898/handbook/eda/section3/
-eda35h3.htm) in python. See [The Use\nof Change Point Detection to Identify
-Software Performance Regressions in a Continuous Integration\nSystem](https://
-dl.acm.org/doi/abs/10.1145/3358960.3375791) and [Creating a Virtuous Cycle
-in\nPerformance Testing at MongoDB](https://dl.acm.org/doi/pdf/10.1145/
-3427921.3450234) for background\non the development and use of this
-library.\n\n## Getting Started - Users\n```\npip install signal-processing-
-algorithms\n```\n\n## Getting Started - Developers\n\nGetting the code:
-\n\n```\n$ git clone git@github.com:mongodb/signal-processing-algorithms.git\n$
-cd signal-processing-algorithms\n```\n\nInstallation\n```\n$ pip install
-poetry\n$ poetry install\n```\nTesting/linting:\n```\n$ poetry run
-pytest\n```\n\nRunning the slow tests:\n```\n$ poetry run pytest --
-runslow\n```\n\n**Some of the larger tests can take a significant amount of
-time (more than 2 hours).**\n\n## Energy statistics\n[Energy Statistics](https:
-//en.wikipedia.org/wiki/Energy_distance) is the statistical concept of Energy
-Distance \nand can be used to measure how similar/different two distributions
-are.\n\nFor statistical samples from two random variables X and Y:\nx1, x2,
-..., xn and y1, y2, ..., yn\n\nE-Statistic is defined as:\n\n[https://
-latex.codecogs.com/gif.latex?E_{n,m}(X,Y):=2A-B-C]\n\nwhere,\n\n[https://
-latex.codecogs.com/gif.latex?A:={\\frac&space;{1}{nm}}\\sum&space;_{i=1}^
-{n}\\sum&space;_{j=1}^{m}\\|x_{i}-y_{j}\\|,B:={\\frac&space;{1}{n^
-{2}}}\\sum&space;_{i=1}^{n}\\sum&space;_{j=1}^{n}\\|x_{i}-x_{j}\\|,C:=
-{\\frac&space;{1}{m^{2}}}\\sum&space;_{i=1}^{m}\\sum&space;_{j=1}^{m}\\|y_{i}-
-y_{j}\\|]\n\nT-statistic is defined as: \n\n[https://latex.codecogs.com/
-gif.latex?T={\\frac&space;{nm}{n&plus;m}}E_{{n,m}}(X,Y)]\n\nE-coefficient of
-inhomogeneity is defined as:\n\n[https://latex.codecogs.com/gif.latex?H=\\frac
-{2E||X-Y||&space;-&space;E||X-X\'||&space;-&space;E||Y-Y\'||}{2E||X-
-Y||}]\n\n\n```\nfrom signal_processing_algorithms.energy_statistics import
-energy_statistics\nfrom some_module import series1, series2\n\n# To get Energy
-Statistics of the distributions.\nes = energy_statistics.get_energy_statistics
-(series1, series2)\n\n# To get Energy Statistics and permutation test results
-of the distributions.\nes_with_probabilities =
+install_requires = \ ['gevent>=21.12.0,<22.0.0', 'greenlet>=1.1.0,<2.0.0',
+'more-itertools>=8.2.0,<9.0.0', 'numpy>=1.24.4,<2.0.0', 'pyyaml>=6.0.0,<7.0.0',
+'scipy>=1.8.1,<2.0.0', 'setuptools<60.0.0', 'structlog>=19.1,<20.0', 'typed-
+ast>=1.5.0,<2.0.0', 'typing-extensions>=4.5.0,<5.0.0'] setup_kwargs = { 'name':
+'signal-processing-algorithms', 'version': '2.1.0', 'description': 'Signal
+Processing Algorithms from MongoDB', 'long_description': '# Signal Processing
+Algorithms\n\nA suite of algorithms implementing [Energy\nStatistics](https://
+en.wikipedia.org/wiki/Energy_distance), [E-Divisive with\nMeans](https://
+arxiv.org/pdf/1306.4933.pdf) and [Generalized ESD Test for\nOutliers](https://
+www.itl.nist.gov/div898/handbook/eda/section3/eda35h3.htm) in python. See [The
+Use\nof Change Point Detection to Identify Software Performance Regressions in
+a Continuous Integration\nSystem](https://dl.acm.org/doi/abs/10.1145/
+3358960.3375791) and [Creating a Virtuous Cycle in\nPerformance Testing at
+MongoDB](https://dl.acm.org/doi/pdf/10.1145/3427921.3450234) for background\non
+the development and use of this library.\n\n## Getting Started -
+Users\n```\npip install signal-processing-algorithms\n```\n\n## Getting Started
+- Developers\n\nGetting the code:\n\n```\n$ git clone git@github.com:mongodb/
+signal-processing-algorithms.git\n$ cd signal-processing-
+algorithms\n```\n\nInstallation\n```\n$ pip install poetry\n$ poetry
+install\n```\nTesting/linting:\n```\n$ poetry run pytest\n```\n\nRunning the
+slow tests:\n```\n$ poetry run pytest --runslow\n```\n\n**Some of the larger
+tests can take a significant amount of time (more than 2 hours).**\n\n## Energy
+statistics\n[Energy Statistics](https://en.wikipedia.org/wiki/Energy_distance)
+is the statistical concept of Energy Distance \nand can be used to measure how
+similar/different two distributions are.\n\nFor statistical samples from two
+random variables X and Y:\nx1, x2, ..., xn and y1, y2, ..., yn\n\nE-Statistic
+is defined as:\n\n[https://latex.codecogs.com/gif.latex?E_{n,m}(X,Y):=2A-B-
+C]\n\nwhere,\n\n[https://latex.codecogs.com/gif.latex?A:={\\frac&space;{1}
+{nm}}\\sum&space;_{i=1}^{n}\\sum&space;_{j=1}^{m}\\|x_{i}-y_{j}\\|,B:=
+{\\frac&space;{1}{n^{2}}}\\sum&space;_{i=1}^{n}\\sum&space;_{j=1}^{n}\\|x_{i}-
+x_{j}\\|,C:={\\frac&space;{1}{m^{2}}}\\sum&space;_{i=1}^{m}\\sum&space;_{j=1}^
+{m}\\|y_{i}-y_{j}\\|]\n\nT-statistic is defined as: \n\n[https://
+latex.codecogs.com/gif.latex?T={\\frac&space;{nm}{n&plus;m}}E_{{n,m}}
+(X,Y)]\n\nE-coefficient of inhomogeneity is defined as:\n\n[https://
+latex.codecogs.com/gif.latex?H=\\frac{2E||X-Y||&space;-&space;E||X-
+X\'||&space;-&space;E||Y-Y\'||}{2E||X-Y||}]\n\n\n```\nfrom
+signal_processing_algorithms.energy_statistics import energy_statistics\nfrom
+some_module import series1, series2\n\n# To get Energy Statistics of the
+distributions.\nes = energy_statistics.get_energy_statistics(series1,
+series2)\n\n# To get Energy Statistics and permutation test results of the
+distributions.\nes_with_probabilities =
 energy_statistics.get_energy_statistics_and_probabilities(series1, series2,
 permutations=100)\n\n```\n\n## Intro to E-Divisive\n\nDetecting distributional
 changes in a series of numerical values can be surprisingly difficult. Simple
 systems based on thresholds or\n mean values can be yield false positives due
 to outliers in the data, and will fail to detect changes in the noise\n profile
 of the series you are analyzing.\n \nOne robust way of detecting many of the
 changes missed by other approaches is to use [E-Divisive with Means](https://
@@ -85,12 +87,12 @@
 \n\nWe allow users to configure a permutation tester with `pvalue`\n and
 `permutations` representing the significance cutoff for algorithm termination
 and permutations to perform for each\n test, respectively.\n \n###
 Example\n```\nfrom signal_processing_algorithms.energy_statistics import
 energy_statistics\nfrom some_module import series\n\nchange_points =
 energy_statistics.e_divisive(series, pvalue=0.01, permutations=100)\n```\n\n',
 'author': 'Alexander Costas', 'author_email': 'alexander.costas@mongodb.com',
-'maintainer': None, 'maintainer_email': None, 'url': 'https://github.com/
+'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
 mongodb/signal-processing-algorithms', 'package_dir': package_dir, 'packages':
 packages, 'package_data': package_data, 'install_requires': install_requires,
 'python_requires': '>=3.8,<4.0', } from build import * build(setup_kwargs)
 setup(**setup_kwargs)
```

### Comparing `signal-processing-algorithms-2.0.1/PKG-INFO` & `signal_processing_algorithms-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: signal-processing-algorithms
-Version: 2.0.1
+Version: 2.1.0
 Summary: Signal Processing Algorithms from MongoDB
 Home-page: https://github.com/mongodb/signal-processing-algorithms
 License: Apache-2.0
 Author: Alexander Costas
 Author-email: alexander.costas@mongodb.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: gevent (>=21.12.0,<22.0.0)
+Requires-Dist: greenlet (>=1.1.0,<2.0.0)
 Requires-Dist: more-itertools (>=8.2.0,<9.0.0)
-Requires-Dist: numpy (>=1.18.1,<2.0.0)
-Requires-Dist: scipy (>=1.3,<2.0)
+Requires-Dist: numpy (>=1.24.4,<2.0.0)
+Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
+Requires-Dist: scipy (>=1.8.1,<2.0.0)
+Requires-Dist: setuptools (<60.0.0)
 Requires-Dist: structlog (>=19.1,<20.0)
-Requires-Dist: typing-extensions (>=3.7.4,<4.0.0)
+Requires-Dist: typed-ast (>=1.5.0,<2.0.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/mongodb/signal-processing-algorithms
 Description-Content-Type: text/markdown
 
 # Signal Processing Algorithms
 
 A suite of algorithms implementing [Energy
 Statistics](https://en.wikipedia.org/wiki/Energy_distance), [E-Divisive with
```

#### html2text {}

```diff
@@ -1,47 +1,51 @@
-Metadata-Version: 2.1 Name: signal-processing-algorithms Version: 2.0.1
+Metadata-Version: 2.1 Name: signal-processing-algorithms Version: 2.1.0
 Summary: Signal Processing Algorithms from MongoDB Home-page: https://
 github.com/mongodb/signal-processing-algorithms License: Apache-2.0 Author:
 Alexander Costas Author-email: alexander.costas@mongodb.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Requires-Dist: more-itertools
-(>=8.2.0,<9.0.0) Requires-Dist: numpy (>=1.18.1,<2.0.0) Requires-Dist: scipy
-(>=1.3,<2.0) Requires-Dist: structlog (>=19.1,<20.0) Requires-Dist: typing-
-extensions (>=3.7.4,<4.0.0) Project-URL: Repository, https://github.com/
-mongodb/signal-processing-algorithms Description-Content-Type: text/markdown #
-Signal Processing Algorithms A suite of algorithms implementing [Energy
-Statistics](https://en.wikipedia.org/wiki/Energy_distance), [E-Divisive with
-Means](https://arxiv.org/pdf/1306.4933.pdf) and [Generalized ESD Test for
-Outliers](https://www.itl.nist.gov/div898/handbook/eda/section3/eda35h3.htm) in
-python. See [The Use of Change Point Detection to Identify Software Performance
-Regressions in a Continuous Integration System](https://dl.acm.org/doi/abs/
-10.1145/3358960.3375791) and [Creating a Virtuous Cycle in Performance Testing
-at MongoDB](https://dl.acm.org/doi/pdf/10.1145/3427921.3450234) for background
-on the development and use of this library. ## Getting Started - Users ``` pip
-install signal-processing-algorithms ``` ## Getting Started - Developers
-Getting the code: ``` $ git clone git@github.com:mongodb/signal-processing-
-algorithms.git $ cd signal-processing-algorithms ``` Installation ``` $ pip
-install poetry $ poetry install ``` Testing/linting: ``` $ poetry run pytest
-``` Running the slow tests: ``` $ poetry run pytest --runslow ``` **Some of the
-larger tests can take a significant amount of time (more than 2 hours).** ##
-Energy statistics [Energy Statistics](https://en.wikipedia.org/wiki/
-Energy_distance) is the statistical concept of Energy Distance and can be used
-to measure how similar/different two distributions are. For statistical samples
-from two random variables X and Y: x1, x2, ..., xn and y1, y2, ..., yn E-
-Statistic is defined as: [https://latex.codecogs.com/gif.latex?E_{n,m}(X,Y):
-=2A-B-C] where, [https://latex.codecogs.com/gif.latex?A:={\frac&space;{1}
-{nm}}\sum&space;_{i=1}^{n}\sum&space;_{j=1}^{m}\|x_{i}-y_{j}\|,B:={\frac&space;
-{1}{n^{2}}}\sum&space;_{i=1}^{n}\sum&space;_{j=1}^{n}\|x_{i}-x_{j}\|,C:=
-{\frac&space;{1}{m^{2}}}\sum&space;_{i=1}^{m}\sum&space;_{j=1}^{m}\|y_{i}-y_
-{j}\|] T-statistic is defined as: [https://latex.codecogs.com/gif.latex?T=
-{\frac&space;{nm}{n&plus;m}}E_{{n,m}}(X,Y)] E-coefficient of inhomogeneity is
-defined as: [https://latex.codecogs.com/gif.latex?H=\frac{2E||X-Y||&space;-
-&space;E||X-X'||&space;-&space;E||Y-Y'||}{2E||X-Y||}] ``` from
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: gevent (>=21.12.0,<22.0.0) Requires-
+Dist: greenlet (>=1.1.0,<2.0.0) Requires-Dist: more-itertools (>=8.2.0,<9.0.0)
+Requires-Dist: numpy (>=1.24.4,<2.0.0) Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
+Requires-Dist: scipy (>=1.8.1,<2.0.0) Requires-Dist: setuptools (<60.0.0)
+Requires-Dist: structlog (>=19.1,<20.0) Requires-Dist: typed-ast
+(>=1.5.0,<2.0.0) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Project-URL:
+Repository, https://github.com/mongodb/signal-processing-algorithms
+Description-Content-Type: text/markdown # Signal Processing Algorithms A suite
+of algorithms implementing [Energy Statistics](https://en.wikipedia.org/wiki/
+Energy_distance), [E-Divisive with Means](https://arxiv.org/pdf/1306.4933.pdf)
+and [Generalized ESD Test for Outliers](https://www.itl.nist.gov/div898/
+handbook/eda/section3/eda35h3.htm) in python. See [The Use of Change Point
+Detection to Identify Software Performance Regressions in a Continuous
+Integration System](https://dl.acm.org/doi/abs/10.1145/3358960.3375791) and
+[Creating a Virtuous Cycle in Performance Testing at MongoDB](https://
+dl.acm.org/doi/pdf/10.1145/3427921.3450234) for background on the development
+and use of this library. ## Getting Started - Users ``` pip install signal-
+processing-algorithms ``` ## Getting Started - Developers Getting the code: ```
+$ git clone git@github.com:mongodb/signal-processing-algorithms.git $ cd
+signal-processing-algorithms ``` Installation ``` $ pip install poetry $ poetry
+install ``` Testing/linting: ``` $ poetry run pytest ``` Running the slow
+tests: ``` $ poetry run pytest --runslow ``` **Some of the larger tests can
+take a significant amount of time (more than 2 hours).** ## Energy statistics
+[Energy Statistics](https://en.wikipedia.org/wiki/Energy_distance) is the
+statistical concept of Energy Distance and can be used to measure how similar/
+different two distributions are. For statistical samples from two random
+variables X and Y: x1, x2, ..., xn and y1, y2, ..., yn E-Statistic is defined
+as: [https://latex.codecogs.com/gif.latex?E_{n,m}(X,Y):=2A-B-C] where, [https:/
+/latex.codecogs.com/gif.latex?A:={\frac&space;{1}{nm}}\sum&space;_{i=1}^
+{n}\sum&space;_{j=1}^{m}\|x_{i}-y_{j}\|,B:={\frac&space;{1}{n^{2}}}\sum&space;_
+{i=1}^{n}\sum&space;_{j=1}^{n}\|x_{i}-x_{j}\|,C:={\frac&space;{1}{m^
+{2}}}\sum&space;_{i=1}^{m}\sum&space;_{j=1}^{m}\|y_{i}-y_{j}\|] T-statistic is
+defined as: [https://latex.codecogs.com/gif.latex?T={\frac&space;{nm}
+{n&plus;m}}E_{{n,m}}(X,Y)] E-coefficient of inhomogeneity is defined as:
+[https://latex.codecogs.com/gif.latex?H=\frac{2E||X-Y||&space;-&space;E||X-
+X'||&space;-&space;E||Y-Y'||}{2E||X-Y||}] ``` from
 signal_processing_algorithms.energy_statistics import energy_statistics from
 some_module import series1, series2 # To get Energy Statistics of the
 distributions. es = energy_statistics.get_energy_statistics(series1, series2) #
 To get Energy Statistics and permutation test results of the distributions.
 es_with_probabilities =
 energy_statistics.get_energy_statistics_and_probabilities(series1, series2,
 permutations=100) ``` ## Intro to E-Divisive Detecting distributional changes
```

