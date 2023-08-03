# Comparing `tmp/smol_k8s_lab-0.9.2.tar.gz` & `tmp/smol_k8s_lab-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smol_k8s_lab-0.9.2.tar", max compression
+gzip compressed data, was "smol_k8s_lab-0.9.3.tar", max compression
```

## Comparing `smol_k8s_lab-0.9.2.tar` & `smol_k8s_lab-0.9.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2022-12-07 19:07:19.797333 smol_k8s_lab-0.9.2/LICENSE
--rw-r--r--   0        0        0     5568 2022-12-07 19:07:19.797333 smol_k8s_lab-0.9.2/README.md
--rw-r--r--   0        0        0     1585 2022-12-07 19:07:19.805333 smol_k8s_lab-0.9.2/pyproject.toml
--rwxr-xr-x   0        0        0    21071 2022-12-07 19:07:19.805333 smol_k8s_lab-0.9.2/smol_k8s_lab/__init__.py
--rwxr-xr-x   0        0        0     3467 2022-12-07 19:07:19.805333 smol_k8s_lab-0.9.2/smol_k8s_lab/bw_cli.py
--rw-r--r--   0        0        0      899 2022-12-07 19:07:19.805333 smol_k8s_lab-0.9.2/smol_k8s_lab/config/config.yml
--rwxr-xr-x   0        0        0     3002 2022-12-07 19:07:19.805333 smol_k8s_lab-0.9.2/smol_k8s_lab/console_logging.py
--rwxr-xr-x   0        0        0     2742 2022-12-07 19:07:19.805333 smol_k8s_lab-0.9.2/smol_k8s_lab/env_config.py
--rwxr-xr-x   0        0        0     5132 2022-12-07 19:07:19.805333 smol_k8s_lab-0.9.2/smol_k8s_lab/help_text.py
--rwxr-xr-x   0        0        0     3327 2022-12-07 19:07:19.805333 smol_k8s_lab-0.9.2/smol_k8s_lab/homelabHelm.py
--rwxr-xr-x   0        0        0     4864 2022-12-07 19:07:19.805333 smol_k8s_lab-0.9.2/smol_k8s_lab/subproc.py
--rw-r--r--   0        0        0     6604 1970-01-01 00:00:00.000000 smol_k8s_lab-0.9.2/setup.py
--rw-r--r--   0        0        0     6822 1970-01-01 00:00:00.000000 smol_k8s_lab-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-07 22:41:22.396617 smol_k8s_lab-0.9.3/LICENSE
+-rw-r--r--   0        0        0     5568 2022-12-07 22:41:22.396617 smol_k8s_lab-0.9.3/README.md
+-rw-r--r--   0        0        0     1585 2022-12-07 22:41:22.400617 smol_k8s_lab-0.9.3/pyproject.toml
+-rwxr-xr-x   0        0        0    21058 2022-12-07 22:41:22.400617 smol_k8s_lab-0.9.3/smol_k8s_lab/__init__.py
+-rwxr-xr-x   0        0        0     3467 2022-12-07 22:41:22.400617 smol_k8s_lab-0.9.3/smol_k8s_lab/bw_cli.py
+-rw-r--r--   0        0        0      899 2022-12-07 22:41:22.400617 smol_k8s_lab-0.9.3/smol_k8s_lab/config/config.yml
+-rwxr-xr-x   0        0        0     3002 2022-12-07 22:41:22.400617 smol_k8s_lab-0.9.3/smol_k8s_lab/console_logging.py
+-rwxr-xr-x   0        0        0     2742 2022-12-07 22:41:22.400617 smol_k8s_lab-0.9.3/smol_k8s_lab/env_config.py
+-rwxr-xr-x   0        0        0     5132 2022-12-07 22:41:22.400617 smol_k8s_lab-0.9.3/smol_k8s_lab/help_text.py
+-rwxr-xr-x   0        0        0     3327 2022-12-07 22:41:22.400617 smol_k8s_lab-0.9.3/smol_k8s_lab/homelabHelm.py
+-rwxr-xr-x   0        0        0     4864 2022-12-07 22:41:22.400617 smol_k8s_lab-0.9.3/smol_k8s_lab/subproc.py
+-rw-r--r--   0        0        0     6604 1970-01-01 00:00:00.000000 smol_k8s_lab-0.9.3/setup.py
+-rw-r--r--   0        0        0     6822 1970-01-01 00:00:00.000000 smol_k8s_lab-0.9.3/PKG-INFO
```

### Comparing `smol_k8s_lab-0.9.2/LICENSE` & `smol_k8s_lab-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-0.9.2/README.md` & `smol_k8s_lab-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-0.9.2/pyproject.toml` & `smol_k8s_lab-0.9.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "smol_k8s_lab"
-version       = "0.9.2"
+version       = "0.9.3"
 description   = "bootstrap simple projects on kubernetes with kind and k3s"
 authors       = ["Jesse Hitch <jessebot@linux.com>"]
 readme        = "README.md"
 packages      = [{include = "smol_k8s_lab"}]
 license       = "AGPL-3.0-or-later"
 homepage      = "https://jessebot.github.io/smol-k8s-lab"
 repository    = "http://github.com/jessebot/smol-k8s-lab"
```

### Comparing `smol_k8s_lab-0.9.2/smol_k8s_lab/__init__.py` & `smol_k8s_lab-0.9.3/smol_k8s_lab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
            "manifests/metallb-native.yaml")
 
     # install manifest and wait
     apply_manifests(url, "metallb-system", "controller",
                     "component=controller")
 
     # metallb requires a address pool configured and a layer 2 advertisement CR
-    print_panel(log.info("Installing IPAddressPool and L2Advertisement custom resources."))
+    log.info("Installing IPAddressPool and L2Advertisement custom resources.")
 
     ip_pool_cr = {'apiVersion': 'metallb.io/v1beta1',
                   'kind': 'IPAddressPool',
                   'metadata': {'name': 'default',
                                'namespace': 'metallb-system'},
                   'spec': {'addresses': address_pool}}
```

### Comparing `smol_k8s_lab-0.9.2/smol_k8s_lab/bw_cli.py` & `smol_k8s_lab-0.9.3/smol_k8s_lab/bw_cli.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-0.9.2/smol_k8s_lab/config/config.yml` & `smol_k8s_lab-0.9.3/smol_k8s_lab/config/config.yml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-0.9.2/smol_k8s_lab/console_logging.py` & `smol_k8s_lab-0.9.3/smol_k8s_lab/console_logging.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-0.9.2/smol_k8s_lab/env_config.py` & `smol_k8s_lab-0.9.3/smol_k8s_lab/env_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-0.9.2/smol_k8s_lab/help_text.py` & `smol_k8s_lab-0.9.3/smol_k8s_lab/help_text.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-0.9.2/smol_k8s_lab/homelabHelm.py` & `smol_k8s_lab-0.9.3/smol_k8s_lab/homelabHelm.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-0.9.2/smol_k8s_lab/subproc.py` & `smol_k8s_lab-0.9.3/smol_k8s_lab/subproc.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-0.9.2/setup.py` & `smol_k8s_lab-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'rich>=12.6.0,<13.0.0']
 
 entry_points = \
 {'console_scripts': ['smol-k8s-lab = smol_k8s_lab:main']}
 
 setup_kwargs = {
     'name': 'smol-k8s-lab',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'bootstrap simple projects on kubernetes with kind and k3s',
     'long_description': '## ☁️ *smol k8s lab* 🧸\n\nA project aimed at getting up and running **quickly** with slimmer k8s distros in one small command line tool.\n\n<p align="center">\n  <a href="https://raw.githubusercontent.com/jessebot/smol-k8s-lab/main/docs/screenshots/help_text.svg">\n      <img src="./docs/screenshots/help_text.svg" alt="Output of smol-k8s-lab --help after cloning the directory and installing the prerequisites.">\n  </a>\n</p>\n\n\n## Docs\n\n### Quick Start\nIf you\'ve already got Python3.11 and brew installed, you should be able to:\n\n```bash\npip3.11 install smol-k8s-lab\n```\n\nWe\'ve also got a [Quickstart guide](https://jessebot.github.io/smol-k8s-lab/quickstart) for you to jump right in!\n\nThere\'s also full tutorials to manually set up different distros in the [docs we maintain](https://jessebot.github.io/smol-k8s-lab/distros) as well as BASH scripts for basic automation of each k8s distro in:\n\n`./distro/{NAME_OF_K8S_DISTRO}/bash_full_quickstart.sh`\n\n## Under the hood\n### Currently supported k8s distros\n\n- [<img src="https://raw.githubusercontent.com/jessebot/smol-k8s-lab/main/docs/icons/k3s_icon.ico" width="26">&nbsp;&nbsp;k3s](https://k3s.io/)\n- [<img src="https://raw.githubusercontent.com/jessebot/smol-k8s-lab/main/docs/icons/kind_icon.png" width="32">&nbsp;KinD](https://kind.sigs.k8s.io/)\n\nWe tend to test first on k3s and then kind.\n\nWe\'re working on k0s next :)\n\n\n### Stack We Install on K8s\n\n|    Application      | What is it? |\n|:--------------------|:------------|\n| &nbsp;🐄 &nbsp;[Local Path Provisioner](https://github.com/rancher/local-path-provisioner) | Default simple local file storage for persistent data |\n| [<img src="https://raw.githubusercontent.com/jessebot/smol-k8s-lab/main/docs/icons/metallb_icon.png" width="32" alt="metallb logo, blue arrow pointing up, with small line on one leg of arrow to show balance">&nbsp; metallb](https://github.io/metallb/metallb) | loadbalancer for metal, since we\'re mostly selfhosting |\n| [<img src="https://raw.githubusercontent.com/jessebot/smol-k8s-lab/main/docs/icons/nginx.ico" width="32" alt="nginx logo, white letter N with green background">&nbsp; nginx-ingress](https://github.io/kubernetes/ingress-nginx) | The ingress controller allows access to the cluster remotely, needed for web traffic |\n| [<img src="https://raw.githubusercontent.com/jessebot/smol-k8s-lab/main/docs/icons/cert-manager_icon.png" width="32" alt="cert manager logo"> &nbsp;cert-manager](https://cert-manager.io/docs/) | For SSL/TLS certificates |\n| [<img src="https://raw.githubusercontent.com/jessebot/smol-k8s-lab/main/docs/icons/k9s_icon.png" alt="k9s logo, outline of dog with ship wheels for eyes" width="32"> &nbsp;k9s](https://k9scli.io/topics/install/) | Terminal based dashboard for kubernetes |\n\n\n#### Optionally installed\n\n| Application/Tool | What is it? |\n|:-----------------|:------------|\n| [<img src="https://raw.githubusercontent.com/jessebot/smol-k8s-lab/main/docs/icons/eso_icon.png" width="32" alt="ESO logo, outline of robot with astricks in a screen in it\'s belly">&nbsp; ESO](https://external-secrets.io/v0.5.9/) | external-secrets-operator integrates external secret management systems like GitLab|\n| [<img src="https://raw.githubusercontent.com/jessebot/smol-k8s-lab/main/docs/icons/argo_icon.png" width="32" alt="argo CD logo, an organer squid wearing a fishbowl helmet">&nbsp; Argo CD](https://github.io/argoproj/argo-helm) | Gitops - Continuous Deployment |\n| [<img src="https://raw.githubusercontent.com/jessebot/smol-k8s-lab/main/docs/icons/kyverno_icon.png"  width="32" alt="kyvero logo">&nbsp; Kyverno](https://github.com/kyverno/kyverno/) | Kubernetes native policy management to enforce policies on k8s resources |\n\nIf you install argocd, and you use bitwarden, we\'ll generate an admin password and automatically place it in your vault if you pass in the `-p` option. Curently only works with Bitwarden.\n\nWant to get started with argocd? If you\'ve installed it via smol-k8s-lab, then you can jump [here](https://github.com/jessebot/argo-example#argo-via-the-gui). Otherwise, if you want to start from scratch, start [here](https://github.com/jessebot/argo-example#argocd)\n\n\n### Tooling Used for the script itself and interface\n\n[![made-with-python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)\n\n- rich (this is what makes all the pretty formatted text)\n- PyYAML (to handle the k8s yamls and configs)\n- bcrypt (to pass a password to argocd and automatically update your bitwarden)\n- click (handles arguments for the script)\n\n\n## Troubleshooting\nIf you\'re stuck, checkout the [Notes](https://jessebot.github.io/smol-k8s-lab/notes) to see if we also got stuck on the same thing at some point :) Under each app or tool, we\'ll have notes on how to learn more about it, as well as any errors we\'ve already battled.\n\n\n## Other Notes\nCheck out the [`optional`](optional) directory for quick examples on apps this script does not default install.\n\ne.g. for postgres, go to [`./optional/postgres`](./optional/postgres)\n\n# Status\nThis is still in beta, as we figure out all the distros we want to support,\nand pin all the versions, but if you\'d like to contribute or just found a :bug:,\nfeel free to open an issue (or pull request), and we\'ll take a look! We\'ll try\nto get back to you asap!\n\n## Collaborators\n<!-- readme: collaborators -start -->\n<!-- readme: collaborators -end -->\n\n## TODO\n- Configure base policies for Kyverno\n- bitwarden: check local env vars for password or api key\n- look into https://kubesec.io/\n',
     'author': 'Jesse Hitch',
     'author_email': 'jessebot@linux.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://jessebot.github.io/smol-k8s-lab',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['smol_k8s_lab'] package_data = \ {'': ['*'], 'smol_k8s_lab': ['config/*']}
 install_requires = \ ['bcrypt>=4.0.1,<5.0.0', 'click>=8.1.3,<9.0.0',
 'pyyaml>=6.0,<7.0', 'requests>=2.28.1,<3.0.0', 'rich>=12.6.0,<13.0.0']
 entry_points = \ {'console_scripts': ['smol-k8s-lab = smol_k8s_lab:main']}
-setup_kwargs = { 'name': 'smol-k8s-lab', 'version': '0.9.2', 'description':
+setup_kwargs = { 'name': 'smol-k8s-lab', 'version': '0.9.3', 'description':
 'bootstrap simple projects on kubernetes with kind and k3s',
 'long_description': '## âï¸ *smol k8s lab* ð§¸\n\nA project aimed at
 getting up and running **quickly** with slimmer k8s distros in one small
 command line tool.\n\n
 \n \n_[Output_of_smol-k8s-lab_--help_after_cloning_the_directory_and_installing
                             the_prerequisites.]\n\n
 \n\n\n## Docs\n\n### Quick Start\nIf you\'ve already got Python3.11 and brew
```

### Comparing `smol_k8s_lab-0.9.2/PKG-INFO` & `smol_k8s_lab-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smol-k8s-lab
-Version: 0.9.2
+Version: 0.9.3
 Summary: bootstrap simple projects on kubernetes with kind and k3s
 Home-page: https://jessebot.github.io/smol-k8s-lab
 License: AGPL-3.0-or-later
 Keywords: kubernetes,homelab,kind,k3s,k8s
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smol-k8s-lab Version: 0.9.2 Summary: bootstrap
+Metadata-Version: 2.1 Name: smol-k8s-lab Version: 0.9.3 Summary: bootstrap
 simple projects on kubernetes with kind and k3s Home-page: https://
 jessebot.github.io/smol-k8s-lab License: AGPL-3.0-or-later Keywords:
 kubernetes,homelab,kind,k3s,k8s Author: Jesse Hitch Author-email:
 jessebot@linux.com Requires-Python: >=3.11,<4.0.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or
 later (AGPLv3+) Classifier: Operating System :: MacOS :: MacOS X Classifier:
```

