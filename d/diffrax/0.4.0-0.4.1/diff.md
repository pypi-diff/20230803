# Comparing `tmp/diffrax-0.4.0.tar.gz` & `tmp/diffrax-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffrax-0.4.0.tar", last modified: Mon May 22 14:23:00 2023, max compression
+gzip compressed data, was "diffrax-0.4.1.tar", last modified: Thu Aug  3 19:27:46 2023, max compression
```

## Comparing `diffrax-0.4.0.tar` & `diffrax-0.4.1.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.527938 diffrax-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 14:22:55.000000 diffrax-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 14:22:55.000000 diffrax-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-22 14:23:00.527938 diffrax-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-22 14:22:55.000000 diffrax-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.519939 diffrax-0.4.0/diffrax/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    27893 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/autocitation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.519939 diffrax-0.4.0/diffrax/brownian/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/brownian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/brownian/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/brownian/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/brownian/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/global_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31501 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/local_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.523939 diffrax-0.4.0/diffrax/nonlinear_solver/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/nonlinear_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/nonlinear_solver/affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/nonlinear_solver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/nonlinear_solver/newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/saveat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.523939 diffrax-0.4.0/diffrax/solver/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/bosh3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/dopri5.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/dopri8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/euler_heun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/heun.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/implicit_euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kencarp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kencarp4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kencarp5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kvaerno3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kvaerno4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/kvaerno5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/leapfrog_midpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/midpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/milstein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/ralston.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/reversible_heun.py
--rw-r--r--   0 runner    (1001) docker     (123)    45338 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/runge_kutta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/semi_implicit_euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/sil3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/solver/tsit5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.523939 diffrax-0.4.0/diffrax/step_size_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/step_size_controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28338 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/step_size_controller/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/step_size_controller/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/step_size_controller/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-05-22 14:22:55.000000 diffrax-0.4.0/diffrax/term.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.519939 diffrax-0.4.0/diffrax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 14:23:00.000000 diffrax-0.4.0/diffrax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:23:00.527938 diffrax-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-22 14:22:56.000000 diffrax-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:00.523939 diffrax-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_adaptive_stepsize_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_brownian.py
--rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_detest.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_global_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_local_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_newton_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_saveat_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_step_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-22 14:22:56.000000 diffrax-0.4.0/test/test_vmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:27:46.050192 diffrax-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 19:27:41.000000 diffrax-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 19:27:41.000000 diffrax-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-08-03 19:27:46.050192 diffrax-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-03 19:27:41.000000 diffrax-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:27:46.042191 diffrax-0.4.1/diffrax/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28215 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/autocitation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:27:46.042191 diffrax-0.4.1/diffrax/brownian/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/brownian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/brownian/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/brownian/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/brownian/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/global_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32942 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/local_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:27:46.042191 diffrax-0.4.1/diffrax/nonlinear_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/nonlinear_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/nonlinear_solver/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/nonlinear_solver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/nonlinear_solver/newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/saveat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:27:46.046192 diffrax-0.4.1/diffrax/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/bosh3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/dopri5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/dopri8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/euler_heun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/heun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/implicit_euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/kencarp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/kencarp4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/kencarp5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/kvaerno3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/kvaerno4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/kvaerno5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/leapfrog_midpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/midpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/milstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/ralston.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/reversible_heun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47205 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/runge_kutta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/semi_implicit_euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/sil3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/solver/tsit5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:27:46.046192 diffrax-0.4.1/diffrax/step_size_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/step_size_controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28338 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/step_size_controller/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/step_size_controller/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/step_size_controller/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-08-03 19:27:41.000000 diffrax-0.4.1/diffrax/term.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:27:46.042191 diffrax-0.4.1/diffrax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-08-03 19:27:46.000000 diffrax-0.4.1/diffrax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-03 19:27:46.000000 diffrax-0.4.1/diffrax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:27:46.000000 diffrax-0.4.1/diffrax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:27:46.000000 diffrax-0.4.1/diffrax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-03 19:27:46.000000 diffrax-0.4.1/diffrax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 19:27:46.000000 diffrax-0.4.1/diffrax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 19:27:46.050192 diffrax-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-03 19:27:41.000000 diffrax-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:27:46.050192 diffrax-0.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_adaptive_stepsize_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_brownian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_detest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_global_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_local_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_newton_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_saveat_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_step_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-08-03 19:27:41.000000 diffrax-0.4.1/test/test_vmap.py
```

### Comparing `diffrax-0.4.0/LICENSE` & `diffrax-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/PKG-INFO` & `diffrax-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffrax
-Version: 0.4.0
+Version: 0.4.1
 Summary: GPU+autodiff-capable ODE/SDE/CDE solvers written in JAX.
 Home-page: https://github.com/patrick-kidger/diffrax
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
@@ -42,15 +42,15 @@
 
 ## Installation
 
 ```
 pip install diffrax
 ```
 
-Requires Python 3.9+, JAX 0.4.4+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.4+.
+Requires Python 3.9+, JAX 0.4.13+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.11+.
 
 ## Documentation
 
 Available at [https://docs.kidger.site/diffrax](https://docs.kidger.site/diffrax).
 
 ## Quick example
 
@@ -80,16 +80,22 @@
     year={2021},
     school={University of Oxford},
 }
 ```
 
 (Also consider starring the project on GitHub.)
 
-## See also
+## See also: other libraries in the JAX ecosystem
 
-Neural networks: [Equinox](https://github.com/patrick-kidger/equinox).
+[Equinox](https://github.com/patrick-kidger/equinox): neural networks.
 
-Type annotations and runtime checking for PyTrees and shape/dtype of JAX arrays: [jaxtyping](https://github.com/google/jaxtyping).
+[Optax](https://github.com/deepmind/optax): first-order gradient (SGD, Adam, ...) optimisers.
 
-Computer vision models: [Eqxvision](https://github.com/paganpasta/eqxvision).
+[Lineax](https://github.com/google/lineax): linear solvers and linear least squares.
 
-SymPy<->JAX conversion; train symbolic expressions via gradient descent: [sympy2jax](https://github.com/google/sympy2jax).
+[jaxtyping](https://github.com/google/jaxtyping): type annotations for shape/dtype of arrays.
+
+[Eqxvision](https://github.com/paganpasta/eqxvision): computer vision models.
+
+[sympy2jax](https://github.com/google/sympy2jax): SymPy<->JAX conversion; train symbolic expressions via gradient descent.
+
+[Levanter](https://github.com/stanford-crfm/levanter): scalable+reliable training of foundation models (e.g. LLMs).
```

### Comparing `diffrax-0.4.0/README.md` & `diffrax-0.4.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ## Installation
 
 ```
 pip install diffrax
 ```
 
-Requires Python 3.9+, JAX 0.4.4+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.4+.
+Requires Python 3.9+, JAX 0.4.13+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.11+.
 
 ## Documentation
 
 Available at [https://docs.kidger.site/diffrax](https://docs.kidger.site/diffrax).
 
 ## Quick example
 
@@ -55,16 +55,22 @@
     year={2021},
     school={University of Oxford},
 }
 ```
 
 (Also consider starring the project on GitHub.)
 
-## See also
+## See also: other libraries in the JAX ecosystem
 
-Neural networks: [Equinox](https://github.com/patrick-kidger/equinox).
+[Equinox](https://github.com/patrick-kidger/equinox): neural networks.
 
-Type annotations and runtime checking for PyTrees and shape/dtype of JAX arrays: [jaxtyping](https://github.com/google/jaxtyping).
+[Optax](https://github.com/deepmind/optax): first-order gradient (SGD, Adam, ...) optimisers.
 
-Computer vision models: [Eqxvision](https://github.com/paganpasta/eqxvision).
+[Lineax](https://github.com/google/lineax): linear solvers and linear least squares.
 
-SymPy<->JAX conversion; train symbolic expressions via gradient descent: [sympy2jax](https://github.com/google/sympy2jax).
+[jaxtyping](https://github.com/google/jaxtyping): type annotations for shape/dtype of arrays.
+
+[Eqxvision](https://github.com/paganpasta/eqxvision): computer vision models.
+
+[sympy2jax](https://github.com/google/sympy2jax): SymPy<->JAX conversion; train symbolic expressions via gradient descent.
+
+[Levanter](https://github.com/stanford-crfm/levanter): scalable+reliable training of foundation models (e.g. LLMs).
```

### Comparing `diffrax-0.4.0/diffrax/__init__.py` & `diffrax-0.4.1/diffrax/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,8 +89,8 @@
     ControlTerm,
     MultiTerm,
     ODETerm,
     WeaklyDiagonalControlTerm,
 )
 
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `diffrax-0.4.0/diffrax/ad.py` & `diffrax-0.4.1/diffrax/ad.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/adjoint.py` & `diffrax-0.4.1/diffrax/adjoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,26 +489,37 @@
         init_state=init_state,
         inner_while_loop=ft.partial(_inner_loop, kind="lax"),
         outer_while_loop=ft.partial(_outer_loop, kind="lax"),
         **kwargs,
     )
 
 
-def _loop_backsolve_fwd(y__args__terms, **kwargs):
+@_loop_backsolve.def_fwd
+def _loop_backsolve_fwd(perturbed, y__args__terms, **kwargs):
+    del perturbed
     final_state, aux_stats = _loop_backsolve(y__args__terms, **kwargs)
     # Note that `final_state.save_state` has type `PyTree[SaveState]`; here we are
     # relying on the guard in `BacksolveAdjoint` that it have trivial structure.
     ts = final_state.save_state.ts
     ys = final_state.save_state.ys
     return (final_state, aux_stats), (ts, ys)
 
 
+def _materialise_none(y, grad_y):
+    if grad_y is None and eqx.is_inexact_array(y):
+        return jnp.zeros_like(y)
+    else:
+        return grad_y
+
+
+@_loop_backsolve.def_bwd
 def _loop_backsolve_bwd(
     residuals,
     grad_final_state__aux_stats,
+    perturbed,
     y__args__terms,
     *,
     self,
     solver,
     stepsize_controller,
     discrete_terminating_event,
     saveat,
@@ -521,21 +532,23 @@
 ):
 
     #
     # Unpack our various arguments. Delete a lot of things just to make sure we're not
     # using them later.
     #
 
-    del init_state, t1
+    del perturbed, init_state, t1
     ts, ys = residuals
     del residuals
     grad_final_state, _ = grad_final_state__aux_stats
     # Note that `grad_final_state.save_state` has type `PyTree[SaveState]`; here we are
     # relying on the guard in `BacksolveAdjoint` that it have trivial structure.
     grad_ys = grad_final_state.save_state.ys
+    # We take the simple way out and don't try to handle symbolic zeros.
+    grad_ys = jtu.tree_map(_materialise_none, ys, grad_ys)
     del grad_final_state, grad_final_state__aux_stats
     y, args, terms = y__args__terms
     del y__args__terms
     diff_args = eqx.filter(args, eqx.is_inexact_array)
     diff_terms = eqx.filter(terms, eqx.is_inexact_array)
     zeros_like_y = jtu.tree_map(jnp.zeros_like, y)
     zeros_like_diff_args = jtu.tree_map(jnp.zeros_like, diff_args)
@@ -658,17 +671,14 @@
 
         aug1, _, _ = state
         a_y1, a_diff_args1, a_diff_terms1 = aug1
 
     return a_y1, a_diff_args1, a_diff_terms1
 
 
-_loop_backsolve.defvjp(_loop_backsolve_fwd, _loop_backsolve_bwd)
-
-
 class BacksolveAdjoint(AbstractAdjoint):
     """Backpropagate through [`diffrax.diffeqsolve`][] by solving the continuous
     adjoint equations backwards-in-time. This is also sometimes known as
     "optimise-then-discretise", the "continuous adjoint method" or simply the "adjoint
     method".
 
     This method implies very low memory usage, but the
```

### Comparing `diffrax-0.4.0/diffrax/autocitation.py` & `diffrax-0.4.1/diffrax/autocitation.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/brownian/base.py` & `diffrax-0.4.1/diffrax/brownian/base.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/brownian/path.py` & `diffrax-0.4.1/diffrax/brownian/path.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/brownian/tree.py` & `diffrax-0.4.1/diffrax/brownian/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,29 +180,29 @@
         # We have w_s, w_t, w_u available to us, and interpolate with the unique
         # parabola passing through them.
         # Why quadratic and not just "linear from w_s to w_t to w_u"? Because linear
         # only gets the conditional mean correct at every point, but not the
         # conditional variance. This means that the Virtual Brownian Tree will pass
         # statistical tests comparing w(t)|(w(s),w(u)) against the true Brownian
         # bridge. (Provided s, t, u are greater than the discretisation level `tol`.)
-        # (If you just do linear then you find that the variance is *every so slightly*
+        # (If you just do linear then you find that the variance is *ever so slightly*
         # too small.)
         s = final_state.s
         u = final_state.u
         w_s = final_state.w_s
         w_t = final_state.w_t
         w_u = final_state.w_u
         rescaled_τ = (τ - s) / (u - s)
         # Fit polynomial as usual.
         # The polynomial ax^2 + bx + c is found by solving
         # [s^2 s 1][a]   [w_s]
         # [t^2 t 1][b] = [w_t]
         # [u^2 u 1][c]   [w_u]
         #
-        # `A` is inverse of the above matrix, rescaled to s=0, t=0.5, u=1.
+        # `A` is the inverse of the above matrix, with s=0, t=0.5, u=1.
         A = jnp.array([[2, -4, 2], [-3, 4, -1], [1, 0, 0]])
         coeffs = jnp.tensordot(A, jnp.stack([w_s, w_t, w_u]), axes=1)
         return jnp.polyval(coeffs, rescaled_τ)
 
 
 VirtualBrownianTree.__init__.__doc__ = """
 **Arguments:**
```

### Comparing `diffrax-0.4.0/diffrax/custom_types.py` & `diffrax-0.4.1/diffrax/custom_types.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/event.py` & `diffrax-0.4.1/diffrax/event.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/global_interpolation.py` & `diffrax-0.4.1/diffrax/global_interpolation.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/heuristics.py` & `diffrax-0.4.1/diffrax/heuristics.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/integrate.py` & `diffrax-0.4.1/diffrax/integrate.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from typing import Any, Callable, get_args, get_origin, Optional, Tuple
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
+from jax.typing import ArrayLike
 
 from .adjoint import AbstractAdjoint, DirectAdjoint, RecursiveCheckpointAdjoint
 from .custom_types import Array, Bool, Int, PyTree, Scalar
 from .event import AbstractDiscreteTerminatingEvent
 from .global_interpolation import DenseInterpolation
 from .heuristics import is_sde, is_unsafe_sde
+from .misc import static_select
 from .saveat import SaveAt, SubSaveAt
 from .solution import is_okay, is_successful, RESULTS, Solution
 from .solver import (
     AbstractItoSolver,
     AbstractSolver,
     AbstractStratonovichSolver,
     Euler,
@@ -25,15 +27,14 @@
     ItoMilstein,
     StratonovichMilstein,
 )
 from .step_size_controller import (
     AbstractAdaptiveStepSizeController,
     AbstractStepSizeController,
     ConstantStepSize,
-    PIDController,
     StepTo,
 )
 from .term import AbstractTerm, MultiTerm, ODETerm, WrapTerm
 
 
 class SaveState(eqx.Module):
     saveat_ts_index: Int
@@ -137,14 +138,27 @@
     else:
         tol = 1e-6
     clip = tnext > t1 - tol
     tclip = jnp.where(keep_step, t1, tprev + 0.5 * (t1 - tprev))
     return jnp.where(clip, tclip, tnext)
 
 
+def _maybe_static(static_x: ArrayLike, x: Array) -> ArrayLike:
+    # Some values (made_jump and result) are not used in many common use-cases. If we
+    # detect that they're unused then we make sure they're non-Array Python values, so
+    # that we can special case on them at trace time and get a performance boost.
+    if isinstance(static_x, (bool, int, float, complex)):
+        return static_x
+    elif type(jax.core.get_aval(static_x)) is jax.core.ConcreteArray:
+        with jax.ensure_compile_time_eval():
+            return static_x.item()
+    else:
+        return x
+
+
 def loop(
     *,
     solver,
     stepsize_controller,
     discrete_terminating_event,
     saveat,
     t0,
@@ -171,41 +185,49 @@
     save_state = jtu.tree_map(
         save_t0, saveat.subs, init_state.save_state, is_leaf=_is_subsaveat
     )
     init_state = eqx.tree_at(
         lambda s: s.save_state, init_state, save_state, is_leaf=_is_none
     )
 
-    # Privileged optimisation for the common case of no jumps. We can reduce
-    # solver compile time with this.
-    # TODO: somehow make this a non-privileged optimisation, i.e. detect when
-    # we can make jumps or not.
-    cannot_make_jump = isinstance(stepsize_controller, (ConstantStepSize, StepTo)) or (
-        isinstance(stepsize_controller, PIDController)
-        and stepsize_controller.jump_ts is None
-    )
+    def _handle_static(state):
+        # We can improve runtime by resolving `result` at trace time if possible.
+        # We can improve compiletime by resolving `made_jump` at trace time if possible.
+        result = _maybe_static(static_result, state.result)
+        made_jump = _maybe_static(static_made_jump, state.made_jump)
+        return eqx.tree_at(
+            lambda s: (s.result, s.made_jump), state, (result, made_jump)
+        )
 
     def cond_fun(state):
-        return (state.tprev < t1) & is_successful(state.result)
+        if isinstance(stepsize_controller, StepTo):
+            # Privileged optimisation.
+            # This is a measurably cheaper check than the tprev < t1 check.
+            out = state.num_steps < len(stepsize_controller.ts) - 1
+        else:
+            out = state.tprev < t1
+        state = _handle_static(state)
+        return out & is_successful(state.result)
 
     def body_fun(state):
+        state = _handle_static(state)
 
         #
         # Actually do some differential equation solving! Make numerical steps, adapt
         # step sizes, all that jazz.
         #
 
         (y, y_error, dense_info, solver_state, solver_result) = solver.step(
             terms,
             state.tprev,
             state.tnext,
             state.y,
             args,
             state.solver_state,
-            False if cannot_make_jump else state.made_jump,
+            state.made_jump,
         )
 
         # e.g. if someone has a sqrt(y) in the vector field, and dt0 is so large that
         # we get a negative value for y, and then get a NaN vector field. (And then
         # everything breaks.) See #143.
         y_error = jtu.tree_map(lambda x: jnp.where(jnp.isnan(x), jnp.inf, x), y_error)
 
@@ -224,51 +246,40 @@
             y,
             args,
             y_error,
             error_order,
             state.controller_state,
         )
         assert jnp.result_type(keep_step) is jnp.dtype(bool)
-        if cannot_make_jump:
-            # Should hopefully get DCE'd out.
-            made_jump = eqxi.error_if(
-                made_jump,
-                made_jump,
-                (
-                    "Internal error in Diffrax: made unexpected jump. Please report an "
-                    "issue at https://github.com/patrick-kidger/diffrax/issues"
-                ),
-            )
 
         #
         # Do some book-keeping.
         #
 
         tprev = jnp.minimum(tprev, t1)
         tnext = _clip_to_end(tprev, tnext, t1, keep_step)
 
         # The other parts of the mutable state are kept/not-kept (based on whether the
         # step was accepted) by the stepsize controller. But it doesn't get access to
         # these parts, so we do them here.
         keep = lambda a, b: jnp.where(keep_step, a, b)
         y = jtu.tree_map(keep, y, state.y)
         solver_state = jtu.tree_map(keep, solver_state, state.solver_state)
-        made_jump = keep(made_jump, state.made_jump)
-        solver_result = keep(solver_result, RESULTS.successful)
+        made_jump = static_select(keep_step, made_jump, state.made_jump)
+        solver_result = static_select(keep_step, solver_result, RESULTS.successful)
 
         # TODO: if we ever support non-terminating events, then they should go in here.
         # In particular the thing to be careful about is in the `if saveat.steps`
         # branch below, where we want to make sure that it is the value of `y` at
         # `tprev` that is actually saved. (And not just the value of `y` at the
         # previous step's `tnext`, i.e. immediately before the jump.)
 
         # Store the first unsuccessful result we get whilst iterating (if any).
-        result = state.result
-        result = jnp.where(is_okay(result), solver_result, result)
-        result = jnp.where(is_okay(result), stepsize_controller_result, result)
+        result = static_select(is_okay(state.result), solver_result, state.result)
+        result = static_select(is_okay(result), stepsize_controller_result, result)
 
         # Count the number of steps, just for statistical purposes.
         num_steps = state.num_steps + 1
         num_accepted_steps = state.num_accepted_steps + keep_step
         # Not just ~keep_step, which does the wrong thing when keep_step is a non-array
         # bool True/False.
         num_rejected_steps = state.num_rejected_steps + jnp.invert(keep_step)
@@ -324,15 +335,23 @@
             )
 
         save_state = jtu.tree_map(
             save_ts, saveat.subs, save_state, is_leaf=_is_subsaveat
         )
 
         def maybe_inplace(i, u, x):
-            return x.at[i].set(u, pred=keep_step)
+            # Annoying hack. We normally call this with `x` wrapped into a buffer
+            # (from Equinox's while loops). However we do also first trace through to
+            # see if we can resolve some values statically, in which case normal JAX
+            # arrays don't support the extra `pred` argument. We don't then use the
+            # result of this so we just skip it.
+            if _filtering:
+                return x
+            else:
+                return x.at[i].set(u, pred=keep_step)
 
         def save_steps(subsaveat: SubSaveAt, save_state: SaveState) -> SaveState:
             if subsaveat.steps:
                 ts = maybe_inplace(save_state.save_index, tprev, save_state.ts)
                 ys = jtu.tree_map(
                     ft.partial(maybe_inplace, save_state.save_index),
                     subsaveat.fn(tprev, y, args),
@@ -385,23 +404,32 @@
                 t0=t0,
                 t1=t1,
                 dt0=dt0,
                 max_steps=max_steps,
                 terms=terms,
                 args=args,
             )
-            result = jnp.where(
+            result = static_select(
                 discrete_terminating_event_occurred,
                 RESULTS.discrete_terminating_event_occurred,
                 result,
             )
             new_state = eqx.tree_at(lambda s: s.result, new_state, result)
 
         return new_state
 
+    _filtering = True
+    static_made_jump = init_state.made_jump
+    static_result = init_state.result
+    filter_state = eqx.filter_eval_shape(body_fun, init_state)
+    _filtering = False
+    static_made_jump = filter_state.made_jump
+    static_result = filter_state.result
+    del filter_state
+
     final_state = outer_while_loop(
         cond_fun, body_fun, init_state, max_steps=max_steps, buffers=_outer_buffers
     )
 
     def _save_t1(subsaveat, save_state):
         if subsaveat.t1 and not subsaveat.steps:
             # If subsaveat.steps then the final value is already saved.
@@ -416,14 +444,15 @@
     save_state = jtu.tree_map(
         _save_t1, saveat.subs, final_state.save_state, is_leaf=_is_subsaveat
     )
     final_state = eqx.tree_at(
         lambda s: s.save_state, final_state, save_state, is_leaf=_is_none
     )
 
+    final_state = _handle_static(final_state)
     result = jnp.where(
         cond_fun(final_state), RESULTS.max_steps_reached, final_state.result
     )
     aux_stats = dict()
     return eqx.tree_at(lambda s: s.result, final_state, result), aux_stats
 
 
@@ -565,15 +594,15 @@
             "Must have (t1 - t0) * dt0 >= 0, we instead got "
             f"t1 with value {t1} and type {type(t1)}, "
             f"t0 with value {t0} and type {type(t0)}, "
             f"dt0 with value {dt0} and type {type(dt0)}"
         )
         with jax.ensure_compile_time_eval():
             pred = (t1 - t0) * dt0 < 0
-        dt0 = eqxi.error_if(dt0, pred, msg)
+        dt0 = eqxi.error_if(jnp.array(dt0), pred, msg)
 
     # Backward compatibility
     if isinstance(
         solver, (EulerHeun, ItoMilstein, StratonovichMilstein)
     ) and _term_compatible(terms, (ODETerm, AbstractTerm)):
         warnings.warn(
             "Passing `terms=(ODETerm(...), SomeOtherTerm(...))` to "
@@ -747,15 +776,15 @@
         )
 
     save_state = jtu.tree_map(_allocate_output, saveat.subs, is_leaf=_is_subsaveat)
     num_steps = 0
     num_accepted_steps = 0
     num_rejected_steps = 0
     made_jump = False if made_jump is None else made_jump
-    result = jnp.array(RESULTS.successful)
+    result = RESULTS.successful
     if saveat.dense:
         if max_steps is None:
             raise ValueError(
                 "`max_steps=None` is incompatible with `saveat.dense=True`"
             )
         (_, _, dense_info, _, _,) = eqx.filter_eval_shape(
             solver.step, terms, tprev, tnext, y0, args, solver_state, made_jump
@@ -867,14 +896,15 @@
         result=result,
         solver_state=solver_state,
         controller_state=controller_state,
         made_jump=made_jump,
     )
 
     error_index = eqxi.unvmap_max(result)
-    sol = eqxi.branched_error_if(
-        sol,
-        throw & jnp.invert(is_okay(result)),
-        error_index,
-        RESULTS.reverse_lookup,
-    )
+    if throw:
+        sol = eqxi.branched_error_if(
+            sol,
+            jnp.invert(is_okay(result)),
+            error_index,
+            RESULTS.reverse_lookup,
+        )
     return sol
```

### Comparing `diffrax-0.4.0/diffrax/local_interpolation.py` & `diffrax-0.4.1/diffrax/local_interpolation.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/misc.py` & `diffrax-0.4.1/diffrax/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from typing import Callable, Optional, Tuple
+from typing import Callable, Optional, Tuple, Union
 
 import jax
+import jax.core
 import jax.flatten_util as fu
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
+from jax.typing import ArrayLike
 
 from .custom_types import Array, PyTree, Scalar
 
 
 _itemsize_kind_type = {
     (1, "i"): jnp.int8,
     (2, "i"): jnp.int16,
@@ -158,7 +160,26 @@
     """
     treedef = jtu.tree_structure(tree, is_leaf=is_leaf)
     return jtu.tree_unflatten(treedef, jax.random.split(key, treedef.num_leaves))
 
 
 def is_tuple_of_ints(obj):
     return isinstance(obj, tuple) and all(isinstance(x, int) for x in obj)
+
+
+def static_select(pred: Union[bool, Array], a: ArrayLike, b: ArrayLike) -> ArrayLike:
+    # This is mostly useful in that it doesn't promote `a` or `b` to Arrays when the
+    # predicate is statically known.
+    # This in turn allows us to perform some trace-time optimisations that XLA isn't
+    # smart enough to do on its own.
+    if (
+        type(pred) is not bool
+        and type(jax.core.get_aval(pred)) is jax.core.ConcreteArray
+    ):
+        with jax.ensure_compile_time_eval():
+            pred = pred.item()
+    if pred is True:
+        return a
+    elif pred is False:
+        return b
+    else:
+        return lax.select(pred, a, b)
```

### Comparing `diffrax-0.4.0/diffrax/nonlinear_solver/affine.py` & `diffrax-0.4.1/diffrax/nonlinear_solver/affine.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/nonlinear_solver/base.py` & `diffrax-0.4.1/diffrax/nonlinear_solver/base.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/nonlinear_solver/newton.py` & `diffrax-0.4.1/diffrax/nonlinear_solver/newton.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/path.py` & `diffrax-0.4.1/diffrax/path.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/saveat.py` & `diffrax-0.4.1/diffrax/saveat.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solution.py` & `diffrax-0.4.1/diffrax/solution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from dataclasses import field
 from typing import Any, Dict, Optional
 
 import equinox.internal as eqxi
-import jax.numpy as jnp
+import jax
 
 from .custom_types import Array, Bool, PyTree, Scalar
 from .global_interpolation import DenseInterpolation
+from .misc import static_select
 from .path import AbstractPath
 
 
 class RESULTS(metaclass=eqxi.ContainerMeta):
     successful = ""
     discrete_terminating_event_occurred = (
         "Terminating solve because a discrete event occurred."
@@ -21,40 +22,46 @@
     implicit_divergence = "Implicit method diverged."
     implicit_nonconvergence = (
         "Implicit method did not converge within the required number of iterations."
     )
 
 
 def is_okay(result: RESULTS) -> Bool:
-    return is_successful(result) | is_event(result)
+    with jax.ensure_compile_time_eval():
+        return is_successful(result) | is_event(result)
 
 
 def is_successful(result: RESULTS) -> Bool:
-    return result == RESULTS.successful
+    with jax.ensure_compile_time_eval():
+        return result == RESULTS.successful
 
 
 # TODO: In the future we may support other event types, in which case this function
 # should be updated.
 def is_event(result: RESULTS) -> Bool:
-    return result == RESULTS.discrete_terminating_event_occurred
+    with jax.ensure_compile_time_eval():
+        return result == RESULTS.discrete_terminating_event_occurred
 
 
 def update_result(old_result: RESULTS, new_result: RESULTS) -> RESULTS:
     """
     Returns:
 
         old | success event_o error_o
     new     |
     --------+-------------------------
     success | success event_o error_o
     event_n | event_n event_o error_o
     error_n | error_n error_n error_o
     """
-    out_result = jnp.where(is_okay(old_result), new_result, old_result)
-    return jnp.where(is_okay(new_result) & is_event(old_result), old_result, out_result)
+    with jax.ensure_compile_time_eval():
+        out_result = static_select(is_okay(old_result), new_result, old_result)
+        return static_select(
+            is_okay(new_result) & is_event(old_result), old_result, out_result
+        )
 
 
 class Solution(AbstractPath):
     """The solution to a differential equation.
 
     **Attributes:**
```

### Comparing `diffrax-0.4.0/diffrax/solver/__init__.py` & `diffrax-0.4.1/diffrax/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/base.py` & `diffrax-0.4.1/diffrax/solver/base.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/bosh3.py` & `diffrax-0.4.1/diffrax/solver/bosh3.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/dopri5.py` & `diffrax-0.4.1/diffrax/solver/dopri5.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/dopri8.py` & `diffrax-0.4.1/diffrax/solver/dopri8.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/euler.py` & `diffrax-0.4.1/diffrax/solver/euler.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/euler_heun.py` & `diffrax-0.4.1/diffrax/solver/euler_heun.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/heun.py` & `diffrax-0.4.1/diffrax/solver/heun.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/implicit_euler.py` & `diffrax-0.4.1/diffrax/solver/implicit_euler.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from equinox.internal import ω
 
 from ..custom_types import Bool, DenseInfo, PyTree, Scalar
 from ..heuristics import is_sde
 from ..local_interpolation import LocalLinearInterpolation
 from ..solution import RESULTS
 from ..term import AbstractTerm
-from .base import AbstractImplicitSolver
+from .base import AbstractAdaptiveSolver, AbstractImplicitSolver
 
 
 _SolverState = None
 
 
 def _implicit_relation(z1, nonlinear_solve_args):
     vf_prod, t1, y0, args, control = nonlinear_solve_args
     diff = (vf_prod(t1, (y0**ω + z1**ω).ω, args, control) ** ω - z1**ω).ω
     return diff
 
 
-class ImplicitEuler(AbstractImplicitSolver):
+class ImplicitEuler(AbstractImplicitSolver, AbstractAdaptiveSolver):
     r"""Implicit Euler method.
 
     A-B-L stable 1st order SDIRK method. Has an embedded 2nd order Heun method for
     adaptive step sizing. Uses 1 stage. Uses a 1st order local linear interpolation for
     dense/ts output.
     """
```

### Comparing `diffrax-0.4.0/diffrax/solver/kencarp3.py` & `diffrax-0.4.1/diffrax/solver/kencarp3.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/kencarp4.py` & `diffrax-0.4.1/diffrax/solver/kencarp4.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/kencarp5.py` & `diffrax-0.4.1/diffrax/solver/kencarp5.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/kvaerno3.py` & `diffrax-0.4.1/diffrax/solver/kvaerno3.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/kvaerno4.py` & `diffrax-0.4.1/diffrax/solver/kvaerno4.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/kvaerno5.py` & `diffrax-0.4.1/diffrax/solver/kvaerno5.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/leapfrog_midpoint.py` & `diffrax-0.4.1/diffrax/solver/leapfrog_midpoint.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/midpoint.py` & `diffrax-0.4.1/diffrax/solver/midpoint.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/milstein.py` & `diffrax-0.4.1/diffrax/solver/milstein.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/ralston.py` & `diffrax-0.4.1/diffrax/solver/ralston.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/reversible_heun.py` & `diffrax-0.4.1/diffrax/solver/reversible_heun.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/runge_kutta.py` & `diffrax-0.4.1/diffrax/solver/runge_kutta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import functools as ft
 from dataclasses import dataclass, field
 from typing import get_args, get_origin, Literal, Optional, Tuple, Union
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
-import jax.flatten_util as jfu
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 from equinox.internal import ω
 
 from ..custom_types import Array, DenseInfo, PyTree, Scalar, sentinel
@@ -214,28 +213,44 @@
 
 # TODO: examine termination criterion for Newton iteration
 # TODO: replace fi with fi=(zi + predictor), where this relation defines some zi, and
 #       iterate to find zi, using zi=0 as the predictor. This should give better
 #       numerical behaviour since the iteration is close to 0. (Although we have
 #       multiplied by the increment of the control, i.e. dt, which is small...)
 def _implicit_relation_f(fi, nonlinear_solve_args):
-    diagonal, vf, prod, ti, yi_partial, args, control = nonlinear_solve_args
+    # We pass stage_index, even without using it, so that custom nonlinear solvers
+    # can special-case on the stage if they want to.
+    (
+        stage_index,
+        diagonal,
+        vf,
+        prod,
+        ti,
+        yi_partial,
+        args,
+        control,
+    ) = nonlinear_solve_args
+    del stage_index
     diff = (
         fi**ω
         - vf(ti, (yi_partial**ω + diagonal * prod(fi, control) ** ω).ω, args) ** ω
     ).ω
     return diff
 
 
 # TODO: consider dividing by diagonal and control
 def _implicit_relation_k(ki, nonlinear_solve_args):
     # c.f:
     # https://github.com/SciML/DiffEqDevMaterials/blob/master/newton/output/main.pdf
     # (Bearing in mind that our ki is dt times smaller than theirs.)
-    diagonal, vf_prod, ti, yi_partial, args, control = nonlinear_solve_args
+    #
+    # We pass stage_index, even without using it, so that custom nonlinear solvers
+    # can special-case on the stage if they want to.
+    stage_index, diagonal, vf_prod, ti, yi_partial, args, control = nonlinear_solve_args
+    del stage_index
     diff = (
         ki**ω
         - vf_prod(ti, (yi_partial**ω + diagonal * ki**ω).ω, args, control) ** ω
     ).ω
     return diff
 
 
@@ -728,14 +743,33 @@
             implicit_diagonal = jnp.asarray(implicit_tableau.a_diagonal)
             implicit_predictor = np.zeros((num_stages, num_stages))
             for i, a_predictor_i in enumerate(implicit_tableau.a_predictor):
                 implicit_predictor[i + 1, : i + 1] = a_predictor_i
             implicit_predictor = jnp.asarray(implicit_predictor)
             implicit_c = get_implicit(tableaus_c)
 
+        if implicit_term is None:
+            implicit_vf = _unused
+            implicit_prod = _unused
+            implicit_vf_prod = _unused
+        else:
+            if eval_fs:
+                assert f0 is not _unused
+                implicit_vf = eqx.filter_closure_convert(implicit_term.vf, t0, y0, args)
+                implicit_prod = eqx.filter_closure_convert(
+                    implicit_term.prod, get_implicit(f0), implicit_control
+                )
+                implicit_vf_prod = _unused
+            else:
+                implicit_vf = _unused
+                implicit_prod = _unused
+                implicit_vf_prod = eqx.filter_closure_convert(
+                    implicit_term.vf_prod, t0, y0, args, implicit_control
+                )
+
         #
         # Run the loop over stages. (This is what you signed up for, and it's taken us
         # several hundred lines of code just to get this far!)
         #
 
         def cond_stage(val):
             stage_index, *_ = val
@@ -785,18 +819,20 @@
                     f_pred = get_implicit(
                         vector_tree_dot(implicit_predictor_i, unsafe_fs)
                     )
                     if not fsal:
                         # FSAL => explicit first stage so the choice of predictor
                         # doesn't matter.
                         f_pred = jtu.tree_map(if_first_stage, f0_for_jac, f_pred)
+                    assert f0 is not _unused
                     f_implicit_args = (
+                        stage_index,
                         implicit_diagonal_i,
-                        implicit_term.vf,
-                        implicit_term.prod,
+                        implicit_vf,
+                        implicit_prod,
                         implicit_ti,
                         yi_partial,
                         args,
                         implicit_control,
                     )
                     k_pred = _unused
                     k_implicit_args = _unused
@@ -807,16 +843,17 @@
                         implicit_predictor_i, get_implicit(unsafe_ks)
                     )
                     if not fsal:
                         # FSAL => explicit first stage so the choice of predictor
                         # doesn't matter.
                         k_pred = jtu.tree_map(if_first_stage, k0_for_jac, k_pred)
                     k_implicit_args = (
+                        stage_index,
                         implicit_diagonal_i,
-                        implicit_term.vf_prod,
+                        implicit_vf_prod,
                         implicit_ti,
                         yi_partial,
                         args,
                         implicit_control,
                     )
 
                 def eval_f_jac():
@@ -945,31 +982,49 @@
             jac_f = _unused
             jac_k = _unused
         else:
             # Set the initial Jacobian to be the identity matrix.
             # For DIRK and SDIRK methods then the choice here doesn't matter; we compute
             # the Jacobian straight away.
             # For ESDIRK methods, this is the Jacobian of an explicit step.
-            #
-            # TODO: fix once we have more advanced nonlinear solvers.
-            # Mildly hacky hardcoding for now.
             if eval_fs:
                 assert f0 is not _unused
-                struct = jax.eval_shape(lambda: jfu.ravel_pytree(get_implicit(f0))[0])
-                jac_f = (
-                    jnp.eye(struct.size, dtype=struct.dtype),
-                    jnp.arange(struct.size, dtype=jnp.int32),
+                f_implicit_args = (
+                    jnp.array(0),
+                    # zero diagonal == identity matrix as the Jacobian
+                    jnp.array(0.0, dtype=implicit_diagonal.dtype),
+                    implicit_vf,
+                    implicit_prod,
+                    t0,
+                    y0,
+                    args,
+                    implicit_control,
+                )
+                jac_f = self.nonlinear_solver.jac(
+                    _implicit_relation_f,
+                    jtu.tree_map(jnp.zeros_like, get_implicit(f0)),
+                    _filter_stop_gradient(f_implicit_args),
                 )
                 jac_k = _unused
             else:
-                struct = jax.eval_shape(lambda: jfu.ravel_pytree(y0)[0])
+                k_implicit_args = (
+                    jnp.array(0),
+                    # zero diagonal == identity matrix as the Jacobian
+                    jnp.array(0.0, dtype=implicit_diagonal.dtype),
+                    implicit_vf_prod,
+                    t0,
+                    y0,
+                    args,
+                    implicit_control,
+                )
                 jac_f = _unused
-                jac_k = (
-                    jnp.eye(struct.size, dtype=struct.dtype),
-                    jnp.arange(struct.size, dtype=jnp.int32),
+                jac_k = self.nonlinear_solver.jac(
+                    _implicit_relation_k,
+                    jtu.tree_map(jnp.zeros_like, y0),
+                    _filter_stop_gradient(k_implicit_args),
                 )
         init_val = (
             init_stage_index,
             y0,
             dummy_f,
             jac_f,
             jac_k,
@@ -1056,15 +1111,15 @@
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         if hasattr(cls, "tableau"):  # Abstract subclasses may not have a tableau.
             diagonal = cls.tableau.a_diagonal[0]
             assert (cls.tableau.a_diagonal == diagonal).all()
 
-    calculate_jacobian = CalculateJacobian.second_stage
+    calculate_jacobian = CalculateJacobian.first_stage
 
 
 class AbstractESDIRK(AbstractDIRK):
     """Abstract base class for all Explicit Singular Diagonal Implicit Runge--Kutta
     solvers.
 
     Subclasses should include a class-level attribute `tableau`, an instance of
```

### Comparing `diffrax-0.4.0/diffrax/solver/semi_implicit_euler.py` & `diffrax-0.4.1/diffrax/solver/semi_implicit_euler.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/sil3.py` & `diffrax-0.4.1/diffrax/solver/sil3.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/solver/tsit5.py` & `diffrax-0.4.1/diffrax/solver/tsit5.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/step_size_controller/adaptive.py` & `diffrax-0.4.1/diffrax/step_size_controller/adaptive.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/step_size_controller/base.py` & `diffrax-0.4.1/diffrax/step_size_controller/base.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/step_size_controller/constant.py` & `diffrax-0.4.1/diffrax/step_size_controller/constant.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/diffrax/term.py` & `diffrax-0.4.1/diffrax/term.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,21 @@
         ode_term = ODETerm(vector_field)
         diffeqsolve(ode_term, ...)
         ```
     """
     vector_field: Callable[[Scalar, PyTree, PyTree], PyTree]
 
     def vf(self, t: Scalar, y: PyTree, args: PyTree) -> PyTree:
-        return self.vector_field(t, y, args)
+        out = self.vector_field(t, y, args)
+        if jtu.tree_structure(out) != jtu.tree_structure(y):
+            raise ValueError(
+                "The vector field inside `ODETerm` must return a pytree with the "
+                "same structure as `y0`."
+            )
+        return jtu.tree_map(lambda o, yi: jnp.broadcast_to(o, jnp.shape(yi)), out, y)
 
     @staticmethod
     def contr(t0: Scalar, t1: Scalar) -> Scalar:
         return t1 - t0
 
     @staticmethod
     def prod(vf: PyTree, control: Scalar) -> PyTree:
```

### Comparing `diffrax-0.4.0/diffrax.egg-info/PKG-INFO` & `diffrax-0.4.1/diffrax.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffrax
-Version: 0.4.0
+Version: 0.4.1
 Summary: GPU+autodiff-capable ODE/SDE/CDE solvers written in JAX.
 Home-page: https://github.com/patrick-kidger/diffrax
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
@@ -42,15 +42,15 @@
 
 ## Installation
 
 ```
 pip install diffrax
 ```
 
-Requires Python 3.9+, JAX 0.4.4+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.4+.
+Requires Python 3.9+, JAX 0.4.13+, and [Equinox](https://github.com/patrick-kidger/equinox) 0.10.11+.
 
 ## Documentation
 
 Available at [https://docs.kidger.site/diffrax](https://docs.kidger.site/diffrax).
 
 ## Quick example
 
@@ -80,16 +80,22 @@
     year={2021},
     school={University of Oxford},
 }
 ```
 
 (Also consider starring the project on GitHub.)
 
-## See also
+## See also: other libraries in the JAX ecosystem
 
-Neural networks: [Equinox](https://github.com/patrick-kidger/equinox).
+[Equinox](https://github.com/patrick-kidger/equinox): neural networks.
 
-Type annotations and runtime checking for PyTrees and shape/dtype of JAX arrays: [jaxtyping](https://github.com/google/jaxtyping).
+[Optax](https://github.com/deepmind/optax): first-order gradient (SGD, Adam, ...) optimisers.
 
-Computer vision models: [Eqxvision](https://github.com/paganpasta/eqxvision).
+[Lineax](https://github.com/google/lineax): linear solvers and linear least squares.
 
-SymPy<->JAX conversion; train symbolic expressions via gradient descent: [sympy2jax](https://github.com/google/sympy2jax).
+[jaxtyping](https://github.com/google/jaxtyping): type annotations for shape/dtype of arrays.
+
+[Eqxvision](https://github.com/paganpasta/eqxvision): computer vision models.
+
+[sympy2jax](https://github.com/google/sympy2jax): SymPy<->JAX conversion; train symbolic expressions via gradient descent.
+
+[Levanter](https://github.com/stanford-crfm/levanter): scalable+reliable training of foundation models (e.g. LLMs).
```

### Comparing `diffrax-0.4.0/diffrax.egg-info/SOURCES.txt` & `diffrax-0.4.1/diffrax.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 diffrax/solver/sil3.py
 diffrax/solver/tsit5.py
 diffrax/step_size_controller/__init__.py
 diffrax/step_size_controller/adaptive.py
 diffrax/step_size_controller/base.py
 diffrax/step_size_controller/constant.py
 test/__init__.py
+test/__main__.py
 test/conftest.py
 test/helpers.py
 test/test_adaptive_stepsize_controller.py
 test/test_adjoint.py
 test/test_brownian.py
 test/test_detest.py
 test/test_event.py
```

### Comparing `diffrax-0.4.0/setup.py` & `diffrax-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 
 python_requires = "~=3.9"
 
-install_requires = ["jax>=0.4.3", "equinox>=0.10.4"]
+install_requires = ["jax>=0.4.13", "equinox>=0.10.11"]
 
 setuptools.setup(
     name=name,
     version=version,
     author=author,
     author_email=author_email,
     maintainer=author,
```

### Comparing `diffrax-0.4.0/test/helpers.py` & `diffrax-0.4.1/test/helpers.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/test/test_adaptive_stepsize_controller.py` & `diffrax-0.4.1/test/test_adaptive_stepsize_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import diffrax
 import equinox as eqx
+import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 
+from .helpers import shaped_allclose
+
 
 def test_step_ts():
     term = diffrax.ODETerm(lambda t, y, args: -0.2 * y)
     solver = diffrax.Dopri5()
     t0 = 0
     t1 = 5
     dt0 = None
@@ -86,7 +89,49 @@
     stepsize_controller = diffrax.PIDController(rtol=1e-4, atol=1e-4)
     _, state = stepsize_controller.init(term, 0, 1, y0, 0.1, None, solver.func, 5)
 
     for y_error in (jnp.array(0.0), jnp.array(3.0), jnp.array(jnp.inf)):
         ys = (y0, y1_candidate, y_error)
         grads = run(ys, stepsize_controller, state)
         assert not any(jnp.isnan(grad).any() for grad in grads)
+
+
+def test_grad_of_discontinuous_forcing():
+    def vector_field(t, y, forcing):
+        y, _ = y
+        dy = -y + forcing(t)
+        dsum = y
+        return dy, dsum
+
+    def run(t):
+        term = diffrax.ODETerm(vector_field)
+        solver = diffrax.Tsit5()
+        t0 = 0
+        t1 = 1
+        dt0 = None
+        y0 = 1.0
+        stepsize_controller = diffrax.PIDController(
+            rtol=1e-8, atol=1e-8, step_ts=t[None]
+        )
+
+        def forcing(s):
+            return jnp.where(s < t, 0, 1)
+
+        sol = diffrax.diffeqsolve(
+            term,
+            solver,
+            t0,
+            t1,
+            dt0,
+            (y0, 0),
+            args=forcing,
+            stepsize_controller=stepsize_controller,
+        )
+        _, sum = sol.ys
+        (sum,) = sum
+        return sum
+
+    r = jax.jit(run)
+    eps = 1e-5
+    finite_diff = (r(0.5) - r(0.5 - eps)) / eps
+    autodiff = jax.jit(jax.grad(run))(0.5)
+    assert shaped_allclose(finite_diff, autodiff)
```

### Comparing `diffrax-0.4.0/test/test_brownian.py` & `diffrax-0.4.1/test/test_brownian.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/test/test_detest.py` & `diffrax-0.4.1/test/test_detest.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/test/test_event.py` & `diffrax-0.4.1/test/test_event.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/test/test_global_interpolation.py` & `diffrax-0.4.1/test/test_global_interpolation.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/test/test_integrate.py` & `diffrax-0.4.1/test/test_integrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -386,7 +386,35 @@
 
     # Test numerical gradients: Diffrax issue #64
     eps = 1e-6
     val = f(1.0)
     val_eps = f(1.0 + eps)
     numerical_grads = (val_eps - val) / eps
     assert shaped_allclose(grads, numerical_grads)
+
+
+def test_concrete_made_jump():
+    for constant in (True, False):
+        if constant:
+            dt0 = 0.1
+            stepsize_controller = diffrax.ConstantStepSize()
+        else:
+            dt0 = None
+            stepsize_controller = diffrax.StepTo([0, 0.3, 1])
+
+        @jax.jit
+        def run(y0):
+            term = diffrax.ODETerm(lambda t, y, args: -y)
+            sol = diffrax.diffeqsolve(
+                term,
+                diffrax.Tsit5(),
+                0,
+                1,
+                dt0,
+                y0,
+                stepsize_controller=stepsize_controller,
+                saveat=diffrax.SaveAt(t1=True, made_jump=True),
+                throw=False,
+            )
+            assert sol.made_jump is False
+
+        run(1)
```

### Comparing `diffrax-0.4.0/test/test_interpolation.py` & `diffrax-0.4.1/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/test/test_local_interpolation.py` & `diffrax-0.4.1/test/test_local_interpolation.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/test/test_newton_solver.py` & `diffrax-0.4.1/test/test_newton_solver.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/test/test_saveat_solution.py` & `diffrax-0.4.1/test/test_saveat_solution.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/test/test_solver.py` & `diffrax-0.4.1/test/test_solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Tuple
 
 import diffrax
 import equinox as eqx
+import jax
 import jax.numpy as jnp
 import jax.random as jr
 import pytest
 
-from .helpers import shaped_allclose
+from .helpers import implicit_tol, shaped_allclose
 
 
 def test_half_solver():
     term = diffrax.ODETerm(lambda t, y, args: -y)
     t0 = 0
     t1 = 1
     y0 = 1.0
@@ -450,7 +451,22 @@
             [9.9607774744245892e-01, 3.5804372350422432e-05, 3.8864481851928275e-03],
             [9.6645973733301294e-01, 3.0746265785786866e-05, 3.3509516401211095e-02],
             [8.4136992384147014e-01, 1.6233909379904643e-05, 1.5861384224914774e-01],
             [6.1723488239606716e-01, 6.1535912746388841e-06, 3.8275896401264059e-01],
         ]
     )
     assert jnp.allclose(sol.ys, true_ys, rtol=1e-3, atol=1e-8)
+
+
+def test_implicit_closure_convert():
+    @jax.grad
+    def f(x):
+        def vector_field(t, y, args):
+            return x * y
+
+        term = diffrax.ODETerm(vector_field)
+        solver = diffrax.Kvaerno3()
+        solver = implicit_tol(solver)
+        out = diffrax.diffeqsolve(term, solver, 0, 1, 0.1, 1.0)
+        return out.ys[0]
+
+    f(1.0)
```

### Comparing `diffrax-0.4.0/test/test_step_to.py` & `diffrax-0.4.1/test/test_step_to.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.4.0/test/test_term.py` & `diffrax-0.4.1/test/test_term.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,25 +32,26 @@
         def derivative(self, t):
             return jrandom.normal(derivkey, (2,))
 
     control = Control()
     term = diffrax.ControlTerm(vector_field, control)
     args = getkey()
     dx = term.contr(0, 1)
-    vf = term.vf(0, None, args)
-    vf_prod = term.vf_prod(0, None, args, dx)
+    y = jnp.array([1.0, 2.0, 3.0])
+    vf = term.vf(0, y, args)
+    vf_prod = term.vf_prod(0, y, args, dx)
     assert dx.shape == (2,)
     assert vf.shape == (3, 2)
     assert vf_prod.shape == (3,)
     assert shaped_allclose(vf_prod, term.prod(vf, dx))
 
     term = term.to_ode()
     dt = term.contr(0, 1)
-    vf = term.vf(0, None, args)
-    vf_prod = term.vf_prod(0, None, args, dt)
+    vf = term.vf(0, y, args)
+    vf_prod = term.vf_prod(0, y, args, dt)
     assert vf.shape == (3,)
     assert vf_prod.shape == (3,)
     assert shaped_allclose(vf_prod, term.prod(vf, dt))
 
 
 def test_weakly_diagional_control_term(getkey):
     vector_field = lambda t, y, args: jrandom.normal(args, (3,))
@@ -66,25 +67,26 @@
         def derivative(self, t):
             return jrandom.normal(derivkey, (3,))
 
     control = Control()
     term = diffrax.WeaklyDiagonalControlTerm(vector_field, control)
     args = getkey()
     dx = term.contr(0, 1)
-    vf = term.vf(0, None, args)
-    vf_prod = term.vf_prod(0, None, args, dx)
+    y = jnp.array([1.0, 2.0, 3.0])
+    vf = term.vf(0, y, args)
+    vf_prod = term.vf_prod(0, y, args, dx)
     assert dx.shape == (3,)
     assert vf.shape == (3,)
     assert vf_prod.shape == (3,)
     assert shaped_allclose(vf_prod, term.prod(vf, dx))
 
     term = term.to_ode()
     dt = term.contr(0, 1)
-    vf = term.vf(0, None, args)
-    vf_prod = term.vf_prod(0, None, args, dt)
+    vf = term.vf(0, y, args)
+    vf_prod = term.vf_prod(0, y, args, dt)
     assert vf.shape == (3,)
     assert vf_prod.shape == (3,)
     assert shaped_allclose(vf_prod, term.prod(vf, dt))
 
 
 def test_ode_adjoint_term(getkey):
     vector_field = lambda t, y, args: -y
```

### Comparing `diffrax-0.4.0/test/test_vmap.py` & `diffrax-0.4.1/test/test_vmap.py`

 * *Files identical despite different names*

