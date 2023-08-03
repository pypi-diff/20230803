# Comparing `tmp/hyload-0.2.7-py3-none-any.whl.zip` & `tmp/hyload-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 27559 bytes, number of entries: 17
+Zip file size: 27664 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat      171 b- defN 23-Jul-31 00:52 hyload/__init__.py
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-31 01:21 hyload/cfg.py
--rw-rw-rw-  2.0 fat    19401 b- defN 23-Jul-31 00:52 hyload/httpclient.py
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Aug-01 11:22 hyload/cfg.py
+-rw-rw-rw-  2.0 fat    20325 b- defN 23-Aug-03 03:08 hyload/httpclient.py
 -rw-rw-rw-  2.0 fat     2627 b- defN 23-Jul-31 00:52 hyload/logger.py
 -rw-rw-rw-  2.0 fat    11771 b- defN 23-Jul-31 00:52 hyload/stats.py
 -rw-rw-rw-  2.0 fat      979 b- defN 23-Jul-08 14:54 hyload/util.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-08 14:54 hyload/tools/__init__.py
 -rw-rw-rw-  2.0 fat     3667 b- defN 23-Jul-08 14:54 hyload/tools/plotperf.py
 -rw-rw-rw-  2.0 fat     2802 b- defN 23-Jul-08 14:54 hyload/tools/plotresource.py
 -rw-rw-rw-  2.0 fat    39521 b- defN 23-Jul-08 14:54 hyload/tools/puttyagents.py
 -rw-rw-rw-  2.0 fat     4303 b- defN 23-Jul-31 01:20 hyload/tools/remoteop.py
 -rw-rw-rw-  2.0 fat     7493 b- defN 23-Jul-14 12:12 hyload/tools/statshub.py
--rw-rw-rw-  2.0 fat     1100 b- defN 23-Jul-31 01:22 hyload-0.2.7.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1509 b- defN 23-Jul-31 01:22 hyload-0.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 01:22 hyload-0.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-31 01:22 hyload-0.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1311 b- defN 23-Jul-31 01:22 hyload-0.2.7.dist-info/RECORD
-17 files, 96771 bytes uncompressed, 25435 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     1100 b- defN 23-Aug-03 03:21 hyload-0.2.8.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1531 b- defN 23-Aug-03 03:21 hyload-0.2.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 03:21 hyload-0.2.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-03 03:21 hyload-0.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1311 b- defN 23-Aug-03 03:21 hyload-0.2.8.dist-info/RECORD
+17 files, 97717 bytes uncompressed, 25540 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: hyload/tools/remoteop.py
 Comment: 
 
 Filename: hyload/tools/statshub.py
 Comment: 
 
-Filename: hyload-0.2.7.dist-info/LICENSE.txt
+Filename: hyload-0.2.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hyload-0.2.7.dist-info/METADATA
+Filename: hyload-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: hyload-0.2.7.dist-info/WHEEL
+Filename: hyload-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: hyload-0.2.7.dist-info/top_level.txt
+Filename: hyload-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: hyload-0.2.7.dist-info/RECORD
+Filename: hyload-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hyload/cfg.py

```diff
@@ -1 +1 @@
-Version = '0.2.7'
+Version = '0.2.8'
```

## hyload/httpclient.py

```diff
@@ -233,18 +233,19 @@
     def send(self,
             method:str,
             url:str,
             params:Union[None,Dict[str,str]]=None,
             headers:Union[None,Dict[str,str]]=None, 
             data:Union[None,Dict[str,str],str,bytes]=None, 
             json=None,
-            debug:bool=False,
-            debug_body_print_max_len:int=4096,
             request_body_encoding:Union[None,str]=None,
-            response_body_encoding:Union[None,str]=None,            
+            debug:bool=False,
+            debug_print_request_body_encoding:Union[None,str]=None,
+            debug_print_response_body_encoding:Union[None,str]=None,    
+            debug_print_body_max_len:int=4096,        
             # duration:int=None,
         ):
         """send HTTP request to server and receive response from server.
 
         Parameters
         ----------
         method : str
@@ -256,31 +257,36 @@
         params : 
             (optional) Dictionary to send in the query string for the HTTP requests.
         headers : 
             (optional) Dictionary of HTTP Headers to send with the HTTP requests.
         data : 
             (optional) Dictionary, bytes, strings to send in the body of the HTTP requests.
         json : 
-            (optional) A JSON serializable Python object to send in the body of the HTTP requests.    
+            (optional) A JSON serializable Python object to send in the body of the HTTP requests.   
+        request_body_encoding : str, optional
+            (optional) HTTP request body bytes encoding, all Python char-encoding are supported. 
+            if not specified, hyload will use 'utf8' as text-encoding.  
         debug : bool, optional
             (optional) Whether print whole HTTP request and response, by default False.
             False : not print
-            True  : print        
-        debug_body_print_max_len : int , optional        
-            (optional) If debug set to True, at most how many chars of HTTP body will be printed. 
-            By default 4096.
-            If body length is larger, the remaining will be replaced with "....."
-        request_body_encoding : str, optional
-            (optional) HTTP request body bytes encoding, all Python char-encoding are supported. 
-            if not specified, hyload will use 'utf8' as text-encoding. 
-        response_body_encoding : str, optional
-            (optional) HTTP response body bytes encoding used for debug print, all Python char-encoding are supported. 
+            True  : print     
+        debug_print_request_body_encoding : str, optional
+            (optional) HTTP request body bytes encoding used for debug print, all Python char-encoding are supported. 
             if not specified, hyload will try to guess it from `Content-Type`.
             if no clue in `Content-Type`, it will use 'utf8' as text-encoding.   
             if set to 'hex', print bytes in hex string format.
+        debug_print_response_body_encoding : str, optional
+            (optional) HTTP response body bytes encoding used for debug print, all Python char-encoding are supported. 
+            if not specified, hyload will try to guess it from `Content-Type`.
+            if no clue in `Content-Type`, it will use 'utf8' as text-encoding.   
+            if set to 'hex', print bytes in hex string format.   
+        debug_print_body_max_len : int , optional        
+            (optional) If debug set to True, at most how many chars of HTTP body will be printed. 
+            By default 4096.
+            If body length is larger, the remaining will be replaced with "....."
 
         Returns
         -------
         _type_
             _description_
 
         Raises
@@ -367,21 +373,31 @@
             # bytes类型，直接放入消息体
             elif type(data) == bytes:
                 body = data
 
         try:
             self._conn.request(method, path, body, headers)
             if debug:
-                print('\n---------------------------')   
+                headers,body = _http_req_msg_buf_cpy.split(b"\r\n\r\n",1)
+                print('\n===========================')  
                 self._print_msg(
-                    _http_req_msg_buf_cpy, 
-                    request_body_encoding, 
+                    headers, 
+                    'utf8', 
                     bcolors.OKGREEN, 
-                    debug_body_print_max_len)  
-                _http_req_msg_buf_cpy = b''
+                    100000)  
+                
+                if body:
+                    print('\r\n\r\n',end='')
+
+                    self._print_msg(
+                        body, 
+                        debug_print_request_body_encoding, 
+                        bcolors.OKGREEN, 
+                        debug_print_body_max_len)  
+                    _http_req_msg_buf_cpy = b''
                 print('\n---------------------------')    
 
         except ConnectionRefusedError:
             errInfo = 'connection refused, maybe server not started'
             print('!!! ConnectionRefusedError\n' + errInfo)
             TestLogger.write(f'80|{errInfo}')
             
@@ -499,24 +515,25 @@
         
         if debug:
             contentEncoding = http_response.getheader('Content-Encoding')
             if contentEncoding == 'gzip':
                 try: raw_body = gzip.decompress(raw_body)
                 except OSError: pass      
 
-            if response_body_encoding is None:
+            if debug_print_response_body_encoding is None:
                 contentType = http_response.getheader('Content-Type')
-                response_body_encoding = self._guessEncodingFromContentType(contentType)
+                debug_print_response_body_encoding = self._guessEncodingFromContentType(contentType)
 
             self._print_msg(
                 raw_body,
-                response_body_encoding, 
+                debug_print_response_body_encoding, 
                 bcolors.OKBLUE,
-                debug_body_print_max_len)           
-            print('\n')
+                debug_print_body_max_len)     
+            
+            print('\n===========================\n')  
 
 
         self.response = HttpResponse(http_response,
                                    raw_body,
                                    int((recvTime-afterSendTime)*1000),
                                    path)
```

## Comparing `hyload-0.2.7.dist-info/LICENSE.txt` & `hyload-0.2.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hyload-0.2.7.dist-info/METADATA` & `hyload-0.2.8.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: hyload
-Version: 0.2.7
+Version: 0.2.8
 Summary: Framework for load testing
 Home-page: http://www.byhy.net
 Download-URL: https://pypi.python.org/pypi/hyload
 Author: baiyueheiyu 白月黑羽
 Author-email: jcyrss@gmail.com
 License: Apache License 2.0
 Keywords: hyload loadtesting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: gevent (>=20.9.0)
+Requires-Dist: gevent (>=22.10.2)
 Requires-Dist: matplotlib
-Requires-Dist: paramiko
-Requires-Dist: websockets
+Requires-Dist: paramiko (>=3.2.0)
+Requires-Dist: websockets (>=11.0.3)
 
 ## Introduction
 
 hyload 是一款性能测试库。目前针对HTTP接口的服务端系统进行性能压力测试。
 
 它提供了一个高效异步收发HTTP消息的库，可以让你使用Python语言自己开发代码。
```

## Comparing `hyload-0.2.7.dist-info/RECORD` & `hyload-0.2.8.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 hyload/__init__.py,sha256=wXjdLCvcOlQV8a7Mku2cQbyWRXheGf7dGkHfjvBqKu8,171
-hyload/cfg.py,sha256=GIdgtOLuSXpL0hEOWZyX4Nrxm6xhf1EIwSc8bGhSh3A,17
-hyload/httpclient.py,sha256=8fjF_T6i8q4Y1HEVKv97Qdn14SgdpqFBnDbup3RtAr4,19401
+hyload/cfg.py,sha256=6azBLSWUx8bv1Wv7aITk0YPiyCOwGxQC2wasyGBgnhU,17
+hyload/httpclient.py,sha256=nhk5h7YeTQhGCRQyU670dIHjpbnjxBrIUrHs_8TxSNY,20325
 hyload/logger.py,sha256=CfxUQM7oPiWuiuXmtiQiD5ViXkdY1t5yo8-SvRWO1q8,2627
 hyload/stats.py,sha256=1BCif-2OTVWEPvSMEIxY_WoJQ0v7I2WxJlkLAXDoIxA,11771
 hyload/util.py,sha256=lNKVVW4vYFueXcvOC4HoIMIiXFUz6skR9shSA7iPsWU,979
 hyload/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hyload/tools/plotperf.py,sha256=H1OszxmfgAYAxX4YEp-_aX66w6slynz9tjDGdpraMMo,3667
 hyload/tools/plotresource.py,sha256=9ydos2xFSA__ANhQ4b_fr5ORJPwWVLCgXoYnYdO5cA4,2802
 hyload/tools/puttyagents.py,sha256=NvL3VhYYka69kh7QTdRzjm7dLN3dB5MuU__K1GmGsW8,39521
 hyload/tools/remoteop.py,sha256=IzpeYMIk-zmNGJD-U_h_N9bSD6FDHy87kH6zgKzg7rA,4303
 hyload/tools/statshub.py,sha256=bPyj9h6eewxRJSJmQpqtkx3DFbvoYbQsWpcFvATFang,7493
-hyload-0.2.7.dist-info/LICENSE.txt,sha256=OGhxEO0MAMle3LEQV8Us5uo4C8pk-jWmCBKyQ7U_gCE,1100
-hyload-0.2.7.dist-info/METADATA,sha256=K40sjgOlvHizeoVZ-IotBLXIfJ8c8H2zyxie7NQbZFQ,1509
-hyload-0.2.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hyload-0.2.7.dist-info/top_level.txt,sha256=ivEyc-v2p5WU0itBl-u9QARFubEqBlHfczIhYbuD_U8,7
-hyload-0.2.7.dist-info/RECORD,,
+hyload-0.2.8.dist-info/LICENSE.txt,sha256=OGhxEO0MAMle3LEQV8Us5uo4C8pk-jWmCBKyQ7U_gCE,1100
+hyload-0.2.8.dist-info/METADATA,sha256=9Yr2tTnFgZulrEV1KnLk6odieI3yQQqwXBCFToYqjCE,1531
+hyload-0.2.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hyload-0.2.8.dist-info/top_level.txt,sha256=ivEyc-v2p5WU0itBl-u9QARFubEqBlHfczIhYbuD_U8,7
+hyload-0.2.8.dist-info/RECORD,,
```

