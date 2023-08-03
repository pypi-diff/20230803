# Comparing `tmp/telebirrTxChecker-0.0.1.tar.gz` & `tmp/telebirrTxChecker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebirrTxChecker-0.0.1.tar", last modified: Wed Aug  2 17:35:10 2023, max compression
+gzip compressed data, was "telebirrTxChecker-0.0.3.tar", last modified: Thu Aug  3 12:23:55 2023, max compression
```

## Comparing `telebirrTxChecker-0.0.1.tar` & `telebirrTxChecker-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 17:35:10.734011 telebirrTxChecker-0.0.1/
--rw-rw-rw-   0        0        0      242 2023-08-02 17:35:10.733009 telebirrTxChecker-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      774 2023-08-02 14:17:15.000000 telebirrTxChecker-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-02 17:35:10.734011 telebirrTxChecker-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      490 2023-08-02 17:34:40.000000 telebirrTxChecker-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:35:10.651943 telebirrTxChecker-0.0.1/telebirrTxChecker.egg-info/
--rw-rw-rw-   0        0        0      242 2023-08-02 17:35:10.000000 telebirrTxChecker-0.0.1/telebirrTxChecker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-08-02 17:35:10.000000 telebirrTxChecker-0.0.1/telebirrTxChecker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 17:35:10.000000 telebirrTxChecker-0.0.1/telebirrTxChecker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-08-02 17:35:10.000000 telebirrTxChecker-0.0.1/telebirrTxChecker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-02 17:35:10.000000 telebirrTxChecker-0.0.1/telebirrTxChecker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 17:35:10.688531 telebirrTxChecker-0.0.1/ttxc/
--rw-rw-rw-   0        0        0       36 2023-08-02 07:00:00.000000 telebirrTxChecker-0.0.1/ttxc/__init__.py
--rw-rw-rw-   0        0        0      170 2023-04-12 15:48:51.000000 telebirrTxChecker-0.0.1/ttxc/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:35:10.697101 telebirrTxChecker-0.0.1/ttxc/errors/
--rw-rw-rw-   0        0        0      150 2023-04-12 15:53:24.000000 telebirrTxChecker-0.0.1/ttxc/errors/__init__.py
--rw-rw-rw-   0        0        0     2088 2023-08-02 07:49:46.000000 telebirrTxChecker-0.0.1/ttxc/main.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:35:10.732011 telebirrTxChecker-0.0.1/ttxc/types/
--rw-rw-rw-   0        0        0       96 2023-04-12 14:48:13.000000 telebirrTxChecker-0.0.1/ttxc/types/__init__.py
--rw-rw-rw-   0        0        0      209 2023-04-12 14:34:21.000000 telebirrTxChecker-0.0.1/ttxc/types/payer.py
--rw-rw-rw-   0        0        0      170 2023-04-12 14:36:00.000000 telebirrTxChecker-0.0.1/ttxc/types/receiver.py
--rw-rw-rw-   0        0        0     1207 2023-08-02 07:00:00.000000 telebirrTxChecker-0.0.1/ttxc/types/transaction.py
--rw-rw-rw-   0        0        0     2261 2023-04-12 17:30:46.000000 telebirrTxChecker-0.0.1/ttxc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:23:55.609854 telebirrTxChecker-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-03 12:23:55.609854 telebirrTxChecker-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:23:55.609854 telebirrTxChecker-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:23:55.605854 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-03 12:23:55.000000 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-03 12:23:55.000000 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:23:55.000000 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-03 12:23:55.000000 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 12:23:55.000000 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:23:55.605854 telebirrTxChecker-0.0.3/ttxc/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:23:55.605854 telebirrTxChecker-0.0.3/ttxc/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:23:55.609854 telebirrTxChecker-0.0.3/ttxc/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/types/payer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/types/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/types/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/utils.py
```

### Comparing `telebirrTxChecker-0.0.1/ttxc/main.py` & `telebirrTxChecker-0.0.3/ttxc/main.py`

 * *Files identical despite different names*

### Comparing `telebirrTxChecker-0.0.1/ttxc/types/transaction.py` & `telebirrTxChecker-0.0.3/ttxc/types/transaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,7 +36,23 @@
 
     @property
     def is_paid(self):
         return self.status.lower() == "completed"
 
     async def save_pdf(self, path: str) -> bool:
         return await self.base.save_pdf(self.id, path)
+
+    def dict(self):
+        return {
+            "id": self.id,
+            "payer": self.payer.__dict__,
+            "receiver": self.receiver.__dict__,
+            "status": self.status,
+            "discount": self.discount,
+            "vat": self.vat,
+            "total_amount_in_word": self.total_amount_in_word,
+            "total_sent": self.total_sent,
+            "date": self.date.isoformat(),
+            "mode": self.mode,
+            "reason": self.reason,
+            "channel": self.channel,
+        }
```

### Comparing `telebirrTxChecker-0.0.1/ttxc/utils.py` & `telebirrTxChecker-0.0.3/ttxc/utils.py`

 * *Files identical despite different names*

