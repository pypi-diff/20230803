# Comparing `tmp/bits-mx-1.0.8.tar.gz` & `tmp/bits-mx-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bits-mx-1.0.8.tar", last modified: Mon Nov  2 19:26:26 2020, max compression
+gzip compressed data, was "bits-mx-1.0.9.tar", last modified: Thu Aug  3 18:08:22 2023, max compression
```

## Comparing `bits-mx-1.0.8.tar` & `bits-mx-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2020-11-02 19:26:26.000000 bits-mx-1.0.8/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      224 2020-11-02 19:26:26.000000 bits-mx-1.0.8/PKG-INFO
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)       26 2019-02-28 14:27:23.000000 bits-mx-1.0.8/README.md
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2020-11-02 19:26:26.000000 bits-mx-1.0.8/bits/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)       89 2019-09-20 16:22:21.000000 bits-mx-1.0.8/bits/__init__.py
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2020-11-02 19:26:26.000000 bits-mx-1.0.8/bits/mx/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      712 2019-09-20 16:22:21.000000 bits-mx-1.0.8/bits/mx/__init__.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     2506 2019-09-20 16:22:21.000000 bits-mx-1.0.8/bits/mx/gnarwl.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     3046 2020-04-24 16:45:24.000000 bits-mx-1.0.8/bits/mx/google.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     2524 2019-09-20 16:22:21.000000 bits-mx-1.0.8/bits/mx/groups.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     1954 2019-09-20 16:22:21.000000 bits-mx-1.0.8/bits/mx/localmail.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     2570 2020-04-24 16:45:24.000000 bits-mx-1.0.8/bits/mx/nicknames.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     4195 2019-09-20 16:22:21.000000 bits-mx-1.0.8/bits/mx/rt.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     9506 2020-11-02 19:24:31.000000 bits-mx-1.0.8/bits/mx/update.py
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2020-11-02 19:26:26.000000 bits-mx-1.0.8/bits_mx.egg-info/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      224 2020-11-02 19:26:26.000000 bits-mx-1.0.8/bits_mx.egg-info/PKG-INFO
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      377 2020-11-02 19:26:26.000000 bits-mx-1.0.8/bits_mx.egg-info/SOURCES.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)        1 2020-11-02 19:26:26.000000 bits-mx-1.0.8/bits_mx.egg-info/dependency_links.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)        1 2020-11-02 19:26:26.000000 bits-mx-1.0.8/bits_mx.egg-info/not-zip-safe
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)       21 2020-11-02 19:26:26.000000 bits-mx-1.0.8/bits_mx.egg-info/requires.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)        5 2020-11-02 19:26:26.000000 bits-mx-1.0.8/bits_mx.egg-info/top_level.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      121 2020-11-02 19:26:26.000000 bits-mx-1.0.8/setup.cfg
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     1017 2020-11-02 19:25:50.000000 bits-mx-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:08:22.656836 bits-mx-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      166 2023-08-03 18:08:22.658361 bits-mx-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       26 2023-03-28 19:15:07.000000 bits-mx-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:08:22.483310 bits-mx-1.0.9/bits/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:08:22.577608 bits-mx-1.0.9/bits/mx/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/mx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/mx/gnarwl.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/mx/google.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/mx/groups.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/mx/localmail.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2023-05-08 19:04:51.000000 bits-mx-1.0.9/bits/mx/nicknames.py
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-05-08 15:26:23.000000 bits-mx-1.0.9/bits/mx/rt.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2023-05-08 19:07:02.000000 bits-mx-1.0.9/bits/mx/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:08:22.649244 bits-mx-1.0.9/bits_mx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      166 2023-08-03 18:08:22.000000 bits-mx-1.0.9/bits_mx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      377 2023-08-03 18:08:22.000000 bits-mx-1.0.9/bits_mx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 18:08:22.000000 bits-mx-1.0.9/bits_mx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 17:20:55.000000 bits-mx-1.0.9/bits_mx.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-03 18:08:22.000000 bits-mx-1.0.9/bits_mx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-03 18:08:22.000000 bits-mx-1.0.9/bits_mx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-08-03 18:08:22.664063 bits-mx-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-08 19:10:28.000000 bits-mx-1.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bits-mx-1.0.8/bits/mx/__init__.py` & `bits-mx-1.0.9/bits/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `bits-mx-1.0.8/bits/mx/gnarwl.py` & `bits-mx-1.0.9/bits/mx/gnarwl.py`

 * *Files identical despite different names*

### Comparing `bits-mx-1.0.8/bits/mx/google.py` & `bits-mx-1.0.9/bits/mx/google.py`

 * *Files identical despite different names*

### Comparing `bits-mx-1.0.8/bits/mx/groups.py` & `bits-mx-1.0.9/bits/mx/groups.py`

 * *Files identical despite different names*

### Comparing `bits-mx-1.0.8/bits/mx/localmail.py` & `bits-mx-1.0.9/bits/mx/localmail.py`

 * *Files identical despite different names*

### Comparing `bits-mx-1.0.8/bits/mx/nicknames.py` & `bits-mx-1.0.9/bits/mx/nicknames.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,28 +57,28 @@
             user_aliases = []
             if user_nicknames:
                 user_aliases = user_nicknames.get('nicknames', [])
 
             # process aliases
             for alias in user_aliases:
                 aliases.append('%s: %s@broadinstitute.org' % (
-                    alias,
-                    username
+                    alias.strip(),
+                    username.strip()
                 ))
 
         # add in sa account aliases for folks without a google sa
         for oid in self.update.all_other_accounts:
             user = self.update.all_other_accounts[oid]
 
             # get ad username, broad username, and google username
             ad_username = user.get('ad_username')
             broad_username = user.get('broad_username')
             google_username = user.get('google_username')
 
             # if ad_username starts with "sa-" and google_username doesn't exist
             if ad_username and ad_username.startswith('sa-') and not google_username:
                 aliases.append('%s: %s@broadinstitute.org' % (
-                    ad_username,
-                    broad_username
+                    ad_username.strip(),
+                    broad_username.strip()
                 ))
 
         return sorted(aliases)
```

### Comparing `bits-mx-1.0.8/bits/mx/rt.py` & `bits-mx-1.0.9/bits/mx/rt.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,38 +26,33 @@
         )
 
         # get program name
         self.program = os.path.basename(sys.argv[0])
 
         # server hosts
         self.help_host = 'help.broadinstitute.org'
-        self.rt_host = 'rt.broadinstitute.org'
 
         # bitsdb monogo collection
         self.collection = {}
 
     def generate(self):
         """Return the contents of the puppetfile."""
         # define header
         output = '# This file is autogenerated by the bits-mx %s script.\n' % (
             self.program
         )
         output += '# Do not make local modifications to this file.\n'
 
         # get aliases
         help_aliases = self.get_aliases(self.update.help_queues, self.help_host)
-        rt_aliases = self.get_aliases(self.update.rt_queues, self.rt_host)
 
         # users without a forward
         output += '\n#\n# %s aliases\n#\n' % (self.help_host)
         output += '\n'.join(help_aliases)
 
-        # users with a forward
-        output += '\n\n#\n# %s aliases\n#\n' % (self.rt_host)
-        output += '\n'.join(rt_aliases)
         return output
 
     def get_alias(self, queue, mailhost):
         """Return an alias entry for an RT queue."""
         # get name and description
         name = queue['Name']
         description = queue['Description']
```

### Comparing `bits-mx-1.0.8/bits/mx/update.py` & `bits-mx-1.0.9/bits/mx/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         self.gnarwl = None
         self.google_other_accounts = None
         self.groups = None
         self.help_queues = None
         self.localmail = None
         self.nicknames = None
         self.people = None
-        self.rt_queues = None
 
     def all(self):
         """Update everything."""
         self.gnarwl_aliases()
         self.gnarwl_ldap()
         self.google_transport()
         self.groups_transport()
@@ -121,24 +120,14 @@
             return self.people
         if self.verbose:
             print('Getting people from PeopleDB...')
         p = self.auth.people()
         self.people = p.getPeople('username')
         return self.people
 
-    def get_rt_queues(self):
-        """Get RT queues from rt."""
-        if self.rt_queues:
-            return self.rt_queues
-        if self.verbose:
-            print('Getting rt queues from RT...')
-        r = self.auth.rt()
-        self.rt_queues = r.getQueues()
-        return self.rt_queues
-
     def gnarwl_aliases(self):
         """Update Gnarwl aliases."""
         g = Gnarwl(self)
         if self.verbose:
             print('Updating gnarwl aliases...')
         # get gnarwl and nickname data
         gnarwl = self.get_gnarwl()
@@ -254,25 +243,19 @@
 
     def rt_aliases(self):
         """Update RT aliases."""
         rt = RT(self)
         if self.verbose:
             print('Updating rt aliases...')
         help_queues = self.get_help_queues()
-        rt_queues = self.get_rt_queues()
         # check help_queues data
         if len(help_queues) < 10:
             print('ERROR: Not enough help entries (%s), exiting.' % (
                 len(help_queues)
             ))
-        # check rt_queues data
-        if len(rt_queues) < 10:
-            print('ERROR: Not enough rt entries (%s), exiting.' % (
-                len(rt_queues)
-            ))
         output = rt.generate()
         # write file
         self.write_file(rt.puppetfile, output)
         if self.verbose:
             print('Wrote rt aliases to: %s\n' % (rt.puppetfile))
 
     def write_file(self, filename, output):
```

### Comparing `bits-mx-1.0.8/setup.py` & `bits-mx-1.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='bits-mx',
 
-    version='1.0.8',
+    version='1.0.9',
 
     description='BITS MX',
     long_description='',
 
     author='Lukas Karlsson',
     author_email='karlsson@broadinstitute.org',
```

