# Comparing `tmp/micrOSDevToolKit-1.21.1.tar.gz` & `tmp/micrOSDevToolKit-1.21.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.21.1.tar", last modified: Tue Aug  1 20:08:06 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.21.2.tar", last modified: Wed Aug  2 17:47:22 2023, max compression
```

## Comparing `micrOSDevToolKit-1.21.1.tar` & `micrOSDevToolKit-1.21.2.tar`

### file list

```diff
@@ -1,255 +1,255 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.723503 micrOSDevToolKit-1.21.1/
--rw-r--r--   0 bnm        (501) staff       (20)      333 2023-07-18 21:54:39.000000 micrOSDevToolKit-1.21.1/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-08-01 20:08:06.722123 micrOSDevToolKit-1.21.1/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.21.1/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.21.1/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.315578 micrOSDevToolKit-1.21.1/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.329491 micrOSDevToolKit-1.21.1/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.1/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.1/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.332517 micrOSDevToolKit-1.21.1/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.21.1/micrOS/SchedulerUT.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.379010 micrOSDevToolKit-1.21.1/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.21.1/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.21.1/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.490203 micrOSDevToolKit-1.21.1/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.21.1/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6205 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.1/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.21.1/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6443 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.1/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.21.1/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.21.1/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-08-01 19:32:01.000000 micrOSDevToolKit-1.21.1/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.21.1/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     3786 2023-08-01 19:30:57.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_aht10.py
--rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_lmpacman.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    19328 2023-07-26 14:42:47.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.21.1/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.21.1/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.21.1/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.21.1/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-29 10:25:26.000000 micrOSDevToolKit-1.21.1/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19349 2023-07-29 10:13:31.000000 micrOSDevToolKit-1.21.1/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.21.1/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/source/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.21.1/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.21.1/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.21.1/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.21.1/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.493405 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-08-01 20:08:06.000000 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     8935 2023-08-01 20:08:06.000000 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-08-01 20:08:06.000000 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-08-01 20:08:06.000000 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-08-01 20:08:06.000000 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-08-01 20:08:06.724174 micrOSDevToolKit-1.21.1/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-08-01 19:35:09.000000 micrOSDevToolKit-1.21.1/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.501959 micrOSDevToolKit-1.21.1/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.21.1/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.21.1/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.21.1/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.21.1/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.520929 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.527045 micrOSDevToolKit-1.21.1/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.21.1/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.21.1/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.21.1/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.21.1/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.541894 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.603010 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5415 2023-08-01 19:28:24.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6584 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.21.1/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.605101 micrOSDevToolKit-1.21.1/toolkit/user_data/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.21.1/toolkit/user_data/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.605965 micrOSDevToolKit-1.21.1/toolkit/user_data/node_config_archive/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/user_data/node_config_archive/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.606344 micrOSDevToolKit-1.21.1/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.719150 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1990 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      759 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     1297 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_aht10.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      512 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_lmpacman.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6191 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5718 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.585735 micrOSDevToolKit-1.21.2/
+-rw-r--r--   0 bnm        (501) staff       (20)      333 2023-07-18 21:54:39.000000 micrOSDevToolKit-1.21.2/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-08-02 17:47:22.584886 micrOSDevToolKit-1.21.2/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.21.2/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.21.2/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.131929 micrOSDevToolKit-1.21.2/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.2/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.158652 micrOSDevToolKit-1.21.2/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.2/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.2/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.162112 micrOSDevToolKit-1.21.2/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.21.2/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.2/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.231388 micrOSDevToolKit-1.21.2/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.2/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.21.2/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.21.2/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.2/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.297366 micrOSDevToolKit-1.21.2/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.21.2/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6218 2023-08-02 12:29:26.000000 micrOSDevToolKit-1.21.2/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.21.2/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6443 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.2/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.21.2/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.21.2/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-08-02 17:26:19.000000 micrOSDevToolKit-1.21.2/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.21.2/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3786 2023-08-01 19:30:57.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_aht10.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3559 2023-08-02 17:26:12.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_lmpacman.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19328 2023-07-26 14:42:47.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-08-02 13:17:09.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.21.2/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.21.2/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.2/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.2/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.21.2/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.21.2/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.21.2/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.21.2/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-29 10:25:26.000000 micrOSDevToolKit-1.21.2/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19349 2023-07-29 10:13:31.000000 micrOSDevToolKit-1.21.2/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.21.2/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.2/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.2/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.21.2/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.21.2/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.21.2/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.21.2/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.300465 micrOSDevToolKit-1.21.2/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-08-02 17:47:21.000000 micrOSDevToolKit-1.21.2/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     8935 2023-08-02 17:47:21.000000 micrOSDevToolKit-1.21.2/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-08-02 17:47:21.000000 micrOSDevToolKit-1.21.2/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-08-02 17:47:21.000000 micrOSDevToolKit-1.21.2/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-08-02 17:47:21.000000 micrOSDevToolKit-1.21.2/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-08-02 17:47:22.585914 micrOSDevToolKit-1.21.2/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-08-02 17:45:16.000000 micrOSDevToolKit-1.21.2/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.307725 micrOSDevToolKit-1.21.2/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.21.2/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.21.2/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.21.2/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.21.2/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.369635 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.375128 micrOSDevToolKit-1.21.2/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.21.2/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.21.2/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.21.2/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.21.2/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.404036 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.515804 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7455 2023-08-02 12:44:06.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5415 2023-08-01 19:28:24.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4828 2023-08-02 12:43:56.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6584 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.21.2/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.516607 micrOSDevToolKit-1.21.2/toolkit/user_data/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.21.2/toolkit/user_data/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.517130 micrOSDevToolKit-1.21.2/toolkit/user_data/node_config_archive/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/user_data/node_config_archive/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.517771 micrOSDevToolKit-1.21.2/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-02 17:47:22.583361 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1990 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      759 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1297 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_aht10.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1193 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_lmpacman.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6191 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5718 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-08-02 17:26:51.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-08-02 17:26:50.000000 micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.21.1/PKG-INFO` & `micrOSDevToolKit-1.21.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.21.1
+Version: 1.21.2
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.21.1/README.md` & `micrOSDevToolKit-1.21.2/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/devToolKit.py` & `micrOSDevToolKit-1.21.2/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/media/dnd.png` & `micrOSDevToolKit-1.21.2/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/media/logo.png` & `micrOSDevToolKit-1.21.2/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/media/logo_mini.png` & `micrOSDevToolKit-1.21.2/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/SchedulerUT.py` & `micrOSDevToolKit-1.21.2/micrOS/SchedulerUT.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.2/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.2/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.21.2/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.21.2/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.2/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.21.2/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/Common.py` & `micrOSDevToolKit-1.21.2/micrOS/source/Common.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         ADC.ATTN_6DB: 6 dB ... of 0-2.2V
         ADC.ATTN_11DB: 11 dB ... of 0-2450mV/
     Note that the absolute maximum voltage rating for input pins is 3.6V. Going near to this boundary risks damage to the IC!
     """
     OBJS = {}
 
     def __init__(self, pin):
-        self.adp_prop = (65535, 2450)                               # 2450mV so 2,45V
+        self.adp_prop = (65535, 2450)                               # raw value, 2450mV (so 2,45V)
         self.adc = None
         if not isinstance(pin, int):
             pin = physical_pin(pin)
         self.adc = ADC(Pin(pin))
         self.adc.atten(ADC.ATTN_11DB)                               # 2450mV measure range
 
     def get(self):
```

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.21.2/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/Debug.py` & `micrOSDevToolKit-1.21.2/micrOS/source/Debug.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.21.2/micrOS/source/Hooks.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.21.2/micrOS/source/InterConnect.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.21.2/micrOS/source/InterpreterShell.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.21.0-1'
+    MICROS_VERSION = '1.21.0-3'
 
     def __init__(self, msg_obj=None):
         """
         comm_obj - communication object - send messages back
                  - comm_obj.reply('msg')
         """
         self.msg_obj = msg_obj
```

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.21.2/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_aht10.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_aht10.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_distance.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,87 @@
-"""
-Source: https://how2electronics.com/temt6000-ambient-light-sensor-arduino-measure-light-intensity/
-ADC.ATTN_0DB — the full range voltage: 1.2V
-ADC.ATTN_2_5DB — the full range voltage: 1.5V
-ADC.ATTN_6DB — the full range voltage: 2.0V
-ADC.ATTN_11DB — the full range voltage: 3.3V
-"""
+from machine import Pin, time_pulse_us
+from utime import sleep_us
 from LogicalPins import physical_pin, pinmap_dump
-from Common import SmartADC
 
-ADC = None
+__TRIGGER_OBJ = None
+__ECHO_OBJ = None
 
 
-def __init_tempt6000():
-    """
-    Setup ADC
-    """
-    global ADC
-    if ADC is None:
-        ADC = SmartADC(physical_pin('temp6000'))
-    return ADC
-
-
-def intensity():
-    """
-    Measure light intensity in %
-    """
-    percent = __init_tempt6000().get()['percent']
-    return {'light intensity [%]': percent}
-
-
-def illuminance():
-    """
-    Measure light illuminance in flux
-    """
-    volts = __init_tempt6000().get()['volt']
-    amps = volts / 10000.0                    # across 10,000 Ohms (voltage divider circuit)
-    microamps = amps * 1000000
-    lux = '{:.2f}'.format(microamps * 2.0)
-    return {'illuminance [lux]': lux}
+def __init_HCSR04():
+    global __TRIGGER_OBJ, __ECHO_OBJ
+    if __TRIGGER_OBJ is None or __ECHO_OBJ is None:
+        trigger_pin = physical_pin('hcsrtrig')
+        echo_pin = physical_pin('hcsrecho')
+        # Init trigger pin (out)
+        __TRIGGER_OBJ = Pin(trigger_pin, mode=Pin.OUT, pull=None)
+        __TRIGGER_OBJ.value(0)
+        # Init echo pin (in)
+        __ECHO_OBJ = Pin(echo_pin, mode=Pin.IN, pull=None)
+    return __TRIGGER_OBJ, __ECHO_OBJ
+
+
+def __send_pulse_and_wait(echo_timeout_us=1000000):
+    trigger_pin, echo_pin = __init_HCSR04()
+    trigger_pin.value(0) # Stabilize the sensor
+    sleep_us(5)
+    trigger_pin.value(1)
+    # Send a 10us pulse.
+    sleep_us(10)
+    trigger_pin.value(0)
+    try:
+        pulse_time = time_pulse_us(echo_pin, 1, echo_timeout_us)
+        return pulse_time
+    except OSError as ex:
+        if ex.args[0] == 110: # 110 = ETIMEDOUT
+            raise OSError('Out of range')
+        raise ex
+
+
+#########################
+# Application functions #
+#########################
+
+def distance_mm():
+    """
+    To calculate the distance we get the pulse_time and divide it by 2
+    (the pulse walk the distance twice) and by 29.1 becasue
+    the sound speed on air (343.2 m/s), that It's equivalent to
+    0.34320 mm/us that is 1mm each 2.91us
+    pulse_time // 2 // 2.91 -> pulse_time // 5.82 -> pulse_time * 100 // 582
+    """
+    return __send_pulse_and_wait() * 100 // 582
+
+
+def distance_cm():
+    return (__send_pulse_and_wait() / 2) / 29.1
+
+
+def deinit():
+    global __TRIGGER_OBJ, __ECHO_OBJ
+    trigger_pin, echo_pin = __init_HCSR04()
+    trigger_pin.deinit()
+    echo_pin.deinit()
+    __TRIGGER_OBJ = None
+    __ECHO_OBJ = None
 
 
 #######################
 # LM helper functions #
 #######################
 
 def pinmap():
     """
     [i] micrOS LM naming convention
     Shows logical pins - pin number(s) used by this Load module
     - info which pins to use for this application
     :return dict: pin name (str) - pin value (int) pairs
     """
-    return pinmap_dump('temp6000')
+    return pinmap_dump(['hcsrtrig', 'hcsrecho'])
 
 
 def help():
     """
     [i] micrOS LM naming convention
     Load Module built-in help message
     :return tuple: list of functions implemented by this application
     """
-    return 'intensity', 'illuminance', 'pinmap', 'INFO sensor:TEMP600'
-
+    return 'distance_mm', 'distance_cm', 'deinit', 'pinmap'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_lmpacman.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_lmpacman.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.21.2/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/Network.py` & `micrOSDevToolKit-1.21.2/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/Notify.py` & `micrOSDevToolKit-1.21.2/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.21.2/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.21.2/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.21.2/micrOS/source/TaskManager.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/Time.py` & `micrOSDevToolKit-1.21.2/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.21.2/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.21.2/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.21.2/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOS/source/urequests.py` & `micrOSDevToolKit-1.21.2/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.21.2/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.21.1
+Version: 1.21.2
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.21.2/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/setup.py` & `micrOSDevToolKit-1.21.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.21.1',
+    version='1.21.2',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.21.1/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.21.2/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.21.2/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.21.2/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/Gateway.py` & `micrOSDevToolKit-1.21.2/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.21.2/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.21.2/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.21.2/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.21.2/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.21.2/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.21.2/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.21.2/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.21.2/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Jul  1 22:39:14 2023 UTC, .py size: 4430 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 12ab a064 4e11 0000  a..........dN...
+00000000: 610d 0d0a 0000 0000 8c4f ca64 dc12 0000  a........O.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6402 6c06 5a06 6404  m.Z...d.d.l.Z.d.
 00000060: 6405 8400 5a07 4700 6406 6407 8400 6407  d...Z.G.d.d...d.
 00000070: 8302 5a08 4700 6408 6409 8400 6409 8302  ..Z.G.d.d...d...
@@ -233,208 +233,234 @@
 00000e80: 2901 4e29 0772 2200 0000 7223 0000 0072  ).N).r"...r#...r
 00000e90: 2400 0000 7213 0000 0072 3800 0000 7237  $...r....r8...r7
 00000ea0: 0000 0072 2d00 0000 7208 0000 0072 0800  ...r-...r....r..
 00000eb0: 0000 7208 0000 0072 0900 0000 7232 0000  ..r....r....r2..
 00000ec0: 004e 0000 0073 0800 0000 0802 0a06 0a06  .N...s..........
 00000ed0: 0a06 7232 0000 0063 0000 0000 0000 0000  ..r2...c........
 00000ee0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000ef0: 733a 0000 0065 005a 0164 005a 0264 015a  s:...e.Z.d.Z.d.Z
-00000f00: 0364 015a 0464 015a 0564 0b64 0364 0484  .d.Z.d.Z.d.d.d..
+00000ef0: 734a 0000 0065 005a 0164 005a 0264 015a  sJ...e.Z.d.Z.d.Z
+00000f00: 0364 015a 0464 015a 0564 0f64 0364 0484  .d.Z.d.Z.d.d.d..
 00000f10: 015a 0664 0564 0684 005a 0764 0764 0884  .Z.d.d...Z.d.d..
-00000f20: 005a 0864 0964 0a84 005a 0964 0253 0029  .Z.d.d...Z.d.S.)
-00000f30: 0cda 0341 4443 da05 6475 6d6d 794e 6302  ...ADC..dummyNc.
-00000f40: 0000 0000 0000 0000 0000 0002 0000 0001  ................
-00000f50: 0000 0043 0000 0073 0400 0000 6400 5300  ...C...s....d.S.
-00000f60: a901 4e72 0800 0000 2902 7212 0000 0072  ..Nr....).r....r
-00000f70: 2700 0000 7208 0000 0072 0800 0000 7209  '...r....r....r.
-00000f80: 0000 0072 1300 0000 6b00 0000 7302 0000  ...r....k...s...
-00000f90: 0000 017a 0c41 4443 2e5f 5f69 6e69 745f  ...z.ADC.__init_
-00000fa0: 5f63 0100 0000 0000 0000 0000 0000 0300  _c..............
-00000fb0: 0000 0100 0000 4f00 0000 7304 0000 0064  ......O...s....d
-00000fc0: 0053 0072 3b00 0000 7208 0000 0072 2800  .S.r;...r....r(.
-00000fd0: 0000 7208 0000 0072 0800 0000 7209 0000  ..r....r....r...
-00000fe0: 00da 0561 7474 656e 6e00 0000 7302 0000  ...attenn...s...
-00000ff0: 0000 017a 0941 4443 2e61 7474 656e 6301  ...z.ADC.attenc.
-00001000: 0000 0000 0000 0000 0000 0003 0000 0001  ................
-00001010: 0000 004f 0000 0073 0400 0000 6400 5300  ...O...s....d.S.
-00001020: 723b 0000 0072 0800 0000 7228 0000 0072  r;...r....r(...r
-00001030: 0800 0000 7208 0000 0072 0900 0000 da05  ....r....r......
-00001040: 7769 6474 6871 0000 0073 0200 0000 0001  widthq...s......
-00001050: 7a09 4144 432e 7769 6474 6863 0100 0000  z.ADC.widthc....
-00001060: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00001070: 4300 0000 7304 0000 0064 0153 0029 024e  C...s....d.S.).N
-00001080: 69a4 0100 0072 0800 0000 722c 0000 0072  i....r....r,...r
-00001090: 0800 0000 7208 0000 0072 0900 0000 da04  ....r....r......
-000010a0: 7265 6164 7400 0000 7302 0000 0000 017a  readt...s......z
-000010b0: 0841 4443 2e72 6561 6429 014e 290a 7222  .ADC.read).N).r"
-000010c0: 0000 0072 2300 0000 7224 0000 005a 0941  ...r#...r$...Z.A
-000010d0: 5454 4e5f 3131 4442 5a0a 5749 4454 485f  TTN_11DBZ.WIDTH_
-000010e0: 3942 4954 5a0b 5749 4454 485f 3130 4249  9BITZ.WIDTH_10BI
-000010f0: 5472 1300 0000 723c 0000 0072 3d00 0000  Tr....r<...r=...
-00001100: 723e 0000 0072 0800 0000 7208 0000 0072  r>...r....r....r
-00001110: 0800 0000 7209 0000 0072 3900 0000 6600  ....r....r9...f.
-00001120: 0000 730e 0000 0008 0104 0104 0104 020a  ..s.............
-00001130: 0308 0308 0372 3900 0000 6300 0000 0000  .....r9...c.....
-00001140: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
-00001150: 0000 0073 3400 0000 6500 5a01 6400 5a02  ...s4...e.Z.d.Z.
-00001160: 6401 6402 8400 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
-00001170: 6405 6406 8400 5a05 6407 6408 8400 5a06  d.d...Z.d.d...Z.
-00001180: 6409 640a 8400 5a07 640b 5300 290c da03  d.d...Z.d.S.)...
-00001190: 4932 4363 0400 0000 0000 0000 0000 0000  I2Cc............
-000011a0: 0400 0000 0200 0000 4300 0000 7316 0000  ........C...s...
-000011b0: 007c 017c 005f 007c 027c 005f 017c 037c  .|.|._.|.|._.|.|
-000011c0: 005f 0264 0053 0072 3b00 0000 2903 da03  ._.d.S.r;...)...
-000011d0: 7363 6cda 0373 6461 7237 0000 00a9 0472  scl..sdar7.....r
-000011e0: 1200 0000 7240 0000 0072 4100 0000 7237  ....r@...rA...r7
-000011f0: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-00001200: 0000 7213 0000 007a 0000 0073 0600 0000  ..r....z...s....
-00001210: 0001 0601 0601 7a0c 4932 432e 5f5f 696e  ......z.I2C.__in
-00001220: 6974 5f5f 6303 0000 0000 0000 0000 0000  it__c...........
-00001230: 0003 0000 000b 0000 0043 0000 0073 3000  .........C...s0.
-00001240: 0000 7400 6401 7c00 6a01 9b00 6402 7c00  ..t.d.|.j...d.|.
-00001250: 6a02 9b00 6403 7c00 6a03 9b00 6404 7c01  j...d.|.j...d.|.
-00001260: 9b00 6405 7c02 9b00 9d0a 8301 0100 6406  ..d.|.........d.
-00001270: 5300 2907 4e7a 135b 4932 4320 7772 6974  S.).Nz.[I2C writ
-00001280: 6574 6f5d 2073 636c 3a20 fa06 2073 6461  eto] scl: .. sda
-00001290: 3a20 fa07 2066 7265 713a 20fa 0720 6164  : .. freq: .. ad
-000012a0: 6472 3a20 7a08 2076 616c 7565 3a20 54a9  dr: z. value: T.
-000012b0: 0472 0400 0000 7240 0000 0072 4100 0000  .r....r@...rA...
-000012c0: 7237 0000 0029 0372 1200 0000 da07 6164  r7...).r......ad
-000012d0: 6472 6573 7372 2b00 0000 7208 0000 0072  dressr+...r....r
-000012e0: 0800 0000 7209 0000 00da 0777 7269 7465  ....r......write
-000012f0: 746f 7f00 0000 7304 0000 0000 012c 017a  to....s......,.z
-00001300: 0b49 3243 2e77 7269 7465 746f 6304 0000  .I2C.writetoc...
-00001310: 0000 0000 0000 0000 0004 0000 000d 0000  ................
-00001320: 0043 0000 0073 3600 0000 7400 6401 7c00  .C...s6...t.d.|.
-00001330: 6a01 9b00 6402 7c00 6a02 9b00 6403 7c00  j...d.|.j...d.|.
-00001340: 6a03 9b00 6404 7c01 9b00 6405 7c02 9b00  j...d.|...d.|...
-00001350: 6406 7c03 9b00 9d0c 8301 0100 6407 5300  d.|.........d.S.
-00001360: 2908 4e7a 175b 4932 4320 7772 6974 6574  ).Nz.[I2C writet
-00001370: 6f5f 6d65 6d5d 2073 636c 3a20 7243 0000  o_mem] scl: rC..
-00001380: 0072 4400 0000 7245 0000 00fa 0620 7265  .rD...rE..... re
-00001390: 673a 207a 0620 6269 743a 2054 7246 0000  g: z. bit: TrF..
-000013a0: 0029 0472 1200 0000 7247 0000 00da 0872  .).r....rG.....r
-000013b0: 6567 6973 7465 72da 0162 7208 0000 0072  egister..br....r
-000013c0: 0800 0000 7209 0000 00da 0b77 7269 7465  ....r......write
-000013d0: 746f 5f6d 656d 8300 0000 7304 0000 0000  to_mem....s.....
-000013e0: 0132 017a 0f49 3243 2e77 7269 7465 746f  .2.z.I2C.writeto
-000013f0: 5f6d 656d 6303 0000 0000 0000 0000 0000  _memc...........
-00001400: 0003 0000 000b 0000 0043 0000 0073 3000  .........C...s0.
-00001410: 0000 7400 6401 7c00 6a01 9b00 6402 7c00  ..t.d.|.j...d.|.
-00001420: 6a02 9b00 6403 7c00 6a03 9b00 6404 7c01  j...d.|.j...d.|.
-00001430: 9b00 6405 7c02 9b00 9d0a 8301 0100 6406  ..d.|.........d.
-00001440: 5300 2907 4e7a 145b 4932 4320 7265 6164  S.).Nz.[I2C read
-00001450: 6672 6f6d 5d20 7363 6c3a 2072 4300 0000  from] scl: rC...
-00001460: 7244 0000 0072 4500 0000 fa07 2062 7974  rD...rE..... byt
-00001470: 653a 20f3 0800 0000 3030 3030 3030 3030  e: .....00000000
-00001480: 7246 0000 0029 0372 1200 0000 7247 0000  rF...).r....rG..
-00001490: 00da 0462 7974 6572 0800 0000 7208 0000  ...byter....r...
-000014a0: 0072 0900 0000 da08 7265 6164 6672 6f6d  .r......readfrom
-000014b0: 8700 0000 7304 0000 0000 012c 017a 0c49  ....s......,.z.I
-000014c0: 3243 2e72 6561 6466 726f 6d63 0400 0000  2C.readfromc....
-000014d0: 0000 0000 0000 0000 0400 0000 0d00 0000  ................
-000014e0: 4300 0000 7336 0000 0074 0064 017c 006a  C...s6...t.d.|.j
-000014f0: 019b 0064 027c 006a 029b 0064 037c 006a  ...d.|.j...d.|.j
-00001500: 039b 0064 047c 019b 0064 057c 029b 0064  ...d.|...d.|...d
-00001510: 067c 039b 009d 0c83 0101 0064 0753 0029  .|.........d.S.)
-00001520: 084e 7a18 5b49 3243 2072 6561 6466 726f  .Nz.[I2C readfro
-00001530: 6d5f 6d65 6d5d 2073 636c 3a20 7243 0000  m_mem] scl: rC..
-00001540: 0072 4400 0000 7245 0000 0072 4900 0000  .rD...rE...rI...
-00001550: 724d 0000 0072 4e00 0000 7246 0000 0029  rM...rN...rF...)
-00001560: 0472 1200 0000 7247 0000 0072 4a00 0000  .r....rG...rJ...
-00001570: 724f 0000 0072 0800 0000 7208 0000 0072  rO...r....r....r
-00001580: 0900 0000 da0c 7265 6164 6672 6f6d 5f6d  ......readfrom_m
-00001590: 656d 8b00 0000 7304 0000 0000 0132 017a  em....s......2.z
-000015a0: 1049 3243 2e72 6561 6466 726f 6d5f 6d65  .I2C.readfrom_me
-000015b0: 6d4e 2908 7222 0000 0072 2300 0000 7224  mN).r"...r#...r$
-000015c0: 0000 0072 1300 0000 7248 0000 0072 4c00  ...r....rH...rL.
-000015d0: 0000 7250 0000 0072 5100 0000 7208 0000  ..rP...rQ...r...
-000015e0: 0072 0800 0000 7208 0000 0072 0900 0000  .r....r....r....
-000015f0: 723f 0000 0078 0000 0073 0a00 0000 0802  r?...x...s......
-00001600: 0805 0804 0804 0804 723f 0000 0063 0000  ........r?...c..
-00001610: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00001620: 0000 0000 0000 731c 0000 0065 005a 0164  ......s....e.Z.d
-00001630: 005a 0287 0066 0164 0164 0284 085a 0387  .Z...f.d.d...Z..
-00001640: 0004 005a 0453 0029 03da 0753 6f66 7449  ...Z.S.)...SoftI
-00001650: 3243 6304 0000 0000 0000 0000 0000 0004  2Cc.............
-00001660: 0000 0005 0000 0003 0000 0073 1400 0000  ...........s....
-00001670: 7400 8300 a001 7c01 7c02 7c03 a103 0100  t.....|.|.|.....
-00001680: 6400 5300 723b 0000 0029 02da 0573 7570  d.S.r;...)...sup
-00001690: 6572 7213 0000 0072 4200 0000 a901 da09  err....rB.......
-000016a0: 5f5f 636c 6173 735f 5f72 0800 0000 7209  __class__r....r.
-000016b0: 0000 0072 1300 0000 9200 0000 7302 0000  ...r........s...
-000016c0: 0000 017a 1053 6f66 7449 3243 2e5f 5f69  ...z.SoftI2C.__i
-000016d0: 6e69 745f 5f29 0572 2200 0000 7223 0000  nit__).r"...r#..
-000016e0: 0072 2400 0000 7213 0000 00da 0d5f 5f63  .r$...r......__c
-000016f0: 6c61 7373 6365 6c6c 5f5f 7208 0000 0072  lasscell__r....r
-00001700: 0800 0000 7254 0000 0072 0900 0000 7252  ....rT...r....rR
-00001710: 0000 0090 0000 0073 0200 0000 0802 7252  .......s......rR
-00001720: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001730: 0000 0000 0200 0000 4000 0000 7314 0000  ........@...s...
-00001740: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
-00001750: 0364 0353 0029 04da 0753 6f66 7453 5049  .d.S.)...SoftSPI
-00001760: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
-00001770: 0001 0000 0043 0000 0073 0400 0000 6400  .....C...s....d.
-00001780: 5300 723b 0000 0072 0800 0000 2904 7212  S.r;...r....).r.
-00001790: 0000 005a 0373 636b 5a04 6d6f 7369 5a04  ...Z.sckZ.mosiZ.
-000017a0: 6d69 736f 7208 0000 0072 0800 0000 7209  misor....r....r.
-000017b0: 0000 0072 1300 0000 9700 0000 7302 0000  ...r........s...
-000017c0: 0000 017a 1053 6f66 7453 5049 2e5f 5f69  ...z.SoftSPI.__i
-000017d0: 6e69 745f 5f4e 2904 7222 0000 0072 2300  nit__N).r"...r#.
-000017e0: 0000 7224 0000 0072 1300 0000 7208 0000  ..r$...r....r...
-000017f0: 0072 0800 0000 7208 0000 0072 0900 0000  .r....r....r....
-00001800: 7257 0000 0096 0000 0073 0200 0000 0801  rW.......s......
-00001810: 7257 0000 0063 0000 0000 0000 0000 0000  rW...c..........
-00001820: 0000 0200 0000 0100 0000 4f00 0000 7304  ..........O...s.
-00001830: 0000 0064 0153 0029 024e 720c 0000 0072  ...d.S.).Nr....r
-00001840: 0800 0000 7205 0000 0072 0800 0000 7208  ....r....r....r.
-00001850: 0000 0072 0900 0000 7237 0000 009b 0000  ...r....r7......
-00001860: 0073 0200 0000 0001 7237 0000 0063 0000  .s......r7...c..
-00001870: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00001880: 0000 4300 0000 730c 0000 0074 0064 0183  ..C...s....t.d..
-00001890: 0101 0064 0253 0029 034e 7a19 5b53 494d  ...d.S.).Nz.[SIM
-000018a0: 5d20 4475 6d6d 7920 6d61 6368 696e 652e  ] Dummy machine.
-000018b0: 7265 7365 7454 a901 da05 7072 696e 7472  resetT....printr
-000018c0: 0800 0000 7208 0000 0072 0800 0000 7209  ....r....r....r.
-000018d0: 0000 00da 0572 6573 6574 9f00 0000 7304  .....reset....s.
-000018e0: 0000 0000 0108 0172 5a00 0000 6300 0000  .......rZ...c...
-000018f0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00001900: 0043 0000 0073 0c00 0000 7400 6401 8301  .C...s....t.d...
-00001910: 0100 6402 5300 2903 4e7a 1e5b 5349 4d5d  ..d.S.).Nz.[SIM]
-00001920: 2044 756d 6d79 206d 6163 6869 6e65 2e73   Dummy machine.s
-00001930: 6f66 745f 7265 7365 7454 7258 0000 0072  oft_resetTrX...r
-00001940: 0800 0000 7208 0000 0072 0800 0000 7209  ....r....r....r.
-00001950: 0000 00da 0a73 6f66 745f 7265 7365 74a4  .....soft_reset.
-00001960: 0000 0073 0400 0000 0001 0801 725b 0000  ...s........r[..
-00001970: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001980: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
-00001990: 0153 0029 024e 7201 0000 0072 0800 0000  .S.).Nr....r....
-000019a0: 7208 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
-000019b0: 0900 0000 da0b 7265 7365 745f 6361 7573  ......reset_caus
-000019c0: 65a9 0000 0073 0200 0000 0001 725c 0000  e....s......r\..
-000019d0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000019e0: 0000 0200 0000 4300 0000 7308 0000 0074  ......C...s....t
-000019f0: 0064 0183 0153 0029 024e 69d2 0400 0029  .d...S.).Ni....)
-00001a00: 01da 0368 6578 7208 0000 0072 0800 0000  ...hexr....r....
-00001a10: 7208 0000 0072 0900 0000 da09 756e 6971  r....r......uniq
-00001a20: 7565 5f69 64ad 0000 0073 0200 0000 0001  ue_id....s......
-00001a30: 725e 0000 0063 0000 0000 0000 0000 0000  r^...c..........
-00001a40: 0000 0000 0000 0200 0000 4300 0000 730c  ..........C...s.
-00001a50: 0000 0074 00a0 01a1 0064 0114 0053 0029  ...t.....d...S.)
-00001a60: 024e 7214 0000 0029 0272 1f00 0000 da07  .Nr....).r......
-00001a70: 7469 6d65 5f6e 7372 0800 0000 7208 0000  time_nsr....r...
-00001a80: 0072 0800 0000 7209 0000 00da 0d74 696d  .r....r......tim
-00001a90: 655f 7075 6c73 655f 7573 b100 0000 7302  e_pulse_us....s.
-00001aa0: 0000 0000 0172 6000 0000 2916 da09 7468  .....r`...)...th
-00001ab0: 7265 6164 696e 6772 0200 0000 721f 0000  readingr....r...
-00001ac0: 0072 1e00 0000 da0b 7369 6d5f 636f 6e73  .r......sim_cons
-00001ad0: 6f6c 6572 0400 0000 da03 7379 7372 0a00  oler......sysr..
-00001ae0: 0000 720b 0000 0072 2500 0000 7230 0000  ..r....r%...r0..
-00001af0: 0072 3200 0000 7239 0000 0072 3f00 0000  .r2...r9...r?...
-00001b00: 7252 0000 0072 5700 0000 7237 0000 0072  rR...rW...r7...r
-00001b10: 5a00 0000 725b 0000 0072 5c00 0000 725e  Z...r[...r\...r^
-00001b20: 0000 0072 6000 0000 7208 0000 0072 0800  ...r`...r....r..
-00001b30: 0000 7208 0000 0072 0900 0000 da08 3c6d  ..r....r......<m
-00001b40: 6f64 756c 653e 0100 0000 7326 0000 000c  odule>....s&....
-00001b50: 0108 0108 010c 0108 0308 050e 1b0e 1d0e  ................
-00001b60: 090e 180e 120e 1810 060e 0508 0408 0508  ................
-00001b70: 0508 0408 04                             .....
+00000f20: 005a 0864 0964 0a84 005a 0964 0b64 0c84  .Z.d.d...Z.d.d..
+00000f30: 005a 0a64 0d64 0e84 005a 0b64 0253 0029  .Z.d.d...Z.d.S.)
+00000f40: 10da 0341 4443 da05 6475 6d6d 794e 6302  ...ADC..dummyNc.
+00000f50: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00000f60: 0000 0043 0000 0073 1400 0000 7c01 7c00  ...C...s....|.|.
+00000f70: 5f00 7c00 a001 a100 7c00 5f02 6400 5300  _.|.....|._.d.S.
+00000f80: a901 4e29 0372 2700 0000 da09 5f41 4443  ..N).r'....._ADC
+00000f90: 5f5f 6765 6e72 2b00 0000 2902 7212 0000  __genr+...).r...
+00000fa0: 0072 2700 0000 7208 0000 0072 0800 0000  .r'...r....r....
+00000fb0: 7209 0000 0072 1300 0000 6b00 0000 7304  r....r....k...s.
+00000fc0: 0000 0000 0106 017a 0c41 4443 2e5f 5f69  .......z.ADC.__i
+00000fd0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00000fe0: 0000 0200 0000 0600 0000 6300 0000 7362  ..........c...sb
+00000ff0: 0000 0074 0064 0164 0264 0383 0344 005d  ...t.d.d.d...D.]
+00001000: 207d 0174 0164 047c 006a 029b 0064 057c   }.t.d.|.j...d.|
+00001010: 019b 009d 0483 0101 007c 0156 0001 0071  .........|.V...q
+00001020: 0c74 0064 0264 0164 0383 0344 005d 207d  .t.d.d.d...D.] }
+00001030: 0174 0164 047c 006a 029b 0064 057c 019b  .t.d.|.j...d.|..
+00001040: 009d 0483 0101 007c 0156 0001 0071 3a71  .......|.V...q:q
+00001050: 0064 0053 0029 064e 7201 0000 0069 ffff  .d.S.).Nr....i..
+00001060: 0000 69f4 0100 007a 0441 4443 287a 0329  ..i....z.ADC(z.)
+00001070: 3a20 2903 da05 7261 6e67 6572 0400 0000  : )...ranger....
+00001080: 7227 0000 0029 0272 1200 0000 da01 6b72  r'...).r......kr
+00001090: 0800 0000 7208 0000 0072 0900 0000 5a05  ....r....r....Z.
+000010a0: 5f5f 6765 6e6f 0000 0073 0c00 0000 0002  __geno...s......
+000010b0: 1001 1601 0801 1001 1601 7a09 4144 432e  ..........z.ADC.
+000010c0: 5f5f 6765 6e63 0100 0000 0000 0000 0000  __genc..........
+000010d0: 0000 0300 0000 0100 0000 4f00 0000 7304  ..........O...s.
+000010e0: 0000 0064 0053 0072 3b00 0000 7208 0000  ...d.S.r;...r...
+000010f0: 0072 2800 0000 7208 0000 0072 0800 0000  .r(...r....r....
+00001100: 7209 0000 00da 0561 7474 656e 7800 0000  r......attenx...
+00001110: 7302 0000 0000 017a 0941 4443 2e61 7474  s......z.ADC.att
+00001120: 656e 6301 0000 0000 0000 0000 0000 0003  enc.............
+00001130: 0000 0001 0000 004f 0000 0073 0400 0000  .......O...s....
+00001140: 6400 5300 723b 0000 0072 0800 0000 7228  d.S.r;...r....r(
+00001150: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
+00001160: 0000 da05 7769 6474 687b 0000 0073 0200  ....width{...s..
+00001170: 0000 0001 7a09 4144 432e 7769 6474 6863  ....z.ADC.widthc
+00001180: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001190: 0200 0000 4300 0000 730a 0000 007c 006a  ....C...s....|.j
+000011a0: 00a0 01a1 0053 0072 3b00 0000 a902 722b  .....S.r;.....r+
+000011b0: 0000 00da 085f 5f6e 6578 745f 5f72 2c00  .....__next__r,.
+000011c0: 0000 7208 0000 0072 0800 0000 7209 0000  ..r....r....r...
+000011d0: 00da 0472 6561 647e 0000 0073 0200 0000  ...read~...s....
+000011e0: 0001 7a08 4144 432e 7265 6164 6301 0000  ..z.ADC.readc...
+000011f0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00001200: 0043 0000 0073 0a00 0000 7c00 6a00 a001  .C...s....|.j...
+00001210: a100 5300 723b 0000 0072 4100 0000 722c  ..S.r;...rA...r,
+00001220: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
+00001230: 0000 da08 7265 6164 5f75 3136 8100 0000  ....read_u16....
+00001240: 7302 0000 0000 017a 0c41 4443 2e72 6561  s......z.ADC.rea
+00001250: 645f 7531 3629 014e 290c 7222 0000 0072  d_u16).N).r"...r
+00001260: 2300 0000 7224 0000 005a 0941 5454 4e5f  #...r$...Z.ATTN_
+00001270: 3131 4442 5a0a 5749 4454 485f 3942 4954  11DBZ.WIDTH_9BIT
+00001280: 5a0b 5749 4454 485f 3130 4249 5472 1300  Z.WIDTH_10BITr..
+00001290: 0000 723c 0000 0072 3f00 0000 7240 0000  ..r<...r?...r@..
+000012a0: 0072 4300 0000 7244 0000 0072 0800 0000  .rC...rD...r....
+000012b0: 7208 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+000012c0: 3900 0000 6600 0000 7312 0000 0008 0104  9...f...s.......
+000012d0: 0104 0104 020a 0408 0908 0308 0308 0372  ...............r
+000012e0: 3900 0000 6300 0000 0000 0000 0000 0000  9...c...........
+000012f0: 0000 0000 0002 0000 0040 0000 0073 3400  .........@...s4.
+00001300: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
+00001310: 5a03 6403 6404 8400 5a04 6405 6406 8400  Z.d.d...Z.d.d...
+00001320: 5a05 6407 6408 8400 5a06 6409 640a 8400  Z.d.d...Z.d.d...
+00001330: 5a07 640b 5300 290c da03 4932 4363 0400  Z.d.S.)...I2Cc..
+00001340: 0000 0000 0000 0000 0000 0400 0000 0200  ................
+00001350: 0000 4300 0000 7316 0000 007c 017c 005f  ..C...s....|.|._
+00001360: 007c 027c 005f 017c 037c 005f 0264 0053  .|.|._.|.|._.d.S
+00001370: 0072 3b00 0000 2903 da03 7363 6cda 0373  .r;...)...scl..s
+00001380: 6461 7237 0000 00a9 0472 1200 0000 7246  dar7.....r....rF
+00001390: 0000 0072 4700 0000 7237 0000 0072 0800  ...rG...r7...r..
+000013a0: 0000 7208 0000 0072 0900 0000 7213 0000  ..r....r....r...
+000013b0: 0087 0000 0073 0600 0000 0001 0601 0601  .....s..........
+000013c0: 7a0c 4932 432e 5f5f 696e 6974 5f5f 6303  z.I2C.__init__c.
+000013d0: 0000 0000 0000 0000 0000 0003 0000 000b  ................
+000013e0: 0000 0043 0000 0073 3000 0000 7400 6401  ...C...s0...t.d.
+000013f0: 7c00 6a01 9b00 6402 7c00 6a02 9b00 6403  |.j...d.|.j...d.
+00001400: 7c00 6a03 9b00 6404 7c01 9b00 6405 7c02  |.j...d.|...d.|.
+00001410: 9b00 9d0a 8301 0100 6406 5300 2907 4e7a  ........d.S.).Nz
+00001420: 135b 4932 4320 7772 6974 6574 6f5d 2073  .[I2C writeto] s
+00001430: 636c 3a20 fa06 2073 6461 3a20 fa07 2066  cl: .. sda: .. f
+00001440: 7265 713a 20fa 0720 6164 6472 3a20 7a08  req: .. addr: z.
+00001450: 2076 616c 7565 3a20 54a9 0472 0400 0000   value: T..r....
+00001460: 7246 0000 0072 4700 0000 7237 0000 0029  rF...rG...r7...)
+00001470: 0372 1200 0000 da07 6164 6472 6573 7372  .r......addressr
+00001480: 2b00 0000 7208 0000 0072 0800 0000 7209  +...r....r....r.
+00001490: 0000 00da 0777 7269 7465 746f 8c00 0000  .....writeto....
+000014a0: 7304 0000 0000 012c 017a 0b49 3243 2e77  s......,.z.I2C.w
+000014b0: 7269 7465 746f 6304 0000 0000 0000 0000  ritetoc.........
+000014c0: 0000 0004 0000 000d 0000 0043 0000 0073  ...........C...s
+000014d0: 3600 0000 7400 6401 7c00 6a01 9b00 6402  6...t.d.|.j...d.
+000014e0: 7c00 6a02 9b00 6403 7c00 6a03 9b00 6404  |.j...d.|.j...d.
+000014f0: 7c01 9b00 6405 7c02 9b00 6406 7c03 9b00  |...d.|...d.|...
+00001500: 9d0c 8301 0100 6407 5300 2908 4e7a 175b  ......d.S.).Nz.[
+00001510: 4932 4320 7772 6974 6574 6f5f 6d65 6d5d  I2C writeto_mem]
+00001520: 2073 636c 3a20 7249 0000 0072 4a00 0000   scl: rI...rJ...
+00001530: 724b 0000 00fa 0620 7265 673a 207a 0620  rK..... reg: z. 
+00001540: 6269 743a 2054 724c 0000 0029 0472 1200  bit: TrL...).r..
+00001550: 0000 724d 0000 00da 0872 6567 6973 7465  ..rM.....registe
+00001560: 72da 0162 7208 0000 0072 0800 0000 7209  r..br....r....r.
+00001570: 0000 00da 0b77 7269 7465 746f 5f6d 656d  .....writeto_mem
+00001580: 9000 0000 7304 0000 0000 0132 017a 0f49  ....s......2.z.I
+00001590: 3243 2e77 7269 7465 746f 5f6d 656d 6303  2C.writeto_memc.
+000015a0: 0000 0000 0000 0000 0000 0003 0000 000b  ................
+000015b0: 0000 0043 0000 0073 3000 0000 7400 6401  ...C...s0...t.d.
+000015c0: 7c00 6a01 9b00 6402 7c00 6a02 9b00 6403  |.j...d.|.j...d.
+000015d0: 7c00 6a03 9b00 6404 7c01 9b00 6405 7c02  |.j...d.|...d.|.
+000015e0: 9b00 9d0a 8301 0100 6406 5300 2907 4e7a  ........d.S.).Nz
+000015f0: 145b 4932 4320 7265 6164 6672 6f6d 5d20  .[I2C readfrom] 
+00001600: 7363 6c3a 2072 4900 0000 724a 0000 0072  scl: rI...rJ...r
+00001610: 4b00 0000 fa07 2062 7974 653a 20f3 0800  K..... byte: ...
+00001620: 0000 3030 3030 3030 3030 724c 0000 0029  ..00000000rL...)
+00001630: 0372 1200 0000 724d 0000 00da 0462 7974  .r....rM.....byt
+00001640: 6572 0800 0000 7208 0000 0072 0900 0000  er....r....r....
+00001650: da08 7265 6164 6672 6f6d 9400 0000 7304  ..readfrom....s.
+00001660: 0000 0000 012c 017a 0c49 3243 2e72 6561  .....,.z.I2C.rea
+00001670: 6466 726f 6d63 0400 0000 0000 0000 0000  dfromc..........
+00001680: 0000 0400 0000 0d00 0000 4300 0000 7336  ..........C...s6
+00001690: 0000 0074 0064 017c 006a 019b 0064 027c  ...t.d.|.j...d.|
+000016a0: 006a 029b 0064 037c 006a 039b 0064 047c  .j...d.|.j...d.|
+000016b0: 019b 0064 057c 029b 0064 067c 039b 009d  ...d.|...d.|....
+000016c0: 0c83 0101 0064 0753 0029 084e 7a18 5b49  .....d.S.).Nz.[I
+000016d0: 3243 2072 6561 6466 726f 6d5f 6d65 6d5d  2C readfrom_mem]
+000016e0: 2073 636c 3a20 7249 0000 0072 4a00 0000   scl: rI...rJ...
+000016f0: 724b 0000 0072 4f00 0000 7253 0000 0072  rK...rO...rS...r
+00001700: 5400 0000 724c 0000 0029 0472 1200 0000  T...rL...).r....
+00001710: 724d 0000 0072 5000 0000 7255 0000 0072  rM...rP...rU...r
+00001720: 0800 0000 7208 0000 0072 0900 0000 da0c  ....r....r......
+00001730: 7265 6164 6672 6f6d 5f6d 656d 9800 0000  readfrom_mem....
+00001740: 7304 0000 0000 0132 017a 1049 3243 2e72  s......2.z.I2C.r
+00001750: 6561 6466 726f 6d5f 6d65 6d4e 2908 7222  eadfrom_memN).r"
+00001760: 0000 0072 2300 0000 7224 0000 0072 1300  ...r#...r$...r..
+00001770: 0000 724e 0000 0072 5200 0000 7256 0000  ..rN...rR...rV..
+00001780: 0072 5700 0000 7208 0000 0072 0800 0000  .rW...r....r....
+00001790: 7208 0000 0072 0900 0000 7245 0000 0085  r....r....rE....
+000017a0: 0000 0073 0a00 0000 0802 0805 0804 0804  ...s............
+000017b0: 0804 7245 0000 0063 0000 0000 0000 0000  ..rE...c........
+000017c0: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+000017d0: 731c 0000 0065 005a 0164 005a 0287 0066  s....e.Z.d.Z...f
+000017e0: 0164 0164 0284 085a 0387 0004 005a 0453  .d.d...Z.....Z.S
+000017f0: 0029 03da 0753 6f66 7449 3243 6304 0000  .)...SoftI2Cc...
+00001800: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00001810: 0003 0000 0073 1400 0000 7400 8300 a001  .....s....t.....
+00001820: 7c01 7c02 7c03 a103 0100 6400 5300 723b  |.|.|.....d.S.r;
+00001830: 0000 0029 02da 0573 7570 6572 7213 0000  ...)...superr...
+00001840: 0072 4800 0000 a901 da09 5f5f 636c 6173  .rH.......__clas
+00001850: 735f 5f72 0800 0000 7209 0000 0072 1300  s__r....r....r..
+00001860: 0000 9f00 0000 7302 0000 0000 017a 1053  ......s......z.S
+00001870: 6f66 7449 3243 2e5f 5f69 6e69 745f 5f29  oftI2C.__init__)
+00001880: 0572 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
+00001890: 7213 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
+000018a0: 6c6c 5f5f 7208 0000 0072 0800 0000 725a  ll__r....r....rZ
+000018b0: 0000 0072 0900 0000 7258 0000 009d 0000  ...r....rX......
+000018c0: 0073 0200 0000 0802 7258 0000 0063 0000  .s......rX...c..
+000018d0: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+000018e0: 0000 4000 0000 7314 0000 0065 005a 0164  ..@...s....e.Z.d
+000018f0: 005a 0264 0164 0284 005a 0364 0353 0029  .Z.d.d...Z.d.S.)
+00001900: 04da 0753 6f66 7453 5049 6304 0000 0000  ...SoftSPIc.....
+00001910: 0000 0000 0000 0004 0000 0001 0000 0043  ...............C
+00001920: 0000 0073 0400 0000 6400 5300 723b 0000  ...s....d.S.r;..
+00001930: 0072 0800 0000 2904 7212 0000 005a 0373  .r....).r....Z.s
+00001940: 636b 5a04 6d6f 7369 5a04 6d69 736f 7208  ckZ.mosiZ.misor.
+00001950: 0000 0072 0800 0000 7209 0000 0072 1300  ...r....r....r..
+00001960: 0000 a400 0000 7302 0000 0000 017a 1053  ......s......z.S
+00001970: 6f66 7453 5049 2e5f 5f69 6e69 745f 5f4e  oftSPI.__init__N
+00001980: 2904 7222 0000 0072 2300 0000 7224 0000  ).r"...r#...r$..
+00001990: 0072 1300 0000 7208 0000 0072 0800 0000  .r....r....r....
+000019a0: 7208 0000 0072 0900 0000 725d 0000 00a3  r....r....r]....
+000019b0: 0000 0073 0200 0000 0801 725d 0000 0063  ...s......r]...c
+000019c0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+000019d0: 0100 0000 4f00 0000 7304 0000 0064 0153  ....O...s....d.S
+000019e0: 0029 024e 720c 0000 0072 0800 0000 7205  .).Nr....r....r.
+000019f0: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
+00001a00: 0000 7237 0000 00a8 0000 0073 0200 0000  ..r7.......s....
+00001a10: 0001 7237 0000 0063 0000 0000 0000 0000  ..r7...c........
+00001a20: 0000 0000 0000 0000 0200 0000 4300 0000  ............C...
+00001a30: 730c 0000 0074 0064 0183 0101 0064 0253  s....t.d.....d.S
+00001a40: 0029 034e 7a19 5b53 494d 5d20 4475 6d6d  .).Nz.[SIM] Dumm
+00001a50: 7920 6d61 6368 696e 652e 7265 7365 7454  y machine.resetT
+00001a60: a901 da05 7072 696e 7472 0800 0000 7208  ....printr....r.
+00001a70: 0000 0072 0800 0000 7209 0000 00da 0572  ...r....r......r
+00001a80: 6573 6574 ac00 0000 7304 0000 0000 0108  eset....s.......
+00001a90: 0172 6000 0000 6300 0000 0000 0000 0000  .r`...c.........
+00001aa0: 0000 0000 0000 0002 0000 0043 0000 0073  ...........C...s
+00001ab0: 0c00 0000 7400 6401 8301 0100 6402 5300  ....t.d.....d.S.
+00001ac0: 2903 4e7a 1e5b 5349 4d5d 2044 756d 6d79  ).Nz.[SIM] Dummy
+00001ad0: 206d 6163 6869 6e65 2e73 6f66 745f 7265   machine.soft_re
+00001ae0: 7365 7454 725e 0000 0072 0800 0000 7208  setTr^...r....r.
+00001af0: 0000 0072 0800 0000 7209 0000 00da 0a73  ...r....r......s
+00001b00: 6f66 745f 7265 7365 74b1 0000 0073 0400  oft_reset....s..
+00001b10: 0000 0001 0801 7261 0000 0063 0000 0000  ......ra...c....
+00001b20: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00001b30: 4300 0000 7304 0000 0064 0153 0029 024e  C...s....d.S.).N
+00001b40: 7201 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
+00001b50: 0800 0000 7208 0000 0072 0900 0000 da0b  ....r....r......
+00001b60: 7265 7365 745f 6361 7573 65b6 0000 0073  reset_cause....s
+00001b70: 0200 0000 0001 7262 0000 0063 0000 0000  ......rb...c....
+00001b80: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00001b90: 4300 0000 7308 0000 0074 0064 0183 0153  C...s....t.d...S
+00001ba0: 0029 024e 69d2 0400 0029 01da 0368 6578  .).Ni....)...hex
+00001bb0: 7208 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
+00001bc0: 0900 0000 da09 756e 6971 7565 5f69 64ba  ......unique_id.
+00001bd0: 0000 0073 0200 0000 0001 7264 0000 0063  ...s......rd...c
+00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bf0: 0200 0000 4300 0000 730c 0000 0074 00a0  ....C...s....t..
+00001c00: 01a1 0064 0114 0053 0029 024e 7214 0000  ...d...S.).Nr...
+00001c10: 0029 0272 1f00 0000 da07 7469 6d65 5f6e  .).r......time_n
+00001c20: 7372 0800 0000 7208 0000 0072 0800 0000  sr....r....r....
+00001c30: 7209 0000 00da 0d74 696d 655f 7075 6c73  r......time_puls
+00001c40: 655f 7573 be00 0000 7302 0000 0000 0172  e_us....s......r
+00001c50: 6600 0000 2916 da09 7468 7265 6164 696e  f...)...threadin
+00001c60: 6772 0200 0000 721f 0000 0072 1e00 0000  gr....r....r....
+00001c70: da0b 7369 6d5f 636f 6e73 6f6c 6572 0400  ..sim_consoler..
+00001c80: 0000 da03 7379 7372 0a00 0000 720b 0000  ....sysr....r...
+00001c90: 0072 2500 0000 7230 0000 0072 3200 0000  .r%...r0...r2...
+00001ca0: 7239 0000 0072 4500 0000 7258 0000 0072  r9...rE...rX...r
+00001cb0: 5d00 0000 7237 0000 0072 6000 0000 7261  ]...r7...r`...ra
+00001cc0: 0000 0072 6200 0000 7264 0000 0072 6600  ...rb...rd...rf.
+00001cd0: 0000 7208 0000 0072 0800 0000 7208 0000  ..r....r....r...
+00001ce0: 0072 0900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001cf0: 0100 0000 7326 0000 000c 0108 0108 010c  ....s&..........
+00001d00: 0108 0308 050e 1b0e 1d0e 090e 180e 1f0e  ................
+00001d10: 1810 060e 0508 0408 0508 0508 0408 04    ...............
```

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/machine.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,24 +101,37 @@
 
 class ADC:
     ATTN_11DB = 'dummy'
     WIDTH_9BIT = 'dummy'
     WIDTH_10BIT = 'dummy'
 
     def __init__(self, pin=None):
-        pass
+        self.pin = pin
+        self.value = self.__gen()
+
+    def __gen(self):
+        while True:
+            for k in range(0, 65535, 500):
+                console(f"ADC({self.pin}): {k}")
+                yield k
+            for k in range(65535, 0, 500):
+                console(f"ADC({self.pin}): {k}")
+                yield k
 
     def atten(self, *args, **kwargs):
         pass
 
     def width(self, *args, **kwargs):
         pass
 
     def read(self):
-        return 420
+        return self.value.__next__()
+
+    def read_u16(self):
+        return self.value.__next__()
 
 
 class I2C:
 
     def __init__(self, scl, sda, freq):
         self.scl = scl
         self.sda = sda
```

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/simulator.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.21.2/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/socketClient.py` & `micrOSDevToolKit-1.21.2/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Common.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Debug.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6366 6770 7574 001a 436f 6e66 6967 4861  cfgput..ConfigHa
 00000050: 6e64 6c65 7200 1865 7865 635f 6c6d 5f63  ndler..exec_lm_c
 00000060: 6f72 6500 1654 6173 6b4d 616e 6167 6572  ore..TaskManager
 00000070: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 00000080: 1465 7272 6c6f 675f 6164 6400 0a44 6562  .errlog_add..Deb
 00000090: 7567 000a 7265 7365 7400 1473 6f66 745f  ug..reset..soft_
 000000a0: 7265 7365 7400 0e6d 6163 6869 6e65 000a  reset..machine..
-000000b0: 5368 656c 6c00 1031 2e32 312e 302d 3100  Shell..1.21.0-1.
+000000b0: 5368 656c 6c00 1031 2e32 312e 302d 3300  Shell..1.21.0-3.
 000000c0: 230e 6d73 675f 6f62 6a00 0c64 6576 6669  #.msg_obj..devfi
 000000d0: 6400 105f 5f64 6576 6669 6400 0861 7574  d..__devfid..aut
 000000e0: 6800 165f 5f61 7574 685f 6d6f 6465 000a  h..__auth_mode..
 000000f0: 6877 7569 6400 0e5f 5f68 7775 6964 0012  hwuid..__hwuid..
 00000100: 5f5f 6175 7468 5f6f 6b00 165f 5f63 6f6e  __auth_ok..__con
 00000110: 665f 6d6f 6465 000e 7665 7273 696f 6e00  f_mode..version.
 00000120: 1c4d 4943 524f 535f 5645 5253 494f 4e00  .MICROS_VERSION.
```

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterruptHandler.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/InterruptHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_aht10.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_aht10.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_lmpacman.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_lmpacman.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Network.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Notify.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/Time.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/urequests.mpy` & `micrOSDevToolKit-1.21.2/toolkit/workspace/precompiled/urequests.mpy`

 * *Files identical despite different names*

