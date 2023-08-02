# Comparing `tmp/RUTTS-0.0.1.tar.gz` & `tmp/RUTTS-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RUTTS-0.0.1.tar", last modified: Thu Jul 27 22:49:48 2023, max compression
+gzip compressed data, was "RUTTS-0.1.0.tar", last modified: Wed Aug  2 22:33:50 2023, max compression
```

## Comparing `RUTTS-0.0.1.tar` & `RUTTS-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-07-27 22:49:48.328230 RUTTS-0.0.1/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     1057 2023-07-27 22:12:45.000000 RUTTS-0.0.1/LICENSE.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-07-27 22:49:48.327996 RUTTS-0.0.1/PKG-INFO
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-07-27 22:49:48.325178 RUTTS-0.0.1/RUTTS/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       27 2023-07-27 21:39:42.000000 RUTTS-0.0.1/RUTTS/__init__.py
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     2886 2023-07-27 21:54:29.000000 RUTTS-0.0.1/RUTTS/infer_onnx.py
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-07-27 22:49:48.327463 RUTTS-0.0.1/RUTTS.egg-info/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-07-27 22:49:48.000000 RUTTS-0.0.1/RUTTS.egg-info/PKG-INFO
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      202 2023-07-27 22:49:48.000000 RUTTS-0.0.1/RUTTS.egg-info/SOURCES.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        1 2023-07-27 22:49:48.000000 RUTTS-0.0.1/RUTTS.egg-info/dependency_links.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       57 2023-07-27 22:49:48.000000 RUTTS-0.0.1/RUTTS.egg-info/requires.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        6 2023-07-27 22:49:48.000000 RUTTS-0.0.1/RUTTS.egg-info/top_level.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       38 2023-07-27 22:49:48.328311 RUTTS-0.0.1/setup.cfg
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      719 2023-07-27 22:48:52.000000 RUTTS-0.0.1/setup.py
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-02 22:33:50.601159 RUTTS-0.1.0/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     1057 2023-07-27 22:12:45.000000 RUTTS-0.1.0/LICENSE.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-02 22:33:50.600914 RUTTS-0.1.0/PKG-INFO
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-02 22:33:50.597908 RUTTS-0.1.0/RUTTS/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       27 2023-07-27 21:39:42.000000 RUTTS-0.1.0/RUTTS/__init__.py
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     3383 2023-08-02 22:30:58.000000 RUTTS-0.1.0/RUTTS/infer_onnx.py
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-02 22:33:50.600427 RUTTS-0.1.0/RUTTS.egg-info/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-02 22:33:50.000000 RUTTS-0.1.0/RUTTS.egg-info/PKG-INFO
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      202 2023-08-02 22:33:50.000000 RUTTS-0.1.0/RUTTS.egg-info/SOURCES.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        1 2023-08-02 22:33:50.000000 RUTTS-0.1.0/RUTTS.egg-info/dependency_links.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       66 2023-08-02 22:33:50.000000 RUTTS-0.1.0/RUTTS.egg-info/requires.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        6 2023-08-02 22:33:50.000000 RUTTS-0.1.0/RUTTS.egg-info/top_level.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       38 2023-08-02 22:33:50.601245 RUTTS-0.1.0/setup.cfg
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      731 2023-08-02 22:33:44.000000 RUTTS-0.1.0/setup.py
```

### Comparing `RUTTS-0.0.1/LICENSE.txt` & `RUTTS-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RUTTS-0.0.1/PKG-INFO` & `RUTTS-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RUTTS
-Version: 0.0.1
+Version: 0.1.0
 Summary: russian text to speech
 Home-page: https://github.com/Tera2Space/RUTTS
 Author: Tera Space
 Author-email: tera2space@gmail.com
 License: MIT
 Keywords: tts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RUTTS-0.0.1/RUTTS/infer_onnx.py` & `RUTTS-0.1.0/RUTTS/infer_onnx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,89 @@
 import scipy.io.wavfile
 import os
 import re
-from phonemizer import phonemize
 import sounddevice as sd
 import onnxruntime
 import numpy as np
 from huggingface_hub import snapshot_download
+from gruut import sentences
+import time
 
 class TTS:
-    def __init__(self, model_name: str, save_path: str = "./model") -> None:
+    def __init__(self, model_name: str, save_path: str = "./model", add_time_to_end: float = 0.8) -> None:
         if not os.path.exists(save_path):
             os.mkdir(save_path)
         
         model_dir = os.path.join(save_path, model_name)
         
         if not os.path.exists(model_dir):
-            snapshot_download(repo_id=model_name, allow_patterns=["*.txt", "*.onnx"], 
-                              local_dir=model_dir
-                              )
+            snapshot_download(repo_id=model_name, 
+                              allow_patterns=["*.txt", "*.onnx"], 
+                              local_dir=model_dir,
+                              local_dir_use_symlinks=False
+                            )
         
         sess_options = onnxruntime.SessionOptions()
         self.model = onnxruntime.InferenceSession(os.path.join(model_dir, "exported/model.onnx"), sess_options=sess_options)
         
         with open(os.path.join(model_dir, "exported/vocab.txt"), "r", encoding="utf-8") as vocab_file:
             self.symbols = vocab_file.read().split("\n")
+            self.symbols = list(map(chr, list(map(int, self.symbols))))
         
         self.symbol_to_id = {s: i for i, s in enumerate(self.symbols)}
-    
+        self.add_time_to_end = add_time_to_end
+
+        
     def _ru_phonems(self, text: str) -> str:
-        '''clean text'''
         text = text.lower()
-        phonemes = phonemize(text, language='ru', backend='espeak', strip=True, preserve_punctuation=True, with_stress=True)
-        phonemes = re.sub(re.compile(r'\s+'), ' ', phonemes)
+        phonemes = ""
+        for sent in sentences(text, lang="ru"):
+            for word in sent:
+                if word.phonemes:
+                    phonemes += "".join(word.phonemes)
+        phonemes = re.sub(re.compile(r'\s+'), ' ', phonemes).lstrip().rstrip()
         return phonemes
     
+    
     def _text_to_sequence(self, text: str) -> list[int]:
         '''convert text to seq'''
         sequence = []
         clean_text = self._ru_phonems(text)
         for symbol in clean_text:
             symbol_id = self.symbol_to_id[symbol]
             sequence += [symbol_id]
         return sequence
     
+    
     def _intersperse(self, lst, item):
         result = [item] * (len(lst) * 2 + 1)
         result[1::2] = lst
         return result
     
+    
     def _get_text(self, text: str) -> list[int]:
         text_norm = self._text_to_sequence(text)
         text_norm = self._intersperse(text_norm, 0)
         return text_norm
     
+    
     def save_wav(self, audio, path:str):
         '''save audio to wav'''
         scipy.io.wavfile.write(path, 22050, audio)
     
+    
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
+    
     
     def __call__(self, text: str, play = False):
         phoneme_ids = self._get_text(text)
         text = np.expand_dims(np.array(phoneme_ids, dtype=np.int64), 0)
         text_lengths = np.array([text.shape[1]], dtype=np.int64)
         scales = np.array(
             [0.667, 1, 0.8],
```

### Comparing `RUTTS-0.0.1/RUTTS.egg-info/PKG-INFO` & `RUTTS-0.1.0/RUTTS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RUTTS
-Version: 0.0.1
+Version: 0.1.0
 Summary: russian text to speech
 Home-page: https://github.com/Tera2Space/RUTTS
 Author: Tera Space
 Author-email: tera2space@gmail.com
 License: MIT
 Keywords: tts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RUTTS-0.0.1/setup.py` & `RUTTS-0.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,18 +8,18 @@
   'Operating System :: MacOS',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='RUTTS',
-  version='0.0.1',
+  version='0.1.0',
   description='russian text to speech',
   url='https://github.com/Tera2Space/RUTTS',  
   author='Tera Space',
   author_email='tera2space@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='tts', 
   packages=find_packages(),
-  install_requires=['scipy', 'phonemizer', 'sounddevice', 'onnxruntime', 'huggingface-hub'] 
+  install_requires=['scipy', 'gruut', 'gruut-lang-ru', 'sounddevice', 'onnxruntime', 'huggingface-hub'] 
 )
```

