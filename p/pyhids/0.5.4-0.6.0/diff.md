# Comparing `tmp/pyhids-0.5.4.tar.gz` & `tmp/pyhids-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhids-0.5.4.tar", max compression
+gzip compressed data, was "pyhids-0.6.0.tar", max compression
```

## Comparing `pyhids-0.5.4.tar` & `pyhids-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rwxr-xr-x   0        0        0    35147 2023-07-21 17:40:28.550202 pyhids-0.5.4/COPYING
--rwxr-xr-x   0        0        0     4307 2023-07-21 17:40:28.546202 pyhids-0.5.4/README.md
--rwxr-xr-x   0        0        0     2643 2023-07-21 17:43:55.448222 pyhids-0.5.4/conf.py
--rw-r--r--   0        0        0        0 2023-07-19 18:15:45.896004 pyhids-0.5.4/pyhids/__init__.py
--rwxr-xr-x   0        0        0     4331 2023-07-21 17:45:03.151520 pyhids-0.5.4/pyhids/genBase.py
--rwxr-xr-x   0        0        0     1770 2023-07-21 17:40:27.914215 pyhids-0.5.4/pyhids/genKeys.py
--rwxr-xr-x   0        0        0    11035 2023-07-21 17:42:18.087889 pyhids-0.5.4/pyhids/pyHIDS.py
--rw-r--r--   0        0        0     1161 2023-07-21 18:07:04.103363 pyhids-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 pyhids-0.5.4/PKG-INFO
+-rwxr-xr-x   0        0        0    35147 2023-07-21 17:40:28.550202 pyhids-0.6.0/COPYING
+-rwxr-xr-x   0        0        0     4718 2023-08-03 12:08:18.728201 pyhids-0.6.0/README.md
+-rwxr-xr-x   0        0        0     2853 2023-08-03 11:38:35.125802 pyhids-0.6.0/conf.py
+-rw-r--r--   0        0        0        0 2023-07-19 18:15:45.896004 pyhids-0.6.0/pyhids/__init__.py
+-rwxr-xr-x   0        0        0     4315 2023-08-02 06:50:21.139800 pyhids-0.6.0/pyhids/genBase.py
+-rwxr-xr-x   0        0        0     1770 2023-07-21 17:40:27.914215 pyhids-0.6.0/pyhids/genKeys.py
+-rw-r--r--   0        0        0     1349 2023-08-03 11:19:10.142113 pyhids-0.6.0/pyhids/hashlookup.py
+-rw-r--r--   0        0        0      850 2023-08-03 12:05:18.302018 pyhids-0.6.0/pyhids/pandora.py
+-rwxr-xr-x   0        0        0    10390 2023-08-02 06:50:21.139800 pyhids-0.6.0/pyhids/pyHIDS.py
+-rw-r--r--   0        0        0      498 2023-08-03 08:21:41.402626 pyhids-0.6.0/pyhids/utils.py
+-rw-r--r--   0        0        0     1206 2023-08-03 12:30:16.477963 pyhids-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5740 1970-01-01 00:00:00.000000 pyhids-0.6.0/PKG-INFO
```

### Comparing `pyhids-0.5.4/COPYING` & `pyhids-0.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyhids-0.5.4/README.md` & `pyhids-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 
 It is recommended to use Python >= 3.11.
 
 ### Features
 
 * checks the integrity of system's files with a list of rules;
 * checks the output of commands (*iptables*, ...);
-* uses an RSA signature to check the integrity of its database;
+* possibity to use RSA to sign to check the integrity of its database;
+* verify files with [Hashlookup](https://github.com/hashlookup);
+* verify files with [Pandora](https://github.com/pandora-analysis);
 * alerts are written in the logs of the system;
 * alerts can be sent via email to a list of users;
 * alerts can be sent on IRC channels through the
   [irker](https://gitlab.com/esr/irker) IRC client (which should be running as
   a daemon).
 
 
@@ -81,14 +83,20 @@
 [18/07/23 22:34:25] [notice] /bin/pamperspective ok
 [18/07/23 22:34:25] [notice] /bin/pod2usage ok
 [18/07/23 22:34:25] Error(s) : 0
 [18/07/23 22:34:25] Warning(s) : 0
 [18/07/23 22:34:25] HIDS finished.
 ```
 
+Check for known malicious files with
+[Hashlookup](https://github.com/hashlookup):
+
+```bash
+$ pyhids hashlookup
+```
 
 #### From the repository
 
 Get pyHIDS source code and copy the
 sample configuration file:
 
 ```bash
@@ -102,15 +110,22 @@
 
 
 ### Configuration
 
 The configuration file of pyHIDS looks like the following:
 
 ```ini
+[hashlookup]
+root_url = https://hashlookup.circl.lu/
+[pandora]
+root_url = https://pandora.circl.lu/
+username = <username>
+password = <password>
 [irc]
+enabled = 0
 channel = irc://irc.libera.chat/#testpyHIDS
 host = localhost
 port = 6697
 [email]
 enabled = 0
 mail_from = pyHIDS@no-reply.com
 mail_to = you_address
```

### Comparing `pyhids-0.5.4/conf.py` & `pyhids-0.6.0/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #! /usr/bin/env python
 
 """
 pyHIDS. Python HIDS. Security software.
 pyHIDS verify the integrity of your system.
-Copyright (C) 2010-2013 Cedric Bonhomme
+Copyright (C) 2010-2023 Cedric Bonhomme
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -44,14 +44,20 @@
 MAIL_ENABLED = bool(config.getint("email", "enabled"))
 MAIL_FROM = config.get("email", "mail_from")
 MAIL_TO = [config.get("email", "mail_to")]
 SMTP_SERVER = config.get("email", "smtp")
 USERNAME = config.get("email", "username")
 PASSWORD = config.get("email", "password")
 
+HASHLOOKUP_URL = config.get("hashlookup", "root_url")
+
+PANDORA_URL = config.get("pandora", "root_url")
+PANDORA_USERNAME = config.get("pandora", "username")
+PANDORA_PASSWORD = config.get("pandora", "password")
+
 # address of the log file :
 LOGS = os.path.join(PATH, "log")
 # address of the database of hash values :
 DATABASE = os.path.join(PATH, "database")
 # address of the signature of the database:
 DATABASE_SIG = os.path.join(PATH, "database.sig")
```

### Comparing `pyhids-0.5.4/pyhids/genBase.py` & `pyhids-0.6.0/pyhids/genBase.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     return result
 
 
 def hash_file(target_file):
     """
     Hash the file given in parameter.
     """
-    sha256_hash = hashlib.sha256()
+    sha1_hash = hashlib.sha1()
     opened_file = None
     hashed_data = None
     data = None
 
     # Handle the errors that may happen
     try:
         opened_file = open(target_file, "rb")
@@ -73,16 +73,16 @@
         globals()["number_of_files_to_scan"] = globals()["number_of_files_to_scan"] - 1
         del list_of_files[list_of_files.index(target_file)]
     finally:
         if data is not None:
             opened_file.close()
 
     if data is not None:
-        sha256_hash.update(data)
-        hashed_data = sha256_hash.hexdigest()
+        sha1_hash.update(data)
+        hashed_data = sha1_hash.hexdigest()
 
     return hashed_data
 
 
 def main(sign_database=False):
     database = {}
     database["files"] = {}
@@ -109,17 +109,17 @@
         try:
             proc = subprocess.Popen(
                 (command), stderr=subprocess.STDOUT, stdout=subprocess.PIPE
             )
         except FileNotFoundError:
             continue
         command_output = proc.stdout.read()
-        sha256_hash = hashlib.sha256()
-        sha256_hash.update(command_output)
-        hashed_data = sha256_hash.hexdigest()
+        sha1_hash = hashlib.sha1()
+        sha1_hash.update(command_output)
+        hashed_data = sha1_hash.hexdigest()
         database["commands"][command] = hashed_data
 
     serialized_database = open(conf.DATABASE, "wb")
     pickle.dump(database, serialized_database)
     serialized_database.close()
 
     print(number_of_files_to_scan, "files in the database.")
```

### Comparing `pyhids-0.5.4/pyhids/genKeys.py` & `pyhids-0.6.0/pyhids/genKeys.py`

 * *Files identical despite different names*

### Comparing `pyhids-0.5.4/pyhids/pyHIDS.py` & `pyhids-0.6.0/pyhids/pyHIDS.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 #!/usr/bin/env python
 
-"""pyHIDS. Python HIDS implementation.
-
-pyHIDS verify the integrity of your system.
-pyHIDS can send alerts by email, log file and syslog.
-"""
-
 """
 pyHIDS. Python HIDS. Security software.
 pyHIDS verify the integrity of your system.
 Copyright (C) 2010-2023 Cedric Bonhomme
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
@@ -44,50 +38,32 @@
 import time
 from contextlib import contextmanager
 from email.mime.text import MIMEText
 
 import rsa
 
 import conf
+from pyhids import utils
 
 # lock object to protect the log file during the writing
 lock = threading.Lock()
 # lock object used when sending alerts via irc
 irker_lock = threading.Lock()
 
 Q = queue.Queue()
 
 
-def load_base():
-    """
-    Load the base file.
-
-    Return a dictionnary wich contains filenames
-    and theirs hash value.
-    """
-    # try to open the saved base of hash values
-    database = None
-    with open(conf.DATABASE, "rb") as serialized_database:
-        database = pickle.load(serialized_database)
-    # try:
-    # base_file = open(conf.DATABASE, "r")
-    # except:
-    # globals()['warning'] = globals()['warning'] + 1
-    # log("Base file " + conf.DATABASE + " does no exist.")
-    return database
-
-
 def compare_hash(target_file, expected_hash):
     """
     Compare 2 hash values.
 
     Compare the hash value of the target file
     with the expected hash value.
     """
-    sha256_hash = hashlib.sha256()
+    sha1_hash = hashlib.sha1()
     opened_file = None
 
     # each log's line contain the local time. it makes research easier.
     local_time = time.strftime("[%d/%m/%y %H:%M:%S]", time.localtime())
 
     # test for safety. Normally expected_hash != "" thanks to genBase.py
     if expected_hash == "":
@@ -109,16 +85,16 @@
         )
     finally:
         if opened_file is not None:
             opened_file.close()
 
     # now we're ready to compare the hash values
     if opened_file is not None:
-        sha256_hash.update(data)
-        hashed_data = sha256_hash.hexdigest()
+        sha1_hash.update(data)
+        hashed_data = sha1_hash.hexdigest()
 
         if hashed_data == expected_hash:
             # no changes, just write a notice in the log file
             log(local_time + " [notice] " + target_file + " ok")
         else:
             # hash has changed, warning
 
@@ -142,17 +118,17 @@
 
 def compare_command_hash(command, expected_hash):
     # each log's line contain the local time. it makes research easier.
     local_time = time.strftime("[%d/%m/%y %H:%M:%S]", time.localtime())
 
     proc = subprocess.Popen(command, stderr=subprocess.STDOUT, stdout=subprocess.PIPE)
     command_output = proc.stdout.read()
-    sha256_hash = hashlib.sha256()
-    sha256_hash.update(command_output)
-    hashed_data = sha256_hash.hexdigest()
+    sha1_hash = hashlib.sha1()
+    sha1_hash.update(command_output)
+    hashed_data = sha1_hash.hexdigest()
 
     if hashed_data == expected_hash:
         # no changes, just write a notice in the log file
         log(local_time + " [notice] " + " ".join(command) + " ok")
     else:
         # hash has changed, warning
 
@@ -288,15 +264,15 @@
         print("Something wrong happens when opening the logs: " + str(e))
         exit(0)
     log(time.strftime("[%d/%m/%y %H:%M:%S] HIDS starting.", time.localtime()))
 
     warning, error = 0, 0
 
     # dictionnary containing filenames and their hash value.
-    base = load_base()
+    base = utils.load_base()
     if base is None:
         print("Base of hash values can not be loaded.")
         exit(0)
 
     report = ""
 
     # Check the integrity of monitored files
```

### Comparing `pyhids-0.5.4/pyproject.toml` & `pyhids-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyHIDS"
-version = "0.5.4"
+version = "0.6.0"
 description = "A host-based intrusion detection system."
 authors = ["Cédric Bonhomme <cedric@cedricbonhomme.org>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 homepage = "https://github.com/cedricbonhomme/pyHIDS"
 repository = "https://github.com/cedricbonhomme/pyHIDS"
@@ -31,14 +31,16 @@
 
 [tool.poetry.scripts]
 pyhids = "bin.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 rsa = "^4.9"
+pyhashlookup = "^1.2.1"
+pypandora = "^1.5.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 mypy = "^1.4.1"
 pre-commit = "^3.3.3"
 
 [build-system]
```

### Comparing `pyhids-0.5.4/PKG-INFO` & `pyhids-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhids
-Version: 0.5.4
+Version: 0.6.0
 Summary: A host-based intrusion detection system.
 Home-page: https://github.com/cedricbonhomme/pyHIDS
 License: GPL-3.0-or-later
 Keywords: hids,security
 Author: Cédric Bonhomme
 Author-email: cedric@cedricbonhomme.org
 Requires-Python: >=3.11,<4.0
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Security
+Requires-Dist: pyhashlookup (>=1.2.1,<2.0.0)
+Requires-Dist: pypandora (>=1.5.0,<2.0.0)
 Requires-Dist: rsa (>=4.9,<5.0)
 Project-URL: Repository, https://github.com/cedricbonhomme/pyHIDS
 Description-Content-Type: text/markdown
 
 ## pyHIDS
 
 ### Presentation
@@ -37,15 +39,17 @@
 
 It is recommended to use Python >= 3.11.
 
 ### Features
 
 * checks the integrity of system's files with a list of rules;
 * checks the output of commands (*iptables*, ...);
-* uses an RSA signature to check the integrity of its database;
+* possibity to use RSA to sign to check the integrity of its database;
+* verify files with [Hashlookup](https://github.com/hashlookup);
+* verify files with [Pandora](https://github.com/pandora-analysis);
 * alerts are written in the logs of the system;
 * alerts can be sent via email to a list of users;
 * alerts can be sent on IRC channels through the
   [irker](https://gitlab.com/esr/irker) IRC client (which should be running as
   a daemon).
 
 
@@ -105,14 +109,20 @@
 [18/07/23 22:34:25] [notice] /bin/pamperspective ok
 [18/07/23 22:34:25] [notice] /bin/pod2usage ok
 [18/07/23 22:34:25] Error(s) : 0
 [18/07/23 22:34:25] Warning(s) : 0
 [18/07/23 22:34:25] HIDS finished.
 ```
 
+Check for known malicious files with
+[Hashlookup](https://github.com/hashlookup):
+
+```bash
+$ pyhids hashlookup
+```
 
 #### From the repository
 
 Get pyHIDS source code and copy the
 sample configuration file:
 
 ```bash
@@ -126,15 +136,22 @@
 
 
 ### Configuration
 
 The configuration file of pyHIDS looks like the following:
 
 ```ini
+[hashlookup]
+root_url = https://hashlookup.circl.lu/
+[pandora]
+root_url = https://pandora.circl.lu/
+username = <username>
+password = <password>
 [irc]
+enabled = 0
 channel = irc://irc.libera.chat/#testpyHIDS
 host = localhost
 port = 6697
 [email]
 enabled = 0
 mail_from = pyHIDS@no-reply.com
 mail_to = you_address
```

