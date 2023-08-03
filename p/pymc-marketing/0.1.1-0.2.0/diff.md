# Comparing `tmp/pymc-marketing-0.1.1.tar.gz` & `tmp/pymc-marketing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc-marketing-0.1.1.tar", last modified: Wed May  3 10:22:24 2023, max compression
+gzip compressed data, was "pymc-marketing-0.2.0.tar", last modified: Thu Aug  3 19:03:36 2023, max compression
```

## Comparing `pymc-marketing-0.1.1.tar` & `pymc-marketing-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.164673 pymc-marketing-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20972 2023-05-03 10:22:24.164673 pymc-marketing-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.160673 pymc-marketing-0.1.1/pymc_marketing/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.160673 pymc-marketing-0.1.1/pymc_marketing/clv/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.164673 pymc-marketing-0.1.1/pymc_marketing/clv/models/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/models/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/models/beta_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/models/gamma_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/models/shifted_beta_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.164673 pymc-marketing-0.1.1/pymc_marketing/mmm/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20190 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/delayed_saturated_mmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/validating.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.160673 pymc-marketing-0.1.1/pymc_marketing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20972 2023-05-03 10:22:24.000000 pymc-marketing-0.1.1/pymc_marketing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-03 10:22:24.000000 pymc-marketing-0.1.1/pymc_marketing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:22:24.000000 pymc-marketing-0.1.1/pymc_marketing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-03 10:22:24.000000 pymc-marketing-0.1.1/pymc_marketing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 10:22:24.000000 pymc-marketing-0.1.1/pymc_marketing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 10:22:24.164673 pymc-marketing-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:03:36.081057 pymc-marketing-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20809 2023-08-03 19:03:36.081057 pymc-marketing-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:03:36.077057 pymc-marketing-0.2.0/pymc_marketing/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:03:36.077057 pymc-marketing-0.2.0/pymc_marketing/clv/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/clv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/clv/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:03:36.077057 pymc-marketing-0.2.0/pymc_marketing/clv/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/clv/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/clv/models/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/clv/models/beta_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18940 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/clv/models/gamma_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/clv/models/pareto_nbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/clv/models/shifted_beta_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/clv/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/clv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:03:36.081057 pymc-marketing-0.2.0/pymc_marketing/mmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/mmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25453 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/mmm/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23419 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/mmm/delayed_saturated_mmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/mmm/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/mmm/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/mmm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/mmm/validating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pymc_marketing/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:03:36.077057 pymc-marketing-0.2.0/pymc_marketing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20809 2023-08-03 19:03:36.000000 pymc-marketing-0.2.0/pymc_marketing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-03 19:03:36.000000 pymc-marketing-0.2.0/pymc_marketing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:03:36.000000 pymc-marketing-0.2.0/pymc_marketing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 19:03:36.000000 pymc-marketing-0.2.0/pymc_marketing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 19:03:36.000000 pymc-marketing-0.2.0/pymc_marketing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-03 19:03:25.000000 pymc-marketing-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 19:03:36.081057 pymc-marketing-0.2.0/setup.cfg
```

### Comparing `pymc-marketing-0.1.1/LICENSE` & `pymc-marketing-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.1/PKG-INFO` & `pymc-marketing-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-marketing
-Version: 0.1.1
+Version: 0.2.0
 Summary: Marketing Statistical Models in PyMC
 Maintainer-email: PyMC Labs <info@pymc-labs.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,15 +202,15 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: repository, https://github.com/pymc-labs/pymc-marketing
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
 <div align="center">
@@ -237,20 +237,14 @@
 ```bash
 mamba create -c conda-forge -n marketing_env pymc-marketing
 mamba activate marketing_env
 ```
 
 See the official [PyMC installation guide](https://www.pymc.io/projects/docs/en/latest/installation.html) if more detail is needed.
 
-For testing purposes, if you wish to install the `main` branch directly from GitHub:
-
-```bash
-pip install git+https://github.com/pymc-labs/pymc-marketing.git
-```
-
 ## Bayesian Media Mix Models (MMMs) in PyMC
 
 In this package we provide an API for a Bayesian media mix model (MMM) specification following [Jin, Yuxue, et al. “Bayesian methods for media mix modeling with carryover and shape effects.” (2017).](https://research.google/pubs/pub46001/) Concretely, given a time series target variable $y_{t}$ (e.g. sales on conversions), media variables $x_{m, t}$ (e.g. impressions, clicks or costs) and a set of control covariates $z_{c, t}$ (e.g. holidays, special events) we consider a linear model of the form
 
 $$
 y_{t} = \alpha + \sum_{m=1}^{M}\beta_{m}f(x_{m, t}) +  \sum_{c=1}^{C}\gamma_{c}z_{c, t} + \varepsilon_{t},
 $$
```

### Comparing `pymc-marketing-0.1.1/README.md` & `pymc-marketing-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,20 +22,14 @@
 ```bash
 mamba create -c conda-forge -n marketing_env pymc-marketing
 mamba activate marketing_env
 ```
 
 See the official [PyMC installation guide](https://www.pymc.io/projects/docs/en/latest/installation.html) if more detail is needed.
 
-For testing purposes, if you wish to install the `main` branch directly from GitHub:
-
-```bash
-pip install git+https://github.com/pymc-labs/pymc-marketing.git
-```
-
 ## Bayesian Media Mix Models (MMMs) in PyMC
 
 In this package we provide an API for a Bayesian media mix model (MMM) specification following [Jin, Yuxue, et al. “Bayesian methods for media mix modeling with carryover and shape effects.” (2017).](https://research.google/pubs/pub46001/) Concretely, given a time series target variable $y_{t}$ (e.g. sales on conversions), media variables $x_{m, t}$ (e.g. impressions, clicks or costs) and a set of control covariates $z_{c, t}$ (e.g. holidays, special events) we consider a linear model of the form
 
 $$
 y_{t} = \alpha + \sum_{m=1}^{M}\beta_{m}f(x_{m, t}) +  \sum_{c=1}^{C}\gamma_{c}z_{c, t} + \varepsilon_{t},
 $$
```

#### html2text {}

```diff
@@ -14,20 +14,18 @@
 data-driven decisions about their marketing campaigns. Optimize your marketing
 strategy and unlock the full potential of your customer data. ## Installation
 Install and activate an environment (e.g. `marketing_env`) with the `pymc-
 marketing` package from [conda-forge](https://conda-forge.org). It may look
 something like the following: ```bash mamba create -c conda-forge -
 n marketing_env pymc-marketing mamba activate marketing_env ``` See the
 official [PyMC installation guide](https://www.pymc.io/projects/docs/en/latest/
-installation.html) if more detail is needed. For testing purposes, if you wish
-to install the `main` branch directly from GitHub: ```bash pip install
-git+https://github.com/pymc-labs/pymc-marketing.git ``` ## Bayesian Media Mix
-Models (MMMs) in PyMC In this package we provide an API for a Bayesian media
-mix model (MMM) specification following [Jin, Yuxue, et al. âBayesian methods
-for media mix modeling with carryover and shape effects.â (2017).](https://
+installation.html) if more detail is needed. ## Bayesian Media Mix Models
+(MMMs) in PyMC In this package we provide an API for a Bayesian media mix model
+(MMM) specification following [Jin, Yuxue, et al. âBayesian methods for media
+mix modeling with carryover and shape effects.â (2017).](https://
 research.google/pubs/pub46001/) Concretely, given a time series target variable
 $y_{t}$ (e.g. sales on conversions), media variables $x_{m, t}$ (e.g.
 impressions, clicks or costs) and a set of control covariates $z_{c, t}$ (e.g.
 holidays, special events) we consider a linear model of the form $$ y_{t} =
 \alpha + \sum_{m=1}^{M}\beta_{m}f(x_{m, t}) + \sum_{c=1}^{C}\gamma_{c}z_{c, t}
 + \varepsilon_{t}, $$ where $\alpha$ is the intercept, $f$ is a media
 transformation function and $\varepsilon_{t}$ is the error therm which we
```

### Comparing `pymc-marketing-0.1.1/pymc_marketing/clv/distributions.py` & `pymc-marketing-0.2.0/pymc_marketing/clv/distributions.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,67 +15,54 @@
 class ContNonContractRV(RandomVariable):
     name = "continuous_non_contractual"
     ndim_supp = 1
     ndims_params = [0, 0, 0, 0]
     dtype = "floatX"
     _print_name = ("ContNonContract", "\\operatorname{ContNonContract}")
 
-    def make_node(self, rng, size, dtype, lam, p, T, T0):
+    def make_node(self, rng, size, dtype, lam, p, T):
         T = pt.as_tensor_variable(T)
-        T0 = pt.as_tensor_variable(T0)
 
-        return super().make_node(rng, size, dtype, lam, p, T, T0)
-
-    def __call__(self, lam, p, T, T0=0, size=None, **kwargs):
-        return super().__call__(lam, p, T, T0, size=size, **kwargs)
+        return super().make_node(rng, size, dtype, lam, p, T)
 
     @classmethod
-    def rng_fn(cls, rng, lam, p, T, T0, size) -> np.ndarray:
+    def rng_fn(cls, rng, lam, p, T, size):
         size = pm.distributions.shape_utils.to_tuple(size)
 
         # TODO: broadcast sizes
         lam = np.asarray(lam)
         p = np.asarray(p)
         T = np.asarray(T)
-        T0 = np.asarray(T0)
 
         if size == ():
-            size = np.broadcast_shapes(lam.shape, p.shape, T.shape, T0.shape)
+            size = np.broadcast_shapes(lam.shape, p.shape, T.shape)
 
         lam = np.broadcast_to(lam, size)
         p = np.broadcast_to(p, size)
         T = np.broadcast_to(T, size)
-        T0 = np.broadcast_to(T0, size)
-
-        output = np.zeros(shape=size + (2,))
 
-        # TODO: Optimize to work in a vectorized manner!
-        def sim_data(lam, p, T, T0):
-            t = T0
-            n = 0
+        x_1 = rng.poisson(lam * T)
+        x_2 = rng.geometric(p)
+        x = np.minimum(x_1, x_2)
 
-            while True:
-                wait = rng.exponential(scale=1 / lam)
-                dropout = rng.binomial(n=1, p=p)
+        nzp = x == 0  # nzp = non-zero purchases
 
-                if t + wait > T:
-                    break
-                else:
-                    t += wait
-                    n += 1
+        if x.shape == ():
+            if nzp:
+                return np.array([0, 0])
+            else:
+                return np.array([rng.beta(x, np.maximum(x_1 + 1 - x_2, 1)) * T, x])
 
-                    if dropout == 1:
-                        break
+        x[nzp] = 1.0  # temporary to avoid errors in rng.beta below
+        t_x = rng.beta(x, np.maximum(x_1 + 1 - x_2, 1)) * T
 
-            return np.array([t, n])
+        x[nzp] = 0.0
+        t_x[nzp] = 0.0
 
-        for index in np.ndindex(*size):
-            output[index] = sim_data(lam[index], p[index], T[index], T0[index])
-
-        return output
+        return np.stack([t_x, x], axis=-1)
 
     def _supp_shape_from_params(*args, **kwargs):
         return (2,)
 
 
 continuous_non_contractual = ContNonContractRV()
 
@@ -101,117 +88,106 @@
     .. [1] Fader, Peter S., Bruce GS Hardie, and Ka Lok Lee. "“Counting your customers”
            the easy way: An alternative to the Pareto/NBD model." Marketing science
            24.2 (2005): 275-284.
     """
     rv_op = continuous_non_contractual
 
     @classmethod
-    def dist(cls, lam, p, T, T0=0, **kwargs):
-        return super().dist([lam, p, T, T0], **kwargs)
+    def dist(cls, lam, p, T, **kwargs):
+        return super().dist([lam, p, T], **kwargs)
 
-    def logp(value, lam, p, T, T0):
+    def logp(value, lam, p, T):
         t_x = value[..., 0]
         x = value[..., 1]
 
         zero_observations = pt.eq(x, 0)
 
-        A = x * pt.log(1 - p) + x * pt.log(lam) - lam * (T - T0)
-        B = pt.log(p) + (x - 1) * pt.log(1 - p) + x * pt.log(lam) - lam * (t_x - T0)
+        A = x * pt.log(1 - p) + x * pt.log(lam) - lam * T
+        B = pt.log(p) + (x - 1) * pt.log(1 - p) + x * pt.log(lam) - lam * t_x
 
         logp = pt.switch(
             zero_observations,
             A,
             pt.logaddexp(A, B),
         )
 
         logp = pt.switch(
             pt.any(
                 (
-                    pt.lt(t_x, T0),
+                    pt.and_(pt.ge(t_x, 0), zero_observations),
+                    pt.lt(t_x, 0),
                     pt.lt(x, 0),
                     pt.gt(t_x, T),
                 ),
             ),
             -np.inf,
             logp,
         )
 
         return check_parameters(
             logp,
             lam > 0,
             0 <= p,
             p <= 1,
-            pt.all(T0 < T),
-            msg="lam > 0, 0 <= p <= 1, T0 < T",
+            msg="lam > 0, 0 <= p <= 1",
         )
 
 
 class ContContractRV(RandomVariable):
     name = "continuous_contractual"
     ndim_supp = 1
     ndims_params = [0, 0, 0, 0]
     dtype = "floatX"
     _print_name = ("ContinuousContractual", "\\operatorname{ContinuousContractual}")
 
-    def make_node(self, rng, size, dtype, lam, p, T, T0):
+    def make_node(self, rng, size, dtype, lam, p, T):
         T = pt.as_tensor_variable(T)
-        T0 = pt.as_tensor_variable(T0)
 
-        return super().make_node(rng, size, dtype, lam, p, T, T0)
+        return super().make_node(rng, size, dtype, lam, p, T)
 
-    def __call__(self, lam, p, T, T0=0, size=None, **kwargs):
-        return super().__call__(lam, p, T, T0, size=size, **kwargs)
+    def __call__(self, lam, p, T, size=None, **kwargs):
+        return super().__call__(lam, p, T, size=size, **kwargs)
 
     @classmethod
-    def rng_fn(cls, rng, lam, p, T, T0, size) -> np.ndarray:
+    def rng_fn(cls, rng, lam, p, T, size):
         size = pm.distributions.shape_utils.to_tuple(size)
 
         # To do: broadcast sizes
         lam = np.asarray(lam)
         p = np.asarray(p)
         T = np.asarray(T)
-        T0 = np.asarray(T0)
 
         if size == ():
-            size = np.broadcast_shapes(lam.shape, p.shape, T.shape, T0.shape)
+            size = np.broadcast_shapes(lam.shape, p.shape, T.shape)
 
         lam = np.broadcast_to(lam, size)
         p = np.broadcast_to(p, size)
         T = np.broadcast_to(T, size)
-        T0 = np.broadcast_to(T0, size)
 
-        output = np.zeros(shape=size + (3,))
+        x_1 = rng.poisson(lam * T)
+        x_2 = rng.geometric(p)
+        x = np.minimum(x_1, x_2)
+
+        nzp = x == 0  # nzp = non-zero purchases
+
+        if x.shape == ():
+            if nzp:
+                return np.array([0, 0, float(x_1 > x_2)])
+            else:
+                return np.array(
+                    [rng.beta(x, np.maximum(x_1 + 1 - x_2, 1)) * T, x, float(x_1 > x_2)]
+                )
 
-        def sim_data(lam, p, T, T0):
-            t = 0
-            n = 0
-
-            dropout = 0
-            while not dropout:
-                wait = rng.exponential(scale=1 / lam)
-                # If we didn't go into the future
-                if (t + wait) < T:
-                    n += 1
-                    t = t + wait
-                    dropout = rng.binomial(n=1, p=p)
-                else:
-                    break
-
-            return np.array(
-                [
-                    t,
-                    n,
-                    dropout,
-                ],
-            )
+        x[nzp] = 1.0  # temporary to avoid errors in rng.beta below
+        t_x = rng.beta(x, np.maximum(x_1 + 1 - x_2, 1)) * T
 
-        for index in np.ndindex(*size):
-            output[index] = sim_data(lam[index], p[index], T[index], T0[index])
+        x[nzp] = 0.0
+        t_x[nzp] = 0.0
 
-        return output
+        return np.stack([t_x, x, (x_1 > x_2).astype(float)], axis=-1)
 
     def _supp_shape_from_params(*args, **kwargs):
         return (3,)
 
 
 continuous_contractual = ContContractRV()
 
@@ -233,66 +209,64 @@
     Mean      :math:`\mathbb{E}[X(t) | \lambda, p, d] = \frac{1}{p} - \frac{1}{p}\exp\left(-\lambda p \min(t, T)\right)`
     ========  ===============================================
 
     """
     rv_op = continuous_contractual
 
     @classmethod
-    def dist(cls, lam, p, T, T0, **kwargs):
-        return super().dist([lam, p, T, T0], **kwargs)
+    def dist(cls, lam, p, T, **kwargs):
+        return super().dist([lam, p, T], **kwargs)
 
-    def logp(value, lam, p, T, T0):
+    def logp(value, lam, p, T):
         t_x = value[..., 0]
         x = value[..., 1]
         churn = value[..., 2]
 
         zero_observations = pt.eq(x, 0)
 
         logp = (x - 1) * pt.log(1 - p) + x * pt.log(lam) - lam * t_x
-        logp += churn * pt.log(p) + (1 - churn) * (
-            pt.log(1 - p) - lam * ((T - T0) - t_x)
-        )
+        logp += churn * pt.log(p) + (1 - churn) * (pt.log(1 - p) - lam * (T - t_x))
 
         logp = pt.switch(
             zero_observations,
-            -lam * (T - T0),
+            -lam * T,
             logp,
         )
 
         logp = pt.switch(
-            pt.any(pt.or_(pt.lt(t_x, 0), pt.lt(x, 0))),
+            pt.any(pt.or_(pt.lt(t_x, 0), zero_observations)),
             -np.inf,
             logp,
         )
         logp = pt.switch(
             pt.all(
                 pt.or_(pt.eq(churn, 0), pt.eq(churn, 1)),
             ),
             logp,
             -np.inf,
         )
         logp = pt.switch(
             pt.any(
                 (
-                    pt.lt(t_x, T0),
+                    pt.lt(t_x, 0),
                     pt.lt(x, 0),
                     pt.gt(t_x, T),
                 ),
             ),
             -np.inf,
             logp,
         )
 
         return check_parameters(
             logp,
             lam > 0,
             0 <= p,
             p <= 1,
-            pt.all(T0 < T),
-            msg="lam > 0, 0 <= p <= 1, T0 < T",
+            pt.all(0 < T),
+            msg="lam > 0, 0 <= p <= 1",
         )
 
 
 class ParetoNBDRV(RandomVariable):
     name = "pareto_nbd"
     ndim_supp = 1
     ndims_params = [0, 0, 0, 0, 0]
@@ -308,15 +282,15 @@
 
         return super().make_node(rng, size, dtype, r, alpha, s, beta, T)
 
     def __call__(self, r, alpha, s, beta, T, size=None, **kwargs):
         return super().__call__(r, alpha, s, beta, T, size=size, **kwargs)
 
     @classmethod
-    def rng_fn(cls, rng, r, alpha, s, beta, T, size) -> np.ndarray:
+    def rng_fn(cls, rng, r, alpha, s, beta, T, size):
         size = pm.distributions.shape_utils.to_tuple(size)
 
         r = np.asarray(r)
         alpha = np.asarray(alpha)
         s = np.asarray(s)
         beta = np.asarray(beta)
         T = np.asarray(T)
```

### Comparing `pymc-marketing-0.1.1/pymc_marketing/clv/models/beta_geo.py` & `pymc-marketing-0.2.0/pymc_marketing/clv/models/beta_geo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import Optional, Union
+from typing import Dict, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
 import pymc as pm
 import pytensor.tensor as pt
 import xarray as xr
 from pymc.distributions.dist_math import check_parameters
+from pymc.util import RandomState
 from pytensor.tensor import TensorVariable
 from scipy.special import expit, hyp2f1
 
 from pymc_marketing.clv.models.basic import CLVModel
 from pymc_marketing.clv.utils import to_xarray
 
 
@@ -28,52 +29,54 @@
 
     Methods below are adapted from the BetaGeoFitter class from the lifetimes package
     (see https://github.com/CamDavidsonPilon/lifetimes/).
 
 
     Parameters
     ----------
-    customer_id: array_like
-        Customer labels. Must not repeat.
-    frequency: array_like
-        The number of purchases of customers.
-    recency: array_like
-        The time of the last, i.e. xth, purchase.
-    T: array_like
-        The time of a customer's period under which they are under observation. By
-        construction of the model, T > t_x.
-    a_prior: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
-    b_prior: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
-    alpha_prior: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
-    r: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
+    data: pd.DataFrame
+        DataFrame containing the following columns:
+            * `frequency`: number of repeat purchases (with possible values 0, 1, 2, ...)
+            * `recency`: time between the first and the last purchase (with possible values 0, 1, 2, ...)
+            * `T`: time between the first purchase and the end of the observation period (with possible values 0, 1, 2, ...)
+            * `customer_id`: unique customer identifier
+    model_config: dict, optional
+        Dictionary of model prior parameters. If not provided, the model will use default priors specified in the `default_model_config` class attribute.
+    sampler_config: dict, optional
+        Dictionary of sampler parameters. Defaults to None.
 
     Examples
     --------
     BG/NBD model for customer
 
     .. code-block:: python
+
         import pymc as pm
         from pymc_marketing.clv import BetaGeoModel
 
         model = BetaGeoFitter(
-            frequency=[4, 0, 6, 3, ...],
-            recency=[30.73, 1.72, 0., 0., ...]
-            p_prior=pm.HalfNormal.dist(10),
-            q_prior=pm.HalfNormal.dist(10),
-            v_prior=pm.HalfNormal.dist(10),
+            data=pd.DataFrame({
+                "frequency"=[4, 0, 6, 3, ...],
+                "recency":[30.73, 1.72, 0., 0., ...]
+            }),
+            model_config={
+                "r": pm.Gamma.dist(alpha=0.1, beta=0.1),
+                "alpha": pm.Gamma.dist(alpha=0.1, beta=0.1),
+                "a": pm.Gamma.dist(alpha=0.1, beta=0.1),
+                "b": pm.Gamma.dist(alpha=0.1, beta=0.1),
+            },
+            sampler_config={
+                "draws": 1000,
+                "tune": 1000,
+                "chains": 2,
+                "cores": 2,
+                "nuts_kwargs": {"target_accept": 0.95},
+            },
         )
-
+        model.build_model()
         model.fit()
         print(model.fit_summary())
 
         # Estimating the expected number of purchases for a randomly chosen
         # individual in a future time period of length t
         expected_num_purchases = model.expected_num_purchases(
             t=[2, 5, 7, 10],
@@ -97,52 +100,74 @@
            P (alive) using the BG/NBD model. Research Note available via
            http://www.brucehardie.com/notes/021/palive_for_BGNBD.pdf.
     .. [3] Fader, P. S. & Hardie, B. G. (2013) Overcoming the BG/NBD Model’s #NUM!
            Error Problem. Research Note available via
            http://brucehardie.com/notes/027/bgnbd_num_error.pdf.
     """
 
-    _model_name = "BG/NBD"  # Beta-Geometric Negative Binomial Distribution
+    _model_type = "BG/NBD"  # Beta-Geometric Negative Binomial Distribution
 
     def __init__(
         self,
-        customer_id: Union[np.ndarray, pd.Series],
-        frequency: Union[np.ndarray, pd.Series, TensorVariable],
-        recency: Union[np.ndarray, pd.Series, TensorVariable],
-        T: Union[np.ndarray, pd.Series, TensorVariable],
-        a_prior: Optional[TensorVariable] = None,
-        b_prior: Optional[TensorVariable] = None,
-        alpha_prior: Optional[TensorVariable] = None,
-        r_prior: Optional[TensorVariable] = None,
+        data: pd.DataFrame,
+        model_config: Optional[Dict] = None,
+        sampler_config: Optional[Dict] = None,
     ):
-        super().__init__()
-
-        self.customer_id = customer_id
-        self.frequency = frequency
-        self.recency = recency
-        self.T = T
-
-        a_prior, b_prior, alpha_prior, r_prior = self._process_priors(
-            a_prior, b_prior, alpha_prior, r_prior
+        try:
+            self.customer_id = data["customer_id"]
+        except KeyError:
+            raise KeyError("customer_id column is missing from data")
+        try:
+            self.frequency = data["frequency"]
+        except KeyError:
+            raise KeyError("frequency column is missing from data")
+        try:
+            self.recency = data["recency"]
+        except KeyError:
+            raise KeyError("recency column is missing from data")
+        try:
+            self.T = data["T"]
+        except KeyError:
+            raise KeyError("T column is missing from data")
+        super().__init__(
+            model_config=model_config,
+            sampler_config=sampler_config,
         )
-
+        self.data = data
+        self.a_prior = self._create_distribution(self.model_config["a_prior"])
+        self.b_prior = self._create_distribution(self.model_config["b_prior"])
+        self.alpha_prior = self._create_distribution(self.model_config["alpha_prior"])
+        self.r_prior = self._create_distribution(self.model_config["r_prior"])
+        self._process_priors(self.a_prior, self.b_prior, self.alpha_prior, self.r_prior)
         # each customer's information should be encapsulated by a single data entry
-        if len(np.unique(customer_id)) != len(customer_id):
+        if len(np.unique(self.customer_id)) != len(self.customer_id):
             raise ValueError(
                 "The BetaGeoModel expects exactly one entry per customer. More than"
                 " one entry is currently provided per customer id."
             )
+        self.coords = {"customer_id": self.customer_id}
 
-        coords = {"customer_id": customer_id}
-        with pm.Model(coords=coords) as self.model:
-            a = self.model.register_rv(a_prior, name="a")
-            b = self.model.register_rv(b_prior, name="b")
+    @property
+    def default_model_config(self) -> Dict[str, Dict]:
+        return {
+            "a_prior": {"dist": "HalfFlat", "kwargs": {}},
+            "b_prior": {"dist": "HalfFlat", "kwargs": {}},
+            "alpha_prior": {"dist": "HalfFlat", "kwargs": {}},
+            "r_prior": {"dist": "HalfFlat", "kwargs": {}},
+        }
+
+    def build_model(
+        self,
+    ) -> None:
+        with pm.Model(coords=self.coords) as self.model:
+            a = self.model.register_rv(self.a_prior, name="a")
+            b = self.model.register_rv(self.b_prior, name="b")
 
-            alpha = self.model.register_rv(alpha_prior, name="alpha")
-            r = self.model.register_rv(r_prior, name="r")
+            alpha = self.model.register_rv(self.alpha_prior, name="alpha")
+            r = self.model.register_rv(self.r_prior, name="r")
 
             def logp(t_x, x, a, b, r, alpha, T):
                 """
                 The log-likelihood expression here aligns with expression (4) from [3]
                 due to the possible numerical instability of expression (3).
                 """
                 x_non_zero = x > 0
@@ -170,43 +195,27 @@
                     alpha > 0,
                     r > 0,
                     msg="a, b, alpha, r > 0",
                 )
 
             pm.Potential(
                 "likelihood",
-                logp(x=frequency, t_x=recency, a=a, b=b, alpha=alpha, r=r, T=T),
+                logp(
+                    x=self.frequency,
+                    t_x=self.recency,
+                    a=a,
+                    b=b,
+                    alpha=alpha,
+                    r=r,
+                    T=self.T,
+                ),
             )
 
-    def _process_priors(self, a_prior, b_prior, alpha_prior, r_prior):
-        # hyper priors for the Gamma params
-        if a_prior is None:
-            a_prior = pm.HalfFlat.dist()
-        else:
-            self._check_prior_ndim(a_prior)
-        if b_prior is None:
-            b_prior = pm.HalfFlat.dist()
-        else:
-            self._check_prior_ndim(b_prior)
-
-        # hyper priors for the Beta params
-        if alpha_prior is None:
-            alpha_prior = pm.HalfFlat.dist()
-        else:
-            self._check_prior_ndim(alpha_prior)
-        if r_prior is None:
-            r_prior = pm.HalfFlat.dist()
-        else:
-            self._check_prior_ndim(r_prior)
-
-        return super()._process_priors(a_prior, b_prior, alpha_prior, r_prior)
-
     def _unload_params(self):
-        trace = self.fit_result.posterior
-
+        trace = self.idata.posterior
         a = trace["a"]
         b = trace["b"]
         alpha = trace["alpha"]
         r = trace["r"]
 
         return a, b, alpha, r
 
@@ -340,7 +349,81 @@
         right_term = 1 - (alpha / (alpha + t)) ** r * hyp2f1(
             r, b, a + b - 1, t / (alpha + t)
         )
 
         return (left_term * right_term).transpose(
             "chain", "draw", "t", missing_dims="ignore"
         )
+
+    def _distribution_new_customers(
+        self,
+        random_seed: Optional[RandomState] = None,
+        var_names: Sequence[str] = ("population_dropout", "population_purchase_rate"),
+    ) -> xr.Dataset:
+        with pm.Model():
+            a = pm.HalfFlat("a")
+            b = pm.HalfFlat("b")
+            alpha = pm.HalfFlat("alpha")
+            r = pm.HalfFlat("r")
+
+            # This is the shape with fit_method="map"
+            if self.fit_result.dims == {"chain": 1, "draw": 1}:
+                shape_kwargs = {"shape": 1000}
+            else:
+                shape_kwargs = {}
+
+            pm.Beta("population_dropout", alpha=a, beta=b, **shape_kwargs)
+            pm.Gamma("population_purchase_rate", alpha=r, beta=alpha, **shape_kwargs)
+
+            return pm.sample_posterior_predictive(
+                self.fit_result,
+                var_names=var_names,
+                random_seed=random_seed,
+            ).posterior_predictive
+
+    def distribution_new_customer_dropout(
+        self,
+        random_seed: Optional[RandomState] = None,
+    ) -> xr.Dataset:
+        """Sample the Beta distribution for the population-level dropout rate.
+
+        This is the probability that a new customer will not make another purchase ("drops out")
+        immediately after any previous purchase.
+
+        Parameters
+        ----------
+        random_seed : RandomState, optional
+            Random state to use for sampling.
+
+        Returns
+        -------
+        xr.Dataset
+            Dataset containing the posterior samples for the population-level dropout rate.
+        """
+        return self._distribution_new_customers(
+            random_seed=random_seed,
+            var_names=["population_dropout"],
+        )["population_dropout"]
+
+    def distribution_new_customer_purchase_rate(
+        self,
+        random_seed: Optional[RandomState] = None,
+    ) -> xr.Dataset:
+        """Sample the Gamma distribution for the population-level purchase rate.
+
+        This is the purchase rate for a new customer and determines the time between
+        purchases for any new customer.
+
+        Parameters
+        ----------
+        random_seed : RandomState, optional
+            Random state to use for sampling.
+
+        Returns
+        -------
+        xr.Dataset
+            Dataset containing the posterior samples for the population-level purchase rate.
+        """
+        return self._distribution_new_customers(
+            random_seed=random_seed,
+            var_names=["population_purchase_rate"],
+        )["population_purchase_rate"]
```

### Comparing `pymc-marketing-0.1.1/pymc_marketing/clv/models/gamma_gamma.py` & `pymc-marketing-0.2.0/pymc_marketing/clv/models/gamma_gamma.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-from typing import Optional, Union
+from typing import Dict, Optional, Union
 
 import numpy as np
 import pandas as pd
 import pymc as pm
 import pytensor.tensor as pt
 import xarray
 from pymc.util import RandomState
 from pytensor.tensor import TensorVariable
 
 from pymc_marketing.clv.models.basic import CLVModel
 from pymc_marketing.clv.utils import customer_lifetime_value, to_xarray
 
 
 class BaseGammaGammaModel(CLVModel):
-    def _process_priors(self, p_prior, q_prior, v_prior):
-        if p_prior is None:
-            p_prior = pm.HalfFlat.dist()
-        else:
-            self._check_prior_ndim(p_prior)
-        if q_prior is None:
-            q_prior = pm.HalfFlat.dist()
-        else:
-            self._check_prior_ndim(q_prior)
-        if v_prior is None:
-            v_prior = pm.HalfFlat.dist()
-        else:
-            self._check_prior_ndim(v_prior)
-
-        return super()._process_priors(p_prior, q_prior, v_prior)
+    def __init__(
+        self,
+        data: pd.DataFrame,
+        model_config: Optional[Dict] = None,
+        sampler_config: Optional[Dict] = None,
+    ):
+        super().__init__(model_config, sampler_config)
+        self.data = data
+        self.p_prior = self._create_distribution(self.model_config["p_prior"])
+        self.q_prior = self._create_distribution(self.model_config["q_prior"])
+        self.v_prior = self._create_distribution(self.model_config["v_prior"])
+        self._process_priors(self.p_prior, self.q_prior, self.v_prior)
 
     def distribution_customer_spend(
         self,
         customer_id: Union[np.ndarray, pd.Series],
         mean_transaction_value: Union[np.ndarray, pd.Series, TensorVariable],
         frequency: Union[np.ndarray, pd.Series, TensorVariable],
         random_seed: Optional[RandomState] = None,
@@ -49,15 +46,15 @@
 
             # Closed form solution to the posterior of nu
             # Eq 5 from [1], p.3
             nu = pm.Gamma("nu", p * x + q, v + x * z_mean, dims=("customer_id",))
             pm.Deterministic("mean_spend", p / nu, dims=("customer_id",))
 
             return pm.sample_posterior_predictive(
-                self.fit_result,
+                self.idata,
                 var_names=["nu", "mean_spend"],
                 random_seed=random_seed,
             ).posterior_predictive["mean_spend"]
 
     def expected_customer_spend(
         self,
         customer_id: Union[np.ndarray, pd.Series],
@@ -71,17 +68,17 @@
         Adapted from: https://github.com/CamDavidsonPilon/lifetimes/blob/aae339c5437ec31717309ba0ec394427e19753c4/lifetimes/fitters/gamma_gamma_fitter.py#L117  # noqa: E501
         """
 
         mean_transaction_value, frequency = to_xarray(
             customer_id, mean_transaction_value, frequency
         )
 
-        p = self.fit_result.posterior["p"]
-        q = self.fit_result.posterior["q"]
-        v = self.fit_result.posterior["v"]
+        p = self.idata.posterior["p"]
+        q = self.idata.posterior["q"]
+        v = self.idata.posterior["v"]
 
         individual_weight = p * frequency / (p * frequency + q - 1)
         population_mean = v * p / (q - 1)
         return (
             1 - individual_weight
         ) * population_mean + individual_weight * mean_transaction_value
 
@@ -95,25 +92,25 @@
             q = pm.HalfFlat("q")
             v = pm.HalfFlat("v")
 
             nu = pm.Gamma("nu", q, v, dims=("new_customer_id",))
             pm.Deterministic("mean_spend", p / nu, dims=("new_customer_id",))
 
             return pm.sample_posterior_predictive(
-                self.fit_result,
+                self.idata,
                 var_names=["nu", "mean_spend"],
                 random_seed=random_seed,
             ).posterior_predictive["mean_spend"]
 
     def expected_new_customer_spend(self) -> xarray.DataArray:
         """Expected transaction value for a new customer"""
 
-        p_mean = self.fit_result.posterior["p"]
-        q_mean = self.fit_result.posterior["q"]
-        v_mean = self.fit_result.posterior["v"]
+        p_mean = self.idata.posterior["p"]
+        q_mean = self.idata.posterior["q"]
+        v_mean = self.idata.posterior["v"]
 
         # Closed form solution to the posterior of nu
         # Eq 3 from [1], p.3
         mean_spend = p_mean * v_mean / (q_mean - 1)
         # We could also provide the variance
         # var_spend = (p_mean ** 2 * v_mean ** 2) / ((q_mean - 1) ** 2 * (q_mean - 2))
 
@@ -167,48 +164,53 @@
     TODO: Explain assumptions of model
 
     Check `GammaGammaModelIndividual` for an equivalent model conditioned
     on individual transaction values.
 
     Parameters
     ----------
-    customer_id: array_like
-        Customer labels. Must not repeat.
-    mean_transaction_value: array_like
-        Mean transaction value of each customer.
-    frequency: array_like
-        Number of transactions observed for each customer.
-    p_prior: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
-    q_prior: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
-    v_prior: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
+    data: pd.DataFrame
+        DataFrame containing the following columns:
+            - customer_id: Customer labels. Must not repeat.
+            - mean_transaction_value: Mean transaction value of each customer.
+            - frequency: Number of transactions observed for each customer.
+    model_config: dict, optional
+        Dictionary of model prior parameters. If not provided, the model will use default priors specified in the `default_model_config` class attribute.
+    sampler_config: dict, optional
+        Dictionary of sampler parameters. Defaults to None.
 
     Examples
     --------
         Gamma-Gamma model condioned on mean transaction value
 
         .. code-block:: python
 
             import pymc as pm
             from pymc_marketing.clv import GammaGammaModel
 
             model = GammaGammaModel(
-                customer_id=[0, 1, 2, 3, ...],
-                mean_transactionn_value=[23.5, 19.3, 11.2, 100.5, ...],
-                frequency=[6, 8, 2, 1, ...],
-                p_prior=pm.HalfNormal.dist(10),
-                q_prior=pm.HalfNormal.dist(10),
-                v_prior=pm.HalfNormal.dist(10),
+                data=pd.DataFrame({
+                    "customer_id": [0, 1, 2, 3, ...],
+                    "mean_transactionn_value" :[23.5, 19.3, 11.2, 100.5, ...],
+                    "frequency": [6, 8, 2, 1, ...],
+                }),
+                model_config={
+                    "p_prior": {dist: 'HalfNorm', kwargs: {}},
+                    "q_prior": {dist: 'HalfStudentT', kwargs: {"nu": 4, "sigma": 10}},
+                    "v_prior": {dist: 'HalfCauchy', kwargs: {}},
+                },
+                sampler_config={
+                    "draws": 1000,
+                    "tune": 1000,
+                    "chains": 2,
+                    "cores": 2,
+                    "nuts_kwargs": {"target_accept": 0.95},
+                },
             )
-
+            model.build_model()
             model.fit()
             print(model.fit_summary())
 
             # Predict spend of customers for which we know transaction history, conditioned on data.
             expected_customer_spend = model.expected_customer_spend(
                 customer_id=[0, 1, 2, 3, ...],
                 mean_transactionn_value=[23.5, 19.3, 11.2, 100.5, ...],
@@ -226,38 +228,59 @@
            value. February, 2, 1-9. http://www.brucehardie.com/notes/025/gamma_gamma.pdf
     .. [2] Peter S. Fader, Bruce G. S. Hardie, and Ka Lok Lee (2005), “RFM and CLV:
            Using iso-value curves for customer base analysis”, Journal of Marketing
            Research, 42 (November), 415-430.
            https://journals.sagepub.com/doi/pdf/10.1509/jmkr.2005.42.4.415
     """
 
-    _model_name = "Gamma-Gamma Model (Mean Transactions)"
+    _model_type = "Gamma-Gamma Model (Mean Transactions)"
 
     def __init__(
         self,
-        customer_id: Union[np.ndarray, pd.Series],
-        mean_transaction_value: Union[np.ndarray, pd.Series, TensorVariable],
-        frequency: Union[np.ndarray, pd.Series, TensorVariable],
-        p_prior: Optional[TensorVariable] = None,
-        q_prior: Optional[TensorVariable] = None,
-        v_prior: Optional[TensorVariable] = None,
+        data: pd.DataFrame,
+        model_config: Optional[Dict] = None,
+        sampler_config: Optional[Dict] = None,
     ):
-        super().__init__()
-
-        p_prior, q_prior, v_prior = self._process_priors(p_prior, q_prior, v_prior)
+        try:
+            self.customer_id: Union[np.ndarray, pd.Series] = data["customer_id"]
+        except KeyError:
+            raise KeyError("data must contain a customer_id column")
+        try:
+            self.mean_transaction_value: Union[
+                np.ndarray, pd.Series, TensorVariable
+            ] = data["mean_transaction_value"]
+        except KeyError:
+            raise KeyError("data must contain a mean_transaction_value column")
+        try:
+            self.frequency: Union[np.ndarray, pd.Series, TensorVariable] = data[
+                "frequency"
+            ]
+        except KeyError:
+            raise KeyError("data must contain a frequency column")
+        super().__init__(
+            data=data, model_config=model_config, sampler_config=sampler_config
+        )
 
-        z_mean = pt.as_tensor_variable(mean_transaction_value)
-        x = pt.as_tensor_variable(frequency)
+        self.coords = {"customer_id": np.unique(self.customer_id)}
 
-        coords = {"customer_id": np.unique(customer_id)}
-        with pm.Model(coords=coords) as self.model:
-            p = self.model.register_rv(p_prior, name="p")
-            q = self.model.register_rv(q_prior, name="q")
-            v = self.model.register_rv(v_prior, name="v")
+    @property
+    def default_model_config(self) -> Dict:
+        return {
+            "p_prior": {"dist": "HalfFlat", "kwargs": {}},
+            "q_prior": {"dist": "HalfFlat", "kwargs": {}},
+            "v_prior": {"dist": "HalfFlat", "kwargs": {}},
+        }
 
+    def build_model(self):
+        z_mean = pt.as_tensor_variable(self.mean_transaction_value)
+        x = pt.as_tensor_variable(self.frequency)
+        with pm.Model(coords=self.coords) as self.model:
+            p = self.model.register_rv(self.p_prior, name="p")
+            q = self.model.register_rv(self.q_prior, name="q")
+            v = self.model.register_rv(self.v_prior, name="v")
             # Likelihood for mean_spend, marginalizing over nu
             # Eq 1a from [1], p.2
             pm.Potential(
                 "likelihood",
                 (
                     pt.gammaln(p * x + q)
                     - pt.gammaln(p * x)
@@ -281,45 +304,54 @@
     TODO: Explain assumptions of model
 
     Check `GammaGammaModel` for an equivalent model conditioned on the average
     transaction value of each user.
 
     Parameters
     ----------
-    customer_id: array_like
-        Customer labels. The same value should be used for each observation
+    data: pd.DataFrame
+        Dataframe containing the following columns:
+            - customer_id: Customer labels. The same value should be used for each observation
         coming from the same customer.
-    individual_transaction_value: array_like
-        Value of individual transactions.
-    p_prior: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
-    q_prior: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
-    v_prior: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
+            - individual_transaction_value: Value of individual transactions.
+    model_config: dict, optional
+        Dictionary of model prior parameters. If not provided, the model will use default priors specified in the `default_model_config` class attribute.
+    sampler_config: dict, optional
+        Dictionary of sampler parameters. Defaults to None.
 
 
     Examples
     --------
 
         Gamma-Gamma model conditioned on individual customer spend
 
         .. code-block:: python
 
             import pymc as pm
-            from pymc_marketing.clv import GammaGammaModel
+            from pymc_marketing.clv import GammaGammaModelIndividual
 
-            model = GammaGammaModel(
-                customer_id=[0, 0, 0, 1, 1, 2, ...],
-                individual_transaction_value=[5.3. 5.7, 6.9, 13.5, 0.3, 19.2 ...],
+            model = GammaGammaModelIndividual(
+                data=pd.DataFrame({
+                    "customer_id": [0, 0, 0, 1, 1, 2, ...],
+                    "individual_transaction_value": [5.3. 5.7, 6.9, 13.5, 0.3, 19.2 ...],
+                }),
+                model_config={
+                    "p_prior": {dist: 'HalfNorm', kwargs: {}},
+                    "q_prior": {dist: 'HalfStudentT', kwargs: {"nu": 4, "sigma": 10}},
+                    "v_prior": {dist: 'HalfCauchy', kwargs: {}},
+                },
+                sampler_config={
+                    "draws": 1000,
+                    "tune": 1000,
+                    "chains": 2,
+                    "cores": 2,
+                    "nuts_kwargs": {"target_accept": 0.95},
+                },
             )
-
+            model.build_model()
             model.fit()
             print(model.fit_summary())
 
             # Predict spend of customers for which we know transaction history,
             # conditioned on data. May include customers not included in fitting
             expected_customer_spend = model.expected_customer_spend(
                 customer_id=[0, 0, 0, 1, 1, 2, ...],
@@ -338,40 +370,58 @@
            value. February, 2, 1-9. http://www.brucehardie.com/notes/025/gamma_gamma.pdf
     .. [2] Peter S. Fader, Bruce G. S. Hardie, and Ka Lok Lee (2005), “RFM and CLV:
            Using iso-value curves for customer base analysis”, Journal of Marketing
            Research, 42 (November), 415-430.
            https://journals.sagepub.com/doi/pdf/10.1509/jmkr.2005.42.4.415
     """
 
-    _model_name = "Gamma-Gamma Model (Individual Transactions)"
+    _model_type = "Gamma-Gamma Model (Individual Transactions)"
 
     def __init__(
         self,
-        customer_id: Union[np.ndarray, pd.Series],
-        individual_transaction_value: Union[np.ndarray, pd.Series, TensorVariable],
-        p_prior: Optional[TensorVariable] = None,
-        q_prior: Optional[TensorVariable] = None,
-        v_prior: Optional[TensorVariable] = None,
+        data: pd.DataFrame,
+        model_config: Optional[Dict] = None,
+        sampler_config: Optional[Dict] = None,
     ):
-        super().__init__()
+        try:
+            self.customer_id: Union[np.ndarray, pd.Series] = data["customer_id"]
+        except KeyError:
+            raise KeyError("data must contain a 'customer_id' column")
+        try:
+            self.individual_transaction_value: Union[
+                np.ndarray, pd.Series, TensorVariable
+            ] = data["individual_transaction_value"]
+        except KeyError:
+            raise KeyError("data must contain a 'individual_transaction_value' column")
+        super().__init__(
+            data=data, model_config=model_config, sampler_config=sampler_config
+        )
+
+    @property
+    def default_model_config(self) -> Dict:
+        return {
+            "p_prior": {"dist": "HalfFlat", "kwargs": {}},
+            "q_prior": {"dist": "HalfFlat", "kwargs": {}},
+            "v_prior": {"dist": "HalfFlat", "kwargs": {}},
+        }
 
-        p_prior, q_prior, v_prior = self._process_priors(p_prior, q_prior, v_prior)
-        z = individual_transaction_value
+    def build_model(self):
+        z = self.individual_transaction_value
 
-        coords = {
-            "customer_id": np.unique(customer_id),
-            "obs": range(len(customer_id)),
+        self.coords = {
+            "customer_id": np.unique(self.customer_id),
+            "obs": range(len(self.customer_id)),
         }
-        with pm.Model(coords=coords) as self.model:
-            p = self.model.register_rv(p_prior, name="p")
-            q = self.model.register_rv(q_prior, name="q")
-            v = self.model.register_rv(v_prior, name="v")
+        with pm.Model(coords=self.coords) as self.model:
+            p = self.model.register_rv(self.p_prior, name="p")
+            q = self.model.register_rv(self.q_prior, name="q")
+            v = self.model.register_rv(self.v_prior, name="v")
 
             nu = pm.Gamma("nu", q, v, dims=("customer_id",))
-            pm.Gamma("spend", p, nu[customer_id], observed=z, dims=("obs",))
+            pm.Gamma("spend", p, nu[self.customer_id], observed=z, dims=("obs",))
 
     def _summarize_mean_data(self, customer_id, individual_transaction_value):
         df = pd.DataFrame(
             {
                 "customer_id": customer_id,
                 "individual_transaction_value": individual_transaction_value,
             }
```

### Comparing `pymc-marketing-0.1.1/pymc_marketing/clv/models/shifted_beta_geo.py` & `pymc-marketing-0.2.0/pymc_marketing/clv/models/shifted_beta_geo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Optional, Sequence, Union
+from typing import Dict, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
 import pymc as pm
 from pymc.util import RandomState
-from pytensor.tensor import TensorVariable
 from xarray import DataArray, Dataset
 
 from pymc_marketing.clv.models import CLVModel
 
 
 class ShiftedBetaGeoModelIndividual(CLVModel):
     """Shifted Beta Geometric model
@@ -20,43 +19,51 @@
       * The probability `theta` varies across customers according to a Beta prior distribution
         with hyperparameters `alpha` and `beta`.
 
     based on [1]_.
 
     Parameters
     ----------
-    customer_id: array_like
-        Customer labels. There should be one unique label for each customer
-    t_churn: array_like
-        Time at which the customer cancelled the contract (starting at 0).
+    data: pd.DataFrame
+        DataFrame containing the following columns:
+            * `customer_id`: Customer labels. There should be one unique label for each customer
+            * `t_churn`: Time at which the customer cancelled the contract (starting at 0).
         It should  equal T for users that have not cancelled by the end of the
         observation period
-    T: array_like
-        Maximum observed time period (starting at 0)
-    alpha_prior: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
-    beta_prior: scalar PyMC distribution, optional
-        PyMC prior distribution, created via `.dist()` API. Defaults to
-        `pm.HalfFlat.dist()`
+            * `T`: Maximum observed time period (starting at 0)
+    model_config: dict, optional
+        Dictionary of model prior parameters. If not provided, the model will use default priors specified in the `default_model_config` class attribute.
+    sampler_config: dict, optional
+        Dictionary of sampler parameters. Defaults to None.
 
 
     Examples
     --------
         .. code-block:: python
 
             import pymc as pm
             from pymc_marketing.clv import ShiftedBetaGeoModelIndividual
 
             model = ShiftedBetaGeoModelIndividual(
-                customer_id=[0, 1, 2, 3, ...],
-                t_churn=[1, 2, 8, 4, 8 ...],
-                T=8,  # Can also be an array with one value per customer
-                alpha_prior=pm.HalfNormal.dist(10),
-                beta_prior=pm.HalfNormal.dist(10),
+                data=pd.DataFrame({
+                    customer_id=[0, 1, 2, 3, ...],
+                    t_churn=[1, 2, 8, 4, 8 ...],
+                    T=[8 for x in range(len(customer_id))],
+                }),
+                model_config={
+                    "alpha_prior": {"dist": "HalfNormal", "kwargs": {"sigma": 10}},
+                    "beta_prior": {"dist": "HalfStudentT", "kwargs": {"nu": 4, "sigma": 10}},
+                },
+                sampler_config={
+                    "draws": 1000,
+                    "tune": 1000,
+                    "chains": 2,
+                    "cores": 2,
+                    "nuts_kwargs": {"target_accept": 0.95},
+                },
             )
 
             model.fit()
             print(model.fit_summary())
 
             # Predict how many periods in the future are existing customers
             likely to cancel (ignoring that some may already have cancelled)
@@ -73,67 +80,75 @@
     References
     ----------
     .. [1] Fader, P. S., & Hardie, B. G. (2007). How to project customer retention.
            Journal of Interactive Marketing, 21(1), 76-90.
            https://journals.sagepub.com/doi/pdf/10.1002/dir.20074
     """
 
-    _model_name = "Shifted-Beta-Geometric Model (Individual Customers)"
+    _model_type = "Shifted-Beta-Geometric Model (Individual Customers)"
 
     def __init__(
         self,
-        customer_id: Union[np.ndarray, pd.Series],
-        t_churn: Union[np.ndarray, pd.Series],
-        T: Union[np.ndarray, pd.Series],
-        alpha_prior: Optional[TensorVariable] = None,
-        beta_prior: Optional[TensorVariable] = None,
+        data: pd.DataFrame,
+        model_config: Optional[Dict] = None,
+        sampler_config: Optional[Dict] = None,
     ):
-        super().__init__()
-
-        t_churn = np.asarray(t_churn)
-        T = np.asarray(T)
-
-        if np.any((t_churn < 0) | (t_churn > T) | np.isnan(t_churn)):
+        try:
+            self.customer_id = data["customer_id"]
+        except KeyError:
+            raise KeyError("data must contain a 'customer_id' column")
+        try:
+            self.t_churn: np.ndarray = np.asarray(data["t_churn"])
+        except KeyError:
+            raise KeyError("data must contain a 't_churn' column")
+        try:
+            self.T: np.ndarray = np.asarray(data["T"])
+        except KeyError:
+            raise KeyError("data must contain a 'T' column")
+        super().__init__(model_config=model_config, sampler_config=sampler_config)
+        self.data = data
+        self.alpha_prior = self._create_distribution(self.model_config["alpha_prior"])
+        self.beta_prior = self._create_distribution(self.model_config["beta_prior"])
+        self._process_priors(self.alpha_prior, self.beta_prior)
+
+        if np.any(
+            (self.t_churn < 0) | (self.t_churn > self.T) | np.isnan(self.t_churn)
+        ):
             raise ValueError(
                 "t_churn must respect 0 < t_churn <= T.\n",
                 "Customers that are still alive should have t_churn = T",
             )
+        self.coords = {"customer_id": np.asarray(self.customer_id)}
 
-        alpha_prior, beta_prior = self._process_priors(alpha_prior, beta_prior)
+    @property
+    def default_model_config(self) -> Dict:
+        return {
+            "alpha_prior": {"dist": "HalfFlat", "kwargs": {}},
+            "beta_prior": {"dist": "HalfFlat", "kwargs": {}},
+        }
 
-        coords = {"customer_id": np.asarray(customer_id)}
-        with pm.Model(coords=coords) as self.model:
-            alpha = self.model.register_rv(alpha_prior, name="alpha")
-            beta = self.model.register_rv(beta_prior, name="beta")
+    def build_model(
+        self,
+    ) -> None:
+        with pm.Model(coords=self.coords) as self.model:
+            alpha = self.model.register_rv(self.alpha_prior, name="alpha")
+            beta = self.model.register_rv(self.beta_prior, name="beta")
 
             theta = pm.Beta("theta", alpha, beta, dims=("customer_id",))
 
             churn_raw = pm.Geometric.dist(theta)
-
             pm.Censored(
                 "churn_censored",
                 churn_raw,
                 lower=None,
-                upper=T,
-                observed=t_churn,
+                upper=self.T,
+                observed=self.t_churn,
                 dims=("customer_id",),
             )
 
-    def _process_priors(self, alpha_prior, beta_prior):
-        if alpha_prior is None:
-            alpha_prior = pm.HalfFlat.dist()
-        else:
-            self._check_prior_ndim(alpha_prior)
-        if beta_prior is None:
-            beta_prior = pm.HalfFlat.dist()
-        else:
-            self._check_prior_ndim(beta_prior)
-
-        return super()._process_priors(alpha_prior, beta_prior)
-
     def distribution_customer_churn_time(
         self, customer_id: Union[np.ndarray, pd.Series], random_seed: RandomState = None
     ) -> DataArray:
         """Sample distribution of churn time for existing customers.
 
         The draws represent the number of periods into the future after which
         a customer cancels their contract.
@@ -146,15 +161,15 @@
             alpha = pm.HalfFlat("alpha")
             beta = pm.HalfFlat("beta")
 
             theta = pm.Beta("theta", alpha, beta, dims=("customer_id",))
             pm.Geometric("churn", theta, dims=("customer_id",))
 
             return pm.sample_posterior_predictive(
-                self.fit_result,
+                self.idata,
                 var_names=["churn"],
                 random_seed=random_seed,
             ).posterior_predictive["churn"]
 
     def _distribution_new_customer(
         self,
         n: int = 1,
@@ -166,15 +181,15 @@
             alpha = pm.HalfFlat("alpha")
             beta = pm.HalfFlat("beta")
 
             theta = pm.Beta("theta", alpha, beta, dims=("new_customer_id",))
             pm.Geometric("churn", theta, dims=("new_customer_id",))
 
             return pm.sample_posterior_predictive(
-                self.fit_result,
+                self.idata,
                 var_names=var_names,
                 random_seed=random_seed,
             ).posterior_predictive
 
     def distribution_new_customer_churn_time(
         self, n: int = 1, random_seed: RandomState = None
     ) -> DataArray:
```

### Comparing `pymc-marketing-0.1.1/pymc_marketing/clv/plotting.py` & `pymc-marketing-0.2.0/pymc_marketing/clv/plotting.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.1/pymc_marketing/clv/utils.py` & `pymc-marketing-0.2.0/pymc_marketing/clv/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,17 +67,16 @@
     -------
     xarray
         DataArray with the estimated customer lifetime values
     """
 
     steps = np.arange(1, time + 1)
     factor = {"W": 4.345, "M": 1.0, "D": 30, "H": 30 * 24}[freq]
-
-    model_dims = transaction_model.fit_result.posterior.dims
-    model_coords = transaction_model.fit_result.posterior.coords
+    model_dims = transaction_model.idata.posterior.dims
+    model_coords = transaction_model.idata.posterior.coords
     clv_coords = {
         "chain": model_coords["chain"],
         "draw": model_coords["draw"],
         "customer_id": np.asarray(customer_id),
     }
     clv = xarray.DataArray(
         np.zeros((model_dims["chain"], model_dims["draw"], len(customer_id))),
```

### Comparing `pymc-marketing-0.1.1/pymc_marketing/mmm/base.py` & `pymc-marketing-0.2.0/pymc_marketing/mmm/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from abc import abstractmethod
 from inspect import (
     getattr_static,
     isdatadescriptor,
     isgetsetdescriptor,
     ismemberdescriptor,
     ismethoddescriptor,
 )
@@ -11,57 +10,49 @@
 import arviz as az
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mtick
 import numpy as np
 import pandas as pd
 import pymc as pm
 import seaborn as sns
-from pymc.util import RandomState
+from pymc_experimental.model_builder import ModelBuilder
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import FunctionTransformer
-from xarray import DataArray
+from xarray import DataArray, Dataset
 
 from pymc_marketing.mmm.validating import (
     ValidateChannelColumns,
     ValidateDateColumn,
     ValidateTargetColumn,
 )
 
 __all__ = ("BaseMMM", "MMM")
 
 
-class BaseMMM:
+class BaseMMM(ModelBuilder):
     model: pm.Model
+    _model_type = "BaseMMM"
+    version = "0.0.2"
 
     def __init__(
         self,
-        data: pd.DataFrame,
-        target_column: str,
         date_column: str,
         channel_columns: Union[List[str], Tuple[str]],
-        validate_data: bool = True,
+        model_config: Optional[Dict] = None,
+        sampler_config: Optional[Dict] = None,
         **kwargs,
     ) -> None:
-        self.data: pd.DataFrame = data
-        self.target_column: str = target_column
+        self.X: Optional[pd.DataFrame] = None
+        self.y: Optional[pd.Series] = None
         self.date_column: str = date_column
         self.channel_columns: Union[List[str], Tuple[str]] = channel_columns
-        self.n_obs: int = data.shape[0]
         self.n_channel: int = len(channel_columns)
         self._fit_result: Optional[az.InferenceData] = None
         self._posterior_predictive: Optional[az.InferenceData] = None
-
-        if validate_data:
-            self.validate(self.data)
-        self.preprocessed_data = self.preprocess(self.data.copy())
-
-        self.build_model(
-            data=self.preprocessed_data,
-            **kwargs,
-        )
+        super().__init__(model_config=model_config, sampler_config=sampler_config)
 
     @property
     def methods(self) -> List[Any]:
         maybe_methods = [getattr_static(self, attr) for attr in dir(self)]
         return [
             method
             for method in maybe_methods
@@ -71,181 +62,285 @@
                 or isdatadescriptor(method)
                 or isgetsetdescriptor(method)
                 or ismemberdescriptor(method)
             )
         ]
 
     @property
-    def validation_methods(self) -> List[Callable[["BaseMMM", pd.DataFrame], None]]:
-        return [
-            method
-            for method in self.methods
-            if getattr(method, "_tags", {}).get("validation", False)
-        ]
+    def validation_methods(
+        self,
+    ) -> Tuple[
+        List[Callable[["BaseMMM", Union[pd.DataFrame, pd.Series]], None]],
+        List[Callable[["BaseMMM", Union[pd.DataFrame, pd.Series]], None]],
+    ]:
+        """
+        A property that provides validation methods for features ("X") and the target variable ("y").
+
+        This property scans the methods of the object and returns those marked for validation.
+        The methods are marked by having a _tags dictionary attribute, with either "validation_X" or "validation_y" set to True.
+        The "validation_X" tag indicates a method used for validating features, and "validation_y" indicates a method used for validating the target variable.
+
+        Returns
+        -------
+        tuple of list of Callable[["BaseMMM", pd.DataFrame], None]
+            A tuple where the first element is a list of methods for "X" validation, and the second element is a list of methods for "y" validation.
+
+        """
+        return (
+            [
+                method
+                for method in self.methods
+                if getattr(method, "_tags", {}).get("validation_X", False)
+            ],
+            [
+                method
+                for method in self.methods
+                if getattr(method, "_tags", {}).get("validation_y", False)
+            ],
+        )
+
+    def validate(self, target: str, data: Union[pd.DataFrame, pd.Series]) -> None:
+        """
+        Validates the input data based on the specified target type.
+
+        This function loops over the validation methods specified for
+        the target type and applies them to the input data.
+
+        Parameters
+        ----------
+        target : str
+            The type of target to be validated.
+            Expected values are "X" for features and "y" for the target variable.
+        data : Union[pd.DataFrame, pd.Series]
+            The input data to be validated.
+
+        Raises
+        ------
+        ValueError
+            If the target type is not "X" or "y", a ValueError will be raised.
+        """
+        if target not in ["X", "y"]:
+            raise ValueError("Target must be either 'X' or 'y'")
+        if target == "X":
+            validation_methods = self.validation_methods[0]
+        elif target == "y":
+            validation_methods = self.validation_methods[1]
+
+        for method in validation_methods:
+            method(self, data)
 
     @property
     def preprocessing_methods(
         self,
-    ) -> List[Callable[["BaseMMM", pd.DataFrame], pd.DataFrame]]:
-        return [
-            method
-            for method in self.methods
-            if getattr(method, "_tags", {}).get("preprocessing", False)
-        ]
+    ) -> Tuple[
+        List[
+            Callable[
+                ["BaseMMM", Union[pd.DataFrame, pd.Series]],
+                Union[pd.DataFrame, pd.Series],
+            ]
+        ],
+        List[
+            Callable[
+                ["BaseMMM", Union[pd.DataFrame, pd.Series]],
+                Union[pd.DataFrame, pd.Series],
+            ]
+        ],
+    ]:
+        """
+        A property that provides preprocessing methods for features ("X") and the target variable ("y").
 
-    def get_target_transformer(self) -> Pipeline:
-        try:
-            return self.target_transformer  # type: ignore
-        except AttributeError:
-            identity_transformer = FunctionTransformer()
-            return Pipeline(steps=[("scaler", identity_transformer)])
+        This property scans the methods of the object and returns those marked for preprocessing.
+        The methods are marked by having a _tags dictionary attribute, with either "preprocessing_X" or "preprocessing_y" set to True.
+        The "preprocessing_X" tag indicates a method used for preprocessing features, and "preprocessing_y" indicates a method used for preprocessing the target variable.
 
-    def validate(self, data: pd.DataFrame):
-        for method in self.validation_methods:
-            method(self, data)
+        Returns
+        -------
+        tuple of list of Callable[["BaseMMM", pd.DataFrame], pd.DataFrame]
+            A tuple where the first element is a list of methods for "X" preprocessing, and the second element is a list of methods for "y" preprocessing.
+        """
+        return (
+            [
+                method
+                for method in self.methods
+                if getattr(method, "_tags", {}).get("preprocessing_X", False)
+            ],
+            [
+                method
+                for method in self.methods
+                if getattr(method, "_tags", {}).get("preprocessing_y", False)
+            ],
+        )
+
+    def preprocess(
+        self, target: str, data: Union[pd.DataFrame, pd.Series]
+    ) -> Union[pd.DataFrame, pd.Series]:
+        """
+        Preprocess the provided data according to the specified target.
 
-    def preprocess(self, data: pd.DataFrame) -> pd.DataFrame:
-        for method in self.preprocessing_methods:
-            data = method(self, data)
-        return data
+        This method applies preprocessing methods to the data ("X" or "y"), which are specified in the preprocessing_methods property of this object.
+        It iteratively applies each method in the appropriate list (either for "X" or "y") to the data.
+
+        Parameters
+        ----------
+        target : str
+            Indicates whether the data represents features ("X") or the target variable ("y").
 
-    @abstractmethod
-    def build_model(self, *args, **kwargs) -> None:
-        raise NotImplementedError()
+        data : pd.DataFrame
+            The data to be preprocessed.
 
-    def get_prior_predictive_data(self, *args, **kwargs) -> az.InferenceData:
+        Returns
+        -------
+        Union[pd.DataFrame, pd.Series]
+            The preprocessed data.
+
+        Raises
+        ------
+        ValueError
+            If the target is neither "X" nor "y".
+
+        Example
+        -------
+        >>> data = pd.DataFrame({"x1": [1, 2, 3], "y": [4, 5, 6]})
+        >>> self.preprocess("X", data)
+        """
+        if target == "X":
+            for method in self.preprocessing_methods[0]:
+                data = method(self, data)
+        elif target == "y":
+            for method in self.preprocessing_methods[1]:
+                data = method(self, data)
+        else:
+            raise ValueError("Target must be either 'X' or 'y'")
+        return data
+
+    def get_target_transformer(self) -> Pipeline:
         try:
-            return self._prior_predictive
+            return self.target_transformer  # type: ignore
         except AttributeError:
-            with self.model:
-                self._prior_predictive: az.InferenceData = pm.sample_prior_predictive(
-                    *args, **kwargs
-                )
-            return self._prior_predictive
+            identity_transformer = FunctionTransformer()
+            return Pipeline(steps=[("scaler", identity_transformer)])
 
-    def fit(
-        self,
-        progressbar: bool = True,
-        random_seed: RandomState = None,
-        *args: Any,
-        **kwargs: Any,
-    ) -> None:
-        with self.model:
-            self._fit_result = pm.sample(
-                progressbar=progressbar, random_seed=random_seed, *args, **kwargs
-            )
-            self._posterior_predictive = pm.sample_posterior_predictive(
-                trace=self._fit_result, progressbar=progressbar, random_seed=random_seed
-            )
+    @property
+    def prior_predictive(self) -> az.InferenceData:
+        if self.idata is None or "prior_predictive" not in self.idata:
+            raise RuntimeError("The model hasn't been fit yet, call .fit() first")
+        return self.idata["prior_predictive"]
 
     @property
-    def fit_result(self) -> az.InferenceData:
-        if self._fit_result is None:
+    def fit_result(self) -> Dataset:
+        if self.idata is None or "posterior" not in self.idata:
             raise RuntimeError("The model hasn't been fit yet, call .fit() first")
-        return self._fit_result
+        return self.idata["posterior"]
 
     @property
-    def posterior_predictive(self) -> az.InferenceData:
-        if self._posterior_predictive is None:
+    def posterior_predictive(self) -> Dataset:
+        if self.idata is None or "posterior_predictive" not in self.idata:
             raise RuntimeError("The model hasn't been fit yet, call .fit() first")
-        return self._posterior_predictive
+        return self.idata["posterior_predictive"]
 
     def plot_prior_predictive(
         self, samples: int = 1_000, **plt_kwargs: Any
     ) -> plt.Figure:
-        prior_predictive_data: az.InferenceData = self.get_prior_predictive_data(
-            samples=samples
-        )
+        prior_predictive_data: az.InferenceData = self.prior_predictive
 
-        likelihood_hdi_94: DataArray = az.hdi(
-            ary=prior_predictive_data["prior_predictive"], hdi_prob=0.94
-        )["likelihood"]
-        likelihood_hdi_50: DataArray = az.hdi(
-            ary=prior_predictive_data["prior_predictive"], hdi_prob=0.50
-        )["likelihood"]
+        likelihood_hdi_94: DataArray = az.hdi(ary=prior_predictive_data, hdi_prob=0.94)[
+            "likelihood"
+        ]
+        likelihood_hdi_50: DataArray = az.hdi(ary=prior_predictive_data, hdi_prob=0.50)[
+            "likelihood"
+        ]
 
         fig, ax = plt.subplots(**plt_kwargs)
+        if self.X is not None and self.y is not None:
+            ax.fill_between(
+                x=np.asarray(self.X[self.date_column]),
+                y1=likelihood_hdi_94[:, 0],
+                y2=likelihood_hdi_94[:, 1],
+                color="C0",
+                alpha=0.2,
+                label="94% HDI",
+            )
 
-        ax.fill_between(
-            x=self.data[self.date_column],
-            y1=likelihood_hdi_94[:, 0],
-            y2=likelihood_hdi_94[:, 1],
-            color="C0",
-            alpha=0.2,
-            label="94% HDI",
-        )
-
-        ax.fill_between(
-            x=self.data[self.date_column],
-            y1=likelihood_hdi_50[:, 0],
-            y2=likelihood_hdi_50[:, 1],
-            color="C0",
-            alpha=0.3,
-            label="50% HDI",
-        )
-
-        ax.plot(
-            self.data[self.date_column],
-            self.preprocessed_data[self.target_column],
-            color="black",
-        )
-        ax.set(title="Prior Predictive Check", xlabel="date", ylabel=self.target_column)
+            ax.fill_between(
+                x=np.asarray(self.X[self.date_column]),
+                y1=likelihood_hdi_50[:, 0],
+                y2=likelihood_hdi_50[:, 1],
+                color="C0",
+                alpha=0.3,
+                label="50% HDI",
+            )
+
+            ax.plot(
+                np.asarray(self.X[self.date_column]),
+                np.asarray(self.preprocessed_data["y"]),
+                color="black",
+            )
+            ax.set(
+                title="Prior Predictive Check", xlabel="date", ylabel=self.output_var
+            )
+        else:
+            raise RuntimeError(
+                "The model hasn't been fit yet, call .fit() first with X and y data."
+            )
         return fig
 
     def plot_posterior_predictive(
         self, original_scale: bool = False, **plt_kwargs: Any
     ) -> plt.Figure:
-        posterior_predictive_data: az.InferenceData = self.posterior_predictive
-
+        posterior_predictive_data: Dataset = self.posterior_predictive
         likelihood_hdi_94: DataArray = az.hdi(
-            ary=posterior_predictive_data["posterior_predictive"], hdi_prob=0.94
+            ary=posterior_predictive_data, hdi_prob=0.94
         )["likelihood"]
         likelihood_hdi_50: DataArray = az.hdi(
-            ary=posterior_predictive_data["posterior_predictive"], hdi_prob=0.50
+            ary=posterior_predictive_data, hdi_prob=0.50
         )["likelihood"]
 
         if original_scale:
             likelihood_hdi_94 = self.get_target_transformer().inverse_transform(
                 Xt=likelihood_hdi_94
             )
             likelihood_hdi_50 = self.get_target_transformer().inverse_transform(
                 Xt=likelihood_hdi_50
             )
 
         fig, ax = plt.subplots(**plt_kwargs)
+        if self.X is not None and self.y is not None:
+            ax.fill_between(
+                x=self.X[self.date_column],
+                y1=likelihood_hdi_94[:, 0],
+                y2=likelihood_hdi_94[:, 1],
+                color="C0",
+                alpha=0.2,
+                label="94% HDI",
+            )
 
-        ax.fill_between(
-            x=self.data[self.date_column],
-            y1=likelihood_hdi_94[:, 0],
-            y2=likelihood_hdi_94[:, 1],
-            color="C0",
-            alpha=0.2,
-            label="94% HDI",
-        )
-
-        ax.fill_between(
-            x=self.data[self.date_column],
-            y1=likelihood_hdi_50[:, 0],
-            y2=likelihood_hdi_50[:, 1],
-            color="C0",
-            alpha=0.3,
-            label="50% HDI",
-        )
-
-        target_to_plot: pd.Series = (
-            self.data[self.target_column]
-            if original_scale
-            else self.preprocessed_data[self.target_column]
-        )
-        ax.plot(self.data[self.date_column], target_to_plot, color="black")
-        ax.set(
-            title="Posterior Predictive Check",
-            xlabel="date",
-            ylabel=self.target_column,
-        )
+            ax.fill_between(
+                x=self.X[self.date_column],
+                y1=likelihood_hdi_50[:, 0],
+                y2=likelihood_hdi_50[:, 1],
+                color="C0",
+                alpha=0.3,
+                label="50% HDI",
+            )
+
+            target_to_plot: np.ndarray = np.asarray(
+                self.y if original_scale else self.preprocessed_data["y"]
+            )
+            ax.plot(
+                np.asarray(self.X[self.date_column]),
+                target_to_plot,
+                color="black",
+            )
+            ax.set(
+                title="Posterior Predictive Check",
+                xlabel="date",
+                ylabel=self.output_var,
+            )
+        else:
+            raise RuntimeError("The model hasn't been fit yet, call .fit() first")
         return fig
 
     def _format_model_contributions(self, var_contribution: str) -> DataArray:
         contributions = az.extract(
             self.fit_result,
             var_names=[var_contribution],
             combined=False,
@@ -286,60 +381,61 @@
                 [
                     "channel_contribution",
                     "control_contribution",
                     "fourier_contribution",
                 ],
             )
         ):
+            if self.X is not None:
+                ax.fill_between(
+                    x=self.X[self.date_column],
+                    y1=hdi.isel(hdi=0),
+                    y2=hdi.isel(hdi=1),
+                    color=f"C{i}",
+                    alpha=0.25,
+                    label=f"$94 %$ HDI ({var_contribution})",
+                )
+                ax.plot(
+                    np.asarray(self.X[self.date_column]),
+                    np.asarray(mean),
+                    color=f"C{i}",
+                )
+        if self.X is not None:
+            intercept = az.extract(
+                self.fit_result, var_names=["intercept"], combined=False
+            )
+            intercept_hdi = np.repeat(
+                a=az.hdi(intercept).intercept.data[None, ...],
+                repeats=self.X[self.date_column].shape[0],
+                axis=0,
+            )
+            ax.plot(
+                np.asarray(self.X[self.date_column]),
+                np.full(len(self.X[self.date_column]), intercept.mean().data),
+                color=f"C{i + 1}",
+            )
             ax.fill_between(
-                x=self.data[self.date_column],
-                y1=hdi.isel(hdi=0),
-                y2=hdi.isel(hdi=1),
-                color=f"C{i}",
+                x=self.X[self.date_column],
+                y1=intercept_hdi[:, 0],
+                y2=intercept_hdi[:, 1],
+                color=f"C{i + 1}",
                 alpha=0.25,
-                label=f"$94 %$ HDI ({var_contribution})",
+                label="$94 %$ HDI (intercept)",
+            )
+            ax.plot(
+                np.asarray(self.X[self.date_column]),
+                np.asarray(self.preprocessed_data["y"]),
+                color="black",
+            )
+            ax.legend(title="components", loc="center left", bbox_to_anchor=(1, 0.5))
+            ax.set(
+                title="Posterior Predictive Model Components",
+                xlabel="date",
+                ylabel=self.output_var,
             )
-            sns.lineplot(
-                x=self.data[self.date_column],
-                y=mean,
-                color=f"C{i}",
-                ax=ax,
-            )
-
-        intercept = az.extract(self.fit_result, var_names=["intercept"], combined=False)
-        intercept_hdi = np.repeat(
-            a=az.hdi(intercept).intercept.data[None, ...],
-            repeats=self.n_obs,
-            axis=0,
-        )
-        sns.lineplot(
-            x=self.data[self.date_column],
-            y=intercept.mean().data,
-            color=f"C{i + 1}",
-            ax=ax,
-        )
-        ax.fill_between(
-            x=self.data[self.date_column],
-            y1=intercept_hdi[:, 0],
-            y2=intercept_hdi[:, 1],
-            color=f"C{i + 1}",
-            alpha=0.25,
-            label="$94 %$ HDI (intercept)",
-        )
-        ax.plot(
-            self.data[self.date_column],
-            self.preprocessed_data[self.target_column],
-            color="black",
-        )
-        ax.legend(title="components", loc="center left", bbox_to_anchor=(1, 0.5))
-        ax.set(
-            title="Posterior Predictive Model Components",
-            xlabel="date",
-            ylabel=self.target_column,
-        )
         return fig
 
     def plot_channel_parameter(self, param_name: str, **plt_kwargs: Any) -> plt.Figure:
         if param_name not in ["alpha", "lam", "beta_channel"]:
             raise ValueError(f"Invalid parameter name: {param_name}")
 
         param_samples_df = pd.DataFrame(
@@ -372,43 +468,52 @@
                 ),
                 channel_contribution.shape,
             ),
             dims=channel_contribution.dims,
             coords=channel_contribution.coords,
         )
 
-    def plot_contribution_curves(self) -> plt.Figure:
+    def plot_direct_contribution_curves(self) -> plt.Figure:
+        """Plots the direct contribution curves. The term "direct" refers to the fact
+        we plots costs vs immediate returns and we do not take into account the lagged
+        effects of the channels e.g. adstock transformations.
+
+        Returns
+        -------
+        plt.Figure
+            Direct contribution curves.
+        """
         channel_contributions = self.compute_channel_contribution_original_scale().mean(
             ["chain", "draw"]
         )
-
         fig, axes = plt.subplots(
             nrows=self.n_channel,
             ncols=1,
             sharex=False,
             sharey=False,
             figsize=(12, 4 * self.n_channel),
             layout="constrained",
         )
 
         for i, channel in enumerate(self.channel_columns):
             ax = axes[i]
-            sns.regplot(
-                x=self.data[self.channel_columns].to_numpy()[:, i],
-                y=channel_contributions.sel(channel=channel),
-                color=f"C{i}",
-                order=2,
-                ci=None,
-                line_kws={
-                    "linestyle": "--",
-                    "alpha": 0.5,
-                    "label": "quadratic fit",
-                },
-                ax=ax,
-            )
+            if self.X is not None:
+                sns.regplot(
+                    x=self.X[self.channel_columns].to_numpy()[:, i],
+                    y=channel_contributions.sel(channel=channel),
+                    color=f"C{i}",
+                    order=2,
+                    ci=None,
+                    line_kws={
+                        "linestyle": "--",
+                        "alpha": 0.5,
+                        "label": "quadratic fit",
+                    },
+                    ax=ax,
+                )
             ax.legend(loc="upper left")
             ax.set(title=f"{channel}", xlabel="total_cost_eur")
 
         fig.suptitle("Contribution Plots", fontsize=16)
         return fig
 
     def compute_mean_contributions_over_time(
@@ -435,14 +540,15 @@
                 combined=True,
             )
             .mean("sample")
             .to_dataframe()
             .squeeze()
             .unstack()
         )
+        contributions_channel_over_time.columns = self.channel_columns
 
         if getattr(self, "control_columns", None):
             contributions_control_over_time = (
                 az.extract(
                     self.fit_result,
                     var_names=["control_contributions"],
                     combined=True,
@@ -494,14 +600,19 @@
             all_contributions_over_time = pd.DataFrame(
                 data=self.get_target_transformer().inverse_transform(
                     all_contributions_over_time
                 ),
                 columns=all_contributions_over_time.columns,
                 index=all_contributions_over_time.index,
             )
+            all_contributions_over_time.columns = (
+                all_contributions_over_time.columns.map(
+                    lambda x: f"channel_{x}" if isinstance(x, int) else x
+                )
+            )
         return all_contributions_over_time
 
     def plot_grouped_contribution_breakdown_over_time(
         self,
         stack_groups: Optional[Dict[str, List[str]]] = None,
         original_scale: bool = False,
         area_kwargs: Optional[Dict[str, Any]] = None,
```

### Comparing `pymc-marketing-0.1.1/pymc_marketing/mmm/preprocessing.py` & `pymc-marketing-0.2.0/pymc_marketing/mmm/preprocessing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 from typing import Any, Callable, List, Tuple, Union
 
 import pandas as pd
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import MaxAbsScaler, StandardScaler
 
 __all__ = [
-    "preprocessing_method",
+    "preprocessing_method_X",
+    "preprocessing_method_y",
     "MaxAbsScaleTarget",
     "MaxAbsScaleChannels",
     "StandardizeControls",
 ]
 
 
-def preprocessing_method(method: Callable) -> Callable:
+def preprocessing_method_X(method: Callable) -> Callable:
     if not hasattr(method, "_tags"):
         method._tags = {}  # type: ignore
-    method._tags["preprocessing"] = True  # type: ignore
+    method._tags["preprocessing_X"] = True  # type: ignore
+    return method
+
+
+def preprocessing_method_y(method: Callable) -> Callable:
+    if not hasattr(method, "_tags"):
+        method._tags = {}  # type: ignore
+    method._tags["preprocessing_y"] = True  # type: ignore
     return method
 
 
 class MaxAbsScaleTarget:
-    target_column: str
     target_transformer: Pipeline
 
-    @preprocessing_method
-    def max_abs_scale_target_data(self, data: pd.DataFrame) -> pd.DataFrame:
-        target_vector = data[self.target_column].to_numpy().reshape(-1, 1)
+    @preprocessing_method_y
+    def max_abs_scale_target_data(self, data: pd.Series) -> pd.Series:
+        target_vector = data.reshape(-1, 1)
         transformers = [("scaler", MaxAbsScaler())]
         pipeline = Pipeline(steps=transformers)
         self.target_transformer: Pipeline = pipeline.fit(X=target_vector)
-        data[self.target_column] = self.target_transformer.transform(
-            X=target_vector
-        ).flatten()
+        data = self.target_transformer.transform(X=target_vector).flatten()
         return data
 
 
 class MaxAbsScaleChannels:
     channel_columns: Union[List[str], Tuple[str]]
 
-    @preprocessing_method
+    @preprocessing_method_X
     def max_abs_scale_channel_data(self, data: pd.DataFrame) -> pd.DataFrame:
-        channel_data: Union[pd.DataFrame, pd.Series[Any]] = data[self.channel_columns]
+        channel_data: Union[
+            pd.DataFrame,
+            pd.Series[Any],
+        ] = data[self.channel_columns]
         transformers = [("scaler", MaxAbsScaler())]
         pipeline: Pipeline = Pipeline(steps=transformers)
         self.channel_transformer: Pipeline = pipeline.fit(X=channel_data.to_numpy())
         data[self.channel_columns] = self.channel_transformer.transform(
             channel_data.to_numpy()
         )
         return data
 
 
 class StandardizeControls:
     control_columns: List[str]  # TODO: Handle Optional[List[str]]
 
-    @preprocessing_method
+    @preprocessing_method_X
     def standardize_control_data(self, data: pd.DataFrame) -> pd.DataFrame:
         control_data: pd.DataFrame = data[self.control_columns]
         transformers = [("scaler", StandardScaler())]
         pipeline: Pipeline = Pipeline(steps=transformers)
         self.control_transformer: Pipeline = pipeline.fit(X=control_data.to_numpy())
         data[self.control_columns] = self.control_transformer.transform(
             control_data.to_numpy()
```

### Comparing `pymc-marketing-0.1.1/pymc_marketing/mmm/transformers.py` & `pymc-marketing-0.2.0/pymc_marketing/mmm/transformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from typing import Union
+
+import numpy as np
+import numpy.typing as npt
 import pytensor.tensor as pt
 from pytensor.tensor.random.utils import params_broadcast_shapes
 
 
 def batched_convolution(x, w, axis: int = 0):
     """Apply a 1D convolution in a vectorized way across multiple batch dimensions.
 
@@ -140,22 +144,21 @@
         pt.as_tensor(alpha)[..., None],
         (pt.arange(l_max, dtype=x.dtype) - pt.as_tensor(theta)[..., None]) ** 2,
     )
     w = w / pt.sum(w, axis=-1, keepdims=True) if normalize else w
     return batched_convolution(x, w, axis=axis)
 
 
-def logistic_saturation(x, lam: float = 0.5):
+def logistic_saturation(x, lam: Union[npt.NDArray[np.float_], float] = 0.5):
     """Logistic saturation transformation.
-
     Parameters
     ----------
     x : tensor
         Input tensor.
-    lam : float, optional, by default 0.5
+    lam : float or array-like, optional, by default 0.5
         Saturation parameter.
 
     Returns
     -------
     tensor
         Transformed tensor.
     """
```

### Comparing `pymc-marketing-0.1.1/pymc_marketing/mmm/utils.py` & `pymc-marketing-0.2.0/pymc_marketing/mmm/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.1/pymc_marketing/mmm/validating.py` & `pymc-marketing-0.2.0/pymc_marketing/mmm/validating.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 from typing import Callable, List, Optional, Tuple, Union
 
 import pandas as pd
 
 __all__ = [
-    "validation_method",
+    "validation_method_X",
+    "validation_method_y",
     "ValidateControlColumns",
     "ValidateTargetColumn",
     "ValidateDateColumn",
     "ValidateChannelColumns",
 ]
 
 
-def validation_method(method: Callable) -> Callable:
+def validation_method_y(method: Callable) -> Callable:
     if not hasattr(method, "_tags"):
         method._tags = {}  # type: ignore
-    method._tags["validation"] = True  # type: ignore
+    method._tags["validation_y"] = True  # type: ignore
     return method
 
 
-class ValidateTargetColumn:
-    target_column: str
+def validation_method_X(method: Callable) -> Callable:
+    if not hasattr(method, "_tags"):
+        method._tags = {}  # type: ignore
+    method._tags["validation_X"] = True  # type: ignore
+    return method
+
 
-    @validation_method
-    def validate_target(self, data: pd.DataFrame) -> None:
-        if self.target_column not in data.columns:
-            raise ValueError(f"target {self.target_column} not in data")
+class ValidateTargetColumn:
+    @validation_method_y
+    def validate_target(self, data: pd.Series) -> None:
+        if len(data) == 0:
+            raise ValueError("y must have at least one element")
 
 
 class ValidateDateColumn:
     date_column: str
 
-    @validation_method
+    @validation_method_X
     def validate_date_col(self, data: pd.DataFrame) -> None:
         if self.date_column not in data.columns:
             raise ValueError(f"date_col {self.date_column} not in data")
         if not data[self.date_column].is_unique:
             raise ValueError(f"date_col {self.date_column} has repeated values")
 
 
 class ValidateChannelColumns:
     channel_columns: Union[List[str], Tuple[str]]
 
-    @validation_method
+    @validation_method_X
     def validate_channel_columns(self, data: pd.DataFrame) -> None:
         if not isinstance(self.channel_columns, (list, tuple)):
             raise ValueError("channel_columns must be a list or tuple")
         if len(self.channel_columns) == 0:
             raise ValueError("channel_columns must not be empty")
         if not set(self.channel_columns).issubset(data.columns):
             raise ValueError(f"channel_columns {self.channel_columns} not in data")
@@ -58,15 +64,15 @@
                 f"channel_columns {self.channel_columns} contains negative values"
             )
 
 
 class ValidateControlColumns:
     control_columns: Optional[List[str]]
 
-    @validation_method
+    @validation_method_X
     def validate_control_columns(self, data: pd.DataFrame) -> None:
         if self.control_columns is None:
             return None
         if not isinstance(self.control_columns, (list, tuple)):
             raise ValueError("control_columns must be None, a list or tuple")
         if len(self.control_columns) == 0:
             raise ValueError(
```

### Comparing `pymc-marketing-0.1.1/pymc_marketing.egg-info/PKG-INFO` & `pymc-marketing-0.2.0/pymc_marketing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-marketing
-Version: 0.1.1
+Version: 0.2.0
 Summary: Marketing Statistical Models in PyMC
 Maintainer-email: PyMC Labs <info@pymc-labs.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,15 +202,15 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: repository, https://github.com/pymc-labs/pymc-marketing
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
 <div align="center">
@@ -237,20 +237,14 @@
 ```bash
 mamba create -c conda-forge -n marketing_env pymc-marketing
 mamba activate marketing_env
 ```
 
 See the official [PyMC installation guide](https://www.pymc.io/projects/docs/en/latest/installation.html) if more detail is needed.
 
-For testing purposes, if you wish to install the `main` branch directly from GitHub:
-
-```bash
-pip install git+https://github.com/pymc-labs/pymc-marketing.git
-```
-
 ## Bayesian Media Mix Models (MMMs) in PyMC
 
 In this package we provide an API for a Bayesian media mix model (MMM) specification following [Jin, Yuxue, et al. “Bayesian methods for media mix modeling with carryover and shape effects.” (2017).](https://research.google/pubs/pub46001/) Concretely, given a time series target variable $y_{t}$ (e.g. sales on conversions), media variables $x_{m, t}$ (e.g. impressions, clicks or costs) and a set of control covariates $z_{c, t}$ (e.g. holidays, special events) we consider a linear model of the form
 
 $$
 y_{t} = \alpha + \sum_{m=1}^{M}\beta_{m}f(x_{m, t}) +  \sum_{c=1}^{C}\gamma_{c}z_{c, t} + \varepsilon_{t},
 $$
```

### Comparing `pymc-marketing-0.1.1/pymc_marketing.egg-info/SOURCES.txt` & `pymc-marketing-0.2.0/pymc_marketing.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 pymc_marketing/clv/distributions.py
 pymc_marketing/clv/plotting.py
 pymc_marketing/clv/utils.py
 pymc_marketing/clv/models/__init__.py
 pymc_marketing/clv/models/basic.py
 pymc_marketing/clv/models/beta_geo.py
 pymc_marketing/clv/models/gamma_gamma.py
+pymc_marketing/clv/models/pareto_nbd.py
 pymc_marketing/clv/models/shifted_beta_geo.py
 pymc_marketing/mmm/__init__.py
 pymc_marketing/mmm/base.py
 pymc_marketing/mmm/delayed_saturated_mmm.py
 pymc_marketing/mmm/preprocessing.py
 pymc_marketing/mmm/transformers.py
 pymc_marketing/mmm/utils.py
```

### Comparing `pymc-marketing-0.1.1/pyproject.toml` & `pymc-marketing-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 
 [project]
 name = "pymc-marketing"
 description = "Marketing Statistical Models in PyMC"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 dynamic = ["version"]
 maintainers = [{ name = "PyMC Labs", email = "info@pymc-labs.io" }]
 
 dependencies = [
     "arviz>=0.13.0",
     "matplotlib>=3.5.1",
     "numpy>=1.17",
     "pandas",
     # NOTE: Keep minimum pymc version in sync with ci.yml `OLDEST_PYMC_VERSION`
-    "pymc>=5.3.0",
+    "pymc>=5.6.1,<5.7.0",
     "scikit-learn>=1.1.1",
     "seaborn>=0.12.2",
-    "xarray"
+    "xarray",
+    "xarray-einstats>=0.5.1",
+    "pymc-experimental==0.0.9",
 ]
 
 [project.optional-dependencies]
 docs = [
     "sphinx",
     "ipython!=8.7.0",
     "myst-parser",
@@ -77,8 +79,11 @@
     "-v",
     "--strict-markers",
     "--strict-config",
     "--cov=pymc_marketing",
     "--cov-report=term-missing",
     "--color=yes",
 ]
+filterwarnings = [
+    "ignore::DeprecationWarning:bokeh.core.property.primitive:37"
+]
 testpaths = "tests"
```

