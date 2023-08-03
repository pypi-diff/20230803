# Comparing `tmp/blue-krill-1.2.3.tar.gz` & `tmp/blue_krill-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue-krill-1.2.3.tar", max compression
+gzip compressed data, was "blue_krill-1.2.4.tar", max compression
```

## Comparing `blue-krill-1.2.3.tar` & `blue_krill-1.2.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0    21760 2022-09-22 07:55:01.307910 blue-krill-1.2.3/README.md
--rw-r--r--   0        0        0      782 2022-09-22 07:55:01.263910 blue-krill-1.2.3/blue_krill/__init__.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/async_utils/__init__.py
--rw-r--r--   0        0        0     1755 2022-09-22 07:55:01.303910 blue-krill-1.2.3/blue_krill/async_utils/django_utils.py
--rw-r--r--   0        0        0    11538 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/async_utils/poll_task.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/auth/__init__.py
--rw-r--r--   0        0        0     6068 2022-05-18 08:54:02.000000 blue-krill-1.2.3/blue_krill/auth/client.py
--rw-r--r--   0        0        0     2683 2022-09-22 07:55:01.263910 blue-krill-1.2.3/blue_krill/auth/jwt.py
--rw-r--r--   0        0        0     1629 2022-05-18 08:54:02.000000 blue-krill-1.2.3/blue_krill/auth/utils.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/connections/__init__.py
--rw-r--r--   0        0        0      824 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/connections/exceptions.py
--rw-r--r--   0        0        0     1718 2022-07-05 06:19:05.000000 blue-krill-1.2.3/blue_krill/connections/ha_algorithm.py
--rw-r--r--   0        0        0     7147 2022-07-05 06:19:05.000000 blue-krill-1.2.3/blue_krill/connections/ha_endpoint_pool.py
--rw-r--r--   0        0        0     1457 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/contextlib.py
--rw-r--r--   0        0        0     6964 2022-03-22 07:12:57.000000 blue-krill-1.2.3/blue_krill/cubing_case.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/data_types/__init__.py
--rw-r--r--   0        0        0     8652 2022-05-05 11:53:08.000000 blue-krill-1.2.3/blue_krill/data_types/enum.py
--rw-r--r--   0        0        0     3603 2022-09-22 07:55:01.263910 blue-krill-1.2.3/blue_krill/data_types/url.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/editions/__init__.py
--rw-r--r--   0        0        0    21379 2022-05-05 11:53:08.000000 blue-krill-1.2.3/blue_krill/editions/editionctl.py
--rw-r--r--   0        0        0     2777 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/encoding.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/encrypt/__init__.py
--rw-r--r--   0        0        0     1993 2022-05-05 11:53:08.000000 blue-krill-1.2.3/blue_krill/encrypt/handler.py
--rw-r--r--   0        0        0     2399 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/encrypt/legacy.py
--rw-r--r--   0        0        0     1699 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/encrypt/utils.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/models/__init__.py
--rw-r--r--   0        0        0      867 2022-05-05 11:53:08.000000 blue-krill-1.2.3/blue_krill/models/better_loaddata/__init__.py
--rw-r--r--   0        0        0      882 2022-05-05 11:53:08.000000 blue-krill-1.2.3/blue_krill/models/better_loaddata/apps.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/models/better_loaddata/management/__init__.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/models/better_loaddata/management/commands/__init__.py
--rw-r--r--   0        0        0     5000 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/models/better_loaddata/management/commands/better_loaddata.py
--rw-r--r--   0        0        0     1686 2022-05-05 11:53:08.000000 blue-krill-1.2.3/blue_krill/models/fields.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/monitoring/__init__.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/monitoring/probe/__init__.py
--rw-r--r--   0        0        0     3827 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/monitoring/probe/base.py
--rw-r--r--   0        0        0      906 2022-05-05 11:53:08.000000 blue-krill-1.2.3/blue_krill/monitoring/probe/exceptions.py
--rw-r--r--   0        0        0     3723 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/monitoring/probe/http.py
--rw-r--r--   0        0        0     2874 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/monitoring/probe/mysql.py
--rw-r--r--   0        0        0     2906 2022-09-22 07:55:01.263910 blue-krill-1.2.3/blue_krill/monitoring/probe/redis.py
--rw-r--r--   0        0        0     1908 2022-04-05 03:07:53.000000 blue-krill-1.2.3/blue_krill/monitoring/probe/tcp.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/monitoring/prometheus/__init__.py
--rw-r--r--   0        0        0     5004 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/monitoring/prometheus/django_utils.py
--rw-r--r--   0        0        0     1344 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/monitoring/prometheus/setups.py
--rw-r--r--   0        0        0        0 2022-05-05 11:53:08.000000 blue-krill-1.2.3/blue_krill/py.typed
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/redis_tools/__init__.py
--rw-r--r--   0        0        0     6517 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/redis_tools/messaging.py
--rw-r--r--   0        0        0     3748 2022-09-22 07:55:01.263910 blue-krill-1.2.3/blue_krill/redis_tools/sentinel.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/secure/__init__.py
--rw-r--r--   0        0        0     3886 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/secure/bk_secure.py
--rw-r--r--   0        0        0     2233 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/secure/dj_environ.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/storages/__init__.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/storages/blobstore/__init__.py
--rw-r--r--   0        0        0     4045 2022-02-14 08:28:27.000000 blue-krill-1.2.3/blue_krill/storages/blobstore/base.py
--rw-r--r--   0        0        0    13903 2022-06-28 02:47:08.000000 blue-krill-1.2.3/blue_krill/storages/blobstore/bkrepo.py
--rw-r--r--   0        0        0     1910 2022-06-28 02:47:08.000000 blue-krill-1.2.3/blue_krill/storages/blobstore/exceptions.py
--rw-r--r--   0        0        0     6262 2022-02-14 08:28:27.000000 blue-krill-1.2.3/blue_krill/storages/blobstore/s3.py
--rw-r--r--   0        0        0    10889 2022-02-14 06:09:36.000000 blue-krill-1.2.3/blue_krill/termcolors.py
--rw-r--r--   0        0        0     1666 2022-05-31 11:39:52.000000 blue-krill-1.2.3/blue_krill/text.py
--rw-r--r--   0        0        0      760 2021-11-30 08:29:35.000000 blue-krill-1.2.3/blue_krill/web/__init__.py
--rw-r--r--   0        0        0     9697 2022-05-05 11:53:08.000000 blue-krill-1.2.3/blue_krill/web/drf_utils.py
--rw-r--r--   0        0        0     5644 2022-05-18 08:54:02.000000 blue-krill-1.2.3/blue_krill/web/std_error.py
--rw-r--r--   0        0        0     1971 2022-09-22 07:55:27.475910 blue-krill-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    24193 2022-09-22 08:00:10.141089 blue-krill-1.2.3/setup.py
--rw-r--r--   0        0        0    22759 2022-09-22 08:00:10.142711 blue-krill-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    23858 2023-08-02 13:04:17.193081 blue_krill-1.2.4/README.md
+-rw-r--r--   0        0        0      782 2023-08-02 13:04:17.193420 blue_krill-1.2.4/blue_krill/__init__.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.193703 blue_krill-1.2.4/blue_krill/async_utils/__init__.py
+-rw-r--r--   0        0        0     1755 2023-08-02 13:04:17.193969 blue_krill-1.2.4/blue_krill/async_utils/django_utils.py
+-rw-r--r--   0        0        0    11538 2023-08-02 13:04:17.194204 blue_krill-1.2.4/blue_krill/async_utils/poll_task.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.194514 blue_krill-1.2.4/blue_krill/auth/__init__.py
+-rw-r--r--   0        0        0     6068 2023-08-02 13:04:17.194834 blue_krill-1.2.4/blue_krill/auth/client.py
+-rw-r--r--   0        0        0     2683 2023-08-02 13:04:17.195041 blue_krill-1.2.4/blue_krill/auth/jwt.py
+-rw-r--r--   0        0        0     1629 2023-08-02 13:04:17.195261 blue_krill-1.2.4/blue_krill/auth/utils.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.195527 blue_krill-1.2.4/blue_krill/connections/__init__.py
+-rw-r--r--   0        0        0      824 2023-08-02 13:04:17.195756 blue_krill-1.2.4/blue_krill/connections/exceptions.py
+-rw-r--r--   0        0        0     1718 2023-08-02 13:04:17.195978 blue_krill-1.2.4/blue_krill/connections/ha_algorithm.py
+-rw-r--r--   0        0        0     7147 2023-08-02 13:04:17.196219 blue_krill-1.2.4/blue_krill/connections/ha_endpoint_pool.py
+-rw-r--r--   0        0        0     1457 2023-08-02 13:04:17.196447 blue_krill-1.2.4/blue_krill/contextlib.py
+-rw-r--r--   0        0        0     6964 2023-08-02 13:04:17.196709 blue_krill-1.2.4/blue_krill/cubing_case.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.196968 blue_krill-1.2.4/blue_krill/data_types/__init__.py
+-rw-r--r--   0        0        0     8652 2023-08-02 13:04:17.197243 blue_krill-1.2.4/blue_krill/data_types/enum.py
+-rw-r--r--   0        0        0     3603 2023-08-02 13:04:17.197452 blue_krill-1.2.4/blue_krill/data_types/url.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.197717 blue_krill-1.2.4/blue_krill/editions/__init__.py
+-rw-r--r--   0        0        0    21379 2023-08-02 13:04:17.198010 blue_krill-1.2.4/blue_krill/editions/editionctl.py
+-rw-r--r--   0        0        0     2777 2023-08-02 13:04:17.198279 blue_krill-1.2.4/blue_krill/encoding.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.198612 blue_krill-1.2.4/blue_krill/encrypt/__init__.py
+-rw-r--r--   0        0        0     4258 2023-08-02 13:04:17.198893 blue_krill-1.2.4/blue_krill/encrypt/handler.py
+-rw-r--r--   0        0        0     2399 2023-08-02 13:04:17.199144 blue_krill-1.2.4/blue_krill/encrypt/legacy.py
+-rw-r--r--   0        0        0     1980 2023-08-02 13:04:17.199393 blue_krill-1.2.4/blue_krill/encrypt/utils.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.199663 blue_krill-1.2.4/blue_krill/models/__init__.py
+-rw-r--r--   0        0        0      867 2023-08-02 13:04:17.199952 blue_krill-1.2.4/blue_krill/models/better_loaddata/__init__.py
+-rw-r--r--   0        0        0      882 2023-08-02 13:04:17.200149 blue_krill-1.2.4/blue_krill/models/better_loaddata/apps.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.200477 blue_krill-1.2.4/blue_krill/models/better_loaddata/management/__init__.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.200756 blue_krill-1.2.4/blue_krill/models/better_loaddata/management/commands/__init__.py
+-rw-r--r--   0        0        0     5000 2023-08-02 13:04:17.200954 blue_krill-1.2.4/blue_krill/models/better_loaddata/management/commands/better_loaddata.py
+-rw-r--r--   0        0        0     1727 2023-08-02 13:04:17.201163 blue_krill-1.2.4/blue_krill/models/fields.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.201456 blue_krill-1.2.4/blue_krill/monitoring/__init__.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.201743 blue_krill-1.2.4/blue_krill/monitoring/probe/__init__.py
+-rw-r--r--   0        0        0     3827 2023-08-02 13:04:17.201968 blue_krill-1.2.4/blue_krill/monitoring/probe/base.py
+-rw-r--r--   0        0        0      906 2023-08-02 13:04:17.202228 blue_krill-1.2.4/blue_krill/monitoring/probe/exceptions.py
+-rw-r--r--   0        0        0     3723 2023-08-02 13:04:17.202424 blue_krill-1.2.4/blue_krill/monitoring/probe/http.py
+-rw-r--r--   0        0        0     2874 2023-08-02 13:04:17.202664 blue_krill-1.2.4/blue_krill/monitoring/probe/mysql.py
+-rw-r--r--   0        0        0     2906 2023-08-02 13:04:17.202887 blue_krill-1.2.4/blue_krill/monitoring/probe/redis.py
+-rw-r--r--   0        0        0     1908 2023-08-02 13:04:17.203106 blue_krill-1.2.4/blue_krill/monitoring/probe/tcp.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.203374 blue_krill-1.2.4/blue_krill/monitoring/prometheus/__init__.py
+-rw-r--r--   0        0        0     5004 2023-08-02 13:04:17.203600 blue_krill-1.2.4/blue_krill/monitoring/prometheus/django_utils.py
+-rw-r--r--   0        0        0     1344 2023-08-02 13:04:17.203851 blue_krill-1.2.4/blue_krill/monitoring/prometheus/setups.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:04:17.204016 blue_krill-1.2.4/blue_krill/py.typed
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.204266 blue_krill-1.2.4/blue_krill/redis_tools/__init__.py
+-rw-r--r--   0        0        0     6517 2023-08-02 13:04:17.204508 blue_krill-1.2.4/blue_krill/redis_tools/messaging.py
+-rw-r--r--   0        0        0     3748 2023-08-02 13:04:17.204720 blue_krill-1.2.4/blue_krill/redis_tools/sentinel.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.205029 blue_krill-1.2.4/blue_krill/secure/__init__.py
+-rw-r--r--   0        0        0     3886 2023-08-02 13:04:17.205245 blue_krill-1.2.4/blue_krill/secure/bk_secure.py
+-rw-r--r--   0        0        0     2233 2023-08-02 13:04:17.205463 blue_krill-1.2.4/blue_krill/secure/dj_environ.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.205758 blue_krill-1.2.4/blue_krill/storages/__init__.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.206033 blue_krill-1.2.4/blue_krill/storages/blobstore/__init__.py
+-rw-r--r--   0        0        0     4045 2023-08-02 13:04:17.206244 blue_krill-1.2.4/blue_krill/storages/blobstore/base.py
+-rw-r--r--   0        0        0    13906 2023-08-02 13:04:17.206477 blue_krill-1.2.4/blue_krill/storages/blobstore/bkrepo.py
+-rw-r--r--   0        0        0     1910 2023-08-02 13:04:17.206671 blue_krill-1.2.4/blue_krill/storages/blobstore/exceptions.py
+-rw-r--r--   0        0        0     6262 2023-08-02 13:04:17.206852 blue_krill-1.2.4/blue_krill/storages/blobstore/s3.py
+-rw-r--r--   0        0        0    10889 2023-08-02 13:04:17.207016 blue_krill-1.2.4/blue_krill/termcolors.py
+-rw-r--r--   0        0        0     1666 2023-08-02 13:04:17.207221 blue_krill-1.2.4/blue_krill/text.py
+-rw-r--r--   0        0        0      760 2023-08-02 13:04:17.207552 blue_krill-1.2.4/blue_krill/web/__init__.py
+-rw-r--r--   0        0        0     9697 2023-08-02 13:04:17.207773 blue_krill-1.2.4/blue_krill/web/drf_utils.py
+-rw-r--r--   0        0        0     5644 2023-08-02 13:04:17.207965 blue_krill-1.2.4/blue_krill/web/std_error.py
+-rw-r--r--   0        0        0     2003 2023-08-02 13:04:17.208818 blue_krill-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    26390 1970-01-01 00:00:00.000000 blue_krill-1.2.4/setup.py
+-rw-r--r--   0        0        0    24911 1970-01-01 00:00:00.000000 blue_krill-1.2.4/PKG-INFO
```

### Comparing `blue-krill-1.2.3/README.md` & `blue_krill-1.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -585,14 +585,62 @@
 r = backend.client
 
 r.set('foo', 'bar')
 # 获得 b'bar'
 r.get('foo')
 ```
 
+### 10 blue_krill.encrypt.handler
+`blue_krill.encrypt.handler` 提够 Fernet 和 SM4 两种对称加密算法，并且为了适应存量数据，在解密时会根据`header`选择相应的算法进行解密。
+具体的使用方式如下:
+
+```python
+from blue_krill.encrypt.handler import EncryptHandler
+
+# 实例化
+# 第一种方式通过传入 encrypt_cipher_type(加密算法类型) 和 secret_key(密钥)
+# encrypt_cipher_type 现有的就是 "FernetCipher" 和 "SM4CTR"，分别对应 Fernet 和 SM4 对称加密算法
+encrypt_handler = EncryptHandler(encrypt_cipher_type='FernetCipher', secret_key=b'PIMCuSRiVqBg5eSzQqZZrOhGFSUtrlS-8_JlIpjHt0A=')
+# 第二种方式，不传入参数时，即 encrypt_cipher_type 和 secret_key 为 None 
+# 会分别通过 django setting 中的 ENCRYPT_CIPHER_TYPE 和 BKKRILL_ENCRYPT_SECRET_KEY 字段设置。
+encrypt_handler = EncryptHandler()
+
+# 加解密使用
+text = "random_text"
+# 加密，根据选择的算法不同，header 也会不同，算法为 Fernet 加密头为 bkcrypt$，算法为 SM4 时，加密头为 sm4ctr$
+# encrypted = "bkcrypt$gAAAAABkyIHPPbOeAOLa3LMc8901rslfBeTdm3rWZntSz5ut7eIDyb9eDgPmzVtL3y-iUBPSxRtZLC2ynlmeKeCNmRmTHpjtWg=="
+# encrypted = "sm4ctr$KI9M5PrhDCmj5ix90OKg/5qYLcR8F3owLlsG"
+encrypted = encrypt_handler.encrypt(text)
+# 解密
+# decrypted = "random_text"
+decrypted = encrypt_handler.decrypt(encrypted)
+```
+
+### 11 blue_krill.models.fields
+`blue_krill.models.fields` 基于 `EncryptHandler` 实现了 `EncryptField`，具体使用：
+```python
+from django.db import models
+from blue_krill.models.fields import EncryptField
+
+
+class User(models.Model):
+    """
+    User.password 在存取时会做加解密
+    """
+    
+    name = models.CharField(max_length=30)
+    # EncryptField 用法与 EncryptHandler 类似
+    # 实例化时，可传入 encrypt_cipher_type 选择加密算法，secret_key 配置密钥
+    # 不传入时，会分别通过 django setting 中的 ENCRYPT_CIPHER_TYPE 和 BKKRILL_ENCRYPT_SECRET_KEY 字段设置。
+    password = EncryptField()
+
+    def __str__(self):
+        return self.name
+```
+
 ## 开发指南
 
 首先安装 [poetry](https://github.com/python-poetry/poetry)，之后在项目目录下执行 `poetry env use python3.6` 初始化开发用虚拟环境。然后用 `poetry shell` 命令激活虚拟环境。
 
 - 执行 `poetry install` 安装所有依赖
 - 使用 `pytest -s .` 执行所有单元测试
```

### Comparing `blue-krill-1.2.3/blue_krill/__init__.py` & `blue_krill-1.2.4/blue_krill/models/better_loaddata/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,8 +4,9 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
-__version__ = '1.2.2'
+# -*- coding: utf-8 -*-
+default_app_config = 'blue_krill.models.better_loaddata.apps.BetterLoadDataConfig'
```

### Comparing `blue-krill-1.2.3/blue_krill/async_utils/__init__.py` & `blue_krill-1.2.4/blue_krill/async_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/async_utils/django_utils.py` & `blue_krill-1.2.4/blue_krill/async_utils/django_utils.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/async_utils/poll_task.py` & `blue_krill-1.2.4/blue_krill/async_utils/poll_task.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/auth/__init__.py` & `blue_krill-1.2.4/blue_krill/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/auth/client.py` & `blue_krill-1.2.4/blue_krill/auth/client.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/auth/jwt.py` & `blue_krill-1.2.4/blue_krill/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/auth/utils.py` & `blue_krill-1.2.4/blue_krill/auth/utils.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/connections/__init__.py` & `blue_krill-1.2.4/blue_krill/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/connections/exceptions.py` & `blue_krill-1.2.4/blue_krill/connections/exceptions.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/connections/ha_algorithm.py` & `blue_krill-1.2.4/blue_krill/connections/ha_algorithm.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/connections/ha_endpoint_pool.py` & `blue_krill-1.2.4/blue_krill/connections/ha_endpoint_pool.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/contextlib.py` & `blue_krill-1.2.4/blue_krill/contextlib.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/cubing_case.py` & `blue_krill-1.2.4/blue_krill/cubing_case.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/data_types/__init__.py` & `blue_krill-1.2.4/blue_krill/data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/data_types/enum.py` & `blue_krill-1.2.4/blue_krill/data_types/enum.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/data_types/url.py` & `blue_krill-1.2.4/blue_krill/data_types/url.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/editions/__init__.py` & `blue_krill-1.2.4/blue_krill/editions/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/editions/editionctl.py` & `blue_krill-1.2.4/blue_krill/editions/editionctl.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/encoding.py` & `blue_krill-1.2.4/blue_krill/encoding.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/encrypt/__init__.py` & `blue_krill-1.2.4/blue_krill/encrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/encrypt/legacy.py` & `blue_krill-1.2.4/blue_krill/encrypt/legacy.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/encrypt/utils.py` & `blue_krill-1.2.4/blue_krill/encrypt/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,26 @@
 
         return settings.BKKRILL_ENCRYPT_SECRET_KEY
     except ImportError:
         logger.exception("you should supply a default secret key")
         raise
 
 
+def get_default_encrypt_cipher_type():
+    """获取默认的加密算法"""
+
+    try:
+        from django.conf import settings
+
+        return settings.ENCRYPT_CIPHER_TYPE
+    except ImportError:
+        logger.exception("you should supply a encrypt cipher type")
+        raise
+
+
 def encrypt_string(s: str, key: Optional[bytes] = None) -> str:
     """Shortcut function: encrypt a string into a fernet token"""
     key = key or get_default_secret_key()
     f = Fernet(key)
     value = f.encrypt(force_bytes(s))
     return force_text(value)
```

### Comparing `blue-krill-1.2.3/blue_krill/models/__init__.py` & `blue_krill-1.2.4/blue_krill/models/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/models/better_loaddata/__init__.py` & `blue_krill-1.2.4/blue_krill/models/better_loaddata/apps.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,9 +4,12 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
-# -*- coding: utf-8 -*-
-default_app_config = 'blue_krill.models.better_loaddata.apps.BetterLoadDataConfig'
+from django.apps import AppConfig
+
+
+class BetterLoadDataConfig(AppConfig):
+    name = "blue_krill.models.better_loaddata"
```

### Comparing `blue-krill-1.2.3/blue_krill/models/better_loaddata/apps.py` & `blue_krill-1.2.4/blue_krill/monitoring/probe/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,12 +4,12 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
-from django.apps import AppConfig
 
 
-class BetterLoadDataConfig(AppConfig):
-    name = "blue_krill.models.better_loaddata"
+class NoFatalIssueError(Exception):
+    def __init__(self, *args, **kwargs):
+        super().__init__("no exact fatal issue, please offer one")
```

### Comparing `blue-krill-1.2.3/blue_krill/models/better_loaddata/management/__init__.py` & `blue_krill-1.2.4/blue_krill/models/better_loaddata/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/models/better_loaddata/management/commands/__init__.py` & `blue_krill-1.2.4/blue_krill/models/better_loaddata/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/models/better_loaddata/management/commands/better_loaddata.py` & `blue_krill-1.2.4/blue_krill/models/better_loaddata/management/commands/better_loaddata.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/models/fields.py` & `blue_krill-1.2.4/blue_krill/models/fields.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,36 +4,35 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
+from typing import Optional
+
 from django.db import models
 
 from blue_krill.encrypt.handler import EncryptHandler
-from blue_krill.encrypt.utils import get_default_secret_key
 
 
 class EncryptField(models.TextField):
     """a field which will be encrypted via cryptography/fernet"""
 
     description = "a field which will be encrypted"
 
-    def __init__(self, secret_key: bytes = get_default_secret_key(), *args, **kwargs):
+    def __init__(self, encrypt_cipher_type: Optional[str] = None, secret_key: Optional[bytes] = None, *args, **kwargs):
         super(EncryptField, self).__init__(*args, **kwargs)
-        self.handler = EncryptHandler(secret_key=secret_key)
+        self.handler = EncryptHandler(encrypt_cipher_type=encrypt_cipher_type, secret_key=secret_key)
 
     def get_prep_value(self, value):
         if value is None:
             return value
-
         return self.handler.encrypt(value)
 
     def get_db_prep_value(self, value, connection, prepared=False):
         return self.get_prep_value(value)
 
     def from_db_value(self, value, expression, connection, context=None):
         if value is None:
             return value
-
         return self.handler.decrypt(value)
```

### Comparing `blue-krill-1.2.3/blue_krill/monitoring/__init__.py` & `blue_krill-1.2.4/blue_krill/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/monitoring/probe/__init__.py` & `blue_krill-1.2.4/blue_krill/monitoring/probe/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/monitoring/probe/base.py` & `blue_krill-1.2.4/blue_krill/monitoring/probe/base.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/monitoring/probe/exceptions.py` & `blue_krill-1.2.4/blue_krill/monitoring/prometheus/setups.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,12 +4,26 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
+import os
 
+MULTIPROC_ENV_NAME = 'prometheus_multiproc_dir'
+DEFAULT_DATA_PATH = '_prometheus_data'
 
-class NoFatalIssueError(Exception):
-    def __init__(self, *args, **kwargs):
-        super().__init__("no exact fatal issue, please offer one")
+
+def setup_multiproc_dir(data_path: str = DEFAULT_DATA_PATH):
+    """Setup multi processes directory
+
+    :param data_path: if MULTIPROC_ENV_NAME has already been configured in env vars, then the
+        data_path parameter won't be used at all
+    """
+    dirname = os.environ.setdefault(MULTIPROC_ENV_NAME, data_path)
+    try:
+        os.mkdir(dirname)
+    except FileExistsError:
+        pass
+    except IOError as e:
+        print(f'unable to make prometheus data directory: {e}')
```

### Comparing `blue-krill-1.2.3/blue_krill/monitoring/probe/http.py` & `blue_krill-1.2.4/blue_krill/monitoring/probe/http.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/monitoring/probe/mysql.py` & `blue_krill-1.2.4/blue_krill/monitoring/probe/mysql.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/monitoring/probe/redis.py` & `blue_krill-1.2.4/blue_krill/monitoring/probe/redis.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/monitoring/probe/tcp.py` & `blue_krill-1.2.4/blue_krill/monitoring/probe/tcp.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/monitoring/prometheus/__init__.py` & `blue_krill-1.2.4/blue_krill/monitoring/prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/monitoring/prometheus/django_utils.py` & `blue_krill-1.2.4/blue_krill/monitoring/prometheus/django_utils.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/monitoring/prometheus/setups.py` & `blue_krill-1.2.4/blue_krill/text.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,26 +4,37 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
-import os
+import sys
 
-MULTIPROC_ENV_NAME = 'prometheus_multiproc_dir'
-DEFAULT_DATA_PATH = '_prometheus_data'
+from blue_krill.data_types.url import MutableURL
 
 
-def setup_multiproc_dir(data_path: str = DEFAULT_DATA_PATH):
-    """Setup multi processes directory
+def remove_suffix(s: str, suffix: str) -> str:
+    """If given string endswith `suffix`, remove the suffix and return the new string"""
+    if sys.version_info >= (3, 9):
+        return s.removesuffix(suffix)
+    if s.endswith(suffix):
+        return s[: -len(suffix)]
+    return s
 
-    :param data_path: if MULTIPROC_ENV_NAME has already been configured in env vars, then the
-        data_path parameter won't be used at all
+
+def remove_prefix(s: str, prefix: str) -> str:
+    """If given string startswith `prefix`, remove the prefix and return the new string"""
+    if sys.version_info >= (3, 9):
+        return s.removeprefix(prefix)
+    if s.startswith(prefix):
+        return s[len(prefix) :]
+    return s
+
+
+def desensitize_url(url: str) -> str:
+    """Obscure the password field in the url
+
+    >>> desensitize_url("scheme://username:password@hostname:6666/path/?foo=bar")
+    "scheme://username:********@hostname:6666/path/?foo=bar"
     """
-    dirname = os.environ.setdefault(MULTIPROC_ENV_NAME, data_path)
-    try:
-        os.mkdir(dirname)
-    except FileExistsError:
-        pass
-    except IOError as e:
-        print(f'unable to make prometheus data directory: {e}')
+    return MutableURL(url).obscure()
```

### Comparing `blue-krill-1.2.3/blue_krill/redis_tools/__init__.py` & `blue_krill-1.2.4/blue_krill/redis_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/redis_tools/messaging.py` & `blue_krill-1.2.4/blue_krill/redis_tools/messaging.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/redis_tools/sentinel.py` & `blue_krill-1.2.4/blue_krill/redis_tools/sentinel.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/secure/__init__.py` & `blue_krill-1.2.4/blue_krill/secure/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/secure/bk_secure.py` & `blue_krill-1.2.4/blue_krill/secure/bk_secure.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/secure/dj_environ.py` & `blue_krill-1.2.4/blue_krill/secure/dj_environ.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/storages/__init__.py` & `blue_krill-1.2.4/blue_krill/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/storages/blobstore/__init__.py` & `blue_krill-1.2.4/blue_krill/storages/blobstore/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/storages/blobstore/base.py` & `blue_krill-1.2.4/blue_krill/storages/blobstore/base.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/storages/blobstore/bkrepo.py` & `blue_krill-1.2.4/blue_krill/storages/blobstore/bkrepo.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,30 +93,30 @@
         :params password str: 密码
         :params association_users List[str]: 关联的真实用户
         :params repo str: 关联的仓库名称
         """
         client = self.get_client()
         url = urljoin(self.endpoint_url, '/auth/api/user/create/repo')
         data = {
-            "admin": True,
+            "admin": False,
             "name": username,
             "pwd": password,
             "userId": username,
             "asstUsers": association_users,
             "group": False,
             "projectId": project,
             "repoName": repo,
         }
         return _validate_resp(client.post(url, json=data, timeout=TIMEOUT_THRESHOLD))
 
     def update_user(self, username: str, password: str, association_users: List[str]):
         """更新用户信息"""
         client = self.get_client()
         url = urljoin(self.endpoint_url, f'/auth/api/user/{username}')
-        data = {"admin": True, "name": username, "pwd": password, "asstUsers": association_users}
+        data = {"admin": False, "name": username, "pwd": password, "asstUsers": association_users}
         return _validate_resp(client.put(url, json=data, timeout=TIMEOUT_THRESHOLD))
 
     def delete_user(self, username: str):
         """删除用户"""
         client = self.get_client()
         url = urljoin(self.endpoint_url, f'/auth/api/user/{username}')
         return _validate_resp(client.delete(url, timeout=TIMEOUT_THRESHOLD))
@@ -169,15 +169,15 @@
         :params password str: 密码
         :params association_users List[str]: 关联的真实用户
         :params project str: 关联的项目名称
         """
         client = self.get_client()
         url = urljoin(self.endpoint_url, '/auth/api/user/create/project')
         data = {
-            "admin": True,
+            "admin": False,
             "name": username,
             "pwd": password,
             "userId": username,
             "asstUsers": association_users,
             "group": False,
             "projectId": project,
         }
```

### Comparing `blue-krill-1.2.3/blue_krill/storages/blobstore/exceptions.py` & `blue_krill-1.2.4/blue_krill/storages/blobstore/exceptions.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/storages/blobstore/s3.py` & `blue_krill-1.2.4/blue_krill/storages/blobstore/s3.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/termcolors.py` & `blue_krill-1.2.4/blue_krill/termcolors.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/web/__init__.py` & `blue_krill-1.2.4/blue_krill/web/__init__.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/web/drf_utils.py` & `blue_krill-1.2.4/blue_krill/web/drf_utils.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/blue_krill/web/std_error.py` & `blue_krill-1.2.4/blue_krill/web/std_error.py`

 * *Files identical despite different names*

### Comparing `blue-krill-1.2.3/pyproject.toml` & `blue_krill-1.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blue-krill"
-version = "1.2.3"
+version = "1.2.4"
 description = "Tools and common packages for blueking paas"
 license = "Apache License 2.0"
 readme = "README.md"
 authors = ["blueking"]
 include = ["blue_krill/py.typed"]
 
 [tool.poetry.dependencies]
@@ -17,14 +17,15 @@
 six = "*"
 click = "*"
 pydantic = "^1.7"
 toml = "*"
 python-editor = "^1.0.4"
 watchdog = "^1.0.2"
 curlify = "^2.2.1"
+bk-crypto-python-sdk = "^1.0.4"
 
 [tool.poetry.dev-dependencies]
 redis = "^3.5.3"
 django = "^3.2.0"
 tox = "^3.18.1"
 requests_mock = "^1.8.0"
 requests-mock = "^1.8.0"
```

### Comparing `blue-krill-1.2.3/setup.py` & `blue_krill-1.2.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,16 @@
  'blue_krill.storages.blobstore',
  'blue_krill.web']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click',
+['bk-crypto-python-sdk>=1.0.4,<2.0.0',
+ 'click',
  'cryptography>=3.0.0,<4.0.0',
  'curlify>=2.2.1,<3.0.0',
  'django-environ>=0.8.1,<0.9.0',
  'pydantic>=1.7,<2.0',
  'pyjwt>=1.7.1',
  'python-editor>=1.0.4,<2.0.0',
  'requests',
@@ -43,22 +44,22 @@
 
 entry_points = \
 {'console_scripts': ['bk-secure = blue_krill.secure.bk_secure:main',
                      'editionctl = blue_krill.editions.editionctl:main']}
 
 setup_kwargs = {
     'name': 'blue-krill',
-    'version': '1.2.3',
+    'version': '1.2.4',
     'description': 'Tools and common packages for blueking paas',
-    'long_description': '# Blue krill\n\nPython 常用工具包模块。\n\n## 使用指南\n\n### 1. blue_krill.secure\n\n加解密、安全相关的工具与模块。\n\n#### 1.1 dj_environ 模块\n\ndj_environ 的主要目的是在 [django-environ](https://github.com/joke2k/django-environ) 之上，增加可以阅读加密环境变量的能力。如需使用，首先需要设置密文环境变量：\n\n```bash\nexport DATABASE_URL=\'<使用 bk-secure 加密后的字符串>\'\nexport FOO=\'<使用 bk-secure 加密后的字符串>\'\n```\n\n然后在 `settings` 模块中，初始化 `SecureEnv` 对象并使用它读取对应配置：\n\n```python\nfrom blue_krill.secure.dj_environ import SecureEnv\n\n# 初始化并加载 .env 文件内容\nsec_env = SecureEnv()\nenviron.Env.read_env()\n\n# 读取为数据库配置\nDATABASES[\'default\'] = sec_env.db()\n\n# 读取为普通配置\nFOO = sec_env(\'FOO\')\n```\n\n#### 1.2 bk-secure 脚本\n\nbk-secure 主要用于配合 dj_environ 模块生成加密环境变量（或配置文件）。使用前，先将 `BK_FERNET_KEY` 设为你所使用的加密 key。一般情况下，这个值等同于 Django 项目的 `BKKRILL_ENCRYPT_SECRET_KEY` 配置项：\n\n```\nexport BK_FERNET_KEY=\'... ...\'\n```\n\n执行 `encrypt` 加密某段明文：\n\n```console\n❯ bk-secure encrypt\nInput string: mysql://u:p@localhost/foo\nThe encrypted token is: gAAAAABfKUtKIBzYc_gyQL-j9TmI35O1d0auLQfYeso6D8Q77ZC9PIuv26ABPFlOQSSPDzT3HcVrhI1K3XwU5Xfs6gP6iAe8RhEAJJhMktp7CKzn7p7imNk=\n```\n\n执行 `decrypt` 解密某段密文：\n\n```console\n❯ bk-secure decrypt\nInput token: gAAAAABfKUtKIBzYc_gyQL-j9TmI35O1d0auLQfYeso6D8Q77ZC9PIuv26ABPFlOQSSPDzT3HcVrhI1K3XwU5Xfs6gP6iAe8RhEAJJhMktp7CKzn7p7imNk=\nThe decrypted result is: mysql://u:p@localhost/foo\n```\n\n使用 `edit` 以明文方式编辑某段密文，并输出新的密文：\n\n```console\n❯ bk-secure edit\nInput token: gAAAAABfKUtKIBzYc_gyQL-j9TmI35O1d0auLQfYeso6D8Q77ZC9PIuv26ABPFlOQSSPDzT3HcVrhI1K3XwU5Xfs6gP6iAe8RhEAJJhMktp7CKzn7p7imNk=\n# 将弹出编辑器界面修改明文，可通过 $EDITOR 环境变量设置编辑器\nThe new value is: mysql://u:p@localhost/foo2\nThe encrypted new value is: gAAAAABfKUui5_YUVxoYEYQG61RSRX1Ll3s1dgkZ5nUEJbCxakWHSyo3AKZFv3GuoQ7cH2Hm5LEU2QDK8C3G-_iog0TmqSbVkIYf0WnksH2DGgedldfbwhs=\n```\n\n### 2. blue_krill.editions\n\n多版本开发相关工具模块\n\n#### 2.1 editionctl 工具\n\n`editonctl` 是用来帮助开发需要支持多版本 Python 项目的工具，使用该工具前，请先把你的项目目录组织成下面这种结构：\n\n```raw\n├── editionctl.toml\n├── editions\n│\xa0\xa0 ├── ee\n│\xa0\xa0 │\xa0\xa0 └── ee.py\n│\xa0\xa0 └── te\n│\xa0\xa0     └── te.py\n└── main\n    └── main.py\n```\n\n其中：\n\n- `editions`：仅保存不同版本所特有的源码文件\n- `main`：项目主目录\n\n#### 2.1.1 创建配置文件\n\n要使用 `editonctl`，首先需要在项目内创建配置文件 `editionctl.toml`。比如，针对上面的项目结构，我们可以创建这样的配置文件：\n\n```toml\n# 项目主目录\nproject_root = \'main\'\n# 项目各版本所在目录\neditions_root = \'editions\'\n\n[[editions]]\n# 版本名称\nname = "TE"\n# 版本相对路径\nrel_directory = \'te\'\n\n[[editions]]\nname = "EE"\nrel_directory = \'ee\'\n```\n\n> 更多配置文件相关说明，可执行 `editionctl help` 查看。\n\n#### 2.1.2 在版本之间切换\n\n在不同版本间切换，需要使用 `editionctl activate {EDITION_NAME}` 命令。执行该命令后，工具会将指定版本下的所有源码文件，拷贝到 `project_root` 中。\n\n```bash\n$ editionctl activate EE\n[2020-12-17 16:51:37,312] INFO: Edition EE activated, linker is default\n```\n\n> 为了避免由工具拷贝的文件被意外提交到源码仓库，这些文件会被添加到 `{project_root}/.gitignore` 中。\n\n#### 2.1.3 重置多版本\n\n假如你想要清除所有由 `editionctl` 工具创建的源码文件，可以执行 `editionctl reset` 命令。执行该命令将删除所有多版本相关文件，只保留主目录。\n\n#### 2.1.4 进入开发模式\n\n在开发多版本项目时，`editions_root` 目录下的当前版本相关文件会被频繁修改。正常情况下，每次修改版本文件后，我们都要手动重新执行 `activate` 命令重新同步文件。\n\n为了简化这个过程，我们可以使用 `editionctl develop`。\n\n执行 `editionctl develop` 命令后，工具将会持续监听当前 `edition` 目录下的任何改动。如果监听到新改动，则自动触发同步机制。\n\n```\n$ editionctl develop\n[2020-12-17 16:56:34,385] INFO: Start watching editions/ee directory for edition EE...\n```\n\n### 3. blue_krill.data_types.enum\n\n枚举相关的数据类型。\n\n### 3.1 FeatureFlag\n\n功能标记(Feature Flag)用于控制当前用户能否感知到某个功能/特性，只提供**开启(enabled)**和**关闭(disabled)**两个状态, 分别对应于布尔值的 True/Flase。\n为了避免各项目重复造轮子, blue_krill 抽象出通用的 FeatureFlag 模型, 同时也提供类似于`枚举(Enum)`的API, 降低使用成本。\n\n#### 3.1.1 如何定义 FeatureFlag\n\n就像定义普通的 Python Class 一样, 定义 FeatureFlag 只需要继承 `blue_krill.data_types.enum::FeatureFlag` 即可。\n```python\nfrom blue_krill.data_types.enum import FeatureFlag, FeatureFlagField\n\n\nclass UserFeatureFlag(FeatureFlag):\n    # 使用类属性声明 FeatureFlagField 时, name 属性会通过描述符协议自动设置, 无需额外指定.\n    WEBCONSOLE = FeatureFlagField(label="使用 WEBConsole")\n    CREATE_SMART_APP = FeatureFlagField(label="创建 Smart 应用")\n    ...\n```\n\n#### 3.1.2 如何添加额外的 FeatureFlag\n\n不同于`枚举值(Enum)`, FeatureFlag 允许在运行过程中动态添加额外的字段或修改已有字段的默认值。\n\n```python\n# 添加额外的 FeatureFlag 时, 需要制定对应的名称.\nUserFeatureFlag.register_feature_flag(FeatureFlagField(name="CHOOSE_SOURCE_ORIGIN", label="选择源码来源"))\n```\n\n### 3.2 StructuredEnum\n\n考虑到我们使用`枚举值(Enum)`时, 往往会给枚举值添加额外的描述字段，为了避免各项目重复造轮子，blue_krill 基于 `Enum` 实现了 StructuredEnum，可以基于配套的 `EnumField` 定义带有额外描述内容的枚举值。\n\n```python\nfrom blue_krill.data_types.enum import EnumField, StructuredEnum\n\n\nclass DiffType(str, StructuredEnum):\n    ADDED = EnumField("added", label="新增")\n    DELETED = EnumField("deleted", label="删除")\n    NOT_MODIFIED = EnumField("not_modified", label="未改动")\n```\n\n### 4. blue_krill.storages.blobstore\n\n对象存储服务的简单封装, 目前支持 **上传**, **下载**, **生成预签名URL** 三个接口.\n\n#### 4.1 S3Store\n\nS3 协议的 BlobStore 实现, 使用时需要额外安装 boto3==\'^1.4.3\', 可参考以下代码进行实例化:\n```python\nfrom blue_krill.storages.blobstore.s3 import S3Store\n\n\nstore = S3Store(\n    bucket="your-bucket",\n    aws_access_key_id=\'your-access-key\',\n    aws_secret_access_key=\'your-secret-key\',\n    endpoint_url=\'your-s3-endpoint\',\n    # Optional\n    region_name=\'your-region, default is `us-east-1`\',\n    signature_version=\'your-signature-version, default is s3v4\',\n)\n```\n\n#### 4.2 BKGenericRepo\n\n底层服务是 **蓝鲸通用二进制仓库** 的底层实现, 可参考以下代码进行实例化:\n\n```python\nfrom blue_krill.storages.blobstore.bkrepo import BKGenericRepo\n\n\nstore = BKGenericRepo(\n    bucket=\'your-bucket\',\n    project=\'your-project-id\',\n    endpoint_url=\'\',\n)\n```\n\n### 5. blue_krill.web\n\n`blue_krill.web` 主要存放与 Web 开发有关的工具集。\n\n#### 5.1 blue_krill.web.std_error\n\n该模块内包含标准的错误码功能。`std_error` 最常见的用法，是通过 `ErrorCode` 定义一套错误码集合：\n\n```python\nfrom blue_krill.web.std_error import ErrorCode\n\nclass ErrorCodes:\n    CREATE_ERROR = ErrorCode(\'创建失败\')\n    DELETE_ERROR = ErrorCode(\'删除失败\')\n\n# 实例化一个全局对象\nerror_codes = ErrorCodes()\n```\n\n当你要抛出某个特定错误时，可以使用下面的语句：\n\n```python\nraise error_codes.CREATE_ERROR\n\n# 使用 .f() / .format() 方法追加错误信息\nraise error_codes.CREATE_ERROR.f(\'追加说明\')\n\n# 传递 replace=True 替换错误信息\nraise error_codes.CREATE_ERROR.f(\'替换信息\', replace=True)\n\n# 设置异常对象的 data 属性，以便在后续处理。可通过 exc_obj.data 属性读取\nraise error_codes.CREATE_ERROR.set_data({\'your\': \'data\'})\n```\n\n> 注意：`APIError` 是不可变类型，调用 `format()` 会克隆并返回一个新对象，而非修改现有对象。\n\n当程序抛出 `APIError` 异常后，为了让用户正常看到错误响应，你必须在 Web 框架里捕获并处理该类异常。\n\n##### 5.1.1 在框架内捕获 APIError 异常\n\n视 Web 框架的不同，捕获与处理 `APIError` 的方式会略有区别，以 `DRF` 框架为例。要捕获 `APIError` 异常，我们首先得创建一个新函数：\n\n```python\n# file: my_module.py\nfrom blue_krill.web.std_error import APIError\n\ndef custom_exception_handler(exc, context):\n    if isinstance(exc, APIError):\n        # 你可以随意修改这里的响应数据结构\n        data = {\n            \'code\': exc.code,\n            \'detail\': exc.message,\n        }\n        return Response(data, status=exc.status_code)\n    # ... 其他异常处理撮箕\n```\n\n创建完函数后，下一步是修改项目配置，将 `EXCEPTION_HANDLER` 调整为该异常捕获函数：\n\n```python\nREST_FRAMEWORK = {\n    \'EXCEPTION_HANDLER\': \'my_module.custom_exception_handler\'\n}\n```\n\n配置完成后，每当你在项目里抛出 `error_codes.CREATE_ERROR`，用户便会看到下面的错误信息：\n\n```json\n{\n    "code": \'CREATE_ERROR\',\n    "detail": \'创建失败\'\n}\n```\n\n##### 5.1.2 ErrorCode API 说明\n\n在创建 `ErrorCode` 对象时，除了可以传入必须的 `message` 参数，还支持传入许多可选的个性化参数：\n\n- `message`: 必选，错误详情信息，可包含字符串模板变量\n- `code_num`: 可选，数字错误代码，默认为 -1\n- `extra_formatter`：可选，额外的错误信息格式化函数\n- `status_code`: 该错误推荐使用的 HTTP 错误代码，默认为 400\n\n这些参数各自有着不同的用途，比如，通过定义 `extra_formatter` 属性，你可以调整 `APIError` 拼装错误信息 `message` 的逻辑。\n\n以下面的代码为例：\n\n```python\n# formatter 函数接收两个参数：默认错误信息、当前异常对象\ndef _format_message(message, exc):\n    # 将错误码拼装到错误信息前\n    return f\'code: {exc.code} - {message}\'\n\nclass ErrorCodes:\n    foo = ErrorCode(\'foo message\', extra_formatter=_format_message)\n```\n\n当你抛出 `foo` 错误码时，由于我们使用了自定义的 `message` 格式化函数，错误详情会变成这样：`code: foo - foo message`。\n\n`ErrorCode` 的 `message` 除了能使用普通字符串以外，还支持字符串模板功能。举个例子，假如你定义的 `message` 是 `name={name}`，那么，当你抛出异常时，可以用 `.format()` 方法传入模板变量，对错误信息进行二次渲染。\n\n```python\nraise error_codes.FOO # 1\nraise error_codes.FOO.format(name=\'foobar\') # 2\n```\n\n1. 用户看到的错误信息是 `name={name}`\n2. 用户看到的错误信息会变为 `name=foobar`\n\n#### 5.2 blue_krill.web.drf_utils\n\n`drf_utils` 模块内包含许多与 DRF 框架有关的工具。\n\n##### 5.2.1 stringify_validation_error\n\n`stringify_validation_error()` 会将由 DRF 框架抛出的 `ValidationError` 校验错误异常对象，转换为可读性更好的错误提示文字。\n\n比如，下面的异常对象：\n\n```python\nValidationError({\'foo\': {\'bar\': [ErrorDetail(\'err1\'), ErrorDetail(\'err2\')]}})\n```\n\n可以被转换为：`[\'foo.bar: err1\', \'foo.bar: err2\']` 这样的文字内容。\n\n### 6. blue_krill.async_utils\n\n#### 6.1 blue_krill.aysnc_utils.poll_tasks\n\n`poll_tasks` 是一个用来执行长时间轮询任务的异步工具模块。它的工作原理是每隔几秒钟，拉起一个 `celery` 任务进行轮询逻辑。当轮询应该结束时，带着结果回调。\n\n要创建一个新的轮询任务，你首先要编写一个 `TaskPoller` 类。\n\n```python\nfrom blue_krill.async_utils.poll_task import TaskPoller, PollingResult\n\nclass MyTaskPoller(TaskPoller):\n\n    # 通过定义下面的属性，修改当前 Poller 类的默认配置\n    # max_retries_on_error = 10\n    # overall_timeout_seconds = 3600 * 24 * 7\n    # default_retry_delay_seconds = 10\n\n    def query(self) -> PollingResult:\n        result = request_api()\n        if result:\n            return PollingResult.done(data={\'result\': ...})\n        else:\n            return PollingResult.doing(data={\'current_value\': ...})\n```\n\n`TaskPoller` 的配置属性含义如下：\n\n- `max_retries_on_error`：当轮询抛出异常的总次数，超过该值后，不再继续下次轮询\n- `overall_timeout_seconds`：当轮询的总执行时间（从第一次轮询开始后计算）超过该值，结束本次轮询并返回超时结果\n- `default_retry_delay_seconds`：两次轮询行为之间相隔的秒数\n\n每个 `TaskPoller` 类都必须重写 `query()` 方法，在其中实现**每次**轮询的真正逻辑。在 `query()` 方法内部，你可以从以下属性读取与本次轮询相关的数据：\n\n- `self.params`：轮询任务启动时的参数，通常为字典 `Dict`\n- `self.metadata`：本次轮询任务的元数据，里面包含轮询开始时间、已完成的轮询次数等数据\n\n`query()` 方法需要返回一个 `PollingResult` 结果，来控制接下来的轮询流程。\n\n不同的轮询结果，代表着不同含义：\n\n- `PollingResult.done()`：表示整个轮询任务已结束，不会启动新异步任务\n- `PollingResult.doing()`：表示应该继续轮询，会派生新的异步任务\n\n在实例化 `PollingResult` 时，你可以通过 `data` 属性传入额外数据。该数据对于不同状态的轮询结果来说，有着不同含义。\n\n- 当轮询返回 `done()` 结果时，`data` 会通过回调传递到 `CallbackHandler` 的 `result` 参数里\n- 当轮询仍在继续，返回 `doing()` 结果时，可在 `TaskPoller` 类中，通过 `self.metadata.last_polling_data` 获取**上次轮询**的 `data` 内容\n\n创建完 TaskPoller 类后，下一步是编写 ResultHandler 结果回调类。\n\n##### 6.1.1 定义 CallbackHandler 类\n\n一个标准的 `CallbackHandler` 如下所示：\n\n```python\nfrom blue_krill.async_utils.poll_task import (\n    CallbackHandler,\n    CallbackResult,\n    TaskPoller\n)\n\nclass MyHandler(CallbackHandler):\n\n    def handle(self, result: CallbackResult, poller: TaskPoller):\n        # 通过 result 和 poller 执行回调逻辑\n        pass\n```\n\n根据轮询的不同执行结果，`CallbackResult.status` 会有几种不同的状态：\n\n- `CallbackStatus.NORMAL`：轮询正常结束，`Poller` 返回的轮询结果为 `DONE` / \'.doing()\'\n- `CallbackStatus.TIMEOUT`：轮询超过了规定时间（``overall_timeout_seconds``）仍未结束，判定为超时\n- `CallbackStatus.EXCEPTION`：轮询时发生了异常，且总异常次数超过最大值：`max_retries_on_error`\n\n为了方便操作，你可以直接调用 `result.is_exception` 属性来获知本次轮询是否正常结束。任何状态不为 `NORMAL` 的结果，`.is_exception` 值都为 `True`。\n\n##### 6.1.2 启动轮询任务\n\n当你定义好 `Poller` 与 `CallbackHandler` 类后，可以用以下方式启动一次轮询任务：\n\n```python\n# params = {\'some_field\': \'value\'}\nMyTaskPoller.start(params, MyHandler)\n```\n\n通过执行 `TaskPoller` 类的 `start()` 方法，程序会派生出一个名为 `poll_task.check_status_until_finished` 的 `celery` 异步任务，之后触发 `TaskPoller` 的 `query()` 方法，不断开始轮询。\n\n#### 6.2 blue_krill.aysnc_utils.django_utils\n这个模块提供了 Django + Celery 相关的一些辅助函数。\n\n#### 6.2.1 apply_async_on_commit\n在开启 Django 事务的过程中，可能会立即触发一些 Celery 异步任务，在事务未提交或回滚时，异步任务执行结果是不可预期的。\n这个函数可以封装 Celery 的异步任务调用：\n- 如果不在事务之中，会立刻触发异步任务；\n- 如果处于事务之中，则会在事务提交后触发；\n\n因为执行时机不确定，这个函数会强制忽略异步任务的返回值。\n\n\n#### 6.2.2 delay_on_commit\n函数 `apply_async_on_commit` 的简化版本，相当于 Celery 中 `apply_async` 和 `delay` 的区别。\n\n### 7. blue_krill.monitoring.probe\n\n`blue_krill.monitoring.probe` 模块提供了常见的健康探针功能。\n\n#### 7.1 blue_krill.monitoring.probe.tcp\n\n`blue_krill.monitoring.probe.tcp` 模块提供了通用的 TCP 健康探针, 可检测是否能建立 TCP 连接。\n\n```python\n# Usage:\nfrom blue_krill.monitoring.probe.tcp import TCPProbe, InternetAddress\n\n\nclass SomeTCPProbe(TCPProbe):\n    name: str = "some"\n    address: InternetAddress = InternetAddress(host="localhost", port=8080)\n\n\nreport = SomeTCPProbe().report()\n```\n\n#### 7.2 blue_krill.monitoring.probe.http\n\n`blue_krill.monitoring.probe.http` 模块提供了通用的 HTTP 健康探针, 可检测 HTTP 服务是否正常工作。\n\n```python\n# Usage\nfrom blue_krill.monitoring.probe.http import HttpProbe\n\n\nclass SomeHttpProbe(HttpProbe):\n    name: str = "some"\n    url: str = "http://localhost/ping"\n\n\nreport = SomeHttpProbe().report()\n\n\nclass SomeHttpWithAuth(HttpProbe):\n    name: str = "some"\n    url: str = "http://localhost/ping"\n    params: Dict = {"token": "dummy"}\n    headers: Dict = {"Authorization": "Basic YWxhZGRpbjpvcGVuc2VzYW1l"}\n\n\nreport = SomeHttpWithAuth().report()\n```\n\n#### 7.3 blue_krill.monitoring.probe.mysql\n\n`blue_krill.monitoring.probe.mysql` 模块提供了通用的 MySQL 健康探针, 可检测 MySQL 服务是否正常工作, 该模块依赖 pymysql。\n\n```python\n# Usage:\nfrom blue_krill.monitoring.probe.mysql import MySQLProbe, MySQLConfig\n\n\nclass SomeMySQLProbe(MySQLProbe):\n    name: str = "some"\n    config = MySQLConfig(host="localhost", port=3306, username="root", password="root", database="information_schema")\n\n\nreport = SomeMySQLProbe().report()\n```\n\n#### 7.4 blue_krill.monitoring.probe.redis\n\n`blue_krill.monitoring.probe.redis` 模块提供了通用的 Redis 健康探针和 Redis Sentinel 集群健康探针, 可检测 Redis 服务是否正常工作, 该模块依赖 redis。\n\n```python\n# Usage:\nfrom blue_krill.monitoring.probe.redis import RedisProbe\n\n\nclass SomeRedisProbe(RedisProbe):\n    name: str = "some"\n    redis_url: str = "redis://localhost:6379/0"\n\n\nreport = SomeRedisProbe().report()\n\n\n# Redis Sentinel\nfrom blue_krill.monitoring.probe.redis import RedisSentinelProbe\n\n\nclass SomeRedisSentinelProbe(RedisSentinelProbe):\n    name: str = "some"\n    redis_url: str = "sentinel://:xxx@localhost:6379/0"\n    master_name: str = "mycluster"\n    sentinel_kwargs: dict = {\'password\': \'xxx\'}\n\n\nreport = SomeRedisSentinelProbe().report()\n```\n\n### 8 blue_krill.cubing_case\n`blue_krill.cubing_case` 增加各个方法互相转换的工具库.\n\n#### 8.1 blue_krill.cubing_case.RegexCubingHelper\n基于多种正则将多种模式混合的字符串进行拆分，转换并组合成新的字符串的工具类。\n\n#### 8.2 blue_krill.cubing_case.CommonCaseConvertor\n在 `blue_krill.cubing_case.RegexCubingHelper` 之上的一个封装实现，将指定的多种模式的字符串转化成常见的方法，包含：\n- 驼峰式：`CubingCase`\n- 小写开头的驼峰式：`cubingCase`\n- 小写下划线式：`cubing_case`\n- 大写下划线式：`CUBING_CASE`\n- 小写连字符式：`cubing-case`\n- 大写下划线式：`CUBING-CASE`\n- 小写点分式：`cubing.case`\n- 大写下划线式：`CUBING.CASE`\n- 小写空格分隔式：`cubing case`\n\n#### 8.3 blue_krill.cubing_case.shortcuts\n`blue_krill.cubing_case.shortcuts` 是 `blue_krill.cubing_case.CommonCaseConvertor` 的一个快捷方式，内置了其转换目标的所有源模式，可以实现所有模式的正反转换。\n\n### 9 blue_krill.redis_tools\n`blue_krill.redis_tools` 提供了 redis 常用工具\n\n#### 9.1 blue_krill.redis_tools.sentinel\n`blue_krill.redis_tools.sentinel` 提供了 redis sentinel 模式下，直接从 url 生成 redis 实例的方法。\n\n```python\n# Usage:\nfrom blue_krill.redis_tools.sentinel import SentinelBackend\n\n\nbackend = SentinelBackend(\'sentinel://xxx@localhost:26347/0\', \'mycluster\', {\'password\': \'xxx\'})\nr = backend.client\n\nr.set(\'foo\', \'bar\')\n# 获得 b\'bar\'\nr.get(\'foo\')\n```\n\n## 开发指南\n\n首先安装 [poetry](https://github.com/python-poetry/poetry)，之后在项目目录下执行 `poetry env use python3.6` 初始化开发用虚拟环境。然后用 `poetry shell` 命令激活虚拟环境。\n\n- 执行 `poetry install` 安装所有依赖\n- 使用 `pytest -s .` 执行所有单元测试\n\n在开发时，如果想让某项目安装本地目录里的 blue-krill 模块，首先切换到对应项目虚拟环境，然后在 blue-krill 目录执行 `pip install -e .` \n\n### 使用 tox 执行单元测试\n\n为了测试包在不同 Python 版本下的稳定性，我们使用了 tox 工具。在项目目录下执行 `tox` 即可执行所有的单元测试。\n\n### 发布包\n\n首先，执行 `poetry build` 命令在 dist 目录下生成当前版本的包(需要检查 dist 目录中的内容是否符合预期，避免上传其他版本覆盖)。然后执行 `twine upload dist/* --repository-url {pypi_address} --username {your_name} --password {your_token}` 将其上传到 pypi 服务器上。\n\n### 以“可编辑模式”安装\n\n进入项目根目录，执行 `pip install -e .` 以“可编辑模式”安装包。该操作要求 pip 为版本 21.3 及以上[（参考）](https://pip.pypa.io/en/stable/news/#v21-3)。\n',
+    'long_description': '# Blue krill\n\nPython 常用工具包模块。\n\n## 使用指南\n\n### 1. blue_krill.secure\n\n加解密、安全相关的工具与模块。\n\n#### 1.1 dj_environ 模块\n\ndj_environ 的主要目的是在 [django-environ](https://github.com/joke2k/django-environ) 之上，增加可以阅读加密环境变量的能力。如需使用，首先需要设置密文环境变量：\n\n```bash\nexport DATABASE_URL=\'<使用 bk-secure 加密后的字符串>\'\nexport FOO=\'<使用 bk-secure 加密后的字符串>\'\n```\n\n然后在 `settings` 模块中，初始化 `SecureEnv` 对象并使用它读取对应配置：\n\n```python\nfrom blue_krill.secure.dj_environ import SecureEnv\n\n# 初始化并加载 .env 文件内容\nsec_env = SecureEnv()\nenviron.Env.read_env()\n\n# 读取为数据库配置\nDATABASES[\'default\'] = sec_env.db()\n\n# 读取为普通配置\nFOO = sec_env(\'FOO\')\n```\n\n#### 1.2 bk-secure 脚本\n\nbk-secure 主要用于配合 dj_environ 模块生成加密环境变量（或配置文件）。使用前，先将 `BK_FERNET_KEY` 设为你所使用的加密 key。一般情况下，这个值等同于 Django 项目的 `BKKRILL_ENCRYPT_SECRET_KEY` 配置项：\n\n```\nexport BK_FERNET_KEY=\'... ...\'\n```\n\n执行 `encrypt` 加密某段明文：\n\n```console\n❯ bk-secure encrypt\nInput string: mysql://u:p@localhost/foo\nThe encrypted token is: gAAAAABfKUtKIBzYc_gyQL-j9TmI35O1d0auLQfYeso6D8Q77ZC9PIuv26ABPFlOQSSPDzT3HcVrhI1K3XwU5Xfs6gP6iAe8RhEAJJhMktp7CKzn7p7imNk=\n```\n\n执行 `decrypt` 解密某段密文：\n\n```console\n❯ bk-secure decrypt\nInput token: gAAAAABfKUtKIBzYc_gyQL-j9TmI35O1d0auLQfYeso6D8Q77ZC9PIuv26ABPFlOQSSPDzT3HcVrhI1K3XwU5Xfs6gP6iAe8RhEAJJhMktp7CKzn7p7imNk=\nThe decrypted result is: mysql://u:p@localhost/foo\n```\n\n使用 `edit` 以明文方式编辑某段密文，并输出新的密文：\n\n```console\n❯ bk-secure edit\nInput token: gAAAAABfKUtKIBzYc_gyQL-j9TmI35O1d0auLQfYeso6D8Q77ZC9PIuv26ABPFlOQSSPDzT3HcVrhI1K3XwU5Xfs6gP6iAe8RhEAJJhMktp7CKzn7p7imNk=\n# 将弹出编辑器界面修改明文，可通过 $EDITOR 环境变量设置编辑器\nThe new value is: mysql://u:p@localhost/foo2\nThe encrypted new value is: gAAAAABfKUui5_YUVxoYEYQG61RSRX1Ll3s1dgkZ5nUEJbCxakWHSyo3AKZFv3GuoQ7cH2Hm5LEU2QDK8C3G-_iog0TmqSbVkIYf0WnksH2DGgedldfbwhs=\n```\n\n### 2. blue_krill.editions\n\n多版本开发相关工具模块\n\n#### 2.1 editionctl 工具\n\n`editonctl` 是用来帮助开发需要支持多版本 Python 项目的工具，使用该工具前，请先把你的项目目录组织成下面这种结构：\n\n```raw\n├── editionctl.toml\n├── editions\n│\xa0\xa0 ├── ee\n│\xa0\xa0 │\xa0\xa0 └── ee.py\n│\xa0\xa0 └── te\n│\xa0\xa0     └── te.py\n└── main\n    └── main.py\n```\n\n其中：\n\n- `editions`：仅保存不同版本所特有的源码文件\n- `main`：项目主目录\n\n#### 2.1.1 创建配置文件\n\n要使用 `editonctl`，首先需要在项目内创建配置文件 `editionctl.toml`。比如，针对上面的项目结构，我们可以创建这样的配置文件：\n\n```toml\n# 项目主目录\nproject_root = \'main\'\n# 项目各版本所在目录\neditions_root = \'editions\'\n\n[[editions]]\n# 版本名称\nname = "TE"\n# 版本相对路径\nrel_directory = \'te\'\n\n[[editions]]\nname = "EE"\nrel_directory = \'ee\'\n```\n\n> 更多配置文件相关说明，可执行 `editionctl help` 查看。\n\n#### 2.1.2 在版本之间切换\n\n在不同版本间切换，需要使用 `editionctl activate {EDITION_NAME}` 命令。执行该命令后，工具会将指定版本下的所有源码文件，拷贝到 `project_root` 中。\n\n```bash\n$ editionctl activate EE\n[2020-12-17 16:51:37,312] INFO: Edition EE activated, linker is default\n```\n\n> 为了避免由工具拷贝的文件被意外提交到源码仓库，这些文件会被添加到 `{project_root}/.gitignore` 中。\n\n#### 2.1.3 重置多版本\n\n假如你想要清除所有由 `editionctl` 工具创建的源码文件，可以执行 `editionctl reset` 命令。执行该命令将删除所有多版本相关文件，只保留主目录。\n\n#### 2.1.4 进入开发模式\n\n在开发多版本项目时，`editions_root` 目录下的当前版本相关文件会被频繁修改。正常情况下，每次修改版本文件后，我们都要手动重新执行 `activate` 命令重新同步文件。\n\n为了简化这个过程，我们可以使用 `editionctl develop`。\n\n执行 `editionctl develop` 命令后，工具将会持续监听当前 `edition` 目录下的任何改动。如果监听到新改动，则自动触发同步机制。\n\n```\n$ editionctl develop\n[2020-12-17 16:56:34,385] INFO: Start watching editions/ee directory for edition EE...\n```\n\n### 3. blue_krill.data_types.enum\n\n枚举相关的数据类型。\n\n### 3.1 FeatureFlag\n\n功能标记(Feature Flag)用于控制当前用户能否感知到某个功能/特性，只提供**开启(enabled)**和**关闭(disabled)**两个状态, 分别对应于布尔值的 True/Flase。\n为了避免各项目重复造轮子, blue_krill 抽象出通用的 FeatureFlag 模型, 同时也提供类似于`枚举(Enum)`的API, 降低使用成本。\n\n#### 3.1.1 如何定义 FeatureFlag\n\n就像定义普通的 Python Class 一样, 定义 FeatureFlag 只需要继承 `blue_krill.data_types.enum::FeatureFlag` 即可。\n```python\nfrom blue_krill.data_types.enum import FeatureFlag, FeatureFlagField\n\n\nclass UserFeatureFlag(FeatureFlag):\n    # 使用类属性声明 FeatureFlagField 时, name 属性会通过描述符协议自动设置, 无需额外指定.\n    WEBCONSOLE = FeatureFlagField(label="使用 WEBConsole")\n    CREATE_SMART_APP = FeatureFlagField(label="创建 Smart 应用")\n    ...\n```\n\n#### 3.1.2 如何添加额外的 FeatureFlag\n\n不同于`枚举值(Enum)`, FeatureFlag 允许在运行过程中动态添加额外的字段或修改已有字段的默认值。\n\n```python\n# 添加额外的 FeatureFlag 时, 需要制定对应的名称.\nUserFeatureFlag.register_feature_flag(FeatureFlagField(name="CHOOSE_SOURCE_ORIGIN", label="选择源码来源"))\n```\n\n### 3.2 StructuredEnum\n\n考虑到我们使用`枚举值(Enum)`时, 往往会给枚举值添加额外的描述字段，为了避免各项目重复造轮子，blue_krill 基于 `Enum` 实现了 StructuredEnum，可以基于配套的 `EnumField` 定义带有额外描述内容的枚举值。\n\n```python\nfrom blue_krill.data_types.enum import EnumField, StructuredEnum\n\n\nclass DiffType(str, StructuredEnum):\n    ADDED = EnumField("added", label="新增")\n    DELETED = EnumField("deleted", label="删除")\n    NOT_MODIFIED = EnumField("not_modified", label="未改动")\n```\n\n### 4. blue_krill.storages.blobstore\n\n对象存储服务的简单封装, 目前支持 **上传**, **下载**, **生成预签名URL** 三个接口.\n\n#### 4.1 S3Store\n\nS3 协议的 BlobStore 实现, 使用时需要额外安装 boto3==\'^1.4.3\', 可参考以下代码进行实例化:\n```python\nfrom blue_krill.storages.blobstore.s3 import S3Store\n\n\nstore = S3Store(\n    bucket="your-bucket",\n    aws_access_key_id=\'your-access-key\',\n    aws_secret_access_key=\'your-secret-key\',\n    endpoint_url=\'your-s3-endpoint\',\n    # Optional\n    region_name=\'your-region, default is `us-east-1`\',\n    signature_version=\'your-signature-version, default is s3v4\',\n)\n```\n\n#### 4.2 BKGenericRepo\n\n底层服务是 **蓝鲸通用二进制仓库** 的底层实现, 可参考以下代码进行实例化:\n\n```python\nfrom blue_krill.storages.blobstore.bkrepo import BKGenericRepo\n\n\nstore = BKGenericRepo(\n    bucket=\'your-bucket\',\n    project=\'your-project-id\',\n    endpoint_url=\'\',\n)\n```\n\n### 5. blue_krill.web\n\n`blue_krill.web` 主要存放与 Web 开发有关的工具集。\n\n#### 5.1 blue_krill.web.std_error\n\n该模块内包含标准的错误码功能。`std_error` 最常见的用法，是通过 `ErrorCode` 定义一套错误码集合：\n\n```python\nfrom blue_krill.web.std_error import ErrorCode\n\nclass ErrorCodes:\n    CREATE_ERROR = ErrorCode(\'创建失败\')\n    DELETE_ERROR = ErrorCode(\'删除失败\')\n\n# 实例化一个全局对象\nerror_codes = ErrorCodes()\n```\n\n当你要抛出某个特定错误时，可以使用下面的语句：\n\n```python\nraise error_codes.CREATE_ERROR\n\n# 使用 .f() / .format() 方法追加错误信息\nraise error_codes.CREATE_ERROR.f(\'追加说明\')\n\n# 传递 replace=True 替换错误信息\nraise error_codes.CREATE_ERROR.f(\'替换信息\', replace=True)\n\n# 设置异常对象的 data 属性，以便在后续处理。可通过 exc_obj.data 属性读取\nraise error_codes.CREATE_ERROR.set_data({\'your\': \'data\'})\n```\n\n> 注意：`APIError` 是不可变类型，调用 `format()` 会克隆并返回一个新对象，而非修改现有对象。\n\n当程序抛出 `APIError` 异常后，为了让用户正常看到错误响应，你必须在 Web 框架里捕获并处理该类异常。\n\n##### 5.1.1 在框架内捕获 APIError 异常\n\n视 Web 框架的不同，捕获与处理 `APIError` 的方式会略有区别，以 `DRF` 框架为例。要捕获 `APIError` 异常，我们首先得创建一个新函数：\n\n```python\n# file: my_module.py\nfrom blue_krill.web.std_error import APIError\n\ndef custom_exception_handler(exc, context):\n    if isinstance(exc, APIError):\n        # 你可以随意修改这里的响应数据结构\n        data = {\n            \'code\': exc.code,\n            \'detail\': exc.message,\n        }\n        return Response(data, status=exc.status_code)\n    # ... 其他异常处理撮箕\n```\n\n创建完函数后，下一步是修改项目配置，将 `EXCEPTION_HANDLER` 调整为该异常捕获函数：\n\n```python\nREST_FRAMEWORK = {\n    \'EXCEPTION_HANDLER\': \'my_module.custom_exception_handler\'\n}\n```\n\n配置完成后，每当你在项目里抛出 `error_codes.CREATE_ERROR`，用户便会看到下面的错误信息：\n\n```json\n{\n    "code": \'CREATE_ERROR\',\n    "detail": \'创建失败\'\n}\n```\n\n##### 5.1.2 ErrorCode API 说明\n\n在创建 `ErrorCode` 对象时，除了可以传入必须的 `message` 参数，还支持传入许多可选的个性化参数：\n\n- `message`: 必选，错误详情信息，可包含字符串模板变量\n- `code_num`: 可选，数字错误代码，默认为 -1\n- `extra_formatter`：可选，额外的错误信息格式化函数\n- `status_code`: 该错误推荐使用的 HTTP 错误代码，默认为 400\n\n这些参数各自有着不同的用途，比如，通过定义 `extra_formatter` 属性，你可以调整 `APIError` 拼装错误信息 `message` 的逻辑。\n\n以下面的代码为例：\n\n```python\n# formatter 函数接收两个参数：默认错误信息、当前异常对象\ndef _format_message(message, exc):\n    # 将错误码拼装到错误信息前\n    return f\'code: {exc.code} - {message}\'\n\nclass ErrorCodes:\n    foo = ErrorCode(\'foo message\', extra_formatter=_format_message)\n```\n\n当你抛出 `foo` 错误码时，由于我们使用了自定义的 `message` 格式化函数，错误详情会变成这样：`code: foo - foo message`。\n\n`ErrorCode` 的 `message` 除了能使用普通字符串以外，还支持字符串模板功能。举个例子，假如你定义的 `message` 是 `name={name}`，那么，当你抛出异常时，可以用 `.format()` 方法传入模板变量，对错误信息进行二次渲染。\n\n```python\nraise error_codes.FOO # 1\nraise error_codes.FOO.format(name=\'foobar\') # 2\n```\n\n1. 用户看到的错误信息是 `name={name}`\n2. 用户看到的错误信息会变为 `name=foobar`\n\n#### 5.2 blue_krill.web.drf_utils\n\n`drf_utils` 模块内包含许多与 DRF 框架有关的工具。\n\n##### 5.2.1 stringify_validation_error\n\n`stringify_validation_error()` 会将由 DRF 框架抛出的 `ValidationError` 校验错误异常对象，转换为可读性更好的错误提示文字。\n\n比如，下面的异常对象：\n\n```python\nValidationError({\'foo\': {\'bar\': [ErrorDetail(\'err1\'), ErrorDetail(\'err2\')]}})\n```\n\n可以被转换为：`[\'foo.bar: err1\', \'foo.bar: err2\']` 这样的文字内容。\n\n### 6. blue_krill.async_utils\n\n#### 6.1 blue_krill.aysnc_utils.poll_tasks\n\n`poll_tasks` 是一个用来执行长时间轮询任务的异步工具模块。它的工作原理是每隔几秒钟，拉起一个 `celery` 任务进行轮询逻辑。当轮询应该结束时，带着结果回调。\n\n要创建一个新的轮询任务，你首先要编写一个 `TaskPoller` 类。\n\n```python\nfrom blue_krill.async_utils.poll_task import TaskPoller, PollingResult\n\nclass MyTaskPoller(TaskPoller):\n\n    # 通过定义下面的属性，修改当前 Poller 类的默认配置\n    # max_retries_on_error = 10\n    # overall_timeout_seconds = 3600 * 24 * 7\n    # default_retry_delay_seconds = 10\n\n    def query(self) -> PollingResult:\n        result = request_api()\n        if result:\n            return PollingResult.done(data={\'result\': ...})\n        else:\n            return PollingResult.doing(data={\'current_value\': ...})\n```\n\n`TaskPoller` 的配置属性含义如下：\n\n- `max_retries_on_error`：当轮询抛出异常的总次数，超过该值后，不再继续下次轮询\n- `overall_timeout_seconds`：当轮询的总执行时间（从第一次轮询开始后计算）超过该值，结束本次轮询并返回超时结果\n- `default_retry_delay_seconds`：两次轮询行为之间相隔的秒数\n\n每个 `TaskPoller` 类都必须重写 `query()` 方法，在其中实现**每次**轮询的真正逻辑。在 `query()` 方法内部，你可以从以下属性读取与本次轮询相关的数据：\n\n- `self.params`：轮询任务启动时的参数，通常为字典 `Dict`\n- `self.metadata`：本次轮询任务的元数据，里面包含轮询开始时间、已完成的轮询次数等数据\n\n`query()` 方法需要返回一个 `PollingResult` 结果，来控制接下来的轮询流程。\n\n不同的轮询结果，代表着不同含义：\n\n- `PollingResult.done()`：表示整个轮询任务已结束，不会启动新异步任务\n- `PollingResult.doing()`：表示应该继续轮询，会派生新的异步任务\n\n在实例化 `PollingResult` 时，你可以通过 `data` 属性传入额外数据。该数据对于不同状态的轮询结果来说，有着不同含义。\n\n- 当轮询返回 `done()` 结果时，`data` 会通过回调传递到 `CallbackHandler` 的 `result` 参数里\n- 当轮询仍在继续，返回 `doing()` 结果时，可在 `TaskPoller` 类中，通过 `self.metadata.last_polling_data` 获取**上次轮询**的 `data` 内容\n\n创建完 TaskPoller 类后，下一步是编写 ResultHandler 结果回调类。\n\n##### 6.1.1 定义 CallbackHandler 类\n\n一个标准的 `CallbackHandler` 如下所示：\n\n```python\nfrom blue_krill.async_utils.poll_task import (\n    CallbackHandler,\n    CallbackResult,\n    TaskPoller\n)\n\nclass MyHandler(CallbackHandler):\n\n    def handle(self, result: CallbackResult, poller: TaskPoller):\n        # 通过 result 和 poller 执行回调逻辑\n        pass\n```\n\n根据轮询的不同执行结果，`CallbackResult.status` 会有几种不同的状态：\n\n- `CallbackStatus.NORMAL`：轮询正常结束，`Poller` 返回的轮询结果为 `DONE` / \'.doing()\'\n- `CallbackStatus.TIMEOUT`：轮询超过了规定时间（``overall_timeout_seconds``）仍未结束，判定为超时\n- `CallbackStatus.EXCEPTION`：轮询时发生了异常，且总异常次数超过最大值：`max_retries_on_error`\n\n为了方便操作，你可以直接调用 `result.is_exception` 属性来获知本次轮询是否正常结束。任何状态不为 `NORMAL` 的结果，`.is_exception` 值都为 `True`。\n\n##### 6.1.2 启动轮询任务\n\n当你定义好 `Poller` 与 `CallbackHandler` 类后，可以用以下方式启动一次轮询任务：\n\n```python\n# params = {\'some_field\': \'value\'}\nMyTaskPoller.start(params, MyHandler)\n```\n\n通过执行 `TaskPoller` 类的 `start()` 方法，程序会派生出一个名为 `poll_task.check_status_until_finished` 的 `celery` 异步任务，之后触发 `TaskPoller` 的 `query()` 方法，不断开始轮询。\n\n#### 6.2 blue_krill.aysnc_utils.django_utils\n这个模块提供了 Django + Celery 相关的一些辅助函数。\n\n#### 6.2.1 apply_async_on_commit\n在开启 Django 事务的过程中，可能会立即触发一些 Celery 异步任务，在事务未提交或回滚时，异步任务执行结果是不可预期的。\n这个函数可以封装 Celery 的异步任务调用：\n- 如果不在事务之中，会立刻触发异步任务；\n- 如果处于事务之中，则会在事务提交后触发；\n\n因为执行时机不确定，这个函数会强制忽略异步任务的返回值。\n\n\n#### 6.2.2 delay_on_commit\n函数 `apply_async_on_commit` 的简化版本，相当于 Celery 中 `apply_async` 和 `delay` 的区别。\n\n### 7. blue_krill.monitoring.probe\n\n`blue_krill.monitoring.probe` 模块提供了常见的健康探针功能。\n\n#### 7.1 blue_krill.monitoring.probe.tcp\n\n`blue_krill.monitoring.probe.tcp` 模块提供了通用的 TCP 健康探针, 可检测是否能建立 TCP 连接。\n\n```python\n# Usage:\nfrom blue_krill.monitoring.probe.tcp import TCPProbe, InternetAddress\n\n\nclass SomeTCPProbe(TCPProbe):\n    name: str = "some"\n    address: InternetAddress = InternetAddress(host="localhost", port=8080)\n\n\nreport = SomeTCPProbe().report()\n```\n\n#### 7.2 blue_krill.monitoring.probe.http\n\n`blue_krill.monitoring.probe.http` 模块提供了通用的 HTTP 健康探针, 可检测 HTTP 服务是否正常工作。\n\n```python\n# Usage\nfrom blue_krill.monitoring.probe.http import HttpProbe\n\n\nclass SomeHttpProbe(HttpProbe):\n    name: str = "some"\n    url: str = "http://localhost/ping"\n\n\nreport = SomeHttpProbe().report()\n\n\nclass SomeHttpWithAuth(HttpProbe):\n    name: str = "some"\n    url: str = "http://localhost/ping"\n    params: Dict = {"token": "dummy"}\n    headers: Dict = {"Authorization": "Basic YWxhZGRpbjpvcGVuc2VzYW1l"}\n\n\nreport = SomeHttpWithAuth().report()\n```\n\n#### 7.3 blue_krill.monitoring.probe.mysql\n\n`blue_krill.monitoring.probe.mysql` 模块提供了通用的 MySQL 健康探针, 可检测 MySQL 服务是否正常工作, 该模块依赖 pymysql。\n\n```python\n# Usage:\nfrom blue_krill.monitoring.probe.mysql import MySQLProbe, MySQLConfig\n\n\nclass SomeMySQLProbe(MySQLProbe):\n    name: str = "some"\n    config = MySQLConfig(host="localhost", port=3306, username="root", password="root", database="information_schema")\n\n\nreport = SomeMySQLProbe().report()\n```\n\n#### 7.4 blue_krill.monitoring.probe.redis\n\n`blue_krill.monitoring.probe.redis` 模块提供了通用的 Redis 健康探针和 Redis Sentinel 集群健康探针, 可检测 Redis 服务是否正常工作, 该模块依赖 redis。\n\n```python\n# Usage:\nfrom blue_krill.monitoring.probe.redis import RedisProbe\n\n\nclass SomeRedisProbe(RedisProbe):\n    name: str = "some"\n    redis_url: str = "redis://localhost:6379/0"\n\n\nreport = SomeRedisProbe().report()\n\n\n# Redis Sentinel\nfrom blue_krill.monitoring.probe.redis import RedisSentinelProbe\n\n\nclass SomeRedisSentinelProbe(RedisSentinelProbe):\n    name: str = "some"\n    redis_url: str = "sentinel://:xxx@localhost:6379/0"\n    master_name: str = "mycluster"\n    sentinel_kwargs: dict = {\'password\': \'xxx\'}\n\n\nreport = SomeRedisSentinelProbe().report()\n```\n\n### 8 blue_krill.cubing_case\n`blue_krill.cubing_case` 增加各个方法互相转换的工具库.\n\n#### 8.1 blue_krill.cubing_case.RegexCubingHelper\n基于多种正则将多种模式混合的字符串进行拆分，转换并组合成新的字符串的工具类。\n\n#### 8.2 blue_krill.cubing_case.CommonCaseConvertor\n在 `blue_krill.cubing_case.RegexCubingHelper` 之上的一个封装实现，将指定的多种模式的字符串转化成常见的方法，包含：\n- 驼峰式：`CubingCase`\n- 小写开头的驼峰式：`cubingCase`\n- 小写下划线式：`cubing_case`\n- 大写下划线式：`CUBING_CASE`\n- 小写连字符式：`cubing-case`\n- 大写下划线式：`CUBING-CASE`\n- 小写点分式：`cubing.case`\n- 大写下划线式：`CUBING.CASE`\n- 小写空格分隔式：`cubing case`\n\n#### 8.3 blue_krill.cubing_case.shortcuts\n`blue_krill.cubing_case.shortcuts` 是 `blue_krill.cubing_case.CommonCaseConvertor` 的一个快捷方式，内置了其转换目标的所有源模式，可以实现所有模式的正反转换。\n\n### 9 blue_krill.redis_tools\n`blue_krill.redis_tools` 提供了 redis 常用工具\n\n#### 9.1 blue_krill.redis_tools.sentinel\n`blue_krill.redis_tools.sentinel` 提供了 redis sentinel 模式下，直接从 url 生成 redis 实例的方法。\n\n```python\n# Usage:\nfrom blue_krill.redis_tools.sentinel import SentinelBackend\n\n\nbackend = SentinelBackend(\'sentinel://xxx@localhost:26347/0\', \'mycluster\', {\'password\': \'xxx\'})\nr = backend.client\n\nr.set(\'foo\', \'bar\')\n# 获得 b\'bar\'\nr.get(\'foo\')\n```\n\n### 10 blue_krill.encrypt.handler\n`blue_krill.encrypt.handler` 提够 Fernet 和 SM4 两种对称加密算法，并且为了适应存量数据，在解密时会根据`header`选择相应的算法进行解密。\n具体的使用方式如下:\n\n```python\nfrom blue_krill.encrypt.handler import EncryptHandler\n\n# 实例化\n# 第一种方式通过传入 encrypt_cipher_type(加密算法类型) 和 secret_key(密钥)\n# encrypt_cipher_type 现有的就是 "FernetCipher" 和 "SM4CTR"，分别对应 Fernet 和 SM4 对称加密算法\nencrypt_handler = EncryptHandler(encrypt_cipher_type=\'FernetCipher\', secret_key=b\'PIMCuSRiVqBg5eSzQqZZrOhGFSUtrlS-8_JlIpjHt0A=\')\n# 第二种方式，不传入参数时，即 encrypt_cipher_type 和 secret_key 为 None \n# 会分别通过 django setting 中的 ENCRYPT_CIPHER_TYPE 和 BKKRILL_ENCRYPT_SECRET_KEY 字段设置。\nencrypt_handler = EncryptHandler()\n\n# 加解密使用\ntext = "random_text"\n# 加密，根据选择的算法不同，header 也会不同，算法为 Fernet 加密头为 bkcrypt$，算法为 SM4 时，加密头为 sm4ctr$\n# encrypted = "bkcrypt$gAAAAABkyIHPPbOeAOLa3LMc8901rslfBeTdm3rWZntSz5ut7eIDyb9eDgPmzVtL3y-iUBPSxRtZLC2ynlmeKeCNmRmTHpjtWg=="\n# encrypted = "sm4ctr$KI9M5PrhDCmj5ix90OKg/5qYLcR8F3owLlsG"\nencrypted = encrypt_handler.encrypt(text)\n# 解密\n# decrypted = "random_text"\ndecrypted = encrypt_handler.decrypt(encrypted)\n```\n\n### 11 blue_krill.models.fields\n`blue_krill.models.fields` 基于 `EncryptHandler` 实现了 `EncryptField`，具体使用：\n```python\nfrom django.db import models\nfrom blue_krill.models.fields import EncryptField\n\n\nclass User(models.Model):\n    """\n    User.password 在存取时会做加解密\n    """\n    \n    name = models.CharField(max_length=30)\n    # EncryptField 用法与 EncryptHandler 类似\n    # 实例化时，可传入 encrypt_cipher_type 选择加密算法，secret_key 配置密钥\n    # 不传入时，会分别通过 django setting 中的 ENCRYPT_CIPHER_TYPE 和 BKKRILL_ENCRYPT_SECRET_KEY 字段设置。\n    password = EncryptField()\n\n    def __str__(self):\n        return self.name\n```\n\n## 开发指南\n\n首先安装 [poetry](https://github.com/python-poetry/poetry)，之后在项目目录下执行 `poetry env use python3.6` 初始化开发用虚拟环境。然后用 `poetry shell` 命令激活虚拟环境。\n\n- 执行 `poetry install` 安装所有依赖\n- 使用 `pytest -s .` 执行所有单元测试\n\n在开发时，如果想让某项目安装本地目录里的 blue-krill 模块，首先切换到对应项目虚拟环境，然后在 blue-krill 目录执行 `pip install -e .` \n\n### 使用 tox 执行单元测试\n\n为了测试包在不同 Python 版本下的稳定性，我们使用了 tox 工具。在项目目录下执行 `tox` 即可执行所有的单元测试。\n\n### 发布包\n\n首先，执行 `poetry build` 命令在 dist 目录下生成当前版本的包(需要检查 dist 目录中的内容是否符合预期，避免上传其他版本覆盖)。然后执行 `twine upload dist/* --repository-url {pypi_address} --username {your_name} --password {your_token}` 将其上传到 pypi 服务器上。\n\n### 以“可编辑模式”安装\n\n进入项目根目录，执行 `pip install -e .` 以“可编辑模式”安装包。该操作要求 pip 为版本 21.3 及以上[（参考）](https://pip.pypa.io/en/stable/news/#v21-3)。\n',
     'author': 'blueking',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.6.2,<3.11',
 }
```

### Comparing `blue-krill-1.2.3/PKG-INFO` & `blue_krill-1.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: blue-krill
-Version: 1.2.3
+Version: 1.2.4
 Summary: Tools and common packages for blueking paas
 License: Apache-2.0
 Author: blueking
 Requires-Python: >=3.6.2,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: bk-crypto-python-sdk (>=1.0.4,<2.0.0)
 Requires-Dist: click
 Requires-Dist: cryptography (>=3.0.0,<4.0.0)
 Requires-Dist: curlify (>=2.2.1,<3.0.0)
-Requires-Dist: dataclasses (>=0.7,<0.8); python_full_version >= "3.6.2" and python_version < "3.7"
+Requires-Dist: dataclasses (>=0.7,<0.8) ; python_full_version >= "3.6.2" and python_version < "3.7"
 Requires-Dist: django-environ (>=0.8.1,<0.9.0)
 Requires-Dist: pydantic (>=1.7,<2.0)
 Requires-Dist: pyjwt (>=1.7.1)
 Requires-Dist: python-editor (>=1.0.4,<2.0.0)
 Requires-Dist: requests
 Requires-Dist: six
 Requires-Dist: toml
@@ -612,14 +613,62 @@
 r = backend.client
 
 r.set('foo', 'bar')
 # 获得 b'bar'
 r.get('foo')
 ```
 
+### 10 blue_krill.encrypt.handler
+`blue_krill.encrypt.handler` 提够 Fernet 和 SM4 两种对称加密算法，并且为了适应存量数据，在解密时会根据`header`选择相应的算法进行解密。
+具体的使用方式如下:
+
+```python
+from blue_krill.encrypt.handler import EncryptHandler
+
+# 实例化
+# 第一种方式通过传入 encrypt_cipher_type(加密算法类型) 和 secret_key(密钥)
+# encrypt_cipher_type 现有的就是 "FernetCipher" 和 "SM4CTR"，分别对应 Fernet 和 SM4 对称加密算法
+encrypt_handler = EncryptHandler(encrypt_cipher_type='FernetCipher', secret_key=b'PIMCuSRiVqBg5eSzQqZZrOhGFSUtrlS-8_JlIpjHt0A=')
+# 第二种方式，不传入参数时，即 encrypt_cipher_type 和 secret_key 为 None 
+# 会分别通过 django setting 中的 ENCRYPT_CIPHER_TYPE 和 BKKRILL_ENCRYPT_SECRET_KEY 字段设置。
+encrypt_handler = EncryptHandler()
+
+# 加解密使用
+text = "random_text"
+# 加密，根据选择的算法不同，header 也会不同，算法为 Fernet 加密头为 bkcrypt$，算法为 SM4 时，加密头为 sm4ctr$
+# encrypted = "bkcrypt$gAAAAABkyIHPPbOeAOLa3LMc8901rslfBeTdm3rWZntSz5ut7eIDyb9eDgPmzVtL3y-iUBPSxRtZLC2ynlmeKeCNmRmTHpjtWg=="
+# encrypted = "sm4ctr$KI9M5PrhDCmj5ix90OKg/5qYLcR8F3owLlsG"
+encrypted = encrypt_handler.encrypt(text)
+# 解密
+# decrypted = "random_text"
+decrypted = encrypt_handler.decrypt(encrypted)
+```
+
+### 11 blue_krill.models.fields
+`blue_krill.models.fields` 基于 `EncryptHandler` 实现了 `EncryptField`，具体使用：
+```python
+from django.db import models
+from blue_krill.models.fields import EncryptField
+
+
+class User(models.Model):
+    """
+    User.password 在存取时会做加解密
+    """
+    
+    name = models.CharField(max_length=30)
+    # EncryptField 用法与 EncryptHandler 类似
+    # 实例化时，可传入 encrypt_cipher_type 选择加密算法，secret_key 配置密钥
+    # 不传入时，会分别通过 django setting 中的 ENCRYPT_CIPHER_TYPE 和 BKKRILL_ENCRYPT_SECRET_KEY 字段设置。
+    password = EncryptField()
+
+    def __str__(self):
+        return self.name
+```
+
 ## 开发指南
 
 首先安装 [poetry](https://github.com/python-poetry/poetry)，之后在项目目录下执行 `poetry env use python3.6` 初始化开发用虚拟环境。然后用 `poetry shell` 命令激活虚拟环境。
 
 - 执行 `poetry install` 安装所有依赖
 - 使用 `pytest -s .` 执行所有单元测试
```

