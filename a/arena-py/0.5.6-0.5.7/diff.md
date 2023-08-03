# Comparing `tmp/arena-py-0.5.6.tar.gz` & `tmp/arena-py-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arena-py-0.5.6.tar", last modified: Thu Aug  3 19:05:32 2023, max compression
+gzip compressed data, was "arena-py-0.5.7.tar", last modified: Thu Aug  3 19:13:52 2023, max compression
```

## Comparing `arena-py-0.5.6.tar` & `arena-py-0.5.7.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:05:32.607083 arena-py-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-03 19:05:21.000000 arena-py-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-08-03 19:05:32.607083 arena-py-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-03 19:05:21.000000 arena-py-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:05:32.595083 arena-py-0.5.6/arena/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3148 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/arena_mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:05:32.595083 arena-py-0.5.6/arena/attributes/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/animation_mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/goto_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/impulse.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/jitsi_video.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/landmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/material.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/morph.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/physics.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/text_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/attributes/video_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:05:32.599083 arena-py-0.5.6/arena/event_loop/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/event_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/event_loop/async_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/event_loop/asyncio_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/event_loop/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/event_loop/lazy_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/event_loop/persistent_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/event_loop/single_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/event_loop/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:05:32.599083 arena-py-0.5.6/arena/events/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/events/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:05:32.603083 arena-py-0.5.6/arena/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/arena_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/cone.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/cylinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/dodecahedron.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/gltf.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/icosahedron.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/light.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/octahedron.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/plane.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/tetrahedron.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/thickline.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/torus.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/torus_knot.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/objects/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:05:32.603083 arena-py-0.5.6/arena/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/scripts/arena_py_permissions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/scripts/arena_py_pub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/scripts/arena_py_signout.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/scripts/arena_py_sub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/scripts/arena_py_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:05:32.603083 arena-py-0.5.6/arena/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/utils/cmd_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-03 19:05:21.000000 arena-py-0.5.6/arena/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:05:32.607083 arena-py-0.5.6/arena_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-08-03 19:05:32.000000 arena-py-0.5.6/arena_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-03 19:05:32.000000 arena-py-0.5.6/arena_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:05:32.000000 arena-py-0.5.6/arena_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-03 19:05:32.000000 arena-py-0.5.6/arena_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-03 19:05:32.000000 arena-py-0.5.6/arena_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 19:05:32.000000 arena-py-0.5.6/arena_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 19:05:32.607083 arena-py-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-03 19:05:21.000000 arena-py-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:13:52.418431 arena-py-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-03 19:13:41.000000 arena-py-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-08-03 19:13:52.418431 arena-py-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-03 19:13:41.000000 arena-py-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:13:52.398431 arena-py-0.5.7/arena/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3148 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/arena_mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:13:52.402431 arena-py-0.5.7/arena/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/animation_mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/goto_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/impulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/jitsi_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/landmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/morph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/physics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/text_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/attributes/video_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:13:52.406431 arena-py-0.5.7/arena/event_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/event_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/event_loop/async_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/event_loop/asyncio_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/event_loop/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/event_loop/lazy_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/event_loop/persistent_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/event_loop/single_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/event_loop/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:13:52.406431 arena-py-0.5.7/arena/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/events/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:13:52.414431 arena-py-0.5.7/arena/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/arena_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/dodecahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/icosahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/octahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/tetrahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/thickline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/torus_knot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/objects/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:13:52.418431 arena-py-0.5.7/arena/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/scripts/arena_py_permissions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/scripts/arena_py_pub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/scripts/arena_py_signout.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/scripts/arena_py_sub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/scripts/arena_py_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:13:52.418431 arena-py-0.5.7/arena/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/utils/cmd_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-03 19:13:41.000000 arena-py-0.5.7/arena/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:13:52.418431 arena-py-0.5.7/arena_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-08-03 19:13:52.000000 arena-py-0.5.7/arena_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-03 19:13:52.000000 arena-py-0.5.7/arena_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:13:52.000000 arena-py-0.5.7/arena_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-03 19:13:52.000000 arena-py-0.5.7/arena_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-03 19:13:52.000000 arena-py-0.5.7/arena_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 19:13:52.000000 arena-py-0.5.7/arena_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 19:13:52.418431 arena-py-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-03 19:13:41.000000 arena-py-0.5.7/setup.py
```

### Comparing `arena-py-0.5.6/LICENSE` & `arena-py-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/PKG-INFO` & `arena-py-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.5.6
+Version: 0.5.7
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/ARENA-py
 Author: Conix Research Center
 Author-email: info@conix.io
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `arena-py-0.5.6/README.md` & `arena-py-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/__main__.py` & `arena-py-0.5.7/arena/__main__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/arena_mqtt.py` & `arena-py-0.5.7/arena/arena_mqtt.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/attributes/__init__.py` & `arena-py-0.5.7/arena/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/attributes/animation.py` & `arena-py-0.5.7/arena/attributes/animation.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/attributes/color.py` & `arena-py-0.5.7/arena/attributes/color.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/attributes/data.py` & `arena-py-0.5.7/arena/attributes/data.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/attributes/impulse.py` & `arena-py-0.5.7/arena/attributes/impulse.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/attributes/landmark.py` & `arena-py-0.5.7/arena/attributes/landmark.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/attributes/material.py` & `arena-py-0.5.7/arena/attributes/material.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/attributes/rotation.py` & `arena-py-0.5.7/arena/attributes/rotation.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/auth.py` & `arena-py-0.5.7/arena/auth.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/base_object.py` & `arena-py-0.5.7/arena/base_object.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/device.py` & `arena-py-0.5.7/arena/device.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/event_loop/asyncio_mqtt.py` & `arena-py-0.5.7/arena/event_loop/asyncio_mqtt.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/event_loop/event_loop.py` & `arena-py-0.5.7/arena/event_loop/event_loop.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/event_loop/lazy_worker.py` & `arena-py-0.5.7/arena/event_loop/lazy_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/event_loop/persistent_worker.py` & `arena-py-0.5.7/arena/event_loop/persistent_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/event_loop/worker.py` & `arena-py-0.5.7/arena/event_loop/worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/events/event.py` & `arena-py-0.5.7/arena/events/event.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/objects/__init__.py` & `arena-py-0.5.7/arena/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/objects/arena_object.py` & `arena-py-0.5.7/arena/objects/arena_object.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/objects/box.py` & `arena-py-0.5.7/arena/objects/box.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/objects/camera.py` & `arena-py-0.5.7/arena/objects/camera.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/objects/gltf.py` & `arena-py-0.5.7/arena/objects/gltf.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/objects/thickline.py` & `arena-py-0.5.7/arena/objects/thickline.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/scene.py` & `arena-py-0.5.7/arena/scene.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/scripts/arena_py_pub.py` & `arena-py-0.5.7/arena/scripts/arena_py_pub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/scripts/arena_py_sub.py` & `arena-py-0.5.7/arena/scripts/arena_py_sub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/utils/cmd_interpreter.py` & `arena-py-0.5.7/arena/utils/cmd_interpreter.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena/utils/utils.py` & `arena-py-0.5.7/arena/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/arena_py.egg-info/PKG-INFO` & `arena-py-0.5.7/arena_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.5.6
+Version: 0.5.7
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/ARENA-py
 Author: Conix Research Center
 Author-email: info@conix.io
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `arena-py-0.5.6/arena_py.egg-info/SOURCES.txt` & `arena-py-0.5.7/arena_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arena-py-0.5.6/setup.py` & `arena-py-0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="arena-py",
-    version="0.5.6",
+    version="0.5.7",
     author="Conix Research Center",
     author_email="info@conix.io",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     description="Draw objects and run programs in the ARENA using Python!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arenaxr/ARENA-py",
```

