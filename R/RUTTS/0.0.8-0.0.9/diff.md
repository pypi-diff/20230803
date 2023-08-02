# Comparing `tmp/RUTTS-0.0.8.tar.gz` & `tmp/RUTTS-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RUTTS-0.0.8.tar", last modified: Tue Aug  1 19:38:00 2023, max compression
+gzip compressed data, was "RUTTS-0.0.9.tar", last modified: Wed Aug  2 22:29:08 2023, max compression
```

## Comparing `RUTTS-0.0.8.tar` & `RUTTS-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-01 19:38:00.686061 RUTTS-0.0.8/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     1057 2023-07-27 22:12:45.000000 RUTTS-0.0.8/LICENSE.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-01 19:38:00.685835 RUTTS-0.0.8/PKG-INFO
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-01 19:38:00.682841 RUTTS-0.0.8/RUTTS/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       27 2023-07-27 21:39:42.000000 RUTTS-0.0.8/RUTTS/__init__.py
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     3134 2023-08-01 19:32:45.000000 RUTTS-0.0.8/RUTTS/infer_onnx.py
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-01 19:38:00.685331 RUTTS-0.0.8/RUTTS.egg-info/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-01 19:38:00.000000 RUTTS-0.0.8/RUTTS.egg-info/PKG-INFO
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      202 2023-08-01 19:38:00.000000 RUTTS-0.0.8/RUTTS.egg-info/SOURCES.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        1 2023-08-01 19:38:00.000000 RUTTS-0.0.8/RUTTS.egg-info/dependency_links.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       66 2023-08-01 19:38:00.000000 RUTTS-0.0.8/RUTTS.egg-info/requires.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        6 2023-08-01 19:38:00.000000 RUTTS-0.0.8/RUTTS.egg-info/top_level.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       38 2023-08-01 19:38:00.686142 RUTTS-0.0.8/setup.cfg
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      731 2023-08-01 19:37:17.000000 RUTTS-0.0.8/setup.py
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-02 22:29:08.780091 RUTTS-0.0.9/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     1057 2023-07-27 22:12:45.000000 RUTTS-0.0.9/LICENSE.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-02 22:29:08.779754 RUTTS-0.0.9/PKG-INFO
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-02 22:29:08.776319 RUTTS-0.0.9/RUTTS/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       27 2023-07-27 21:39:42.000000 RUTTS-0.0.9/RUTTS/__init__.py
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     3306 2023-08-02 22:26:34.000000 RUTTS-0.0.9/RUTTS/infer_onnx.py
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-02 22:29:08.779093 RUTTS-0.0.9/RUTTS.egg-info/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-02 22:29:08.000000 RUTTS-0.0.9/RUTTS.egg-info/PKG-INFO
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      202 2023-08-02 22:29:08.000000 RUTTS-0.0.9/RUTTS.egg-info/SOURCES.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        1 2023-08-02 22:29:08.000000 RUTTS-0.0.9/RUTTS.egg-info/dependency_links.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       66 2023-08-02 22:29:08.000000 RUTTS-0.0.9/RUTTS.egg-info/requires.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        6 2023-08-02 22:29:08.000000 RUTTS-0.0.9/RUTTS.egg-info/top_level.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       38 2023-08-02 22:29:08.780177 RUTTS-0.0.9/setup.cfg
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      731 2023-08-02 22:28:31.000000 RUTTS-0.0.9/setup.py
```

### Comparing `RUTTS-0.0.8/LICENSE.txt` & `RUTTS-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RUTTS-0.0.8/PKG-INFO` & `RUTTS-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RUTTS
-Version: 0.0.8
+Version: 0.0.9
 Summary: russian text to speech
 Home-page: https://github.com/Tera2Space/RUTTS
 Author: Tera Space
 Author-email: tera2space@gmail.com
 License: MIT
 Keywords: tts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RUTTS-0.0.8/RUTTS/infer_onnx.py` & `RUTTS-0.0.9/RUTTS/infer_onnx.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import re
 import sounddevice as sd
 import onnxruntime
 import numpy as np
 from huggingface_hub import snapshot_download
 from gruut import sentences
+import time
 
 class TTS:
     def __init__(self, model_name: str, save_path: str = "./model") -> None:
         if not os.path.exists(save_path):
             os.mkdir(save_path)
         
         model_dir = os.path.join(save_path, model_name)
@@ -66,16 +67,21 @@
     
     def save_wav(self, audio, path:str):
         '''save audio to wav'''
         scipy.io.wavfile.write(path, 22050, audio)
     
     
     def play_audio(self, audio):
-        '''play audio'''
-        sd.play(audio, 22050, blocking=True)
+        # sd.play(audio, 22050, blocking=True) # GOOD FOR LINUX but not for Windows :(
+        sd.play(audio, 22050)
+        time.sleep(
+            (len(audio)/22050) 
+            +
+            self.add_time_to_end
+            )
     
     
     def __call__(self, text: str, play = False):
         phoneme_ids = self._get_text(text)
         text = np.expand_dims(np.array(phoneme_ids, dtype=np.int64), 0)
         text_lengths = np.array([text.shape[1]], dtype=np.int64)
         scales = np.array(
```

### Comparing `RUTTS-0.0.8/RUTTS.egg-info/PKG-INFO` & `RUTTS-0.0.9/RUTTS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RUTTS
-Version: 0.0.8
+Version: 0.0.9
 Summary: russian text to speech
 Home-page: https://github.com/Tera2Space/RUTTS
 Author: Tera Space
 Author-email: tera2space@gmail.com
 License: MIT
 Keywords: tts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RUTTS-0.0.8/setup.py` & `RUTTS-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   'Operating System :: MacOS',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='RUTTS',
-  version='0.0.8',
+  version='0.0.9',
   description='russian text to speech',
   url='https://github.com/Tera2Space/RUTTS',  
   author='Tera Space',
   author_email='tera2space@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='tts',
```

