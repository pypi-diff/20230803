# Comparing `tmp/rria_api-1.0.5.tar.gz` & `tmp/rria_api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rria_api-1.0.5.tar", max compression
+gzip compressed data, was "rria_api-1.0.6.tar", max compression
```

## Comparing `rria_api-1.0.5.tar` & `rria_api-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      848 2023-08-01 19:29:35.064063 rria_api-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1509 2023-04-10 17:18:59.252547 rria_api-1.0.5/README.md
--rw-r--r--   0        0        0       29 2023-04-10 17:18:59.257980 rria_api-1.0.5/rria_api/__init__.py
--rw-r--r--   0        0        0     1321 2023-03-24 11:48:25.776937 rria_api-1.0.5/rria_api/gen3/action_gen3.py
--rw-r--r--   0        0        0     1559 2023-03-24 11:48:25.778442 rria_api-1.0.5/rria_api/gen3/api_gen3/device_connection.py
--rw-r--r--   0        0        0     7947 2023-08-01 19:28:24.939682 rria_api-1.0.5/rria_api/gen3/api_gen3/gen3_api.py
--rw-r--r--   0        0        0      637 2023-03-24 11:48:25.778442 rria_api-1.0.5/rria_api/gen3/connect_gen3.py
--rw-r--r--   0        0        0     1342 2023-03-24 11:48:25.779454 rria_api-1.0.5/rria_api/ned/action_ned.py
--rw-r--r--   0        0        0      360 2023-03-24 11:48:25.779454 rria_api-1.0.5/rria_api/ned/connect_ned.py
--rw-r--r--   0        0        0    22047 2023-04-10 17:18:59.258978 rria_api-1.0.5/rria_api/poetry.lock
--rw-r--r--   0        0        0    10829 2023-04-10 17:18:59.258978 rria_api-1.0.5/rria_api/robot_facade.py
--rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 rria_api-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      687 2023-08-03 11:59:21.659738 rria_api-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1509 2023-08-02 13:38:32.621902 rria_api-1.0.6/README.md
+-rw-r--r--   0        0        0       29 2023-08-02 13:30:21.915376 rria_api-1.0.6/rria_api/__init__.py
+-rw-r--r--   0        0        0     1321 2023-03-24 11:48:25.776937 rria_api-1.0.6/rria_api/gen3/action_gen3.py
+-rw-r--r--   0        0        0     1559 2023-03-24 11:48:25.778442 rria_api-1.0.6/rria_api/gen3/api_gen3/device_connection.py
+-rw-r--r--   0        0        0     7954 2023-08-02 13:28:02.768683 rria_api-1.0.6/rria_api/gen3/api_gen3/gen3_api.py
+-rw-r--r--   0        0        0      637 2023-03-24 11:48:25.778442 rria_api-1.0.6/rria_api/gen3/connect_gen3.py
+-rw-r--r--   0        0        0     1342 2023-03-24 11:48:25.779454 rria_api-1.0.6/rria_api/ned/action_ned.py
+-rw-r--r--   0        0        0      360 2023-03-24 11:48:25.779454 rria_api-1.0.6/rria_api/ned/connect_ned.py
+-rw-r--r--   0        0        0    22047 2023-04-10 17:18:59.258978 rria_api-1.0.6/rria_api/poetry.lock
+-rw-r--r--   0        0        0    10829 2023-04-10 17:18:59.258978 rria_api-1.0.6/rria_api/robot_object.py
+-rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 rria_api-1.0.6/PKG-INFO
```

### Comparing `rria_api-1.0.5/pyproject.toml` & `rria_api-1.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "rria-api"
-version = "1.0.5"
+version = "1.0.6"
 description = ""
 authors = ["felipeadsm <97059009+felipeadsm@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "rria_api" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyniryo = "^1.1.2"
-kortex_api = {path = "kortex_api-2.3.0.post34-py3-none-any.whl"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 taskipy = "^1.10.3"
 ipython = "^8.11.0"
 
@@ -24,11 +23,8 @@
 pymdown-extensions = "^9.9.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.taskipy.tasks]
-docs = "mkdocs serve"
-pre_test = "task lint"
-test = "pytest -s -x --cov=copychat -vv"
-post_test = "coverage html"
+docs = "mkdocs serve"
```

### Comparing `rria_api-1.0.5/README.md` & `rria_api-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ```
 from rria_api.robot_facade import *
 
 # Create gen3 RobotObject
 gen3_lite = RobotObject('172.22.64.105', 'gen3')
 
-# Create Nirio NED RobotObject
+# Create Niryo NED RobotObject
 ned = RobotObject('169.254.200.200', 'ned')
 
 gen3_lite.connect_robot()
 ned.connect_robot()
 
 gen3_lite.move_joints(30.0, 30.0, 30.0, 30.0, 30.0, 30.0)
 ned.move_joints(30.0, 30.0, 30.0, 30.0, 30.0, 30.0)
```

### Comparing `rria_api-1.0.5/rria_api/gen3/action_gen3.py` & `rria_api-1.0.6/rria_api/gen3/action_gen3.py`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.5/rria_api/gen3/api_gen3/device_connection.py` & `rria_api-1.0.6/rria_api/gen3/api_gen3/device_connection.py`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.5/rria_api/gen3/api_gen3/gen3_api.py` & `rria_api-1.0.6/rria_api/gen3/api_gen3/gen3_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,18 +48,18 @@
         if finished:
             print("Safe position reached")
         else:
             print("Timeout on action notification wait")
         return finished
 
     @staticmethod
-    def populate_angular_pose(jointPose, durationFactor):
+    def populate_angular_pose(joint_pose, duration_factor):
         waypoint = Base_pb2.AngularWaypoint()
-        waypoint.angles.extend(jointPose)
-        waypoint.duration = durationFactor * 5.0
+        waypoint.angles.extend(joint_pose)
+        waypoint.duration = duration_factor * 5.0
 
         return waypoint
 
     # Método utilizado para mover o robô para waypoints definidos.
     def move_trajectory(self, base, joints_list):
         base_servo_mode = Base_pb2.ServoingModeInformation()
         base_servo_mode.servoing_mode = Base_pb2.SINGLE_LEVEL_SERVOING
@@ -71,20 +71,20 @@
         waypoints.duration = 0.0
         waypoints.use_optimal_blending = False
 
         index = 0
         for joint_pose in joint_poses:
             waypoint = waypoints.waypoints.add()
             waypoint.name = "waypoint_" + str(index)
-            durationFactor = 1
+            duration_factor = 1
             # Joints/motors 5 and 7 are slower and need more time
             if index == 4 or index == 6:
-                durationFactor = 6  # Min 30 seconds
+                duration_factor = 6  # Min 30 seconds
 
-            waypoint.angular_waypoint.CopyFrom(self.populate_angular_pose(joint_pose, durationFactor))
+            waypoint.angular_waypoint.CopyFrom(self.populate_angular_pose(joint_pose, duration_factor))
             index = index + 1
 
             # Verify validity of waypoints
         result = base.ValidateWaypointList(waypoints)
         if len(result.trajectory_error_report.trajectory_error_elements) == 0:
 
             e = threading.Event()
```

### Comparing `rria_api-1.0.5/rria_api/gen3/connect_gen3.py` & `rria_api-1.0.6/rria_api/gen3/connect_gen3.py`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.5/rria_api/ned/action_ned.py` & `rria_api-1.0.6/rria_api/ned/action_ned.py`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.5/rria_api/poetry.lock` & `rria_api-1.0.6/rria_api/poetry.lock`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.5/rria_api/robot_facade.py` & `rria_api-1.0.6/rria_api/robot_object.py`

 * *Files identical despite different names*

### Comparing `rria_api-1.0.5/PKG-INFO` & `rria_api-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: rria-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 Author: felipeadsm
 Author-email: 97059009+felipeadsm@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kortex_api @ file:///C:/Users/fasm/Documents/GitHub/rria_api/kortex_api-2.3.0.post34-py3-none-any.whl
 Requires-Dist: pyniryo (>=1.1.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # RRIA-API
 
 The `rria-api` is an easy-to-use package that provides a common interface to control robots used by the Residence in Robotics
 and AI at the UFPE's informatics center. The API currently supports the use of Kinova Gen3 lite and Niryo NED, with
@@ -45,15 +44,15 @@
 
 ```
 from rria_api.robot_facade import *
 
 # Create gen3 RobotObject
 gen3_lite = RobotObject('172.22.64.105', 'gen3')
 
-# Create Nirio NED RobotObject
+# Create Niryo NED RobotObject
 ned = RobotObject('169.254.200.200', 'ned')
 
 gen3_lite.connect_robot()
 ned.connect_robot()
 
 gen3_lite.move_joints(30.0, 30.0, 30.0, 30.0, 30.0, 30.0)
 ned.move_joints(30.0, 30.0, 30.0, 30.0, 30.0, 30.0)
```

