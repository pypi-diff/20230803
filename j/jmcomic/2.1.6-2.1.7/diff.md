# Comparing `tmp/jmcomic-2.1.6.tar.gz` & `tmp/jmcomic-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.1.6.tar", last modified: Mon Jul 31 05:53:01 2023, max compression
+gzip compressed data, was "jmcomic-2.1.7.tar", last modified: Thu Aug  3 09:02:57 2023, max compression
```

## Comparing `jmcomic-2.1.6.tar` & `jmcomic-2.1.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:53:01.701327 jmcomic-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 05:52:47.000000 jmcomic-2.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-31 05:53:01.701327 jmcomic-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-31 05:52:47.000000 jmcomic-2.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 05:53:01.701327 jmcomic-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-31 05:52:47.000000 jmcomic-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:53:01.697327 jmcomic-2.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:53:01.701327 jmcomic-2.1.6/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:53:01.701327 jmcomic-2.1.6/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-31 05:53:01.000000 jmcomic-2.1.6/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-31 05:53:01.000000 jmcomic-2.1.6/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 05:53:01.000000 jmcomic-2.1.6/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 05:53:01.000000 jmcomic-2.1.6/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 05:53:01.000000 jmcomic-2.1.6/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:02:57.143454 jmcomic-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 09:02:45.000000 jmcomic-2.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-03 09:02:57.143454 jmcomic-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-03 09:02:45.000000 jmcomic-2.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 09:02:57.143454 jmcomic-2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-03 09:02:45.000000 jmcomic-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:02:57.139454 jmcomic-2.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:02:57.139454 jmcomic-2.1.7/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-03 09:02:45.000000 jmcomic-2.1.7/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 09:02:45.000000 jmcomic-2.1.7/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-08-03 09:02:45.000000 jmcomic-2.1.7/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-08-03 09:02:45.000000 jmcomic-2.1.7/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-08-03 09:02:45.000000 jmcomic-2.1.7/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-08-03 09:02:45.000000 jmcomic-2.1.7/src/jmcomic/jm_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-08-03 09:02:45.000000 jmcomic-2.1.7/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-08-03 09:02:45.000000 jmcomic-2.1.7/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-08-03 09:02:45.000000 jmcomic-2.1.7/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:02:57.143454 jmcomic-2.1.7/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-03 09:02:57.000000 jmcomic-2.1.7/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 09:02:57.000000 jmcomic-2.1.7/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:02:57.000000 jmcomic-2.1.7/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-03 09:02:57.000000 jmcomic-2.1.7/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 09:02:57.000000 jmcomic-2.1.7/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.1.6/LICENSE` & `jmcomic-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.6/PKG-INFO` & `jmcomic-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.1.6/README.md` & `jmcomic-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.6/setup.py` & `jmcomic-2.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.6/src/jmcomic/jm_client_impl.py` & `jmcomic-2.1.7/src/jmcomic/jm_client_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         if retry_count < self.retry_times:
             return self.request_with_retry(request, url, domain_index, retry_count + 1, **kwargs)
         else:
             return self.request_with_retry(request, url, domain_index + 1, 0, **kwargs)
 
     # noinspection PyMethodMayBeStatic, PyUnusedLocal
     def before_retry(self, e, kwargs, retry_count, url):
-        jm_debug('error', str(e))
+        jm_debug('retry', str(e))
 
     def enable_cache(self, debug=False):
         def wrap_func_cache(func_name, cache_dict_name):
             import common
             if common.VERSION > '0.4.8':
                 if hasattr(self, cache_dict_name):
                     return
@@ -127,16 +127,19 @@
 
     def get_jmcomic_url(self, postman=None):
         return JmModuleConfig.get_jmcomic_url(postman or self.get_root_postman())
 
     def get_jmcomic_domain_all(self, postman=None):
         return JmModuleConfig.get_jmcomic_domain_all(postman or self.get_root_postman())
 
+    # noinspection PyUnusedLocal
     def fallback(self, request, url, domain_index, retry_count, **kwargs):
-        raise AssertionError(f"请求重试全部失败: [{url}], {self.domain_list}")
+        msg = f"请求重试全部失败: [{url}], {self.domain_list}"
+        jm_debug('fallback', "msg")
+        raise AssertionError(msg)
 
 
 # 基于网页实现的JmClient
 class JmHtmlClient(AbstractJmClient):
 
     def get_album_detail(self, album_id) -> JmAlbumDetail:
         # 参数校验
@@ -402,7 +405,19 @@
         token = hashlib.md5(f"{key_ts}{JmModuleConfig.MAGIC_18COMICAPPCONTENT}".encode()).hexdigest()
         return {
             "token": token,
             "tokenparam": f"{key_ts},1.5.2",
             "user-agent": "okhttp/3.12.1",
             "accept-encoding": "gzip",
         }, key_ts
+
+
+class AsyncSaveImageClient(JmImageClient):
+
+    def __init__(self, workers=None) -> None:
+        from concurrent.futures import ThreadPoolExecutor, Future
+        self.executor = ThreadPoolExecutor(max_workers=workers)
+        self.future_list: List[Future] = []
+
+    def save_image_resp(self, *args, **kwargs):
+        future = self.executor.submit(lambda: super().save_image_resp(*args, **kwargs))
+        self.future_list.append(future)
```

### Comparing `jmcomic-2.1.6/src/jmcomic/jm_client_interface.py` & `jmcomic-2.1.7/src/jmcomic/jm_client_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -232,27 +232,29 @@
         @param decode_image: 要保存的是解密后的图还是原图
         """
         # 请求图片
         resp = self.get_jm_image(img_url)
 
         resp.require_success()
 
-        # gif图无需加解密，需要最先判断
+        return self.save_image_resp(decode_image, img_save_path, img_url, resp, scramble_id)
 
+    def save_image_resp(self, decode_image, img_save_path, img_url, resp, scramble_id):
+        # gif图无需加解密，需要最先判断
         if self.img_is_not_need_to_decode(img_url, resp):
             JmImageSupport.save_resp_img(resp, img_save_path, False)
         else:
             resp.transfer_to(img_save_path, scramble_id, decode_image, img_url)
 
     def download_by_image_detail(self,
                                  image: JmImageDetail,
                                  img_save_path,
                                  decode_image=True,
                                  ):
-        self.download_image(
+        return self.download_image(
             image.download_url,
             img_save_path,
             image.scramble_id,
             decode_image=decode_image,
         )
 
     def get_jm_image(self, img_url) -> JmImageResp:
```

### Comparing `jmcomic-2.1.6/src/jmcomic/jm_config.py` & `jmcomic-2.1.7/src/jmcomic/jm_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,32 @@
     default_photo_title = 'default-photo-title'
     default_photo_id = 'default-photo-id'
 
     # debug
     enable_jm_debug = True
     debug_executor = default_jm_debug
     postman_constructor = default_postman_constructor
+    DOWNLOADER_CLASS = None
+    OPTION_CLASS = None
+
+    @classmethod
+    def downloader_class(cls):
+        if cls.DOWNLOADER_CLASS is not None:
+            return cls.DOWNLOADER_CLASS
+
+        from .jm_downloader import JmDownloader
+        return JmDownloader
+
+    @classmethod
+    def option_class(cls):
+        if cls.OPTION_CLASS is not None:
+            return cls.OPTION_CLASS
+
+        from .jm_option import JmOption
+        return JmOption
 
     @classmethod
     @field_cache("DOMAIN")
     def domain(cls, postman=None):
         """
         由于禁漫的域名经常变化，调用此方法可以获取一个当前可用的最新的域名 domain，
         并且设置把 domain 设置为禁漫模块的默认域名。
@@ -111,16 +129,15 @@
     def get_jmcomic_url(cls, postman=None):
         """
         访问禁漫的永久网域，从而得到一个可用的禁漫网址
         @return: https://jm-comic2.cc
         """
         postman = postman or cls.new_postman(session=True)
 
-        resp = postman.get(cls.JM_REDIRECT_URL)
-        url = resp.url
+        url = postman.with_redirect_catching().get(cls.JM_REDIRECT_URL)
         cls.jm_debug('获取禁漫地址', f'[{cls.JM_REDIRECT_URL}] → [{url}]')
         return url
 
     @classmethod
     @field_cache("DOMAIN_LIST")
     def get_jmcomic_domain_all(cls, postman=None):
         """
```

### Comparing `jmcomic-2.1.6/src/jmcomic/jm_entity.py` & `jmcomic-2.1.7/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.6/src/jmcomic/jm_option.py` & `jmcomic-2.1.7/src/jmcomic/jm_option.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,10 @@
 from .jm_client_impl import *
 
 
-# noinspection PyMethodMayBeStatic
-class DownloadCallback:
-
-    def before_album(self, album: JmAlbumDetail):
-        jm_debug('album-before',
-                 f'本子获取成功: [{album.id}], '
-                 f'作者: [{album.author}], '
-                 f'章节数: [{len(album)}], '
-                 f'标题: [{album.title}], '
-                 )
-
-    def after_album(self, album: JmAlbumDetail):
-        jm_debug('album-after', f'本子下载完成: [{album.id}]')
-
-    def before_photo(self, photo: JmPhotoDetail):
-        jm_debug('photo-before',
-                 f'开始下载章节: {photo.id} ({photo.album_id}[{photo.index}/{len(photo.from_album)}]), '
-                 f'标题: [{photo.title}], '
-                 f'图片数为[{len(photo)}]'
-                 )
-
-    def after_photo(self, photo: JmPhotoDetail):
-        jm_debug('photo-after',
-                 f'章节下载完成: {photo.id} ({photo.album_id}[{photo.index}/{len(photo.from_album)}])')
-
-    def before_image(self, image: JmImageDetail, img_save_path):
-        if image.is_exists:
-            jm_debug('image-before',
-                     f'图片已存在: {image.tag} ← [{img_save_path}]'
-                     )
-        else:
-            jm_debug('image-before',
-                     f'图片准备下载: {image.tag}, [{image.img_url}] → [{img_save_path}]'
-                     )
-
-    def after_image(self, image: JmImageDetail, img_save_path):
-        jm_debug('image-after',
-                 f'图片下载完成: {image.tag}, [{image.img_url}] → [{img_save_path}]')
-
-
 class DirRule:
     rule_sample = [
         # 根目录 / Album-id / Photo-序号 /
         'Bd_Aid_Pindex',  # 禁漫网站的默认下载方式
         # 根目录 / Album-作者 / Album-标题 / Photo-序号 /
         'Bd_Aauthor_Atitle_Pindex',
         # 根目录 / Photo-序号&标题 /
@@ -135,15 +95,15 @@
     def parse_dsl(self, base_dir: str):
         for k, func in self.dsl_support.items():
             if k in base_dir:
                 base_dir = base_dir.replace(k, func(base_dir))
         return base_dir
 
 
-class JmOption(DownloadCallback):
+class JmOption:
     JM_OP_VER = '2.0'
 
     def __init__(self,
                  dir_rule: Dict,
                  download: Dict,
                  client: Dict,
                  filepath=None,
```

### Comparing `jmcomic-2.1.6/src/jmcomic/jm_toolkit.py` & `jmcomic-2.1.7/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.6/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.1.7/src/jmcomic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

