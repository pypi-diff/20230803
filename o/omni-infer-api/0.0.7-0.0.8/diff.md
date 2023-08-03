# Comparing `tmp/omni_infer_api-0.0.7-py3-none-any.whl.zip` & `tmp/omni_infer_api-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 9576 bytes, number of entries: 20
+Zip file size: 9578 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat      122 b- defN 23-Aug-01 08:12 omniifer_api/__init__.py
 -rw-rw-rw-  2.0 fat      127 b- defN 23-Aug-02 09:02 omniifer_api/config.py
 -rw-rw-rw-  2.0 fat      181 b- defN 23-Jul-30 01:30 omniifer_api/error.py
 -rw-rw-rw-  2.0 fat       94 b- defN 23-Jul-31 07:03 omniifer_api/image_generate/__init__.py
--rw-rw-rw-  2.0 fat     2759 b- defN 23-Aug-02 04:24 omniifer_api/image_generate/img2img.py
+-rw-rw-rw-  2.0 fat     2761 b- defN 23-Aug-03 11:21 omniifer_api/image_generate/img2img.py
 -rw-rw-rw-  2.0 fat      762 b- defN 23-Aug-02 04:24 omniifer_api/image_generate/progress.py
--rw-rw-rw-  2.0 fat     3808 b- defN 23-Aug-02 09:43 omniifer_api/image_generate/txt2img.py
+-rw-rw-rw-  2.0 fat     3810 b- defN 23-Aug-03 11:21 omniifer_api/image_generate/txt2img.py
 -rw-rw-rw-  2.0 fat      210 b- defN 23-Aug-02 07:08 omniifer_api/model_list/__init__.py
 -rw-rw-rw-  2.0 fat      872 b- defN 23-Aug-02 04:24 omniifer_api/model_list/get_model.py
 -rw-rw-rw-  2.0 fat      478 b- defN 23-Aug-02 04:24 omniifer_api/model_list/get_models.py
 -rw-rw-rw-  2.0 fat      236 b- defN 23-Aug-02 09:42 omniifer_api/model_list/model_available.py
 -rw-rw-rw-  2.0 fat      758 b- defN 23-Aug-02 04:27 omniifer_api/model_list/put_model.py
 -rw-rw-rw-  2.0 fat     1270 b- defN 23-Aug-02 09:43 omniifer_api/model_list/search_models.py
 -rw-rw-rw-  2.0 fat      581 b- defN 23-Aug-02 04:27 omniifer_api/model_list/update.py
 -rw-rw-rw-  2.0 fat       33 b- defN 23-Jul-31 07:37 omniifer_api/tools/__init__.py
 -rw-rw-rw-  2.0 fat      307 b- defN 23-Jul-30 02:18 omniifer_api/tools/response_check.py
--rw-rw-rw-  2.0 fat      199 b- defN 23-Aug-02 09:44 omni_infer_api-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-02 09:44 omni_infer_api-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-02 09:44 omni_infer_api-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1768 b- defN 23-Aug-02 09:44 omni_infer_api-0.0.7.dist-info/RECORD
-20 files, 14670 bytes uncompressed, 6630 bytes compressed:  54.8%
+-rw-rw-rw-  2.0 fat      199 b- defN 23-Aug-03 11:22 omni_infer_api-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 11:22 omni_infer_api-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-03 11:22 omni_infer_api-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1768 b- defN 23-Aug-03 11:22 omni_infer_api-0.0.8.dist-info/RECORD
+20 files, 14674 bytes uncompressed, 6632 bytes compressed:  54.8%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: omniifer_api/tools/__init__.py
 Comment: 
 
 Filename: omniifer_api/tools/response_check.py
 Comment: 
 
-Filename: omni_infer_api-0.0.7.dist-info/METADATA
+Filename: omni_infer_api-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: omni_infer_api-0.0.7.dist-info/WHEEL
+Filename: omni_infer_api-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: omni_infer_api-0.0.7.dist-info/top_level.txt
+Filename: omni_infer_api-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: omni_infer_api-0.0.7.dist-info/RECORD
+Filename: omni_infer_api-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omniifer_api/image_generate/img2img.py

```diff
@@ -17,16 +17,16 @@
     if not 1 <= n_iter <= 8:
         raise error.OMNI_INFER_API_ERROR("Error n iter: " + str(n_iter))
     if not 1 <= steps <= 50:
         raise error.OMNI_INFER_API_ERROR("Error steps: " + str(steps))
     if not 1 <= cfg_scale <= 30:
         raise error.OMNI_INFER_API_ERROR("Error cfg scale: " + str(cfg_scale))
     if seed == -1:
-        seed = random.randrange(0, 2 ^ 32)
-    if not 0 <= seed <= 2 ^ 32:
+        seed = random.randrange(0, 2 ** 32)
+    if not 0 <= seed <= 2 ** 32:
         raise error.OMNI_INFER_API_ERROR("Error seed: " + str(seed))
     if not 1 <= height <= 2048:
         raise error.OMNI_INFER_API_ERROR("Error height: " + str(height))
     if not 1 <= width <= 2048:
         raise error.OMNI_INFER_API_ERROR("Error width: " + str(width))
     if not clip_skip > 0:
         raise error.OMNI_INFER_API_ERROR("Error clip skip: " + str(clip_skip))
```

## omniifer_api/image_generate/txt2img.py

```diff
@@ -17,16 +17,16 @@
     if not 1 <= n_iter <= 8:
         raise error.OMNI_INFER_API_ERROR("Error n iter: " + str(n_iter))
     if not 1 <= steps <= 50:
         raise error.OMNI_INFER_API_ERROR("Error steps: " + str(steps))
     if not 1 <= cfg_scale <= 30:
         raise error.OMNI_INFER_API_ERROR("Error cfg scale: " + str(cfg_scale))
     if seed == -1:
-        seed = random.randrange(0, 2 ^ 32)
-    if not 0 <= seed <= 2 ^ 32:
+        seed = random.randrange(0, 2 ** 32)
+    if not 0 <= seed <= 2 ** 32:
         raise error.OMNI_INFER_API_ERROR("Error seed: " + str(seed))
     if not 1 <= height <= 2048:
         raise error.OMNI_INFER_API_ERROR("Error height: " + str(height))
     if not 1 <= width <= 2048:
         raise error.OMNI_INFER_API_ERROR("Error width: " + str(width))
     if not clip_skip > 0:
         raise error.OMNI_INFER_API_ERROR("Error clip skip: " + str(clip_skip))
```

## Comparing `omni_infer_api-0.0.7.dist-info/RECORD` & `omni_infer_api-0.0.8.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 omniifer_api/__init__.py,sha256=u0VFTki9sLh0vIMB7nFn2nL86ZNYFVJ72p2PkNccNjs,122
 omniifer_api/config.py,sha256=j728wO-wLS5Q6y5IlPX7nhn9QS-brLnVbKOt-RcwM_k,127
 omniifer_api/error.py,sha256=0vXK1xTR3KjXsYCcw9W3G4Wz9q5QEcsCRR1hfKA2gZk,181
 omniifer_api/image_generate/__init__.py,sha256=NBmouScnfMygwpFo0xX5Ezm4h0FZLKvQqEdnt1HvS_4,94
-omniifer_api/image_generate/img2img.py,sha256=F8pnsYnI41e-jYfq4hf7rLh_CKy1829OYEwMP8sfVHk,2759
+omniifer_api/image_generate/img2img.py,sha256=_PVavB94BdgIou31-MVC3zTnmo9l8qlN_PchuIuSJuQ,2761
 omniifer_api/image_generate/progress.py,sha256=D9BmnjK86L4uF4mmfU4YLlnaGKTL6uReH0KmAeRxlhI,762
-omniifer_api/image_generate/txt2img.py,sha256=BBws5PpuIKuZANN-E_Brxgk2Nklx7aFfSF6knpwears,3808
+omniifer_api/image_generate/txt2img.py,sha256=j5tHrN3x62ZJIqI-Bv2WTtEqNTD64watEYhbQwzYfsA,3810
 omniifer_api/model_list/__init__.py,sha256=ZBkOXuP_7TQZsXfWQJMVygGXpq2HAtOI59cTVnC4zwM,210
 omniifer_api/model_list/get_model.py,sha256=JfGnbk09SEshvJ_veSKoqh-5_HjPInK8UliCsHthtXU,872
 omniifer_api/model_list/get_models.py,sha256=831qL54ESVJCVS95cNxZzmn416UMDYBCGgygFf_-8P0,478
 omniifer_api/model_list/model_available.py,sha256=Y-2uCgXfBbDPz-mjVkVPW2QL7KcZ2f34uSt5Ma1vMFE,236
 omniifer_api/model_list/put_model.py,sha256=ooYNTWaHt0MAq4Inrc1g8yrlnFA1Iv6TMwCYKkp7OUc,758
 omniifer_api/model_list/search_models.py,sha256=IKkpZ-TS9_xQwJbMB9sYGVYNIpST7BfFSf9EkxoYUtY,1270
 omniifer_api/model_list/update.py,sha256=v_WrUh0SVG6f4-hbH_LBdtUmAFWBPnEp7ukDPVkSK9g,581
 omniifer_api/tools/__init__.py,sha256=PbUs8cnYO79sGl1Y6zsKhOiZHHExEidiyrntyJ-aTDg,33
 omniifer_api/tools/response_check.py,sha256=PJbyxy5CXICZnRenoS1Qxyvp3vYzSOCAQSbUGqdTzJc,307
-omni_infer_api-0.0.7.dist-info/METADATA,sha256=n78Xu3EO_vaVaH6IuscaEHMC44VClaKnEsmQ86Jksj8,199
-omni_infer_api-0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-omni_infer_api-0.0.7.dist-info/top_level.txt,sha256=-5RhHKNFz5hCy5blJH5c-osZ5xLeU7Vk5unquKrtgIM,13
-omni_infer_api-0.0.7.dist-info/RECORD,,
+omni_infer_api-0.0.8.dist-info/METADATA,sha256=uj8cSrT_JiSDDSrteJclkMA4BK8Ed2RHsHwFKHFxZds,199
+omni_infer_api-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+omni_infer_api-0.0.8.dist-info/top_level.txt,sha256=-5RhHKNFz5hCy5blJH5c-osZ5xLeU7Vk5unquKrtgIM,13
+omni_infer_api-0.0.8.dist-info/RECORD,,
```

