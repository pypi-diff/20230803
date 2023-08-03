# Comparing `tmp/anatomy-0.1.4.tar.gz` & `tmp/anatomy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anatomy-0.1.4.tar", last modified: Thu Nov 17 12:15:47 2022, max compression
+gzip compressed data, was "anatomy-0.1.5.tar", last modified: Thu Aug  3 16:20:38 2023, max compression
```

## Comparing `anatomy-0.1.4.tar` & `anatomy-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-11-17 12:15:47.739758 anatomy-0.1.4/
--rw-rw-rw-   0        0        0     1090 2022-09-19 09:37:38.000000 anatomy-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    18408 2022-11-17 12:15:47.738755 anatomy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    17655 2022-11-17 12:13:12.000000 anatomy-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2022-11-17 12:15:47.732756 anatomy-0.1.4/anatomy/
--rw-rw-rw-   0        0        0      494 2022-11-17 12:08:21.000000 anatomy-0.1.4/anatomy/__init__.py
--rw-rw-rw-   0        0        0     4696 2022-09-27 13:04:11.000000 anatomy-0.1.4/anatomy/_algorithm.py
--rw-rw-rw-   0        0        0    11761 2022-10-05 11:58:24.000000 anatomy-0.1.4/anatomy/_base.py
--rw-rw-rw-   0        0        0     2975 2022-09-19 14:29:22.000000 anatomy-0.1.4/anatomy/_models.py
--rw-rw-rw-   0        0        0     2670 2022-10-19 10:06:08.000000 anatomy-0.1.4/anatomy/_subsets.py
-drwxrwxrwx   0        0        0        0 2022-11-17 12:15:47.737754 anatomy-0.1.4/anatomy.egg-info/
--rw-rw-rw-   0        0        0    18408 2022-11-17 12:15:47.000000 anatomy-0.1.4/anatomy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2022-11-17 12:15:47.000000 anatomy-0.1.4/anatomy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-17 12:15:47.000000 anatomy-0.1.4/anatomy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2022-11-17 12:15:47.000000 anatomy-0.1.4/anatomy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-11-17 12:15:47.000000 anatomy-0.1.4/anatomy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-17 12:15:47.739758 anatomy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      669 2022-11-17 12:08:13.000000 anatomy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:20:38.448448 anatomy-0.1.5/
+-rw-rw-rw-   0        0        0     1090 2023-08-03 16:15:29.000000 anatomy-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0    19976 2023-08-03 16:20:38.443358 anatomy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    19199 2023-08-03 16:13:40.000000 anatomy-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 16:20:38.442321 anatomy-0.1.5/anatomy/
+-rw-rw-rw-   0        0        0      517 2023-08-03 16:15:42.000000 anatomy-0.1.5/anatomy/__init__.py
+-rw-rw-rw-   0        0        0     4696 2022-09-27 13:04:11.000000 anatomy-0.1.5/anatomy/_algorithm.py
+-rw-rw-rw-   0        0        0    11761 2022-10-05 11:58:24.000000 anatomy-0.1.5/anatomy/_base.py
+-rw-rw-rw-   0        0        0     4419 2023-08-03 15:34:43.000000 anatomy-0.1.5/anatomy/_mas.py
+-rw-rw-rw-   0        0        0     3041 2023-02-02 15:07:34.000000 anatomy-0.1.5/anatomy/_models.py
+-rw-rw-rw-   0        0        0     2670 2022-10-19 10:06:08.000000 anatomy-0.1.5/anatomy/_subsets.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:20:38.443358 anatomy-0.1.5/anatomy.egg-info/
+-rw-rw-rw-   0        0        0    19976 2023-08-03 16:20:38.000000 anatomy-0.1.5/anatomy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-08-03 16:20:38.000000 anatomy-0.1.5/anatomy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 16:20:38.000000 anatomy-0.1.5/anatomy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-03 16:20:38.000000 anatomy-0.1.5/anatomy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-03 16:20:38.000000 anatomy-0.1.5/anatomy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 16:20:38.448448 anatomy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-08-03 10:00:07.000000 anatomy-0.1.5/setup.py
```

### Comparing `anatomy-0.1.4/LICENSE` & `anatomy-0.1.5/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 The MIT License (MIT)
 
-Copyright 2022 Sander Schwenk-Nebbe
+Copyright 2023 Sander Schwenk-Nebbe
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `anatomy-0.1.4/PKG-INFO` & `anatomy-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: anatomy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Shapley-based decomposition to anatomize the of out-of-sample accuracy of time-series forecasting models
 Home-page: https://github.com/sander-sn/anatomy
 Author: Sander Schwenk-Nebbe
 Author-email: sandersn@econ.au.dk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Introduction
 
-This package implements the $\text{oShapley-VI}_p$ (out-of-sample Shapley-based variable importance) and $\text{PBSV}_p$ (performance-based Shapley value) proposed in the "The Anatomy of Out-of-Sample Forecasting Accuracy" paper by Daniel Borup, Philippe Goulet Coulombe, David E. Rapach, Erik Christian Montes Schütte, and Sander Schwenk-Nebbe, which is available to download for free at SSRN: [https://ssrn.com/abstract=4278745](https://ssrn.com/abstract=4278745).
+This package implements the $\text{oShapley-VI}_p$ (out-of-sample Shapley-based variable importance), $\text{PBSV}_p$ (performance-based Shapley value), MAS (model accordance score) and MAS hypothesis testing, proposed in the "The Anatomy of Out-of-Sample Forecasting Accuracy" paper by Daniel Borup, Philippe Goulet Coulombe, David E. Rapach, Erik Christian Montes Schütte, and Sander Schwenk-Nebbe, which is available to download for free at SSRN: [https://ssrn.com/abstract=4278745](https://ssrn.com/abstract=4278745).
 
-The $\text{PBSV}_p$ is a Shapley-based decomposition that measures the contributions of an individual predictor $p$ in fitted models to the out-of-sample loss.
+The $\text{PBSV}_p$ is a Shapley-based decomposition that measures the contributions of an individual predictor $p$ in fitted models to the out-of-sample loss. While a performance metric like the RMSE focuses solely on out-of-sample performance, MAS evaluates whether a model's out-of-sample success mirrors what it has learned from the in-sample data by comparing $\text{iShapley-VI}_p$ (or $\text{oShapley-VI}_p$) to $\text{PBSV}_p$. The MAS paired with a performance metric such as the RMSE provides insight into the model's "intentional success" (see [below example](#model-accordance-score)).
 
 The interpretation of PBSVs is straightforward: if $\text{PBSV}_p$ is negative (positive), predictor $p$ reduces (increases) the loss and is thus beneficial for (detrimental to) forecasting accuracy in the out-of-sample period. Taking the sum of the individual contributions (including the contribution of the empty set) yields the decomposed loss exactly (due to the efficiency property of Shapley values; see [below example](#the-efficiency-property)).
 
 Please cite our paper if you find the package useful:
 
     Borup, Daniel and Coulombe, Philippe Goulet and Rapach, David E. and Montes Schütte, Erik Christian and Schwenk-Nebbe, Sander (2022). “The Anatomy of Out-of-Sample Forecasting Accuracy”. Federal Reserve Bank of Atlanta Working Paper 2022-16. https://doi.org/10.29338/wp2022-16.
 
@@ -258,24 +258,24 @@
 ## ... the RMSE of the forecasts in a subperiod:
 
     subset = pd.date_range("2021-07-28", "2021-08-06").map(lambda x: x.date())
     	    
     def transform(y_hat, y):  
         return np.sqrt(np.mean((y - y_hat) ** 2))  
         
-    df = anatomy.explain(  
+    df_pbsv_rmse = anatomy.explain(  
         model_sets=AnatomyModelCombination(groups=groups),  
         transformer=AnatomyModelOutputTransformer(transform=transform),  
         explanation_subset=subset 
     )
 
 which yields the change in root mean squared error in the ten-day period attributable to each predictor:
 
 ```
->>> df
+>>> df_pbsv_rmse
                                  base_contribution       x_0       x_1       x_2
 rf     2021-07-28 -> 2021-08-06           1.402950 -0.149847 -0.199615  0.118059
 ols    2021-07-28 -> 2021-08-06           1.404761 -0.155275 -0.323760  0.317055
 ols+rf 2021-07-28 -> 2021-08-06           1.403853 -0.169584 -0.275408  0.211672
 ```
 
 ### _Interpretation_
@@ -284,41 +284,65 @@
 
 
 ## ... or just the raw forecasts:
 
     def transform(y_hat):
         return y_hat
         
-    df = anatomy.explain(
+    df_oshapley = anatomy.explain(
         model_sets=AnatomyModelCombination(groups=groups),
         transformer=AnatomyModelOutputTransformer(transform=transform)
     )
 
 which yields the change in the forecast attributable to each predictor:
 
-    >>> df
+    >>> df_oshapley
                        base_contribution       x_0       x_1       x_2
     rf     2021-07-28           0.070861  0.222932  0.360182 -0.315820
            2021-07-29           0.070354  0.250389 -0.617779  0.984992
            2021-07-30           0.071163 -1.514547  0.839562 -0.835136
     ...                              ...       ...       ...       ...
 
 ### *Interpretation*
 
 Decomposing the forecasts themselves yields contributions that bear no relation to forecasting accuracy. Hence, a negative or positive contribution means no more than a decrease or increase in the forecast at that period attributable to the given predictor, which may or may not have be good for forecasting accuracy.
 
 ***Hence: beware, a high average absolute contribution does not necessarily translate into a high gain in accuracy. That is precisely why we need to decompose the loss directly, and in consequence, take into account our target and how far away our forecasts were from it.***
 
-From the anatomized raw forecasts, we can compute the  $\text{oShapley-VI}$ by averaging over the magnitudes of the invididual contributions:
+From the anatomized raw forecasts, we can compute the $\text{oShapley-VI}$ by averaging over the magnitudes of the invididual contributions (here for the ``ols+rf`` combination):
+
+    >>> df_oshapley.loc["ols+rf"].abs().mean(axis=0)
+    base_contribution    0.078415
+    x_0                  0.864057
+    x_1                  0.786044
+    x_2                  0.770115
+
+## Model Accordance Score:
+
+We can compute the MAS for our combination model (``ols+rf``) using $\text{oShapley-VI}$ and, for instance, the $\text{PBSV(RMSE)}_p$:
+
+    vi = df_oshapley.loc["ols+rf"].abs().mean(axis=0).drop("base_contribution")
+    pbsv = df_pbsv_rmse.loc["ols+rf"].iloc[0].drop("base_contribution")
+
+    h0 = MAS.H0(p=vi.shape[0])               # generate mas(p) under the null
+    loss_type = MAS.LossType.LOWER_IS_BETTER # rmse => lower is better
+
+    mas = MAS(vi, pbsv, loss_type, h0).compute()
+
+which yields the MAS:
+
+    >>> mas
+    {'mas': 1.0, 'mas_p_val': 0.0}
+
+### *Interpretation*
+
+In this example, the ranking of $\text{oShapley-VI}$ is identical to the signed-ranking of $\text{PBSV(RMSE)}_p$.
+Thus, MAS is 1 (perfect) and the null hypothesis of no relation between $\text{oShapley-VI}$ and $\text{PBSV(RMSE)}_p$ is rejected
+(``mas_p_val`` is the probability of observing a MAS lower or equal to ``mas`` under the null).
 
-    >>> df.abs().mean(axis=0)
-    base_contribution    0.078436
-    x_0                  0.865098
-    x_1                  0.787327
-    x_2                  0.773340
 
 ## The Efficiency property
 
 *During estimation, the `Anatomy` checks that the individual attributions of the predictors to the forecasts sum up exactly to the forecasts produced by the models. The estimation would be aborted if efficiency does not hold.*
 
 Due to the efficiency property of Shapley values, summing the individual contributions yields the decomposed value exactly. We can check that the results that `Anatomy` yields are consistet. We can recover the RMSE from the decomposed RMSE, but we can also recover the RMSE from the decomposed forecasts. Let's make sure that they match.
```

### Comparing `anatomy-0.1.4/README.md` & `anatomy-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # Introduction
 
-This package implements the $\text{oShapley-VI}_p$ (out-of-sample Shapley-based variable importance) and $\text{PBSV}_p$ (performance-based Shapley value) proposed in the "The Anatomy of Out-of-Sample Forecasting Accuracy" paper by Daniel Borup, Philippe Goulet Coulombe, David E. Rapach, Erik Christian Montes Schütte, and Sander Schwenk-Nebbe, which is available to download for free at SSRN: [https://ssrn.com/abstract=4278745](https://ssrn.com/abstract=4278745).
+This package implements the $\text{oShapley-VI}_p$ (out-of-sample Shapley-based variable importance), $\text{PBSV}_p$ (performance-based Shapley value), MAS (model accordance score) and MAS hypothesis testing, proposed in the "The Anatomy of Out-of-Sample Forecasting Accuracy" paper by Daniel Borup, Philippe Goulet Coulombe, David E. Rapach, Erik Christian Montes Schütte, and Sander Schwenk-Nebbe, which is available to download for free at SSRN: [https://ssrn.com/abstract=4278745](https://ssrn.com/abstract=4278745).
 
-The $\text{PBSV}_p$ is a Shapley-based decomposition that measures the contributions of an individual predictor $p$ in fitted models to the out-of-sample loss.
+The $\text{PBSV}_p$ is a Shapley-based decomposition that measures the contributions of an individual predictor $p$ in fitted models to the out-of-sample loss. While a performance metric like the RMSE focuses solely on out-of-sample performance, MAS evaluates whether a model's out-of-sample success mirrors what it has learned from the in-sample data by comparing $\text{iShapley-VI}_p$ (or $\text{oShapley-VI}_p$) to $\text{PBSV}_p$. The MAS paired with a performance metric such as the RMSE provides insight into the model's "intentional success" (see [below example](#model-accordance-score)).
 
 The interpretation of PBSVs is straightforward: if $\text{PBSV}_p$ is negative (positive), predictor $p$ reduces (increases) the loss and is thus beneficial for (detrimental to) forecasting accuracy in the out-of-sample period. Taking the sum of the individual contributions (including the contribution of the empty set) yields the decomposed loss exactly (due to the efficiency property of Shapley values; see [below example](#the-efficiency-property)).
 
 Please cite our paper if you find the package useful:
 
     Borup, Daniel and Coulombe, Philippe Goulet and Rapach, David E. and Montes Schütte, Erik Christian and Schwenk-Nebbe, Sander (2022). “The Anatomy of Out-of-Sample Forecasting Accuracy”. Federal Reserve Bank of Atlanta Working Paper 2022-16. https://doi.org/10.29338/wp2022-16.
 
@@ -246,24 +246,24 @@
 ## ... the RMSE of the forecasts in a subperiod:
 
     subset = pd.date_range("2021-07-28", "2021-08-06").map(lambda x: x.date())
     	    
     def transform(y_hat, y):  
         return np.sqrt(np.mean((y - y_hat) ** 2))  
         
-    df = anatomy.explain(  
+    df_pbsv_rmse = anatomy.explain(  
         model_sets=AnatomyModelCombination(groups=groups),  
         transformer=AnatomyModelOutputTransformer(transform=transform),  
         explanation_subset=subset 
     )
 
 which yields the change in root mean squared error in the ten-day period attributable to each predictor:
 
 ```
->>> df
+>>> df_pbsv_rmse
                                  base_contribution       x_0       x_1       x_2
 rf     2021-07-28 -> 2021-08-06           1.402950 -0.149847 -0.199615  0.118059
 ols    2021-07-28 -> 2021-08-06           1.404761 -0.155275 -0.323760  0.317055
 ols+rf 2021-07-28 -> 2021-08-06           1.403853 -0.169584 -0.275408  0.211672
 ```
 
 ### _Interpretation_
@@ -272,41 +272,65 @@
 
 
 ## ... or just the raw forecasts:
 
     def transform(y_hat):
         return y_hat
         
-    df = anatomy.explain(
+    df_oshapley = anatomy.explain(
         model_sets=AnatomyModelCombination(groups=groups),
         transformer=AnatomyModelOutputTransformer(transform=transform)
     )
 
 which yields the change in the forecast attributable to each predictor:
 
-    >>> df
+    >>> df_oshapley
                        base_contribution       x_0       x_1       x_2
     rf     2021-07-28           0.070861  0.222932  0.360182 -0.315820
            2021-07-29           0.070354  0.250389 -0.617779  0.984992
            2021-07-30           0.071163 -1.514547  0.839562 -0.835136
     ...                              ...       ...       ...       ...
 
 ### *Interpretation*
 
 Decomposing the forecasts themselves yields contributions that bear no relation to forecasting accuracy. Hence, a negative or positive contribution means no more than a decrease or increase in the forecast at that period attributable to the given predictor, which may or may not have be good for forecasting accuracy.
 
 ***Hence: beware, a high average absolute contribution does not necessarily translate into a high gain in accuracy. That is precisely why we need to decompose the loss directly, and in consequence, take into account our target and how far away our forecasts were from it.***
 
-From the anatomized raw forecasts, we can compute the  $\text{oShapley-VI}$ by averaging over the magnitudes of the invididual contributions:
+From the anatomized raw forecasts, we can compute the $\text{oShapley-VI}$ by averaging over the magnitudes of the invididual contributions (here for the ``ols+rf`` combination):
+
+    >>> df_oshapley.loc["ols+rf"].abs().mean(axis=0)
+    base_contribution    0.078415
+    x_0                  0.864057
+    x_1                  0.786044
+    x_2                  0.770115
+
+## Model Accordance Score:
+
+We can compute the MAS for our combination model (``ols+rf``) using $\text{oShapley-VI}$ and, for instance, the $\text{PBSV(RMSE)}_p$:
+
+    vi = df_oshapley.loc["ols+rf"].abs().mean(axis=0).drop("base_contribution")
+    pbsv = df_pbsv_rmse.loc["ols+rf"].iloc[0].drop("base_contribution")
+
+    h0 = MAS.H0(p=vi.shape[0])               # generate mas(p) under the null
+    loss_type = MAS.LossType.LOWER_IS_BETTER # rmse => lower is better
+
+    mas = MAS(vi, pbsv, loss_type, h0).compute()
+
+which yields the MAS:
+
+    >>> mas
+    {'mas': 1.0, 'mas_p_val': 0.0}
+
+### *Interpretation*
+
+In this example, the ranking of $\text{oShapley-VI}$ is identical to the signed-ranking of $\text{PBSV(RMSE)}_p$.
+Thus, MAS is 1 (perfect) and the null hypothesis of no relation between $\text{oShapley-VI}$ and $\text{PBSV(RMSE)}_p$ is rejected
+(``mas_p_val`` is the probability of observing a MAS lower or equal to ``mas`` under the null).
 
-    >>> df.abs().mean(axis=0)
-    base_contribution    0.078436
-    x_0                  0.865098
-    x_1                  0.787327
-    x_2                  0.773340
 
 ## The Efficiency property
 
 *During estimation, the `Anatomy` checks that the individual attributions of the predictors to the forecasts sum up exactly to the forecasts produced by the models. The estimation would be aborted if efficiency does not hold.*
 
 Due to the efficiency property of Shapley values, summing the individual contributions yields the decomposed value exactly. We can check that the results that `Anatomy` yields are consistet. We can recover the RMSE from the decomposed RMSE, but we can also recover the RMSE from the decomposed forecasts. Let's make sure that they match.
```

### Comparing `anatomy-0.1.4/anatomy/_algorithm.py` & `anatomy-0.1.5/anatomy/_algorithm.py`

 * *Files identical despite different names*

### Comparing `anatomy-0.1.4/anatomy/_base.py` & `anatomy-0.1.5/anatomy/_base.py`

 * *Files identical despite different names*

### Comparing `anatomy-0.1.4/anatomy/_models.py` & `anatomy-0.1.5/anatomy/_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,10 +77,10 @@
         transform: Union[Callable[[np.ndarray], np.ndarray], Callable[[np.ndarray, np.ndarray], np.ndarray]]
     ):
         """
         :param transform: function used to transform model output; must have named argument y_hat (contains
          raw model output) and can optionally use named argumeny y (contains true target);
          let transformer return aggregated result instead of series to get an aggregated (global) explanation
         """
-        assert "y_hat" in transform.__code__.co_varnames
-        assert all([x in ["y_hat", "y"] for x in transform.__code__.co_varnames])
+        assert "y_hat" in transform.__code__.co_varnames[:transform.__code__.co_argcount]
+        assert all([x in ["y_hat", "y"] for x in transform.__code__.co_varnames[:transform.__code__.co_argcount]])
         self.transform = transform
```

### Comparing `anatomy-0.1.4/anatomy/_subsets.py` & `anatomy-0.1.5/anatomy/_subsets.py`

 * *Files identical despite different names*

### Comparing `anatomy-0.1.4/anatomy.egg-info/PKG-INFO` & `anatomy-0.1.5/anatomy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: anatomy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Shapley-based decomposition to anatomize the of out-of-sample accuracy of time-series forecasting models
 Home-page: https://github.com/sander-sn/anatomy
 Author: Sander Schwenk-Nebbe
 Author-email: sandersn@econ.au.dk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Introduction
 
-This package implements the $\text{oShapley-VI}_p$ (out-of-sample Shapley-based variable importance) and $\text{PBSV}_p$ (performance-based Shapley value) proposed in the "The Anatomy of Out-of-Sample Forecasting Accuracy" paper by Daniel Borup, Philippe Goulet Coulombe, David E. Rapach, Erik Christian Montes Schütte, and Sander Schwenk-Nebbe, which is available to download for free at SSRN: [https://ssrn.com/abstract=4278745](https://ssrn.com/abstract=4278745).
+This package implements the $\text{oShapley-VI}_p$ (out-of-sample Shapley-based variable importance), $\text{PBSV}_p$ (performance-based Shapley value), MAS (model accordance score) and MAS hypothesis testing, proposed in the "The Anatomy of Out-of-Sample Forecasting Accuracy" paper by Daniel Borup, Philippe Goulet Coulombe, David E. Rapach, Erik Christian Montes Schütte, and Sander Schwenk-Nebbe, which is available to download for free at SSRN: [https://ssrn.com/abstract=4278745](https://ssrn.com/abstract=4278745).
 
-The $\text{PBSV}_p$ is a Shapley-based decomposition that measures the contributions of an individual predictor $p$ in fitted models to the out-of-sample loss.
+The $\text{PBSV}_p$ is a Shapley-based decomposition that measures the contributions of an individual predictor $p$ in fitted models to the out-of-sample loss. While a performance metric like the RMSE focuses solely on out-of-sample performance, MAS evaluates whether a model's out-of-sample success mirrors what it has learned from the in-sample data by comparing $\text{iShapley-VI}_p$ (or $\text{oShapley-VI}_p$) to $\text{PBSV}_p$. The MAS paired with a performance metric such as the RMSE provides insight into the model's "intentional success" (see [below example](#model-accordance-score)).
 
 The interpretation of PBSVs is straightforward: if $\text{PBSV}_p$ is negative (positive), predictor $p$ reduces (increases) the loss and is thus beneficial for (detrimental to) forecasting accuracy in the out-of-sample period. Taking the sum of the individual contributions (including the contribution of the empty set) yields the decomposed loss exactly (due to the efficiency property of Shapley values; see [below example](#the-efficiency-property)).
 
 Please cite our paper if you find the package useful:
 
     Borup, Daniel and Coulombe, Philippe Goulet and Rapach, David E. and Montes Schütte, Erik Christian and Schwenk-Nebbe, Sander (2022). “The Anatomy of Out-of-Sample Forecasting Accuracy”. Federal Reserve Bank of Atlanta Working Paper 2022-16. https://doi.org/10.29338/wp2022-16.
 
@@ -258,24 +258,24 @@
 ## ... the RMSE of the forecasts in a subperiod:
 
     subset = pd.date_range("2021-07-28", "2021-08-06").map(lambda x: x.date())
     	    
     def transform(y_hat, y):  
         return np.sqrt(np.mean((y - y_hat) ** 2))  
         
-    df = anatomy.explain(  
+    df_pbsv_rmse = anatomy.explain(  
         model_sets=AnatomyModelCombination(groups=groups),  
         transformer=AnatomyModelOutputTransformer(transform=transform),  
         explanation_subset=subset 
     )
 
 which yields the change in root mean squared error in the ten-day period attributable to each predictor:
 
 ```
->>> df
+>>> df_pbsv_rmse
                                  base_contribution       x_0       x_1       x_2
 rf     2021-07-28 -> 2021-08-06           1.402950 -0.149847 -0.199615  0.118059
 ols    2021-07-28 -> 2021-08-06           1.404761 -0.155275 -0.323760  0.317055
 ols+rf 2021-07-28 -> 2021-08-06           1.403853 -0.169584 -0.275408  0.211672
 ```
 
 ### _Interpretation_
@@ -284,41 +284,65 @@
 
 
 ## ... or just the raw forecasts:
 
     def transform(y_hat):
         return y_hat
         
-    df = anatomy.explain(
+    df_oshapley = anatomy.explain(
         model_sets=AnatomyModelCombination(groups=groups),
         transformer=AnatomyModelOutputTransformer(transform=transform)
     )
 
 which yields the change in the forecast attributable to each predictor:
 
-    >>> df
+    >>> df_oshapley
                        base_contribution       x_0       x_1       x_2
     rf     2021-07-28           0.070861  0.222932  0.360182 -0.315820
            2021-07-29           0.070354  0.250389 -0.617779  0.984992
            2021-07-30           0.071163 -1.514547  0.839562 -0.835136
     ...                              ...       ...       ...       ...
 
 ### *Interpretation*
 
 Decomposing the forecasts themselves yields contributions that bear no relation to forecasting accuracy. Hence, a negative or positive contribution means no more than a decrease or increase in the forecast at that period attributable to the given predictor, which may or may not have be good for forecasting accuracy.
 
 ***Hence: beware, a high average absolute contribution does not necessarily translate into a high gain in accuracy. That is precisely why we need to decompose the loss directly, and in consequence, take into account our target and how far away our forecasts were from it.***
 
-From the anatomized raw forecasts, we can compute the  $\text{oShapley-VI}$ by averaging over the magnitudes of the invididual contributions:
+From the anatomized raw forecasts, we can compute the $\text{oShapley-VI}$ by averaging over the magnitudes of the invididual contributions (here for the ``ols+rf`` combination):
+
+    >>> df_oshapley.loc["ols+rf"].abs().mean(axis=0)
+    base_contribution    0.078415
+    x_0                  0.864057
+    x_1                  0.786044
+    x_2                  0.770115
+
+## Model Accordance Score:
+
+We can compute the MAS for our combination model (``ols+rf``) using $\text{oShapley-VI}$ and, for instance, the $\text{PBSV(RMSE)}_p$:
+
+    vi = df_oshapley.loc["ols+rf"].abs().mean(axis=0).drop("base_contribution")
+    pbsv = df_pbsv_rmse.loc["ols+rf"].iloc[0].drop("base_contribution")
+
+    h0 = MAS.H0(p=vi.shape[0])               # generate mas(p) under the null
+    loss_type = MAS.LossType.LOWER_IS_BETTER # rmse => lower is better
+
+    mas = MAS(vi, pbsv, loss_type, h0).compute()
+
+which yields the MAS:
+
+    >>> mas
+    {'mas': 1.0, 'mas_p_val': 0.0}
+
+### *Interpretation*
+
+In this example, the ranking of $\text{oShapley-VI}$ is identical to the signed-ranking of $\text{PBSV(RMSE)}_p$.
+Thus, MAS is 1 (perfect) and the null hypothesis of no relation between $\text{oShapley-VI}$ and $\text{PBSV(RMSE)}_p$ is rejected
+(``mas_p_val`` is the probability of observing a MAS lower or equal to ``mas`` under the null).
 
-    >>> df.abs().mean(axis=0)
-    base_contribution    0.078436
-    x_0                  0.865098
-    x_1                  0.787327
-    x_2                  0.773340
 
 ## The Efficiency property
 
 *During estimation, the `Anatomy` checks that the individual attributions of the predictors to the forecasts sum up exactly to the forecasts produced by the models. The estimation would be aborted if efficiency does not hold.*
 
 Due to the efficiency property of Shapley values, summing the individual contributions yields the decomposed value exactly. We can check that the results that `Anatomy` yields are consistet. We can recover the RMSE from the decomposed RMSE, but we can also recover the RMSE from the decomposed forecasts. Let's make sure that they match.
```

### Comparing `anatomy-0.1.4/setup.py` & `anatomy-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from pathlib import Path
 
 setup(
     name="anatomy",
-    version="0.1.4",
+    version="0.1.5",
     packages=["anatomy"],
     install_requires=[
         "joblib>=0.15.0",
         "numpy>=1.18.1",
         "pandas>=1.0.0"
     ],
     python_requires=">=3.9",
```

