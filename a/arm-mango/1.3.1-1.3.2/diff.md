# Comparing `tmp/arm-mango-1.3.1.tar.gz` & `tmp/arm_mango-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arm-mango-1.3.1.tar", max compression
+gzip compressed data, was "arm_mango-1.3.2.tar", max compression
```

## Comparing `arm-mango-1.3.1.tar` & `arm_mango-1.3.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    11357 2022-07-09 05:12:38.000000 arm-mango-1.3.1/LICENSE
--rw-r--r--   0        0        0    23264 2023-01-21 04:22:18.188972 arm-mango-1.3.1/README.md
--rw-r--r--   0        0        0      143 2023-01-21 04:22:18.258761 arm-mango-1.3.1/mango/__init__.py
--rwxr-xr-x   0        0        0        0 2023-01-06 12:23:27.333605 arm-mango-1.3.1/mango/domain/__init__.py
--rw-r--r--   0        0        0     2974 2022-07-09 05:12:44.000000 arm-mango-1.3.1/mango/domain/batch_parameter_sampler.py
--rw-r--r--   0        0        0      121 2022-07-09 05:12:44.000000 arm-mango-1.3.1/mango/domain/distribution.py
--rw-r--r--   0        0        0     7246 2023-01-21 04:22:18.259045 arm-mango-1.3.1/mango/domain/domain_space.py
--rw-r--r--   0        0        0    15383 2023-01-21 04:22:18.259322 arm-mango-1.3.1/mango/metatuner.py
--rwxr-xr-x   0        0        0        0 2023-01-06 12:23:27.333678 arm-mango-1.3.1/mango/optimizer/__init__.py
--rw-r--r--   0        0        0      248 2022-07-09 05:12:42.000000 arm-mango-1.3.1/mango/optimizer/base_predictor.py
--rw-r--r--   0        0        0    13839 2023-01-21 04:22:18.259600 arm-mango-1.3.1/mango/optimizer/bayesian_learning.py
--rw-r--r--   0        0        0     1878 2022-07-09 05:12:42.000000 arm-mango-1.3.1/mango/scheduler.py
--rw-r--r--   0        0        0    13348 2023-01-21 04:22:18.259807 arm-mango-1.3.1/mango/tuner.py
--rw-r--r--   0        0        0      752 2023-01-21 04:22:18.260215 arm-mango-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    24693 2023-01-21 04:27:44.620339 arm-mango-1.3.1/setup.py
--rw-r--r--   0        0        0    24075 2023-01-21 04:27:44.621564 arm-mango-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-09 05:12:38.000000 arm_mango-1.3.2/LICENSE
+-rw-r--r--   0        0        0    23264 2023-08-03 14:19:55.422043 arm_mango-1.3.2/README.md
+-rw-r--r--   0        0        0      143 2023-01-21 04:22:18.258761 arm_mango-1.3.2/mango/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-01-06 12:23:27.333605 arm_mango-1.3.2/mango/domain/__init__.py
+-rw-r--r--   0        0        0     2974 2022-07-09 05:12:44.000000 arm_mango-1.3.2/mango/domain/batch_parameter_sampler.py
+-rw-r--r--   0        0        0      121 2022-07-09 05:12:44.000000 arm_mango-1.3.2/mango/domain/distribution.py
+-rw-r--r--   0        0        0     7246 2023-01-21 04:22:18.259045 arm_mango-1.3.2/mango/domain/domain_space.py
+-rw-r--r--   0        0        0    15383 2023-01-21 04:22:18.259322 arm_mango-1.3.2/mango/metatuner.py
+-rwxr-xr-x   0        0        0        0 2023-01-06 12:23:27.333678 arm_mango-1.3.2/mango/optimizer/__init__.py
+-rw-r--r--   0        0        0      248 2022-07-09 05:12:42.000000 arm_mango-1.3.2/mango/optimizer/base_predictor.py
+-rw-r--r--   0        0        0    13839 2023-01-21 04:22:18.259600 arm_mango-1.3.2/mango/optimizer/bayesian_learning.py
+-rw-r--r--   0        0        0     1878 2022-07-09 05:12:42.000000 arm_mango-1.3.2/mango/scheduler.py
+-rw-r--r--   0        0        0    13348 2023-08-03 14:19:55.425788 arm_mango-1.3.2/mango/tuner.py
+-rw-r--r--   0        0        0      752 2023-08-03 14:25:18.677874 arm_mango-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    24174 1970-01-01 00:00:00.000000 arm_mango-1.3.2/PKG-INFO
```

### Comparing `arm-mango-1.3.1/LICENSE` & `arm_mango-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arm-mango-1.3.1/README.md` & `arm_mango-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `arm-mango-1.3.1/mango/domain/batch_parameter_sampler.py` & `arm_mango-1.3.2/mango/domain/batch_parameter_sampler.py`

 * *Files identical despite different names*

### Comparing `arm-mango-1.3.1/mango/domain/domain_space.py` & `arm_mango-1.3.2/mango/domain/domain_space.py`

 * *Files identical despite different names*

### Comparing `arm-mango-1.3.1/mango/metatuner.py` & `arm_mango-1.3.2/mango/metatuner.py`

 * *Files identical despite different names*

### Comparing `arm-mango-1.3.1/mango/optimizer/bayesian_learning.py` & `arm_mango-1.3.2/mango/optimizer/bayesian_learning.py`

 * *Files identical despite different names*

### Comparing `arm-mango-1.3.1/mango/scheduler.py` & `arm_mango-1.3.2/mango/scheduler.py`

 * *Files identical despite different names*

### Comparing `arm-mango-1.3.1/mango/tuner.py` & `arm_mango-1.3.2/mango/tuner.py`

 * *Files identical despite different names*

### Comparing `arm-mango-1.3.1/pyproject.toml` & `arm_mango-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arm-mango"
-version = "1.3.1"
+version = "1.3.2"
 description = "parallel bayesian optimization over complex search spaces"
 authors = ["Sandeep Singh Sandha <sandha.iitr@gmail.com>", "Mohit Aggarwal <mohitagg@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/ARM-software/mango"
 repository = "https://github.com/ARM-software/mango"
 packages = [
```

### Comparing `arm-mango-1.3.1/setup.py` & `arm_mango-1.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,541 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: arm-mango
+Version: 1.3.2
+Summary: parallel bayesian optimization over complex search spaces
+Home-page: https://github.com/ARM-software/mango
+License: Apache-2.0
+Author: Sandeep Singh Sandha
+Author-email: sandha.iitr@gmail.com
+Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: attrdict (>=2.0.1)
+Requires-Dist: numpy (>=1.17.0)
+Requires-Dist: scikit_learn (>=0.21.3)
+Requires-Dist: scipy (>=1.4.1)
+Requires-Dist: tqdm (>=4.36.1)
+Project-URL: Repository, https://github.com/ARM-software/mango
+Description-Content-Type: text/markdown
 
-packages = \
-['mango', 'mango.domain', 'mango.optimizer']
+# Mango: A parallel hyperparameter tuning library
 
-package_data = \
-{'': ['*']}
+**Mango** is a python library to find the optimal hyperparameters for machine learning classifiers. 
+Mango enables parallel optimization over complex search spaces of continuous/discrete/categorical values.
 
-install_requires = \
-['attrdict>=2.0.1',
- 'numpy>=1.17.0',
- 'scikit_learn>=0.21.3',
- 'scipy>=1.4.1',
- 'tqdm>=4.36.1']
-
-setup_kwargs = {
-    'name': 'arm-mango',
-    'version': '1.3.1',
-    'description': 'parallel bayesian optimization over complex search spaces',
-    'long_description': '# Mango: A parallel hyperparameter tuning library\n\n**Mango** is a python library to find the optimal hyperparameters for machine learning classifiers. \nMango enables parallel optimization over complex search spaces of continuous/discrete/categorical values.\n\n**Check out the quick 12 seconds demo** of Mango approximating a complex decision boundary of SVM\n\n[![AirSim Drone Demo Video](documents/demo_video.png)](https://youtu.be/hFmSdDLLUfY)\n\nMango has the following salient features:\n- Easily define complex search spaces compatible with the scikit-learn.\n- A novel state-of-the-art gradient-free optimizer for continuous/discrete/categorical values.\n- Modular design to schedule objective function on local, cluster,  or cloud infrastructure.\n- Failure detection in the application layer for scalability on commodity hardware.\n- New features are continuously added due to the testing and usage in production settings.\n\n\n## Index\n1. [Installation](#setup)\n2. [Getting started ](#getting-started)\n3. [Hyperparameter tuning example ](#knnexample)\n4. [Search space definitions](#DomainSpace)\n5. [Scheduler](#scheduler)\n6. [Optional configurations](#MangoConfigurations)\n7. [Additional features](#AdditionalFeatures)\n8. [CASH feature](#CASHFeature)\n9. [Platform-aware neural architecture search](https://github.com/ARM-software/mango/tree/master/examples/THIN-Bayes)\n10. [Mango introduction slides](https://github.com/ARM-software/mango/blob/master/documents/Mango_github_slides.pdf) & [Mango production usage slides](https://github.com/ARM-software/mango/blob/master/documents/Mango_cogml_slides.pdf).\n11. [Core Mango research papers to cite](#CorePapers) and [novel applications built over Mango](#ApplicationPapers)\n\n<!--\n11. [Mango paper (ICASSP 2020)](https://arxiv.org/pdf/2005.11394.pdf) & [Mango paper (CogMI 2021)](https://github.com/ARM-software/mango/blob/master/documents/Mango_CogMI_paper.pdf).\n-->\n\n<!--\n7. [Schedule Objective Function on Celery](#Celery)\n8. [Algorithms](#mangoAlgorithms)\n9. [ Tune Hyperparameters of Facebook Prophet ](https://github.com/ARM-software/mango/blob/master/examples/Prophet_Classifier.ipynb)\n10. [ Tune Hyperparameters of xgboost XGBRegressor ](https://github.com/ARM-software/mango/blob/master/examples/Xgboost_Example.ipynb)\n11. [ Tune Hyperparameters of xgboost XGBClassifier ](https://github.com/ARM-software/mango/blob/master/examples/Xgboost_XGBClassifier.ipynb)\n12. [Tune Hyperparameters of SVM](https://github.com/ARM-software/mango/blob/master/examples/SVM_Example.ipynb)\n13. [ More Examples](https://github.com/ARM-software/mango/tree/master/examples)\n14. [ Contact & Questions ](#contactDetails)\n-->\n\n<a name="setup"></a>\n## 1. Installation\nUsing `pip`:\n```\npip install arm-mango\n```\nFrom source:\n```\n$ git clone https://github.com/ARM-software/mango.git\n$ cd mango\n$ pip3 install .\n```\n\n<!--\n- Mango requires scikit-learn and is developed for python 3, some other packages are installed which required to optimize xgboost classifiers and fbprophet.\n!-->\n\n\n<a name="getting-started"></a>\n## 2. Getting Started\nMango is straightforward to use. Following example minimizes the quadratic function whose input is an integer between -10 and 10.\n\n```python\nfrom mango import scheduler, Tuner\n\n# Search space\nparam_space = dict(x=range(-10,10))\n\n# Quadratic objective Function\n@scheduler.serial\ndef objective(x):\n    return x * x\n\n# Initialize and run Tuner\ntuner = Tuner(param_space, objective)\nresults = tuner.minimize()\n\nprint(f\'Optimal value of parameters: {results["best_params"]} and objective: {results["best_objective"]}\')```\n# => Optimal value of parameters: {\'x\': 0}  and objective: 0\n```\n\n<a name="knnexample"></a>\n## 3. Hyperparameter Tuning Example\n\n```python\nfrom sklearn import datasets\nfrom sklearn.neighbors import KNeighborsClassifier\nfrom sklearn.model_selection import cross_val_score\n\nfrom mango import Tuner, scheduler\n\n# search space for KNN classifier\'s hyperparameters\n# n_neighbors can vary between 1 and 50, with different choices of algorithm\nparam_space = dict(n_neighbors=range(1, 50),\n                   algorithm=[\'auto\', \'ball_tree\', \'kd_tree\', \'brute\'])\n\n\n@scheduler.serial\ndef objective(**params):\n    X, y = datasets.load_breast_cancer(return_X_y=True)\n    clf = KNeighborsClassifier(**params)\n    score = cross_val_score(clf, X, y, scoring=\'accuracy\').mean()\n    return score\n\n\ntuner = Tuner(param_space, objective)\nresults = tuner.maximize()\nprint(\'best parameters:\', results[\'best_params\'])\nprint(\'best accuracy:\', results[\'best_objective\'])\n# => best parameters: {\'algorithm\': \'ball_tree\', \'n_neighbors\': 11}\n# => best accuracy: 0.9332401800962584\n```\nNote that best parameters may be different but accuracy should be ~ 0.93. More examples are available\nin the `examples` directory ([Facebook\'s Prophet](https://github.com/ARM-software/mango/blob/master/examples/Prophet_Classifier.ipynb),\n[XGBoost](https://github.com/ARM-software/mango/blob/master/examples/Xgboost_XGBClassifier.ipynb), [SVM](https://github.com/ARM-software/mango/blob/master/examples/SVM_Example.ipynb)).\n\n\n<a name="DomainSpace"></a>\n## 4. Search Space\nThe search space defines the range and distribution of input parameters to the objective function.\nMango search space is compatible with scikit-learn\'s parameter space definitions used in\n[RandomizedSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html)\n or [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html).\nThe search space is defined as a dictionary with keys being the parameter names (string) and values being\nlist of discreet choices, range of integers or the distributions. Example of some common search spaces are:\n\n### Integer\nFollowing space defines `x` as an integer parameters with values in `range(-10, 11)` (11 is not included):\n```python\nparam_space = dict(x=range(-10, 11)) #=> -10, -9, ..., 10\n# you can use steps for sparse ranges\nparam_space = dict(x=range(0, 101, 10)) #=> 0, 10, 20, ..., 100\n```\nIntegers are uniformly sampled from the given range and are assumed to be ordered and treated as continuous variables.\n\n### Categorical\nDiscreet categories can be defined as lists. For example:\n```python\n# string\nparam_space = dict(color=[\'red\', \'blue\', \'green\'])\n# float\nparam_space = dict(v=[0.2, 0.1, 0.3])\n# mixed\nparam_space = dict(max_features=[\'auto\', 0.2, 0.3])\n```\nLists are uniformly sampled and are assumed to be unordered. They are one-hot encoded internally.\n\n### Distributions\nAll the distributions supported by [`scipy.stats`](https://docs.scipy.org/doc/scipy/reference/stats.html) are supported.\nIn general, distributions must provide a `rvs` method for sampling.\n\n#### Uniform distribution\nUsing `uniform(loc, scale)` one obtains the uniform distribution on `[loc, loc + scale]`.\n```python\nfrom scipy.stats import uniform\n\n# uniformly distributed between -1 and 1\nparam_space = dict(a=uniform(-1, 2))\n```\n\n#### Log uniform distribution\nWe have added [loguniform](https://github.com/ARM-software/mango/blob/master/mango/domain/distribution.py) distribution by extending the `scipy.stats.distributions` constructs.\nUsing `loguniform(loc, scale)` one obtains the loguniform distribution on <code>[10<sup>loc</sup>, 10<sup>loc + scale</sup>]</code>.\n```python\nfrom mango.domain.distribution import loguniform\n\n# log uniformly distributed between 10^-3 and 10^-1\nparam_space = dict(learning_rate=loguniform(-3, 2))\n```\n\n\n### Hyperparameter search space examples\nExample hyperparameter search space for [Random Forest Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html):\n```python\nparam_space =  dict(\n    max_features=[\'sqrt\', \'log2\', .1, .3, .5, .7, .9],\n    n_estimators=range(10, 1000, 50), # 10 to 1000 in steps of 50\n    bootstrap=[True, False],\n    max_depth=range(1, 20),\n    min_samples_leaf=range(1, 10)\n)\n```\n\n\nExample search space for [XGBoost Classifier](https://xgboost.readthedocs.io/en/latest/python/python_api.html#xgboost.XGBClassifier):\n```python\nfrom scipy.stats import uniform\nfrom mango.domain.distribution import loguniform\n\nparam_space = {\n    \'n_estimators\': range(10, 2001, 100), # 10 to 2000 in steps of 100\n    \'max_depth\': range(1, 15), # 1 to 14\n    \'reg_alpha\': loguniform(-3, 6),  # 10^-3 to 10^3\n    \'booster\': [\'gbtree\', \'gblinear\'],\n    \'colsample_bylevel\': uniform(0.05, 0.95), # 0.05 to 1.0\n    \'colsample_bytree\': uniform(0.05, 0.95), # 0.05 to 1.0\n    \'learning_rate\': loguniform(-3, 3),  # 0.001 to 1\n    \'reg_lambda\': loguniform(-3, 6),  # 10^-3 to 10^3\n    \'min_child_weight\': loguniform(0, 2), # 1 to 100\n    \'subsample\': uniform(0.1, 0.89) # 0.1 to 0.99\n}\n```\n\nExample search space for [SVM](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html):\n```python\nfrom scipy.stats import uniform\nfrom mango.domain.distribution import loguniform\n\nparam_dict = {\n    \'kernel\': [\'rbf\', \'sigmoid\'],\n    \'gamma\': uniform(0.1, 4), # 0.1 to 4.1\n    \'C\': loguniform(-7, 8) # 10^-7 to 10\n}\n```\n\n<a name="scheduler"></a>\n## 5. Scheduler\n\nMango is designed to take advantage of distributed computing. The objective function can be scheduled to\nrun locally or on a cluster with parallel evaluations. Mango is designed to allow the use of any distributed\ncomputing framework (like Celery or Kubernetes). The `scheduler` module comes with some pre-defined\nschedulers.\n\n### Serial scheduler\nSerial scheduler runs locally with one objective function evaluation at a time\n```python\nfrom mango import scheduler\n\n@scheduler.serial\ndef objective(x):\n    return x * x\n```\n\n### Parallel scheduler\nParallel scheduler runs locally and uses `joblib` to evaluate the objective functions in parallel\n```python\nfrom mango import scheduler\n\n@scheduler.parallel(n_jobs=2)\ndef objective(x):\n    return x * x\n```\n`n_jobs` specifies the number of parallel evaluations. `n_jobs = -1` uses all the available cpu cores\non the machine. See [simple_parallel](https://github.com/ARM-software/mango/tree/master/examples/simple_parallel.py)\nfor full working example.\n\n### Custom distributed scheduler\nUsers can define their own distribution strategies using `custom` scheduler. To do so, users need to define\nan objective function that takes a list of parameters and returns the list of results:\n```python\nfrom mango import scheduler\n\n@scheduler.custom(n_jobs=4)\ndef objective(params_batch):\n    """ Template for custom distributed objective function\n    Args:\n        params_batch (list): Batch of parameter dictionaries to be evaluated in parallel\n\n    Returns:\n        list: Values of objective function at given parameters\n    """\n    # evaluate the objective on a distributed framework\n    ...\n    return results\n```\n\nFor example the following snippet uses [Celery](http://www.celeryproject.org/):\n```python\nimport celery\nfrom mango import Tuner, scheduler\n\n# connect to celery backend\napp = celery.Celery(\'simple_celery\', backend=\'rpc://\')\n\n# remote celery task\n@app.task\ndef remote_objective(x):\n    return x * x\n\n@scheduler.custom(n_jobs=4)\ndef objective(params_batch):\n    jobs = celery.group(remote_objective.s(params[\'x\']) for params in params_batch)()\n    return jobs.get()\n\nparam_space = dict(x=range(-10, 10))\n\ntuner = Tuner(param_space, objective)\nresults = tuner.minimize()\n```\nA working example to tune hyperparameters of KNN using Celery is [here](https://github.com/ARM-software/mango/tree/master/examples/knn_celery.py).\n\n<!--\n<a name="ObjectiveFunction"></a>\n## 5. More on Objective Function\nThe serial objective function has the following structure.\n\n```python\ndef objective_function(params_list):\n    evaluations = []\n    for hyper_par in params_list:\n        result =  evaluate_function_on_hyper_par\n        evaluations.append(result)\n    return evaluations\n```\nThe objective function is called with the input list of hyper parameters. Each element of the list is the dictionary which is a sample drawn from the domain space of variables. Mango expects the objective function to return the list of\nevaluations which has the same size as the args_list. Each value of the evaluations list is the function evaluated at hyperparameters\nof params_list in the same order. A rich set of objective functions are shown in the [examples](https://github.com/ARM-software/mango/tree/master/examples). The size of the params_list is controlled by the batch_size configuration parameter of Mango. By default,\nbatch_size is 1. The configuration parameters of Mango are explained in the [Mango Configurations](#MangoConfigurations) section.\n\nThe sample skeleton of the Celery based parallel objective function in Mango is as following.\n\n```python\ndef objective_celery(params_list):\n    process_queue = []\n    for par in params_list:\n        process = train_clf.delay(par)\n        process_queue.append((process, par))\n    evals = []\n    params = []\n    for process, par in process_queue:\n        result = process.get()\n        evals.append(result)\n        params.append(par)\n    return params, evals\n```\n-->\n\n<a name="MangoConfigurations"></a>\n## 6. Optional configurations\n\nThe default configuration parameters used by the Mango as below:\n```python\n{\'param_dict\': ...,\n \'userObjective\': ...,\n \'domain_size\': 5000,\n \'initial_random\': 1,\n \'num_iteration\': 20,\n \'batch_size\': 1}\n```\nThe configuration parameters are:\n- *domain_size*: The size which is explored in each iteration by the gaussian process. Generally, a larger size is preferred if higher dimensional functions are optimized. More on this will be added with details about the internals of bayesian optimization.\n- *initial_random*: The number of random samples tried. Note: Mango returns all the random samples together. Users can exploit this to parallelize the random runs without any constraint.\n- *num_iteration*: The total number of iterations used by Mango to find the optimal value.\n- *batch_size*: The size of args_list passed to the objective function for parallel evaluation. For larger batch sizes, Mango internally uses intelligent sampling to decide the optimal samples to evaluate.\n- *early_stopping*: A Callable to specify custom stopping criteria. The callback has the following signature:\n   ```python\n  def early_stopping(results):\n      \'\'\'\n          results is the same as dict returned by tuner\n          keys available: params_tries, objective_values,\n              best_objective, best_params\n      \'\'\'\n      ...\n      return True/False\n  ```\n    Early stopping is one of Mango\'s important features that allow to early terminate the current parallel search\n    based on the custom user-designed criteria, such as the total optimization time spent, current validation accuracy\n    achieved, or improvements in the past few iterations. For usage see early stopping examples [notebook](https://github.com/ARM-software/mango/blob/master/examples/EarlyStopping.ipynb).\n- *constraint*: A callable to specify constraints on parameter space. It has the following\n  signature:\n  ```python\n  def constraint(samples: List[dict]) -> List[bool]:\n    \'\'\'\n        Given a list of samples (each sample is a dict with parameter names as keys)\n        Returns a list of True/False elements indicating whether the corresponding sample\n        satisfies the constraints or not\n    \'\'\'\n  ```\n  See [this](<examples/Test functions for constrained optimization.ipynb>) notebook for an example.\n- *initial_custom*: A list of initial evaluation points to warm up the optimizer instead of random sampling. For example, for a search space with two parameters `x1` and `x2` the input could be:   `[{\'x1\': 10, \'x2\': -5}, {\'x1\': 0, \'x2\': 10}]`. This allows the user to customize the initial evaluation points and therefore guide the optimization process. If this option is given then `initial_random` is ignored.  \n\n\nThe default configuration parameters can be modified, as shown below. Only the parameters whose values need to adjusted can be passed as the dictionary.\n\n```python\nconf_dict = dict(num_iteration=40, domain_size=10000, initial_random=3)\n\ntuner = Tuner(param_dict, objective, conf_dict)\n```\n\n<a name="AdditionalFeatures"></a>\n## 7. Additional Features\n### Handling runtime failed evaluation\nAt runtime, failed evaluations are widespread in production deployments. Mango abstractions enable users to make progress even in the presence of failures by only using the correct evaluations. The syntax can return the successful evaluation, and the user can flexibly keep track of failures, for example, using timeouts. Examples showing the usage of Mango in the presence of failures: [serial execution](https://github.com/ARM-software/mango/blob/master/examples/Failure_Handling.ipynb) and [parallel execution](https://github.com/ARM-software/mango/blob/master/examples/Failure_Handling_Parallel.ipynb)\n\n### Neural Architecture Search\nMango can also do an efficient neural architecture search. An example on the MNIST dataset to search for optimal filter sizes, the number of filters, etc., is [available](https://github.com/ARM-software/mango/blob/master/examples/NAS_Mnist.ipynb).\n\nMore extensive examples are available in the [THIN-Bayes](https://github.com/ARM-software/mango/tree/master/examples/THIN-Bayes) folder doing *Neural Architecture Search* for a class of neural networks and classical models for different regression and classification tasks. \n\n<!--\n<a name="Celery"></a>\n## 7. Schedule Objective Function on Celery\nUser-defined objective function can be scheduled on local, cluster or cloud infrastructure. The objective function scheduler\nis entirely independent of the Mango. This design was chosen to enable the scheduling of varied resource objective function according to developer needs. We have included examples using [Celery](http://www.celeryproject.org/). In the sample\nexamples, celery workers are used to evaluate the objective function in parallel. These examples assume celery is installed, and workers\nare running. Default celery configurations can be modified in the [file](https://github.com/ARM-software/mango/blob/master/examples/classifiers/celery.py).\n\n- [KNN example using celery workers](https://github.com/ARM-software/mango/blob/master/examples/KNN_Celery.ipynb)\n- [Prophet example using celery workers](https://github.com/ARM-software/mango/blob/master/examples/Prophet_Celery.ipynb)\n\nMore examples will be included to show the scheduling of objective function using local threads/processes. By default examples schedule\nthe objective function on the local machine itself.\n\n<a name ="mangoAlgorithms"></a>\n## 8. Algorithms\nThe optimization algorithms in Mango are based on widely used Bayesian optimization techniques, extended to sample a batch of configurations in parallel. Currently, Mango provides two parallel optimization algorithms that use the upper confidence bound as the acquisition function. The first algorithm uses hallucination combined with exponential rescaling of the surrogate function to select a batch. In the second algorithm, we create clusters of acquisition function in spatially distinct search spaces, and select the maximum value within each cluster to create the batch.\n\n<a name="contactDetails"></a>\n## More Details\nDetails about specifying parameter/variable domain space, user objective function, and internals of Mango will be added.\nPlease stay tuned.\n-->\n\n<a name="CASHFeature"></a>\n## 8. Combiner Classifier Selection and Optimization (CASH)\nMango now provides a novel functionality of combined classifier selection and optimization. It allows developers to directly specify a set of classifiers along with their different hyperparameter spaces. Mango internally finds the best classifier along with the optimal parameters with the least possible number of overall iterations. The examples are  available [here](https://github.com/ARM-software/mango/tree/master/benchmarking/MetaTuner_Examples)\n\nThe important parts in the skeletion code are as below.\n\n```python\nfrom mango import MetaTuner\n\n#define search spaces and objective functions as done for tuner.\n\nparam_space_list = [param_space1, param_space2, param_space3, param_space4, ..]\nobjective_list = [objective_1, objective_2, objective_3, objective_4, ..]\n\nmetatuner = MetaTuner(param_space_list, objective_list)\n\nresults = metatuner.run()\n\nprint(\'best_objective:\',results[\'best_objective\'])\nprint(\'best_params:\',results[\'best_params\'])\nprint(\'best_objective_fid:\',results[\'best_objective_fid\'])\n\n```\n\n## Participate\n\n<a name="CorePapers"></a>\n### Core Papers to Cite Mango\n\nMore technical details are available in the [Mango paper-1 (ICASSP 2020)](https://arxiv.org/pdf/2005.11394.pdf) and [Mango paper-2 (CogMI 2021)](https://drive.google.com/file/d/1uzcTUfLM3JSc47RLQJin-YzybwNl6BZO/view)\nPlease cite them as:\n```\n@inproceedings{sandha2020mango,\n  title={Mango: A Python Library for Parallel Hyperparameter Tuning},\n  author={Sandha, Sandeep Singh and Aggarwal, Mohit and Fedorov, Igor and Srivastava, Mani},\n  booktitle={ICASSP 2020-2020 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},\n  pages={3987--3991},\n  year={2020},\n  organization={IEEE}\n}\n```\n```\n@inproceedings{sandha2021mango,\n  title={Enabling Hyperparameter Tuning of Machine Learning Classifiers in Production},\n  author={Sandha, Sandeep Singh and Aggarwal, Mohit and Saha, Swapnil Sayan and Srivastava, Mani},\n  booktitle={CogMI 2021, IEEE International Conference on Cognitive Machine Intelligence},\n  year={2021},\n  organization={IEEE}\n}\n```\n\n<a name="ApplicationPapers"></a>\n### Novel Applications built over Mango\n```\n@article{saha2022auritus,\n  title={Auritus: An open-source optimization toolkit for training and development of human movement models and filters using earables},\n  author={Saha, Swapnil Sayan and Sandha, Sandeep Singh and Pei, Siyou and Jain, Vivek and Wang, Ziqi and Li, Yuchen and Sarker, Ankur and Srivastava, Mani},\n  journal={Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies},\n  volume={6},\n  number={2},\n  pages={1--34},\n  year={2022},\n  publisher={ACM New York, NY, USA}\n}\n```\n```\n@article{saha2022tinyodom,\n  title={Tinyodom: Hardware-aware efficient neural inertial navigation},\n  author={Saha, Swapnil Sayan and Sandha, Sandeep Singh and Garcia, Luis Antonio and Srivastava, Mani},\n  journal={Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies},\n  volume={6},\n  number={2},\n  pages={1--32},\n  year={2022},\n  publisher={ACM New York, NY, USA}\n}\n```\n```\n@article{saha2022thin,\n  title={THIN-Bayes: Platform-Aware Machine Learning for Low-End IoT Devices},\n  author={Saha, Swapnil Sayan and Sandha, Sandeep Singh and Aggarwal, Mohit and Srivastava, Mani},\n  year={2022}\n}\n```\n\n\n### Slides\n\nSlides explaining Mango abstractions and design choices are available. [Mango Slides-1](https://github.com/ARM-software/mango/blob/master/documents/Mango_github_slides.pdf), [Mango Slides-2](https://drive.google.com/file/d/1_sUOnbW-LkHMMcjq_WgzabN7IQ-wBRgn/view).\n\n### Contribute\n\nPlease take a look at [open issues](https://github.com/ARM-software/mango/issues) if you are looking for areas to contribute to.\n\n### Questions\n\nFor any questions feel free to reach out by creating an issue [here](https://github.com/ARM-software/mango/issues/new).\n',
-    'author': 'Sandeep Singh Sandha',
-    'author_email': 'sandha.iitr@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ARM-software/mango',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8',
+**Check out the quick 12 seconds demo** of Mango approximating a complex decision boundary of SVM
+
+[![AirSim Drone Demo Video](documents/demo_video.png)](https://youtu.be/hFmSdDLLUfY)
+
+Mango has the following salient features:
+- Easily define complex search spaces compatible with the scikit-learn.
+- A novel state-of-the-art gradient-free optimizer for continuous/discrete/categorical values.
+- Modular design to schedule objective function on local, cluster,  or cloud infrastructure.
+- Failure detection in the application layer for scalability on commodity hardware.
+- New features are continuously added due to the testing and usage in production settings.
+
+
+## Index
+1. [Installation](#setup)
+2. [Getting started ](#getting-started)
+3. [Hyperparameter tuning example ](#knnexample)
+4. [Search space definitions](#DomainSpace)
+5. [Scheduler](#scheduler)
+6. [Optional configurations](#MangoConfigurations)
+7. [Additional features](#AdditionalFeatures)
+8. [CASH feature](#CASHFeature)
+9. [Platform-aware neural architecture search](https://github.com/ARM-software/mango/tree/master/examples/THIN-Bayes)
+10. [Mango introduction slides](https://github.com/ARM-software/mango/blob/master/documents/Mango_github_slides.pdf) & [Mango production usage slides](https://github.com/ARM-software/mango/blob/master/documents/Mango_cogml_slides.pdf).
+11. [Core Mango research papers to cite](#CorePapers) and [novel applications built over Mango](#ApplicationPapers)
+
+<!--
+11. [Mango paper (ICASSP 2020)](https://arxiv.org/pdf/2005.11394.pdf) & [Mango paper (CogMI 2021)](https://github.com/ARM-software/mango/blob/master/documents/Mango_CogMI_paper.pdf).
+-->
+
+<!--
+7. [Schedule Objective Function on Celery](#Celery)
+8. [Algorithms](#mangoAlgorithms)
+9. [ Tune Hyperparameters of Facebook Prophet ](https://github.com/ARM-software/mango/blob/master/examples/Prophet_Classifier.ipynb)
+10. [ Tune Hyperparameters of xgboost XGBRegressor ](https://github.com/ARM-software/mango/blob/master/examples/Xgboost_Example.ipynb)
+11. [ Tune Hyperparameters of xgboost XGBClassifier ](https://github.com/ARM-software/mango/blob/master/examples/Xgboost_XGBClassifier.ipynb)
+12. [Tune Hyperparameters of SVM](https://github.com/ARM-software/mango/blob/master/examples/SVM_Example.ipynb)
+13. [ More Examples](https://github.com/ARM-software/mango/tree/master/examples)
+14. [ Contact & Questions ](#contactDetails)
+-->
+
+<a name="setup"></a>
+## 1. Installation
+Using `pip`:
+```
+pip install arm-mango
+```
+From source:
+```
+$ git clone https://github.com/ARM-software/mango.git
+$ cd mango
+$ pip3 install .
+```
+
+<!--
+- Mango requires scikit-learn and is developed for python 3, some other packages are installed which required to optimize xgboost classifiers and fbprophet.
+!-->
+
+
+<a name="getting-started"></a>
+## 2. Getting Started
+Mango is straightforward to use. Following example minimizes the quadratic function whose input is an integer between -10 and 10.
+
+```python
+from mango import scheduler, Tuner
+
+# Search space
+param_space = dict(x=range(-10,10))
+
+# Quadratic objective Function
+@scheduler.serial
+def objective(x):
+    return x * x
+
+# Initialize and run Tuner
+tuner = Tuner(param_space, objective)
+results = tuner.minimize()
+
+print(f'Optimal value of parameters: {results["best_params"]} and objective: {results["best_objective"]}')```
+# => Optimal value of parameters: {'x': 0}  and objective: 0
+```
+
+<a name="knnexample"></a>
+## 3. Hyperparameter Tuning Example
+
+```python
+from sklearn import datasets
+from sklearn.neighbors import KNeighborsClassifier
+from sklearn.model_selection import cross_val_score
+
+from mango import Tuner, scheduler
+
+# search space for KNN classifier's hyperparameters
+# n_neighbors can vary between 1 and 50, with different choices of algorithm
+param_space = dict(n_neighbors=range(1, 50),
+                   algorithm=['auto', 'ball_tree', 'kd_tree', 'brute'])
+
+
+@scheduler.serial
+def objective(**params):
+    X, y = datasets.load_breast_cancer(return_X_y=True)
+    clf = KNeighborsClassifier(**params)
+    score = cross_val_score(clf, X, y, scoring='accuracy').mean()
+    return score
+
+
+tuner = Tuner(param_space, objective)
+results = tuner.maximize()
+print('best parameters:', results['best_params'])
+print('best accuracy:', results['best_objective'])
+# => best parameters: {'algorithm': 'ball_tree', 'n_neighbors': 11}
+# => best accuracy: 0.9332401800962584
+```
+Note that best parameters may be different but accuracy should be ~ 0.93. More examples are available
+in the `examples` directory ([Facebook's Prophet](https://github.com/ARM-software/mango/blob/master/examples/Prophet_Classifier.ipynb),
+[XGBoost](https://github.com/ARM-software/mango/blob/master/examples/Xgboost_XGBClassifier.ipynb), [SVM](https://github.com/ARM-software/mango/blob/master/examples/SVM_Example.ipynb)).
+
+
+<a name="DomainSpace"></a>
+## 4. Search Space
+The search space defines the range and distribution of input parameters to the objective function.
+Mango search space is compatible with scikit-learn's parameter space definitions used in
+[RandomizedSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html)
+ or [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html).
+The search space is defined as a dictionary with keys being the parameter names (string) and values being
+list of discreet choices, range of integers or the distributions. Example of some common search spaces are:
+
+### Integer
+Following space defines `x` as an integer parameters with values in `range(-10, 11)` (11 is not included):
+```python
+param_space = dict(x=range(-10, 11)) #=> -10, -9, ..., 10
+# you can use steps for sparse ranges
+param_space = dict(x=range(0, 101, 10)) #=> 0, 10, 20, ..., 100
+```
+Integers are uniformly sampled from the given range and are assumed to be ordered and treated as continuous variables.
+
+### Categorical
+Discreet categories can be defined as lists. For example:
+```python
+# string
+param_space = dict(color=['red', 'blue', 'green'])
+# float
+param_space = dict(v=[0.2, 0.1, 0.3])
+# mixed
+param_space = dict(max_features=['auto', 0.2, 0.3])
+```
+Lists are uniformly sampled and are assumed to be unordered. They are one-hot encoded internally.
+
+### Distributions
+All the distributions supported by [`scipy.stats`](https://docs.scipy.org/doc/scipy/reference/stats.html) are supported.
+In general, distributions must provide a `rvs` method for sampling.
+
+#### Uniform distribution
+Using `uniform(loc, scale)` one obtains the uniform distribution on `[loc, loc + scale]`.
+```python
+from scipy.stats import uniform
+
+# uniformly distributed between -1 and 1
+param_space = dict(a=uniform(-1, 2))
+```
+
+#### Log uniform distribution
+We have added [loguniform](https://github.com/ARM-software/mango/blob/master/mango/domain/distribution.py) distribution by extending the `scipy.stats.distributions` constructs.
+Using `loguniform(loc, scale)` one obtains the loguniform distribution on <code>[10<sup>loc</sup>, 10<sup>loc + scale</sup>]</code>.
+```python
+from mango.domain.distribution import loguniform
+
+# log uniformly distributed between 10^-3 and 10^-1
+param_space = dict(learning_rate=loguniform(-3, 2))
+```
+
+
+### Hyperparameter search space examples
+Example hyperparameter search space for [Random Forest Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html):
+```python
+param_space =  dict(
+    max_features=['sqrt', 'log2', .1, .3, .5, .7, .9],
+    n_estimators=range(10, 1000, 50), # 10 to 1000 in steps of 50
+    bootstrap=[True, False],
+    max_depth=range(1, 20),
+    min_samples_leaf=range(1, 10)
+)
+```
+
+
+Example search space for [XGBoost Classifier](https://xgboost.readthedocs.io/en/latest/python/python_api.html#xgboost.XGBClassifier):
+```python
+from scipy.stats import uniform
+from mango.domain.distribution import loguniform
+
+param_space = {
+    'n_estimators': range(10, 2001, 100), # 10 to 2000 in steps of 100
+    'max_depth': range(1, 15), # 1 to 14
+    'reg_alpha': loguniform(-3, 6),  # 10^-3 to 10^3
+    'booster': ['gbtree', 'gblinear'],
+    'colsample_bylevel': uniform(0.05, 0.95), # 0.05 to 1.0
+    'colsample_bytree': uniform(0.05, 0.95), # 0.05 to 1.0
+    'learning_rate': loguniform(-3, 3),  # 0.001 to 1
+    'reg_lambda': loguniform(-3, 6),  # 10^-3 to 10^3
+    'min_child_weight': loguniform(0, 2), # 1 to 100
+    'subsample': uniform(0.1, 0.89) # 0.1 to 0.99
 }
+```
+
+Example search space for [SVM](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html):
+```python
+from scipy.stats import uniform
+from mango.domain.distribution import loguniform
+
+param_dict = {
+    'kernel': ['rbf', 'sigmoid'],
+    'gamma': uniform(0.1, 4), # 0.1 to 4.1
+    'C': loguniform(-7, 8) # 10^-7 to 10
+}
+```
+
+<a name="scheduler"></a>
+## 5. Scheduler
+
+Mango is designed to take advantage of distributed computing. The objective function can be scheduled to
+run locally or on a cluster with parallel evaluations. Mango is designed to allow the use of any distributed
+computing framework (like Celery or Kubernetes). The `scheduler` module comes with some pre-defined
+schedulers.
+
+### Serial scheduler
+Serial scheduler runs locally with one objective function evaluation at a time
+```python
+from mango import scheduler
+
+@scheduler.serial
+def objective(x):
+    return x * x
+```
+
+### Parallel scheduler
+Parallel scheduler runs locally and uses `joblib` to evaluate the objective functions in parallel
+```python
+from mango import scheduler
+
+@scheduler.parallel(n_jobs=2)
+def objective(x):
+    return x * x
+```
+`n_jobs` specifies the number of parallel evaluations. `n_jobs = -1` uses all the available cpu cores
+on the machine. See [simple_parallel](https://github.com/ARM-software/mango/tree/master/examples/simple_parallel.py)
+for full working example.
+
+### Custom distributed scheduler
+Users can define their own distribution strategies using `custom` scheduler. To do so, users need to define
+an objective function that takes a list of parameters and returns the list of results:
+```python
+from mango import scheduler
+
+@scheduler.custom(n_jobs=4)
+def objective(params_batch):
+    """ Template for custom distributed objective function
+    Args:
+        params_batch (list): Batch of parameter dictionaries to be evaluated in parallel
+
+    Returns:
+        list: Values of objective function at given parameters
+    """
+    # evaluate the objective on a distributed framework
+    ...
+    return results
+```
+
+For example the following snippet uses [Celery](http://www.celeryproject.org/):
+```python
+import celery
+from mango import Tuner, scheduler
+
+# connect to celery backend
+app = celery.Celery('simple_celery', backend='rpc://')
+
+# remote celery task
+@app.task
+def remote_objective(x):
+    return x * x
+
+@scheduler.custom(n_jobs=4)
+def objective(params_batch):
+    jobs = celery.group(remote_objective.s(params['x']) for params in params_batch)()
+    return jobs.get()
+
+param_space = dict(x=range(-10, 10))
+
+tuner = Tuner(param_space, objective)
+results = tuner.minimize()
+```
+A working example to tune hyperparameters of KNN using Celery is [here](https://github.com/ARM-software/mango/tree/master/examples/knn_celery.py).
+
+<!--
+<a name="ObjectiveFunction"></a>
+## 5. More on Objective Function
+The serial objective function has the following structure.
+
+```python
+def objective_function(params_list):
+    evaluations = []
+    for hyper_par in params_list:
+        result =  evaluate_function_on_hyper_par
+        evaluations.append(result)
+    return evaluations
+```
+The objective function is called with the input list of hyper parameters. Each element of the list is the dictionary which is a sample drawn from the domain space of variables. Mango expects the objective function to return the list of
+evaluations which has the same size as the args_list. Each value of the evaluations list is the function evaluated at hyperparameters
+of params_list in the same order. A rich set of objective functions are shown in the [examples](https://github.com/ARM-software/mango/tree/master/examples). The size of the params_list is controlled by the batch_size configuration parameter of Mango. By default,
+batch_size is 1. The configuration parameters of Mango are explained in the [Mango Configurations](#MangoConfigurations) section.
+
+The sample skeleton of the Celery based parallel objective function in Mango is as following.
+
+```python
+def objective_celery(params_list):
+    process_queue = []
+    for par in params_list:
+        process = train_clf.delay(par)
+        process_queue.append((process, par))
+    evals = []
+    params = []
+    for process, par in process_queue:
+        result = process.get()
+        evals.append(result)
+        params.append(par)
+    return params, evals
+```
+-->
+
+<a name="MangoConfigurations"></a>
+## 6. Optional configurations
+
+The default configuration parameters used by the Mango as below:
+```python
+{'param_dict': ...,
+ 'userObjective': ...,
+ 'domain_size': 5000,
+ 'initial_random': 1,
+ 'num_iteration': 20,
+ 'batch_size': 1}
+```
+The configuration parameters are:
+- *domain_size*: The size which is explored in each iteration by the gaussian process. Generally, a larger size is preferred if higher dimensional functions are optimized. More on this will be added with details about the internals of bayesian optimization.
+- *initial_random*: The number of random samples tried. Note: Mango returns all the random samples together. Users can exploit this to parallelize the random runs without any constraint.
+- *num_iteration*: The total number of iterations used by Mango to find the optimal value.
+- *batch_size*: The size of args_list passed to the objective function for parallel evaluation. For larger batch sizes, Mango internally uses intelligent sampling to decide the optimal samples to evaluate.
+- *early_stopping*: A Callable to specify custom stopping criteria. The callback has the following signature:
+   ```python
+  def early_stopping(results):
+      '''
+          results is the same as dict returned by tuner
+          keys available: params_tries, objective_values,
+              best_objective, best_params
+      '''
+      ...
+      return True/False
+  ```
+    Early stopping is one of Mango's important features that allow to early terminate the current parallel search
+    based on the custom user-designed criteria, such as the total optimization time spent, current validation accuracy
+    achieved, or improvements in the past few iterations. For usage see early stopping examples [notebook](https://github.com/ARM-software/mango/blob/master/examples/EarlyStopping.ipynb).
+- *constraint*: A callable to specify constraints on parameter space. It has the following
+  signature:
+  ```python
+  def constraint(samples: List[dict]) -> List[bool]:
+    '''
+        Given a list of samples (each sample is a dict with parameter names as keys)
+        Returns a list of True/False elements indicating whether the corresponding sample
+        satisfies the constraints or not
+    '''
+  ```
+  See [this](<examples/Test functions for constrained optimization.ipynb>) notebook for an example.
+- *initial_custom*: A list of initial evaluation points to warm up the optimizer instead of random sampling. For example, for a search space with two parameters `x1` and `x2` the input could be:   `[{'x1': 10, 'x2': -5}, {'x1': 0, 'x2': 10}]`. This allows the user to customize the initial evaluation points and therefore guide the optimization process. If this option is given then `initial_random` is ignored.  
+
+
+The default configuration parameters can be modified, as shown below. Only the parameters whose values need to adjusted can be passed as the dictionary.
+
+```python
+conf_dict = dict(num_iteration=40, domain_size=10000, initial_random=3)
+
+tuner = Tuner(param_dict, objective, conf_dict)
+```
+
+<a name="AdditionalFeatures"></a>
+## 7. Additional Features
+### Handling runtime failed evaluation
+At runtime, failed evaluations are widespread in production deployments. Mango abstractions enable users to make progress even in the presence of failures by only using the correct evaluations. The syntax can return the successful evaluation, and the user can flexibly keep track of failures, for example, using timeouts. Examples showing the usage of Mango in the presence of failures: [serial execution](https://github.com/ARM-software/mango/blob/master/examples/Failure_Handling.ipynb) and [parallel execution](https://github.com/ARM-software/mango/blob/master/examples/Failure_Handling_Parallel.ipynb)
+
+### Neural Architecture Search
+Mango can also do an efficient neural architecture search. An example on the MNIST dataset to search for optimal filter sizes, the number of filters, etc., is [available](https://github.com/ARM-software/mango/blob/master/examples/NAS_Mnist.ipynb).
+
+More extensive examples are available in the [THIN-Bayes](https://github.com/ARM-software/mango/tree/master/examples/THIN-Bayes) folder doing *Neural Architecture Search* for a class of neural networks and classical models for different regression and classification tasks. 
+
+<!--
+<a name="Celery"></a>
+## 7. Schedule Objective Function on Celery
+User-defined objective function can be scheduled on local, cluster or cloud infrastructure. The objective function scheduler
+is entirely independent of the Mango. This design was chosen to enable the scheduling of varied resource objective function according to developer needs. We have included examples using [Celery](http://www.celeryproject.org/). In the sample
+examples, celery workers are used to evaluate the objective function in parallel. These examples assume celery is installed, and workers
+are running. Default celery configurations can be modified in the [file](https://github.com/ARM-software/mango/blob/master/examples/classifiers/celery.py).
+
+- [KNN example using celery workers](https://github.com/ARM-software/mango/blob/master/examples/KNN_Celery.ipynb)
+- [Prophet example using celery workers](https://github.com/ARM-software/mango/blob/master/examples/Prophet_Celery.ipynb)
+
+More examples will be included to show the scheduling of objective function using local threads/processes. By default examples schedule
+the objective function on the local machine itself.
+
+<a name ="mangoAlgorithms"></a>
+## 8. Algorithms
+The optimization algorithms in Mango are based on widely used Bayesian optimization techniques, extended to sample a batch of configurations in parallel. Currently, Mango provides two parallel optimization algorithms that use the upper confidence bound as the acquisition function. The first algorithm uses hallucination combined with exponential rescaling of the surrogate function to select a batch. In the second algorithm, we create clusters of acquisition function in spatially distinct search spaces, and select the maximum value within each cluster to create the batch.
+
+<a name="contactDetails"></a>
+## More Details
+Details about specifying parameter/variable domain space, user objective function, and internals of Mango will be added.
+Please stay tuned.
+-->
+
+<a name="CASHFeature"></a>
+## 8. Combiner Classifier Selection and Optimization (CASH)
+Mango now provides a novel functionality of combined classifier selection and optimization. It allows developers to directly specify a set of classifiers along with their different hyperparameter spaces. Mango internally finds the best classifier along with the optimal parameters with the least possible number of overall iterations. The examples are  available [here](https://github.com/ARM-software/mango/tree/master/benchmarking/MetaTuner_Examples)
+
+The important parts in the skeletion code are as below.
+
+```python
+from mango import MetaTuner
+
+#define search spaces and objective functions as done for tuner.
+
+param_space_list = [param_space1, param_space2, param_space3, param_space4, ..]
+objective_list = [objective_1, objective_2, objective_3, objective_4, ..]
+
+metatuner = MetaTuner(param_space_list, objective_list)
+
+results = metatuner.run()
+
+print('best_objective:',results['best_objective'])
+print('best_params:',results['best_params'])
+print('best_objective_fid:',results['best_objective_fid'])
+
+```
+
+## Participate
+
+<a name="CorePapers"></a>
+### Core Papers to Cite Mango
+
+More technical details are available in the [Mango paper-1 (ICASSP 2020)](https://arxiv.org/pdf/2005.11394.pdf) and [Mango paper-2 (CogMI 2021)](https://drive.google.com/file/d/1uzcTUfLM3JSc47RLQJin-YzybwNl6BZO/view)
+Please cite them as:
+```
+@inproceedings{sandha2020mango,
+  title={Mango: A Python Library for Parallel Hyperparameter Tuning},
+  author={Sandha, Sandeep Singh and Aggarwal, Mohit and Fedorov, Igor and Srivastava, Mani},
+  booktitle={ICASSP 2020-2020 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
+  pages={3987--3991},
+  year={2020},
+  organization={IEEE}
+}
+```
+```
+@inproceedings{sandha2021mango,
+  title={Enabling Hyperparameter Tuning of Machine Learning Classifiers in Production},
+  author={Sandha, Sandeep Singh and Aggarwal, Mohit and Saha, Swapnil Sayan and Srivastava, Mani},
+  booktitle={CogMI 2021, IEEE International Conference on Cognitive Machine Intelligence},
+  year={2021},
+  organization={IEEE}
+}
+```
+
+<a name="ApplicationPapers"></a>
+### Novel Applications built over Mango
+```
+@article{saha2022auritus,
+  title={Auritus: An open-source optimization toolkit for training and development of human movement models and filters using earables},
+  author={Saha, Swapnil Sayan and Sandha, Sandeep Singh and Pei, Siyou and Jain, Vivek and Wang, Ziqi and Li, Yuchen and Sarker, Ankur and Srivastava, Mani},
+  journal={Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies},
+  volume={6},
+  number={2},
+  pages={1--34},
+  year={2022},
+  publisher={ACM New York, NY, USA}
+}
+```
+```
+@article{saha2022tinyodom,
+  title={Tinyodom: Hardware-aware efficient neural inertial navigation},
+  author={Saha, Swapnil Sayan and Sandha, Sandeep Singh and Garcia, Luis Antonio and Srivastava, Mani},
+  journal={Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies},
+  volume={6},
+  number={2},
+  pages={1--32},
+  year={2022},
+  publisher={ACM New York, NY, USA}
+}
+```
+```
+@article{saha2022thin,
+  title={THIN-Bayes: Platform-Aware Machine Learning for Low-End IoT Devices},
+  author={Saha, Swapnil Sayan and Sandha, Sandeep Singh and Aggarwal, Mohit and Srivastava, Mani},
+  year={2022}
+}
+```
+
+
+### Slides
+
+Slides explaining Mango abstractions and design choices are available. [Mango Slides-1](https://github.com/ARM-software/mango/blob/master/documents/Mango_github_slides.pdf), [Mango Slides-2](https://drive.google.com/file/d/1_sUOnbW-LkHMMcjq_WgzabN7IQ-wBRgn/view).
+
+### Contribute
+
+Please take a look at [open issues](https://github.com/ARM-software/mango/issues) if you are looking for areas to contribute to.
+
+### Questions
 
+For any questions feel free to reach out by creating an issue [here](https://github.com/ARM-software/mango/issues/new).
 
-setup(**setup_kwargs)
```

