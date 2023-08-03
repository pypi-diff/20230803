# Comparing `tmp/Seance-0.0.5-py3-none-any.whl.zip` & `tmp/Seance-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 15609 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat     2360 b- defN 23-Jun-21 13:29 Seance/Explainer.py
--rw-rw-rw-  2.0 fat    11987 b- defN 23-Jul-29 23:02 Seance/Forecaster.py
--rw-rw-rw-  2.0 fat    10887 b- defN 23-Jul-29 23:01 Seance/Optimizer.py
+Zip file size: 15839 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat     2392 b- defN 23-Aug-02 14:22 Seance/Explainer.py
+-rw-rw-rw-  2.0 fat    13078 b- defN 23-Aug-03 17:10 Seance/Forecaster.py
+-rw-rw-rw-  2.0 fat    11395 b- defN 23-Jul-30 23:54 Seance/Optimizer.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:41 Seance/__init__.py
 -rw-rw-rw-  2.0 fat     3358 b- defN 23-May-18 13:18 Seance/Builder/PanelAxis.py
 -rw-rw-rw-  2.0 fat     3916 b- defN 23-Jul-06 20:13 Seance/Builder/PreProcess.py
 -rw-rw-rw-  2.0 fat     6595 b- defN 23-May-31 15:17 Seance/Builder/Transformations.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:40 Seance/Builder/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-Jun-03 01:07 Seance/basis_functions/__init__.py
 -rw-rw-rw-  2.0 fat      845 b- defN 23-Jul-06 19:45 Seance/basis_functions/fourier_basis.py
 -rw-rw-rw-  2.0 fat     2834 b- defN 23-May-31 21:10 Seance/basis_functions/linear_basis.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-29 23:03 Seance-0.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2725 b- defN 23-Jul-29 23:03 Seance-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-29 23:03 Seance-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-29 23:03 Seance-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1303 b- defN 23-Jul-29 23:03 Seance-0.0.5.dist-info/RECORD
-16 files, 48077 bytes uncompressed, 13461 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Aug-03 17:14 Seance-0.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2725 b- defN 23-Aug-03 17:14 Seance-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 17:14 Seance-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-03 17:14 Seance-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1303 b- defN 23-Aug-03 17:14 Seance-0.0.6.dist-info/RECORD
+16 files, 49708 bytes uncompressed, 13691 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: Seance/basis_functions/fourier_basis.py
 Comment: 
 
 Filename: Seance/basis_functions/linear_basis.py
 Comment: 
 
-Filename: Seance-0.0.5.dist-info/LICENSE
+Filename: Seance-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: Seance-0.0.5.dist-info/METADATA
+Filename: Seance-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: Seance-0.0.5.dist-info/WHEEL
+Filename: Seance-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: Seance-0.0.5.dist-info/top_level.txt
+Filename: Seance-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: Seance-0.0.5.dist-info/RECORD
+Filename: Seance-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Seance/Explainer.py

```diff
@@ -4,15 +4,15 @@
 import pandas as pd
 import shap
 sns.set_style('darkgrid')
 
 
 def rename_column(column_name):
     if 'basis' in column_name:
-        return 'Trend'
+        return 'LBF'
     if 'fourier' in column_name:
         return 'Seasonality'
     if 'ar_' in column_name:
         return 'AutoRegressiveLag'
     return column_name
 
 class Explainer:
@@ -54,7 +54,9 @@
             refined.plot(kind='bar', stacked=True)
 
 #%%
 if __name__ == '__main__':
     exp = Explainer(seance_obj=seance, id_column='ID', date_column='Datetime')
     exp.explain(seance.processed_df, seance.pred_X)
     model_obj = seance.mlforecast.models_['LGBMRegressor']
+
+    look = seance.processed_df
```

## Seance/Forecaster.py

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 import numpy as np
 import lightgbm as lgb
+from sklearn.linear_model import LinearRegression, Ridge
 from mlforecast import MLForecast
 from Seance.Builder import PreProcess
 from Seance.basis_functions.fourier_basis import get_fourier_series, get_future_fourier
 from Seance.basis_functions.linear_basis import get_basis, get_future_basis
 
 class Forecaster:
     def __init__(self,
@@ -33,14 +34,15 @@
 
     def fit(self,
             df,
             target_column,
             id_column,
             date_column,
             freq,
+            model='lightgbm',
             alpha=None,
             time_exogenous=None,
             id_exogenous=None,
             id_feature_columns=None,
             time_feature_columns=None,
             scale=True,
             scale_type='standard',
@@ -83,14 +85,15 @@
             bagging_fraction=1.0,
             feature_fraction=1.0,
             **kwargs,
             ):
         if scale_type == 'none':
             scale=False
         self.scale = scale
+        self.model = model
         self.seasonal_period = seasonal_period
         self.fourier_order = fourier_order
         self.date_column = date_column
         self.id_column = id_column
         self.freq = freq
         self.n_basis = n_basis
         self.decay = decay
@@ -143,57 +146,74 @@
         if self.n_basis is not None and self.n_basis:
             self.basis_list = []
             basis = self.processed_df.groupby('Seance ID')[target_column].apply(self.linear_basis)
             self.processed_df = pd.concat([self.processed_df, basis], axis=1)
         if self.seasonal_period is not None:
             self.processed_df = self.processed_df.merge(seasonal_df, on=date_column)
         self.processed_df['cat_id_col'] = self.processed_df['Seance ID'].copy()
-        lgb_params = {'sample_weights': sample_weights,
-                      'metric': metric,
-                      'learning_rate':learning_rate,
-                      'min_child_samples':min_child_samples,
-                      'num_leaves':num_leaves,
-                      'n_estimators':n_estimators,
-                      'learning_rate':learning_rate,
-                      'num_threads': num_threads,
-                       'bagging_freq': bagging_freq,
-                      'verbose': verbose,
-                        'lambda_l1': lambda_l1,
-                        'lambda_l2': lambda_l2,
-                        'bagging_fraction': bagging_fraction,
-                        'feature_fraction': feature_fraction,
-                        'objective': objective,
-                        }
         if categorical_columns is not None:
             forecast_columns += categorical_columns
             for column in categorical_columns:
                 self.processed_df[column] = self.processed_df[column].astype('category')
         if self.seasonal_period is not None:
             forecast_columns += [i for i in list(seasonal_df.columns) if i != date_column]
         if self.n_basis is not None and self.n_basis:
             forecast_columns += list(basis.columns)
-        self.mlforecast = MLForecast(models=[lgb.LGBMRegressor(**lgb_params)],
-                                     freq=freq,
-                                     lags=lags,
-                                     differences=differences,
-                                     **kwargs)
-
+        if self.model == 'lightgbm':
+            lgb_params = {'sample_weights': sample_weights,
+                          'metric': metric,
+                          'learning_rate':learning_rate,
+                          'min_child_samples':min_child_samples,
+                          'num_leaves':num_leaves,
+                          'n_estimators':n_estimators,
+                          'learning_rate':learning_rate,
+                          'num_threads': num_threads,
+                           'bagging_freq': bagging_freq,
+                          'verbose': verbose,
+                            'lambda_l1': lambda_l1,
+                            'lambda_l2': lambda_l2,
+                            'bagging_fraction': bagging_fraction,
+                            'feature_fraction': feature_fraction,
+                            'objective': objective,
+                            }
+            self.mlforecast = MLForecast(models=[lgb.LGBMRegressor(**lgb_params)],
+                                         freq=freq,
+                                         lags=lags,
+                                         differences=differences,
+                                         **kwargs)
+            self.pred_col = 'LGBMRegressor'
+        elif self.model == 'linear_regression':
+            self.mlforecast = MLForecast(models=[LinearRegression()],
+                                         freq=freq,
+                                         lags=lags,
+                                         differences=differences,
+                                         **kwargs)
+            self.pred_col = 'LinearRegression'
+        elif self.model == 'ridge':
+            if alpha is None:
+                alpha = 1
+            self.mlforecast = MLForecast(models=[Ridge(alpha=alpha)],
+                                         freq=freq,
+                                         lags=lags,
+                                         differences=differences,
+                                         **kwargs)
+            self.pred_col = 'Ridge'
         fitted = self.mlforecast.fit(self.processed_df[forecast_columns],
                                     id_col='Seance ID',
                                     time_col=date_column,
                                     target_col=target_column,
                                     static_features=categorical_columns)
-        self.model_obj = fitted.models_['LGBMRegressor']
+        self.model_obj = fitted.models_[self.pred_col]
         return fitted
 
     def inverse_transform(self, df):
         seance_id = df['Seance ID'].iloc[0]
-        unscaled = self.processor._transformers[seance_id](df['LGBMRegressor'].values)
+        unscaled = self.processor._transformers[seance_id](df[self.pred_col].values)
         unscaled = np.array(unscaled).reshape(-1)
-        df['LGBMRegressor'] = unscaled
+        df[self.pred_col] = unscaled
         return df
 
     def predict(self, forecast_horizon):
         self.forecast_horizon = forecast_horizon
         future_dates = pd.date_range(start=self.time_periods.iloc[-1],
                                      freq=self.freq,
                                      periods=forecast_horizon + 1)[1:]
@@ -233,18 +253,19 @@
         self.pred_X = pred_X
         predicted = self.mlforecast.predict(horizon=forecast_horizon,
                                             dynamic_dfs=self.dynamic_dfs)
         predicted = predicted.merge(self.run_dict['global']['ID Mapping'],
                                     on='Seance ID')
         if self.scale:
             predicted = predicted.groupby('Seance ID').apply(self.inverse_transform)
-        predicted['LGBMRegressor'] = predicted['LGBMRegressor'].clip(lower=self.floor)
+        predicted[self.pred_col] = predicted[self.pred_col].clip(lower=self.floor)
         predicted = predicted.sort_values([self.id_column, self.date_column])
-        if any(np.isnan(predicted['LGBMRegressor'])):
+        if any(np.isnan(predicted[self.pred_col])):
             print('Nan found when Inverse Transforming, use a more stable transformer such as "standard"')
         return predicted
 
     def plot_importance(self, max_num_features=20):
-        lgb.plot_importance(self.mlforecast.models_['LGBMRegressor'],
+        lgb.plot_importance(self.mlforecast.models_[self.pred_col],
                             max_num_features=max_num_features)
         return
 
+
```

## Seance/Optimizer.py

```diff
@@ -10,16 +10,16 @@
 from Seance.Forecaster import Forecaster
 # optuna.logging.set_verbosity(optuna.logging.WARNING)
 
 
 @njit
 def smape(A, F):
     return 100/len(A) * np.sum(2 * np.abs(F - A) / (0.0001 + (np.abs(A) + np.abs(F))))
-def grouped_smape(df, target_column):
-    return smape(df[target_column].values, df['LGBMRegressor'].values)
+def grouped_smape(df, target_column, predicted_column):
+    return smape(df[target_column].values, df[predicted_column].values)
 
 class Optimize:
     def __init__(self,
                  df,
                  target_column,
                  date_column,
                  id_column,
@@ -33,14 +33,15 @@
                  max_n_estimators=500,
                  ar_lags=None,
                  scale_types=['log','standard','minmax','robust_boxcox','none'],
                  min_bagging_pct=.6,
                  max_bagging_pct=1.0,
                  min_feature_fraction=.6,
                  max_n_basis=25,
+                 model='lightgbm',
                  timeout=None):
         self.df = df.sort_values([id_column, date_column])
         if isinstance(seasonal_period, list):
             self.max_pulse = max(seasonal_period)
         else:
             self.max_pulse = seasonal_period
         self.seasonal_period = seasonal_period
@@ -48,14 +49,15 @@
         self.test_size = test_size
         self.n_trials = n_trials
         self.target_column = target_column
         self.date_column = date_column
         self.id_column = id_column
         self.timeout = timeout
         self.freq = freq
+        self.model = model
         self.max_n_estimators = max_n_estimators
         # if ar_lags is None and seasonal_period is not None:
         #     ar_lags = list(np.arange(1, self.max_pulse + 1))
         # if ar_lags is None and seasonal_period is None:
         #     ar_lags = list(np.arange(1, 13))
         self.ar_lags = ar_lags
         self.metric= metric
@@ -80,68 +82,73 @@
         # self.train_df[self.date_column] = pd.to_datetime(self.train_df[self.date_column]).dt.
         self.test_df = df[df['test_split'] == True]
 
     def scorer(self, params, metric):
         scores = []
         # for train_index, test_index in cv_splits:
         try:
-            # print(params)
             model_obj = Forecaster()
             model_obj.fit(self.train_df,
                           target_column=self.target_column,
                           date_column=self.date_column,
                           id_column=self.id_column,
                           freq=self.freq,
                           categorical_columns=self.categorical_columns,
+                          model=self.model,
                           **params)
             predicted = model_obj.predict(self.test_size)
             self.predicted = predicted
             if len(predicted) != len(self.test_df):
                 print('Predicted not the same size as test set')
     
-            if any(np.isnan(predicted['LGBMRegressor'])):
+            if any(np.isnan(predicted[model_obj.pred_col])):
                 scores.append(np.inf)
             else:
                 # predicted[self.date_column] = predicted[self.date_column].dt.tz_localize(None)
                 self.test_df[self.date_column] = self.test_df[self.date_column].dt.tz_localize(None)
                 self.cv_df = self.test_df[[self.id_column, self.date_column, self.target_column]].merge(predicted, on=[self.id_column, self.date_column])
                 if metric == 'mse':
-                    scores.append(mean_squared_error(self.cv_df[self.target_column].values, self.cv_df['LGBMRegressor'].values))
+                    scores.append(mean_squared_error(self.cv_df[self.target_column].values, self.cv_df[model_obj.pred_col].values))
                 elif metric == 'smape':
-                    scores.append(self.cv_df.groupby(self.id_column).apply(grouped_smape, self.target_column))
+                    scores.append(self.cv_df.groupby(self.id_column).apply(grouped_smape, self.target_column, model_obj.pred_col))
         except Exception as e:
                 scores.append(np.inf)
                 print(f'ERROR WHILE TUNING: {e}')
         return np.mean(scores)
 
 
     def objective(self, trial):
         params = {
-            "n_estimators": trial.suggest_int(name="n_estimators", low=50, high=self.max_n_estimators),
-            'lambda_l1': trial.suggest_float('lambda_l1', 1e-8, 10.0),
-            'lambda_l2': trial.suggest_float('lambda_l2', 1e-8, 10.0),
-            'num_leaves': trial.suggest_int('num_leaves', 2, 512),
-            'feature_fraction': trial.suggest_float('feature_fraction', self.min_feature_fraction, 1.0),
-            'bagging_fraction': trial.suggest_float('bagging_fraction', self.min_bagging_pct, self.max_bagging_pct),
-            'bagging_freq': trial.suggest_int('bagging_freq', 0, 15),
-            'min_child_samples': trial.suggest_int('min_child_samples', 1, 100),
             "use_id": trial.suggest_categorical("use_id", [True, False]),
-            "objective": trial.suggest_categorical("objective", ['regression', 'regression_l1']),
             "n_basis": trial.suggest_int("n_basis", 0, self.max_n_basis),
             "differences": trial.suggest_categorical("differences", [None, 1]),
             "decay": trial.suggest_categorical("decay", [-1,
                                                          .05,
                                                          .1,
                                                          .25,
                                                          .5,
                                                          .75,
                                                          .9,
                                                          .99]),
             "scale_type": trial.suggest_categorical("scale_type", self.scale_types),
         }
+        if self.model == 'lightgbm':
+            params.update({"n_estimators": trial.suggest_int(name="n_estimators", low=50, high=self.max_n_estimators),
+                           'min_child_samples': trial.suggest_int('min_child_samples', 1, 100),
+                            'lambda_l1': trial.suggest_float('lambda_l1', 1e-8, 10.0),
+                            'lambda_l2': trial.suggest_float('lambda_l2', 1e-8, 10.0),
+                            'num_leaves': trial.suggest_int('num_leaves', 2, 512),
+                            'feature_fraction': trial.suggest_float('feature_fraction', self.min_feature_fraction, 1.0),
+                            'bagging_fraction': trial.suggest_float('bagging_fraction', self.min_bagging_pct, self.max_bagging_pct),
+                            'bagging_freq': trial.suggest_int('bagging_freq', 0, 15),
+                            "objective": trial.suggest_categorical("objective", ['regression', 'regression_l1'])
+            })
+        elif self.model == 'ridge':
+            params.update({"alpha": trial.suggest_float("alpha", 1e-8, 1000.0)
+                           })
         if self.seasonal_period:
             params.update({'seasonal_period': trial.suggest_categorical("seasonal_period", [None, self.seasonal_period])})
         if self.ar_lags is not None:
             params.update({'lags': trial.suggest_categorical("lags", self.ar_lags)})
         else:
             if self.seasonal_period:
                 params.update({'lags': trial.suggest_int(name="lags", low=1, high=self.max_pulse + 1)})
@@ -186,21 +193,22 @@
     # best_params, study = opt.fit(seed=1)
     import time
     tic = time.perf_counter()
     opt = Optimize(train_df[['V', 'Datetime', 'ID']],
                 target_column='V',
                 date_column='Datetime',
                 id_column='ID',
-                freq='W',
+                freq='M',
                 metric='smape',
-                seasonal_period=None,
+                seasonal_period=12,
+                model='lightgbm',
                 # ar_lags=[list(range(1, 4))],
                 test_size=26,
-                n_trials=10,
-                timeout=60)
+                # n_trials=10,
+                timeout=60*60*3)
     best_params, study = opt.fit(seed=1)
     toc = time.perf_counter()
     print(toc - tic)
 
 #%%
     look = opt.test_df
     look2 = opt.predicted
```

## Comparing `Seance-0.0.5.dist-info/LICENSE` & `Seance-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Seance-0.0.5.dist-info/METADATA` & `Seance-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Seance
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Wrapper around MLForecast.
 Home-page: https://github.com/tblume1992/Seance
 Author: Tyler Blume
 Author-email: tblume@mail.USF.edu
 Keywords: forecasting,time series,lightgbm,mlforecast
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: optuna
 Requires-Dist: mlforecast
 
-## SeÃ¡nce v0.0.1
+## SeÃ¡nce v0.0.5
 
 A simple wrapper around Nixtla's MLForecast aimed at streamlining plug-and-play forecasting.
 
 A general pattern is to optimize then forecast such as:
 
 ```
 from mlforecast.utils import generate_daily_series
```

## Comparing `Seance-0.0.5.dist-info/RECORD` & `Seance-0.0.6.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Seance/Explainer.py,sha256=ViUQvXZhsyrKjAscA88NOmBZEXwBl6pldjKe8IJ_fT0,2360
-Seance/Forecaster.py,sha256=exTxoAirjiDFNlvKDHlovpHP5RH2LU8oEk3xCEIvyJ8,11987
-Seance/Optimizer.py,sha256=rUcoC1Zv0YMS8riK7NW-Nei2t2j4Q_3MGnuk2yK0btU,10887
+Seance/Explainer.py,sha256=f_SHRq6cbtqKmU6wX3pO3WgRrD4xA-QHHEpG1LYcZ0o,2392
+Seance/Forecaster.py,sha256=p5baHpdIwWQnD6Qm3PyOPS9PFrfEcy9VuBhjOT8jUN4,13078
+Seance/Optimizer.py,sha256=6HcRxJMnROPNxMu7rU_F4XvN5UYDREFiyzYATus5epg,11395
 Seance/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/Builder/PanelAxis.py,sha256=w5YYnDXgprHWUzCWcqqBEkV1xJ_6qLabzW_PIbQF9ZQ,3358
 Seance/Builder/PreProcess.py,sha256=lXDwzPEYw_01pDEB9533v60uqYJEQE7Jb12vjIxmWhA,3916
 Seance/Builder/Transformations.py,sha256=JY27tWWvxha2JXhVgOALQFJUhV-N2Hcmg2u9hhBSeaA,6595
 Seance/Builder/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/basis_functions/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/basis_functions/fourier_basis.py,sha256=8KePMSK7FGqu9t_mkir101B2OvJGZ-FY9kqepiJSCyw,845
 Seance/basis_functions/linear_basis.py,sha256=1RHj--VkbA4heV8QwzNE7a9O0-aPu3Br3EqLlcuUHWU,2834
-Seance-0.0.5.dist-info/LICENSE,sha256=Dk4ScfuH6m_hggBOkCWWWoKU4wkTVtAInrZB4yhn5HU,1087
-Seance-0.0.5.dist-info/METADATA,sha256=MVj3RASdJ4lDUiAJY7_lepUNjZb0kZaFlu1jZluCcmc,2725
-Seance-0.0.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-Seance-0.0.5.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
-Seance-0.0.5.dist-info/RECORD,,
+Seance-0.0.6.dist-info/LICENSE,sha256=Dk4ScfuH6m_hggBOkCWWWoKU4wkTVtAInrZB4yhn5HU,1087
+Seance-0.0.6.dist-info/METADATA,sha256=6RFVmAWjPpqaeoDHgXkqy7cMs7unZZZh6JlB5xXHFZI,2725
+Seance-0.0.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+Seance-0.0.6.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
+Seance-0.0.6.dist-info/RECORD,,
```

