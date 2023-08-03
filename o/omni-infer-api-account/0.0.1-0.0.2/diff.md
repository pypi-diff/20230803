# Comparing `tmp/omni_infer_api_account-0.0.1-py3-none-any.whl.zip` & `tmp/omni_infer_api_account-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8677 bytes, number of entries: 10
+Zip file size: 8701 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Aug-01 13:09 omniinfer_account/__init__.py
 -rw-rw-rw-  2.0 fat    14108 b- defN 23-Aug-02 11:51 omniinfer_account/account.py
 -rw-rw-rw-  2.0 fat      365 b- defN 23-Aug-02 11:58 omniinfer_account/config.py
 -rw-rw-rw-  2.0 fat     3266 b- defN 23-Aug-01 08:30 omniinfer_account/data.py
 -rw-rw-rw-  2.0 fat      184 b- defN 23-Jul-31 09:25 omniinfer_account/error.py
--rw-rw-rw-  2.0 fat    14606 b- defN 23-Aug-02 12:05 omniinfer_account/system.py
--rw-rw-rw-  2.0 fat      239 b- defN 23-Aug-02 12:07 omni_infer_api_account-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-02 12:07 omni_infer_api_account-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-02 12:07 omni_infer_api_account-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      859 b- defN 23-Aug-02 12:07 omni_infer_api_account-0.0.1.dist-info/RECORD
-10 files, 33818 bytes uncompressed, 7195 bytes compressed:  78.7%
+-rw-rw-rw-  2.0 fat    14803 b- defN 23-Aug-02 12:50 omniinfer_account/system.py
+-rw-rw-rw-  2.0 fat      239 b- defN 23-Aug-02 13:29 omni_infer_api_account-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-02 13:29 omni_infer_api_account-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-02 13:29 omni_infer_api_account-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      859 b- defN 23-Aug-02 13:29 omni_infer_api_account-0.0.2.dist-info/RECORD
+10 files, 34015 bytes uncompressed, 7219 bytes compressed:  78.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: omniinfer_account/error.py
 Comment: 
 
 Filename: omniinfer_account/system.py
 Comment: 
 
-Filename: omni_infer_api_account-0.0.1.dist-info/METADATA
+Filename: omni_infer_api_account-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: omni_infer_api_account-0.0.1.dist-info/WHEEL
+Filename: omni_infer_api_account-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: omni_infer_api_account-0.0.1.dist-info/top_level.txt
+Filename: omni_infer_api_account-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: omni_infer_api_account-0.0.1.dist-info/RECORD
+Filename: omni_infer_api_account-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omniinfer_account/system.py

```diff
@@ -62,14 +62,17 @@
         i = 0
         while not self.update_stop:
             time.sleep(1)
             i += 1
             if i >= config.update_interval:
                 logging.info("Update: update")
                 omniifer_api.update()
+                logging.info("Update: backup account data")
+                for key in self.account_list:
+                    self.account_list[key].save(os.path.join(self.path, key + ".json"))
                 i = 0
         logging.info("Update: stop")
         self.update_stop = False
 
     # resolve task thread, auto start after __init__, auto stop before stopping
     def task_resolve(self):
         logging.info("Task: Started task resolve")
```

## Comparing `omni_infer_api_account-0.0.1.dist-info/RECORD` & `omni_infer_api_account-0.0.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 omniinfer_account/__init__.py,sha256=8xVBC5zKvhEXnKS-yvAICUvJoUgdJbScMAuK4SDlYJ8,81
 omniinfer_account/account.py,sha256=ohlq9_-DXhVsx00e4g1tnqzrc3pGzJS4eHkxuibO1CE,14108
 omniinfer_account/config.py,sha256=XBxhdj5B8-TxcaZhUdAe3xu8Ruxzb64O20WE_kZKupw,365
 omniinfer_account/data.py,sha256=T4EJ3ltamEa4tOVPz9phVH0GD5DEQYNg9KVJdwv9-DI,3266
 omniinfer_account/error.py,sha256=SN5KyCv7ekz0aatzSMfq5tF60SEUckt2-7uyyl4VdW0,184
-omniinfer_account/system.py,sha256=iYRxfIEObwD8W2WuhuqidfOo44cZu7Uolia-sQmkV3Q,14606
-omni_infer_api_account-0.0.1.dist-info/METADATA,sha256=Mg4YJSyyPA1tZ3Eyxo3AV9MYFSUoG9HjlmPAKMvhnhw,239
-omni_infer_api_account-0.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-omni_infer_api_account-0.0.1.dist-info/top_level.txt,sha256=VYfZEk7HEk2argDpUHIImB1bxq7PaIdrKN9yKXDTOVQ,18
-omni_infer_api_account-0.0.1.dist-info/RECORD,,
+omniinfer_account/system.py,sha256=Xv0CQ5mK388TtdD9Ms5W8Lpw7B4c9bh1yR7Zv7a4h7E,14803
+omni_infer_api_account-0.0.2.dist-info/METADATA,sha256=HAEjy9zu7P8A9ZSFVHGrjknBkgtt_x5UXAUKNQNkr6A,239
+omni_infer_api_account-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+omni_infer_api_account-0.0.2.dist-info/top_level.txt,sha256=VYfZEk7HEk2argDpUHIImB1bxq7PaIdrKN9yKXDTOVQ,18
+omni_infer_api_account-0.0.2.dist-info/RECORD,,
```

