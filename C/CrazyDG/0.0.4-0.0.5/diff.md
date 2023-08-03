# Comparing `tmp/CrazyDG-0.0.4.tar.gz` & `tmp/CrazyDG-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrazyDG-0.0.4.tar", last modified: Thu Aug  3 02:18:10 2023, max compression
+gzip compressed data, was "CrazyDG-0.0.5.tar", last modified: Thu Aug  3 10:21:59 2023, max compression
```

## Comparing `CrazyDG-0.0.4.tar` & `CrazyDG-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.810583 CrazyDG-0.0.4/
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.802767 CrazyDG-0.0.4/CrazyDG/
--rw-r--r--   0 daegeun    (501) staff       (20)      183 2023-08-03 02:12:58.000000 CrazyDG-0.0.4/CrazyDG/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.805042 CrazyDG-0.0.4/CrazyDG/control/
--rw-r--r--   0 daegeun    (501) staff       (20)     2003 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/control/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/control/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/control/integral_loop.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/control/optimus_prime.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.805554 CrazyDG-0.0.4/CrazyDG/crazy/
--rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/crazy/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/crazy/crazy.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.805788 CrazyDG-0.0.4/CrazyDG/guidance/
--rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 02:04:21.000000 CrazyDG-0.0.4/CrazyDG/guidance/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.807558 CrazyDG-0.0.4/CrazyDG/guidance/utils/
--rw-r--r--   0 daegeun    (501) staff       (20)      114 2023-08-03 02:08:21.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      948 2023-08-03 02:04:57.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/_goto.py
--rw-r--r--   0 daegeun    (501) staff       (20)      827 2023-08-03 02:05:05.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/_hover.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1102 2023-08-03 02:05:11.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/_landing.py
--rw-r--r--   0 daegeun    (501) staff       (20)      971 2023-08-03 02:05:20.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/_takeoff.py
--rw-r--r--   0 daegeun    (501) staff       (20)       86 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/smoother.py
--rw-r--r--   0 daegeun    (501) staff       (20)      971 2023-08-03 02:17:42.000000 CrazyDG-0.0.4/CrazyDG/main_example.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.809048 CrazyDG-0.0.4/CrazyDG/navigation/
--rw-r--r--   0 daegeun    (501) staff       (20)      518 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/navigation/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1658 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/navigation/imu.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2096 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/navigation/imu_setup.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/navigation/qualisys.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.809954 CrazyDG-0.0.4/CrazyDG/recorder/
--rw-r--r--   0 daegeun    (501) staff       (20)       63 2023-08-03 02:12:37.000000 CrazyDG-0.0.4/CrazyDG/recorder/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     3146 2023-08-03 02:15:01.000000 CrazyDG-0.0.4/CrazyDG/recorder/recorder.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2451 2023-08-03 02:12:37.000000 CrazyDG-0.0.4/CrazyDG/recorder/visualizer.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.803962 CrazyDG-0.0.4/CrazyDG.egg-info/
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 02:18:10.000000 CrazyDG-0.0.4/CrazyDG.egg-info/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)      867 2023-08-03 02:18:10.000000 CrazyDG-0.0.4/CrazyDG.egg-info/SOURCES.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:18:10.000000 CrazyDG-0.0.4/CrazyDG.egg-info/dependency_links.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:18:10.000000 CrazyDG-0.0.4/CrazyDG.egg-info/not-zip-safe
--rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 02:18:10.000000 CrazyDG-0.0.4/CrazyDG.egg-info/top_level.txt
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 02:18:10.810293 CrazyDG-0.0.4/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/README.md
--rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 02:18:10.810651 CrazyDG-0.0.4/setup.cfg
--rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 02:12:53.000000 CrazyDG-0.0.4/setup.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.213108 CrazyDG-0.0.5/
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.204178 CrazyDG-0.0.5/CrazyDG/
+-rw-r--r--   0 daegeun    (501) staff       (20)      215 2023-08-03 10:12:32.000000 CrazyDG-0.0.5/CrazyDG/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.206744 CrazyDG-0.0.5/CrazyDG/control/
+-rw-r--r--   0 daegeun    (501) staff       (20)     2159 2023-08-03 10:11:52.000000 CrazyDG-0.0.5/CrazyDG/control/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/control/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/control/integral_loop.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/control/optimus_prime.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.207297 CrazyDG-0.0.5/CrazyDG/crazy/
+-rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/crazy/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/crazy/crazy.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.207574 CrazyDG-0.0.5/CrazyDG/guidance/
+-rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 02:04:21.000000 CrazyDG-0.0.5/CrazyDG/guidance/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.210269 CrazyDG-0.0.5/CrazyDG/guidance/utils/
+-rw-r--r--   0 daegeun    (501) staff       (20)      114 2023-08-03 02:08:21.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      944 2023-08-03 10:00:35.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/_goto.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      804 2023-08-03 10:01:00.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/_hover.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1169 2023-08-03 10:02:43.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/_landing.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1011 2023-08-03 10:09:19.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/_landing_supporter.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      964 2023-08-03 10:03:33.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/_takeoff.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       86 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/smoother.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1018 2023-08-03 10:19:59.000000 CrazyDG-0.0.5/CrazyDG/main_example.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.211391 CrazyDG-0.0.5/CrazyDG/navigation/
+-rw-r--r--   0 daegeun    (501) staff       (20)      966 2023-08-03 10:11:41.000000 CrazyDG-0.0.5/CrazyDG/navigation/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1658 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/navigation/imu.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2096 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/navigation/imu_setup.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/navigation/qualisys.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.212459 CrazyDG-0.0.5/CrazyDG/recorder/
+-rw-r--r--   0 daegeun    (501) staff       (20)       63 2023-08-03 02:12:37.000000 CrazyDG-0.0.5/CrazyDG/recorder/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     3205 2023-08-03 10:13:00.000000 CrazyDG-0.0.5/CrazyDG/recorder/recorder.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2451 2023-08-03 02:12:37.000000 CrazyDG-0.0.5/CrazyDG/recorder/visualizer.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.205460 CrazyDG-0.0.5/CrazyDG.egg-info/
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 10:21:59.000000 CrazyDG-0.0.5/CrazyDG.egg-info/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)      912 2023-08-03 10:21:59.000000 CrazyDG-0.0.5/CrazyDG.egg-info/SOURCES.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 10:21:59.000000 CrazyDG-0.0.5/CrazyDG.egg-info/dependency_links.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 10:21:59.000000 CrazyDG-0.0.5/CrazyDG.egg-info/not-zip-safe
+-rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 10:21:59.000000 CrazyDG-0.0.5/CrazyDG.egg-info/top_level.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 10:21:59.212850 CrazyDG-0.0.5/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/README.md
+-rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 10:21:59.213174 CrazyDG-0.0.5/setup.cfg
+-rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 10:20:43.000000 CrazyDG-0.0.5/setup.py
```

### Comparing `CrazyDG-0.0.4/CrazyDG/control/__init__.py` & `CrazyDG-0.0.5/CrazyDG/control/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-from crazy import CrazyDragon
+from ..crazy import CrazyDragon
 
 from threading import Thread
 
 from .integral_loop import _dot_thrust
 from .integral_loop import _thrust_clip
 
 from .optimus_prime import _command_as_RPY
 from .optimus_prime import _command_is_not_in_there
 
-from constants import alpha
+from .constants import alpha
 
 from numpy import zeros, array
 
 from time import sleep
 
 
 
 class Controller( Thread ):
 
     def __init__( self, cf: CrazyDragon, config ):
         
-        super().__init__( self, daemon=True )
+        super().__init__()
+
+        self.daemon = True
 
         self.cf = cf
         self.dt = config['dt']
         self.n  = config['n']
 
         self.ready_for_command = False
 
+        self.acc_cmd = zeros(3)
+        self.command = zeros(4)
+        self.thrust  = array( [alpha * 9.81], dtype=int )
+
 
     def init_send_setpoint( self ):
         ## commander
         commander = self.cf.commander
         ## initialize
         commander.send_setpoint( 0, 0, 0, 0 )
         self.ready_for_command = True
@@ -54,23 +60,25 @@
 
         n  = self.n
         dt = self.dt / n
 
         att_cur = cf.att
         acc_cur = cf.acc
 
-        acc_cmd = zeros(3)
-        command = zeros(4)
-        thrust  = array( [alpha * 9.81], dtype=int )
+        acc_cmd = self.acc_cmd
+        command = self.command
+        thrust  = self.thrust
 
         while not self.ready_for_command:
             sleep( 0.1 )
 
         while self.ready_for_command:
 
+            acc_cmd[:] = cf.command
+
             _command_is_not_in_there( acc_cmd, att_cur )
 
             _command_as_RPY( acc_cmd, command )
 
             if ( acc_cmd[2] == 0 ):
                 sleep( dt )
                 return
@@ -81,11 +89,11 @@
 
                 thrust[0] = _thrust_clip( thrust[0] )
 
                 commander.send_setpoint(
                     command[0],
                     command[1],
                     command[2],
-                    command[3]
+                    thrust[0]
                 )
 
                 sleep( dt )
```

### Comparing `CrazyDG-0.0.4/CrazyDG/control/optimus_prime.py` & `CrazyDG-0.0.5/CrazyDG/control/optimus_prime.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.4/CrazyDG/guidance/utils/_goto.py` & `CrazyDG-0.0.5/CrazyDG/guidance/utils/_goto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from crazy import CrazyDragon
+from ...crazy import CrazyDragon
 
 from .smoother import smooth_command
 
 from .constants import Kp, Kd, g
 
 from numpy import array, zeros
 
@@ -34,15 +34,15 @@
     des[:] = destination
 
     cf.destination[:] = des
 
     for _ in range( n ):
 
         des_cmd[:] = smooth_command( 
-            des, cur, t, int( T/2 )
+            des, cur, t, 2.0
         )
 
         P_pos[:] = des_cmd - pos
         D_pos[:] = vel
 
         acc_cmd[:] = 0
         acc_cmd[:] += P_pos * Kp
```

### Comparing `CrazyDG-0.0.4/CrazyDG/guidance/utils/_hover.py` & `CrazyDG-0.0.5/CrazyDG/guidance/utils/_takeoff.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,42 +6,48 @@
 
 from numpy import array, zeros
 
 from time import sleep
 
 
 
-def hover( cf: CrazyDragon, T, dt=0.1 ):
+def takeoff( cf: CrazyDragon, h=1.5, T=3, dt=0.1 ):
 
     cur     = zeros(3)
     des     = zeros(3)
     des_cmd = zeros(3)
     acc_cmd = zeros(3)
     P_pos   = zeros(3)
     D_pos   = zeros(3)
     care_g  = array([0,0,g])
 
-    print( 'hover' )
+    print( 'take-off' )
 
     n = int( T / dt )
     t = 0
 
     command = cf.command
 
     cur[:] = cf.pos
     pos    = cf.pos
     vel    = cf.vel
 
-    des[:] = cur[:]
+    des[ 0 ] = cur[0]
+    des[ 1 ] = cur[1]
+    des[ 2 ] = h
 
     cf.destination[:] = des
 
     for _ in range( n ):
 
-        P_pos[:] = des - pos
+        des_cmd[:] = smooth_command( 
+            des, cur, t, 1.5
+        )
+
+        P_pos[:] = des_cmd - pos
         D_pos[:] = vel
 
         acc_cmd[:] = 0
         acc_cmd[:] += P_pos * Kp
         acc_cmd[:] -= D_pos * Kd
         acc_cmd[:] += care_g
```

### Comparing `CrazyDG-0.0.4/CrazyDG/guidance/utils/_landing.py` & `CrazyDG-0.0.5/CrazyDG/guidance/utils/_landing.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from numpy        import array, zeros
 from numpy.linalg import norm
 
 from time import sleep
 
 
 
-def landing( cf: CrazyDragon, h=0.2, T=3, dt=0.1, step=0.075 ):
+def landing( cf: CrazyDragon, option=1, h=0.2, T=3, dt=0.1, step=0.075 ):
 
     cur     = zeros(3)
     des     = zeros(3)
     des_cmd = zeros(3)
     acc_cmd = zeros(3)
     P_pos   = zeros(3)
     D_pos   = zeros(3)
@@ -28,31 +28,35 @@
 
     command = cf.command
 
     cur[:] = cf.pos
     pos    = cf.pos
     vel    = cf.vel
 
-    des[0] = cur[0]
-    des[1] = cur[1]
-    des[2] = h
+    if option:
+        des[0] = cur[0]
+        des[1] = cur[1]
+        des[2] = h
+    else:
+        des[0] = 0
+        des[1] = 0
+        des[2] = h
 
     cf.destination[:] = des
 
     for _ in range( n ):
 
         des_cmd[:] = smooth_command( 
-            des, cur, t, int( T/2 )
+            des, cur, t, 3.0
         )
 
         P_pos[:] = des_cmd - pos
         D_pos[:] = vel
 
-        if ( norm( pos - des ) ) < 0.1:
-            care_g[2] -= step
+        if ( norm( pos - des ) ) < 0.2:
             break
 
         acc_cmd[:] = 0
         acc_cmd[:] += P_pos * Kp
         acc_cmd[:] -= D_pos * Kd
         acc_cmd[:] += care_g
```

### Comparing `CrazyDG-0.0.4/CrazyDG/guidance/utils/_takeoff.py` & `CrazyDG-0.0.5/CrazyDG/guidance/utils/_hover.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,48 +6,41 @@
 
 from numpy import array, zeros
 
 from time import sleep
 
 
 
-def takeoff( cf: CrazyDragon, h=1.5, T=3, dt=0.1 ):
+def hover( cf: CrazyDragon, T, dt=0.1 ):
 
     cur     = zeros(3)
     des     = zeros(3)
-    des_cmd = zeros(3)
     acc_cmd = zeros(3)
     P_pos   = zeros(3)
     D_pos   = zeros(3)
     care_g  = array([0,0,g])
 
-    print( 'take-off' )
+    print( 'hover' )
 
     n = int( T / dt )
     t = 0
 
     command = cf.command
 
     cur[:] = cf.pos
     pos    = cf.pos
     vel    = cf.vel
 
-    des[ 0 ] = cur[0]
-    des[ 1 ] = cur[1]
-    des[ 2 ] = h
+    des[:] = cur[:]
 
     cf.destination[:] = des
 
     for _ in range( n ):
 
-        des_cmd[:] = smooth_command( 
-            des, cur, t, int( T/2 )
-        )
-
-        P_pos[:] = des_cmd - pos
+        P_pos[:] = des - pos
         D_pos[:] = vel
 
         acc_cmd[:] = 0
         acc_cmd[:] += P_pos * Kp
         acc_cmd[:] -= D_pos * Kd
         acc_cmd[:] += care_g
```

### Comparing `CrazyDG-0.0.4/CrazyDG/main_example.py` & `CrazyDG-0.0.5/CrazyDG/main_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 from control import Controller
 
 from recorder import Recorder
 
 from crazy import CrazyDragon
 
+from cflib                         import crtp
 from cflib.crazyflie.syncCrazyflie import SyncCrazyflie
 from cflib.utils                   import uri_helper
 
-from numpy import array
-
 nav_config = {
     'body_name': 'cf1'
 }
 
 ctr_config = {
     'dt': 0.1,
     'n' : 5
@@ -22,14 +21,16 @@
 
 
 
 uri = uri_helper.uri_from_env( default='radio://0/80/2M/E7E7E7E702' )
 
 
 if __name__ == "__main__":
+
+    crtp.init_drivers()
     
     _cf = CrazyDragon()
 
     with SyncCrazyflie( uri, cf=_cf ) as scf:
 
         NAV = Navigation( _cf, nav_config )
         CTR = Controller( _cf, ctr_config )
```

### Comparing `CrazyDG-0.0.4/CrazyDG/navigation/imu.py` & `CrazyDG-0.0.5/CrazyDG/navigation/imu.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.4/CrazyDG/navigation/imu_setup.py` & `CrazyDG-0.0.5/CrazyDG/navigation/imu_setup.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.4/CrazyDG/navigation/qualisys.py` & `CrazyDG-0.0.5/CrazyDG/navigation/qualisys.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.4/CrazyDG/recorder/recorder.py` & `CrazyDG-0.0.5/CrazyDG/recorder/recorder.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,24 +35,26 @@
             'posref': array_type_data_callback,
             'att'   : array_type_data_callback,
             'cmd'   : array_type_data_callback,
             'thrust': float_type_data_callback
         }
         ## data storage
         self.record_datastrg = {
+            'acc'   : zeros((3,n)),
             'acccmd': zeros((3,n)),
             'vel'   : zeros((3,n)),
             'pos'   : zeros((3,n)),
             'posref': zeros((3,n)),
             'att'   : zeros((3,n)),
             'cmd'   : zeros((4,n)),
             'thrust': zeros((1,n))
         }
         ## realtime data
         self.realtime_data = {
+            'acc'   : cf.acc,
             'acccmd': cf.command,
             'vel'   : cf.vel,
             'pos'   : cf.pos,
             'posref': cf.destination,
             'att'   : cf.att,
             'cmd'   : commander.command,
             'thrust': commander.thrust
@@ -63,15 +65,15 @@
 
         sleep(0.1)
 
         cf = self.cf
 
         while self.recording:
 
-            self.record_datastrg['acc'][:,self.record_length] = cf.rot @ self.realtime_data['acc']
+            self.record_datastrg['acc'][:,self.record_length] = self.realtime_data['acc']
 
             for key, callback in self.record_callback.items():
 
                 datastrg = self.record_datastrg[key]
                 data     = self.realtime_data[key]
 
                 callback( datastrg, data, self.record_length )
```

### Comparing `CrazyDG-0.0.4/CrazyDG/recorder/visualizer.py` & `CrazyDG-0.0.5/CrazyDG/recorder/visualizer.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.4/CrazyDG.egg-info/SOURCES.txt` & `CrazyDG-0.0.5/CrazyDG.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 CrazyDG/crazy/__init__.py
 CrazyDG/crazy/crazy.py
 CrazyDG/guidance/__init__.py
 CrazyDG/guidance/utils/__init__.py
 CrazyDG/guidance/utils/_goto.py
 CrazyDG/guidance/utils/_hover.py
 CrazyDG/guidance/utils/_landing.py
+CrazyDG/guidance/utils/_landing_supporter.py
 CrazyDG/guidance/utils/_takeoff.py
 CrazyDG/guidance/utils/constants.py
 CrazyDG/guidance/utils/smoother.py
 CrazyDG/navigation/__init__.py
 CrazyDG/navigation/imu.py
 CrazyDG/navigation/imu_setup.py
 CrazyDG/navigation/qualisys.py
```

### Comparing `CrazyDG-0.0.4/setup.py` & `CrazyDG-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='CrazyDG',
-    version='0.0.4',
+    version='0.0.5',
     description='CrazyDG is for convenience',
     author='Daegeun02',
     author_email='redhawkdg02@gmail.com',
     url='https://github.com/Daegeun02/CrazyDG.git',
     install_requires=[],
     packages=find_packages( exclude=[] ),
     keywords=['CrazyDG', 'by daegeun', 'for convenience'],
```

