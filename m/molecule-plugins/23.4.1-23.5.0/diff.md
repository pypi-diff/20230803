# Comparing `tmp/molecule-plugins-23.4.1.tar.gz` & `tmp/molecule-plugins-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-plugins-23.4.1.tar", last modified: Thu Apr 27 17:49:56 2023, max compression
+gzip compressed data, was "molecule-plugins-23.5.0.tar", last modified: Thu Aug  3 12:51:48 2023, max compression
```

## Comparing `molecule-plugins-23.4.1.tar` & `molecule-plugins-23.5.0.tar`

### file list

```diff
@@ -1,319 +1,323 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.922895 molecule-plugins-23.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.850895 molecule-plugins-23.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.850895 molecule-plugins-23.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-27 17:49:56.922895 molecule-plugins-23.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.798894 molecule-plugins-23.4.1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.850895 molecule-plugins-23.4.1/doc/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/doc/ec2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/doc/ec2/platforms.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.850895 molecule-plugins-23.4.1/doc/vagrant/
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/doc/vagrant/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.798894 molecule-plugins-23.4.1/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.850895 molecule-plugins-23.4.1/molecule/test-podman/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/molecule/test-podman/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/molecule/test-podman/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/molecule/test-podman/verify.yml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:49:56.922895 molecule-plugins-23.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.802894 molecule-plugins-23.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.854894 molecule-plugins-23.4.1/src/molecule_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.854894 molecule-plugins-23.4.1/src/molecule_plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.854894 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.802894 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/containers/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/containers/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.806894 molecule-plugins-23.4.1/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/containers/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/docker/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/docker/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.806894 molecule-plugins-23.4.1/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.862894 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.862894 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/filter_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.862894 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/tasks/create_network.yml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/tasks/delete_network.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.862894 molecule-plugins-23.4.1/src/molecule_plugins/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.862894 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.810894 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.814894 molecule-plugins-23.4.1/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/files/windows_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/handlers/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/podman/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/podman/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.818894 molecule-plugins-23.4.1/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.818894 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.874894 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.874894 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24598 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/modules/vagrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.874894 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.854894 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.838894 molecule-plugins-23.4.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.874894 molecule-plugins-23.4.1/test/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.874894 molecule-plugins-23.4.1/test/azure/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/functional/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.822894 molecule-plugins-23.4.1/test/azure/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.822894 molecule-plugins-23.4.1/test/azure/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.826894 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.826894 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.878895 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.878895 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.878895 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.878895 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.878895 molecule-plugins-23.4.1/test/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.882895 molecule-plugins-23.4.1/test/containers/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/functional/test_containers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.830894 molecule-plugins-23.4.1/test/containers/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.830894 molecule-plugins-23.4.1/test/containers/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.830894 molecule-plugins-23.4.1/test/containers/scenarios/driver/containers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.830894 molecule-plugins-23.4.1/test/containers/scenarios/driver/containers/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.882895 molecule-plugins-23.4.1/test/containers/scenarios/driver/containers/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/scenarios/driver/containers/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/scenarios/driver/containers/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.882895 molecule-plugins-23.4.1/test/docker/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/docker/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/docker/scenarios/env-substitution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/docker/scenarios/env-substitution/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.882895 molecule-plugins-23.4.1/test/docker/scenarios/env-substitution/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/env-substitution/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/env-substitution/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/docker/scenarios/with-context/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.886895 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/default/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/default/FOO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.886895 molecule-plugins-23.4.1/test/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.886895 molecule-plugins-23.4.1/test/ec2/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/functional/test_ec2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/ec2/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/ec2/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.886895 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.886895 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.890895 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.890895 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.890895 molecule-plugins-23.4.1/test/gce/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.890895 molecule-plugins-23.4.1/test/gce/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/functional/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.838894 molecule-plugins-23.4.1/test/gce/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.894895 molecule-plugins-23.4.1/test/gce/scenarios/linux/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.894895 molecule-plugins-23.4.1/test/gce/scenarios/linux/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/files/windows_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.894895 molecule-plugins-23.4.1/test/gce/scenarios/linux/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/handlers/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.894895 molecule-plugins-23.4.1/test/gce/scenarios/linux/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/tasks/create_linux_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/tasks/create_windows_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/gce/scenarios/windows/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/gce/scenarios/windows/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/files/windows_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/gce/scenarios/windows/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/handlers/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/gce/scenarios/windows/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/tasks/create_linux_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/tasks/create_windows_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/verify.yml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/podman/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/podman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/podman/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/podman/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/podman/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/vagrant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.902895 molecule-plugins-23.4.1/test/vagrant/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/functional/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.842894 molecule-plugins-23.4.1/test/vagrant/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.842894 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.902895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/config_options/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/config_options/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/config_options/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/config_options/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.902895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.906895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.910895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/hostname/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/hostname/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/hostname/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/hostname/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.910895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/invalid/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/invalid/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/invalid/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.910895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/multi-node/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/multi-node/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/multi-node/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/multi-node/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.914895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/network/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/network/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/network/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/network/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.914895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/provider_config_options/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/provider_config_options/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/provider_config_options/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/provider_config_options/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.918895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/vagrant_root/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/vagrant_root/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/vagrant_root/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/vagrant_root/verify.yml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.918895 molecule-plugins-23.4.1/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/tools/Vagrantfile
--rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/tools/create_testbox.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     6414 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/tools/test-setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.206114 molecule-plugins-23.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/.ansible-lint-ignore
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.158112 molecule-plugins-23.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.158112 molecule-plugins-23.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-03 12:51:48.206114 molecule-plugins-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.138111 molecule-plugins-23.5.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.158112 molecule-plugins-23.5.0/doc/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/doc/ec2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/doc/ec2/platforms.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.158112 molecule-plugins-23.5.0/doc/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/doc/vagrant/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.138111 molecule-plugins-23.5.0/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.158112 molecule-plugins-23.5.0/molecule/test-podman/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/molecule/test-podman/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/molecule/test-podman/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/molecule/test-podman/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:51:48.206114 molecule-plugins-23.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.138111 molecule-plugins-23.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.162112 molecule-plugins-23.5.0/src/molecule_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 12:51:47.000000 molecule-plugins-23.5.0/src/molecule_plugins/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.162112 molecule-plugins-23.5.0/src/molecule_plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.162112 molecule-plugins-23.5.0/src/molecule_plugins/azure/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/azure/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.138111 molecule-plugins-23.5.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.166112 molecule-plugins-23.5.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/azure/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.166112 molecule-plugins-23.5.0/src/molecule_plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.166112 molecule-plugins-23.5.0/src/molecule_plugins/containers/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/containers/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.142111 molecule-plugins-23.5.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.166112 molecule-plugins-23.5.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/containers/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.166112 molecule-plugins-23.5.0/src/molecule_plugins/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/docker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.166112 molecule-plugins-23.5.0/src/molecule_plugins/docker/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/docker/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.142111 molecule-plugins-23.5.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.166112 molecule-plugins-23.5.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/docker/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.166112 molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.166112 molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/filter_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.166112 molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/tasks/create_network.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/tasks/delete_network.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.170112 molecule-plugins-23.5.0/src/molecule_plugins/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.170112 molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.142111 molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.170112 molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/ec2/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.170112 molecule-plugins-23.5.0/src/molecule_plugins/gce/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/gce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.170112 molecule-plugins-23.5.0/src/molecule_plugins/gce/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/gce/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.142111 molecule-plugins-23.5.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.170112 molecule-plugins-23.5.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/gce/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.170112 molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.170112 molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7441 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/files/windows_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.170112 molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/handlers/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.170112 molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.174112 molecule-plugins-23.5.0/src/molecule_plugins/podman/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/podman/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.174112 molecule-plugins-23.5.0/src/molecule_plugins/podman/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/podman/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.142111 molecule-plugins-23.5.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.174112 molecule-plugins-23.5.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/podman/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.174112 molecule-plugins-23.5.0/src/molecule_plugins/podman/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/podman/playbooks/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/podman/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/podman/playbooks/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.174112 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.174112 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.142111 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.174112 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.174112 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/modules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25464 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/modules/vagrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.178113 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/playbooks/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/src/molecule_plugins/vagrant/playbooks/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.162112 molecule-plugins-23.5.0/src/molecule_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-03 12:51:48.000000 molecule-plugins-23.5.0/src/molecule_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-08-03 12:51:48.000000 molecule-plugins-23.5.0/src/molecule_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:51:48.000000 molecule-plugins-23.5.0/src/molecule_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-03 12:51:48.000000 molecule-plugins-23.5.0/src/molecule_plugins.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-03 12:51:48.000000 molecule-plugins-23.5.0/src/molecule_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 12:51:48.000000 molecule-plugins-23.5.0/src/molecule_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.150111 molecule-plugins-23.5.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.178113 molecule-plugins-23.5.0/test/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.178113 molecule-plugins-23.5.0/test/azure/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/functional/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/azure/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/azure/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.178113 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.178113 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.178113 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/multi-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/multi-node/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/multi-node/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.178113 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/azure/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.178113 molecule-plugins-23.5.0/test/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.182113 molecule-plugins-23.5.0/test/containers/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/containers/functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/containers/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/containers/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/containers/functional/test_containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/containers/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/containers/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/containers/scenarios/driver/containers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/containers/scenarios/driver/containers/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.182113 molecule-plugins-23.5.0/test/containers/scenarios/driver/containers/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/containers/scenarios/driver/containers/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/containers/scenarios/driver/containers/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/containers/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.182113 molecule-plugins-23.5.0/test/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/docker/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/docker/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/docker/scenarios/env-substitution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/docker/scenarios/env-substitution/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.182113 molecule-plugins-23.5.0/test/docker/scenarios/env-substitution/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/docker/scenarios/env-substitution/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/docker/scenarios/env-substitution/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/docker/scenarios/with-context/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/docker/scenarios/with-context/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.186113 molecule-plugins-23.5.0/test/docker/scenarios/with-context/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/docker/scenarios/with-context/molecule/default/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/docker/scenarios/with-context/molecule/default/FOO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/docker/scenarios/with-context/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/docker/scenarios/with-context/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/docker/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/docker/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.186113 molecule-plugins-23.5.0/test/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.186113 molecule-plugins-23.5.0/test/ec2/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/functional/test_ec2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/ec2/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/ec2/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.146111 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.186113 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/default/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.186113 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.186113 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.186113 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/ec2/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.190113 molecule-plugins-23.5.0/test/gce/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.190113 molecule-plugins-23.5.0/test/gce/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/functional/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.150111 molecule-plugins-23.5.0/test/gce/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.190113 molecule-plugins-23.5.0/test/gce/scenarios/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.190113 molecule-plugins-23.5.0/test/gce/scenarios/linux/files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7485 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/files/windows_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.194113 molecule-plugins-23.5.0/test/gce/scenarios/linux/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/handlers/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.194113 molecule-plugins-23.5.0/test/gce/scenarios/linux/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/tasks/create_linux_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/tasks/create_windows_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/linux/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.194113 molecule-plugins-23.5.0/test/gce/scenarios/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.194113 molecule-plugins-23.5.0/test/gce/scenarios/windows/files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7485 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/files/windows_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.194113 molecule-plugins-23.5.0/test/gce/scenarios/windows/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/handlers/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.194113 molecule-plugins-23.5.0/test/gce/scenarios/windows/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/tasks/create_linux_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/tasks/create_windows_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/scenarios/windows/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/gce/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.198113 molecule-plugins-23.5.0/test/podman/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/podman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/podman/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/podman/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/podman/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.198113 molecule-plugins-23.5.0/test/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.198113 molecule-plugins-23.5.0/test/vagrant/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/functional/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.150111 molecule-plugins-23.5.0/test/vagrant/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.150111 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.198113 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/config_options/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/config_options/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/config_options/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/config_options/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.202113 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.202113 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/default-compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/default-compat/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/default-compat/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/default-compat/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/default-compat/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.202113 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/hostname/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/hostname/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/hostname/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/hostname/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.202113 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/invalid/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/invalid/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.202113 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/multi-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/multi-node/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/multi-node/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/multi-node/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.206114 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/network/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/network/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/network/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.206114 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/provider_config_options/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/provider_config_options/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/provider_config_options/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/provider_config_options/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.206114 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/vagrant_root/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/vagrant_root/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/vagrant_root/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/vagrant_root/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/test/vagrant/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:48.206114 molecule-plugins-23.5.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/tools/Vagrantfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/tools/create_testbox.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/tools/extract_plugin_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/tools/generate-templates.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6414 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/tools/test-setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-08-03 12:51:28.000000 molecule-plugins-23.5.0/tox.ini
```

### Comparing `molecule-plugins-23.4.1/.github/workflows/release.yml` & `molecule-plugins-23.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/.github/workflows/tox.yml` & `molecule-plugins-23.5.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/.gitignore` & `molecule-plugins-23.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/LICENSE` & `molecule-plugins-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/PKG-INFO` & `molecule-plugins-23.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-plugins
-Version: 23.4.1
+Version: 23.5.0
 Summary: Molecule Plugins
 Author-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 Maintainer-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule-plugins
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule-plugins
```

### Comparing `molecule-plugins-23.4.1/README.md` & `molecule-plugins-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/bindep.txt` & `molecule-plugins-23.5.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/conftest.py` & `molecule-plugins-23.5.0/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/doc/ec2/README.rst` & `molecule-plugins-23.5.0/doc/ec2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 .. code-block:: bash
 
    molecule init role -d ec2 my-role
 
 This will create a new folder *my-role* containing a bare-bone generated
 role like you would do with ``ansible-galaxy init`` command.
 It will also contain a molecule folder with a default scenario
-using the ec2 driver (using ansible community.aws.ec2_instance collection).
+using the ec2 driver (using ansible amazon.aws.ec2_instance collection).
 Install the collection using
 `ansible-galaxy install -r test_requirements.yml`.
 
 In a pre-existing role
 ^^^^^^^^^^^^^^^^^^^^^^
 .. code-block:: bash
```

### Comparing `molecule-plugins-23.4.1/doc/ec2/platforms.rst` & `molecule-plugins-23.5.0/doc/ec2/platforms.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 assign_public_ip            Assign a public ip, default = True
 aws_profile                 Boto profile, default = AWS_PROFILE or omits
 boot_wait_seconds           Amount of time to wait after ssh starts
 cloud_config                Dictionary suitable for instance user_data
 connection_options          See Connection Options section
 image                       AMI to use, see Image Selection section
 image_filters               Filters to select AMI, see Image Selection section
+iam_instance_profile        The IAM instance profile for the instance
 image_name                  Name of AMI, see Image Selection section
 image_owner                 Owner of AMI, see Image Selection section
 instance_type               AWS EC2 instance type, defaults to t3a.medium
 key_inject_method           "cloud-init" or "ec2", see SSH Key section
 key_name                    SSH key name, see SSH Key section
 name                        Name for platform entry, used for Ansible inventory
 private_key_path            SSH key private path, see SSH Key section
```

### Comparing `molecule-plugins-23.4.1/doc/vagrant/README.rst` & `molecule-plugins-23.5.0/doc/vagrant/README.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/pyproject.toml` & `molecule-plugins-23.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -92,25 +92,28 @@
   "ARG",
   "B006",
   "B028",
   "BLE",
   "C901",
   "D",
   "DTZ",
-  "EXE",
   "FBT",
   "INP",
   "ISC",
   "N",
+  "PERF203",
   "PGH",
   "PLR",
   "PT",
   "PTH",
   "RET",
   "S",
+  # not sure we'll open a bug for every TODO.
+  "TD003",
+  "FIX002",
   "TRY",
 ]
 select = ["ALL"]
 target-version = "py39"
 # Same as Black.
 line-length = 88
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst` & `molecule-plugins-23.5.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml`

 * *Files 2% similar despite different names*

```diff
@@ -39,25 +39,25 @@
         ssh_key_file: "{{ keypair_path }}"
       register: key_pair
 
     - name: Create molecule instance(s)
       azure.azcollection.azure_rm_virtualmachine:
         resource_group: "{{ resource_group_name }}"
         name: "{{ item.name }}"
-        vm_size: Standard_A0
+        vm_size: Standard_B1ms
         admin_username: "{{ ssh_user }}"
         public_ip_allocation_method: Dynamic
         ssh_password_enabled: false
         ssh_public_keys:
           - path: "/home/{{ ssh_user }}/.ssh/authorized_keys"
             key_data: "{{ key_pair.ssh_public_key }}"
         image:
           offer: CentOS
           publisher: OpenLogic
-          sku: '7.4'
+          sku: '8_5-gen2'
           version: latest
       register: server
       with_items: "{{ molecule_yml.platforms }}"
       async: 7200
       poll: 0
 
     - name: Wait for instance(s) creation to complete
@@ -72,15 +72,15 @@
         - Convert instance config dict to a list
         - Dump instance config
         - Wait for SSH
 
   handlers:
     - name: Populate instance config dict
       ansible.builtin.set_fact:
-        instance_conf_dict:
+        instance_conf_dict:  # noqa: jinja[spacing]
           {
             "instance": "{{ item.ansible_facts.azure_vm.name }}",
             "address": "{{ item.ansible_facts.azure_vm
               .properties.networkProfile.networkInterfaces[0]
               .properties.ipConfigurations[0]
               .properties.publicIPAddress
               .properties.ipAddress }}",
@@ -95,15 +95,15 @@
       ansible.builtin.set_fact:
         instance_conf: "{{ instance_config_dict.results | map(attribute='ansible_facts.instance_conf_dict') | list }}"
 
     - name: Dump instance config
       ansible.builtin.copy:
         content: "{{ instance_conf | to_json | from_json | to_yaml }}"
         dest: "{{ molecule_instance_config }}"
-        mode: 0664
+        mode: "0664"
 
     - name: Wait for SSH
       ansible.builtin.wait_for:
         port: "{{ ssh_port }}"
         host: "{{ item.address }}"
         search_regex: SSH
         delay: 10
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -24,9 +24,9 @@
         instance_conf: {}
 
   handlers:
     - name: Dump instance config
       ansible.builtin.copy:
         content: "{{ instance_conf | to_json | from_json | to_yaml }}"
         dest: "{{ molecule_instance_config }}"
-        mode: 0644
+        mode: "0644"
 {%- endraw %}
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/azure/driver.py` & `molecule-plugins-23.5.0/src/molecule_plugins/azure/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         instance_config_dict = util.safe_load_file(self._config.driver.instance_config)
 
         return next(
             item for item in instance_config_dict if item["instance"] == instance_name
         )
 
     def sanity_checks(self):
-        # FIXME(decentral1se): Implement sanity checks
+        # TODO(decentral1se): Implement sanity checks
         pass
 
     def template_dir(self):
         """Return path to its own cookiecutterm templates. It is used by init
         command in order to figure out where to load the templates from.
         """
         return os.path.join(os.path.dirname(__file__), "cookiecutter")
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/containers/driver.py` & `molecule-plugins-23.5.0/src/molecule_plugins/containers/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/docker/driver.py` & `molecule-plugins-23.5.0/src/molecule_plugins/docker/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/Dockerfile.j2` & `molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/create.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/create.yml`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
         state: started
         recreate: false
         log_driver: json-file
         command: "{{ (command_directives_dict | default({}))[item.name] | default(omit) }}"
         command_handling: "{{ item.command_handling | default('compatibility') }}"
         user: "{{ item.user | default(omit) }}"
         pid_mode: "{{ item.pid_mode | default(omit) }}"
+        runtime: "{{ item.runtime | default(omit) }}"
         privileged: "{{ item.privileged | default(omit) }}"
         security_opts: "{{ item.security_opts | default(omit) }}"
         devices: "{{ item.devices | default(omit) }}"
         links: "{{ item.links | default(omit) }}"
         volumes: "{{ item.volumes | default(omit) }}"
         mounts: "{{ item.mounts | default(omit) }}"
         tmpfs: "{{ item.tmpfs | default(omit) }}"
@@ -168,15 +169,17 @@
         dns_servers: "{{ item.dns_servers | default(omit) }}"
         etc_hosts: "{{ item.etc_hosts | default(omit) }}"
         env: "{{ item.env | default(omit) }}"
         restart_policy: "{{ item.restart_policy | default(omit) }}"
         restart_retries: "{{ item.restart_retries | default(omit) }}"
         tty: "{{ item.tty | default(omit) }}"
         labels: "{{ molecule_labels | combine(item.labels | default({})) }}"
-        container_default_behavior: "{{ item.container_default_behavior | default('compatibility' if ansible_version.full is version_compare('2.10', '>=') else omit) }}"
+        container_default_behavior: >-
+          {{ item.container_default_behavior
+             | default('compatibility' if ansible_version.full is version_compare('2.10', '>=') else omit) }}
         stop_signal: "{{ item.stop_signal | default(omit) }}"
         kill_signal: "{{ item.kill_signal | default(omit) }}"
         cgroupns_mode: "{{ item.cgroupns_mode | default(omit) }}"
         platform: "{{ item.platform | default(omit) }}"
         comparisons:
           platform: ignore
       register: server
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/destroy.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/destroy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,17 @@
         cacert_path: "{{ item.cacert_path | default((lookup('env', 'DOCKER_CERT_PATH') + '/ca.pem') if lookup('env', 'DOCKER_CERT_PATH') else omit) }}"
         cert_path: "{{ item.cert_path | default((lookup('env', 'DOCKER_CERT_PATH') + '/cert.pem') if lookup('env', 'DOCKER_CERT_PATH') else omit) }}"
         key_path: "{{ item.key_path | default((lookup('env', 'DOCKER_CERT_PATH') + '/key.pem') if lookup('env', 'DOCKER_CERT_PATH') else omit) }}"
         tls_verify: "{{ item.tls_verify | default(lookup('env', 'DOCKER_TLS_VERIFY')) or false }}"
         state: absent
         force_kill: "{{ item.force_kill | default(true) }}"
         keep_volumes: "{{ item.keep_volumes | default(true) }}"
-        container_default_behavior: "{{ item.container_default_behavior | default('compatibility' if ansible_version.full is version_compare('2.10', '>=') else omit) }}"
+        container_default_behavior: >-
+          {{ item.container_default_behavior
+             | default('compatibility' if ansible_version.full is version_compare('2.10', '>=') else omit) }}
       register: server
       loop: "{{ molecule_yml.platforms }}"
       loop_control:
         label: "{{ item.name }}"
       no_log: false
       async: 7200
       poll: 0
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py` & `molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/tasks/create_network.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/tasks/create_network.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst` & `molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 {% raw -%}
 ---
 - name: Create
   hosts: localhost
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
-  collections:
-    - community.aws
-    - community.crypto
   vars:
     # Run config handling
     default_run_id: "{{ lookup('password', '/dev/null chars=ascii_lowercase length=5') }}"
     default_run_config:
       run_id: "{{ default_run_id }}"
 
     run_config_path: "{{ lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY') }}/run-config.yml"
@@ -81,15 +78,15 @@
            | product(molecule_yml.platforms | map('dict2items') | list)
            | map('flatten', levels=1)
            | list
            | map('items2dict')
            | list }}
   pre_tasks:
     - name: Validate platform configurations
-      assert:
+      ansible.builtin.assert:
         that:
           - platforms | length > 0
           - platform.name is string and platform.name | length > 0
           - platform.assign_public_ip is boolean
           - platform.aws_profile is string
           - platform.boot_wait_seconds is integer and platform.boot_wait_seconds >= 0
           - platform.cloud_config is mapping
@@ -116,80 +113,82 @@
         quiet: true
       loop: '{{ platforms }}'
       loop_control:
         loop_var: platform
         label: "{{ platform.name }}"
   tasks:
     - name: Write run config to file
-      copy:
+      ansible.builtin.copy:
         dest: "{{ run_config_path }}"
         content: "{{ run_config | to_yaml }}"
+        mode: "0600"
 
     - name: Generate local key pairs
-      openssh_keypair:
+      community.crypto.openssh_keypair:
         path: "{{ item.private_key_path }}"
         type: rsa
         size: 2048
         regenerate: never
       loop: "{{ platforms }}"
       loop_control:
         label: "{{ item.name }}"
       register: local_keypairs
 
     - name: Look up EC2 AMI(s) by owner and name (if image not set)
-      ec2_ami_info:
+      amazon.aws.ec2_ami_info:
         owners: "{{ item.image_owner }}"
         filters: "{{ item.image_filters | default({}) | combine(image_name_map) }}"
       vars:
-        image_name_map: "{% if item.image_name is defined and item.image_name | length > 0 %}{{ { 'name': item.image_name } }}{% else %}{}{% endif %}"
+        image_name_map: "{% if item.image_name is defined and item.image_name | length > 0 %}{{ {'name': item.image_name} }}{% else %}{}{% endif %}"
       loop: "{{ platforms }}"
       loop_control:
         label: "{{ item.name }}"
       when: not item.image
       register: ami_info
 
     - name: Look up subnets to determine VPCs (if needed)
-      ec2_vpc_subnet_info:
+      amazon.aws.ec2_vpc_subnet_info:
         subnet_ids: "{{ item.vpc_subnet_id }}"
       loop: "{{ platforms }}"
       loop_control:
         label: "{{ item.name }}"
       when: not item.vpc_id
       register: subnet_info
 
     - name: Validate discovered information
-      assert:
+      ansible.builtin.assert:
         that:
           - platform.image or (ami_info.results[index].images | length > 0)
           - platform.vpc_id or (subnet_info.results[index].subnets | length > 0)
         quiet: true
       loop: "{{ platforms }}"
       loop_control:
         loop_var: platform
         index_var: index
         label: "{{ platform.name }}"
 
     - name: Create ephemeral EC2 keys (if needed)
-      ec2_key:
+      amazon.aws.ec2_key:
         profile: "{{ item.aws_profile | default(omit) }}"
         region: "{{ item.region | default(omit) }}"
         name: "{{ item.key_name }}"
         key_material: "{{ local_keypair.public_key }}"
       vars:
         local_keypair: "{{ local_keypairs.results[index] }}"
       loop: "{{ platforms }}"
       loop_control:
         index_var: index
         label: "{{ item.name }}"
       when: item.key_inject_method == "ec2"
       register: ec2_keys
 
     - name: Create ephemeral security groups (if needed)
-      ec2_group:
+      amazon.aws.ec2_security_group:
         profile: "{{ item.aws_profile | default(omit) }}"
+        iam_instance_profile: "{{ item.iam_instance_profile | default(omit) }}"
         region: "{{ item.region | default(omit) }}"
         vpc_id: "{{ item.vpc_id or vpc_subnet.vpc_id }}"
         name: "{{ item.security_group_name }}"
         description: "{{ item.security_group_description }}"
         rules: "{{ item.security_group_rules }}"
         rules_egress: "{{ item.security_group_rules_egress }}"
       vars:
@@ -197,15 +196,15 @@
       loop: "{{ platforms }}"
       loop_control:
         index_var: index
         label: "{{ item.name }}"
       when: item.security_groups | length == 0
 
     - name: Create ephemeral EC2 instance(s)
-      ec2_instance:
+      amazon.aws.ec2_instance:
         profile: "{{ item.aws_profile | default(omit) }}"
         region: "{{ item.region | default(omit) }}"
         filters: "{{ platform_filters }}"
         instance_type: "{{ item.instance_type }}"
         image_id: "{{ platform_image_id }}"
         vpc_subnet_id: "{{ item.vpc_subnet_id }}"
         security_groups: "{{ platform_security_groups }}"
@@ -245,28 +244,30 @@
       loop_control:
         index_var: index
         label: "{{ item.name }}"
       register: ec2_instances_async
       async: 7200
       poll: 0
 
-    - block:
+    - name: Instance boot block
+      when: ec2_instances_async is changed
+      block:
         - name: Wait for instance creation to complete
-          async_status:
+          ansible.builtin.async_status:
             jid: "{{ item.ansible_job_id }}"
           loop: "{{ ec2_instances_async.results }}"
           loop_control:
             index_var: index
             label: "{{ platforms[index].name }}"
           register: ec2_instances
           until: ec2_instances is finished
           retries: 300
 
         - name: Collect instance configs
-          set_fact:
+          ansible.builtin.set_fact:
             instance_config:
               instance: "{{ item.name }}"
               address: "{{ item.assign_public_ip | ternary(instance.public_ip_address, instance.private_ip_address) }}"
               user: "{{ item.ssh_user }}"
               port: "{{ item.ssh_port }}"
               identity_file: "{{ item.private_key_path }}"
               instance_ids:
@@ -276,48 +277,48 @@
           loop: "{{ platforms }}"
           loop_control:
             index_var: index
             label: "{{ item.name }}"
           register: instance_configs
 
         - name: Write Molecule instance configs
-          copy:
+          ansible.builtin.copy:
             dest: "{{ molecule_instance_config }}"
             content: >-
               {{ instance_configs.results
                    | map(attribute='ansible_facts.instance_config')
                    | list
                    | to_json
                    | from_json
                    | to_yaml }}
+            mode: "0600"
 
         - name: Start SSH pollers
-          wait_for:
+          ansible.builtin.wait_for:
             host: "{{ item.address }}"
             port: "{{ item.port }}"
             search_regex: SSH
             delay: 10
             timeout: 320
           loop: "{{ instance_configs.results | map(attribute='ansible_facts.instance_config') | list }}"
           loop_control:
             label: "{{ item.instance }}"
           register: ssh_wait_async
           async: 300
           poll: 0
 
         - name: Wait for SSH
-          async_status:
+          ansible.builtin.async_status:
             jid: "{{ item.ansible_job_id }}"
           loop: "{{ ssh_wait_async.results }}"
           loop_control:
             index_var: index
             label: "{{ platforms[index].name }}"
           register: ssh_wait
-          until: ssh_wait_async is finished
+          until: ssh_wait is finished
           retries: 300
           delay: 1
 
         - name: Wait for boot process to finish
-          pause:
+          ansible.builtin.pause:
             seconds: "{{ platforms | map(attribute='boot_wait_seconds') | max }}"
-      when: ec2_instances_async is changed
 {%- endraw %}
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 {% raw -%}
 ---
 - name: Destroy
   hosts: localhost
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
-  collections:
-    - community.aws
   vars:
     # Run config handling
     default_run_id: "{{ lookup('password', '/dev/null chars=ascii_lowercase length=5') }}"
     default_run_config:
       run_id: "{{ default_run_id }}"
 
     run_config_path: "{{ lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY') }}/run-config.yml"
@@ -42,15 +40,15 @@
            | map('items2dict')
            | list }}
 
     # Stored instance config
     instance_config: "{{ (lookup('file', molecule_instance_config, errors='ignore') or '{}') | from_yaml }}"
   pre_tasks:
     - name: Validate platform configurations
-      assert:
+      ansible.builtin.assert:
         that:
           - platforms | length > 0
           - platform.name is string and platform.name | length > 0
           - platform.aws_profile is string
           - platform.key_inject_method is in ["cloud-init", "ec2"]
           - platform.key_name is string and platform.key_name | length > 0
           - platform.region is string
@@ -61,78 +59,79 @@
         quiet: true
       loop: '{{ platforms }}'
       loop_control:
         loop_var: platform
         label: "{{ platform.name }}"
   tasks:
     - name: Look up subnets to determine VPCs (if needed)
-      ec2_vpc_subnet_info:
+      amazon.aws.ec2_vpc_subnet_info:
         subnet_ids: "{{ item.vpc_subnet_id }}"
       loop: "{{ platforms }}"
       loop_control:
         label: "{{ item.name }}"
       when: not item.vpc_id
       register: subnet_info
 
     - name: Validate discovered information
-      assert:
+      ansible.builtin.assert:
         that: platform.vpc_id or (subnet_info.results[index].subnets | length > 0)
         quiet: true
       loop: "{{ platforms }}"
       loop_control:
         loop_var: platform
         index_var: index
         label: "{{ platform.name }}"
 
     - name: Destroy ephemeral EC2 instances
-      ec2_instance:
+      amazon.aws.ec2_instance:
         profile: "{{ item.aws_profile | default(omit) }}"
         region: "{{ item.region | default(omit) }}"
         instance_ids: "{{ instance_config | map(attribute='instance_ids') | flatten }}"
         state: absent
       loop: "{{ platforms }}"
       loop_control:
         label: "{{ item.name }}"
       register: ec2_instances_async
       async: 7200
       poll: 0
 
     - name: Wait for instance destruction to complete
-      async_status:
+      ansible.builtin.async_status:
         jid: "{{ item.ansible_job_id }}"
       loop: "{{ ec2_instances_async.results }}"
       loop_control:
         index_var: index
         label: "{{ platforms[index].name }}"
       register: ec2_instances
       until: ec2_instances is finished
       retries: 300
 
     - name: Write Molecule instance configs
-      copy:
+      ansible.builtin.copy:
         dest: "{{ molecule_instance_config }}"
         content: "{{ {} | to_yaml }}"
+        mode: "0644"
 
     - name: Destroy ephemeral security groups (if needed)
-      ec2_group:
+      amazon.aws.ec2_security_group:
         profile: "{{ item.aws_profile | default(omit) }}"
         region: "{{ item.region | default(omit) }}"
         vpc_id: "{{ item.vpc_id or vpc_subnet.vpc_id }}"
         name: "{{ item.security_group_name }}"
         state: absent
       vars:
         vpc_subnet: "{{ subnet_info.results[index].subnets[0] }}"
       loop: "{{ platforms }}"
       loop_control:
         index_var: index
         label: "{{ item.name }}"
       when: item.security_groups | length == 0
 
     - name: Destroy ephemeral keys (if needed)
-      ec2_key:
+      amazon.aws.ec2_key:
         profile: "{{ item.aws_profile | default(omit) }}"
         region: "{{ item.region | default(omit) }}"
         name: "{{ item.key_name }}"
         state: absent
       loop: "{{ platforms }}"
       loop_control:
         index_var: index
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/ec2/driver.py` & `molecule-plugins-23.5.0/src/molecule_plugins/ec2/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         data_response = ec2_client.get_password_data(InstanceId=instance_id)
         decoded = b64decode(data_response["PasswordData"])
         with open(key_file, "rb") as f:
             key = load_pem_private_key(f.read(), None, default_backend())
         return key.decrypt(decoded, PKCS1v15()).decode("utf-8")
 
     def sanity_checks(self):
-        # FIXME(decentral1se): Implement sanity checks
+        # TODO(decentral1se): Implement sanity checks
         pass
 
     def template_dir(self):
         """Return path to its own cookiecutterm templates. It is used by init
         command in order to figure out where to load the templates from.
         """
         return os.path.join(os.path.dirname(__file__), "cookiecutter")
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/gce/driver.py` & `molecule-plugins-23.5.0/src/molecule_plugins/gce/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         instance_config_dict = util.safe_load_file(self._config.driver.instance_config)
 
         return next(
             item for item in instance_config_dict if item["instance"] == instance_name
         )
 
     def sanity_checks(self):
-        # FIXME(decentral1se): Implement sanity checks
+        # TODO(decentral1se): Implement sanity checks
         pass
 
     def template_dir(self):
         """Return path to its own cookiecutterm templates. It is used by init
         command in order to figure out where to load the templates from.
         """
         return os.path.join(os.path.dirname(__file__), "cookiecutter")
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/create.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/create.yml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,19 @@
   hosts: localhost
   connection: local
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
   vars:
     ssh_identity_file: "{{ lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY') }}/ssh_key"
     gcp_project_id: "{{ molecule_yml.driver.project_id | default(lookup('env', 'GCE_PROJECT_ID')) }}"
-
+    gcp_net_name: "{{ molecule_yml.driver.network_name | default('default') }}"
+    gcp_project: "{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}"
+    gcp_net: "https://www.googleapis.com/compute/v1/projects/{{ gcp_project }}/global/networks/{{ gcp_net_name }}"
+    gcp_snet_name: "{{ molecule_yml.driver.subnetwork_name | default('default') }}"
+    gcp_snet: "https://compute.googleapis.com/compute/v1/projects/{{ gcp_project }}/regions/{{ molecule_yml.driver.region }}/subnetworks/{{ gcp_snet_name }}"
   tasks:
     - name: Make sure if linux or windows either specified
       ansible.builtin.assert:
         that:
           - molecule_yml.driver.instance_os_type | lower == "linux" or
             molecule_yml.driver.instance_os_type | lower == "windows"
         fail_msg: "instance_os_type is possible only to specify linux or windows either"
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/destroy.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/destroy.yml`

 * *Files 18% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     - name: Destroy molecule instance(s)
       google.cloud.gcp_compute_instance:
         name: "{{ item.name }}"
         state: absent
         zone: "{{ item.zone | default(molecule_yml.driver.region + '-b') }}"
         project: "{{ molecule_yml.driver.project_id | default(lookup('env', 'GCE_PROJECT_ID')) }}"
         scopes: "{{ molecule_yml.driver.scopes | default(['https://www.googleapis.com/auth/compute'], True) }}"
-        service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-        service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+        service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+        service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
         auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
       register: async_results
       loop: "{{ molecule_yml.platforms }}"
       async: 7200
       poll: 0
       notify:
         - "Wipe out instance config"
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/files/windows_auth.py` & `molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/files/windows_auth.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/handlers/main.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/handlers/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 ---
 - name: Populate instance config dict Linux
   ansible.builtin.set_fact:
     instance_conf_dict:
       {
         "instance": "{{ instance_info.name }}",
-        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
-        "user": "{{ lookup('env','USER') }}",
+        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP
+          if molecule_yml.driver.external_access
+          else instance_info.networkInterfaces.0.networkIP }}",
+        "user": "{{ lookup('env', 'USER') }}",
         "port": "22",
         "identity_file": "{{ ssh_identity_file }}",
         "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
       }
   loop: "{{ server.results }}"
   loop_control:
     loop_var: instance_info
@@ -17,15 +19,17 @@
   register: instance_conf_dict
 
 - name: Populate instance config dict Windows
   ansible.builtin.set_fact:
     instance_conf_dict:
       {
         "instance": "{{ instance_info.name }}",
-        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
+        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP
+          if molecule_yml.driver.external_access
+          else instance_info.networkInterfaces.0.networkIP }}",
         "user": "molecule_usr",
         "password": "{{ instance_info.password }}",
         "port": "{{ instance_info.winrm_port | default(5986) }}",
         "winrm_transport": "{{ molecule_yml.driver.winrm_transport | default('ntlm') }}",
         "winrm_server_cert_validation": "{{ molecule_yml.driver.winrm_server_cert_validation | default('ignore') }}",
         "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
       }
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/linux/tasks/create_linux_instance.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 ---
 - name: Create ssh keypair
   community.crypto.openssh_keypair:
-    comment: "{{ lookup('env','USER') }} user for Molecule"
+    comment: "{{ lookup('env', 'USER') }} user for Molecule"
     path: "{{ ssh_identity_file }}"
   register: keypair
 
-- name: "Create molecule Linux instance(s)"
+- name: Create molecule Linux instance(s)
   google.cloud.gcp_compute_instance:
     state: present
     name: "{{ item.name }}"
     machine_type: "{{ item.machine_type | default('n1-standard-1') }}"
     metadata:
-      ssh-keys: "{{ lookup('env','USER') }}:{{ keypair.public_key }}"
-    scheduling:
-      preemptible: "{{ item.preemptible | default(false) }}"
+      ssh-keys: "{{ lookup('env', 'USER') }}:{{ keypair.public_key }}"
     disks:
       - auto_delete: true
         boot: true
         initialize_params:
           disk_size_gb: "{{ item.disk_size_gb | default(omit) }}"
           source_image: "{{ item.image | default('projects/debian-cloud/global/images/family/debian-10') }}"
           source_image_encryption_key:
             raw_key: "{{ item.image_encryption_key | default(omit) }}"
     network_interfaces:
-      - network:
-          selfLink: "https://www.googleapis.com/compute/v1/projects/{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}/global/networks/{{ molecule_yml.driver.network_name | default('default') }}"
-        subnetwork:
-          selfLink: "https://compute.googleapis.com/compute/v1/projects/{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}/regions/{{ molecule_yml.driver.region }}/subnetworks/{{ molecule_yml.driver.subnetwork_name | default('default') }}"
-        access_configs: "{{ [{'name': 'instance_ip', 'type': 'ONE_TO_ONE_NAT'}] if molecule_yml.driver.external_access else [] }}"
+      "{{ [ { 'network': my_network.resources.0 | default(omit), 'subnetwork': my_subnetwork.resources.0 | default(omit) } | combine(external_access_config
+      | default([]) ) ] }}"
     zone: "{{ item.zone | default(molecule_yml.driver.region + '-b') }}"
     project: "{{ gcp_project_id }}"
     scopes: "{{ molecule_yml.driver.scopes | default(['https://www.googleapis.com/auth/compute'], True) }}"
-    service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-    service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+    service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+    service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
     auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
   register: async_results
   loop: "{{ molecule_yml.platforms }}"
   loop_control:
     pause: 3
   async: 7200
   poll: 0
@@ -46,17 +41,17 @@
     jid: "{{ item.ansible_job_id }}"
   loop: "{{ async_results.results }}"
   register: server
   until: server.finished
   retries: 300
   delay: 10
   notify:
-    - "Populate instance config dict Linux"
-    - "Convert instance config dict to a list"
-    - "Dump instance config"
+    - Populate instance config dict Linux
+    - Convert instance config dict to a list
+    - Dump instance config
 
 - name: Wait for SSH
   ansible.builtin.wait_for:
     port: 22
     host: "{{ item.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else item.networkInterfaces.0.networkIP }}"
     search_regex: SSH
     delay: 10
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,23 +12,23 @@
         initialize_params:
           disk_size_gb: "{{ item.disk_size_gb | default(omit) }}"
           source_image: "{{ item.image | default('projects/windows-cloud/global/images/family/windows-2019') }}"
           source_image_encryption_key:
             raw_key: "{{ item.image_encryption_key | default(omit) }}"
     network_interfaces:
       - network:
-          selfLink: "https://www.googleapis.com/compute/v1/projects/{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}/global/networks/{{ molecule_yml.driver.network_name | default('default') }}"
+          selfLink: "{{ gcp_net }}"
         subnetwork:
-          selfLink: "https://compute.googleapis.com/compute/v1/projects/{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}/regions/{{ molecule_yml.driver.region }}/subnetworks/{{ molecule_yml.driver.subnetwork_name | default('default') }}"
+          selfLink: "{{ gcp_snet }}"
         access_configs: "{{ [{'name': 'instance_ip', 'type': 'ONE_TO_ONE_NAT'}] if molecule_yml.driver.external_access else [] }}"
     zone: "{{ item.zone | default(molecule_yml.driver.region + '-b') }}"
     project: "{{ gcp_project_id }}"
     scopes: "{{ molecule_yml.driver.scopes | default(['https://www.googleapis.com/auth/compute'], True) }}"
-    service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-    service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+    service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+    service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
     auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
   register: async_results
   loop: "{{ molecule_yml.platforms }}"
   async: 7200
   poll: 0
 
 - name: Wait for instance(s) creation to complete
@@ -48,25 +48,30 @@
   ansible.builtin.wait_for:
     port: 5986
     host: "{{ item.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else item.networkInterfaces.0.networkIP }}"
     delay: 10
   loop: "{{ server.results }}"
 
 - name: Prepare Windows User
-  ansible.builtin.script: ./files/windows_auth.py --instance {{ item.name }} --zone {{ item.zone | default(molecule_yml.driver.region + '-b') }} --project {{ gcp_project_id }} --username molecule_usr
+  ansible.builtin.script: >
+    ./files/windows_auth.py
+    --instance {{ item.name }}
+    --zone {{ item.zone | default(molecule_yml.driver.region + '-b') }}
+    --project {{ gcp_project_id }}
+    --username molecule_usr
   args:
     executable: python3
   environment:
     GOOGLE_APPLICATION_CREDENTIALS: "{{ molecule_yml.driver.service_account_file | default(lookup('env', 'GCP_SERVICE_ACCOUNT_FILE'), true) }}"
   loop: "{{ molecule_yml.platforms }}"
   changed_when:
     - password.rc == 0
     - password.stdout
   register: password
   retries: 10
   delay: 10
 
 - name: Add password for instances in server list
   ansible.builtin.set_fact:
-    win_instances: "{{ win_instances|default([]) + [dict(item[0], password=item[1].stdout_lines |last)] }}"
+    win_instances: "{{ win_instances | default([]) + [dict(item[0], password=item[1].stdout_lines | last)] }}"
   loop: "{{ server.results | zip(password.results) | list }}"
   no_log: true
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/podman/driver.py` & `molecule-plugins-23.5.0/src/molecule_plugins/podman/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
           image: centos:8
           privileged: true
           command: "/usr/sbin/init"
           tty: True
 
     .. code-block:: bash
 
-        $ python3 -m pip install molecule[podman]
+        $ python3 -m pip install molecule-plugins[podman]
 
     When pulling from a private registry, it is the user's discretion to decide
     whether to use hard-code strings or environment variables for passing
     credentials to molecule.
 
     .. important::
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/Dockerfile.j2` & `molecule-plugins-23.5.0/src/molecule_plugins/podman/playbooks/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/create.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/podman/playbooks/create.yml`

 * *Files 5% similar despite different names*

```diff
@@ -13,26 +13,40 @@
       register: _podman_path
       changed_when: false
 
     - name: Register podman executable path
       ansible.builtin.set_fact:
         podman_cmd: "{{ _podman_path.stdout }}"
 
+    - name: Get passwd entries for USER env
+      ansible.builtin.getent:
+        database: passwd
+        key: "{{ lookup('env', 'USER') }}"
+
+    - name: Get shell async_dir
+      ansible.builtin.set_fact:
+        _shell_async_dir: >-
+          {{ lookup('ansible.builtin.config', 'async_dir', plugin_type='shell', plugin_name='sh')
+             | regex_replace('^~', ansible_facts.getent_passwd[lookup('env', 'USER')][4]) }}
+
     - name: Set async_dir for HOME env
       ansible.builtin.set_fact:
-        ansible_async_dir: "{{ lookup('env', 'HOME') }}/.ansible_async/"
-      when: (lookup('env', 'HOME'))
+        ansible_async_dir: >-
+          {{ _shell_async_dir
+             | regex_replace('^' + ansible_facts.getent_passwd[lookup('env', 'USER')][4], lookup('env', 'HOME')) }}
+      when: lookup('env', 'HOME') != ansible_facts.getent_passwd[lookup('env', 'USER')][4]
 
     - name: Log into a container registry
       ansible.builtin.command: >
         {{ podman_cmd }} login
         --username {{ item.registry.credentials.username }}
         --password {{ item.registry.credentials.password }}
         --tls-verify={{ item.tls_verify | default(lookup('env', 'DOCKER_TLS_VERIFY')) or false }}
-        {% if lookup('env', 'DOCKER_CERT_PATH') %}--cert-dir {{ item.cert_path | default(lookup('env', 'DOCKER_CERT_PATH') + '/cert.pem') }}{% endif %}
+        {% if lookup('env', 'DOCKER_CERT_PATH') %}
+        --cert-dir {{ item.cert_path | default(lookup('env', 'DOCKER_CERT_PATH') + '/cert.pem') }}{% endif %}
         {{ item.registry.url }}
       with_items: "{{ molecule_yml.platforms }}"
       loop_control:
         label: >-
           "{{ item.name }} registry username:
           {{ item.registry.credentials.username | default('None specified') }}"
       when:
@@ -82,15 +96,15 @@
     - name: Build an Ansible compatible image # noqa: no-handler
       ansible.builtin.command: >
         {{ podman_cmd }} build
         -f {{ item.dest }}
         -t molecule_local/{{ item.item.image }}
         {% if item.item.buildargs is defined %}{% for i, k in item.item.buildargs.items() %}--build-arg={{ i }}={{ k }}{% endfor %}{% endif %}
         {% if item.item.pull is defined %}--pull={{ item.item.pull }}{% endif %}
-        {{ molecule_scenario_directory + '/' + (item.item.dockerfile | default( 'Dockerfile.j2')) | dirname }}
+        {{ molecule_scenario_directory + '/' + (item.item.dockerfile | default('Dockerfile.j2')) | dirname }}
       with_items: "{{ platforms.results }}"
       loop_control:
         label: "{{ item.item.image | default('None specified') }}"
       when:
         - platforms.changed or podman_images.results | map(attribute='images') | select('equalto', []) | list | count >= 0
         - not item.item.pre_build_image | default(false)
       register: result
@@ -165,19 +179,21 @@
         {% if item.tmpfs is defined %}{% for i in item.tmpfs %}--tmpfs={{ i }} {% endfor %}{% endif %}
         {% if item.capabilities is defined %}{% for i in item.capabilities %}--cap-add={{ i }} {% endfor %}{% endif %}
         {% if item.exposed_ports is defined %}--expose="{{ item.exposed_ports | join(',') }}"{% endif %}
         {% if item.published_ports is defined %}{% for i in item.published_ports %}--publish={{ i }} {% endfor %}{% endif %}
         {% if item.ulimits is defined %}{% for i in item.ulimits %}--ulimit={{ i }} {% endfor %}{% endif %}
         {% if item.dns_servers is defined %}--dns="{{ item.dns_servers | join(',') }}"{% endif %}
         {% if item.env is defined %}{% for i, k in item.env.items() %}--env={{ i }}={{ k }} {% endfor %}{% endif %}
-        {% if item.restart_policy is defined %}--restart={{ item.restart_policy }}{% if item.restart_retries is defined %}:{{ item.restart_retries }}{% endif %}{% endif %}
+        {% if item.restart_policy is defined %}
+        --restart={{ item.restart_policy }}{% if item.restart_retries is defined %}:{{ item.restart_retries }}{% endif %}{% endif %}
         {% if item.tty is defined %}--tty={{ item.tty }}{% endif %}
         {% if item.network is defined %}--network={{ item.network }}{% endif %}
         {% if item.ip is defined %}--ip={{ item.ip }}{% endif %}
-        {% if item.etc_hosts is defined %}{% for i, k in item.etc_hosts.items() %}{% if i != item.name %}--add-host {{ i }}:{{ k }} {% endif %}{% endfor %}{% endif %}
+        {% if item.etc_hosts is defined %}
+        {% for i, k in item.etc_hosts.items() %}{% if i != item.name %}--add-host {{ i }}:{{ k }} {% endif %}{% endfor %}{% endif %}
         {% if item.hostname is defined %}--hostname={{ item.hostname }}{% elif item.name is defined %}--hostname={{ item.name }}{% endif %}
         {% if item.systemd is defined %}--systemd={{ item.systemd | string | lower }}{% endif %}
         {{ item.extra_opts | default([]) | join(' ') }}
         {{ item.pre_build_image | default(false) | ternary('', 'molecule_local/') }}{{ item.image }}
         {{ (command_directives_dict | default({}))[item.name] | default('') }}
       register: server
       with_items: "{{ molecule_yml.platforms }}"
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/destroy.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,63 @@
 ---
-- name: Destroy
-  hosts: localhost
-  connection: local
-  gather_facts: false
-  no_log: "{{ molecule_no_log }}"
-  become: "{{ not (item.rootless|default(true)) }}"
-  vars:
-    podman_exec: "{{ lookup('env','MOLECULE_PODMAN_EXECUTABLE')|default('podman',true) }}"
-  tasks:
-    - name: Set async_dir for HOME env
-      ansible.builtin.set_fact:
-        ansible_async_dir: "{{ lookup('env', 'HOME') }}/.ansible_async/"
-      when: (lookup('env', 'HOME'))
+- name: Create ssh keypair
+  community.crypto.openssh_keypair:
+    comment: "{{ lookup('env', 'USER') }} user for Molecule"
+    path: "{{ ssh_identity_file }}"
+  register: keypair
 
-    - name: Destroy molecule instance(s)
-      ansible.builtin.shell: "{{ podman_exec }} container exists {{ item.name }} && {{ podman_exec }} rm -f {{ item.name }} || true"
-      register: server
-      with_items: "{{ molecule_yml.platforms }}"
-      async: 7200
-      poll: 0
-      changed_when: true
+- name: "Create molecule Linux instance(s)"
+  google.cloud.gcp_compute_instance:
+    state: present
+    name: "{{ item.name }}"
+    machine_type: "{{ item.machine_type | default('n1-standard-1') }}"
+    metadata:
+      ssh-keys: "{{ lookup('env', 'USER') }}:{{ keypair.public_key }}"
+    scheduling:
+      preemptible: "{{ item.preemptible | default(false) }}"
+    disks:
+      - auto_delete: true
+        boot: true
+        initialize_params:
+          disk_size_gb: "{{ item.disk_size_gb | default(omit) }}"
+          source_image: "{{ item.image | default('projects/debian-cloud/global/images/family/debian-10') }}"
+          source_image_encryption_key:
+            raw_key: "{{ item.image_encryption_key | default(omit) }}"
+    network_interfaces:
+      - network:
+          selfLink: "{{ gcp_net }}"
+        subnetwork:
+          selfLink: "{{ gcp_snet }}"
+        access_configs: "{{ [{'name': 'instance_ip', 'type': 'ONE_TO_ONE_NAT'}] if molecule_yml.driver.external_access else [] }}"
+    zone: "{{ item.zone | default(molecule_yml.driver.region + '-b') }}"
+    project: "{{ gcp_project_id }}"
+    scopes: "{{ molecule_yml.driver.scopes | default(['https://www.googleapis.com/auth/compute'], True) }}"
+    service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+    service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
+    auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
+  register: async_results
+  loop: "{{ molecule_yml.platforms }}"
+  loop_control:
+    pause: 3
+  async: 7200
+  poll: 0
 
-    - name: Wait for instance(s) deletion to complete
-      become: "{{ not item.item.rootless | default(omit) }}"
-      ansible.builtin.async_status:
-        jid: "{{ item.ansible_job_id }}"
-      register: podman_jobs
-      until: podman_jobs.finished
-      retries: 300
-      with_items: "{{ server.results }}"
+- name: Wait for instance(s) creation to complete
+  ansible.builtin.async_status:
+    jid: "{{ item.ansible_job_id }}"
+  loop: "{{ async_results.results }}"
+  register: server
+  until: server.finished
+  retries: 300
+  delay: 10
+  notify:
+    - "Populate instance config dict Linux"
+    - "Convert instance config dict to a list"
+    - "Dump instance config"
 
-    - name: Delete podman network dedicated to this scenario
-      containers.podman.podman_network:
-        name: "{{ item.network }}"
-        executable: "{{ podman_exec }}"
-        state: absent
-      when:
-        - item.network is defined
-      loop: "{{ molecule_yml.platforms | flatten(levels=1) }}"
-      loop_control:
-        extended: true
-        label: "{{ item.name }}: {{ item.network | default('None specified') }}"
+- name: Wait for SSH
+  ansible.builtin.wait_for:
+    port: 22
+    host: "{{ item.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else item.networkInterfaces.0.networkIP }}"
+    search_regex: SSH
+    delay: 10
+  loop: "{{ server.results }}"
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst` & `molecule-plugins-23.5.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/driver.py` & `molecule-plugins-23.5.0/src/molecule_plugins/vagrant/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/modules/vagrant.py` & `molecule-plugins-23.5.0/src/molecule_plugins/vagrant/modules/vagrant.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 
 import contextlib
+import copy
 import datetime
 import os
 import subprocess
 import sys
+from collections.abc import MutableMapping
 
+import jinja2
 from ansible.module_utils.basic import AnsibleModule
 
-import molecule
-import molecule.util
-
 try:
     import vagrant
 except ImportError:
     sys.exit("ERROR: Driver missing, install python-vagrant.")
 ANSIBLE_METADATA = {
     "metadata_version": "0.1",
     "status": ["preview"],
@@ -195,14 +195,16 @@
 {%- macro dict2args(dictionary) -%}
   {% set sep = joiner(", ") %}
   {%- for key, value in dictionary.items() -%}
     {{ sep() }}{{ key }}: {{ ruby_format(value) }}
   {%- endfor -%}
 {%- endmacro -%}
 
+# Ansible managed
+
 Vagrant.configure('2') do |config|
   if Vagrant.has_plugin?('vagrant-cachier')
     {% if cachier is not none and cachier in [ "machine", "box" ] %}
     config.cache.scope = '{{ cachier }}'
     {% else %}
     config.cache.disable!
     {% endif %}
@@ -210,18 +212,18 @@
 
 {% for instance in instances %}
   config.vm.define "{{ instance.name }}" do |c|
     ##
     # Box definition
     ##
     c.vm.box = "{{ instance.box }}"
-    {{ 'c.vm.box_version = "{}"'.format(instance.box_version) if instance.box_version }}
-    {{ 'c.vm.box_url = "{}"'.format(instance.box_url) if instance.box_url }}
-    {{ 'c.vm.box_download_checksum = "{}"'.format(instance.box_download_checksum) if instance.box_download_checksum }}
-    {{ 'c.vm.box_download_checksum_type = "{}"'.format(instance.box_download_checksum_type) if instance.box_download_checksum_type }}
+    {{ 'c.vm.box_version = "{}"'.format(instance.box_version) | safe if instance.box_version }}
+    {{ 'c.vm.box_url = "{}"'.format(instance.box_url) | safe if instance.box_url }}
+    {{ 'c.vm.box_download_checksum = "{}"'.format(instance.box_download_checksum) | safe if instance.box_download_checksum }}
+    {{ 'c.vm.box_download_checksum_type = "{}"'.format(instance.box_download_checksum_type) | safe if instance.box_download_checksum_type }}
 
     ##
     # Config options
     ##
     {% if instance.config_options['synced_folder'] is sameas false %}
     c.vm.synced_folder ".", "/vagrant", disabled: true
     {% endif %}
@@ -255,14 +257,17 @@
     ##
     # Provider
     ##
     c.vm.provider "{{ instance.provider }}" do |{{ instance.provider | lower }}, override|
       {% if instance.provider == "vsphere" %}
       {{ instance.provider | lower }}.memory_mb = {{ instance.memory }}
       {{ instance.provider | lower }}.cpu_count = {{ instance.cpus }}
+      {% elif instance.provider == 'vmware_esxi' %}
+      {{ instance.provider | lower }}.guest_memsize = {{ instance.memory }}
+      {{ instance.provider | lower }}.guest_numvcpus = {{ instance.cpus }}
       {% elif instance.provider.startswith('vmware_') %}
       {{ instance.provider | lower }}.vmx['memsize'] = {{ instance.memory }}
       {{ instance.provider | lower }}.vmx['numvcpus'] = {{ instance.cpus }}
       {% else %}
       {{ instance.provider | lower }}.memory = {{ instance.memory }}
       {{ instance.provider | lower }}.cpus = {{ instance.cpus }}
       {% endif %}
@@ -331,14 +336,35 @@
 stderr:
     description: Output on stderr
     returned: changed
     type: str
 """
 
 
+# Taken from molecule.util.
+def merge_dicts(a: MutableMapping, b: MutableMapping) -> MutableMapping:
+    """Merge the values of b into a and returns a new dict.
+
+    This function uses the same algorithm as Ansible's `combine(recursive=True)` filter.
+
+    :param a: the target dictionary
+    :param b: the dictionary to import
+    :return: dict
+    """
+    result = copy.deepcopy(a)
+
+    for k, v in b.items():
+        if k in a and isinstance(a[k], dict) and isinstance(v, dict):
+            result[k] = merge_dicts(a[k], v)
+        else:
+            result[k] = v
+
+    return result
+
+
 class VagrantClient:
     def __init__(self, module) -> None:
         self._module = module
         self.provision = self._module.params["provision"]
         self.cachier = self._module.params["cachier"]
 
         # compat
@@ -441,17 +467,15 @@
                 )
             self._module.exit_json(
                 changed=changed,
                 log=self._get_stdout_log(),
                 results=self._conf(),
             )
 
-        msg = "Failed to start the VM(s): See log file '{}'".format(
-            self._get_stderr_log(),
-        )
+        msg = f"Failed to start the VM(s): See log file '{self._get_stderr_log()}'"
         with open(self._get_stderr_log(), encoding="utf-8") as f:
             self.result["stderr"] = f.read()
         self._module.fail_json(msg=msg, **self.result)
 
     def destroy(self):
         changed = False
         if self._created() > 0:
@@ -544,21 +568,23 @@
                 msg="Either workdir parameter or MOLECULE_EPHEMERAL_DIRECTORY env variable has to be set",
             )
         conf["vagrantfile"] = os.path.join(conf["workdir"], "Vagrantfile")
         return conf
 
     def _write_vagrantfile(self):
         instances = self._get_vagrant_config_dict()
-        template = molecule.util.render_template(
-            VAGRANTFILE_TEMPLATE,
+        j_env = jinja2.Environment(autoescape=True)
+        t = j_env.from_string(VAGRANTFILE_TEMPLATE)
+        template = t.render(
             instances=instances,
             cachier=self.cachier,
             no_kvm=not os.path.exists("/dev/kvm"),
         )
-        molecule.util.write_file(self._vagrantfile, template)
+        with open(self._vagrantfile, "w") as f:
+            f.write(template)
 
     def _write_configs(self):
         self._write_vagrantfile()
         try:
             self._vagrant.validate(self._config["workdir"])
         except subprocess.CalledProcessError as e:
             self._module.fail_json(
@@ -624,38 +650,39 @@
             "provider": self._module.params["provider_name"],
             "provider_options": {},
             "provider_raw_config_args": instance.get("provider_raw_config_args", None),
             "provider_override_args": instance.get("provider_override_args", None),
         }
 
         d["config_options"].update(
-            molecule.util.merge_dicts(
+            merge_dicts(
                 d["config_options"],
                 instance.get("config_options", {}),
             ),
         )
         if "cachier" in d["config_options"]:
             self.cachier = d["config_options"]["cachier"]
             self._module.warn(
                 "Please convert your molecule.yml to move cachier parameter to driver:. Compat layer will be removed later.",
             )
 
         d["provider_options"].update(
-            molecule.util.merge_dicts(
+            merge_dicts(
                 d["provider_options"],
                 instance.get("provider_options", {}),
             ),
         )
 
         return d
 
     def _get_vagrant_config_dict(self):
-        config_list = []
-        for instance in self.instances:
-            config_list.append(self._get_instance_vagrant_config_dict(instance))
+        config_list = [
+            self._get_instance_vagrant_config_dict(instance)
+            for instance in self.instances
+        ]
         return config_list
 
     def _get_stdout_log(self):
         return self._get_vagrant_log("out")
 
     def _get_stderr_log(self):
         return self._get_vagrant_log("err")
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/create.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/vagrant/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/destroy.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/vagrant/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/prepare.yml` & `molecule-plugins-23.5.0/src/molecule_plugins/vagrant/playbooks/prepare.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins.egg-info/PKG-INFO` & `molecule-plugins-23.5.0/src/molecule_plugins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-plugins
-Version: 23.4.1
+Version: 23.5.0
 Summary: Molecule Plugins
 Author-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 Maintainer-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule-plugins
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule-plugins
```

### Comparing `molecule-plugins-23.4.1/src/molecule_plugins.egg-info/SOURCES.txt` & `molecule-plugins-23.5.0/src/molecule_plugins.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .ansible-lint
+.ansible-lint-ignore
 .flake8
 .gitignore
 .pre-commit-config.yaml
 LICENSE
+MANIFEST.in
 README.md
 bindep.txt
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 requirements.yml
@@ -199,8 +201,10 @@
 test/vagrant/scenarios/molecule/provider_config_options/molecule.yml
 test/vagrant/scenarios/molecule/provider_config_options/verify.yml
 test/vagrant/scenarios/molecule/vagrant_root/converge.yml
 test/vagrant/scenarios/molecule/vagrant_root/molecule.yml
 test/vagrant/scenarios/molecule/vagrant_root/verify.yml
 tools/Vagrantfile
 tools/create_testbox.sh
+tools/extract_plugin_names.py
+tools/generate-templates.sh
 tools/test-setup.sh
```

### Comparing `molecule-plugins-23.4.1/test/azure/functional/conftest.py` & `molecule-plugins-23.5.0/test/azure/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/azure/functional/test_azure.py` & `molecule-plugins-23.5.0/test/azure/functional/test_azure.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py` & `molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml` & `molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py` & `molecule-plugins-23.5.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/containers/functional/conftest.py` & `molecule-plugins-23.5.0/test/containers/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/containers/functional/test_containers.py` & `molecule-plugins-23.5.0/test/containers/functional/test_containers.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/docker/test_func.py` & `molecule-plugins-23.5.0/test/docker/test_func.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/ec2/functional/conftest.py` & `molecule-plugins-23.5.0/test/ec2/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/ec2/functional/test_ec2.py` & `molecule-plugins-23.5.0/test/ec2/functional/test_ec2.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py` & `molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml` & `molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py` & `molecule-plugins-23.5.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/gce/functional/conftest.py` & `molecule-plugins-23.5.0/test/gce/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/gce/functional/test_func.py` & `molecule-plugins-23.5.0/test/gce/functional/test_func.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/linux/INSTALL.md` & `molecule-plugins-23.5.0/test/gce/scenarios/linux/INSTALL.md`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/linux/create.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/linux/create.yml`

 * *Files 8% similar despite different names*

```diff
@@ -6,55 +6,54 @@
   no_log: "{{ molecule_no_log }}"
   vars:
     ssh_identity_file: "{{ lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY') }}/ssh_key"
     gcp_project_id: "{{ molecule_yml.driver.project_id | default(lookup('env', 'GCE_PROJECT_ID')) }}"
 
   tasks:
     - name: Make sure if linux or windows either specified
-      assert:
+      ansible.builtin.assert:
         that:
-          - molecule_yml.driver.instance_os_type | lower == "linux" or
-            molecule_yml.driver.instance_os_type | lower == "windows"
-        fail_msg: "instance_os_type is possible only to specify linux or windows either"
+          - molecule_yml.driver.instance_os_type | lower == "linux" or molecule_yml.driver.instance_os_type | lower == "windows"
+        fail_msg: instance_os_type is possible only to specify linux or windows either
 
     - name: Get network info
       google.cloud.gcp_compute_network_info:
         filters:
           - name = "{{ molecule_yml.driver.network_name | default('default') }}"
         project: "{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}"
-        service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-        service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+        service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+        service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
         auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
       register: my_network
 
     - name: Get subnetwork info
       google.cloud.gcp_compute_subnetwork_info:
         filters:
           - name = "{{ molecule_yml.driver.subnetwork_name | default('default') }}"
         project: "{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}"
         region: "{{ molecule_yml.driver.region }}"
-        service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-        service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+        service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+        service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
         auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
       register: my_subnetwork
 
     - name: Set external access config
-      set_fact:
+      ansible.builtin.set_fact:
         external_access_config:
           - access_configs:
-              - name: "External NAT"
-                type: "ONE_TO_NAT"
+              - name: External NAT
+                type: ONE_TO_NAT
       when: molecule_yml.driver.external_access
 
     - name: Include create_linux_instance tasks
-      include_tasks: tasks/create_linux_instance.yml
+      ansible.builtin.include_tasks: tasks/create_linux_instance.yml
       when:
         - molecule_yml.driver.instance_os_type  | lower == "linux"
 
     - name: Include create_windows_instance tasks
-      include_tasks: tasks/create_windows_instance.yml
+      ansible.builtin.include_tasks: tasks/create_windows_instance.yml
       when:
         - molecule_yml.driver.instance_os_type  | lower == "windows"
 
   handlers:
     - name: Import main handler tasks
-      import_tasks: handlers/main.yml
+      ansible.builtin.import_tasks: handlers/main.yml
```

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/linux/destroy.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/linux/destroy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -9,30 +9,30 @@
     - name: Destroy molecule instance(s)
       google.cloud.gcp_compute_instance:
         name: "{{ item.name }}"
         state: absent
         zone: "{{ item.zone | default(molecule_yml.driver.region + '-b') }}"
         project: "{{ molecule_yml.driver.project_id | default(lookup('env', 'GCE_PROJECT_ID')) }}"
         scopes: "{{ molecule_yml.driver.scopes | default(['https://www.googleapis.com/auth/compute'], True) }}"
-        service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-        service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+        service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+        service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
         auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
       register: async_results
       loop: "{{ molecule_yml.platforms }}"
       async: 7200
       poll: 0
       notify:
-        - "Wipe out instance config"
-        - "Dump instance config"
+        - Wipe out instance config
+        - Dump instance config
 
     - name: Wait for instance(s) deletion to complete
-      async_status:
+      ansible.builtin.async_status:
         jid: "{{ item.ansible_job_id }}"
       register: server
       until: server.finished
       retries: 300
       delay: 10
       loop: "{{ async_results.results }}"
 
   handlers:
     - name: Import main handler tasks
-      import_tasks: handlers/main.yml
+      ansible.builtin.import_tasks: handlers/main.yml
```

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/linux/files/windows_auth.py` & `molecule-plugins-23.5.0/test/gce/scenarios/linux/files/windows_auth.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/linux/handlers/main.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/linux/handlers/main.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 ---
 - name: Populate instance config dict Linux
-  set_fact:
+  ansible.builtin.set_fact:
     instance_conf_dict:
-      {
-        "instance": "{{ instance_info.name }}",
-        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
-        "user": "{{ lookup('env','USER') }}",
-        "port": "22",
-        "identity_file": "{{ ssh_identity_file }}",
-        "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
-      }
+      instance: "{{ instance_info.name }}"
+      address:
+        "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP
+        }}"
+      user: "{{ lookup('env', 'USER') }}"
+      port: "22"
+      identity_file: "{{ ssh_identity_file }}"
+      instance_os_type: "{{ molecule_yml.driver.instance_os_type }}"
   loop: "{{ server.results }}"
   loop_control:
     loop_var: instance_info
   no_log: true
   register: instance_conf_dict
 
 - name: Populate instance config dict Windows
-  set_fact:
+  ansible.builtin.set_fact:
     instance_conf_dict:
-      {
-        "instance": "{{ instance_info.name }}",
-        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
-        "user": "molecule_usr",
-        "password": "{{ instance_info.password }}",
-        "port": "{{ instance_info.winrm_port | default(5986) }}",
-        "winrm_transport": "{{ molecule_yml.driver.winrm_transport | default('ntlm') }}",
-        "winrm_server_cert_validation": "{{ molecule_yml.driver.winrm_server_cert_validation | default('ignore') }}",
-        "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
-      }
+      instance: "{{ instance_info.name }}"
+      address:
+        "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP
+        }}"
+      user: molecule_usr
+      password: "{{ instance_info.password }}"
+      port: "{{ instance_info.winrm_port | default(5986) }}"
+      winrm_transport: "{{ molecule_yml.driver.winrm_transport | default('ntlm') }}"
+      winrm_server_cert_validation: "{{ molecule_yml.driver.winrm_server_cert_validation | default('ignore') }}"
+      instance_os_type: "{{ molecule_yml.driver.instance_os_type }}"
   loop: "{{ win_instances }}"
   loop_control:
     loop_var: instance_info
   no_log: true
   register: instance_conf_dict
 
 - name: Wipe out instance config
-  set_fact:
+  ansible.builtin.set_fact:
     instance_conf: {}
-
 - name: Convert instance config dict to a list
-  set_fact:
+  ansible.builtin.set_fact:
     instance_conf: "{{ instance_conf_dict.results | map(attribute='ansible_facts.instance_conf_dict') | list }}"
 
 - name: Dump instance config
-  copy:
+  ansible.builtin.copy:
     content: "{{ instance_conf }}"
     dest: "{{ molecule_instance_config }}"
     mode: "0600"
```

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/linux/molecule.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/windows/molecule.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ---
 dependency:
   name: galaxy
 driver:
   name: gce
   project_id: change-to-id-of-the-gcp-project # if not set, will default to env GCE_PROJECT_ID
-  auth_kind: null # set to machineaccount or serviceaccount or application - if set to null will read env GCP_AUTH_KIND
-  service_account_email: null # set to an email associated with the project - if set to null, will default to GCP_SERVICE_ACCOUNT_EMAIL. Should not be set if using auth_kind serviceaccount.
-  service_account_file: null # set to the path to the JSON credentials file - if set to null, will default to env GCP_SERVICE_ACCOUNT_FILE
+  auth_kind: # set to machineaccount or serviceaccount or application - if set to null will read env GCP_AUTH_KIND
+  service_account_email: # set to an email associated with the project - if set to null, will default to GCP_SERVICE_ACCOUNT_EMAIL. Should not be set if using auth_kind serviceaccount.
+  service_account_file: # set to the path to the JSON credentials file - if set to null, will default to env GCP_SERVICE_ACCOUNT_FILE
   region: us-west1 # REQUIRED. example: us-central1
   external_access: false # chose whether to create a public IP for the VM or not - default is private IP only
-  instance_os_type: linux # will be considered linux by default, but can be explicitely set to windows
+  instance_os_type: windows # will be considered linux by default, but can be explicitely set to windows
 platforms:
   - name: linuxgce-createdbymolecule # is an instance name
     machine_type: n1-standard-1 # define your machine type
-    zone: null # example: us-west1-b, will default to zone b of driver.region
+    zone: # example: us-west1-b, will default to zone b of driver.region
 provisioner:
   name: ansible
 verifier:
   name: ansible
```

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/linux/tasks/create_linux_instance.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/windows/tasks/create_linux_instance.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 ---
 - name: Create ssh keypair
   community.crypto.openssh_keypair:
-    comment: "{{ lookup('env','USER') }} user for Molecule"
+    comment: "{{ lookup('env', 'USER') }} user for Molecule"
     path: "{{ ssh_identity_file }}"
   register: keypair
 
 - name: Create molecule Linux instance(s)
   google.cloud.gcp_compute_instance:
     state: present
     name: "{{ item.name }}"
     machine_type: "{{ item.machine_type | default('n1-standard-1') }}"
     metadata:
-      ssh-keys: "{{ lookup('env','USER') }}:{{ keypair.public_key }}}"
+      ssh-keys: "{{ lookup('env', 'USER') }}:{{ keypair.public_key }}"
     disks:
       - auto_delete: true
         boot: true
         initialize_params:
           disk_size_gb: "{{ item.disk_size_gb | default(omit) }}"
           source_image: "{{ item.image | default('projects/debian-cloud/global/images/family/debian-10') }}"
           source_image_encryption_key:
             raw_key: "{{ item.image_encryption_key | default(omit) }}"
-    network_interfaces: "{{ [ { 'network': my_network.resources.0 | default(omit), 'subnetwork': my_subnetwork.resources.0 | default(omit) } | combine(external_access_config | default([]) ) ] }}"
+    network_interfaces:
+      "{{ [ { 'network': my_network.resources.0 | default(omit), 'subnetwork': my_subnetwork.resources.0 | default(omit) } | combine(external_access_config
+      | default([]) ) ] }}"
     zone: "{{ item.zone | default(molecule_yml.driver.region + '-b') }}"
     project: "{{ gcp_project_id }}"
     scopes: "{{ molecule_yml.driver.scopes | default(['https://www.googleapis.com/auth/compute'], True) }}"
-    service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-    service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+    service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+    service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
     auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
   register: async_results
   loop: "{{ molecule_yml.platforms }}"
   loop_control:
     pause: 3
   async: 7200
   poll: 0
 
 - name: Wait for instance(s) creation to complete
-  async_status:
+  ansible.builtin.async_status:
     jid: "{{ item.ansible_job_id }}"
   loop: "{{ async_results.results }}"
   register: server
   until: server.finished
   retries: 300
   delay: 10
   notify:
-    - "Populate instance config dict Linux"
-    - "Convert instance config dict to a list"
-    - "Dump instance config"
+    - Populate instance config dict Linux
+    - Convert instance config dict to a list
+    - Dump instance config
 
 - name: Wait for SSH
-  wait_for:
+  ansible.builtin.wait_for:
     port: 22
     host: "{{ item.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else item.networkInterfaces.0.networkIP }}"
     search_regex: SSH
     delay: 10
   loop: "{{ server.results }}"
```

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/linux/tasks/create_windows_instance.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/linux/tasks/create_windows_instance.yml`

 * *Files 6% similar despite different names*

```diff
@@ -8,56 +8,60 @@
       - auto_delete: true
         boot: true
         initialize_params:
           disk_size_gb: "{{ item.disk_size_gb | default(omit) }}"
           source_image: "{{ item.image | default('projects/windows-cloud/global/images/family/windows-2019') }}"
           source_image_encryption_key:
             raw_key: "{{ item.image_encryption_key | default(omit) }}"
-    network_interfaces: "{{ [ { 'network': my_network.resources.0 | default(omit), 'subnetwork': my_subnetwork.resources.0 | default(omit) } | combine(external_access_config | default([])) ] }}"
+    network_interfaces:
+      "{{ [ { 'network': my_network.resources.0 | default(omit), 'subnetwork': my_subnetwork.resources.0 | default(omit) } | combine(external_access_config
+      | default([])) ] }}"
     zone: "{{ item.zone | default(molecule_yml.driver.region + '-b') }}"
     project: "{{ gcp_project_id }}"
     scopes: "{{ molecule_yml.driver.scopes | default(['https://www.googleapis.com/auth/compute'], True) }}"
-    service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-    service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+    service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+    service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
     auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
   register: async_results
   loop: "{{ molecule_yml.platforms }}"
   async: 7200
   poll: 0
 
 - name: Wait for instance(s) creation to complete
-  async_status:
+  ansible.builtin.async_status:
     jid: "{{ item.ansible_job_id }}"
   loop: "{{ async_results.results }}"
   register: server
   until: server.finished
   retries: 300
   delay: 10
   notify:
-    - "Populate instance config dict Windows"
-    - "Convert instance config dict to a list"
-    - "Dump instance config"
+    - Populate instance config dict Windows
+    - Convert instance config dict to a list
+    - Dump instance config
 
 - name: Wait for WinRM
-  wait_for:
+  ansible.builtin.wait_for:
     port: 5986
     host: "{{ item.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else item.networkInterfaces.0.networkIP }}"
     delay: 10
   loop: "{{ server.results }}"
 
 - name: Prepare Windows User
-  script: ./files/windows_auth.py --instance {{ item.name }} --zone {{ item.zone | default(molecule_yml.driver.region + '-b') }} --project {{ gcp_project_id }} --username molecule_usr
+  ansible.builtin.script:
+    ./files/windows_auth.py --instance {{ item.name }} --zone {{ item.zone | default(molecule_yml.driver.region + '-b') }} --project {{ gcp_project_id
+    }} --username molecule_usr
   args:
     executable: python3
   loop: "{{ molecule_yml.platforms }}"
   changed_when:
     - password.rc == 0
     - password.stdout
   register: password
   retries: 10
   delay: 10
 
 - name: Add password for instances in server list
-  set_fact:
-    win_instances: "{{ win_instances|default([]) + [dict(item[0], password=item[1].stdout_lines |last)] }}"
+  ansible.builtin.set_fact:
+    win_instances: "{{ win_instances | default([]) + [dict(item[0], password=item[1].stdout_lines | last)] }}"
   loop: "{{ server.results | zip(password.results) | list }}"
   no_log: true
```

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/windows/INSTALL.md` & `molecule-plugins-23.5.0/test/gce/scenarios/windows/INSTALL.md`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/windows/create.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/windows/create.yml`

 * *Files 8% similar despite different names*

```diff
@@ -6,55 +6,54 @@
   no_log: "{{ molecule_no_log }}"
   vars:
     ssh_identity_file: "{{ lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY') }}/ssh_key"
     gcp_project_id: "{{ molecule_yml.driver.project_id | default(lookup('env', 'GCE_PROJECT_ID')) }}"
 
   tasks:
     - name: Make sure if linux or windows either specified
-      assert:
+      ansible.builtin.assert:
         that:
-          - molecule_yml.driver.instance_os_type | lower == "linux" or
-            molecule_yml.driver.instance_os_type | lower == "windows"
-        fail_msg: "instance_os_type is possible only to specify linux or windows either"
+          - molecule_yml.driver.instance_os_type | lower == "linux" or molecule_yml.driver.instance_os_type | lower == "windows"
+        fail_msg: instance_os_type is possible only to specify linux or windows either
 
     - name: Get network info
       google.cloud.gcp_compute_network_info:
         filters:
           - name = "{{ molecule_yml.driver.network_name | default('default') }}"
         project: "{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}"
-        service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-        service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+        service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+        service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
         auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
       register: my_network
 
     - name: Get subnetwork info
       google.cloud.gcp_compute_subnetwork_info:
         filters:
           - name = "{{ molecule_yml.driver.subnetwork_name | default('default') }}"
         project: "{{ molecule_yml.driver.vpc_host_project | default(gcp_project_id) }}"
         region: "{{ molecule_yml.driver.region }}"
-        service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-        service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+        service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+        service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
         auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
       register: my_subnetwork
 
     - name: Set external access config
-      set_fact:
+      ansible.builtin.set_fact:
         external_access_config:
           - access_configs:
-              - name: "External NAT"
-                type: "ONE_TO_NAT"
+              - name: External NAT
+                type: ONE_TO_NAT
       when: molecule_yml.driver.external_access
 
     - name: Include create_linux_instance tasks
-      include_tasks: tasks/create_linux_instance.yml
+      ansible.builtin.include_tasks: tasks/create_linux_instance.yml
       when:
         - molecule_yml.driver.instance_os_type  | lower == "linux"
 
     - name: Include create_windows_instance tasks
-      include_tasks: tasks/create_windows_instance.yml
+      ansible.builtin.include_tasks: tasks/create_windows_instance.yml
       when:
         - molecule_yml.driver.instance_os_type  | lower == "windows"
 
   handlers:
     - name: Import main handler tasks
-      import_tasks: handlers/main.yml
+      ansible.builtin.import_tasks: handlers/main.yml
```

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/windows/destroy.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/windows/destroy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -9,30 +9,30 @@
     - name: Destroy molecule instance(s)
       google.cloud.gcp_compute_instance:
         name: "{{ item.name }}"
         state: absent
         zone: "{{ item.zone | default(molecule_yml.driver.region + '-b') }}"
         project: "{{ molecule_yml.driver.project_id | default(lookup('env', 'GCE_PROJECT_ID')) }}"
         scopes: "{{ molecule_yml.driver.scopes | default(['https://www.googleapis.com/auth/compute'], True) }}"
-        service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-        service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+        service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+        service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
         auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
       register: async_results
       loop: "{{ molecule_yml.platforms }}"
       async: 7200
       poll: 0
       notify:
-        - "Wipe out instance config"
-        - "Dump instance config"
+        - Wipe out instance config
+        - Dump instance config
 
     - name: Wait for instance(s) deletion to complete
-      async_status:
+      ansible.builtin.async_status:
         jid: "{{ item.ansible_job_id }}"
       register: server
       until: server.finished
       retries: 300
       delay: 10
       loop: "{{ async_results.results }}"
 
   handlers:
     - name: Import main handler tasks
-      import_tasks: handlers/main.yml
+      ansible.builtin.import_tasks: handlers/main.yml
```

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/windows/files/windows_auth.py` & `molecule-plugins-23.5.0/test/gce/scenarios/windows/files/windows_auth.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/windows/handlers/main.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/windows/handlers/main.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 ---
 - name: Populate instance config dict Linux
-  set_fact:
+  ansible.builtin.set_fact:
     instance_conf_dict:
-      {
-        "instance": "{{ instance_info.name }}",
-        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
-        "user": "{{ lookup('env','USER') }}",
-        "port": "22",
-        "identity_file": "{{ ssh_identity_file }}",
-        "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
-      }
+      instance: "{{ instance_info.name }}"
+      address:
+        "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP
+        }}"
+      user: "{{ lookup('env', 'USER') }}"
+      port: "22"
+      identity_file: "{{ ssh_identity_file }}"
+      instance_os_type: "{{ molecule_yml.driver.instance_os_type }}"
   loop: "{{ server.results }}"
   loop_control:
     loop_var: instance_info
   no_log: true
   register: instance_conf_dict
 
 - name: Populate instance config dict Windows
-  set_fact:
+  ansible.builtin.set_fact:
     instance_conf_dict:
-      {
-        "instance": "{{ instance_info.name }}",
-        "address": "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP }}",
-        "user": "molecule_usr",
-        "password": "{{ instance_info.password }}",
-        "port": "{{ instance_info.winrm_port | default(5986) }}",
-        "winrm_transport": "{{ molecule_yml.driver.winrm_transport | default('ntlm') }}",
-        "winrm_server_cert_validation": "{{ molecule_yml.driver.winrm_server_cert_validation | default('ignore') }}",
-        "instance_os_type": "{{ molecule_yml.driver.instance_os_type }}",
-      }
+      instance: "{{ instance_info.name }}"
+      address:
+        "{{ instance_info.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else instance_info.networkInterfaces.0.networkIP
+        }}"
+      user: molecule_usr
+      password: "{{ instance_info.password }}"
+      port: "{{ instance_info.winrm_port | default(5986) }}"
+      winrm_transport: "{{ molecule_yml.driver.winrm_transport | default('ntlm') }}"
+      winrm_server_cert_validation: "{{ molecule_yml.driver.winrm_server_cert_validation | default('ignore') }}"
+      instance_os_type: "{{ molecule_yml.driver.instance_os_type }}"
   loop: "{{ win_instances }}"
   loop_control:
     loop_var: instance_info
   no_log: true
   register: instance_conf_dict
 
 - name: Wipe out instance config
-  set_fact:
+  ansible.builtin.set_fact:
     instance_conf: {}
-
 - name: Convert instance config dict to a list
-  set_fact:
+  ansible.builtin.set_fact:
     instance_conf: "{{ instance_conf_dict.results | map(attribute='ansible_facts.instance_conf_dict') | list }}"
 
 - name: Dump instance config
-  copy:
+  ansible.builtin.copy:
     content: "{{ instance_conf }}"
     dest: "{{ molecule_instance_config }}"
     mode: "0600"
```

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/windows/molecule.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/linux/molecule.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ---
 dependency:
   name: galaxy
 driver:
   name: gce
   project_id: change-to-id-of-the-gcp-project # if not set, will default to env GCE_PROJECT_ID
-  auth_kind: null # set to machineaccount or serviceaccount or application - if set to null will read env GCP_AUTH_KIND
-  service_account_email: null # set to an email associated with the project - if set to null, will default to GCP_SERVICE_ACCOUNT_EMAIL. Should not be set if using auth_kind serviceaccount.
-  service_account_file: null # set to the path to the JSON credentials file - if set to null, will default to env GCP_SERVICE_ACCOUNT_FILE
+  auth_kind: # set to machineaccount or serviceaccount or application - if set to null will read env GCP_AUTH_KIND
+  service_account_email: # set to an email associated with the project - if set to null, will default to GCP_SERVICE_ACCOUNT_EMAIL. Should not be set if using auth_kind serviceaccount.
+  service_account_file: # set to the path to the JSON credentials file - if set to null, will default to env GCP_SERVICE_ACCOUNT_FILE
   region: us-west1 # REQUIRED. example: us-central1
   external_access: false # chose whether to create a public IP for the VM or not - default is private IP only
-  instance_os_type: windows # will be considered linux by default, but can be explicitely set to windows
+  instance_os_type: linux # will be considered linux by default, but can be explicitely set to windows
 platforms:
   - name: linuxgce-createdbymolecule # is an instance name
     machine_type: n1-standard-1 # define your machine type
-    zone: null # example: us-west1-b, will default to zone b of driver.region
+    zone: # example: us-west1-b, will default to zone b of driver.region
 provisioner:
   name: ansible
 verifier:
   name: ansible
```

### Comparing `molecule-plugins-23.4.1/test/gce/scenarios/windows/tasks/create_linux_instance.yml` & `molecule-plugins-23.5.0/test/gce/scenarios/windows/tasks/create_windows_instance.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 ---
-- name: Create ssh keypair
-  community.crypto.openssh_keypair:
-    comment: "{{ lookup('env','USER') }} user for Molecule"
-    path: "{{ ssh_identity_file }}"
-  register: keypair
-
-- name: Create molecule Linux instance(s)
+- name: Create molecule Windows instance(s)
   google.cloud.gcp_compute_instance:
     state: present
     name: "{{ item.name }}"
     machine_type: "{{ item.machine_type | default('n1-standard-1') }}"
-    metadata:
-      ssh-keys: "{{ lookup('env','USER') }}:{{ keypair.public_key }}}"
     disks:
       - auto_delete: true
         boot: true
         initialize_params:
           disk_size_gb: "{{ item.disk_size_gb | default(omit) }}"
-          source_image: "{{ item.image | default('projects/debian-cloud/global/images/family/debian-10') }}"
+          source_image: "{{ item.image | default('projects/windows-cloud/global/images/family/windows-2019') }}"
           source_image_encryption_key:
             raw_key: "{{ item.image_encryption_key | default(omit) }}"
-    network_interfaces: "{{ [ { 'network': my_network.resources.0 | default(omit), 'subnetwork': my_subnetwork.resources.0 | default(omit) } | combine(external_access_config | default([]) ) ] }}"
+    network_interfaces:
+      "{{ [ { 'network': my_network.resources.0 | default(omit), 'subnetwork': my_subnetwork.resources.0 | default(omit) } | combine(external_access_config
+      | default([])) ] }}"
     zone: "{{ item.zone | default(molecule_yml.driver.region + '-b') }}"
     project: "{{ gcp_project_id }}"
     scopes: "{{ molecule_yml.driver.scopes | default(['https://www.googleapis.com/auth/compute'], True) }}"
-    service_account_email: "{{ molecule_yml.driver.service_account_email | default (omit, true) }}"
-    service_account_file: "{{ molecule_yml.driver.service_account_file | default (omit, true) }}"
+    service_account_email: "{{ molecule_yml.driver.service_account_email | default(omit, true) }}"
+    service_account_file: "{{ molecule_yml.driver.service_account_file | default(omit, true) }}"
     auth_kind: "{{ molecule_yml.driver.auth_kind | default(omit, true) }}"
   register: async_results
   loop: "{{ molecule_yml.platforms }}"
-  loop_control:
-    pause: 3
   async: 7200
   poll: 0
 
 - name: Wait for instance(s) creation to complete
-  async_status:
+  ansible.builtin.async_status:
     jid: "{{ item.ansible_job_id }}"
   loop: "{{ async_results.results }}"
   register: server
   until: server.finished
   retries: 300
   delay: 10
   notify:
-    - "Populate instance config dict Linux"
-    - "Convert instance config dict to a list"
-    - "Dump instance config"
+    - Populate instance config dict Windows
+    - Convert instance config dict to a list
+    - Dump instance config
 
-- name: Wait for SSH
-  wait_for:
-    port: 22
+- name: Wait for WinRM
+  ansible.builtin.wait_for:
+    port: 5986
     host: "{{ item.networkInterfaces.0.accessConfigs.0.natIP if molecule_yml.driver.external_access else item.networkInterfaces.0.networkIP }}"
-    search_regex: SSH
     delay: 10
   loop: "{{ server.results }}"
+
+- name: Prepare Windows User
+  ansible.builtin.script:
+    ./files/windows_auth.py --instance {{ item.name }} --zone {{ item.zone | default(molecule_yml.driver.region + '-b') }} --project {{ gcp_project_id
+    }} --username molecule_usr
+  args:
+    executable: python3
+  loop: "{{ molecule_yml.platforms }}"
+  changed_when:
+    - password.rc == 0
+    - password.stdout
+  register: password
+  retries: 10
+  delay: 10
+
+- name: Add password for instances in server list
+  ansible.builtin.set_fact:
+    win_instances: "{{ win_instances | default([]) + [dict(item[0], password=item[1].stdout_lines | last)] }}"
+  loop: "{{ server.results | zip(password.results) | list }}"
+  no_log: true
```

### Comparing `molecule-plugins-23.4.1/test/podman/test_func.py` & `molecule-plugins-23.5.0/test/podman/test_func.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/vagrant/functional/conftest.py` & `molecule-plugins-23.5.0/test/vagrant/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/vagrant/functional/test_func.py` & `molecule-plugins-23.5.0/test/vagrant/functional/test_func.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/create.yml` & `molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/default-compat/create.yml`

 * *Files 6% similar despite different names*

```diff
@@ -40,21 +40,19 @@
 
     - name: Create molecule instances configuration
       when: server is changed # noqa no-handler
       block:
         - name: Populate instance config dict
           ansible.builtin.set_fact:
             instance_conf_dict:
-              {
-                "instance": "{{ item.Host }}",
-                "address": "{{ item.HostName }}",
-                "user": "{{ item.User }}",
-                "port": "{{ item.Port }}",
-                "identity_file": "{{ item.IdentityFile }}",
-              }
+              instance: "{{ item.Host }}"
+              address: "{{ item.HostName }}"
+              user: "{{ item.User }}"
+              port: "{{ item.Port }}"
+              identity_file: "{{ item.IdentityFile }}"
           with_items: "{{ server.results }}"
           register: instance_config_dict
 
         - name: Convert instance config dict to a list
           ansible.builtin.set_fact:
             instance_conf: "{{ instance_config_dict.results | map(attribute='ansible_facts.instance_conf_dict') | list }}"
```

### Comparing `molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/destroy.yml` & `molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/default-compat/destroy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     # causes issues.
 
     # Mandatory configuration for Molecule to function.
 
     - name: Populate instance config
       ansible.builtin.set_fact:
         instance_conf: {}
-
     - name: Dump instance config # noqa no-handler
       ansible.builtin.copy:
         content: |
           # Molecule managed
           {{ instance_conf | to_json | from_json | to_yaml }}
         dest: "{{ molecule_instance_config }}"
         mode: "0600"
```

### Comparing `molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/hostname/verify.yml` & `molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/hostname/verify.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/vagrant_root/verify.yml` & `molecule-plugins-23.5.0/test/vagrant/scenarios/molecule/vagrant_root/verify.yml`

 * *Files 14% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     - name: Print workdir file content
       ansible.builtin.debug:
         var: workdir_content.stdout
 
     - name: Check /tmp/workdir content
       ansible.builtin.assert:
         that:
-          - "workdir_content.stdout == lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY')"
+          - workdir_content.stdout == lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY')
```

### Comparing `molecule-plugins-23.4.1/tools/create_testbox.sh` & `molecule-plugins-23.5.0/tools/create_testbox.sh`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/tools/test-setup.sh` & `molecule-plugins-23.5.0/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.1/tox.ini` & `molecule-plugins-23.5.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     DOCKER_*
     PYTEST_*
     REQUESTS_CA_BUNDLE
     SSH_AUTH_SOCK
     SSL_CERT_FILE
     TOXENV
     TWINE_*
+    USER
 allowlist_externals =
     bash
     twine
     pytest
     pre-commit
 
 [testenv:pkg]
@@ -73,13 +74,17 @@
     bash -c "rm -rf {toxinidir}/dist/ && mkdir -p {toxinidir}/dist/"
     # ./build.sh
     python -m build
     twine check --strict dist/*
 
 [testenv:lint]
 description = Performs linting, style checks
-skip_install = true
-sitepackages = false
+allowlist_externals =
+    bash
+    rm
 deps =
     pre-commit
+    toml
 commands =
+    bash {toxinidir}/tools/generate-templates.sh
     pre-commit run -a
+    rm -rf test/roles
```

