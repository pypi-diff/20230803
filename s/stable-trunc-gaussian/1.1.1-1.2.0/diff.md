# Comparing `tmp/stable-trunc-gaussian-1.1.1.tar.gz` & `tmp/stable-trunc-gaussian-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-trunc-gaussian-1.1.1.tar", last modified: Mon Jul 31 20:15:45 2023, max compression
+gzip compressed data, was "stable-trunc-gaussian-1.2.0.tar", last modified: Wed Aug  2 23:48:15 2023, max compression
```

## Comparing `stable-trunc-gaussian-1.1.1.tar` & `stable-trunc-gaussian-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-31 20:15:45.093144 stable-trunc-gaussian-1.1.1/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     1078 2023-07-25 17:33:32.000000 stable-trunc-gaussian-1.1.1/LICENSE
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-25 18:10:36.000000 stable-trunc-gaussian-1.1.1/MANIFEST.in
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4842 2023-07-31 20:15:45.093144 stable-trunc-gaussian-1.1.1/PKG-INFO
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     2992 2023-07-31 20:08:29.000000 stable-trunc-gaussian-1.1.1/README.md
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      799 2023-07-31 19:53:28.000000 stable-trunc-gaussian-1.1.1/pyproject.toml
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-31 20:15:45.093144 stable-trunc-gaussian-1.1.1/setup.cfg
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-31 20:15:45.089144 stable-trunc-gaussian-1.1.1/src/
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-31 20:15:45.089144 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      213 2023-07-31 19:52:48.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/__init__.py
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)    10080 2023-07-31 20:08:29.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/parallel_trunc_gaussian.py
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     7429 2023-07-30 03:59:16.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/sequential_trunc_gaussian.py
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4095 2023-07-30 04:02:06.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/tests.py
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-31 20:15:45.093144 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4842 2023-07-31 20:15:45.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/PKG-INFO
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      469 2023-07-31 20:15:45.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/SOURCES.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)        1 2023-07-31 20:15:45.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/dependency_links.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       20 2023-07-31 20:15:45.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/requires.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       22 2023-07-31 20:15:45.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/top_level.txt
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-08-02 23:48:15.423095 stable-trunc-gaussian-1.2.0/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     1078 2023-07-25 17:33:32.000000 stable-trunc-gaussian-1.2.0/LICENSE
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-25 18:10:36.000000 stable-trunc-gaussian-1.2.0/MANIFEST.in
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4842 2023-08-02 23:48:15.423095 stable-trunc-gaussian-1.2.0/PKG-INFO
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     2992 2023-07-31 20:08:29.000000 stable-trunc-gaussian-1.2.0/README.md
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      799 2023-08-02 23:46:49.000000 stable-trunc-gaussian-1.2.0/pyproject.toml
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-08-02 23:48:15.423095 stable-trunc-gaussian-1.2.0/setup.cfg
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-08-02 23:48:15.419094 stable-trunc-gaussian-1.2.0/src/
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-08-02 23:48:15.423095 stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      213 2023-08-02 23:47:05.000000 stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian/__init__.py
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)    12723 2023-08-02 22:06:12.000000 stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian/parallel_trunc_gaussian.py
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     7429 2023-07-30 03:59:16.000000 stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian/sequential_trunc_gaussian.py
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     5666 2023-08-02 22:05:14.000000 stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian/tests.py
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-08-02 23:48:15.423095 stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian.egg-info/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4842 2023-08-02 23:48:15.000000 stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian.egg-info/PKG-INFO
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      469 2023-08-02 23:48:15.000000 stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian.egg-info/SOURCES.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)        1 2023-08-02 23:48:15.000000 stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian.egg-info/dependency_links.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       20 2023-08-02 23:48:15.000000 stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian.egg-info/requires.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       22 2023-08-02 23:48:15.000000 stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian.egg-info/top_level.txt
```

### Comparing `stable-trunc-gaussian-1.1.1/LICENSE` & `stable-trunc-gaussian-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-trunc-gaussian-1.1.1/PKG-INFO` & `stable-trunc-gaussian-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-trunc-gaussian
-Version: 1.1.1
+Version: 1.2.0
 Summary: A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch.
 Author-email: Carlos Núñez Molina <ccaarlos@ugr.es>
 License: MIT License
         
         Copyright (c) 2023 Carlos Núñez Molina
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stable-trunc-gaussian-1.1.1/README.md` & `stable-trunc-gaussian-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `stable-trunc-gaussian-1.1.1/pyproject.toml` & `stable-trunc-gaussian-1.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="stable-trunc-gaussian"
-version="1.1.1"
+version="1.2.0"
 description="A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch."
 readme="README.md"
 authors = [{ name = "Carlos Núñez Molina", email = "ccaarlos@ugr.es" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/parallel_trunc_gaussian.py` & `stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian/parallel_trunc_gaussian.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 ---- Stable Truncated Gaussian ----
 
 Implementation of truncated gaussian which results numerically stable even when the mu parameter is outside the
 interval [a,b] given by the bounds.
 In order to obtain this implementation, we have employed the formulas detailed on https://github.com/cossio/
 TruncatedNormal.jl/blob/23bfc7d0189ca6857e2e498006bbbed2a8b58be7/notes/normal.pdf
-
-Right now, we only implement the following methods: mean, variance and log_prob.
+Our implementation is also inspired by torch_truncnorm: https://github.com/toshas/torch_truncnorm/blob/main/TruncatedNormal.py#L40
 """
 
 import torch
-from torch.special import erf, erfc, erfcx
+from torch.special import erf, erfc, erfcx, erfinv
 from torch.distributions import Distribution, constraints
+from torch.distributions.kl import register_kl
 from torch import where
 import math
 
 # Constants
 SQRT_PI = math.sqrt(math.pi)
 SQRT_2 = math.sqrt(2)
 SQRT_2_PI = math.sqrt(2*math.pi)
@@ -23,19 +23,17 @@
 INV_SQRT_PI = 1/SQRT_PI
 INV_PI = 1/math.pi
 SQRT_2_DIV_SQRT_PI = SQRT_2 / SQRT_PI
 LOG_SQRT_2_PI = math.log(SQRT_2_PI)
 LOG_2 = math.log(2)
 
 
-EPS = torch.finfo(torch.float32).eps
-
 class ParallelTruncatedGaussian(Distribution):
 
-	has_rsample = False
+	has_rsample = True
 
 	arg_constraints = {
 		'mu': constraints.real,
 		'sigma': constraints.positive,
 		'a': constraints.real,
 		'b': constraints.real,
 	}
@@ -68,14 +66,18 @@
 
 		# Calculate the mean and var once and store them
 		self._mean = self._calculate_mean()
 		self._variance = self._calculate_variance()
 
 		# Calculate log(Z) = log(big_phi(beta)-big_phi(alpha))
 		self._log_Z = self._calculate_log_Z()
+		self._Z = torch.exp(self._log_Z)
+
+		# big_phi(alpha), used in the icdf (and rsample) methods
+		self._big_phi_alpha = self._big_phi(self._alpha)
 
 	# I override __repr__ because parameter names that appear in arg_constraints are of the form
 	# 'param' but instance attributes are of the form '_param' 
 	def __repr__(self) -> str:
 		param_names = [k for k, _ in self.arg_constraints.items() if '_'+k in self.__dict__]
 		args_string = ', '.join(['{}: {}'.format(p, self.__dict__['_'+p]
 								if self.__dict__['_'+p].numel() == 1
@@ -105,14 +107,22 @@
 	@property
 	def beta(self):
 		return self._beta
 	
 	# --- Auxiliary methods ---
 
 	@staticmethod
+	def _big_phi(x):
+		return 0.5*(1 + erf(INV_SQRT_2*x))
+
+	@staticmethod
+	def _inv_big_phi(x):
+		return SQRT_2 * erfinv(2*x-1)
+
+	@staticmethod
 	def _delta(x, y):
 		return torch.exp(x**2 - y**2)
 	
 	# Taylor expansion of F_1(x, eps=y-x)
 	@staticmethod
 	def _P_1(x, eps):
 		t0 = SQRT_PI*x
@@ -209,14 +219,16 @@
 		out4 = where(out4_cond, out4_m, 0)
 
 		# Add them up into a single tensor
 		final_out = out1 + out2 + out3 + out4
 
 		return final_out
 
+	# --- Main methods ---
+
 	# Numerically stable implementation of Z=log(big_phi(beta)-big_phi(alpha))
 	def _calculate_log_Z(self):
 		alpha, beta, mu, mean_d = self._alpha, self._beta, self._mu, self._mean.detach()
 
 		# Obtain masks
 		with torch.no_grad():
 			out1_cond = torch.logical_and(alpha>=0, beta>=0)
@@ -228,28 +240,34 @@
 		alpha2, beta2, mu2 = where(out2_cond, alpha, 1), where(out2_cond, beta, 0), where(out2_cond, mu, mean_d+1)
 		alpha3, beta3 = where(out3_cond, alpha, 0), where(out3_cond, beta, 1)
 
 		# Apply operations
 		out1_m = -torch.log( (self._mean-mu1) / self._sigma ) - LOG_SQRT_2_PI - (alpha1**2)/2 + \
 				torch.log(1 - torch.exp( (alpha1+beta1)*(alpha1-beta1) / 2 ))
 		out2_m = -torch.log( (mu2-self._mean) / self._sigma ) - LOG_SQRT_2_PI - (beta2**2)/2 + \
-			    torch.log(1 - torch.exp( (alpha2+beta2)*(beta2-alpha2) / 2))
+				torch.log(1 - torch.exp( (alpha2+beta2)*(beta2-alpha2) / 2))
 		out3_m = -LOG_2 + torch.log(erf(beta3*INV_SQRT_2) - erf(alpha3*INV_SQRT_2))
 
 		# Unmask tensors, by setting masked values to 0
 		out1 = where(out1_cond, out1_m, 0)
 		out2 = where(out2_cond, out2_m, 0)
 		out3 = where(out3_cond, out3_m, 0)
 
 		# Add them up into a single tensor
 		final_out = out1 + out2 + out3
 
 		return final_out	
 	
-	# --- Main methods ---
+	@property
+	def log_Z(self):
+		return self._log_Z
+
+	@property
+	def Z(self):
+		return self._Z
 
 	# Mean of the distribution (after truncation)
 	def _calculate_mean(self):
 		cls = self.__class__
 		fraction = SQRT_2_DIV_SQRT_PI * cls._F_1(self._alpha*INV_SQRT_2, self._beta*INV_SQRT_2)
 		result = self._mu + fraction*self._sigma
 
@@ -282,12 +300,66 @@
 
 		# x must be inside the interval [a, b]
 		if torch.any(x < self._a) or torch.any(x > self._b):
 			raise ValueError(f"parameter 'x' ({x}) is outside the [a={self._a}, b={self._b}] interval")
 
 		xi = (x-self._mu)/self._sigma
 		term_1 = -torch.log(self._sigma)
-		term_2 = -LOG_SQRT_2_PI - (xi**2)/2    
+		term_2 = -LOG_SQRT_2_PI - (xi**2)/2
 		term_3 = -self._log_Z
 		result = term_1 + term_2 + term_3
 
 		return result
+
+	# Inverse cumulative distribution function
+	def icdf(self, x):
+		return self._inv_big_phi( self._big_phi_alpha + x*self._Z )*self._sigma + self._mu
+
+	"""
+	From https://pytorch.org/docs/stable/distributions.html
+	Generates a sample_shape shaped reparameterized sample or sample_shape shaped batch of 
+	reparameterized samples if the distribution parameters are batched.
+	This sampling process is differentiable.
+	Current rsample implementation extracted from https://github.com/toshas/torch_truncnorm
+
+	Note: right now, the implementation of rsample is numerically unstable!!
+	"""
+	def rsample(self, sample_shape: torch.Size = torch.Size()):
+		shape = self._extended_shape(sample_shape)
+		
+		p = torch.empty(shape, device=self._mu.device).uniform_(0,1)
+		
+		return self.icdf(p)
+
+"""
+--- KL Divergence ---
+Function for calculating the KL divergence between two Truncated Gaussian distributions.
+
+We use the formulas detailed in the paper "Statistical Divergences between 
+Densities of Truncated Exponential Families with Nested Supports: Duo Bregman
+and Duo Jensen Divergences" by Frank Nielsen (see Eq. 111).
+
+Don't call this function directly. Instead, do the following:
+
+	from torch.distributions.kl import kl_divergence
+
+	...
+
+	value = kl_divergence(trunc_gauss_1, trunc_gauss_2)
+"""
+@register_kl(ParallelTruncatedGaussian, ParallelTruncatedGaussian)
+def kl_truncgauss_truncgauss(d1, d2):
+	mu1, sigma1, a1, b1, log_Z1, mean1, var1 = d1.mu, d1.sigma, d1.a, d1.b, d1.log_Z, d1.mean, d1.variance
+	mu2, sigma2, a2, b2, log_Z2, mean2, var2 = d2.mu, d2.sigma, d2.a, d2.b, d2.log_Z, d2.mean, d2.variance
+	inv_sqr_sigma1 = 1/(sigma1**2)
+	inv_sqr_sigma2 = 1/(sigma2**2)
+
+	# The interval [a1, b1] must be inside the interval [a2, b2]
+	# Otherwise, the KL divergence is infinite
+	if a1 < a2 or b1 > b2:
+		raise Exception(f"Interval [a1={a1}, b1={b1}] must be inside interval [a2={a2}, b2={b2}]. Otherwise, KL Divergence equals +inf.")
+
+	# Calculate KL(d1 || d2)
+	kl_divergence = 0.5*mu2*inv_sqr_sigma2 - 0.5*mu1*inv_sqr_sigma1 + torch.log(sigma2/sigma1) + log_Z2 - log_Z1 - \
+					(mu2*inv_sqr_sigma2 - mu1*inv_sqr_sigma1)*mean1 - (0.5*inv_sqr_sigma1 - 0.5*inv_sqr_sigma2)*(var1+mean1**2)
+
+	return kl_divergence
```

### Comparing `stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/sequential_trunc_gaussian.py` & `stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian/sequential_trunc_gaussian.py`

 * *Files identical despite different names*

### Comparing `stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/tests.py` & `stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian/tests.py`

 * *Files 22% similar despite different names*

```diff
@@ -96,14 +96,55 @@
     [-999,-999.5,1,-1000,-999],
     [-1000,-999,1,-1000,-999],
     [-999.1,-1000,1,-1000,-999],
     [-999.999,-3.5,1,-1000,-999],
     [-999.45,-1130.8,1,-1000,-999]
 ]
 
+# Values for testing the icdf (and, thus, rsample)
+# In order: percentile, mu, sigma, a, b
+icdf_values = [
+    [0,0,1,-1,1],
+    [0.5,-1,1,-1,1],
+    [1,-10,1,-1,1],
+    [0.2,1,1,-1,1],
+    [0.01,10,1,-1,1],
+    [0.99,10,100,-1,1],
+    [0.3894,10,0.01,-1,1],
+
+    [0.1,2.5,1,2,3],
+    [0.2,2,1,2,3],
+    [0.3,3,1,2,3],
+    [0.4,0,1,2,3],
+    [0.5,-100,1,2,3],
+    [0.6,100,1,2,3],
+    [0.7,100,0.01,2,3],
+    [0.8,100,100,2,3],
+
+    [0.9,20,1,20,2000],
+    [1,2000,1,20,2000],
+    [0.9999,30,1,20,2000],
+    [0.0001,1990,1,20,2000],
+    [0.99999,10000,1,20,2000],
+    [0.00001,-10000,1,20,2000],
+    [0.4598,-10000,100,20,2000],
+
+    [0.1992,999.5,1,999,1000],
+    [0.1446,999,1,999,1000],
+    [0.78913,1000,1,999,1000],
+    [0.4113,3.5,1,999,1000],
+    [0.1617,1130.8,1,999,1000],
+
+    [0.0146,-999.5,1,-1000,-999],
+    [0.981616,-999,1,-1000,-999],
+    [0.16464,-1000,1,-1000,-999],
+    [0.89131,-3.5,1,-1000,-999],
+    [0.16566,-1130.8,1,-1000,-999]
+]
+
 # Returns the mean obtained with scipy and then the mean obtained with my code
 def calculate_mean(mu, sigma, a, b):
     m1 = TG(t(mu), t(sigma), t(a), t(b)).mean
 
     a_, b_ = (a - mu) / sigma, (b - mu) / sigma
     m2 = truncnorm.mean(a=a_, b=b_, loc=mu, scale=sigma)
 
@@ -121,14 +162,22 @@
     p1 = TG(t(mu), t(sigma), t(a), t(b)).log_prob(t(x))
 
     a_, b_ = (a - mu) / sigma, (b - mu) / sigma
     p2 = truncnorm.logpdf(x, a=a_, b=b_, loc=mu, scale=sigma)
 
     return p2, p1
 
+def calculate_icdf(percentile, mu, sigma, a, b):
+    icdf1 = TG(t(mu), t(sigma), t(a), t(b)).icdf(t(percentile))
+
+    a_, b_ = (a - mu) / sigma, (b - mu) / sigma
+    icdf2 = truncnorm.ppf(q=percentile, a=a_, b=b_, loc=mu, scale=sigma)
+
+    return icdf2, icdf1
+
 def check_mean_and_var():
     for mu, sigma, a, b in mean_and_val_values:
         t_mean, p_mean = calculate_mean(mu, sigma, a, b)
         t_var, p_var = calculate_var(mu, sigma, a, b)
 
         if not math.isclose(t_mean, p_mean, rel_tol=REL_TOL):
             print(f"Different means - Scipy:{t_mean}, TN:{p_mean} - mu:{mu}, sigma:{sigma}, a:{a}, b:{b}")
@@ -139,10 +188,18 @@
 def check_log_prob():
     for x, mu, sigma, a, b in log_prob_values:
         t_p, p_p = calculate_log_prob(x, mu, sigma, a, b)
 
         if not math.isclose(t_p, p_p, rel_tol=REL_TOL):
             print(f"Different log probs - Scipy:{t_p}, TN:{p_p} - x:{x}, mu:{mu}, sigma:{sigma}, a:{a}, b:{b}")
 
+def check_icdf():
+    for percentile, mu, sigma, a, b in icdf_values:
+        t_icdf, p_icdf = calculate_icdf(percentile, mu, sigma, a, b)
+
+        if not math.isclose(t_icdf, p_icdf, rel_tol=REL_TOL):
+            print(f"Different icdfs - Scipy:{t_icdf}, TN:{p_icdf} - percentile:{percentile}, mu:{mu}, sigma:{sigma}, a:{a}, b:{b}")
+
 if __name__ == '__main__':
-    check_mean_and_var()
-    check_log_prob()
+    #check_mean_and_var()
+    #check_log_prob()
+    check_icdf()
```

### Comparing `stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/PKG-INFO` & `stable-trunc-gaussian-1.2.0/src/stable_trunc_gaussian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-trunc-gaussian
-Version: 1.1.1
+Version: 1.2.0
 Summary: A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch.
 Author-email: Carlos Núñez Molina <ccaarlos@ugr.es>
 License: MIT License
         
         Copyright (c) 2023 Carlos Núñez Molina
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

