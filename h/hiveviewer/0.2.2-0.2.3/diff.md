# Comparing `tmp/hiveviewer-0.2.2.tar.gz` & `tmp/hiveviewer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiveviewer-0.2.2.tar", last modified: Wed Aug  2 04:47:02 2023, max compression
+gzip compressed data, was "hiveviewer-0.2.3.tar", last modified: Thu Aug  3 06:11:20 2023, max compression
```

## Comparing `hiveviewer-0.2.2.tar` & `hiveviewer-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.455361 hiveviewer-0.2.2/
--rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.2.2/LICENSE
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-02 04:47:02.455192 hiveviewer-0.2.2/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.2.2/README.md
--rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.2.2/pyproject.toml
--rw-r--r--   0 yin        (501) staff       (20)       38 2023-08-02 04:47:02.455411 hiveviewer-0.2.2/setup.cfg
--rw-r--r--   0 yin        (501) staff       (20)     1006 2023-08-02 04:45:55.000000 hiveviewer-0.2.2/setup.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.445181 hiveviewer-0.2.2/src/
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.446833 hiveviewer-0.2.2/src/hiveviewer/
--rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.2.2/src/hiveviewer/__init__.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.449201 hiveviewer-0.2.2/src/hiveviewer/dataloader/
--rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.2.2/src/hiveviewer/dataloader/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     3169 2023-07-21 04:18:15.000000 hiveviewer-0.2.2/src/hiveviewer/dataloader/base.py
--rw-r--r--   0 yin        (501) staff       (20)      519 2023-07-21 03:59:25.000000 hiveviewer-0.2.2/src/hiveviewer/dataloader/load_csv.py
--rw-r--r--   0 yin        (501) staff       (20)      512 2023-07-21 03:19:27.000000 hiveviewer-0.2.2/src/hiveviewer/dataloader/load_excel.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.449954 hiveviewer-0.2.2/src/hiveviewer/evaluation/
--rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.2.2/src/hiveviewer/evaluation/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     7284 2023-08-02 03:41:50.000000 hiveviewer-0.2.2/src/hiveviewer/evaluation/calculator.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.450938 hiveviewer-0.2.2/src/hiveviewer/optimization/
--rw-r--r--   0 yin        (501) staff       (20)      128 2023-08-01 02:03:43.000000 hiveviewer-0.2.2/src/hiveviewer/optimization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)      770 2023-08-02 03:43:12.000000 hiveviewer-0.2.2/src/hiveviewer/optimization/base.py
--rw-r--r--   0 yin        (501) staff       (20)     5984 2023-08-02 04:46:32.000000 hiveviewer-0.2.2/src/hiveviewer/optimization/multiple_objective.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.452759 hiveviewer-0.2.2/src/hiveviewer/sampling/
--rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.2.2/src/hiveviewer/sampling/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.2.2/src/hiveviewer/sampling/base.py
--rw-r--r--   0 yin        (501) staff       (20)     1394 2023-07-31 03:32:57.000000 hiveviewer-0.2.2/src/hiveviewer/sampling/frequency_sampler.py
--rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.2.2/src/hiveviewer/sampling/gini_sampler.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.454831 hiveviewer-0.2.2/src/hiveviewer/visualization/
--rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/lorenz_curve.py
--rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/plot_trisurf.py
--rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/venn2.py
--rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/venn3.py
--rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/venn_base.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.447924 hiveviewer-0.2.2/src/hiveviewer.egg-info/
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-02 04:47:02.000000 hiveviewer-0.2.2/src/hiveviewer.egg-info/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)     1013 2023-08-02 04:47:02.000000 hiveviewer-0.2.2/src/hiveviewer.egg-info/SOURCES.txt
--rw-r--r--   0 yin        (501) staff       (20)        1 2023-08-02 04:47:02.000000 hiveviewer-0.2.2/src/hiveviewer.egg-info/dependency_links.txt
--rw-r--r--   0 yin        (501) staff       (20)       82 2023-08-02 04:47:02.000000 hiveviewer-0.2.2/src/hiveviewer.egg-info/requires.txt
--rw-r--r--   0 yin        (501) staff       (20)       11 2023-08-02 04:47:02.000000 hiveviewer-0.2.2/src/hiveviewer.egg-info/top_level.txt
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.852433 hiveviewer-0.2.3/
+-rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.2.3/LICENSE
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-03 06:11:20.852279 hiveviewer-0.2.3/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.2.3/README.md
+-rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.2.3/pyproject.toml
+-rw-r--r--   0 yin        (501) staff       (20)       38 2023-08-03 06:11:20.852491 hiveviewer-0.2.3/setup.cfg
+-rw-r--r--   0 yin        (501) staff       (20)     1006 2023-08-03 06:10:45.000000 hiveviewer-0.2.3/setup.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.845913 hiveviewer-0.2.3/src/
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.847546 hiveviewer-0.2.3/src/hiveviewer/
+-rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.2.3/src/hiveviewer/__init__.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.849123 hiveviewer-0.2.3/src/hiveviewer/dataloader/
+-rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.2.3/src/hiveviewer/dataloader/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     3200 2023-08-03 06:08:44.000000 hiveviewer-0.2.3/src/hiveviewer/dataloader/base.py
+-rw-r--r--   0 yin        (501) staff       (20)      885 2023-08-03 06:08:42.000000 hiveviewer-0.2.3/src/hiveviewer/dataloader/load_csv.py
+-rw-r--r--   0 yin        (501) staff       (20)      862 2023-08-03 06:10:38.000000 hiveviewer-0.2.3/src/hiveviewer/dataloader/load_excel.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.849526 hiveviewer-0.2.3/src/hiveviewer/evaluation/
+-rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.2.3/src/hiveviewer/evaluation/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     7362 2023-08-02 08:49:24.000000 hiveviewer-0.2.3/src/hiveviewer/evaluation/calculator.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.850110 hiveviewer-0.2.3/src/hiveviewer/optimization/
+-rw-r--r--   0 yin        (501) staff       (20)      128 2023-08-01 02:03:43.000000 hiveviewer-0.2.3/src/hiveviewer/optimization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)      770 2023-08-02 03:43:12.000000 hiveviewer-0.2.3/src/hiveviewer/optimization/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     6582 2023-08-03 06:07:28.000000 hiveviewer-0.2.3/src/hiveviewer/optimization/multiple_objective.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.851050 hiveviewer-0.2.3/src/hiveviewer/sampling/
+-rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.2.3/src/hiveviewer/sampling/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.2.3/src/hiveviewer/sampling/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     1394 2023-07-31 03:32:57.000000 hiveviewer-0.2.3/src/hiveviewer/sampling/frequency_sampler.py
+-rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.2.3/src/hiveviewer/sampling/gini_sampler.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.852057 hiveviewer-0.2.3/src/hiveviewer/visualization/
+-rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/lorenz_curve.py
+-rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/plot_trisurf.py
+-rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/venn2.py
+-rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/venn3.py
+-rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/venn_base.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.848412 hiveviewer-0.2.3/src/hiveviewer.egg-info/
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-03 06:11:20.000000 hiveviewer-0.2.3/src/hiveviewer.egg-info/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)     1013 2023-08-03 06:11:20.000000 hiveviewer-0.2.3/src/hiveviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yin        (501) staff       (20)        1 2023-08-03 06:11:20.000000 hiveviewer-0.2.3/src/hiveviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yin        (501) staff       (20)       82 2023-08-03 06:11:20.000000 hiveviewer-0.2.3/src/hiveviewer.egg-info/requires.txt
+-rw-r--r--   0 yin        (501) staff       (20)       11 2023-08-03 06:11:20.000000 hiveviewer-0.2.3/src/hiveviewer.egg-info/top_level.txt
```

### Comparing `hiveviewer-0.2.2/LICENSE` & `hiveviewer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.2/PKG-INFO` & `hiveviewer-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.2.2/README.md` & `hiveviewer-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.2/setup.py` & `hiveviewer-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "openpyxl",
         "optuna",
     ],
 )
 
 setup(
     name="hiveviewer",
-    version="0.2.2",
+    version="0.2.3",
     author="Yin Cheng",
     author_email="yin.sjtu@gmail.com",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/yinsn/hiveviewer",
     python_requires=">=3.6",
     description="Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.",
```

### Comparing `hiveviewer-0.2.2/src/hiveviewer/dataloader/base.py` & `hiveviewer-0.2.3/src/hiveviewer/dataloader/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 import pandas as pd
 
 
 class BaseDataLoader(ABC):
     """Base class for data loaders."""
 
-    def __init__(self, file_path: str, file_name: str, file_type: str = "csv") -> None:
+    def __init__(
+        self, file_path: str, file_name: Optional[str] = None, file_type: str = "csv"
+    ) -> None:
         self.file_path = file_path
         self.file_type = file_type
         self.file_name = file_name
         self.df = self.load_data()
 
     @abstractmethod
     def load_data(self) -> pd.DataFrame:
```

### Comparing `hiveviewer-0.2.2/src/hiveviewer/evaluation/calculator.py` & `hiveviewer-0.2.3/src/hiveviewer/evaluation/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             )
         elif self.equation_type == "sum":
             weights_array = np.array(weights_for_equation).reshape(-1, 1)
             self.df["overall_score"] = self.selected_values @ weights_array
 
     def calculate_wuauc(
         self,
-        groupby: str,
+        groupby: Optional[str],
         weights_for_equation: List,
         weights_for_groups: Optional[pd.Series] = None,
         label_column: str = "label",
         auc: bool = False,
     ) -> float:
         """Calculate weighted user AUC.
 
@@ -79,22 +79,23 @@
         """
         self.get_overall_score(weights_for_equation)
         if auc:
             result = float(
                 roc_auc_score(self.df[label_column], self.df["overall_score"])
             )
         else:
-            grouped = self.df.groupby(groupby).apply(
-                lambda x: float(roc_auc_score(x[label_column], x["overall_score"]))
-            )
-            if weights_for_groups is not None:
-                counts_sorted = weights_for_groups.loc[grouped.index]
-                result = float(np.average(grouped, weights=counts_sorted.values))
-            else:
-                result = float(np.mean(grouped))
+            if groupby is not None:
+                grouped = self.df.groupby(groupby).apply(
+                    lambda x: float(roc_auc_score(x[label_column], x["overall_score"]))
+                )
+                if weights_for_groups is not None:
+                    counts_sorted = weights_for_groups.loc[grouped.index]
+                    result = float(np.average(grouped, weights=counts_sorted.values))
+                else:
+                    result = float(np.mean(grouped))
         return result
 
     def create_score_columns(
         self, boundary_dict: dict, score_column: str = "score"
     ) -> None:
         """Create score columns.
```

### Comparing `hiveviewer-0.2.2/src/hiveviewer/optimization/base.py` & `hiveviewer-0.2.3/src/hiveviewer/optimization/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.2/src/hiveviewer/optimization/multiple_objective.py` & `hiveviewer-0.2.3/src/hiveviewer/optimization/multiple_objective.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 from typing import List, Optional
 
-import numpy as np
 import optuna
 from optuna.trial import Trial
 
 from ..evaluation.calculator import Calculator
 from .base import BaseObjective
 
 
@@ -38,14 +37,15 @@
         super().__init__(direction, formula, first_order, dirichlet)
         self.calculators: List[Calculator] = []
         self.calculator_flags: List[str] = []
         self.hyperparameters: List[Optional[float]] = []
         self.target_columns: List[str] = []
         self.weights_num = weights_num
         self.formula = formula
+        self.groupbys: List[Optional[str]] = []
         self.power = power
         self.first_order = first_order
         self.first_order_lower_bound = first_order_lower_bound
         self.first_order_upper_bound = first_order_upper_bound
         self.dirichlet = dirichlet
         if log_file:
             self.build_logger(log_file)
@@ -59,14 +59,15 @@
 
     def add_calculator(
         self,
         calculator: Calculator,
         flag: str,
         target_column: str,
         hyperparameter: Optional[float] = None,
+        groupby: Optional[str] = None,
     ) -> None:
         """Add calculators to the objective.
 
         Args:
             calculator (Calculator): calculator building blocks.
             flag (str ["wuauc", "profolio", "logmse"]): type of calculation.
             target_column (str): target column to calculate.
@@ -74,14 +75,18 @@
         self.calculators.append(calculator)
         self.calculator_flags.append(flag)
         self.target_columns.append(target_column)
         if hyperparameter is not None:
             self.hyperparameters.append(hyperparameter)
         else:
             self.hyperparameters.append(None)
+        if groupby is not None:
+            self.groupbys.append(groupby)
+        else:
+            self.groupbys.append(None)
 
     def objective(
         self,
         trial: Trial,
     ) -> float:
         """
         Calculate the objective value.
@@ -110,18 +115,19 @@
                         self.first_order_lower_bound,
                         self.first_order_upper_bound,
                         log=True,
                     )
                 )
 
         targets: List[float] = []
-        for calculator, flag, hyperparameter, target_column in zip(
+        for calculator, flag, hyperparameter, groupby, target_column in zip(
             self.calculators,
             self.calculator_flags,
             self.hyperparameters,
+            self.groupbys,
             self.target_columns,
         ):
             weights: List[float] = []
             if not (self.first_order):
                 weights = power_weights
             elif calculator.equation_type == "product" and self.power:
                 weights = power_weights + first_order_weights
@@ -134,30 +140,39 @@
                 _, concentration = calculator.calculate_portfolio_concentration(
                     target_column=target_column,
                     expected_return=hyperparameter,
                 )
                 targets.append(concentration)
             elif flag == "wuauc":
                 wuauc = calculator.calculate_wuauc(
-                    groupby=target_column,
+                    groupby=groupby,
+                    label_column=target_column,
                     weights_for_equation=weights,
                 )
                 targets.append(wuauc)
+            elif flag == "auc":
+                auc = calculator.calculate_wuauc(
+                    groupby=groupby,
+                    label_column=target_column,
+                    weights_for_equation=weights,
+                    auc=True,
+                )
+                targets.append(auc)
             elif flag == "woauc":
                 woauc = calculator.calculate_woauc(
                     weights_for_equation=weights,
                 )
                 targets.append(sum(woauc))
             elif flag == "logmse":
                 mse = calculator.calculate_log_mse(
                     target_column=target_column,
                 )
                 targets.append(mse)
 
-        local_vars = {"targets": targets, "sum": sum}
+        local_vars = {"targets": targets, "sum": sum, "max": max, "min": min}
         result = float(eval(self.formula, {"__builtins__": None}, local_vars))
         if self.logger:
             self.logger.info(f"Trial {trial.number} finished with result: {result}")
             self.logger.info(f"targets: {targets}")
             self.logger.info(f"weights: {weights}")
             if self.first_order:
                 self.logger.info(f"first_order_weights: {first_order_weights}")
```

### Comparing `hiveviewer-0.2.2/src/hiveviewer/sampling/base.py` & `hiveviewer-0.2.3/src/hiveviewer/sampling/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.2/src/hiveviewer/sampling/frequency_sampler.py` & `hiveviewer-0.2.3/src/hiveviewer/sampling/frequency_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.2/src/hiveviewer/sampling/gini_sampler.py` & `hiveviewer-0.2.3/src/hiveviewer/sampling/gini_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.2/src/hiveviewer/visualization/lorenz_curve.py` & `hiveviewer-0.2.3/src/hiveviewer/visualization/lorenz_curve.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.2/src/hiveviewer/visualization/plot_trisurf.py` & `hiveviewer-0.2.3/src/hiveviewer/visualization/plot_trisurf.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.2/src/hiveviewer/visualization/venn2.py` & `hiveviewer-0.2.3/src/hiveviewer/visualization/venn2.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.2/src/hiveviewer/visualization/venn3.py` & `hiveviewer-0.2.3/src/hiveviewer/visualization/venn3.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.2/src/hiveviewer/visualization/venn_base.py` & `hiveviewer-0.2.3/src/hiveviewer/visualization/venn_base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.2/src/hiveviewer.egg-info/PKG-INFO` & `hiveviewer-0.2.3/src/hiveviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.2.2/src/hiveviewer.egg-info/SOURCES.txt` & `hiveviewer-0.2.3/src/hiveviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

