# Comparing `tmp/FinQuant-0.4.0.tar.gz` & `tmp/FinQuant-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinQuant-0.4.0.tar", last modified: Sun Jul 23 20:38:51 2023, max compression
+gzip compressed data, was "FinQuant-0.5.0.tar", last modified: Wed Aug  2 14:42:03 2023, max compression
```

## Comparing `FinQuant-0.4.0.tar` & `FinQuant-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:38:51.294643 FinQuant-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:38:51.294643 FinQuant-0.4.0/FinQuant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-07-23 20:38:51.000000 FinQuant-0.4.0/FinQuant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-23 20:38:51.000000 FinQuant-0.4.0/FinQuant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 20:38:51.000000 FinQuant-0.4.0/FinQuant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-23 20:38:51.000000 FinQuant-0.4.0/FinQuant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-23 20:38:51.000000 FinQuant-0.4.0/FinQuant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-23 20:38:11.000000 FinQuant-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-07-23 20:38:51.298643 FinQuant-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-07-23 20:38:11.000000 FinQuant-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:38:51.294643 FinQuant-0.4.0/finquant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 20:38:11.000000 FinQuant-0.4.0/finquant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-23 20:38:11.000000 FinQuant-0.4.0/finquant/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-07-23 20:38:11.000000 FinQuant-0.4.0/finquant/efficient_frontier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-23 20:38:11.000000 FinQuant-0.4.0/finquant/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-23 20:38:11.000000 FinQuant-0.4.0/finquant/minimise_fun.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-23 20:38:11.000000 FinQuant-0.4.0/finquant/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-23 20:38:11.000000 FinQuant-0.4.0/finquant/moving_average.py
--rw-r--r--   0 runner    (1001) docker     (123)    48218 2023-07-23 20:38:11.000000 FinQuant-0.4.0/finquant/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-23 20:38:11.000000 FinQuant-0.4.0/finquant/quants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-23 20:38:11.000000 FinQuant-0.4.0/finquant/returns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-23 20:38:11.000000 FinQuant-0.4.0/finquant/stock.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-23 20:38:11.000000 FinQuant-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-23 20:38:51.298643 FinQuant-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-23 20:38:11.000000 FinQuant-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:38:51.294643 FinQuant-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-23 20:38:11.000000 FinQuant-0.4.0/tests/test_efficient_frontier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-23 20:38:11.000000 FinQuant-0.4.0/tests/test_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-23 20:38:11.000000 FinQuant-0.4.0/tests/test_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-23 20:38:11.000000 FinQuant-0.4.0/tests/test_optimisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-23 20:38:11.000000 FinQuant-0.4.0/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-23 20:38:11.000000 FinQuant-0.4.0/tests/test_quants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-23 20:38:11.000000 FinQuant-0.4.0/tests/test_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-23 20:38:11.000000 FinQuant-0.4.0/tests/test_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:03.066974 FinQuant-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:03.066974 FinQuant-0.5.0/FinQuant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-08-02 14:42:02.000000 FinQuant-0.5.0/FinQuant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-02 14:42:03.000000 FinQuant-0.5.0/FinQuant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:42:02.000000 FinQuant-0.5.0/FinQuant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-02 14:42:02.000000 FinQuant-0.5.0/FinQuant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 14:42:02.000000 FinQuant-0.5.0/FinQuant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 14:41:18.000000 FinQuant-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-08-02 14:42:03.066974 FinQuant-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-08-02 14:41:18.000000 FinQuant-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:03.066974 FinQuant-0.5.0/finquant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:18.000000 FinQuant-0.5.0/finquant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-08-02 14:41:18.000000 FinQuant-0.5.0/finquant/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-08-02 14:41:18.000000 FinQuant-0.5.0/finquant/efficient_frontier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-02 14:41:18.000000 FinQuant-0.5.0/finquant/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-02 14:41:18.000000 FinQuant-0.5.0/finquant/minimise_fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-08-02 14:41:18.000000 FinQuant-0.5.0/finquant/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-08-02 14:41:18.000000 FinQuant-0.5.0/finquant/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49729 2023-08-02 14:41:18.000000 FinQuant-0.5.0/finquant/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-08-02 14:41:18.000000 FinQuant-0.5.0/finquant/quants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-02 14:41:18.000000 FinQuant-0.5.0/finquant/returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-02 14:41:18.000000 FinQuant-0.5.0/finquant/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-02 14:41:18.000000 FinQuant-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-02 14:42:03.070974 FinQuant-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-02 14:41:18.000000 FinQuant-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:03.066974 FinQuant-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-02 14:41:18.000000 FinQuant-0.5.0/tests/test_efficient_frontier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-02 14:41:18.000000 FinQuant-0.5.0/tests/test_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-08-02 14:41:18.000000 FinQuant-0.5.0/tests/test_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-02 14:41:18.000000 FinQuant-0.5.0/tests/test_optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-08-02 14:41:18.000000 FinQuant-0.5.0/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-08-02 14:41:18.000000 FinQuant-0.5.0/tests/test_quants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-08-02 14:41:18.000000 FinQuant-0.5.0/tests/test_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-02 14:41:18.000000 FinQuant-0.5.0/tests/test_stock.py
```

### Comparing `FinQuant-0.4.0/FinQuant.egg-info/PKG-INFO` & `FinQuant-0.5.0/FinQuant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: FinQuant
-Version: 0.4.0
+Version: 0.5.0
 Summary: A program for financial portfolio management, analysis and optimisation
 Home-page: https://github.com/fmilthaler/FinQuant
-Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.4.0.tar.gz
+Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.5.0.tar.gz
 Author: Frank Milthaler
 Author-email: f.milthaler@gmail.com
 License: MIT
 Project-URL: Documentation, https://finquant.readthedocs.io
 Keywords: finance,portfolio,investment,numerical,optimisation,monte carlo,efficient frontier,quantitative,quant
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -17,30 +17,30 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
+Provides-Extra: cd
 Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: cd
+Provides-Extra: test
 License-File: LICENSE.txt
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-logo.png" width="45%">
 </p>
 
 <p align="center">
   <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
     <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
   </a>
   <a href="https://pypi.org/project/FinQuant">
-    <img src="https://img.shields.io/badge/pypi-v0.4.0-brightgreen.svg?style=popout" alt='pypi'>
+    <img src="https://img.shields.io/badge/pypi-v0.5.0-brightgreen.svg?style=popout" alt='pypi'>
   </a>
   <a href="https://github.com/fmilthaler/FinQuant">
     <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
   </a>
   <a href="http://finquant.readthedocs.io/">
     <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
   </a>
@@ -274,16 +274,19 @@
 ### Building a portfolio with preset data
 `./example/Example-Build-Portfolio-from-file.py`: Shows how to use *FinQuant* to build a financial portfolio by providing stock price data yourself, e.g. by reading data from disk/file.
 
 ### Analysis of a portfolio
 `./example/Example-Analysis.py`: This example shows how to use an instance of `finquant.portfolio.Portfolio`, get the portfolio's quantities, such as
  - Expected Returns,
  - Volatility,
+ - Downside Risk,
+ - Value at Risk, 
  - Sharpe Ratio,
- - Value at Risk.
+ - Sortino Ratio,
+ - Beta parameter.
 
 It also shows how to extract individual stocks from the given portfolio. Moreover it shows how to compute and visualise:
  - the different Returns provided by the module `finquant.returns`,
  - *Moving Averages*, a band of *Moving Averages*, and a *Bollinger Band*.
 
 ### Optimisation of a portfolio
 `./example/Example-Optimisation.py`: This example focusses on the optimisation of a portfolio. To achieve this, the example shows the usage of `finquant.efficient_frontier.EfficientFrontier` for optimising the portfolio, for the
@@ -293,8 +296,7 @@
  - Maximum Sharpe Ratio for a given target Volatility.
 
 Furthermore, it is also shown how the entire *Efficient Frontier* and the optimal portfolios can be computed and visualised. If needed, it also gives an example of plotting the individual stocks of the given portfolio within the computed *Efficient Frontier*.
 
 Also, the optimisation of a portfolio and its visualisation based on a *Monte Carlo* is shown.
 
 Finally, *FinQuant*'s visualisation methods allow for overlays, if this is desired. Thus, with only the following few lines of code, one can create an overlay of the *Monte Carlo* run, the *Efficient Frontier*, its optimised portfolios for *Minimum Volatility* and *Maximum Sharpe Ratio*, as well as the portfolio's individual stocks.
-
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: FinQuant Version: 0.4.0 Summary: A program for
+Metadata-Version: 2.1 Name: FinQuant Version: 0.5.0 Summary: A program for
 financial portfolio management, analysis and optimisation Home-page: https://
 github.com/fmilthaler/FinQuant Download-URL: https://github.com/fmilthaler/
-FinQuant/archive/v0.4.0.tar.gz Author: Frank Milthaler Author-email:
+FinQuant/archive/v0.5.0.tar.gz Author: Frank Milthaler Author-email:
 f.milthaler@gmail.com License: MIT Project-URL: Documentation, https://
 finquant.readthedocs.io Keywords:
 finance,portfolio,investment,numerical,optimisation,monte carlo,efficient
 frontier,quantitative,quant Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
-Provides-Extra: test Provides-Extra: dev Provides-Extra: docs Provides-Extra:
-cd License-File: LICENSE.txt
+Provides-Extra: cd Provides-Extra: dev Provides-Extra: docs Provides-Extra:
+test License-File: LICENSE.txt
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-
                                    logo.png]
 [pypi] [pypi] [GitHub_Actions] [docs] [contributors] [contributions] [license]
 # FinQuant *FinQuant* is a program for financial **portfolio management,
 analysis and optimisation**. This README only gives a brief overview of
 *FinQuant*. The interested reader should refer to its [documentation](https://
 finquant.readthedocs.io "FinQuant Documentation"). ## Table of contents -
@@ -153,21 +153,22 @@
 from-web.py`: Shows how to use *FinQuant* to build a financial portfolio by
 downloading stock price data through the Python package `quandl`/`yfinance`.
 ### Building a portfolio with preset data `./example/Example-Build-Portfolio-
 from-file.py`: Shows how to use *FinQuant* to build a financial portfolio by
 providing stock price data yourself, e.g. by reading data from disk/file. ###
 Analysis of a portfolio `./example/Example-Analysis.py`: This example shows how
 to use an instance of `finquant.portfolio.Portfolio`, get the portfolio's
-quantities, such as - Expected Returns, - Volatility, - Sharpe Ratio, - Value
-at Risk. It also shows how to extract individual stocks from the given
-portfolio. Moreover it shows how to compute and visualise: - the different
-Returns provided by the module `finquant.returns`, - *Moving Averages*, a band
-of *Moving Averages*, and a *Bollinger Band*. ### Optimisation of a portfolio
-`./example/Example-Optimisation.py`: This example focusses on the optimisation
-of a portfolio. To achieve this, the example shows the usage of
+quantities, such as - Expected Returns, - Volatility, - Downside Risk, - Value
+at Risk, - Sharpe Ratio, - Sortino Ratio, - Beta parameter. It also shows how
+to extract individual stocks from the given portfolio. Moreover it shows how to
+compute and visualise: - the different Returns provided by the module
+`finquant.returns`, - *Moving Averages*, a band of *Moving Averages*, and a
+*Bollinger Band*. ### Optimisation of a portfolio `./example/Example-
+Optimisation.py`: This example focusses on the optimisation of a portfolio. To
+achieve this, the example shows the usage of
 `finquant.efficient_frontier.EfficientFrontier` for optimising the portfolio,
 for the - Minimum Volatility - Maximum Sharpe Ratio - Minimum Volatility for a
 given target Return - Maximum Sharpe Ratio for a given target Volatility.
 Furthermore, it is also shown how the entire *Efficient Frontier* and the
 optimal portfolios can be computed and visualised. If needed, it also gives an
 example of plotting the individual stocks of the given portfolio within the
 computed *Efficient Frontier*. Also, the optimisation of a portfolio and its
```

### Comparing `FinQuant-0.4.0/FinQuant.egg-info/SOURCES.txt` & `FinQuant-0.5.0/FinQuant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FinQuant-0.4.0/LICENSE.txt` & `FinQuant-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FinQuant-0.4.0/PKG-INFO` & `FinQuant-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: FinQuant
-Version: 0.4.0
+Version: 0.5.0
 Summary: A program for financial portfolio management, analysis and optimisation
 Home-page: https://github.com/fmilthaler/FinQuant
-Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.4.0.tar.gz
+Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.5.0.tar.gz
 Author: Frank Milthaler
 Author-email: f.milthaler@gmail.com
 License: MIT
 Project-URL: Documentation, https://finquant.readthedocs.io
 Keywords: finance,portfolio,investment,numerical,optimisation,monte carlo,efficient frontier,quantitative,quant
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -17,30 +17,30 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
+Provides-Extra: cd
 Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: cd
+Provides-Extra: test
 License-File: LICENSE.txt
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-logo.png" width="45%">
 </p>
 
 <p align="center">
   <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
     <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
   </a>
   <a href="https://pypi.org/project/FinQuant">
-    <img src="https://img.shields.io/badge/pypi-v0.4.0-brightgreen.svg?style=popout" alt='pypi'>
+    <img src="https://img.shields.io/badge/pypi-v0.5.0-brightgreen.svg?style=popout" alt='pypi'>
   </a>
   <a href="https://github.com/fmilthaler/FinQuant">
     <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
   </a>
   <a href="http://finquant.readthedocs.io/">
     <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
   </a>
@@ -274,16 +274,19 @@
 ### Building a portfolio with preset data
 `./example/Example-Build-Portfolio-from-file.py`: Shows how to use *FinQuant* to build a financial portfolio by providing stock price data yourself, e.g. by reading data from disk/file.
 
 ### Analysis of a portfolio
 `./example/Example-Analysis.py`: This example shows how to use an instance of `finquant.portfolio.Portfolio`, get the portfolio's quantities, such as
  - Expected Returns,
  - Volatility,
+ - Downside Risk,
+ - Value at Risk, 
  - Sharpe Ratio,
- - Value at Risk.
+ - Sortino Ratio,
+ - Beta parameter.
 
 It also shows how to extract individual stocks from the given portfolio. Moreover it shows how to compute and visualise:
  - the different Returns provided by the module `finquant.returns`,
  - *Moving Averages*, a band of *Moving Averages*, and a *Bollinger Band*.
 
 ### Optimisation of a portfolio
 `./example/Example-Optimisation.py`: This example focusses on the optimisation of a portfolio. To achieve this, the example shows the usage of `finquant.efficient_frontier.EfficientFrontier` for optimising the portfolio, for the
@@ -293,8 +296,7 @@
  - Maximum Sharpe Ratio for a given target Volatility.
 
 Furthermore, it is also shown how the entire *Efficient Frontier* and the optimal portfolios can be computed and visualised. If needed, it also gives an example of plotting the individual stocks of the given portfolio within the computed *Efficient Frontier*.
 
 Also, the optimisation of a portfolio and its visualisation based on a *Monte Carlo* is shown.
 
 Finally, *FinQuant*'s visualisation methods allow for overlays, if this is desired. Thus, with only the following few lines of code, one can create an overlay of the *Monte Carlo* run, the *Efficient Frontier*, its optimised portfolios for *Minimum Volatility* and *Maximum Sharpe Ratio*, as well as the portfolio's individual stocks.
-
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: FinQuant Version: 0.4.0 Summary: A program for
+Metadata-Version: 2.1 Name: FinQuant Version: 0.5.0 Summary: A program for
 financial portfolio management, analysis and optimisation Home-page: https://
 github.com/fmilthaler/FinQuant Download-URL: https://github.com/fmilthaler/
-FinQuant/archive/v0.4.0.tar.gz Author: Frank Milthaler Author-email:
+FinQuant/archive/v0.5.0.tar.gz Author: Frank Milthaler Author-email:
 f.milthaler@gmail.com License: MIT Project-URL: Documentation, https://
 finquant.readthedocs.io Keywords:
 finance,portfolio,investment,numerical,optimisation,monte carlo,efficient
 frontier,quantitative,quant Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
-Provides-Extra: test Provides-Extra: dev Provides-Extra: docs Provides-Extra:
-cd License-File: LICENSE.txt
+Provides-Extra: cd Provides-Extra: dev Provides-Extra: docs Provides-Extra:
+test License-File: LICENSE.txt
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-
                                    logo.png]
 [pypi] [pypi] [GitHub_Actions] [docs] [contributors] [contributions] [license]
 # FinQuant *FinQuant* is a program for financial **portfolio management,
 analysis and optimisation**. This README only gives a brief overview of
 *FinQuant*. The interested reader should refer to its [documentation](https://
 finquant.readthedocs.io "FinQuant Documentation"). ## Table of contents -
@@ -153,21 +153,22 @@
 from-web.py`: Shows how to use *FinQuant* to build a financial portfolio by
 downloading stock price data through the Python package `quandl`/`yfinance`.
 ### Building a portfolio with preset data `./example/Example-Build-Portfolio-
 from-file.py`: Shows how to use *FinQuant* to build a financial portfolio by
 providing stock price data yourself, e.g. by reading data from disk/file. ###
 Analysis of a portfolio `./example/Example-Analysis.py`: This example shows how
 to use an instance of `finquant.portfolio.Portfolio`, get the portfolio's
-quantities, such as - Expected Returns, - Volatility, - Sharpe Ratio, - Value
-at Risk. It also shows how to extract individual stocks from the given
-portfolio. Moreover it shows how to compute and visualise: - the different
-Returns provided by the module `finquant.returns`, - *Moving Averages*, a band
-of *Moving Averages*, and a *Bollinger Band*. ### Optimisation of a portfolio
-`./example/Example-Optimisation.py`: This example focusses on the optimisation
-of a portfolio. To achieve this, the example shows the usage of
+quantities, such as - Expected Returns, - Volatility, - Downside Risk, - Value
+at Risk, - Sharpe Ratio, - Sortino Ratio, - Beta parameter. It also shows how
+to extract individual stocks from the given portfolio. Moreover it shows how to
+compute and visualise: - the different Returns provided by the module
+`finquant.returns`, - *Moving Averages*, a band of *Moving Averages*, and a
+*Bollinger Band*. ### Optimisation of a portfolio `./example/Example-
+Optimisation.py`: This example focusses on the optimisation of a portfolio. To
+achieve this, the example shows the usage of
 `finquant.efficient_frontier.EfficientFrontier` for optimising the portfolio,
 for the - Minimum Volatility - Maximum Sharpe Ratio - Minimum Volatility for a
 given target Return - Maximum Sharpe Ratio for a given target Volatility.
 Furthermore, it is also shown how the entire *Efficient Frontier* and the
 optimal portfolios can be computed and visualised. If needed, it also gives an
 example of plotting the individual stocks of the given portfolio within the
 computed *Efficient Frontier*. Also, the optimisation of a portfolio and its
```

### Comparing `FinQuant-0.4.0/README.md` & `FinQuant-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </p>
 
 <p align="center">
   <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
     <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
   </a>
   <a href="https://pypi.org/project/FinQuant">
-    <img src="https://img.shields.io/badge/pypi-v0.4.0-brightgreen.svg?style=popout" alt='pypi'>
+    <img src="https://img.shields.io/badge/pypi-v0.5.0-brightgreen.svg?style=popout" alt='pypi'>
   </a>
   <a href="https://github.com/fmilthaler/FinQuant">
     <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
   </a>
   <a href="http://finquant.readthedocs.io/">
     <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
   </a>
@@ -245,16 +245,19 @@
 ### Building a portfolio with preset data
 `./example/Example-Build-Portfolio-from-file.py`: Shows how to use *FinQuant* to build a financial portfolio by providing stock price data yourself, e.g. by reading data from disk/file.
 
 ### Analysis of a portfolio
 `./example/Example-Analysis.py`: This example shows how to use an instance of `finquant.portfolio.Portfolio`, get the portfolio's quantities, such as
  - Expected Returns,
  - Volatility,
+ - Downside Risk,
+ - Value at Risk, 
  - Sharpe Ratio,
- - Value at Risk.
+ - Sortino Ratio,
+ - Beta parameter.
 
 It also shows how to extract individual stocks from the given portfolio. Moreover it shows how to compute and visualise:
  - the different Returns provided by the module `finquant.returns`,
  - *Moving Averages*, a band of *Moving Averages*, and a *Bollinger Band*.
 
 ### Optimisation of a portfolio
 `./example/Example-Optimisation.py`: This example focusses on the optimisation of a portfolio. To achieve this, the example shows the usage of `finquant.efficient_frontier.EfficientFrontier` for optimising the portfolio, for the
@@ -264,8 +267,7 @@
  - Maximum Sharpe Ratio for a given target Volatility.
 
 Furthermore, it is also shown how the entire *Efficient Frontier* and the optimal portfolios can be computed and visualised. If needed, it also gives an example of plotting the individual stocks of the given portfolio within the computed *Efficient Frontier*.
 
 Also, the optimisation of a portfolio and its visualisation based on a *Monte Carlo* is shown.
 
 Finally, *FinQuant*'s visualisation methods allow for overlays, if this is desired. Thus, with only the following few lines of code, one can create an overlay of the *Monte Carlo* run, the *Efficient Frontier*, its optimised portfolios for *Minimum Volatility* and *Maximum Sharpe Ratio*, as well as the portfolio's individual stocks.
-
```

#### html2text {}

```diff
@@ -136,21 +136,22 @@
 from-web.py`: Shows how to use *FinQuant* to build a financial portfolio by
 downloading stock price data through the Python package `quandl`/`yfinance`.
 ### Building a portfolio with preset data `./example/Example-Build-Portfolio-
 from-file.py`: Shows how to use *FinQuant* to build a financial portfolio by
 providing stock price data yourself, e.g. by reading data from disk/file. ###
 Analysis of a portfolio `./example/Example-Analysis.py`: This example shows how
 to use an instance of `finquant.portfolio.Portfolio`, get the portfolio's
-quantities, such as - Expected Returns, - Volatility, - Sharpe Ratio, - Value
-at Risk. It also shows how to extract individual stocks from the given
-portfolio. Moreover it shows how to compute and visualise: - the different
-Returns provided by the module `finquant.returns`, - *Moving Averages*, a band
-of *Moving Averages*, and a *Bollinger Band*. ### Optimisation of a portfolio
-`./example/Example-Optimisation.py`: This example focusses on the optimisation
-of a portfolio. To achieve this, the example shows the usage of
+quantities, such as - Expected Returns, - Volatility, - Downside Risk, - Value
+at Risk, - Sharpe Ratio, - Sortino Ratio, - Beta parameter. It also shows how
+to extract individual stocks from the given portfolio. Moreover it shows how to
+compute and visualise: - the different Returns provided by the module
+`finquant.returns`, - *Moving Averages*, a band of *Moving Averages*, and a
+*Bollinger Band*. ### Optimisation of a portfolio `./example/Example-
+Optimisation.py`: This example focusses on the optimisation of a portfolio. To
+achieve this, the example shows the usage of
 `finquant.efficient_frontier.EfficientFrontier` for optimising the portfolio,
 for the - Minimum Volatility - Maximum Sharpe Ratio - Minimum Volatility for a
 given target Return - Maximum Sharpe Ratio for a given target Volatility.
 Furthermore, it is also shown how the entire *Efficient Frontier* and the
 optimal portfolios can be computed and visualised. If needed, it also gives an
 example of plotting the individual stocks of the given portfolio within the
 computed *Efficient Frontier*. Also, the optimisation of a portfolio and its
```

### Comparing `FinQuant-0.4.0/finquant/asset.py` & `FinQuant-0.5.0/finquant/asset.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,17 @@
         - ``kurtosis`` (``float``): Kurtosis of the asset.
 
     The ``Asset`` class provides methods to compute various quantities such as expected return,
     volatility, skewness, and kurtosis based on the historical price data of the asset.
 
     """
 
-    def __init__(self, data: pd.Series, name: str, asset_type: str = 'Market index') -> None:
+    def __init__(
+        self, data: pd.Series, name: str, asset_type: str = "Market index"
+    ) -> None:
         """
         :Input:
          :data: ``pandas.Series``, of asset prices
          :name: ``str``, Name of the asset
          :asset_type: ``str`` (default: ``'Market index'``), Type of the asset (e.g., "Stock" or "Market index")
         """
         self.data = data
@@ -115,8 +117,8 @@
         string += f"\nKurtosis: {self.kurtosis:0.5f}"
         string += "\n" + "-" * 50
         print(string)
 
     def __str__(self):
         # print short description
         string = f"Contains information about {self.asset_type}: {self.name}."
-        return string
+        return string
```

### Comparing `FinQuant-0.4.0/finquant/efficient_frontier.py` & `FinQuant-0.5.0/finquant/efficient_frontier.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.4.0/finquant/market.py` & `FinQuant-0.5.0/finquant/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 common functionality and attributes for financial assets. It provides additional methods
 and attributes specific to market indices.
 
 """
 
 import numpy as np
 import pandas as pd
+
 from finquant.asset import Asset
 from finquant.returns import daily_returns, historical_mean_return
 
 
 class Market(Asset):
     """
     Class representing a market index.
@@ -39,8 +40,8 @@
         self.daily_returns = self.comp_daily_returns()
 
     # functions to compute quantities
     def comp_daily_returns(self) -> pd.Series:
         """Computes the daily returns (percentage change) of the market index.
         See ``finquant.returns.daily_returns``.
         """
-        return daily_returns(self.data)
+        return daily_returns(self.data)
```

### Comparing `FinQuant-0.4.0/finquant/minimise_fun.py` & `FinQuant-0.5.0/finquant/minimise_fun.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.4.0/finquant/monte_carlo.py` & `FinQuant-0.5.0/finquant/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.4.0/finquant/moving_average.py` & `FinQuant-0.5.0/finquant/moving_average.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.4.0/finquant/portfolio.py` & `FinQuant-0.5.0/finquant/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 and makes the most common quantitative calculations, such as:
 
 - cumulative returns of the portfolio's stocks
 - daily returns of the portfolio's stocks (daily percentage change),
 - daily log returns of the portfolio's stocks,
 - Expected (annualised) Return,
 - Volatility,
-- Sharpe Ratio,
+- Downside Risk,
 - Value at Risk,
+- Sharpe Ratio,
+- Sortino Ratio,
 - Beta parameter (optional),
 - skewness of the portfolio's stocks,
 - Kurtosis of the portfolio's stocks,
 - the portfolio's covariance matrix.
 
 Furthermore, the constructed portfolio can be optimised for
 
@@ -45,25 +47,32 @@
 - Portfolio with the minimum Volatility for a given Expected Return based
   on a numerical optimisation
 - Portfolio with the maximum Sharpe Ratio for a given target Volatility
   based on a numerical optimisation
 - Individual stocks of the portfolio (Expected Return over Volatility)
 """
 
-from typing import List
 import datetime
+from typing import List
 
 import matplotlib.pylab as plt
 import numpy as np
 import pandas as pd
 
 from finquant.efficient_frontier import EfficientFrontier
 from finquant.market import Market
 from finquant.monte_carlo import MonteCarloOpt
-from finquant.quants import sharpe_ratio, value_at_risk, weighted_mean, weighted_std
+from finquant.quants import (
+    downside_risk,
+    sharpe_ratio,
+    sortino_ratio,
+    value_at_risk,
+    weighted_mean,
+    weighted_std,
+)
 from finquant.returns import (
     cumulative_returns,
     daily_log_returns,
     daily_returns,
     historical_mean_return,
 )
 from finquant.stock import Stock
@@ -81,16 +90,18 @@
         """Initiates ``Portfolio``."""
         # initilisating instance variables
         self.portfolio = pd.DataFrame()
         self.stocks = {}
         self.data = pd.DataFrame()
         self.expected_return = None
         self.volatility = None
-        self.sharpe = None
+        self.downside_risk = None
         self.var = None
+        self.sharpe = None
+        self.sortino = None
         self.skew = None
         self.kurtosis = None
         self.totalinvestment = None
         self.var_confidence_level = 0.95
         self.risk_free_rate = 0.005
         self.freq = 252
         # instance variables for Efficient Frontier and
@@ -222,16 +233,18 @@
 
     def _update(self):
         # sanity check (only update values if none of the below is empty):
         if not (self.portfolio.empty or not self.stocks or self.data.empty):
             self.totalinvestment = self.portfolio.Allocation.sum()
             self.expected_return = self.comp_expected_return(freq=self.freq)
             self.volatility = self.comp_volatility(freq=self.freq)
-            self.sharpe = self.comp_sharpe()
+            self.downside_risk = self.comp_downside_risk(freq=self.freq)
             self.var = self.comp_var()
+            self.sharpe = self.comp_sharpe()
+            self.sortino = self.comp_sortino()
             self.skew = self._comp_skew()
             self.kurtosis = self._comp_kurtosis()
             if self.market_index is not None:
                 self.beta = self.comp_beta()
 
     def get_stock(self, name):
         """Returns the instance of ``Stock`` with name ``name``.
@@ -345,14 +358,30 @@
         if not isinstance(freq, int):
             raise ValueError("freq is expected to be an integer.")
         # computing the volatility of a portfolio
         volatility = weighted_std(self.comp_cov(), self.comp_weights()) * np.sqrt(freq)
         self.volatility = volatility
         return volatility
 
+    def comp_downside_risk(self, freq=252):
+        """Computes the downside risk of the portfolio.
+
+        :Input:
+         :freq: ``int`` (default: ``252``), number of trading days, default
+             value corresponds to trading days in a year
+
+        :Output:
+         :downside risk: ``float`` downside risk of the portfolio.
+        """
+        downs_risk = downside_risk(
+            self.data, self.comp_weights(), self.risk_free_rate
+        ) * np.sqrt(freq)
+        self.downside_risk = downs_risk
+        return downs_risk
+
     def comp_cov(self):
         """Compute and return a ``pandas.DataFrame`` of the covariance matrix
         of the portfolio.
 
         :Output:
          :cov: a ``pandas.DataFrame`` of the covariance matrix of the portfolio.
         """
@@ -399,14 +428,25 @@
         # compute the Beta parameter of the portfolio
         weights = self.comp_weights()
         beta = weighted_mean(self.beta_stocks.transpose()["beta"].values, weights)
 
         self.beta = beta
         return beta
 
+    def comp_sortino(self, freq=252):
+        """Compute and return the Sortino Ratio of the portfolio
+
+        :Output:
+         :sortino: ``float``, the Sortino Ratio of the portfolio
+         May be NaN if the portoflio outperformed the risk free rate at every point
+        """
+        return sortino_ratio(
+            self.expected_return, self.downside_risk, self.risk_free_rate
+        )
+
     def _comp_skew(self):
         """Computes and returns the skewness of the stocks in the portfolio."""
         return self.data.skew()
 
     def _comp_kurtosis(self):
         """Computes and returns the Kurtosis of the stocks in the portfolio."""
         return self.data.kurt()
@@ -660,16 +700,19 @@
             )
 
     def properties(self):
         """Nicely prints out the properties of the portfolio:
 
         - Expected Return,
         - Volatility,
+        - Downside Risk,
+        - Value at Risk (VaR),
+        - Confidence level of VaR,
         - Sharpe Ratio,
-        - Value at Risk,
+        - Sortino Ratio,
         - Beta (optional),
         - skewness,
         - Kurtosis
 
         as well as the allocation of the stocks across the portfolio.
         """
         # nicely printing out information and quantities of the portfolio
@@ -678,18 +721,20 @@
         string += f"\nStocks: {', '.join(stocknames)}"
         if self.market_index is not None:
             string += f"\nMarket Index: {self.market_index.name}"
         string += f"\nTime window/frequency: {self.freq}"
         string += f"\nRisk free rate: {self.risk_free_rate}"
         string += f"\nPortfolio Expected Return: {self.expected_return:0.3f}"
         string += f"\nPortfolio Volatility: {self.volatility:0.3f}"
-        string += f"\nPortfolio Sharpe Ratio: {self.sharpe:0.3f}"
+        string += f"\nPortfolio Downside Risk: {self.downside_risk:0.3f}"
         string += f"\nPortfolio Value at Risk: {self.var:0.3f}"
         string += f"\nConfidence level of Value at Risk: "
         string += f"{self.var_confidence_level * 100:0.2f} %"
+        string += f"\nPortfolio Sharpe Ratio: {self.sharpe:0.3f}"
+        string += f"\nPortfolio Sortino Ratio: {self.sortino:0.3f}"
         if self.beta is not None:
             string += f"\nPortfolio Beta: {self.beta:0.3f}"
         string += "\n\nSkewness:"
         string += "\n" + str(self.skew.to_frame().transpose())
         string += "\n\nKurtosis:"
         string += "\n" + str(self.kurtosis.to_frame().transpose())
         string += "\n\nInformation:"
@@ -1210,15 +1255,17 @@
     # pylint: disable=R0916
     if (
         pf.portfolio.empty
         or pf.data.empty
         or not pf.stocks
         or pf.expected_return is None
         or pf.volatility is None
+        or pf.downside_risk is None
         or pf.sharpe is None
+        or pf.sortino is None
         or pf.skew is None
         or pf.kurtosis is None
     ):
         raise ValueError(
             "Should not get here. Something went wrong while "
             + "creating an instance of Portfolio."
             + docstring_msg
```

### Comparing `FinQuant-0.4.0/finquant/quants.py` & `FinQuant-0.5.0/finquant/quants.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 """
 
 
 import numpy as np
 import pandas as pd
 from scipy.stats import norm
 
+from finquant.returns import weighted_mean_daily_returns
+
 
 def weighted_mean(means, weights):
     """Computes the weighted mean/average, or in the case of a
     financial portfolio, it can be used for the Expected Return
     of said portfolio.
 
     :Input:
@@ -71,14 +73,68 @@
     if not isinstance(
         risk_free_rate, (int, float, np.int32, np.int64, np.float32, np.float64)
     ):
         raise ValueError("risk_free_rate is expected to be an integer or float.")
     return (exp_return - risk_free_rate) / float(volatility)
 
 
+def sortino_ratio(exp_return, downside_risk, risk_free_rate=0.005):
+    """Computes the Sortino Ratio
+
+    :Input:
+     :exp_return: ``int``/``float``, Expected Return of a portfolio
+     :downside_risk: ``int``/``float``, Downside Risk of a portfolio
+     :risk_free_rate: ``int``/``float`` (default= ``0.005``), risk free rate
+
+    :Output:
+     :sortino ratio: ``float``/``NaN`` ``(exp_return - risk_free_rate)/float(downside_risk)``.
+     Can be ``NaN`` if ``downside_risk`` is zero
+    """
+    if not isinstance(
+        exp_return, (int, float, np.int32, np.int64, np.float32, np.float64)
+    ):
+        raise ValueError("exp_return is expected to be an integer or float.")
+    if not isinstance(
+        downside_risk, (int, float, np.int32, np.int64, np.float32, np.float64)
+    ):
+        raise ValueError("volatility is expected to be an integer or float.")
+    if not isinstance(
+        risk_free_rate, (int, float, np.int32, np.int64, np.float32, np.float64)
+    ):
+        raise ValueError("risk_free_rate is expected to be an integer or float.")
+    if float(downside_risk) == 0:
+        return np.nan
+    else:
+        return (exp_return - risk_free_rate) / float(downside_risk)
+
+
+def downside_risk(data: pd.DataFrame, weights, risk_free_rate=0.005) -> float:
+    """Computes the downside risk (target downside deviation of returns).
+
+    :Input:
+      :data: ``pandas.DataFrame`` with daily stock prices
+      :weights: ``numpy.ndarray``/``pd.Series`` of weights
+      :risk_free_rate: ``int``/``float`` (default=``0.005``), risk free rate
+
+    :Output:
+      :downside_risk: ``float``, target downside deviation
+    """
+    if not isinstance(data, pd.DataFrame):
+        raise ValueError("data is expected to be a Pandas.DataFrame.")
+    if not isinstance(weights, (pd.Series, np.ndarray)):
+        raise ValueError("weights is expected to be a pandas.Series/np.ndarray.")
+    if not isinstance(
+        risk_free_rate, (int, float, np.int32, np.int64, np.float32, np.float64)
+    ):
+        raise ValueError("risk_free_rate is expected to be an integer or float.")
+
+    wtd_daily_mean = weighted_mean_daily_returns(data, weights)
+    return np.sqrt(np.mean(np.minimum(0, wtd_daily_mean - risk_free_rate) ** 2))
+
+
 def value_at_risk(investment, mu, sigma, conf_level=0.95) -> float:
     """Computes and returns the expected value at risk of an investment/assets.
 
     :Input:
      :investment: ``float``/``int``, total value of the investment
      :mu: ``float``/``int`` average/mean return of the investment
      :sigma: ``float``/``int`` standard deviation of the investment
```

### Comparing `FinQuant-0.4.0/finquant/returns.py` & `FinQuant-0.5.0/finquant/returns.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,27 @@
     :Output:
      :ret: a ``pandas.DataFrame`` of daily percentage change of Returns
          of given stock prices.
     """
     return data.pct_change().dropna(how="all").replace([np.inf, -np.inf], np.nan)
 
 
+def weighted_mean_daily_returns(data, weights):
+    """Returns DataFrame with the daily weighted mean returns
+
+    :Input:
+      :data: ``pandas.DataFrame`` with daily stock prices
+      :weights: ``numpy.ndarray``/``pd.Series`` of weights
+
+    :Output:
+      :ret: ``numpy.array`` of weighted mean daily percentage change of Returns
+    """
+    return np.dot(daily_returns(data), weights)
+
+
 def daily_log_returns(data):
     """
     Returns DataFrame with daily log returns
 
     :math:`R_{\\log} = \\log\\left(1 + \\dfrac{\\text{price}_{t_i} - \\text{price}_{t_{i-1}}}
     {\\text{price}_{t_{i-1}}}\\right)`
```

### Comparing `FinQuant-0.4.0/finquant/stock.py` & `FinQuant-0.5.0/finquant/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 The ``Stock`` class inherits from the ``Asset`` class in ``finquant.asset``, which provides common
 functionality and attributes for financial assets.
 
 """
 
 import numpy as np
 import pandas as pd
+
 from finquant.asset import Asset
 from finquant.returns import daily_returns, historical_mean_return
 
 
 class Stock(Asset):
     """Class that contains information about a stock/fund.
```

### Comparing `FinQuant-0.4.0/setup.py` & `FinQuant-0.5.0/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 def read_requirements(file_path):
     return [line.strip() for line in read_file(file_path).splitlines() if line.strip()]
 
 
 install_requires = read_requirements("requirements.txt")
 
 extras_require = {
-    "test": read_requirements("requirements_test.txt"),
+    "cd": read_requirements("requirements_cd.txt"),
     "dev": read_requirements("requirements_dev.txt"),
     "docs": read_requirements("requirements_docs.txt"),
-    "cd": read_requirements("requirements_cd.txt"),
+    "test": read_requirements("requirements_test.txt"),
 }
 
 setuptools.setup(
     name="FinQuant",
     version=version["version"],
     author="Frank Milthaler",
     author_email="f.milthaler@gmail.com",
```

### Comparing `FinQuant-0.4.0/tests/test_market.py` & `FinQuant-0.5.0/tests/test_market.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.4.0/tests/test_moving_average.py` & `FinQuant-0.5.0/tests/test_moving_average.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.4.0/tests/test_portfolio.py` & `FinQuant-0.5.0/tests/test_portfolio.py`

 * *Files identical despite different names*

```diff
@@ -1,11 +1,12 @@
 ###############################################################
 # testing modules portfolio, optimisation, efficient_frontier #
 # all through the interfaces in Portfolio                     #
 ###############################################################
+
 import datetime
 import os
 import pathlib
 
 import matplotlib.pylab as plt
 import numpy as np
 import pandas as pd
```

### Comparing `FinQuant-0.4.0/tests/test_quants.py` & `FinQuant-0.5.0/tests/test_quants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+import pdb
+
 import numpy as np
+import pandas as pd
 import pytest
 
 from finquant.quants import (
     annualised_portfolio_quantities,
+    downside_risk,
     sharpe_ratio,
+    sortino_ratio,
     value_at_risk,
     weighted_mean,
     weighted_std,
 )
 
 
 def test_weighted_mean():
@@ -30,14 +35,19 @@
 
 
 def test_sharpe_ratio():
     assert sharpe_ratio(0.5, 0.2, 0.02) == 2.4
     assert sharpe_ratio(0.5, 0.22, 0.005) == 2.25
 
 
+def test_sortino_ratio():
+    assert sortino_ratio(0.5, 0.0, 0.02) is np.NaN
+    assert sortino_ratio(0.005, 8.5, 0.005) == 0.0
+
+
 def test_value_at_risk():
     assert abs(value_at_risk(1e2, 0.5, 0.25, 0.95) - 91.12) <= 1e-1
     assert abs(value_at_risk(1e3, 0.8, 0.5, 0.99) - 1963.17) <= 1e-1
     assert abs(value_at_risk(1e4, -0.1, 0.25, 0.9) - 2203.88) <= 1e-1
     assert abs(value_at_risk(1e4, 0.1, -0.25, 0.9) - (-2203.88)) <= 1e-1
     assert abs(value_at_risk(1e4, -0.1, -0.25, 0.9) - (-4203.88)) <= 1e-1
     assert value_at_risk(0, 0.1, 0.5, 0.9) == 0
@@ -73,7 +83,21 @@
     weights = np.array([1, 1])
     mean = np.array([1, 2])
     weights = np.array([-3, 5])
     res = annualised_portfolio_quantities(weights, mean, Sigma, 0, 252)
     orig = (1764, 347.79304190854657, 5.071981861166303)
     for i in range(len(res)):
         assert abs(res[i] - orig[i]) <= 1e-15
+
+
+def test_downside_risk():
+    data1 = pd.DataFrame({"1": [1, 2, 4, 8], "2": [1, 2, 3, 4]})
+    weights = np.array([0.25, 0.75])
+    rf_rate = 0.005
+    dr1 = downside_risk(data1, weights, rf_rate)
+    assert dr1 == 0
+
+    data2 = pd.DataFrame({"1": [7, 6, 5, 4, 3]})
+    weights = np.array([1])
+    rf_rate = 0.0
+    dr2 = downside_risk(data2, weights, rf_rate)
+    assert abs(dr2 - 0.19409143531019335) <= 1e-15
```

### Comparing `FinQuant-0.4.0/tests/test_returns.py` & `FinQuant-0.5.0/tests/test_returns.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import numpy as np
 import pandas as pd
 
 from finquant.returns import (
     cumulative_returns,
     daily_log_returns,
     daily_returns,
     historical_mean_return,
+    weighted_mean_daily_returns,
 )
 
 
 def test_cumulative_returns():
     orig = [
         list(range(10)),
         [0, -0.025, -0.05, -0.075, -0.1, -0.125, -0.15, -0.175, -0.2, -0.225],
@@ -37,14 +39,31 @@
     d = {"1": l1, "2": l2}
     df = pd.DataFrame(d)
     ret = daily_returns(df)
     assert all(abs(ret["1"].values - orig[0]) <= 1e-15)
     assert all(abs(ret["2"].values - orig[1]) <= 1e-15)
 
 
+def test_weighted_daily_mean_returns():
+    l1 = [1.0, 1.5, 2.25, 3.375]
+    l2 = [1.0, 2.0, 4.0, 8.0]
+    expected = [0.5 * 0.25 + 1 * 0.75 for i in range(len(l1) - 1)]
+    weights = np.array([0.25, 0.75])
+    d = {"1": l1, "2": l2}
+    df = pd.DataFrame(d)
+    ret = weighted_mean_daily_returns(df, weights)
+    assert all(abs(ret - expected) <= 1e-15)
+
+    d = {"1": l1}
+    expected = [0.5 for i in range(len(l1) - 1)]
+    df = pd.DataFrame(d)
+    ret = weighted_mean_daily_returns(df, np.array([1]))
+    assert all(abs(ret - expected) <= 1e-15)
+
+
 def test_daily_log_returns():
     orig = [
         [
             0.6931471805599453,
             0.4054651081081644,
             0.28768207245178085,
             0.22314355131420976,
```

### Comparing `FinQuant-0.4.0/tests/test_stock.py` & `FinQuant-0.5.0/tests/test_stock.py`

 * *Files identical despite different names*

