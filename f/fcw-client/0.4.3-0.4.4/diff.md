# Comparing `tmp/fcw_client-0.4.3.tar.gz` & `tmp/fcw_client-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcw_client-0.4.3.tar", max compression
+gzip compressed data, was "fcw_client-0.4.4.tar", max compression
```

## Comparing `fcw_client-0.4.3.tar` & `fcw_client-0.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-03-15 17:29:23.101730 fcw_client-0.4.3/examples/fcw_client_python/__init__.py
--rw-r--r--   0        0        0     5492 2023-07-19 17:29:18.505068 fcw_client-0.4.3/examples/fcw_client_python/client_python.py
--rw-r--r--   0        0        0     3637 2023-07-19 14:02:25.650830 fcw_client-0.4.3/examples/fcw_client_python/client_python_simple.py
--rw-r--r--   0        0        0        0 2023-03-15 17:29:23.107730 fcw_client-0.4.3/fcw_client/__init__.py
--rw-r--r--   0        0        0     9489 2023-07-19 17:26:13.266409 fcw_client-0.4.3/fcw_client/client_common.py
--rw-r--r--   0        0        0      862 2023-07-19 17:36:23.391424 fcw_client-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      232 2023-07-19 16:44:57.728297 fcw_client-0.4.3/README.md
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 fcw_client-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-15 17:29:23.101730 fcw_client-0.4.4/examples/fcw_client_python/__init__.py
+-rw-r--r--   0        0        0     5541 2023-08-03 15:20:16.122967 fcw_client-0.4.4/examples/fcw_client_python/client_python.py
+-rw-r--r--   0        0        0     3695 2023-08-03 15:28:02.967614 fcw_client-0.4.4/examples/fcw_client_python/client_python_simple.py
+-rw-r--r--   0        0        0        0 2023-03-15 17:29:23.107730 fcw_client-0.4.4/fcw_client/__init__.py
+-rw-r--r--   0        0        0     9508 2023-08-03 15:26:06.839603 fcw_client-0.4.4/fcw_client/client_common.py
+-rw-r--r--   0        0        0      922 2023-08-03 15:37:04.268381 fcw_client-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      232 2023-07-19 16:44:57.728297 fcw_client-0.4.4/README.md
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 fcw_client-0.4.4/PKG-INFO
```

### Comparing `fcw_client-0.4.3/examples/fcw_client_python/client_python.py` & `fcw_client-0.4.4/examples/fcw_client_python/client_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
         rate_timer = RateTimer(rate=fps, time_function=time.perf_counter, iteration_miss_warning=True)
         # Start time
         start_time = time.perf_counter_ns()
         # Check elapsed time or stopped flag
         # Play time in ns
         play_time_ns = args.play_time * 1.0e+9
         # Main processing loop
+        logger.info("Start sending images ...")
         while time.perf_counter_ns() - start_time < play_time_ns and not stopped:
             # Read single frame from a stream
             ret, frame = cap.read()
             if not ret:
                 break
             # Send to FCW service for detection/processing
             collision_warning_client.send_image(frame)
```

### Comparing `fcw_client-0.4.3/examples/fcw_client_python/client_python_simple.py` & `fcw_client-0.4.4/examples/fcw_client_python/client_python_simple.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 from era_5g_interface.utils.rate_timer import RateTimer
 
 # Set logging
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 logger = logging.getLogger("FCW client python")
 
 # Testing video file
-TEST_VIDEO_FILE = str("../../videos/video3.mp4")
+TEST_VIDEO_FILE = str("../../../videos/video3.mp4")
 # TEST_VIDEO_FILE = str("rtsp://127.0.0.1:8554/webcam.h264")
 
 # Testing configuration of the algorithm
-CONFIG_FILE = Path("../../config/config.yaml")
+CONFIG_FILE = Path("../../../config/config.yaml")
 
 # Testing camera settings - specific for the particular input
-CAMERA_CONFIG_FILE = Path("../../videos/video3.yaml")
+CAMERA_CONFIG_FILE = Path("../../../videos/video3.yaml")
 
 
 def results_callback(results: Dict[str, Any]) -> None:
     """Callback which process the results from the FCW service.
 
         Args:
             results (Dict[str, Any]): The results in JSON format.
@@ -72,14 +72,15 @@
             camera_config=args.camera, fps=fps, results_callback=results_callback
         )
 
         # Rate timer for control the speed of a loop (fps)
         rate_timer = RateTimer(rate=fps)
 
         # Main processing loop
+        logger.info("Start sending images...")
         while True:
             # Read single frame from a stream
             ret, frame = cap.read()
             if not ret:
                 break
             # Send to FCW service for detection/processing
             collision_warning_client.send_image(frame)
@@ -87,15 +88,15 @@
             rate_timer.sleep()
         cap.release()
 
     except FailedToConnect as ex:
         logger.error(f"Failed to connect to server: {ex}")
         sys.exit(1)
     except KeyboardInterrupt:
-        logger.info("Terminating...")
+        logger.info("Terminating ...")
     except Exception as ex:
         traceback.print_exc()
         logger.error(f"Exception: {repr(ex)}")
         sys.exit(1)
     finally:
         if collision_warning_client is not None:
             collision_warning_client.stop()
```

### Comparing `fcw_client-0.4.3/fcw_client/client_common.py` & `fcw_client-0.4.4/fcw_client/client_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,17 +182,15 @@
             )
             self.results_callback = self.results_viewer.get_results
         self.stream_type = stream_type
         self.frame_id = 0
 
         # Create FCW client
         self.client = NetAppClientBase(self.results_callback)
-        logger.info(
-            f"Register with netapp_address: {netapp_address}"
-        )
+        logger.info(f"Register with netapp_address: {netapp_address}")
         # Register client
         try:
             if self.stream_type is StreamType.H264:
                 self.client.register(
                     netapp_address,
                     args={"h264": True, "config": self.config_dict, "camera_config": self.camera_config_dict,
                           "fps": self.fps,
@@ -204,14 +202,15 @@
                     args={"config": self.config_dict, "camera_config": self.camera_config_dict, "fps": self.fps}
                 )
             else:
                 raise Exception("Unknown stream type")
         except Exception as e:
             self.client.disconnect()
             raise e
+        logger.info(f"Client registered")
 
     def send_image(self, frame: np.ndarray, timestamp: Optional[int] = None) -> None:
         """Send image to FCW service including rectification.
 
         Args:
             frame (np.ndarray): Image in numpy array format ("bgr24").
             timestamp (int, optional): Timestamp for frame and results synchronization.
```

### Comparing `fcw_client-0.4.3/pyproject.toml` & `fcw_client-0.4.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "fcw-client"
-version = "0.4.3"
+version = "0.4.4"
 description = "Early collision warning Network Application for Transportation use case - client part"
 authors = ["Petr Kleparnik <pkleparnik@cognitechna.cz>", "Roman Juranek <rjuranek@cognitechna.cz>"]
 readme = "README.md"
 repository = "https://github.com/5G-ERA/CollisionWarningService"
 packages = [{include = "fcw_client"}, {include = "fcw_client_python", from = "examples"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 pyyaml = ">=6.0"
 opencv-python = ">=4.6"
 era-5g-client = ">=0.4.1"
 era-5g-interface = ">=0.4.1"
 fcw-core-utils = ">=0.4.3"
+websocket-client = ">=1.5.1"
+simple-websocket = ">=0.9.0"
 
 [tool.poetry.scripts]
 fcw_client_python = "fcw_client_python.client_python:main"
 fcw_client_python_simple = "fcw_client_python.client_python_simple:main"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `fcw_client-0.4.3/PKG-INFO` & `fcw_client-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcw-client
-Version: 0.4.3
+Version: 0.4.4
 Summary: Early collision warning Network Application for Transportation use case - client part
 Home-page: https://github.com/5G-ERA/CollisionWarningService
 Author: Petr Kleparnik
 Author-email: pkleparnik@cognitechna.cz
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: era-5g-client (>=0.4.1)
 Requires-Dist: era-5g-interface (>=0.4.1)
 Requires-Dist: fcw-core-utils (>=0.4.3)
 Requires-Dist: opencv-python (>=4.6)
 Requires-Dist: pyyaml (>=6.0)
+Requires-Dist: simple-websocket (>=0.9.0)
+Requires-Dist: websocket-client (>=1.5.1)
 Project-URL: Repository, https://github.com/5G-ERA/CollisionWarningService
 Description-Content-Type: text/markdown
 
 # Forward Collision Warning - client part
 
 Early collision warning Network Application for Transportation use case - client part.
 The package contains client modules for Forward Collision Warning, including simple examples.
```

