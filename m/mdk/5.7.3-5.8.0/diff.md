# Comparing `tmp/mdk-5.7.3.tar.gz` & `tmp/mdk-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdk-5.7.3.tar", last modified: Tue Jul 25 23:20:51 2023, max compression
+gzip compressed data, was "mdk-5.8.0.tar", last modified: Thu Aug  3 21:46:24 2023, max compression
```

## Comparing `mdk-5.7.3.tar` & `mdk-5.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-25 23:20:51.628290 mdk-5.7.3/
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1068 2023-07-21 16:55:29.000000 mdk-5.7.3/LICENSE
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1430 2023-07-25 23:20:51.628290 mdk-5.7.3/PKG-INFO
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      921 2023-07-21 16:55:29.000000 mdk-5.7.3/README.md
-drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-25 23:20:51.628290 mdk-5.7.3/mdk/
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        0 2023-07-21 16:55:29.000000 mdk-5.7.3/mdk/__init__.py
--rwxrwxr-x   0 austin    (3007) ldap-eng  (2001)     3620 2023-07-21 16:55:29.000000 mdk-5.7.3/mdk/main.py
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)    16978 2023-07-25 23:19:57.000000 mdk-5.7.3/mdk/utils.py
-drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-25 23:20:51.628290 mdk-5.7.3/mdk.egg-info/
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1430 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/PKG-INFO
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      241 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/SOURCES.txt
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        1 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/dependency_links.txt
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)       38 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/entry_points.txt
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        9 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/requires.txt
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        4 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/top_level.txt
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)       67 2023-07-25 23:20:51.628290 mdk-5.7.3/setup.cfg
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      985 2023-07-21 16:55:29.000000 mdk-5.7.3/setup.py
+drwxr-xr-x   0 dspyz     (1000) dspyz     (1000)        0 2023-08-03 21:46:24.087436 mdk-5.8.0/
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)     1068 2023-08-03 20:53:39.000000 mdk-5.8.0/LICENSE
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)     1410 2023-08-03 21:46:24.087436 mdk-5.8.0/PKG-INFO
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)      921 2023-08-03 20:53:39.000000 mdk-5.8.0/README.md
+drwxr-xr-x   0 dspyz     (1000) dspyz     (1000)        0 2023-08-03 21:46:24.087436 mdk-5.8.0/mdk/
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)        0 2023-08-03 20:53:39.000000 mdk-5.8.0/mdk/__init__.py
+-rwxr-xr-x   0 dspyz     (1000) dspyz     (1000)     3966 2023-08-03 21:04:15.000000 mdk-5.8.0/mdk/main.py
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)    17206 2023-08-03 21:13:02.000000 mdk-5.8.0/mdk/utils.py
+drwxr-xr-x   0 dspyz     (1000) dspyz     (1000)        0 2023-08-03 21:46:24.087436 mdk-5.8.0/mdk.egg-info/
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)     1410 2023-08-03 21:46:24.000000 mdk-5.8.0/mdk.egg-info/PKG-INFO
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)      241 2023-08-03 21:46:24.000000 mdk-5.8.0/mdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)        1 2023-08-03 21:46:24.000000 mdk-5.8.0/mdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)       37 2023-08-03 21:46:24.000000 mdk-5.8.0/mdk.egg-info/entry_points.txt
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)        9 2023-08-03 21:46:24.000000 mdk-5.8.0/mdk.egg-info/requires.txt
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)        4 2023-08-03 21:46:24.000000 mdk-5.8.0/mdk.egg-info/top_level.txt
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)       67 2023-08-03 21:46:24.087436 mdk-5.8.0/setup.cfg
+-rw-r--r--   0 dspyz     (1000) dspyz     (1000)      985 2023-08-03 20:53:39.000000 mdk-5.8.0/setup.py
```

### Comparing `mdk-5.7.3/LICENSE` & `mdk-5.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdk-5.7.3/PKG-INFO` & `mdk-5.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: mdk
-Version: 5.7.3
+Version: 5.8.0
 Summary: a docker-compose helper
 Home-page: https://matician.com/
 Author: Michael Darr
 Author-email: mdarr@matician.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -40,9 +39,7 @@
 
 ## FAQ
 
 ### How do I add custom configuration to containers created by `mdk`?
 `mdk` automatically loads additional options from two files:
 * `ext.mdk.json` located in the same directory as `mdk.json`
 * `~/.config/mdk/mdk.json`
-
-
```

### Comparing `mdk-5.7.3/README.md` & `mdk-5.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mdk-5.7.3/mdk/main.py` & `mdk-5.8.0/mdk/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,31 +9,41 @@
         def callback(ctx, param, value):
             backend.no_gpu = value
         return click.option(
             '--nogpu', '--no-gpu',
             default=False, is_flag=True, expose_value=False,
             callback=callback)(f)
 
+    def nvidia_option(f):
+        def callback(ctx, param, value):
+            backend.nvidia = value
+        return click.option(
+            '--nvidia',
+            default=False, is_flag=True, expose_value=False,
+            callback=callback)(f)
+
     @click.group()
     @click.version_option(version=VERSION)
     def cli():
         pass
 
     @cli.command(name="bash")
     @nogpu_option
+    @nvidia_option
     def mdk_bash():
         backend.start(implicit=True)
         backend.cmd('exec', '-it', '--env=TERM', '@CONTAINER@', 'bash', '-l')
 
     @cli.command(name="down")
     def mdk_down():
         backend.delete()
 
     @cli.command(name="exec", context_settings=dict(allow_interspersed_args=False))
     @nogpu_option
+    @nvidia_option
     @click.option("--interactive/--non-interactive", default=True, is_flag=True)
     @click.option("--tty/--no-tty", default=True, is_flag=True)
     @click.argument("command", nargs=-1, type=click.UNPROCESSED)
     def mdk_exec(command, interactive, tty):
         args = (
             (['--interactive'] if interactive else []) +
             (['--tty', '--env=TERM'] if tty else [])
@@ -86,14 +96,15 @@
 
     @cli.command(name="rm")
     def mdk_rm():
         backend.delete()
 
     @cli.command(name="sh")
     @nogpu_option
+    @nvidia_option
     def mdk_sh():
         backend.start(implicit=True)
         backend.cmd('exec', '-it', '--env=TERM', '@CONTAINER@', 'sh')
 
     @cli.command(name="start")
     def mdk_start():
         backend.start()
@@ -108,17 +119,19 @@
 
     @cli.command(name="unpause")
     def mdk_unpause():
         backend.cmd('unpause', '@CONTAINER@', quiet=True)
 
     @cli.command(name="up")
     @nogpu_option
+    @nvidia_option
     def mdk_up():
         backend.start(ensure_up_to_date=True)
 
     @cli.command(name="zsh")
     @nogpu_option
+    @nvidia_option
     def mdk_zsh():
         backend.start(implicit=True)
         backend.cmd('exec', '-it', '--env=TERM', '@CONTAINER@', 'zsh')
 
     cli(*args, **kwargs)
```

### Comparing `mdk-5.7.3/mdk/utils.py` & `mdk-5.8.0/mdk/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         self.opts_hash = info['Config']['Labels'].get(OPTS_HASH_LABEL_KEY, '')
 
 
 class MdkBackend:
 
     # settable publicly
     no_gpu = False
+    nvidia = False
 
     def __init__(self):
         self.conf_version = ()
         self.conf_root = None
         self.conf_paths = []
         self.conf_data = []
         self._inspect = None
@@ -270,14 +271,19 @@
         # hacky way to allow overriding --gpus
         if self.no_gpu:
             opt_builder = [x for x in opt_builder if not x.startswith('--gpus=')]
             while '--gpus' in opt_builder:
                 gpu_idx = opt_builder.index('--gpus')
                 del opt_builder[gpu_idx:gpu_idx+2]
 
+        if self.nvidia:
+            opt_builder.extend(
+                ["-e", "NVIDIA_DRIVER_CAPABILITIES=compute,utility,graphics"]
+            )
+
         # old images required --tty to start and run properly
         if self.conf_version < (5, 0):
             opt_builder += ['--tty']
 
         # mount git to not having to explain yourself on every commit. Note that this is not the right
         # location but later when we start the container, we will symlink ~/.gitconfig to /.gitconfig
         gitconfig_path = os.path.expanduser("~/.gitconfig")
@@ -318,15 +324,16 @@
         line('Status', self.inspect.status)
         if self.inspect.created:
             line('Image', self.inspect.image)
             line('ID', self.inspect.id)
             line('Command', self.inspect.command)
 
     def cmd(self, *args: str, quiet=False) -> None:
-        cmd = ['docker'] + [(self.container_name() if a == '@CONTAINER@' else a) for a in args]
+        docker = 'nvidia-docker' if self.nvidia else 'docker'
+        cmd = [docker] + [(self.container_name() if a == '@CONTAINER@' else a) for a in args]
         Log.cmd(cmd)
         code = subprocess.run(cmd, stdout=subprocess.PIPE if quiet else None).returncode
         if code != 0:
             Log.error(f'Command failed with exit code {code}!')
             sys.exit(code)
 
     def create(self, implicit=False, nogpu=False) -> None:
```

### Comparing `mdk-5.7.3/mdk.egg-info/PKG-INFO` & `mdk-5.8.0/mdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: mdk
-Version: 5.7.3
+Version: 5.8.0
 Summary: a docker-compose helper
 Home-page: https://matician.com/
 Author: Michael Darr
 Author-email: mdarr@matician.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -40,9 +39,7 @@
 
 ## FAQ
 
 ### How do I add custom configuration to containers created by `mdk`?
 `mdk` automatically loads additional options from two files:
 * `ext.mdk.json` located in the same directory as `mdk.json`
 * `~/.config/mdk/mdk.json`
-
-
```

### Comparing `mdk-5.7.3/setup.py` & `mdk-5.8.0/setup.py`

 * *Files identical despite different names*

