# Comparing `tmp/nemusicapi-0.1.0.tar.gz` & `tmp/nemusicapi-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.1.0.tar", max compression
+gzip compressed data, was "nemusicapi-0.1.1a1.tar", max compression
```

## Comparing `nemusicapi-0.1.0.tar` & `nemusicapi-0.1.1a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.0/LICENSE
--rw-r--r--   0        0        0      311 2023-08-03 09:11:40.318932 nemusicapi-0.1.0/nemusicapi/__init__.py
--rw-r--r--   0        0        0     4829 2023-08-03 09:08:35.550244 nemusicapi-0.1.0/nemusicapi/api.py
--rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.0/nemusicapi/exception.py
--rw-r--r--   0        0        0      338 2023-08-03 08:13:25.809448 nemusicapi-0.1.0/nemusicapi/type.py
--rw-r--r--   0        0        0      464 2023-08-03 09:11:50.295603 nemusicapi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1285 2023-08-03 08:27:02.179801 nemusicapi-0.1.0/README.md
--rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 nemusicapi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0      311 2023-08-03 09:11:40.318932 nemusicapi-0.1.1a1/nemusicapi/__init__.py
+-rw-r--r--   0        0        0     4864 2023-08-03 09:30:55.310463 nemusicapi-0.1.1a1/nemusicapi/api.py
+-rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.1a1/nemusicapi/exception.py
+-rw-r--r--   0        0        0      338 2023-08-03 08:13:25.809448 nemusicapi-0.1.1a1/nemusicapi/type.py
+-rw-r--r--   0        0        0      466 2023-08-03 09:31:05.117090 nemusicapi-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1285 2023-08-03 08:27:02.179801 nemusicapi-0.1.1a1/README.md
+-rw-r--r--   0        0        0     1906 1970-01-01 00:00:00.000000 nemusicapi-0.1.1a1/PKG-INFO
```

### Comparing `nemusicapi-0.1.0/LICENSE` & `nemusicapi-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.1.0/nemusicapi/api.py` & `nemusicapi-0.1.1a1/nemusicapi/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,31 +11,30 @@
 from nemusicapi.exception import NoDownloadDirException
 from nemusicapi.type import QualityLevel, EncodeType
 
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
-def aes_encrypt(text, key):
+def aes_encrypt(raw_text: str, raw_key: str):
+    key = raw_key.encode('utf-8')  # 将密钥转换为utf-8格式
     iv = '0102030405060708'.encode('utf-8')  # iv偏移量
-    text = text.encode('utf-8')  # 将明文转换为utf-8格式
-    pad = 16 - len(text) % 16
-    text = text + (pad * chr(pad)).encode('utf-8')  # 明文需要转成二进制，且可以被16整除
-    key = key.encode('utf-8')  # 将密钥转换为utf-8格式
     encryptor = AES.new(key, AES.MODE_CBC, iv)  # 创建一个AES对象
-    encrypt_text = encryptor.encrypt(text)  # 加密
-    encrypt_text = base64.b64encode(encrypt_text)  # base4编码转换为byte字符串
+    _text = raw_text.encode('utf-8')  # 将明文转换为utf-8格式
+    pad = 16 - len(_text) % 16
+    text = _text + (pad * chr(pad)).encode('utf-8')  # 明文需要转成二进制，且可以被16整除
+    _encrypt_text = encryptor.encrypt(text)  # 加密
+    encrypt_text = base64.b64encode(_encrypt_text)  # base64编码转换为byte字符串
     return encrypt_text.decode('utf-8')
 
 
-# RSA加密获得encSeckey
-def rsa_encrypt(str, key, f):
-    str = str[::-1]  # 随机字符串逆序排列
-    str = bytes(str, 'utf-8')  # 将随机字符串转换为byte类型的数据
-    sec_key = int(codecs.encode(str, encoding='hex'), 16) ** int(key, 16) % int(f, 16)  # RSA加密
+def rsa_encrypt(raw_text: str, key: str, f: str):
+    _text = raw_text[::-1]  # 随机字符串逆序排列
+    text = bytes(_text, 'utf-8')  # 将随机字符串转换为byte类型的数据
+    sec_key = int(codecs.encode(text, encoding='hex'), 16) ** int(key, 16) % int(f, 16)  # RSA加密
     return format(sec_key, 'x').zfill(256)  # RSA加密后字符串长度为256，不足的补x
 
 
 def get_params(raw_params: str):
     random_str = ''.join(random.sample('abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789', 16))
     encText = aes_encrypt(raw_params, '0CoJUm6Qyw8W8jud')
     params = aes_encrypt(encText, random_str)
```

### Comparing `nemusicapi-0.1.0/README.md` & `nemusicapi-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.1.0/PKG-INFO` & `nemusicapi-0.1.1a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.1.0
+Version: 0.1.1a1
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

