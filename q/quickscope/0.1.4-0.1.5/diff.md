# Comparing `tmp/quickscope-0.1.4.tar.gz` & `tmp/quickscope-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickscope-0.1.4.tar", last modified: Sat Jul 22 17:57:06 2023, max compression
+gzip compressed data, was "quickscope-0.1.5.tar", last modified: Thu Aug  3 03:42:41 2023, max compression
```

## Comparing `quickscope-0.1.4.tar` & `quickscope-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-22 17:57:06.292819 quickscope-0.1.4/
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     1714 2023-07-22 17:57:06.292819 quickscope-0.1.4/PKG-INFO
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     1470 2022-08-11 18:50:20.000000 quickscope-0.1.4/README.md
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       98 2022-07-28 05:50:42.000000 quickscope-0.1.4/pyproject.toml
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-22 17:57:06.292819 quickscope-0.1.4/quickscope/
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       62 2023-07-22 17:41:56.000000 quickscope-0.1.4/quickscope/__init__.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       34 2022-08-11 18:04:52.000000 quickscope-0.1.4/quickscope/__main__.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     2576 2023-07-22 16:41:07.000000 quickscope-0.1.4/quickscope/common.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)    19251 2023-07-22 17:10:28.000000 quickscope-0.1.4/quickscope/shooter.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)    12729 2022-08-11 00:03:27.000000 quickscope-0.1.4/quickscope/statuspage.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)    11434 2022-08-11 18:57:26.000000 quickscope-0.1.4/quickscope/tracker.py
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-22 17:57:06.292819 quickscope-0.1.4/quickscope.egg-info/
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     1714 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/PKG-INFO
--rw-rw-r--   0 audrey    (1000) audrey    (1000)      376 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/SOURCES.txt
--rw-rw-r--   0 audrey    (1000) audrey    (1000)        1 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/dependency_links.txt
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       55 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/entry_points.txt
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       30 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/requires.txt
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       11 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/top_level.txt
--rw-rw-r--   0 audrey    (1000) audrey    (1000)      526 2023-07-22 17:57:06.292819 quickscope-0.1.4/setup.cfg
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-08-03 03:42:41.689743 quickscope-0.1.5/
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     2187 2023-08-03 03:42:41.689743 quickscope-0.1.5/PKG-INFO
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     1943 2023-07-29 13:15:42.000000 quickscope-0.1.5/README.md
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       98 2023-07-26 22:56:35.000000 quickscope-0.1.5/pyproject.toml
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-08-03 03:42:41.689743 quickscope-0.1.5/quickscope/
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       62 2023-08-03 03:42:26.000000 quickscope-0.1.5/quickscope/__init__.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       34 2023-07-26 22:56:35.000000 quickscope-0.1.5/quickscope/__main__.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     3176 2023-08-02 23:16:16.000000 quickscope-0.1.5/quickscope/common.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)    27095 2023-08-03 02:47:47.000000 quickscope-0.1.5/quickscope/shooter.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)    13465 2023-07-27 21:05:41.000000 quickscope-0.1.5/quickscope/statuspage.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)    15970 2023-08-03 00:44:21.000000 quickscope-0.1.5/quickscope/tracker.py
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-08-03 03:42:41.689743 quickscope-0.1.5/quickscope.egg-info/
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     2187 2023-08-03 03:42:41.000000 quickscope-0.1.5/quickscope.egg-info/PKG-INFO
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)      451 2023-08-03 03:42:41.000000 quickscope-0.1.5/quickscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)        1 2023-08-03 03:42:41.000000 quickscope-0.1.5/quickscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       55 2023-08-03 03:42:41.000000 quickscope-0.1.5/quickscope.egg-info/entry_points.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       45 2023-08-03 03:42:41.000000 quickscope-0.1.5/quickscope.egg-info/requires.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       17 2023-08-03 03:42:41.000000 quickscope-0.1.5/quickscope.egg-info/top_level.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)      544 2023-08-03 03:42:41.689743 quickscope-0.1.5/setup.cfg
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-08-03 03:42:41.689743 quickscope-0.1.5/tests/
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)        0 2023-07-26 22:56:35.000000 quickscope-0.1.5/tests/__init__.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)      151 2023-07-26 22:56:35.000000 quickscope-0.1.5/tests/script_basic.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     3091 2023-07-26 22:56:35.000000 quickscope-0.1.5/tests/test.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)      492 2023-07-29 13:51:56.000000 quickscope-0.1.5/tests/test_ignore.py
```

### Comparing `quickscope-0.1.4/PKG-INFO` & `quickscope-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: quickscope
-Version: 0.1.4
+Version: 0.1.5
 Summary: A lightweight and scalable A/D CTF exploit shooter
 Home-page: https://github.com/shellphish/quickscope
 License: zlib
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Quickscope
 
 Quickscope is a lightweight exploit thrower for attack-defense CTFs.
 This entails being able to communicate with a game interface (the *tracker*) and being able to launch exploits (the *shooter*).
 
 `pip install quickscope`
 
+## How do I write an exploit?
+
+Write an ordinary script that takes its input as the environment variables `$HOST` and `$FLAG_ID`.
+You should hardcode the port used for the service, unless it is a very special variable service, in which case you should use `$PORT`.
+`chmod +x` the script and make sure it has a shebang.
+You should put the text `x-service-name: servicename` in your script somewhere so that the shooter knows to shoot it against the service `servicename`.
+
 ## How do I launch an exploit?
 
 `quickscope --everyone --script my_exploit.py`
 
 Your exploit must contain the text `x-service-name: <myservice>`, where `<myservice>` is replaced with the name of the service to fire at.
 
 ## How do I launch all my exploits forever?
@@ -37,13 +44,13 @@
 class MyTracker(Tracker):
     ...
 
 if __name__ == '__main__':
     MyTracker.main()
 ```
 
-You should implement the values marked as not implemented in tracker.py - this means `FLAG_REGEX`, `get_status`, submit_flags`, and `instrument_targets`.
+You should implement the values marked as not implemented in tracker.py - this means `FLAG_REGEX`, `get_status`, `submit_flags`, and `instrument_targets`.
 See [fake/stub_tracker.py](fake/stub_tracker.py) for an example implementation!
 
 You can then directly run your script and it will start tracking the game.
 
 If you're running the tracker in a non-hardcoded location, you will need to specify the `--server` argument to the shooter.
```

### Comparing `quickscope-0.1.4/README.md` & `quickscope-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Quickscope
 
 Quickscope is a lightweight exploit thrower for attack-defense CTFs.
 This entails being able to communicate with a game interface (the *tracker*) and being able to launch exploits (the *shooter*).
 
 `pip install quickscope`
 
+## How do I write an exploit?
+
+Write an ordinary script that takes its input as the environment variables `$HOST` and `$FLAG_ID`.
+You should hardcode the port used for the service, unless it is a very special variable service, in which case you should use `$PORT`.
+`chmod +x` the script and make sure it has a shebang.
+You should put the text `x-service-name: servicename` in your script somewhere so that the shooter knows to shoot it against the service `servicename`.
+
 ## How do I launch an exploit?
 
 `quickscope --everyone --script my_exploit.py`
 
 Your exploit must contain the text `x-service-name: <myservice>`, where `<myservice>` is replaced with the name of the service to fire at.
 
 ## How do I launch all my exploits forever?
@@ -28,13 +35,13 @@
 class MyTracker(Tracker):
     ...
 
 if __name__ == '__main__':
     MyTracker.main()
 ```
 
-You should implement the values marked as not implemented in tracker.py - this means `FLAG_REGEX`, `get_status`, submit_flags`, and `instrument_targets`.
+You should implement the values marked as not implemented in tracker.py - this means `FLAG_REGEX`, `get_status`, `submit_flags`, and `instrument_targets`.
 See [fake/stub_tracker.py](fake/stub_tracker.py) for an example implementation!
 
 You can then directly run your script and it will start tracking the game.
 
 If you're running the tracker in a non-hardcoded location, you will need to specify the `--server` argument to the shooter.
```

### Comparing `quickscope-0.1.4/quickscope/common.py` & `quickscope-0.1.5/quickscope/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Dict, Optional
 import enum
 from dataclasses import dataclass, field
 from dataclasses_json import config, DataClassJsonMixin
 from collections import defaultdict
 import logging
+from datetime import datetime, timedelta
 
 PORT = 3356
 
 @dataclass(frozen=True)
 class Team(DataClassJsonMixin):
     name: str
     hostname: str
@@ -17,28 +18,48 @@
     name: str
     port: int
 
 @dataclass(frozen=True)
 class Target(DataClassJsonMixin):
     team: Team
     service: Service
-    flag_id: str
+    flag_id: Optional[str] = None
     tick: Optional[int] = None
 
-    def same_process(self, other: 'Target'):
+    def same_process(self, other: 'Target') -> bool:
         return self.team == other.team and self.service == other.service
 
 class SubmissionResult(enum.Enum):
     OK = 'OK'
     INVALID = 'INVALID'
     UNKNOWN = 'UNKNOWN'
     TOO_OLD = 'TOO_OLD'
     SELF = 'SELF'
     ALREADY_SUBMITTED = 'ALREADY_SUBMITTED'
 
+class ScriptResult(enum.Enum):
+    SUCCESS = "SUCCESS"
+    FAILURE = "FAILURE"
+    TIMEOUT = "TIMEOUT"
+    #ONGOING = "ONGOING"
+
+@dataclass(frozen=True)
+class ScriptMetrics(DataClassJsonMixin):
+    script: str
+    script_hash: str
+    corpus_hash: Optional[str]
+    host: str
+    target: Target
+    start_time: datetime
+    duration: timedelta = field(metadata=config(encoder=lambda t: t.total_seconds(), decoder=lambda f: timedelta(seconds=f)))
+    status: ScriptResult
+    exit_code: int
+    flags_seen: int
+    flags: str
+
 @dataclass(frozen=True)
 class Submission(DataClassJsonMixin):
     flag: bytes = field(metadata=config(encoder=lambda b: b.decode('latin-1'), decoder=lambda s: s.encode('latin-1')))
     target: Target
     script: str
 
 @dataclass
@@ -77,15 +98,15 @@
         decoder=lambda l: {Target.from_dict(e['target']): TargetStatus.from_dict(e['status']) for e in l},
     ))
     script_info: Dict[str, ScriptStatus]  # keyed on hash
     tick_timeout: int
     retry_timeout: int
     error_log: str
 
-def setup_logging():
+def setup_logging() -> None:
     """installs logging configuration. run this before any other code"""
     root = logging.getLogger()
     root.setLevel(logging.INFO)
     logging.getLogger('quickscope').setLevel('DEBUG')
     ch = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
     fm = logging.Formatter(
```

### Comparing `quickscope-0.1.4/quickscope/shooter.py` & `quickscope-0.1.5/quickscope/tracker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,561 +1,424 @@
-from typing import List, Optional, Tuple, Union, Set, Dict
-import subprocess
-import pathlib
-import datetime
-import select
+from typing import Optional, List, Dict, Set, Any
+from collections import defaultdict
+import random
+import concurrent.futures
+import threading
+import nclib
+import io
 import time
+import pickle
 import os
-import sys
 import argparse
-import re
-import hashlib
-import threading
-import psutil
-from dataclasses import dataclass
-import queue
-import resource
 import logging
+import queue
+import sys
 import signal
+import IPython
 
-import nclib
-
-from .common import PORT, Target, Submission, Team, Service, setup_logging
-from .statuspage import statuspage
+from .common import *
 
 
 logger = logging.getLogger(__name__)
 
-SERVICE_NAME_RE = re.compile(br'x-service-name: ([-\w_=+,./?]+)')
-
-parser = argparse.ArgumentParser('quickscope')
-parser.add_argument('--corpus', help='A directory of exploits to fire')
-parser.add_argument('--script', help='A single script to fire')
-parser.add_argument('--server', help='The shooter tracker to connect to', default='172.23.0.5:%d' % PORT)
-parser.add_argument('--procs', help='The level of parallelism to use', type=int)
-parser.add_argument('--adaptive-procs', help='Measure system load to determine level of parallelism',
-                    action='store_true')
-parser.add_argument('--host', help='The single host to shoot at')
-parser.add_argument('--port', help='The single port to shoot at', type=int)
-parser.add_argument('--flag-id', help='The single flag id to shoot at')
-parser.add_argument('--everyone', help='Fire at all live targets and quit', action='store_true')
-parser.add_argument('--forever', help='Fire at all live targets until the end of time', action='store_true')
-parser.add_argument('--batch', help='Tunes the number of targets which are claimed at once', type=int, default=1)
-parser.add_argument('--logdir', help='Directory to store logs in')
-parser.add_argument('--no-stdout', help='Disable printing exploit logs to stdout', action='store_true')
-parser.add_argument('--timeout', help='Timeout (seconds) for each exploit run', type=int)
-parser.add_argument('--mem-limit', help='Memory limit to impose on exploit scripts (GB)', type=float, default=2)
-parser.add_argument('--status-html', help='Dump status to file as html and exit')
-
-class NotAnExploit(ValueError):
-    pass
-
-@dataclass
-class Single:
-    host: str
-    port: int
-    flag_id: str
-
-@dataclass
-class Everyone:
-    pass
-
-@dataclass
-class Forever:
-    pass
-
-TargetMode = Union[Single, Everyone, Forever]
-
-def parse_target_mode(args) -> TargetMode:
-    results: List[TargetMode] = []
-    if args.forever:
-        results.append(Forever())
-    if args.everyone:
-        results.append(Everyone())
-    if args.flag_id is not None or args.host is not None or args.port is not None:
-        if args.flag_id is None or args.host is None or args.port is None:
-            sys.stderr.write("Must provide all of --host/--port/--flag-id or none at all\n")
-            sys.stderr.flush()
-            sys.exit(1)
-        results.append(Single(host=args.host, port=args.port, flag_id=args.flag_id))
-
-    if len(results) != 1:
-        sys.stderr.write("Must provide exactly one of --everyone, --forever, or --host/--port/--flag-id\n")
-        sys.stderr.flush()
-        sys.exit(1)
-
-    return results[0]
-
-def get_flag_regex(server):
-    sock = nclib.Netcat(server)
-    sock.sendln(b'getregex')
-    return re.compile(sock.readln().strip())
-
-class ScriptManager:
-    def __init__(self, script: str, server: str, batch: int, target_mode: TargetMode, toplevel=False):
-        self.server = server
-        self.script_name = script
-        self.toplevel = toplevel
-        self.service_name, self.script_hash = get_script_service_name_and_hash(script)
-        if self.script_hash is None:
-            raise NotAnExploit("Please put `x-service-name: service name` (or x-shooter-ignore) somewhere in " + script)
-        if self.service_name is None:
-            raise NotAnExploit()
-        if not os.access(self.script_name, os.X_OK):
-            if not self.script_name.endswith('.py'):
-                raise NotAnExploit(script + " is not executable - how do I run it?")
-
-        self.batch = batch
-        self.target_mode = target_mode
-        self.eof = False
-        self.buffer: List[Target] = []
-
-    def _buffer_targets(self):
-        if self.eof:
-            return
-
-        if isinstance(self.target_mode, Forever):
-            sock = nclib.Netcat(self.server, raise_timeout=True)
-            sock.sendln(b'gettargets')
-            sock.sendln(self.script_hash)
-            sock.sendln(self.script_name)
-            sock.sendln(self.service_name)
-            sock.sendln(str(self.batch).encode())
+class ArgsNamespace(argparse.Namespace):
+    database: Optional[str]
+    flag_log: Optional[str]
+    shell: bool
+
+class Tracker:
+    # HERE'S WHAT YOU IMPLEMENT
+    FLAG_REGEX: bytes = NotImplemented
+
+    def get_status(self) -> GameStatus:
+        raise NotImplementedError
+
+    def submit_flags(self, flags: List[Submission]) -> List[SubmissionLog]:
+        raise NotImplementedError
+
+    def instrument_targets(self, targets: List[Target]) -> List[Target]:
+        """
+        This is called just before shooting at the given target list - each target in the list will be shot at once.
+
+        This gives the tracker the ability to record that shooting at a target is occurring and to modify the target
+        list, for example, to remove targets with rate-limiting imposed.
+        """
+        raise NotImplementedError
+
+    TICK_TIMEOUT = 3
+    RETRY_TIMEOUT = 3
+    BIND_TO = '0.0.0.0'
+    WORKER_THREADS = 8
+
+    # DON'T TOUCH THIS
+
+    @classmethod
+    def arg_parser(cls) -> argparse.ArgumentParser:
+        parser = argparse.ArgumentParser()
+        parser.add_argument('--database', help='Use this file for state persistence')
+        parser.add_argument('--flag-log', help='Use this file to log all seen flags')
+        parser.add_argument('--shell', help='Drop into an interactive shell instead of running the tracker', action='store_true')
+        return parser
+
+    @classmethod
+    def main(cls) -> None:
+        args = cls.arg_parser().parse_args(namespace=ArgsNamespace())
+
+        setup_logging()
+
+        if args.database is not None and os.path.exists(args.database):
+            with open(args.database, 'rb') as fp:
+                inst = pickle.load(fp)
+        else:
+            inst = cls()
 
+        if args.shell:
+            IPython.start_ipython(argv=[], user_ns=locals() | globals())  # type: ignore
+        else:
             try:
-                lines = sock.recvall(timeout=10).splitlines()
-            except nclib.NetcatTimeout:
-                logger.warning("Server did not respond with target list")
-                self.eof = True
-                return
-
-            self.buffer.extend(Target.from_json(line.decode()) for line in lines)
-            if not self.buffer:
-                self.eof = True
-        elif isinstance(self.target_mode, Everyone):
-            sock = nclib.Netcat(self.server, raise_timeout=True)
-            sock.sendln(b'gettargetsdumb')
-            sock.sendln(self.service_name)
+                inst.boot()
+                inst.run(args)
+            except KeyboardInterrupt:
+                pass
+            finally:
+                if args.database is not None:
+                    with open(args.database, 'wb') as fp:
+                        pickle.dump(inst, fp)
+                    print(f'Saved database to {args.database}')
+
+    def __init__(self) -> None:
+        self.lock: threading.Lock = threading.Lock()
+        self.tick: int = -1
+        self.targets: Dict[Target, TargetStatus] = {}
+        self.script_info: Dict[str, ScriptStatus] = {}  # keyed on hash
+        self.script_queues: Dict[str, List[Target]] = defaultdict(list)
+        self.submit_buffer: List[Submission] = []
+        self.submit_buffer_lock: threading.Lock = threading.Lock()
+        self.flag_log: Optional[io.IOBase] = None
+        self.script_metrics_queue: queue.Queue[ScriptMetrics] = queue.Queue(maxsize=300)
+        self.script_metrics_subscribers: Set[nclib.Netcat] = set()
+
+        self.submit_thread: threading.Thread = threading.Thread(target=self._submit_thread, daemon=True)
+        self.metrics_thread: threading.Thread = threading.Thread(target=self._metrics_thread, daemon=True)
+        self.scraper_thread: threading.Thread = threading.Thread(target=self._scraper_thread, daemon=True)
+
+        root = logging.getLogger()
+        buf = io.StringIO()
+        sh = logging.StreamHandler(buf)
+        fm = logging.Formatter(
+            "%(asctime)s - %(name)-25s - %(funcName)-10s - %(levelname)-5s - %(message)s")
+        sh.setFormatter(fm)
+        sh.setLevel('WARNING')
+        root.addHandler(sh)
+
+        self.logging_memory: io.StringIO = buf
+
+        assert b'\n' not in self.FLAG_REGEX
+
+    def boot(self) -> None:
+        logger.info("Tracker starting on %s:%s", self.BIND_TO, PORT)
+        self.submit_thread.start()
+        self.metrics_thread.start()
+        self.scraper_thread.start()
 
-            try:
-                lines = sock.recvall(timeout=10).splitlines()
-            except nclib.NetcatTimeout:
-                logger.warning("Server did not respond with target list")
-                self.eof = True
-                return
-
-            self.buffer.extend(Target.from_json(line.decode()) for line in lines)
-            self.eof = True
-        elif isinstance(self.target_mode, Single):
-            self.buffer.append(Target(
-                team=Team(name=self.target_mode.host, hostname=self.target_mode.host),
-                service=Service(name=str(self.target_mode.port), port=self.target_mode.port),
-                flag_id=self.target_mode.flag_id,
-            ))
-            self.eof = True
+        def bye(*args: Any) -> None:
+            sys.exit()
 
-    def __iter__(self):
-        return self
+        signal.signal(signal.SIGTERM, bye)
 
-    def __next__(self):
-        while True:
-            if not self.buffer:
-                try:
-                    self._buffer_targets()
-                except nclib.NetcatError:
-                    logger.exception('Failed to retrieve targets')
-            if not self.buffer:
-                if isinstance(self.target_mode, Forever) and self.toplevel:
-                    self.eof = False
-                    time.sleep(4)
-                    continue
-                raise StopIteration()
-            return self.script_name, self.buffer.pop()
+    def __getstate__(self) -> Dict[str, Any]:
+        return {
+            '__version__': 1,
+            'tick': self.tick,
+            'targets': self.targets,
+            'script_info': self.script_info,
+            'script_queues': self.script_queues,
+            'submit_buffer': self.submit_buffer,
+        }
+
+    def __setstate__(self, state: Dict[str, Any]) -> None:
+        version = state.pop('__version__')
+        if version == 1:
+            self.__init__() # type: ignore
+            self.tick = state['tick']
+            self.targets = state['targets']
+            self.script_info = state['script_info']
+            self.script_queues = state['script_queues']
+            self.submit_buffer = state['submit_buffer']
+        else:
+            raise NotImplementedError("Unsupported database")
 
-class CorpusManager:
-    def __init__(self, corpus, server, batch, target_mode):
-        if isinstance(target_mode, Single):
-            sys.stderr.write("Error: cannot specify --corpus and --host/--port/--flag-id\n")
-            sys.stderr.flush()
-            sys.exit(1)
-
-        self.corpus = corpus
-        self.server = server
-        self.batch = batch
-        self.target_mode = target_mode
-
-        self.children = []
-        self.eof = False
-        self._collect()
+    def run(self, args: ArgsNamespace) -> None:
+        server = nclib.server.TCPServer((self.BIND_TO, PORT))
+        if args.flag_log is not None:
+            self.flag_log = open(args.flag_log, 'ab')
+        try:
+            with concurrent.futures.ThreadPoolExecutor(self.WORKER_THREADS) as executor:
+                for client in server:
+                    executor.submit(self.handle, client)
+        finally:
+            if self.flag_log is not None:
+                self.flag_log.close()
+                self.flag_log = None
 
-    def _collect(self):
-        if self.eof:
+    def handle(self, sock: nclib.Netcat) -> None:
+        line = b''
+        try:
+            line = sock.readln(max_size=100, timeout=1).strip()
+            if line == b'submit':
+                self.serve_submit(sock)
+            elif line == b'getregex':
+                self.serve_getregex(sock)
+            elif line == b'gettargets':
+                self.serve_gettargets(sock)
+            elif line == b'gettargetsdumb':
+                self.serve_gettargetsdumb(sock)
+            elif line == b'getstatus':
+                self.serve_getstatus(sock)
+            elif line == b'pubmetrics':
+                self.serve_pubmetrics(sock)
+            elif line == b'submetrics':
+                self.script_metrics_subscribers.add(sock)
+            else:
+                raise Exception("not a command", line)
+        except Exception:
+            logger.exception("Exception in handle()")
+        finally:
+            if line != b'submetrics':
+                sock.close()
+
+    def serve_pubmetrics(self, sock: nclib.Netcat) -> None:
+        lines = sock.recvall(timeout=1)
+        if not lines:
             return
-        for root, dirs, files in os.walk(self.corpus):
-            for stem in files:
-                filename = os.path.join(root, stem)
-                try:
-                    child = ScriptManager(filename, self.server, self.batch, self.target_mode)
-                except NotAnExploit as e:
-                    if e.args:
-                        logger.warning("%s", e.args[0])
-                else:
-                    self.children.append(child)
-        self.eof = True
-
-    def __iter__(self):
-        return self
+        for line in lines.splitlines():
+            try:
+                metric = ScriptMetrics.from_json(line.decode())
+                self.script_metrics_queue.put(metric)
+            except Exception:
+                logger.exception("Exception during metrics parsing")
 
-    def __next__(self):
+    def _metrics_thread(self) -> None:
         while True:
-            if not self.children:
-                self._collect()
+            metric = self.script_metrics_queue.get()
             try:
-                child = self.children.pop(0)
-            except IndexError:
-                if isinstance(self.target_mode, Forever):
-                    self.eof = False
-                    time.sleep(4)
-                    continue
-                else:
-                    raise StopIteration()
-
+                for sock in list(self.script_metrics_subscribers):
+                    try:
+                        sock.sendline(metric.to_json().encode())
+                    except (nclib.NetcatError, OSError):
+                        self.script_metrics_subscribers.remove(sock)
+            except Exception:
+                logger.exception("Exception during metrics broadcast")
+                time.sleep(10)
+
+    def serve_submit(self, sock: nclib.Netcat) -> None:
+        lines = sock.recvall(timeout=1)
+        if not lines:
+            return
+        submissions = []
+        for line in lines.splitlines():
             try:
-                result = next(child)
-            except StopIteration:
-                continue
-
-            self.children.append(child)
-            return result
+                submission = Submission.from_json(line.decode())
+                submissions.append(submission)
+                if self.flag_log is not None:
+                    self.flag_log.write(submission.flag + b'\n')
 
-class SynchronousPool:
-    def apply(self, iterator, *args, **kwargs):
-        for script, target in iterator:
-            shoot(script, target, *args, **kwargs)
-
-class AsyncPool:
-    def __init__(self, procs: int):
-        self.queue: "queue.Queue[Tuple[str, Target]]" = queue.Queue(maxsize=1)
-        self.threads = [threading.Thread(target=self.worker, daemon=True) for _ in range(procs)]
-        self.args = None
-        self.kwargs = None
-        for thread in self.threads:
-            thread.start()
-
-    def apply(self, iterator, *args, **kwargs):
-        self.args = args
-        self.kwargs = kwargs
-        for script, target in iterator:
-            self.queue.put((script, target), block=True)
-        self.queue.join()
-
-    def worker(self):
-        while True:
-            script, target = self.queue.get(block=True)
-            try:
-                shoot(script, target, *self.args, **self.kwargs)
-            except:
-                logger.exception("Failed to shoot")
-            finally:
-                self.queue.task_done()
+            except Exception:
+                logger.exception("Exception during submit parsing")
 
-class AdaptivePool:
-    # warning: instances of this class will never be garbage collected
+        if self.flag_log is not None:
+            self.flag_log.flush()
 
-    def __init__(self):
-        self.cpu_utilization = 0.0
-        self.mem_utilization = 0.0
-        self.watcher_thread = threading.Thread(target=self.load_watcher, daemon=True)
-        self.watcher_thread.start()
-        self.worker_threads: List[threading.Thread] = []
-
-        self.args = None
-        self.kwargs = None
-        self.queue = queue.Queue(maxsize=1)
-        self.lock = threading.Lock()
-        self.live_tasks = 0
-        self.target_threads = 1
+        try:
+            results = self.submit_flags(submissions)
+        except Exception:
+            logger.exception("Exception during submit")
+            results = []
+        self.process_successful_submissions(submissions, results, sock)
 
-    def load_watcher(self):
+    def _submit_thread(self) -> None:
         while True:
-            self.cpu_utilization = psutil.cpu_percent(1) / 100.0
-            self.mem_utilization = psutil.virtual_memory().percent / 100.0
-
-            if self.live_tasks == self.target_threads and self.cpu_utilization < 0.9 and self.mem_utilization < 0.75:
-                self.target_threads += 1
-                logger.info("Increasing target threads to %s", self.target_threads)
-            elif self.cpu_utilization > 0.99 or self.mem_utilization > 0.95 and self.target_threads > 1:
-                self.target_threads -= 1
-                logger.info("Decreasing target threads to %s", self.target_threads)
-
-            while self.worker_threads and not self.worker_threads[-1].is_alive():
-                self.worker_threads[-1].join()
-                self.worker_threads.pop(-1)
-
-            while len(self.worker_threads) < self.target_threads:
-                self.worker_threads.append(
-                    threading.Thread(target=self.worker, args=(len(self.worker_threads),), daemon=True)
+            time.sleep(10)
+            next_batch = None
+            with self.submit_buffer_lock:
+                if len(self.submit_buffer) > 0:
+                    next_batch = self.submit_buffer
+                    self.submit_buffer = []
+            if next_batch is not None:
+                try:
+                    results = self.submit_flags(next_batch)
+                except Exception:
+                    logger.exception("Exception during submit retry")
+                    results = []
+                self.process_successful_submissions(next_batch, results, None)
+
+    def process_successful_submissions(
+            self,
+            submissions: List[Submission],
+            results: List[SubmissionLog],
+            sock: Optional[nclib.Netcat]=None
+    ) -> None:
+        submissions_set = set(submissions)
+        for result in results:
+            try:
+                submissions_set.remove(result.submission)
+            except KeyError:
+                pass
+            if result.result == SubmissionResult.SELF:
+                self.untarget_host_port(result.submission.target)
+            elif result.result == SubmissionResult.OK:
+                logger.info(
+                    "Got points on %s:%s",
+                    result.submission.target.team.name,
+                    result.submission.target.service.name
                 )
-                self.worker_threads[-1].start()
+                if sock is not None:
+                    try:
+                        sock.sendline(result.submission.flag)
+                    except BrokenPipeError:
+                        pass
+                self.untarget_target(result.submission.target)
+            elif result.result == SubmissionResult.ALREADY_SUBMITTED:
+                self.untarget_target(result.submission.target)
+            elif result.result == SubmissionResult.INVALID:
+                logger.warning("Getting bogus flags for %s", result.submission.target)
+                pass
+            elif result.result == SubmissionResult.UNKNOWN:
+                pass
+            elif result.result == SubmissionResult.TOO_OLD:
+                pass
+            else:
+                logger.error("Bad submission result: %s (is your submitter misbehaving?)",
+                             result.result)
 
-    def apply(self, iterator, *args, **kwargs):
-        self.args = args
-        self.kwargs = kwargs
-        for script, target in iterator:
-            self.queue.put((script, target), block=True)
-        self.queue.join()
+        with self.submit_buffer_lock:
+            self.submit_buffer.extend(submissions_set)
 
-    def worker(self, ident):
-        while True:
-            if ident >= self.target_threads:
-                return
-            script, target = self.queue.get(block=True)
-            with self.lock:
-                self.live_tasks += 1
-            try:
-                shoot(script, target, *self.args, **self.kwargs)
-            except:
-                logger.exception("Failed to shoot")
-            finally:
-                self.queue.task_done()
-                with self.lock:
-                    self.live_tasks -= 1
-
-def get_script_service_name_and_hash(script) -> Tuple[Optional[str], Optional[str]]:
-    with open(script, 'rb') as fp:
-        script_bytes = fp.read()
-    match = SERVICE_NAME_RE.search(script_bytes)
-    h = hashlib.md5()
-    h.update(script_bytes)
-    hd = h.hexdigest()
-    if b'x-shooter-ignore' in script_bytes:
-        return None, hd
-    if match:
-        return match.group(1).decode(), hd
-    return None, None
-
-LIVE_PROCESSES: Set[subprocess.Popen] = set()
-
-def kill_live_processes():
-    for proc in list(LIVE_PROCESSES):
-        proc.kill()
-
-def shoot(
-    script: str,
-    target: Target,
-    timeout: Optional[int],
-    logdir: Optional[str],
-    flag_regex: re.Pattern,
-    use_stdout: bool,
-    mem_limit: float,
-):
-    if timeout is None:
-        timeout = 999999999
-    deadline = time.time() + timeout
-    cmd = [os.path.join('.', os.path.basename(script))]
-    env = dict(os.environ)
-    for name in ('host', 'victim', 'enemy'):
-        env[name] = env[name.upper()] = target.team.hostname
-    for name in ('port',):
-        env[name] = env[name.upper()] = str(target.service.port)
-    for name in ('flagid', 'flag_id', 'fid', 'id'):
-        env[name] = env[name.upper()] = target.flag_id
-
-    if not os.access(script, os.X_OK):
-        if script.endswith('.py'):
-            cmd.insert(0, 'python3')
-
-    def preexec_limits():
-        size_bytes = int(mem_limit * 1024 * 1024 * 1024)
-        #resource.setrlimit(resource.RLIMIT_STACK, (size_bytes, size_bytes))
-        resource.setrlimit(resource.RLIMIT_DATA, (size_bytes, size_bytes))
-        os.setpgrp()
-
-    proc = subprocess.Popen(
-        cmd,
-        stdin=subprocess.PIPE,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.STDOUT,
-        cwd=os.path.dirname(os.path.realpath(script)),
-        preexec_fn=preexec_limits,
-        env=env,
-    )
-    assert proc.stdout is not None
-    LIVE_PROCESSES.add(proc)
-    head_buf: List[bytes] = []
-    tail_buf: List[bytes] = []
-    buf_full = False
-    BUF_SIZE = 20
-
-    hit_timeout = False
-    while True:
-        r, _, _ = select.select([proc.stdout], [], [], max(0., deadline - time.time()))
-        if not r:
-            hit_timeout = True
-            if use_stdout:
-                print('TIMEOUT')
-            break
-        line = proc.stdout.readline()
-        if not line:
-            break
-        if use_stdout:
-            sys.stdout.buffer.write(line)
-            sys.stdout.buffer.flush()
-        if len(head_buf) < BUF_SIZE:
-            head_buf.append(line)
-        else:
-            tail_buf.append(line)
-            if len(tail_buf) >= BUF_SIZE:
-                tail_buf.pop(0)
-                buf_full = True
-
-        for flag in flag_regex.finditer(line):
-            while True:
-                try:
-                    SUBMISSION_QUEUE.put(Submission(flag=flag.group(0), target=target, script=script))
-                except queue.Full:
-                    logger.warning("Submission queue is full")
-                    time.sleep(5)
-                else:
-                    break
+    def serve_getregex(self, sock: nclib.Netcat) -> None:
+        sock.sendln(self.FLAG_REGEX)
 
-    try:
-        proc.wait(deadline - time.time())
-        try:
-            os.killpg(proc.pid, signal.SIGKILL)
-        except ProcessLookupError:
-            pass
-    except subprocess.TimeoutExpired:
-        try:
-            os.killpg(proc.pid, signal.SIGKILL)
-        except ProcessLookupError:
-            pass
-        proc.wait()
-    LIVE_PROCESSES.remove(proc)
+    def serve_gettargets(self, sock: nclib.Netcat) -> None:
+        script_id = sock.readln(max_size=100, timeout=1).strip().decode()
+        script_name = sock.readln(max_size=100, timeout=1).strip().decode()
+        service_name = sock.readln(max_size=100, timeout=1).strip().decode()
+        n = int(sock.readln(max_size=100, timeout=1).strip().decode())
+        if script_id not in self.script_info:
+            with self.lock:
+                if script_id not in self.script_info:
+                    self.script_info[script_id] = ScriptStatus(
+                        filename=script_name,
+                        service_name=service_name,
+                        tick_first_seen=self.tick,
+                        tick_last_seen=self.tick,
+                    )
+        self.script_info[script_id].tick_last_seen = self.tick
+        targets = self.get_targets_for_script(script_id, service_name, n)
+        targets = self.instrument_targets(targets)
+        for target in targets:
+            sock.sendln(target.to_json().encode())
+
+    def serve_gettargetsdumb(self, sock: nclib.Netcat) -> None:
+        service_name = sock.readln(max_size=100, timeout=1).strip().decode()
+
+        targets = self.get_targets_for_tick(service_name, self.tick)
+        targets = self.instrument_targets(targets)
+        for target in targets:
+            sock.sendln(target.to_json().encode())
+
+    def serve_getstatus(self, sock: nclib.Netcat) -> None:
+        result = ShooterStatus(
+            tick=self.tick,
+            script_info=self.script_info,
+            targets=dict(self.targets),
+            tick_timeout=self.TICK_TIMEOUT,
+            retry_timeout=self.RETRY_TIMEOUT,
+            error_log=self.logging_memory.getvalue(),
+        )
+        sock.send(result.to_json().encode())
 
-    if logdir is not None:
-        log_filename = os.path.join(logdir, script + '-' + datetime.datetime.now().isoformat())
-        pathlib.Path(log_filename).parent.mkdir(parents=True, exist_ok=True)
-        with open(log_filename, 'wb') as fp:
-            fp.writelines(head_buf)
-            if buf_full:
-                fp.write(b'...\n')
-            fp.writelines(tail_buf)
-            if hit_timeout:
-                fp.write(b'TIMEOUT\n')
-
-
-SUBMISSIONS_DONE = False
-SUBMISSION_QUEUE: "queue.Queue[Submission]" = queue.Queue(maxsize=10000)
-NOTIFIED_SOCKS = []
-FLAG_MAPPING: Dict[bytes, Submission] = {}
-
-def submission_routine(server, debounce):
-    buffer = set()
-    while not SUBMISSIONS_DONE:
-        deadline = time.time() + debounce
+    def _scraper_thread(self) -> None:
         while True:
             try:
-                submission = SUBMISSION_QUEUE.get(block=True, timeout=deadline - time.time())
-            except (queue.Empty, ValueError):  # ValueError = negative timeout
-                break
-            else:
-                buffer.add(submission)
-                FLAG_MAPPING[submission.flag.strip()] = submission
+                status = self.get_status()
+            except Exception:
+                logger.exception("Error getting status")
+                time.sleep(10)
+                continue
 
-        if buffer:
-            try:
-                sock = nclib.Netcat(server)
-            except:
-                logger.exception('Could not connect to server for flag submission')
+            if status.tick == self.tick:
+                time.sleep(10)
                 continue
-            try:
-                sock.sendln(b'submit')
-                sock.send(b''.join(s.to_json().encode() + b'\n' for s in buffer))
-                sock.shutdown_wr()
-            except:
-                logger.exception('Failed to submit flags')
-            else:
-                buffer.clear()
-            NOTIFIED_SOCKS.append(sock)
+            self.ingest_status(status)
 
-def notification_routine():
-    while not SUBMISSIONS_DONE or NOTIFIED_SOCKS:
-        r, _, _ = nclib.select(NOTIFIED_SOCKS, [], [], timeout=1)
-        for sock in r:
-            line = sock.recvln()
-            if not line:
-                NOTIFIED_SOCKS.remove(sock)
-            else:
-                submission = FLAG_MAPPING.get(line.strip(), None)
-                if submission is None:
-                    logger.warning("Got points on unknown flag?")
+    def ingest_status(self, gamestatus: GameStatus) -> None:
+        with self.lock:
+            self.tick = gamestatus.tick
+
+            for target in gamestatus.targets:
+                if target in self.targets:
+                    self.targets[target].tick_last_seen = gamestatus.tick
                 else:
-                    logger.info("Got points on %s:%s", submission.target.team.name, submission.target.service.name)
+                    self.targets[target] = TargetStatus(tick_first_seen=gamestatus.tick, tick_last_seen=gamestatus.tick)
 
+            to_remove = []
+            for target, status in self.targets.items():
+                if status.tick_last_seen < gamestatus.tick - self.TICK_TIMEOUT:
+                    to_remove.append(target)
+            for target in to_remove:
+                self.targets.pop(target)
+
+    def untarget_host_port(self, bad_target: Target) -> None:
+        with self.lock:
+            for target, status in self.targets.items():
+                if target.same_process(bad_target):
+                    status.retired = True
 
-def main():
-    setup_logging()
-    ctrl_c_times = 0
-    def force_exit(*args):
-        nonlocal ctrl_c_times
-        global SUBMISSIONS_DONE
-        if ctrl_c_times == 0:
-            sys.stderr.write("CTRL-C again to force exit\n")
-            sys.stderr.flush()
-            ctrl_c_times += 1
-        else:
-            sys.stderr.write("Cancelling all tasks and exiting\n")
-            sys.stderr.flush()
-            SUBMISSIONS_DONE = True
-            sys.exit()
+    def untarget_target(self, target: Target) -> None:
+        try:
+            self.targets[target].retired = True
+        except KeyError:
+            pass
 
-    signal.signal(signal.SIGINT, force_exit)
+    def get_targets_for_script(self, script_id: str, service_name: str, n: int) -> List[Target]:
+        result = None
+        found_one = False
+        with self.lock:
+            if len(self.script_queues[script_id]) >= n:
+                result, self.script_queues[script_id] = self.script_queues[script_id][:n], self.script_queues[script_id][n:]
+                found_one = True
+
+        if result is None:
+            newstuff = []
+            for target, status in self.targets.items():
+                if target.service.name != service_name:
+                    continue
+                found_one = True
+                if status.retired:
+                    continue
+                if status.script_status[script_id].runs >= self.RETRY_TIMEOUT:
+                    continue
+                status.script_status[script_id].runs += 1
+                newstuff.append(target)
+            random.shuffle(newstuff)
 
-    args = parser.parse_args(sys.argv[1:])
-    if args.status_html:
-        statuspage(args.server, args.status_html)
-        return
-
-    target_mode = parse_target_mode(args)
-    if args.corpus is not None:
-        if args.script is not None:
-            sys.stderr.write("Error: only specify one of --corpus or --script\n")
-            sys.stderr.flush()
-            sys.exit(1)
-        mgr = CorpusManager(args.corpus, args.server, args.batch, target_mode)
-    elif args.script is not None:
-        mgr = ScriptManager(args.script, args.server, args.batch, target_mode, toplevel=True)
-    else:
-        sys.stderr.write("Error: must specify one of --corpus or --script\n")
-        sys.stderr.flush()
-        sys.exit(1)
-
-    if args.adaptive_procs:
-        pool = AdaptivePool()
-    elif args.procs:
-        pool = AsyncPool(args.procs)
-    else:
-        pool = SynchronousPool()
-
-    debounce = 5 if isinstance(target_mode, Forever) else 1
-    submission_thread = threading.Thread(target=submission_routine, args=(args.server, debounce))
-    submission_thread.start()
-    notification_thread = threading.Thread(target=notification_routine)
-    notification_thread.start()
-
-    pool.apply(
-        mgr,
-        timeout=args.timeout,
-        logdir=args.logdir,
-        flag_regex=get_flag_regex(args.server),
-        use_stdout=not args.no_stdout,
-        mem_limit=args.mem_limit,
-    )
-
-    global SUBMISSIONS_DONE
-    SUBMISSIONS_DONE = True
-    submission_thread.join()
-    notification_thread.join()
+            with self.lock:
+                self.script_queues[script_id].extend(newstuff)
+                result, self.script_queues[script_id] = self.script_queues[script_id][:n], self.script_queues[script_id][n:]
+
+        if not found_one:
+            logger.warning("Someone requested unknown service %s", repr(service_name))
+        return result
+
+    def get_targets_for_tick(self, service_name: str, tick: int) -> List[Target]:
+        result = []
+        found_one = False
+        for target, status in self.targets.items():
+            if target.service.name != service_name:
+                continue
+            found_one = True
+            if status.tick_last_seen != tick:
+                continue
+            result.append(target)
 
-if __name__ == '__main__':
-    main()
+        if not found_one:
+            logger.warning("Someone requested unknown service %s", repr(service_name))
+        return result
```

### Comparing `quickscope-0.1.4/quickscope/statuspage.py` & `quickscope-0.1.5/quickscope/statuspage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from typing import Tuple, Dict, List, Type
 import json.decoder
-from typing import Tuple, Dict, List
 import html
 from collections import defaultdict
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json
 import logging
 import math
 import nclib
+import http.server
 
 
 logger = logging.getLogger(__name__)
 
 STATUS_HTML = """<!DOCTYPE html>
 <html lang="en-US">
 <head>
@@ -162,24 +163,40 @@
 class TickReport:
     expected_shots: int = 0
     total_shots: int = 0
     flags_by_service: Dict[str, FlagsReport] = field(default_factory=lambda: defaultdict(FlagsReport))
     flags_by_team: Dict[str, FlagsReport] = field(default_factory=lambda: defaultdict(FlagsReport))
     flags_by_team_service: Dict[Tuple[str, str], FlagsReport] = field(default_factory=lambda: defaultdict(FlagsReport))
 
-def statuspage(server, outfile):
+class StatusServer(http.server.ThreadingHTTPServer):
+    def __init__(self, bind_address: Tuple[str, int], handler_class: Type["StatusHandler"], qs_server: str):
+        super().__init__(bind_address, handler_class)
+        self.qs_server: str = qs_server
+
+class StatusHandler(http.server.BaseHTTPRequestHandler):
+    server: StatusServer
+
+    def do_GET(self) -> None:
+        data = statuspage(self.server.qs_server).encode()
+        self.send_response(http.HTTPStatus.OK)
+        self.send_header("Content-type", 'text/html')
+        self.send_header("Content-Length", str(len(data)))
+        self.end_headers()
+        self.wfile.write(data)
+
+def statuspage(server: str) -> str:
     sock = nclib.Netcat(server)
     sock.sendln(b'getstatus')
     recved = sock.recvall()
     try:
         dicts = json.loads(recved.decode())
         data: ShooterStatus = ShooterStatus.from_dict(dicts)
     except json.decoder.JSONDecodeError:
-        logger.exception('JSON decode error for status: %s', recved)
-        return
+        logger.exception('JSON decode error for status: %r', recved)
+        return 'JSON decode error for status: %r' % recved
 
     sock.close()
 
     scripts_by_service: defaultdict[str, List[Tuple[str, ScriptStatus]]] = defaultdict(list)
     for script_hash, script_info in data.script_info.items():
         scripts_by_service[script_info.service_name].append((script_hash, script_info))
 
@@ -233,43 +250,42 @@
         title=f'{html.escape(team)} - {report.got_flags}/{report.total_flags}',
         chart=build_pie([max(0, report.total_flags - report.got_flags), report.got_flags], ['red', 'green']),
         tick=tick,
         service="ALL",
         role="get",
     ) for tick, tick_data in ticks.items() for team, report in tick_data.flags_by_team.items()) + '\n'
 
-    with open(outfile, 'w', encoding='utf-8') as fp:
-        fp.write(STATUS_HTML % dict(progress=ticks_html, services=services_html, teams=teams_html,
-                                    errorlog=data.error_log))
+    return STATUS_HTML % dict(progress=ticks_html, services=services_html, teams=teams_html,
+                                errorlog=data.error_log)
 
-def endpoint(pAngleInRadians, pRadius, pCentreOffsetX, pCentreOffsetY):
+def endpoint(pAngleInRadians: float, pRadius: float, pCentreOffsetX: float, pCentreOffsetY: float) -> Tuple[float, float]:
     """
     Calculate position of point on circle given an angle, a radius, and the location of the center of the circle
     Zero line points west.
     """
     lCosAngle = math.cos(pAngleInRadians)
     lSinAngle = math.sin(pAngleInRadians)
     lStartLineDestinationX =  pCentreOffsetX - (pRadius * lCosAngle)  # originally said lRadius
     lStartLineDestinationY =  pCentreOffsetY - (pRadius * lSinAngle)
 
     return (lStartLineDestinationX, lStartLineDestinationY)
 
 # https://drumcoder.co.uk/blog/2010/nov/16/python-code-generate-svg-pie-chart/
-def build_pie(slices, colors):
+def build_pie(slices: List[int], colors: List[str]) -> str:
     if sum(slices) == 0:
         slices = [1]
         colors = ['white']
 
     OFFSET_X = 75
     OFFSET_Y = 75
     RADIUS = 65
     INNER_RADIUS = 30
     DEGREES_IN_CIRCLE = 360.0
 
-    current_angle = 0
+    current_angle = 0.
     total = sum(slices)
     path_elem = ""
 
     for gradient, slice in zip(colors, slices):
         degrees = (DEGREES_IN_CIRCLE / total) * slice
 
         if degrees <= 0:
```

### Comparing `quickscope-0.1.4/quickscope.egg-info/PKG-INFO` & `quickscope-0.1.5/quickscope.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: quickscope
-Version: 0.1.4
+Version: 0.1.5
 Summary: A lightweight and scalable A/D CTF exploit shooter
 Home-page: https://github.com/shellphish/quickscope
 License: zlib
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Quickscope
 
 Quickscope is a lightweight exploit thrower for attack-defense CTFs.
 This entails being able to communicate with a game interface (the *tracker*) and being able to launch exploits (the *shooter*).
 
 `pip install quickscope`
 
+## How do I write an exploit?
+
+Write an ordinary script that takes its input as the environment variables `$HOST` and `$FLAG_ID`.
+You should hardcode the port used for the service, unless it is a very special variable service, in which case you should use `$PORT`.
+`chmod +x` the script and make sure it has a shebang.
+You should put the text `x-service-name: servicename` in your script somewhere so that the shooter knows to shoot it against the service `servicename`.
+
 ## How do I launch an exploit?
 
 `quickscope --everyone --script my_exploit.py`
 
 Your exploit must contain the text `x-service-name: <myservice>`, where `<myservice>` is replaced with the name of the service to fire at.
 
 ## How do I launch all my exploits forever?
@@ -37,13 +44,13 @@
 class MyTracker(Tracker):
     ...
 
 if __name__ == '__main__':
     MyTracker.main()
 ```
 
-You should implement the values marked as not implemented in tracker.py - this means `FLAG_REGEX`, `get_status`, submit_flags`, and `instrument_targets`.
+You should implement the values marked as not implemented in tracker.py - this means `FLAG_REGEX`, `get_status`, `submit_flags`, and `instrument_targets`.
 See [fake/stub_tracker.py](fake/stub_tracker.py) for an example implementation!
 
 You can then directly run your script and it will start tracking the game.
 
 If you're running the tracker in a non-hardcoded location, you will need to specify the `--server` argument to the shooter.
```

### Comparing `quickscope-0.1.4/setup.cfg` & `quickscope-0.1.5/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 license_files = LICENSE
 description = A lightweight and scalable A/D CTF exploit shooter
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 install_requires = 
-	nclib
+	nclib >= 1.0.3
 	psutil
 	dataclasses-json
+	ipython
 python_requires = >= 3.8
 packages = find:
 
 [options.entry_points]
 console_scripts = 
 	quickscope = quickscope.shooter:main
```

