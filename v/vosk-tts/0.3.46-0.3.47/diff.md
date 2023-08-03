# Comparing `tmp/vosk_tts-0.3.46-py3-none-any.whl.zip` & `tmp/vosk_tts-0.3.47-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10268 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-07 00:49 vosk_tts/__init__.py
--rw-r--r--  2.0 unx     1769 b- defN 23-Apr-07 00:55 vosk_tts/cli.py
--rw-r--r--  2.0 unx     2400 b- defN 23-Apr-07 00:49 vosk_tts/g2p.py
--rw-r--r--  2.0 unx     5586 b- defN 23-Apr-07 01:32 vosk_tts/model.py
--rw-r--r--  2.0 unx     1740 b- defN 23-Apr-07 00:49 vosk_tts/synth.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-07 01:34 vosk_tts-0.3.46.dist-info/LICENSE
--rw-r--r--  2.0 unx      858 b- defN 23-Apr-07 01:34 vosk_tts-0.3.46.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 01:34 vosk_tts-0.3.46.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Apr-07 01:34 vosk_tts-0.3.46.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-07 01:34 vosk_tts-0.3.46.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      858 b- defN 23-Apr-07 01:34 vosk_tts-0.3.46.dist-info/RECORD
-11 files, 24717 bytes uncompressed, 8820 bytes compressed:  64.3%
+Zip file size: 10550 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       42 b- defN 23-May-14 18:54 vosk_tts/__init__.py
+-rw-r--r--  2.0 unx     1769 b- defN 23-May-14 18:54 vosk_tts/cli.py
+-rw-r--r--  2.0 unx     2400 b- defN 23-May-14 18:54 vosk_tts/g2p.py
+-rw-r--r--  2.0 unx     5586 b- defN 23-May-14 18:54 vosk_tts/model.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-Aug-03 08:41 vosk_tts/synth.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-03 08:42 vosk_tts-0.3.47.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1900 b- defN 23-Aug-03 08:42 vosk_tts-0.3.47.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 08:42 vosk_tts-0.3.47.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Aug-03 08:42 vosk_tts-0.3.47.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Aug-03 08:42 vosk_tts-0.3.47.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      860 b- defN 23-Aug-03 08:42 vosk_tts-0.3.47.dist-info/RECORD
+11 files, 25870 bytes uncompressed, 9102 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: vosk_tts/model.py
 Comment: 
 
 Filename: vosk_tts/synth.py
 Comment: 
 
-Filename: vosk_tts-0.3.46.dist-info/LICENSE
+Filename: vosk_tts-0.3.47.dist-info/LICENSE
 Comment: 
 
-Filename: vosk_tts-0.3.46.dist-info/METADATA
+Filename: vosk_tts-0.3.47.dist-info/METADATA
 Comment: 
 
-Filename: vosk_tts-0.3.46.dist-info/WHEEL
+Filename: vosk_tts-0.3.47.dist-info/WHEEL
 Comment: 
 
-Filename: vosk_tts-0.3.46.dist-info/entry_points.txt
+Filename: vosk_tts-0.3.47.dist-info/entry_points.txt
 Comment: 
 
-Filename: vosk_tts-0.3.46.dist-info/top_level.txt
+Filename: vosk_tts-0.3.47.dist-info/top_level.txt
 Comment: 
 
-Filename: vosk_tts-0.3.46.dist-info/RECORD
+Filename: vosk_tts-0.3.47.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vosk_tts/__init__.py

```diff
@@ -0,0 +1,3 @@
+00000000: 6672 6f6d 202e 6d6f 6465 6c20 696d 706f  from .model impo
+00000010: 7274 202a 0a66 726f 6d20 2e73 796e 7468  rt *.from .synth
+00000020: 2069 6d70 6f72 7420 2a0a                  import *.
```

## vosk_tts/synth.py

```diff
@@ -14,42 +14,46 @@
     ) -> np.ndarray:
         """Normalize audio and convert to int16 range"""
         audio_norm = audio * (max_wav_value / max(0.01, np.max(np.abs(audio))))
         audio_norm = np.clip(audio_norm, -max_wav_value, max_wav_value)
         audio_norm = audio_norm.astype("int16")
         return audio_norm
 
-    def synth(self, text, oname):
+    def synth_audio(self, text):
 
         phoneme_ids = self.model.g2p(text)
 
         text = np.expand_dims(np.array(phoneme_ids, dtype=np.int64), 0)
         text_lengths = np.array([text.shape[1]], dtype=np.int64)
         scales = np.array([0.667, 1.0, 0.8], dtype=np.float32)
 
         start_time = time.perf_counter()
         audio = self.model.onnx.run(
             None,
             {
                 "input": text,
                 "input_lengths": text_lengths,
                 "scales": scales,
-                "sid": None
             },
         )[0].squeeze((0, 1))
 
         audio = self.audio_float_to_int16(audio.squeeze())
         end_time = time.perf_counter()
 
         audio_duration_sec = audio.shape[-1] / 22050
         infer_sec = end_time - start_time
         real_time_factor = (
             infer_sec / audio_duration_sec if audio_duration_sec > 0 else 0.0
         )
 
         print("Real-time factor: %0.2f (infer=%0.2f sec, audio=%0.2f sec)" % (real_time_factor, infer_sec, audio_duration_sec))
+        return audio
+
+    def synth(self, text, oname):
+
+        audio = self.synth_audio(text)
 
         with wave.open(oname, "w") as f:
             f.setnchannels(1)
             f.setsampwidth(2)
             f.setframerate(22050)
             f.writeframes(audio.tobytes())
```

## Comparing `vosk_tts-0.3.46.dist-info/LICENSE` & `vosk_tts-0.3.47.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vosk_tts-0.3.46.dist-info/RECORD` & `vosk_tts-0.3.47.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-vosk_tts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+vosk_tts/__init__.py,sha256=OVQsWlFF68si4rKJFtCcwlX--LYc7CSCOn1Kg8Uibvg,42
 vosk_tts/cli.py,sha256=38-XjpiIuAw-9ja0W3XadRV-dI-p-GlfypdfZm-A8Pg,1769
 vosk_tts/g2p.py,sha256=u1aKRW-G3Cwmtviy3pDNePTSkNvemNKw-tQTankT9lQ,2400
 vosk_tts/model.py,sha256=pa2dDNyNert6_pyKI6ouCsY4Rqze33dvQokecVJTpfw,5586
-vosk_tts/synth.py,sha256=K1VXd4D-BgHWUh-rMJh_kIbz-X0OagjNIBvdWlx-QI4,1740
-vosk_tts-0.3.46.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-vosk_tts-0.3.46.dist-info/METADATA,sha256=maCVyZ6vyxFKisypajNrAPtXer-bSnlnrklWn9k6J6c,858
-vosk_tts-0.3.46.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vosk_tts-0.3.46.dist-info/entry_points.txt,sha256=K-WoVxWxiIH_T7nNvqtPI5ycsSwtaNCvQXq6_r9dvlI,48
-vosk_tts-0.3.46.dist-info/top_level.txt,sha256=FaXgnbIzrcWwBJp-TwQ-5Dxee0iOHHgdNsxrdg6CQww,9
-vosk_tts-0.3.46.dist-info/RECORD,,
+vosk_tts/synth.py,sha256=_RJ8PwVbx4Tb5F_Wu8R4wzf3KE83oRJ0608C_jLdy-o,1807
+vosk_tts-0.3.47.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+vosk_tts-0.3.47.dist-info/METADATA,sha256=XzQLsYaxrX0CR49N3YGe5dMYgikhUoOTVQ4WHUP5r60,1900
+vosk_tts-0.3.47.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+vosk_tts-0.3.47.dist-info/entry_points.txt,sha256=K-WoVxWxiIH_T7nNvqtPI5ycsSwtaNCvQXq6_r9dvlI,48
+vosk_tts-0.3.47.dist-info/top_level.txt,sha256=FaXgnbIzrcWwBJp-TwQ-5Dxee0iOHHgdNsxrdg6CQww,9
+vosk_tts-0.3.47.dist-info/RECORD,,
```

