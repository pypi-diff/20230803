# Comparing `tmp/t3qai_client-1.1.2-py3-none-any.whl.zip` & `tmp/t3qai_client-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15100 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     1639 b- defN 22-Jul-12 06:56 t3qai_client/__init__.py
--rw-rw-rw-  2.0 fat    23600 b- defN 22-Jul-06 05:31 t3qai_client/t3qai_helper.py
--rw-rw-rw-  2.0 fat     6328 b- defN 22-Jul-12 03:38 t3qai_client/t3qai_serving.py
--rw-rw-rw-  2.0 fat    11533 b- defN 22-Jul-12 06:57 t3qai_client-1.1.2.dist-info/LICENSE-2.0.txt
--rw-rw-rw-  2.0 fat     2758 b- defN 22-Jul-12 06:57 t3qai_client-1.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jul-12 06:57 t3qai_client-1.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 22-Jul-12 06:57 t3qai_client-1.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      673 b- defN 22-Jul-12 06:57 t3qai_client-1.1.2.dist-info/RECORD
-8 files, 46636 bytes uncompressed, 13924 bytes compressed:  70.1%
+Zip file size: 15106 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     1639 b- defN 23-Aug-03 08:00 t3qai_client/__init__.py
+-rw-rw-rw-  2.0 fat    23600 b- defN 23-Aug-03 08:00 t3qai_client/t3qai_helper.py
+-rw-rw-rw-  2.0 fat     6328 b- defN 23-Aug-03 08:00 t3qai_client/t3qai_serving.py
+-rw-rw-rw-  2.0 fat    11533 b- defN 23-Aug-03 08:01 t3qai_client-1.1.3.dist-info/LICENSE-2.0.txt
+-rw-rw-rw-  2.0 fat     2850 b- defN 23-Aug-03 08:01 t3qai_client-1.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 08:01 t3qai_client-1.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-03 08:01 t3qai_client-1.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      673 b- defN 23-Aug-03 08:01 t3qai_client-1.1.3.dist-info/RECORD
+8 files, 46728 bytes uncompressed, 13930 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: t3qai_client/t3qai_helper.py
 Comment: 
 
 Filename: t3qai_client/t3qai_serving.py
 Comment: 
 
-Filename: t3qai_client-1.1.2.dist-info/LICENSE-2.0.txt
+Filename: t3qai_client-1.1.3.dist-info/LICENSE-2.0.txt
 Comment: 
 
-Filename: t3qai_client-1.1.2.dist-info/METADATA
+Filename: t3qai_client-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: t3qai_client-1.1.2.dist-info/WHEEL
+Filename: t3qai_client-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: t3qai_client-1.1.2.dist-info/top_level.txt
+Filename: t3qai_client-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: t3qai_client-1.1.2.dist-info/RECORD
+Filename: t3qai_client-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t3qai_client/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.2"
+__version__ = "1.1.1"
 
 from t3qai_client.t3qai_helper import train_start as train_start
 from t3qai_client.t3qai_helper import train_finish as train_finish
 from t3qai_client.t3qai_helper import train_load_param as train_load_param
 from t3qai_client.t3qai_helper import inference_load_param as inference_load_param
 from t3qai_client.t3qai_helper import train_load_path as train_load_path
 from t3qai_client.t3qai_helper import load_data as load_data
```

## Comparing `t3qai_client-1.1.2.dist-info/LICENSE-2.0.txt` & `t3qai_client-1.1.3.dist-info/LICENSE-2.0.txt`

 * *Files identical despite different names*

## Comparing `t3qai_client-1.1.2.dist-info/METADATA` & `t3qai_client-1.1.3.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,93 +1,94 @@
-Metadata-Version: 2.1
-Name: t3qai-client
-Version: 1.1.2
-Summary: t3qai client module
-Home-page: 
-Download-URL: 
-Author: t3q
-Author-email: lab@t3q.com
-Keywords: t3q,t3qai,t3qai client,t3qai_client
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE-2.0.txt
-Requires-Dist: fastapi
-Requires-Dist: uvicorn
-Requires-Dist: pandas
-Requires-Dist: requests
-Requires-Dist: python-multipart
-
-# t3qai_client Description
-a library for t3qai platform client.
-
-The client module provides properties/functions
-that links platform and client's learning/Inference algorithm.
-
-- Provide platform path properties
-- Provides functions to link learning state, set log, call learning parameter elements, load data, save learning results, and download inference results
-
-## To install with pip
-```
-pip install t3qai_client
-
-```
-
-## How to Use (Example)
-### properties
-```
-## train
-from t3qai_client import T3QAI_TRAIN_OUTPUT_PATH, T3QAI_TRAIN_MODEL_PATH, T3QAI_TRAIN_DATA_PATH, T3QAI_TEST_DATA_PATH, T3QAI_MODULE_PATH
-
-## inference
-from t3qai_client import T3QAI_INIT_MODEL_PATH
-```
-
-### functions
-```
-import t3qai_client as tc
-
-## link learning state
-tc.train_start()
-tc.train_finish(result, result_msg)
-
-## set log
-# train
-tc.train_set_logger()
-# inference
-tc.inference_set_logger()
-
-## call learning parameter elements
-# train
-params = tc.train_load_param()
-batch_size= int(params['batch_size'])
-# inference
-params = tc.inference_load_param()
-batch_size= int(params['batch_size'])
-
-## load data
-# To use this function, the dataset with id and label must pass through the preprocessing module.
-(train_id, train_x, train_y), (test_id, test_x, test_y) = tc.load_data()
-
-## save learning results
-# To draw charts inside the platform, use this function to save the learning results.
-# save result (Loss, PCA 2D)
-eval_results={}
-eval_results['predict_y'] = [0, 1, 0]     # predict y
-eval_results['actual_y'] = [[0], [1], [0]]  # actual y
-eval_results['test_id'] = [0,1,2]        # test id(unique id)
-eval_results['loss']=  float(0.3)        # loss
-tc.train_save_result_metrics(eval_results)
-# save classifacation result (Accuary, Loss, Confusion Matrix, Pricision/Recall//F1-score)
-eval_results={}
-eval_results['predict_y'] = [0, 1, 0]
-eval_results['actual_y'] = [[0], [1], [0]]
-eval_results['test_id'] = [0,1,2]
-eval_results['loss'] =  float(0.3)
-tc.train_save_classification_result(metrics)
-
-## To download inference results at platform (2 options -> file_obj or file_path)
-from t3qai_client import DownloadFile
-result = DownloadFile(file_obj=resultobj, file_name=filename)
-result = DownloadFile(file_path=save_path, file_name=filename)
-```
+Metadata-Version: 2.1
+Name: t3qai-client
+Version: 1.1.3
+Summary: t3qai client module
+Home-page: UNKNOWN
+Author: t3q
+Author-email: lab@t3q.com
+License: UNKNOWN
+Keywords: t3q,t3qai,t3qai client,t3qai_client
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+Requires-Dist: fastapi
+Requires-Dist: uvicorn
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: python-multipart
+
+# t3qai_client Description
+a library for t3qai platform client.
+
+The client module provides properties/functions
+that links platform and client's learning/Inference algorithm.
+
+- Provide platform path properties
+- Provides functions to link learning state, set log, call learning parameter elements, load data, save learning results, and download inference results
+
+## To install with pip
+```
+pip install t3qai_client
+
+```
+
+## How to Use (Example)
+### properties
+```
+## train
+from t3qai_client import T3QAI_TRAIN_OUTPUT_PATH, T3QAI_TRAIN_MODEL_PATH, T3QAI_TRAIN_DATA_PATH, T3QAI_TEST_DATA_PATH, T3QAI_MODULE_PATH
+
+## inference
+from t3qai_client import T3QAI_INIT_MODEL_PATH
+```
+
+### functions
+```
+import t3qai_client as tc
+
+## link learning state
+tc.train_start()
+tc.train_finish(result, result_msg)
+
+## set log
+# train
+tc.train_set_logger()
+# inference
+tc.inference_set_logger()
+
+## call learning parameter elements
+# train
+params = tc.train_load_param()
+batch_size= int(params['batch_size'])
+# inference
+params = tc.inference_load_param()
+batch_size= int(params['batch_size'])
+
+## load data
+# To use this function, the dataset with id and label must pass through the preprocessing module.
+(train_id, train_x, train_y), (test_id, test_x, test_y) = tc.load_data()
+
+## save learning results
+# To draw charts inside the platform, use this function to save the learning results.
+# save result (Loss, PCA 2D)
+eval_results={}
+eval_results['predict_y'] = [0, 1, 0]     # predict y
+eval_results['actual_y'] = [[0], [1], [0]]  # actual y
+eval_results['test_id'] = [0,1,2]        # test id(unique id)
+eval_results['loss']=  float(0.3)        # loss
+tc.train_save_result_metrics(eval_results)
+# save classifacation result (Accuary, Loss, Confusion Matrix, Pricision/Recall//F1-score)
+eval_results={}
+eval_results['predict_y'] = [0, 1, 0]
+eval_results['actual_y'] = [[0], [1], [0]]
+eval_results['test_id'] = [0,1,2]
+eval_results['loss'] =  float(0.3)
+tc.train_save_classification_result(metrics)
+
+## To download inference results at platform (2 options -> file_obj or file_path)
+from t3qai_client import DownloadFile
+result = DownloadFile(file_obj=resultobj, file_name=filename)
+result = DownloadFile(file_path=save_path, file_name=filename)
+```
+
```

## Comparing `t3qai_client-1.1.2.dist-info/RECORD` & `t3qai_client-1.1.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-t3qai_client/__init__.py,sha256=_XnhY7dVHfxV7U90cvFnB8oNC6bSw8XalraUK0SDfhk,1639
+t3qai_client/__init__.py,sha256=77s_ELw_PXqJY82x2hWn6OU8CDZCxKdvtN5wsvP7xIY,1639
 t3qai_client/t3qai_helper.py,sha256=qOhvsnlwD1HTnoe2ZycKwFP9n2W-wmlX-HXsCXa2YpM,23600
 t3qai_client/t3qai_serving.py,sha256=aadhlm4Di0gU9s5ZsA3Xch1SjI7wvxNh1ygYOoYty84,6328
-t3qai_client-1.1.2.dist-info/LICENSE-2.0.txt,sha256=thx4yBYMK9EojcuEfGeSPZ4xsnPVNBR8XYMtziBGiWI,11533
-t3qai_client-1.1.2.dist-info/METADATA,sha256=xqvD3fUGQSyGC1KFiEXYOoK2ybVulNRO3bgtIoDZpNk,2758
-t3qai_client-1.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-t3qai_client-1.1.2.dist-info/top_level.txt,sha256=-peQr4CAunIVn62-N5YE4UpLbZJ76mWPDOJGcy36mN8,13
-t3qai_client-1.1.2.dist-info/RECORD,,
+t3qai_client-1.1.3.dist-info/LICENSE-2.0.txt,sha256=thx4yBYMK9EojcuEfGeSPZ4xsnPVNBR8XYMtziBGiWI,11533
+t3qai_client-1.1.3.dist-info/METADATA,sha256=dRBa1sWBfPONYGIf832tF8faU8ui_sVo12aplporrN8,2850
+t3qai_client-1.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+t3qai_client-1.1.3.dist-info/top_level.txt,sha256=-peQr4CAunIVn62-N5YE4UpLbZJ76mWPDOJGcy36mN8,13
+t3qai_client-1.1.3.dist-info/RECORD,,
```

