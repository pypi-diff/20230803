# Comparing `tmp/1password-0.6.2.tar.gz` & `tmp/1password-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1password-0.6.2.tar", last modified: Thu Nov 10 17:04:16 2022, max compression
+gzip compressed data, was "1password-1.0.1.tar", last modified: Thu Aug  3 10:28:42 2023, max compression
```

## Comparing `1password-0.6.2.tar` & `1password-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 17:04:16.205538 1password-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 17:04:16.205538 1password-0.6.2/1password.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-11-10 17:04:16.000000 1password-0.6.2/1password.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-11-10 17:04:16.000000 1password-0.6.2/1password.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 17:04:16.000000 1password-0.6.2/1password.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-10 17:04:16.000000 1password-0.6.2/1password.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-10 17:04:16.000000 1password-0.6.2/1password.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-11-10 17:03:50.000000 1password-0.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-10 17:03:50.000000 1password-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-11-10 17:04:16.205538 1password-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6217 2022-11-10 17:03:50.000000 1password-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-10 17:04:00.000000 1password-0.6.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)     6770 2022-11-10 17:03:50.000000 1password-0.6.2/install_op.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 17:04:16.205538 1password-0.6.2/onepassword/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-10 17:03:50.000000 1password-0.6.2/onepassword/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13293 2022-11-10 17:03:50.000000 1password-0.6.2/onepassword/client.py
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-10 17:03:50.000000 1password-0.6.2/onepassword/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7838 2022-11-10 17:03:50.000000 1password-0.6.2/onepassword/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 17:04:16.205538 1password-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-11-10 17:03:50.000000 1password-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 17:04:16.205538 1password-0.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (121)     3006 2022-11-10 17:03:50.000000 1password-0.6.2/test/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:28:42.764228 1password-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:28:42.756228 1password-1.0.1/1password.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-08-03 10:28:42.000000 1password-1.0.1/1password.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-03 10:28:42.000000 1password-1.0.1/1password.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:28:42.000000 1password-1.0.1/1password.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 10:28:42.000000 1password-1.0.1/1password.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 10:28:42.000000 1password-1.0.1/1password.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-03 10:28:13.000000 1password-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 10:28:13.000000 1password-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-08-03 10:28:42.764228 1password-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-08-03 10:28:13.000000 1password-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 10:28:30.000000 1password-1.0.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-08-03 10:28:13.000000 1password-1.0.1/install_op.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:28:42.756228 1password-1.0.1/onepassword/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 10:28:13.000000 1password-1.0.1/onepassword/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-08-03 10:28:13.000000 1password-1.0.1/onepassword/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-03 10:28:13.000000 1password-1.0.1/onepassword/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-08-03 10:28:13.000000 1password-1.0.1/onepassword/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 10:28:42.764228 1password-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-03 10:28:13.000000 1password-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:28:42.756228 1password-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-03 10:28:13.000000 1password-1.0.1/test/test_client.py
```

### Comparing `1password-0.6.2/1password.egg-info/PKG-INFO` & `1password-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,85 @@
-Metadata-Version: 2.1
-Name: 1password
-Version: 0.6.2
-Summary: A Python client and wrapper around the 1Password CLI.
-Home-page: https://github.com/wandera/1password-client
-Author: David Pryce
-Author-email: david.pryce@wandera.com
-License: MIT
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # OnePassword python client
 [![PyPi release](https://github.com/wandera/1password-client/actions/workflows/publish-to-pypi.yml/badge.svg?branch=main&event=push)](https://github.com/wandera/1password-client/actions/workflows/publish-to-pypi.yml)
 [![CodeQL](https://github.com/wandera/1password-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/wandera/1password-client/actions/workflows/codeql-analysis.yml)
 
 Python client around the 1Password password manager cli for usage within python code and
 Jupyter Notebooks. Developed by Data Scientists from Jamf.
 
-Warning: this client is for use with 1Password 7 and earlier. For 1Password 8 there is a different CLI2, which we have 
-not yet fully tested within this client. Feel free to attempt to use a higher version of the cli or this client with
-1Password 8 and submit PRs to fix issues.
-
+## Supported versions
+There are some of the pre-requisites that are needed to use the library. We automatically install the cli for Mac and
+Linux users when installing the library. Windows users see below for help.
+
+- 1Password App: 8+
+- 1Password cli: 2+
+- Python: 3.10+
+
+## Operating systems
+The library is split into two parts: installation and client in which we are slowly updating to cover as many operating
+systems as possible the following table should ensure users understand what this library can and can't do at time of 
+install.
+
+|                 | MacOS | Linux | 
+|-----------------|-------|-------|
+| Fully supported | Y     | Y     | 
+| CLI install     | Y     | Y     | 
+| SSO login       | Y     | Y     | 
+| Login via App   | Y     | Y     | 
+| Biometrics auth | Y     | Y     | 
+| Password auth   | Y     | Y     | 
+| CLI client      | Y     | Y     | 
 
 ## Installation
 ```bash
 pip install 1password
 ```
 
 If you have issues with PyYaml or other distutils installed packages then use:
 ```bash
 pip install --ignore-installed 1password
 ```
 
 You are welcome to install and manage `op` yourself by visiting
 [the CLI1 downloads page](https://app-updates.agilebits.com/product_history/CLI ) to download the version you require 
-and follow instructions for your platform.
+and follow instructions for your platform as long as it's major version 2.
 
-The above commands will check `op` is present already and if not will install the best `op` cli it can work out plus 
-the python client itself. 
+The above commands pip commands will check `op` is present already and if not will install the supported `op` cli 
+plus the python client itself. 
 This is currently fixed at `op` version 1.12.5 to ensure compatibility. If you wish to use a higher version of `op` you
 can by following [this guide](https://developer.1password.com/docs/cli/upgrade), 
 however note that we cannot ensure it will work with our client yet. 
 
 MacOS users will be prompted with a separate installation window to ensure you have a signed version of `op` - make
 sure to check other desktops that the installer might pop up on. 
 
+
 ### Optional pre-requisites
 #### base32
 This utility is used to create a unique guid for your device but this isn't a hard requirement from AgileBits 
 and so if you see `base32: command not found` an empty string will be used instead, 
 and the client will still work fully.
 
 If you really want to, you can make sure you have this installed by installing coreutils. Details per platform can
 be found here: https://command-not-found.com/base32
 
 ## Basic Usage
-Currently tested on MacOS and Linux.
+Since v2 of the cli it is advised to connect your CLI to the local app installed on the device, thus removing the need
+for secret keys and passwords in the terminal or shell. Read here on how to do that: 
+https://developer.1password.com/docs/cli/get-started#step-2-turn-on-the-1password-desktop-app-integration
+
+An added extra for Mac users is that you can also enable TouchID for the app and by linking your cli with the app you 
+will get biometric login for both. 
+
+Once this is done any initial usage of the cli, and our client will request you to authenticate either via the app or 
+using your biometrics and then you can continue.
+
+We are sure there are use cases where the app cannot be linked and hence a password etc is till required so this 
+functionality is still present from our v1 implementation and can be described below
 
+### Password authentication
 On first usage users will be asked for both the enrolled email, secret key and password. 
 There is also verification of your account domain and name. 
 
 For all following usages you will only be asked for a password.
 
 You will be given 3 attempts and then pointed to reset password documentation or alternatively you can
 restart your kernel.
@@ -88,14 +102,15 @@
 
 # Get all fields, one field or more fields for an item with uuid="example"
 op.get_item(uuid="example")
 op.get_item(uuid="example", fields="username")
 op.get_item(uuid="example", fields=["username", "password"])
 
 ```
+## 
 
 ### Input formats
 To be sure what you are using is of the right format
 
 - Enrolled email: standard email format e.g. user@example.com 
 - Secret key: provided by 1Password e.g. ##-######-######-#####-#####-#####-#####
 - Account domain: domain that you would login to 1Password via browser e.g. example.1password.com
@@ -190,8 +205,7 @@
     - encode
     - forget
     - get
     - list
     - reactivate
     - remove
     - suspend
-- Use the new CLI update method
```

### Comparing `1password-0.6.2/LICENSE.txt` & `1password-1.0.1/LICENSE.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Wandera
+Copyright (c) 2023 Jamf
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `1password-0.6.2/PKG-INFO` & `1password-1.0.1/1password.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: 1password
-Version: 0.6.2
+Version: 1.0.1
 Summary: A Python client and wrapper around the 1Password CLI.
 Home-page: https://github.com/wandera/1password-client
 Author: David Pryce
-Author-email: david.pryce@wandera.com
+Author-email: david.prycecompson@jamf.com
 License: MIT
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.7
@@ -18,54 +18,85 @@
 # OnePassword python client
 [![PyPi release](https://github.com/wandera/1password-client/actions/workflows/publish-to-pypi.yml/badge.svg?branch=main&event=push)](https://github.com/wandera/1password-client/actions/workflows/publish-to-pypi.yml)
 [![CodeQL](https://github.com/wandera/1password-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/wandera/1password-client/actions/workflows/codeql-analysis.yml)
 
 Python client around the 1Password password manager cli for usage within python code and
 Jupyter Notebooks. Developed by Data Scientists from Jamf.
 
-Warning: this client is for use with 1Password 7 and earlier. For 1Password 8 there is a different CLI2, which we have 
-not yet fully tested within this client. Feel free to attempt to use a higher version of the cli or this client with
-1Password 8 and submit PRs to fix issues.
-
+## Supported versions
+There are some of the pre-requisites that are needed to use the library. We automatically install the cli for Mac and
+Linux users when installing the library. Windows users see below for help.
+
+- 1Password App: 8+
+- 1Password cli: 2+
+- Python: 3.10+
+
+## Operating systems
+The library is split into two parts: installation and client in which we are slowly updating to cover as many operating
+systems as possible the following table should ensure users understand what this library can and can't do at time of 
+install.
+
+|                 | MacOS | Linux | 
+|-----------------|-------|-------|
+| Fully supported | Y     | Y     | 
+| CLI install     | Y     | Y     | 
+| SSO login       | Y     | Y     | 
+| Login via App   | Y     | Y     | 
+| Biometrics auth | Y     | Y     | 
+| Password auth   | Y     | Y     | 
+| CLI client      | Y     | Y     | 
 
 ## Installation
 ```bash
 pip install 1password
 ```
 
 If you have issues with PyYaml or other distutils installed packages then use:
 ```bash
 pip install --ignore-installed 1password
 ```
 
 You are welcome to install and manage `op` yourself by visiting
 [the CLI1 downloads page](https://app-updates.agilebits.com/product_history/CLI ) to download the version you require 
-and follow instructions for your platform.
+and follow instructions for your platform as long as it's major version 2.
 
-The above commands will check `op` is present already and if not will install the best `op` cli it can work out plus 
-the python client itself. 
+The above commands pip commands will check `op` is present already and if not will install the supported `op` cli 
+plus the python client itself. 
 This is currently fixed at `op` version 1.12.5 to ensure compatibility. If you wish to use a higher version of `op` you
 can by following [this guide](https://developer.1password.com/docs/cli/upgrade), 
 however note that we cannot ensure it will work with our client yet. 
 
 MacOS users will be prompted with a separate installation window to ensure you have a signed version of `op` - make
 sure to check other desktops that the installer might pop up on. 
 
+
 ### Optional pre-requisites
 #### base32
 This utility is used to create a unique guid for your device but this isn't a hard requirement from AgileBits 
 and so if you see `base32: command not found` an empty string will be used instead, 
 and the client will still work fully.
 
 If you really want to, you can make sure you have this installed by installing coreutils. Details per platform can
 be found here: https://command-not-found.com/base32
 
 ## Basic Usage
-Currently tested on MacOS and Linux.
+Since v2 of the cli it is advised to connect your CLI to the local app installed on the device, thus removing the need
+for secret keys and passwords in the terminal or shell. Read here on how to do that: 
+https://developer.1password.com/docs/cli/get-started#step-2-turn-on-the-1password-desktop-app-integration
+
+An added extra for Mac users is that you can also enable TouchID for the app and by linking your cli with the app you 
+will get biometric login for both. 
+
+Once this is done any initial usage of the cli, and our client will request you to authenticate either via the app or 
+using your biometrics and then you can continue.
+
+We are sure there are use cases where the app cannot be linked and hence a password etc is till required so this 
+functionality is still present from our v1 implementation and can be described below
 
+### Password authentication
 On first usage users will be asked for both the enrolled email, secret key and password. 
 There is also verification of your account domain and name. 
 
 For all following usages you will only be asked for a password.
 
 You will be given 3 attempts and then pointed to reset password documentation or alternatively you can
 restart your kernel.
@@ -88,14 +119,15 @@
 
 # Get all fields, one field or more fields for an item with uuid="example"
 op.get_item(uuid="example")
 op.get_item(uuid="example", fields="username")
 op.get_item(uuid="example", fields=["username", "password"])
 
 ```
+## 
 
 ### Input formats
 To be sure what you are using is of the right format
 
 - Enrolled email: standard email format e.g. user@example.com 
 - Secret key: provided by 1Password e.g. ##-######-######-#####-#####-#####-#####
 - Account domain: domain that you would login to 1Password via browser e.g. example.1password.com
@@ -190,8 +222,7 @@
     - encode
     - forget
     - get
     - list
     - reactivate
     - remove
     - suspend
-- Use the new CLI update method
```

### Comparing `1password-0.6.2/README.md` & `1password-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,102 @@
+Metadata-Version: 2.1
+Name: 1password
+Version: 1.0.1
+Summary: A Python client and wrapper around the 1Password CLI.
+Home-page: https://github.com/wandera/1password-client
+Author: David Pryce
+Author-email: david.prycecompson@jamf.com
+License: MIT
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # OnePassword python client
 [![PyPi release](https://github.com/wandera/1password-client/actions/workflows/publish-to-pypi.yml/badge.svg?branch=main&event=push)](https://github.com/wandera/1password-client/actions/workflows/publish-to-pypi.yml)
 [![CodeQL](https://github.com/wandera/1password-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/wandera/1password-client/actions/workflows/codeql-analysis.yml)
 
 Python client around the 1Password password manager cli for usage within python code and
 Jupyter Notebooks. Developed by Data Scientists from Jamf.
 
-Warning: this client is for use with 1Password 7 and earlier. For 1Password 8 there is a different CLI2, which we have 
-not yet fully tested within this client. Feel free to attempt to use a higher version of the cli or this client with
-1Password 8 and submit PRs to fix issues.
-
+## Supported versions
+There are some of the pre-requisites that are needed to use the library. We automatically install the cli for Mac and
+Linux users when installing the library. Windows users see below for help.
+
+- 1Password App: 8+
+- 1Password cli: 2+
+- Python: 3.10+
+
+## Operating systems
+The library is split into two parts: installation and client in which we are slowly updating to cover as many operating
+systems as possible the following table should ensure users understand what this library can and can't do at time of 
+install.
+
+|                 | MacOS | Linux | 
+|-----------------|-------|-------|
+| Fully supported | Y     | Y     | 
+| CLI install     | Y     | Y     | 
+| SSO login       | Y     | Y     | 
+| Login via App   | Y     | Y     | 
+| Biometrics auth | Y     | Y     | 
+| Password auth   | Y     | Y     | 
+| CLI client      | Y     | Y     | 
 
 ## Installation
 ```bash
 pip install 1password
 ```
 
 If you have issues with PyYaml or other distutils installed packages then use:
 ```bash
 pip install --ignore-installed 1password
 ```
 
 You are welcome to install and manage `op` yourself by visiting
 [the CLI1 downloads page](https://app-updates.agilebits.com/product_history/CLI ) to download the version you require 
-and follow instructions for your platform.
+and follow instructions for your platform as long as it's major version 2.
 
-The above commands will check `op` is present already and if not will install the best `op` cli it can work out plus 
-the python client itself. 
+The above commands pip commands will check `op` is present already and if not will install the supported `op` cli 
+plus the python client itself. 
 This is currently fixed at `op` version 1.12.5 to ensure compatibility. If you wish to use a higher version of `op` you
 can by following [this guide](https://developer.1password.com/docs/cli/upgrade), 
 however note that we cannot ensure it will work with our client yet. 
 
 MacOS users will be prompted with a separate installation window to ensure you have a signed version of `op` - make
 sure to check other desktops that the installer might pop up on. 
 
+
 ### Optional pre-requisites
 #### base32
 This utility is used to create a unique guid for your device but this isn't a hard requirement from AgileBits 
 and so if you see `base32: command not found` an empty string will be used instead, 
 and the client will still work fully.
 
 If you really want to, you can make sure you have this installed by installing coreutils. Details per platform can
 be found here: https://command-not-found.com/base32
 
 ## Basic Usage
-Currently tested on MacOS and Linux.
+Since v2 of the cli it is advised to connect your CLI to the local app installed on the device, thus removing the need
+for secret keys and passwords in the terminal or shell. Read here on how to do that: 
+https://developer.1password.com/docs/cli/get-started#step-2-turn-on-the-1password-desktop-app-integration
+
+An added extra for Mac users is that you can also enable TouchID for the app and by linking your cli with the app you 
+will get biometric login for both. 
+
+Once this is done any initial usage of the cli, and our client will request you to authenticate either via the app or 
+using your biometrics and then you can continue.
+
+We are sure there are use cases where the app cannot be linked and hence a password etc is till required so this 
+functionality is still present from our v1 implementation and can be described below
 
+### Password authentication
 On first usage users will be asked for both the enrolled email, secret key and password. 
 There is also verification of your account domain and name. 
 
 For all following usages you will only be asked for a password.
 
 You will be given 3 attempts and then pointed to reset password documentation or alternatively you can
 restart your kernel.
@@ -71,14 +119,15 @@
 
 # Get all fields, one field or more fields for an item with uuid="example"
 op.get_item(uuid="example")
 op.get_item(uuid="example", fields="username")
 op.get_item(uuid="example", fields=["username", "password"])
 
 ```
+## 
 
 ### Input formats
 To be sure what you are using is of the right format
 
 - Enrolled email: standard email format e.g. user@example.com 
 - Secret key: provided by 1Password e.g. ##-######-######-#####-#####-#####-#####
 - Account domain: domain that you would login to 1Password via browser e.g. example.1password.com
@@ -173,8 +222,7 @@
     - encode
     - forget
     - get
     - list
     - reactivate
     - remove
     - suspend
-- Use the new CLI update method
```

### Comparing `1password-0.6.2/install_op.py` & `1password-1.0.1/install_op.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 import os
 import wget
 import zipfile
 import platform
 from subprocess import Popen, PIPE
 
-version_string = "v1.12.5"
+
+cli_version = "2.19.0"
+version_string = "v{}".format(cli_version)
+os.environ["OP_VERSION_STR"] = version_string
 platform_links = {
     "Darwin": {
-        "x86_64": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_apple_universal_{}.pkg".format(version_string,
+        "x86_64": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_apple_universal_{}.pkg".format(version_string,
+                                                                                                   version_string),
+        "arm64": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_apple_universal_{}.pkg".format(version_string,
                                                                                                    version_string),
         "download_loc": "/usr/local/bin/"
     },
     "FreeBSD": {
-        "i386": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_freebsd_386_{}.zip".format(version_string,
+        "i386": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_freebsd_386_{}.zip".format(version_string,
                                                                                              version_string),
-        "i686": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_freebsd_386_{}.zip".format(version_string,
+        "i686": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_freebsd_386_{}.zip".format(version_string,
                                                                                              version_string),
-        "x86_64": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_freebsd_amd64_{}.zip".format(version_string,
+        "x86_64": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_freebsd_amd64_{}.zip".format(version_string,
                                                                                                  version_string),
-        "arm": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_freebsd_arm_{}.zip".format(version_string,
+        "arm": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_freebsd_arm_{}.zip".format(version_string,
                                                                                             version_string),
-        "aarch64_be": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_freebsd_arm_{}.zip".format(version_string,
+        "aarch64_be": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_freebsd_arm_{}.zip".format(version_string,
                                                                                                    version_string),
-        "aarch64": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_freebsd_arm_{}.zip".format(version_string,
+        "aarch64": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_freebsd_arm_{}.zip".format(version_string,
                                                                                                 version_string),
-        "armv8b": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_freebsd_arm_{}.zip".format(version_string,
+        "armv8b": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_freebsd_arm_{}.zip".format(version_string,
                                                                                                version_string),
-        "armv8l": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_freebsd_arm_{}.zip".format(version_string,
+        "armv8l": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_freebsd_arm_{}.zip".format(version_string,
                                                                                                version_string),
         "download_loc": "/usr/local/bin/"
     },
     "Linux": {
-        "i386": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_linux_386_{}.zip".format(version_string,
+        "i386": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_linux_386_{}.zip".format(version_string,
                                                                                            version_string),
-        "i686": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_linux_386_{}.zip".format(version_string,
+        "i686": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_linux_386_{}.zip".format(version_string,
                                                                                            version_string),
-        "x86_64": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_linux_amd64_{}.zip".format(version_string,
+        "x86_64": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_linux_amd64_{}.zip".format(version_string,
                                                                                                version_string),
-        "aarch64_be": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_linux_arm_{}.zip".format(version_string,
+        "aarch64_be": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_linux_arm_{}.zip".format(version_string,
                                                                                                  version_string),
-        "aarch64": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_linux_arm_{}.zip".format(version_string,
+        "aarch64": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_linux_arm_{}.zip".format(version_string,
                                                                                               version_string),
-        "armv8b": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_linux_arm_{}.zip".format(version_string,
+        "armv8b": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_linux_arm_{}.zip".format(version_string,
                                                                                              version_string),
-        "armv8l": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_linux_arm_{}.zip".format(version_string,
+        "armv8l": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_linux_arm_{}.zip".format(version_string,
                                                                                              version_string),
-        "arm": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_linux_arm_{}.zip".format(version_string,
+        "arm": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_linux_arm_{}.zip".format(version_string,
                                                                                           version_string),
         "download_loc": "/usr/local/bin/"
     },
     "OpenBSD": {
-        "i386": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_openbsd_386_{}.zip".format(version_string,
+        "i386": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_openbsd_386_{}.zip".format(version_string,
                                                                                              version_string),
-        "i686": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_openbsd_386_{}.zip".format(version_string,
+        "i686": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_openbsd_386_{}.zip".format(version_string,
                                                                                              version_string),
-        "x86_64": "https://cache.agilebits.com/dist/1P/op/pkg/{}/op_openbsd_amd64_{}.zip".format(version_string,
+        "x86_64": "https://cache.agilebits.com/dist/1P/op2/pkg/{}/op_openbsd_amd64_{}.zip".format(version_string,
                                                                                                  version_string),
         "download_loc": "/usr/local/bin/"
     }
 }
 
 
 def read_bash_return(cmd, single=True):
@@ -67,61 +72,78 @@
     process.close()
     if single:
         return str(preprocessed.split("\n")[0])
     else:
         return str(preprocessed)
 
 
-def check_install_required():  # pragma: no cover
-    """
-    Helper function to check if op cli is already installed
-
-    :returns: :obj:`bool`: True or False
-
-     """
-    op = read_bash_return("op --version")
-    if op == "":
-        return True
-    else:
-        return False
-
-
 def mkdirpy(directory):
     if not os.path.exists(directory):
         os.makedirs(directory)
 
 
-def install_op():  # pragma: no cover
-    """
-    Helper function to download, unzip, install and chmod op cli files
-    """
-    if check_install_required():
-        system = str(platform.system())
+class CliInstaller:  # pragma: no cover
+    def __init__(self):
+        self.system = str(platform.system())
         machine = str(platform.machine())
-        link = platform_links[system][machine]
-        local_bin = platform_links[system]["download_loc"]
-        try:
-            os.chmod(local_bin, 0o755)
-        except PermissionError:
-            local_bin = os.path.join(os.environ["HOME"], "op-downloads")
-            mkdirpy(local_bin)
-            os.chmod(local_bin, 0o755)
-        op_file = link.split("/")[-1]
-        download_path = os.path.join(local_bin, op_file)
-        print('Downloading the 1Password CLI: {}'.format(op_file))
-        wget.download(link, download_path)
-        if link[-4:] != ".pkg":
-            zip_ref = zipfile.ZipFile(download_path, 'r')
-            zip_ref.extractall(local_bin)
-            zip_ref.close()
-            os.chmod(os.path.join(local_bin, 'op'), 0o755)
+        self.link = platform_links[self.system][machine]
+        self.download_location = platform_links[self.system]["download_loc"]
+
+    def install(self):
+        if self.system in platform_links.keys():
+            self.install_linux_mac()
         else:
-            Popen(["open", os.path.join(local_bin, op_file)], stdin=PIPE, stdout=PIPE)  # pragma: no cover
-    else:
-        print("op already installed")
+            raise OSError("Operating system not supported")
+
+    def check_install_required(self):  # pragma: no cover
+        """
+        Helper function to check if op cli is already installed
+
+        :returns: :obj:`bool`: True or False
+
+         """
+        op = read_bash_return("op --version")
+        if op == "":
+            return True, self.download_location
+        else:
+            if op == cli_version:
+                return False, ""
+            else:
+                existing_location = read_bash_return("which op")
+                return True, existing_location
+
+    def install_linux_mac(self):
+        """
+            Helper function to download, unzip, install and chmod op cli files
+            """
+        install_check, install_loc = self.check_install_required()
+        if install_check:
+            if install_loc == self.download_location:
+                local_bin = self.download_location
+            else:
+                local_bin = install_loc
+            try:
+                os.chmod(local_bin, 0o755)
+            except PermissionError:
+                local_bin = os.path.join(os.environ["HOME"], "op-downloads")
+                mkdirpy(local_bin)
+                os.chmod(local_bin, 0o755)
+            op_file = self.link.split("/")[-1]
+            download_path = os.path.join(local_bin, op_file)
+            print('Downloading the 1Password CLI: {}'.format(op_file))
+            wget.download(self.link, download_path)
+            if self.link[-4:] != ".pkg":
+                zip_ref = zipfile.ZipFile(download_path, 'r')
+                zip_ref.extractall(local_bin)
+                zip_ref.close()
+                os.chmod(os.path.join(local_bin, 'op'), 0o755)
+            else:
+                Popen(["open", os.path.join(local_bin, op_file)], stdin=PIPE, stdout=PIPE)  # pragma: no cover
+        else:
+            print("op already installed, with supported version.")
 
 
-def install_chocolatey():
-    """
-    Helper function for installing Windows package management requires that installation performed in admin role
-    """
-    pass
+if __name__ == '__main__':
+    # Run wizard if executed from terminal
+    install_cli = CliInstaller()
+    install_cli.install()
+    print()
```

### Comparing `1password-0.6.2/onepassword/utils.py` & `1password-1.0.1/onepassword/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,46 +50,37 @@
 
     :return: domain (str)
     """
     return address.split("@")[1].split(".")[0]
 
 
 def get_session_key(process_resp_before):
-    new_line_response = [x for x in str(process_resp_before).split(" ") if "\\r\\n" in x]
+    new_line_response = [x for x in process_resp_before.decode("utf-8").split("\n") if "\r" not in x]
     if len(new_line_response) != 1:
         raise IndexError("Session keys not parsed correctly from response: {}.".format(process_resp_before))
     else:
-        return new_line_response[0].split("\\r\\n")[1]
+        return new_line_response[0]
 
 
-def _spawn_signin(command, m_password):
+def _spawn_signin(command, m_password) -> str | bool:
     if command != "":
-        child = pexpect.spawn(command)
-        child.expect([master_password_regex, pexpect.EOF])
-        if child.isalive():
-            try:
-                child.sendline(m_password)
-            except OSError:
-                child.close()
-                child = pexpect.spawn(command)
-                child.expect([master_password_regex, pexpect.EOF])
-                child.sendline(m_password)
+        p = pexpect.spawn(command)
+        index = p.expect(master_password_regex)
+        if index == 0:
+            p.sendline(m_password)
+            index = p.expect([pexpect.EOF, "\(401\) Unauthorized"])
+            if index == 0:
+                sess_key = get_session_key(p.before)
+                p.close()
+                return sess_key
+            elif index == 1:
+                print("Input master password is not correct. Please try again")
+                return False
         else:
-            child.close()
-            child = pexpect.spawn(command)
-            child.expect([master_password_regex, pexpect.EOF])
-            child.sendline(m_password)
-        resp = child.expect(['Enter your six-digit authentication code:', pexpect.EOF])
-        if resp != 1:
-            auth_code = str(input("Please input your 1Password six-digit authentication code: "))
-            child.sendline(auth_code)
-            child.expect(pexpect.EOF)
-        sess_key = get_session_key(child.before)
-        child.close()
-        return sess_key
+            raise IOError("Onepassword command not valid")
     else:
         raise IOError("Spawn command not valid")
 
 
 class BashProfile:
     def __init__(self):
         f = None
```

### Comparing `1password-0.6.2/setup.py` & `1password-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 from setuptools.command.install import install
 
 
 class PostDevelopCommand(develop):
     """Post-installation for development mode."""
     def run(self):
         develop.run(self)
-        from install_op import install_op
-        install_op()
+        from install_op import CliInstaller
+        install_cli = CliInstaller()
+        install_cli.install()
 
 
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
-        from install_op import install_op
-        install_op()
-
+        from install_op import CliInstaller
+        install_cli = CliInstaller()
+        install_cli.install()
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 root_dir = os.getcwd()
@@ -30,15 +31,15 @@
     version = version_file.read().strip()
 
 
 setup(
     name="1password",
     version=version,
     author="David Pryce",
-    author_email="david.pryce@wandera.com",
+    author_email="david.prycecompson@jamf.com",
     description="A Python client and wrapper around the 1Password CLI.",
     long_description=readme(),
     long_description_content_type='text/markdown',
     install_requires=[
         "wget",
         "pyyaml",
         "pycryptodome",
```

### Comparing `1password-0.6.2/test/test_client.py` & `1password-1.0.1/test/test_client.py`

 * *Files identical despite different names*

