# Comparing `tmp/sparglim-0.1.2.tar.gz` & `tmp/sparglim-0.1.3.tar.gz`

## Comparing `sparglim-0.1.2.tar` & `sparglim-0.1.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 sparglim-0.1.2/.dockerignore
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.2/.editorconfig
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 sparglim-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.2/RELEASE.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 sparglim-0.1.2/config-template.md
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 sparglim-0.1.2/config.md
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 sparglim-0.1.2/generate-config.sh
--rwxr-xr-x   0        0        0     1828 2020-02-02 00:00:00.000000 sparglim-0.1.2/generate_config_docs.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 sparglim-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/docker/Dockerfile.jupyterlab-sparglim
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/docker/Dockerfile.sparglim-server
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-on-k8s/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
--rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/scripts/reload.sh
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/sparglim-server/README.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 sparglim-0.1.2/docker/Dockerfile.jupyterlab-sparglim
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.2/docker/Dockerfile.sparglim-server
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sparglim-0.1.2/docker/README.md
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/README.md
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/sparglim-server/README.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/exceptions.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/py.typed
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/utils.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/config/__init__.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/config/builder.py
--rw-r--r--   0        0        0    11573 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/config/configer.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/config/k8s.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/server/__init__.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/server/cli.py
--rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/server/daemon.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/server/tailer.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/sql/__init__.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/sql/magic.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/test_builder.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/test_daemon.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/test_magic.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/example/people.json
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/mock/sbin/entrypoint.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/mock/sbin/mock_spark_server.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/mock/sbin/start-connect-server.sh
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.2/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.2/LICENSE
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 sparglim-0.1.2/README.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparglim-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 sparglim-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 sparglim-0.1.3/.dockerignore
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.3/.editorconfig
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 sparglim-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.3/RELEASE.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 sparglim-0.1.3/config-template.md
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 sparglim-0.1.3/config.md
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 sparglim-0.1.3/generate-config.sh
+-rwxr-xr-x   0        0        0     1828 2020-02-02 00:00:00.000000 sparglim-0.1.3/generate_config_docs.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 sparglim-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/docker/Dockerfile.jupyterlab-sparglim
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/docker/Dockerfile.sparglim-server
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/jupyter-sparglim-on-k8s/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/jupyter-sparglim-sc/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
+-rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/scripts/reload.sh
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/sparglim-server/README.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.3/dev/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 sparglim-0.1.3/docker/Dockerfile.jupyterlab-sparglim
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.3/docker/Dockerfile.sparglim-server
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sparglim-0.1.3/docker/README.md
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/jupyter-sparglim-on-k8s/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/jupyter-sparglim-sc/README.md
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/sparglim-server/README.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.3/examples/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/exceptions.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/py.typed
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/utils.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/config/__init__.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/config/builder.py
+-rw-r--r--   0        0        0    11573 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/config/configer.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/config/k8s.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/server/__init__.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/server/cli.py
+-rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/server/daemon.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/server/tailer.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/sql/__init__.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 sparglim-0.1.3/sparglim/sql/magic.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 sparglim-0.1.3/tests/test_builder.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.3/tests/test_daemon.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 sparglim-0.1.3/tests/test_magic.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.3/tests/example/people.json
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.3/tests/mock/sbin/entrypoint.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.3/tests/mock/sbin/mock_spark_server.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.3/tests/mock/sbin/start-connect-server.sh
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 sparglim-0.1.3/README.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparglim-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 sparglim-0.1.3/PKG-INFO
```

### Comparing `sparglim-0.1.2/.pre-commit-config.yaml` & `sparglim-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/RELEASE.md` & `sparglim-0.1.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/config-template.md` & `sparglim-0.1.3/config-template.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/config.md` & `sparglim-0.1.3/config.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/generate_config_docs.py` & `sparglim-0.1.3/generate_config_docs.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/.github/workflows/publish.yml` & `sparglim-0.1.3/.github/workflows/publish.yml`

 * *Files 5% similar despite different names*

```diff
@@ -61,25 +61,25 @@
         file: ./docker/Dockerfile.sparglim-server
         push: true
         tags: ${{ secrets.DOCKERHUB_USERNAME }}/sparglim-server:${{  github.ref_name }}
 
     # Build latest if release
     -
       name: Build and push jupyterlab-sparglim_latest
+      if: '!github.event.release.prerelease'
       id: docker_build_jupyterlab_sparglim_latest
-      if: '!github.event.prerelease'
       uses: docker/build-push-action@v4
       with:
         context: .
         file: ./docker/Dockerfile.jupyterlab-sparglim
         push: true
         tags: ${{ secrets.DOCKERHUB_USERNAME }}/jupyterlab-sparglim:latest
     -
       name: Build and push sparglim-server_latest
-      if: '!github.event.prerelease'
+      if: '!github.event.release.prerelease'
       id: docker_build_sparglim_server_latest
       uses: docker/build-push-action@v4
       with:
         context: .
         file: ./docker/Dockerfile.sparglim-server
         push: true
         tags: ${{ secrets.DOCKERHUB_USERNAME }}/sparglim-server:latest
```

### Comparing `sparglim-0.1.2/.github/workflows/python-package.yml` & `sparglim-0.1.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/dev/docker/Dockerfile.jupyterlab-sparglim` & `sparglim-0.1.3/dev/docker/Dockerfile.jupyterlab-sparglim`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml` & `sparglim-0.1.3/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/dev/jupyter-sparglim-sc/README.md` & `sparglim-0.1.3/dev/jupyter-sparglim-sc/README.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml` & `sparglim-0.1.3/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml` & `sparglim-0.1.3/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/dev/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.3/dev/sparglim-server/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/README.md` & `sparglim-0.1.3/examples/jupyter-sparglim-on-k8s/README.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml` & `sparglim-0.1.3/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/examples/jupyter-sparglim-sc/README.md` & `sparglim-0.1.3/examples/jupyter-sparglim-sc/README.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml` & `sparglim-0.1.3/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml` & `sparglim-0.1.3/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/examples/sparglim-server/README.md` & `sparglim-0.1.3/examples/sparglim-server/README.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/examples/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.3/examples/sparglim-server/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/sparglim/utils.py` & `sparglim-0.1.3/sparglim/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,14 +45,25 @@
     jars_dir: Path = Path(spark_home) / "jars"
     for p in jars_dir.glob("spark-core*"):
         # spark-core_2.12-3.4.1.jar -> 2.12
         return p.stem.split("_")[-1].split("-")[0]
     return None
 
 
+def exist_connect_server_package():
+    spark_home = os.getenv("SPARK_HOME")
+    if not spark_home:
+        return False
+    jars_dir: Path = Path(spark_home) / "jars"
+    for p in jars_dir.glob("spark-connect*"):
+        # eg. spark-connect_2.12-3.4.1.jar
+        return True
+    return False
+
+
 class Singleton(type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
```

### Comparing `sparglim-0.1.2/sparglim/config/builder.py` & `sparglim-0.1.3/sparglim/config/builder.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/sparglim/config/configer.py` & `sparglim-0.1.3/sparglim/config/configer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/sparglim/config/k8s.py` & `sparglim-0.1.3/sparglim/config/k8s.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/sparglim/server/cli.py` & `sparglim-0.1.3/sparglim/server/cli.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/sparglim/server/daemon.py` & `sparglim-0.1.3/sparglim/server/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 
 import psutil
 
 from sparglim.config.configer import SparkEnvConfiger
 from sparglim.exceptions import DaemonError, UnconfigurableError
 from sparglim.log import logger
 from sparglim.server.tailer import Tailer
-from sparglim.utils import get_scala_version, get_spark_version, port_is_used
+from sparglim.utils import (
+    exist_connect_server_package,
+    get_scala_version,
+    get_spark_version,
+    port_is_used,
+)
 
 
 class Daemon:
     # This daemon is designed for spark connect server in the frontend
     # Run the connect server in a container and monitor its state, if it is down, restart it
     # Stop the daemon when the KeyboardInterrupt is raised
     # This will not start duplicate connect server, unless using different root_dir and port
@@ -51,21 +56,18 @@
         if not self.start_cmd_path.exists():
             raise UnconfigurableError(
                 f"{self.start_cmd_path.name} not found in $SPARK_HOME/sbin, check your SPARK_HOME"
             )
 
         SPARK_VERSION = os.getenv("SPARK_VERSION", get_spark_version())
         SCALA_VERSION = os.getenv("SCALA_VERSION", get_scala_version())
-        add_connect_package = os.getenv("SPARGLIM_SERVER_CONNECT_PACKAGES", "false") in [
-            "true",
-            "True",
-        ]
         self.daemon_package = []
-        if add_connect_package and (SPARK_VERSION and SCALA_VERSION):
-            # Specify the spark-connect package or use the default one
+        if not exist_connect_server_package() and (SPARK_VERSION and SCALA_VERSION):
+            # Specify the spark-connect package if no such package in $SPARK_HOME/jars
+            # Spark will download the package from maven repo
             self.daemon_package.append(
                 f"org.apache.spark:spark-connect_{SCALA_VERSION}:{SPARK_VERSION}"
             )
         self.builder = SparkEnvConfiger().config_connect_server(
             self.mode, k8s_config_path=k8s_config_path
         )
```

### Comparing `sparglim-0.1.2/sparglim/server/tailer.py` & `sparglim-0.1.3/sparglim/server/tailer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/sparglim/sql/__init__.py` & `sparglim-0.1.3/sparglim/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/sparglim/sql/magic.py` & `sparglim-0.1.3/sparglim/sql/magic.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/tests/conftest.py` & `sparglim-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/tests/test_builder.py` & `sparglim-0.1.3/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/tests/test_daemon.py` & `sparglim-0.1.3/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/tests/test_magic.py` & `sparglim-0.1.3/tests/test_magic.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/tests/mock/sbin/entrypoint.py` & `sparglim-0.1.3/tests/mock/sbin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/tests/mock/sbin/mock_spark_server.py` & `sparglim-0.1.3/tests/mock/sbin/mock_spark_server.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/.gitignore` & `sparglim-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/LICENSE` & `sparglim-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/README.md` & `sparglim-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/pyproject.toml` & `sparglim-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.2/PKG-INFO` & `sparglim-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparglim
-Version: 0.1.2
+Version: 0.1.3
 Summary: sparglim
 Project-URL: Source, https://github.com/wh1isper/sparglim
 Author-email: wh1isper <9573586@qq.com>
 License: BSD license
 License-File: LICENSE
 Keywords: ipython,magic,pyspark,sparglim,spark
 Classifier: Programming Language :: Python :: 3
```

