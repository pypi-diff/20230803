# Comparing `tmp/yaylib-1.0.6.tar.gz` & `tmp/yaylib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-1.0.6.tar", last modified: Sat Jul 29 08:11:48 2023, max compression
+gzip compressed data, was "yaylib-1.0.7.tar", last modified: Wed Aug  2 23:10:28 2023, max compression
```

## Comparing `yaylib-1.0.6.tar` & `yaylib-1.0.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 08:11:48.989841 yaylib-1.0.6/
--rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.6/LICENSE
--rw-rw-rw-   0        0        0    12824 2023-07-29 08:11:48.988645 yaylib-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    11961 2023-07-29 04:57:25.000000 yaylib-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 08:11:48.989841 yaylib-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-07-24 11:24:25.000000 yaylib-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:11:48.943778 yaylib-1.0.6/tests/
--rw-rw-rw-   0        0        0        0 2023-07-28 03:22:00.000000 yaylib-1.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-07-28 03:15:02.000000 yaylib-1.0.6/tests/config.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_call.py
--rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_cassandra.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_chat.py
--rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_group.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_misc.py
--rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_post.py
--rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_review.py
--rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_thread.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_user.py
--rw-rw-rw-   0        0        0     1908 2023-07-28 03:21:48.000000 yaylib-1.0.6/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:11:48.951038 yaylib-1.0.6/yaylib/
--rw-rw-rw-   0        0        0      668 2023-07-25 06:44:17.000000 yaylib-1.0.6/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:11:48.988645 yaylib-1.0.6/yaylib/api/
--rw-rw-rw-   0        0        0      715 2023-07-25 06:44:11.000000 yaylib-1.0.6/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0    10523 2023-07-28 01:49:59.000000 yaylib-1.0.6/yaylib/api/api.py
--rw-rw-rw-   0        0        0     9429 2023-07-23 06:18:02.000000 yaylib-1.0.6/yaylib/api/call.py
--rw-rw-rw-   0        0        0     2713 2023-07-28 02:06:00.000000 yaylib-1.0.6/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    14964 2023-07-29 04:53:58.000000 yaylib-1.0.6/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    23695 2023-07-18 08:52:45.000000 yaylib-1.0.6/yaylib/api/group.py
--rw-rw-rw-   0        0        0     8347 2023-07-28 02:06:16.000000 yaylib-1.0.6/yaylib/api/login.py
--rw-rw-rw-   0        0        0     7417 2023-07-18 08:52:45.000000 yaylib-1.0.6/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    33686 2023-07-22 09:13:37.000000 yaylib-1.0.6/yaylib/api/post.py
--rw-rw-rw-   0        0        0     4488 2023-07-18 08:52:45.000000 yaylib-1.0.6/yaylib/api/review.py
--rw-rw-rw-   0        0        0     5945 2023-07-18 08:52:45.000000 yaylib-1.0.6/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    23744 2023-07-19 12:23:37.000000 yaylib-1.0.6/yaylib/api/user.py
--rw-rw-rw-   0        0        0     9409 2023-07-28 13:12:41.000000 yaylib-1.0.6/yaylib/api/websocket.py
--rw-rw-rw-   0        0        0    86741 2023-07-29 04:54:07.000000 yaylib-1.0.6/yaylib/client.py
--rw-rw-rw-   0        0        0    18801 2023-07-29 08:11:00.000000 yaylib-1.0.6/yaylib/config.py
--rw-rw-rw-   0        0        0     2131 2023-07-18 08:52:45.000000 yaylib-1.0.6/yaylib/errors.py
--rw-rw-rw-   0        0        0    56113 2023-07-21 11:49:21.000000 yaylib-1.0.6/yaylib/models.py
--rw-rw-rw-   0        0        0    34292 2023-07-21 11:34:08.000000 yaylib-1.0.6/yaylib/responses.py
--rw-rw-rw-   0        0        0     4649 2023-07-28 02:06:59.000000 yaylib-1.0.6/yaylib/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:11:48.974284 yaylib-1.0.6/yaylib.egg-info/
--rw-rw-rw-   0        0        0    12824 2023-07-29 08:11:48.000000 yaylib-1.0.6/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-07-29 08:11:48.000000 yaylib-1.0.6/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 08:11:48.000000 yaylib-1.0.6/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-29 08:11:48.000000 yaylib-1.0.6/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-29 08:11:48.000000 yaylib-1.0.6/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 23:10:28.635736 yaylib-1.0.7/
+-rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0    12901 2023-08-02 23:10:28.634728 yaylib-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11986 2023-08-01 05:26:45.000000 yaylib-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-02 23:10:28.635736 yaylib-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1646 2023-07-30 14:47:09.000000 yaylib-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:10:28.586065 yaylib-1.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:22:00.000000 yaylib-1.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-07-28 03:15:02.000000 yaylib-1.0.7/tests/config.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_call.py
+-rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_chat.py
+-rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_group.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_post.py
+-rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_review.py
+-rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_thread.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_user.py
+-rw-rw-rw-   0        0        0     1908 2023-07-28 03:21:48.000000 yaylib-1.0.7/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:10:28.595564 yaylib-1.0.7/yaylib/
+-rw-rw-rw-   0        0        0      668 2023-07-25 06:44:17.000000 yaylib-1.0.7/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:10:28.633723 yaylib-1.0.7/yaylib/api/
+-rw-rw-rw-   0        0        0      715 2023-07-25 06:44:11.000000 yaylib-1.0.7/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0    14771 2023-07-31 09:13:51.000000 yaylib-1.0.7/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     9429 2023-07-23 06:18:02.000000 yaylib-1.0.7/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     2713 2023-07-28 02:06:00.000000 yaylib-1.0.7/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    14964 2023-07-29 04:53:58.000000 yaylib-1.0.7/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    23494 2023-07-30 13:58:08.000000 yaylib-1.0.7/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     8253 2023-07-31 09:13:58.000000 yaylib-1.0.7/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     7417 2023-07-18 08:52:45.000000 yaylib-1.0.7/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    33647 2023-07-30 13:59:19.000000 yaylib-1.0.7/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     4445 2023-07-30 13:59:56.000000 yaylib-1.0.7/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     5945 2023-07-18 08:52:45.000000 yaylib-1.0.7/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    23685 2023-07-30 14:01:24.000000 yaylib-1.0.7/yaylib/api/user.py
+-rw-rw-rw-   0        0        0     9409 2023-07-28 13:12:41.000000 yaylib-1.0.7/yaylib/api/websocket.py
+-rw-rw-rw-   0        0        0    86744 2023-08-01 05:27:28.000000 yaylib-1.0.7/yaylib/client.py
+-rw-rw-rw-   0        0        0    18880 2023-07-31 07:48:17.000000 yaylib-1.0.7/yaylib/config.py
+-rw-rw-rw-   0        0        0     2131 2023-07-18 08:52:45.000000 yaylib-1.0.7/yaylib/errors.py
+-rw-rw-rw-   0        0        0    56113 2023-07-21 11:49:21.000000 yaylib-1.0.7/yaylib/models.py
+-rw-rw-rw-   0        0        0    34292 2023-07-21 11:34:08.000000 yaylib-1.0.7/yaylib/responses.py
+-rw-rw-rw-   0        0        0     1643 2023-07-31 07:40:14.000000 yaylib-1.0.7/yaylib/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:10:28.619004 yaylib-1.0.7/yaylib.egg-info/
+-rw-rw-rw-   0        0        0    12901 2023-08-02 23:10:28.000000 yaylib-1.0.7/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-08-02 23:10:28.000000 yaylib-1.0.7/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 23:10:28.000000 yaylib-1.0.7/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-08-02 23:10:28.000000 yaylib-1.0.7/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-02 23:10:28.000000 yaylib-1.0.7/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-1.0.6/LICENSE` & `yaylib-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/PKG-INFO` & `yaylib-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.6
+Version: 1.0.7
 Summary: 同世代と趣味の通話コミュニティ - Yay! (イェイ) で、投稿やタイムラインの取得、リツイートやいいねの実行、フォローや投稿の検索など様々な機能を利用可能なAPIクライアントツールです。
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
 License: MIT
 Keywords: yay,yaylib,api,bot,tool,client,library,wrapper,ボット,ライブラリ,ツール
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div><a id="readme-top"></a></div>
 <div align="center">
     <img src="https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
@@ -62,44 +63,44 @@
   </ol>
 </details>
 
 <!-- インストール -->
 
 ## [<img src="https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-11d24c8c142b" width="30" height="30" />](https://github.com/qvco) Installation
 
-**※ Python 3.11 かそれ以上のバージョンが必要です。**
+**※ Python 3.10 以上のバージョンが必要です。**
 
-「yaylib」をインストールするには、以下のコマンドを実行します:
+「yaylib」をインストールするには、以下のコマンドをターミナル上で実行します:
 
 ```bash
 pip install yaylib
 ```
 
 <br>
 
 > **Note**
 > 開発バージョンをインストールする場合は、以下の手順を実行します:
 
 ```bash
-git clone https://github.com/qvco/yaylib
+git clone https://github.com/qvco/yaylib.git
 
 cd yaylib
 
 pip install -r requirements.txt
 
 pip install -e .
 ```
 
 「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
 ## [<img src="https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-3994884d2ba3" width="30" height="30" />](https://github.com/qvco) Quick Example
 
-### yaylib 利用で実現できること
+<!-- ### yaylib 利用で実現できること
 
 <table>
     <tr>
         <th>カテゴリ</th>
         <th>「yaylib」で自動化できること</th>
         <th>応用先</th>
     </tr>
@@ -138,15 +139,15 @@
             <li>DMを送る</li>
         </td>
 		<td>
             <li>Yay! 自動運用</li>
             <li>Yay! Bot開発</li>
         </td>
 	</tr>
-</table>
+</table> -->
 
 #### ✨ 投稿を作成する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.6 Summary:
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.7 Summary:
 åä¸ä»£ã¨è¶£å³ã®éè©±ã³ãã¥ããã£ - Yay! (ã¤ã§ã¤)
 ã§ãæç¨¿ãã¿ã¤ã ã©ã¤ã³ã®åå¾ããªãã¤ã¼ããããã­ã®å®è¡ããã©ã­ã¼ãæç¨¿ã®æ¤ç´¢ãªã©æ§ããªæ©è½ãå©ç¨å¯è½ãªAPIã¯ã©ã¤ã¢ã³ããã¼ã«ã§ãã
 Home-page: https://github.com/qvco/yaylib Download-URL: https://github.com/
 qvco/yaylib Author: Qvco, Konn Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn Maintainer-email: nikola.desuga@gmail.com License: MIT
 Keywords:
 yay,yaylib,api,bot,tool,client,library,wrapper,ããã,ã©ã¤ãã©ãª,ãã¼ã«
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown License-File: LICENSE
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
+text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
@@ -30,42 +31,29 @@
    2. ä½¿ç¨ä¾
    3. yaylib_ã§èªçããã­ããããã¡
    4. Buy_me_a_coffee
    5. å±åéçºã«ã¤ãã¦
    6. åè²¬äºé 
    7. å©ç¨è¨±è«¾
   ## [[https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-
-11d24c8c142b]](https://github.com/qvco) Installation **â» Python 3.11
-ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
-ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
+11d24c8c142b]](https://github.com/qvco) Installation **â» Python 3.10
+ä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
+ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããã¿ã¼ããã«ä¸ã§å®è¡ãã¾ã:
 ```bash pip install yaylib ```
 > **Note** >
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããå ´åã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
-```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
+```bash git clone https://github.com/qvco/yaylib.git cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## [
 [https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-
-3994884d2ba3]](https://github.com/qvco) Quick Example ### yaylib
-å©ç¨ã§å®ç¾ã§ãããã¨
-ã«ãã´ãª       ãyaylibãã§èªååã§ãããã¨     å¿ç¨å
-                               æç¨¿æå ±åå¾                                         SNSãã¼ã¿ãã¼ã±ãã£ã³ã°
-ãã¼ã¿åé�ã¦ã¼ã¶ã¼æå ±åå¾                             ãã¬ã³ãè§£æ
-                               äººæ°ã®ã¯ã¼ãåå¾                             ãã¼ãºèª¿æ»
-                               ãã©ã­ã¼/ãã©ã­ã¯ã¼æå ±åå¾
-ã¢ã«ã¦ã³ã�æç¨¿ãã                                                     Yay! èªåéç¨
-(æç¨¿é¢é£)     ãªãã¤ã¼ããã                                   Yay! Botéçº
-                               ããã­ãã
-                               ãã©ã­ã¼ãã/ãã©ã­ã¼è§£é¤ãã
-ã¢ã«ã¦ã³ã�ãã­ãã¯ãã/ãã­ãã¯è§£é¤ãYay! èªåéç¨
-(ã¦ã¼ã¶ã¼é¢ãã¥ã¼ããã/ãã¥ã¼ãè§£é¤ãYay! Botéçº
-                               DMãéã
-#### â¨ æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client()
-api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã")
-api.create_post("Hello with yaylib!") ``` #### â¨
+3994884d2ba3]](https://github.com/qvco) Quick Example  #### â¨
+æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client() api.login
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
+("Hello with yaylib!") ``` #### â¨
 åãè¾¼ã¿ãªã³ã¯ã®æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
 shared_url="https://github.com/qvco/yaylib") ``` #### â¨
 ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") filename = api.upload_image( image_type="post", #
```

### Comparing `yaylib-1.0.6/README.md` & `yaylib-1.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,44 +44,44 @@
   </ol>
 </details>
 
 <!-- インストール -->
 
 ## [<img src="https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-11d24c8c142b" width="30" height="30" />](https://github.com/qvco) Installation
 
-**※ Python 3.11 かそれ以上のバージョンが必要です。**
+**※ Python 3.10 以上のバージョンが必要です。**
 
-「yaylib」をインストールするには、以下のコマンドを実行します:
+「yaylib」をインストールするには、以下のコマンドをターミナル上で実行します:
 
 ```bash
 pip install yaylib
 ```
 
 <br>
 
 > **Note**
 > 開発バージョンをインストールする場合は、以下の手順を実行します:
 
 ```bash
-git clone https://github.com/qvco/yaylib
+git clone https://github.com/qvco/yaylib.git
 
 cd yaylib
 
 pip install -r requirements.txt
 
 pip install -e .
 ```
 
 「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
 ## [<img src="https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-3994884d2ba3" width="30" height="30" />](https://github.com/qvco) Quick Example
 
-### yaylib 利用で実現できること
+<!-- ### yaylib 利用で実現できること
 
 <table>
     <tr>
         <th>カテゴリ</th>
         <th>「yaylib」で自動化できること</th>
         <th>応用先</th>
     </tr>
@@ -120,15 +120,15 @@
             <li>DMを送る</li>
         </td>
 		<td>
             <li>Yay! 自動運用</li>
             <li>Yay! Bot開発</li>
         </td>
 	</tr>
-</table>
+</table> -->
 
 #### ✨ 投稿を作成する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
```

#### html2text {}

```diff
@@ -19,42 +19,29 @@
    2. ä½¿ç¨ä¾
    3. yaylib_ã§èªçããã­ããããã¡
    4. Buy_me_a_coffee
    5. å±åéçºã«ã¤ãã¦
    6. åè²¬äºé 
    7. å©ç¨è¨±è«¾
   ## [[https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-
-11d24c8c142b]](https://github.com/qvco) Installation **â» Python 3.11
-ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
-ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
+11d24c8c142b]](https://github.com/qvco) Installation **â» Python 3.10
+ä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
+ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããã¿ã¼ããã«ä¸ã§å®è¡ãã¾ã:
 ```bash pip install yaylib ```
 > **Note** >
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããå ´åã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
-```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
+```bash git clone https://github.com/qvco/yaylib.git cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## [
 [https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-
-3994884d2ba3]](https://github.com/qvco) Quick Example ### yaylib
-å©ç¨ã§å®ç¾ã§ãããã¨
-ã«ãã´ãª       ãyaylibãã§èªååã§ãããã¨     å¿ç¨å
-                               æç¨¿æå ±åå¾                                         SNSãã¼ã¿ãã¼ã±ãã£ã³ã°
-ãã¼ã¿åé�ã¦ã¼ã¶ã¼æå ±åå¾                             ãã¬ã³ãè§£æ
-                               äººæ°ã®ã¯ã¼ãåå¾                             ãã¼ãºèª¿æ»
-                               ãã©ã­ã¼/ãã©ã­ã¯ã¼æå ±åå¾
-ã¢ã«ã¦ã³ã�æç¨¿ãã                                                     Yay! èªåéç¨
-(æç¨¿é¢é£)     ãªãã¤ã¼ããã                                   Yay! Botéçº
-                               ããã­ãã
-                               ãã©ã­ã¼ãã/ãã©ã­ã¼è§£é¤ãã
-ã¢ã«ã¦ã³ã�ãã­ãã¯ãã/ãã­ãã¯è§£é¤ãYay! èªåéç¨
-(ã¦ã¼ã¶ã¼é¢ãã¥ã¼ããã/ãã¥ã¼ãè§£é¤ãYay! Botéçº
-                               DMãéã
-#### â¨ æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client()
-api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã")
-api.create_post("Hello with yaylib!") ``` #### â¨
+3994884d2ba3]](https://github.com/qvco) Quick Example  #### â¨
+æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client() api.login
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
+("Hello with yaylib!") ``` #### â¨
 åãè¾¼ã¿ãªã³ã¯ã®æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
 shared_url="https://github.com/qvco/yaylib") ``` #### â¨
 ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") filename = api.upload_image( image_type="post", #
```

### Comparing `yaylib-1.0.6/setup.py` & `yaylib-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "cryptography>=41.0.1",
     "websocket-client>=1.6.0",
 ]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
```

### Comparing `yaylib-1.0.6/tests/config.py` & `yaylib-1.0.7/tests/config.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/tests/test_call.py` & `yaylib-1.0.7/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/tests/test_cassandra.py` & `yaylib-1.0.7/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/tests/test_chat.py` & `yaylib-1.0.7/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/tests/test_group.py` & `yaylib-1.0.7/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/tests/test_misc.py` & `yaylib-1.0.7/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/tests/test_post.py` & `yaylib-1.0.7/tests/test_post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/tests/test_review.py` & `yaylib-1.0.7/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/tests/test_thread.py` & `yaylib-1.0.7/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/tests/test_user.py` & `yaylib-1.0.7/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/tests/test_utils.py` & `yaylib-1.0.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib/__init__.py` & `yaylib-1.0.7/yaylib/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib/api/__init__.py` & `yaylib-1.0.7/yaylib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib/api/call.py` & `yaylib-1.0.7/yaylib/api/call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib/api/cassandra.py` & `yaylib-1.0.7/yaylib/api/cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib/api/chat.py` & `yaylib-1.0.7/yaylib/api/chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib/api/group.py` & `yaylib-1.0.7/yaylib/api/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     GroupsResponse,
     GroupUserResponse,
     GroupUsersResponse,
     UnreadStatusResponse,
     UsersResponse,
     UsersByTimestampResponse,
 )
-from ..utils import signed_info_calculating
 
 
 def accept_moderator_offer(self, group_id: int, access_token: str = None):
     self._check_authorization(access_token)
     response = self._make_request(
         "PUT",
         endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/deputize",
@@ -144,14 +143,15 @@
     hide_from_game_eight: bool = None,
     allow_members_to_post_media: bool = None,
     allow_members_to_post_url: bool = None,
     guidelines: str = None,
     access_token: str = None,
 ) -> CreateGroupResponse:
     self._check_authorization(access_token)
+    timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.GROUPS_V3}/new",
         payload={
             "topic": topic,
             "description": description,
             "secret": secret,
@@ -165,18 +165,16 @@
             "allow_thread_creation_by": allow_thread_creation_by,
             "gender": gender,
             "generation_groups_limit": generation_groups_limit,
             "group_category_id": group_category_id,
             "cover_image_filename": cover_image_filename,
             "uuid": self.uuid,
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
-            "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid, int(datetime.now().timestamp())
-            ),
+            "timestamp": timestamp,
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
             "sub_category_id": sub_category_id,
             "hide_from_game_eight": hide_from_game_eight,
             "allow_members_to_post_image_and_video": allow_members_to_post_media,
             "allow_members_to_post_url": allow_members_to_post_url,
             "guidelines": guidelines,
         },
         data_type=CreateGroupResponse,
@@ -582,45 +580,43 @@
     return response
 
 
 def send_moderator_offers(
     self, group_id: int, user_ids: List[int], access_token: str = None
 ):
     self._check_authorization(access_token)
+    timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/deputize/mass",
         payload={
             "user_ids[]": user_ids,
             "uuid": self.uuid,
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
-            "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid, int(datetime.now().timestamp())
-            ),
+            "timestamp": timestamp,
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
         },
         access_token=access_token,
     )
     self.logger.info("Offered users to become a group moderator.")
     return response
 
 
 def send_ownership_offer(self, group_id: int, user_id: int, access_token: str = None):
     self._check_authorization(access_token)
+    timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/transfer",
         payload={
             "user_id": user_id,
             "uuid": self.uuid,
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
-            "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid, int(datetime.now().timestamp())
-            ),
+            "timestamp": timestamp,
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
         },
         access_token=access_token,
     )
     self.logger.info("Offered user to become a group owner.")
     return response
 
 
@@ -680,14 +676,15 @@
     hide_from_game_eight: bool = None,
     allow_members_to_post_media: bool = None,
     allow_members_to_post_url: bool = None,
     guidelines: str = None,
     access_token: str = None,
 ) -> GroupResponse:
     self._check_authorization(access_token)
+    timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/update",
         payload={
             "topic": topic,
             "description": description,
             "secret": secret,
@@ -702,18 +699,16 @@
             "gender": gender,
             "generation_groups_limit": generation_groups_limit,
             "group_category_id": group_category_id,
             "cover_image_filename": cover_image_filename,
             "sub_category_id": sub_category_id,
             "uuid": self.uuid,
             "api_key": self.api_key,
-            "timestamp": int(datetime.now().timestamp()),
-            "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid, int(datetime.now().timestamp())
-            ),
+            "timestamp": timestamp,
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
             "hide_from_game_eight": hide_from_game_eight,
             "allow_members_to_post_image_and_video": allow_members_to_post_media,
             "allow_members_to_post_url": allow_members_to_post_url,
             "guidelines": guidelines,
         },
         data_type=GroupResponse,
         access_token=access_token,
```

### Comparing `yaylib-1.0.6/yaylib/api/login.py` & `yaylib-1.0.7/yaylib/api/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,25 +21,18 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from datetime import datetime
 from cryptography.fernet import Fernet
 
-from ..config import Configs, Endpoints
+from ..config import Endpoints
 from ..errors import AuthenticationError, ForbiddenError
 from ..responses import LoginUserResponse, LoginUpdateResponse, TokenResponse
-from ..utils import (
-    Colors,
-    console_print,
-    load_session,
-    save_session,
-    decrypt,
-    signed_info_calculating,
-)
+from ..utils import Colors, console_print
 
 
 def change_email(
     self,
     email: str,
     password: str,
     email_grant_token: str = None,
@@ -110,31 +103,29 @@
     except AuthenticationError:
         return False
 
 
 def login_with_email(
     self, email: str, password: str, secret_key: str = None
 ) -> LoginUserResponse:
-    if self.save_session:
-        session = load_session(
-            base_path=self.base_path,
-            session_filename=self.session_filename,
-            check_email=email,
-        )
-        if session is not None and secret_key is not None:
+    if self.save_cookie_file:
+        cookies = self.load_cookies(email)
+
+        if cookies is not None and secret_key is not None:
             self.secret_key = secret_key
             self.fernet = Fernet(secret_key)
-            session = decrypt(fernet=self.fernet, session=session)
+            self.cookies = self.decrypt_cookies(self.fernet, cookies)
             self.session.headers.setdefault(
-                "Authorization", f"Bearer {session['access_token']}"
+                "Authorization", f"Bearer {self.access_token}"
             )
-            self.logger.info(f"Successfully logged in as '{session['user_id']}'")
-            return LoginUserResponse(session)
-        elif session is not None:
-            message = f"{Colors.WARNING}Session file found. The 'secret_key' must be provided to decrypt the credentials.{Colors.RESET}"
+            self.logger.info(f"Successfully logged in as '{self.user_id}'")
+            return LoginUserResponse(cookies)
+
+        elif cookies is not None:
+            message = f"{Colors.WARNING}Cookie file found. The 'secret_key' must be provided to decrypt the credentials.{Colors.RESET}"
             console_print(message)
 
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V3}/login_with_email",
         payload={
             "api_key": self.api_key,
@@ -147,29 +138,33 @@
 
     if response.access_token is None:
         raise ForbiddenError("Invalid email or password.")
 
     self.session.headers.setdefault("Authorization", f"Bearer {response.access_token}")
     self.logger.info(f"Successfully logged in as '{response.user_id}'")
 
-    if self.save_session:
+    if self.save_cookie_file:
         secret_key = Fernet.generate_key()
-        self.secret_key = secret_key
+        self.secret_key = secret_key.decode()
         self.fernet = Fernet(secret_key)
 
         console_print(
             f"Your 'secret_key' for {Colors.BOLD + email + Colors.RESET} is: {Colors.OKGREEN + secret_key.decode() + Colors.RESET}",
             "Please copy and securely store this key in a safe location.",
             "For more information, visit: https://github.com/qvco/yaylib/blob/master/docs/API-Reference/login/login.md",
         )
 
-        save_session(
-            base_path=self.base_path,
-            session_filename=self.session_filename,
-            fernet=self.fernet,
+        self.cookies = {
+            "access_token": response.access_token,
+            "refresh_token": response.refresh_token,
+            "user_id": response.user_id,
+            "email": email,
+        }
+
+        self.save_cookies(
             access_token=response.access_token,
             refresh_token=response.refresh_token,
             user_id=response.user_id,
             email=email,
         )
 
     return response
@@ -180,14 +175,15 @@
         self._check_authorization(access_token)
         response = self._make_request(
             "POST",
             endpoint=f"{Endpoints.USERS_V1}/logout",
             payload={"uuid": self.uuid},
             access_token=access_token,
         )
+        self._cookies = {}
         self.session.headers.pop("Authorization", None)
         self.logger.info("User has logged out.")
         return response
 
     except:
         self.logger.error("User is not logged in.")
         return None
@@ -207,15 +203,15 @@
         "POST",
         endpoint=f"{Endpoints.USERS_V2}/restore",
         payload={
             "user_id": user_id,
             "api_key": self.api_key,
             "uuid": self.uuid,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
         },
         access_token=access_token,
     )
     self.logger.info("User has been restored.")
     return response
```

### Comparing `yaylib-1.0.6/yaylib/api/misc.py` & `yaylib-1.0.7/yaylib/api/misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib/api/post.py` & `yaylib-1.0.7/yaylib/api/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     PostResponse,
     PostsResponse,
     PostLikersResponse,
     PostTagsResponse,
     LikePostsResponse,
     ValidationPostResponse,
 )
-from ..utils import signed_info_calculating
 
 
 def add_bookmark(
     self, user_id: int, post_id: int, access_token: str = None
 ) -> BookmarkPostResponse:
     self._check_authorization(access_token)
     response = self._make_request(
@@ -112,15 +111,15 @@
             "font_size": font_size,
             "color": color,
             "group_id": group_id,
             "call_type": call_type,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
             "category_id": category_id,
             "game_title": game_title,
             "joinable_by": joinable_by,
             "message_tags": message_tags,
             "attachment_filename": attachment_filename,
             "attachment_2_filename": attachment_2_filename,
             "attachment_3_filename": attachment_3_filename,
@@ -410,15 +409,15 @@
             "text": text,
             "font_size": font_size,
             "color": color,
             "group_id": group_id,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
         },
         data_type=Post,
         access_token=access_token,
     )
     self.logger.info("Share post has been created.")
     return response
 
@@ -1095,15 +1094,15 @@
         payload={
             "text": text,
             "font_size": font_size,
             "color": color,
             "message_tags": str(message_tags),
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
         },
         access_token=access_token,
     )
     self.logger.info("Post has been updated.")
     return response
```

### Comparing `yaylib-1.0.6/yaylib/api/review.py` & `yaylib-1.0.7/yaylib/api/review.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 """
 
 from datetime import datetime
 from typing import List
 
 from ..config import Endpoints
 from ..responses import ReviewsResponse
-from ..utils import signed_info_calculating
 
 
 def create_review(self, user_id: int, comment: str, access_token: str = None):
     self._check_authorization(access_token)
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V1}/reviews/{user_id}",
@@ -50,15 +49,15 @@
         endpoint=f"{Endpoints.USERS_V1}/reviews",
         payload={
             "user_ids": user_ids,
             "comment": comment,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(
+            "signed_info": self.generate_signed_info(
                 self.uuid, timestamp, shared_key=True
             ),
         },
         access_token=access_token,
     )
     self.logger.info("Reviews have been sent to multiple users.")
     return response
```

### Comparing `yaylib-1.0.6/yaylib/api/thread.py` & `yaylib-1.0.7/yaylib/api/thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib/api/user.py` & `yaylib-1.0.7/yaylib/api/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     UsersResponse,
     RankingUsersResponse,
     UserEmailResponse,
     HimaUsersResponse,
     UsersByTimestampResponse,
     UserTimestampResponse,
 )
-from ..utils import signed_info_calculating, signed_version_calculating
 
 
 def delete_footprint(self, user_id: int, footprint_id: int, access_token: str = None):
     self._check_authorization(access_token)
     response = self._make_request(
         "DELETE",
         endpoint=f"{Endpoints.USERS_V2}/{user_id}/footprints/{footprint_id}",
@@ -71,15 +70,15 @@
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V2}/destroy",
         payload={
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
         },
         access_token=access_token,
     )
     self.logger.info("User has been deleted.")
     return response
 
 
@@ -454,16 +453,16 @@
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V3}/register",
         payload={
             "app_version": self.api_version,
             "timestamp": timestamp,
             "api_key": self.api_key,
-            "signed_version": signed_version_calculating(),
-            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+            "signed_version": self.generate_signed_version(),
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
             "uuid": self.uuid,
             "nickname": nickname,
             "birth_date": birth_date,
             "gender": gender,
             "country_code": country_code,
             "biography": biography,
             "prefecture": prefecture,
@@ -603,16 +602,16 @@
         endpoint=f"{Endpoints.USERS_V2}/edit",
         payload={
             "nickname": nickname,
             "is_private": is_private,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
-            "signed_version": signed_version_calculating(),
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
+            "signed_version": self.generate_signed_version(),
         },
         access_token=access_token,
     )
     self.logger.info("Follow permission has been enabled.")
     return response
 
 
@@ -665,15 +664,15 @@
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V1}/language",
         payload={
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
             "language": language,
         },
         access_token=access_token,
     )
     self.logger.info("Language has been updated.")
     return response
 
@@ -703,15 +702,15 @@
             "country_code": country_code,
             "profile_icon_filename": profile_icon_filename,
             "cover_image_filename": cover_image_filename,
             "username": username,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+            "signed_info": self.generate_signed_info(self.device_uuid, timestamp),
         },
         access_token=access_token,
     )
     self.logger.info("User profile has been updated.")
     return response
```

### Comparing `yaylib-1.0.6/yaylib/api/websocket.py` & `yaylib-1.0.7/yaylib/api/websocket.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib/client.py` & `yaylib-1.0.7/yaylib/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,16 +336,16 @@
         - access_token: str - (optional)
         - proxy: str - (optional)
         - max_retries: int - (optional)
         - backoff_factor: float - (optional)
         - timeout: int - (optional)
         - err_lang: str - (optional)
         - base_path: str - (optional)
-        - save_session: bool - (optional)
-        - session_filename: str - (optional)
+        - save_cookie_file: bool - (optional)
+        - cookie_filename: str - (optional)
         - loglevel: int - (optional)
 
     <https://github.com/qvco/yaylib>
 
     ---
 
     ### Yay! (nanameue, Inc.) API Client
```

### Comparing `yaylib-1.0.6/yaylib/config.py` & `yaylib-1.0.7/yaylib/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 SOFTWARE.
 """
 
 from enum import Enum
 
 
 class Configs:
-    YAYLIB_VERSION = "1.0.6"
+    YAYLIB_VERSION = "1.0.7"
     YAY_API_VERSION = "3.20"
     YAY_VERSION_NAME = "3.20.1"
     YAY_API_VERSION_KEY = "d4420f4943bebe2831c20b2b4cb4a8c1"
     YAY_API_KEY = "ccd59ee269c01511ba763467045c115779fcae3050238a252f1bd1a4b65cfec6"
     YAY_SHARED_KEY = "yayZ1"
     YAY_STORE_KEY = "yayZ1payment"
     AGORA_APP_ID = "79046b8c9be54945b7f10a4d128d5395"
@@ -39,14 +39,15 @@
     YAY_REVIEW_HOST_2 = "cas-stg.yay.space"
     YAY_STAGING_HOST_1 = "stg.yay.space"
     YAY_STAGING_HOST_2 = "cas.yay.space"
     YAY_CABLE_HOST = "cable.yay.space"
     YAY_PRODUCTION_HOST = "api.yay.space"
     ID_CARD_CHECK_HOST_PRODUCTION = "idcardcheck.com"
     ID_CARD_CHECK_HOST_STAGING = "stg.idcardcheck.com"
+    COOKIE_PROPERTIES = ["access_token", "refresh_token", "user_id", "email"]
     USER_AGENT = "android 11 (3.5x 1440x2960 Galaxy S9)"
     REQUEST_HEADERS = {
         "Host": YAY_PRODUCTION_HOST,
         "X-App-Version": YAY_API_VERSION,
         "User-Agent": USER_AGENT,
         "X-Device-Info": f"yay {YAY_VERSION_NAME} {USER_AGENT}",
         "X-Device-Uuid": "",
```

### Comparing `yaylib-1.0.6/yaylib/errors.py` & `yaylib-1.0.7/yaylib/errors.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib/models.py` & `yaylib-1.0.7/yaylib/models.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib/responses.py` & `yaylib-1.0.7/yaylib/responses.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.6/yaylib.egg-info/PKG-INFO` & `yaylib-1.0.7/yaylib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.6
+Version: 1.0.7
 Summary: 同世代と趣味の通話コミュニティ - Yay! (イェイ) で、投稿やタイムラインの取得、リツイートやいいねの実行、フォローや投稿の検索など様々な機能を利用可能なAPIクライアントツールです。
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
 License: MIT
 Keywords: yay,yaylib,api,bot,tool,client,library,wrapper,ボット,ライブラリ,ツール
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div><a id="readme-top"></a></div>
 <div align="center">
     <img src="https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
@@ -62,44 +63,44 @@
   </ol>
 </details>
 
 <!-- インストール -->
 
 ## [<img src="https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-11d24c8c142b" width="30" height="30" />](https://github.com/qvco) Installation
 
-**※ Python 3.11 かそれ以上のバージョンが必要です。**
+**※ Python 3.10 以上のバージョンが必要です。**
 
-「yaylib」をインストールするには、以下のコマンドを実行します:
+「yaylib」をインストールするには、以下のコマンドをターミナル上で実行します:
 
 ```bash
 pip install yaylib
 ```
 
 <br>
 
 > **Note**
 > 開発バージョンをインストールする場合は、以下の手順を実行します:
 
 ```bash
-git clone https://github.com/qvco/yaylib
+git clone https://github.com/qvco/yaylib.git
 
 cd yaylib
 
 pip install -r requirements.txt
 
 pip install -e .
 ```
 
 「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
 ## [<img src="https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-3994884d2ba3" width="30" height="30" />](https://github.com/qvco) Quick Example
 
-### yaylib 利用で実現できること
+<!-- ### yaylib 利用で実現できること
 
 <table>
     <tr>
         <th>カテゴリ</th>
         <th>「yaylib」で自動化できること</th>
         <th>応用先</th>
     </tr>
@@ -138,15 +139,15 @@
             <li>DMを送る</li>
         </td>
 		<td>
             <li>Yay! 自動運用</li>
             <li>Yay! Bot開発</li>
         </td>
 	</tr>
-</table>
+</table> -->
 
 #### ✨ 投稿を作成する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.6 Summary:
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.7 Summary:
 åä¸ä»£ã¨è¶£å³ã®éè©±ã³ãã¥ããã£ - Yay! (ã¤ã§ã¤)
 ã§ãæç¨¿ãã¿ã¤ã ã©ã¤ã³ã®åå¾ããªãã¤ã¼ããããã­ã®å®è¡ããã©ã­ã¼ãæç¨¿ã®æ¤ç´¢ãªã©æ§ããªæ©è½ãå©ç¨å¯è½ãªAPIã¯ã©ã¤ã¢ã³ããã¼ã«ã§ãã
 Home-page: https://github.com/qvco/yaylib Download-URL: https://github.com/
 qvco/yaylib Author: Qvco, Konn Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn Maintainer-email: nikola.desuga@gmail.com License: MIT
 Keywords:
 yay,yaylib,api,bot,tool,client,library,wrapper,ããã,ã©ã¤ãã©ãª,ãã¼ã«
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown License-File: LICENSE
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
+text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
@@ -30,42 +31,29 @@
    2. ä½¿ç¨ä¾
    3. yaylib_ã§èªçããã­ããããã¡
    4. Buy_me_a_coffee
    5. å±åéçºã«ã¤ãã¦
    6. åè²¬äºé 
    7. å©ç¨è¨±è«¾
   ## [[https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-
-11d24c8c142b]](https://github.com/qvco) Installation **â» Python 3.11
-ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
-ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
+11d24c8c142b]](https://github.com/qvco) Installation **â» Python 3.10
+ä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
+ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããã¿ã¼ããã«ä¸ã§å®è¡ãã¾ã:
 ```bash pip install yaylib ```
 > **Note** >
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããå ´åã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
-```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
+```bash git clone https://github.com/qvco/yaylib.git cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## [
 [https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-
-3994884d2ba3]](https://github.com/qvco) Quick Example ### yaylib
-å©ç¨ã§å®ç¾ã§ãããã¨
-ã«ãã´ãª       ãyaylibãã§èªååã§ãããã¨     å¿ç¨å
-                               æç¨¿æå ±åå¾                                         SNSãã¼ã¿ãã¼ã±ãã£ã³ã°
-ãã¼ã¿åé�ã¦ã¼ã¶ã¼æå ±åå¾                             ãã¬ã³ãè§£æ
-                               äººæ°ã®ã¯ã¼ãåå¾                             ãã¼ãºèª¿æ»
-                               ãã©ã­ã¼/ãã©ã­ã¯ã¼æå ±åå¾
-ã¢ã«ã¦ã³ã�æç¨¿ãã                                                     Yay! èªåéç¨
-(æç¨¿é¢é£)     ãªãã¤ã¼ããã                                   Yay! Botéçº
-                               ããã­ãã
-                               ãã©ã­ã¼ãã/ãã©ã­ã¼è§£é¤ãã
-ã¢ã«ã¦ã³ã�ãã­ãã¯ãã/ãã­ãã¯è§£é¤ãYay! èªåéç¨
-(ã¦ã¼ã¶ã¼é¢ãã¥ã¼ããã/ãã¥ã¼ãè§£é¤ãYay! Botéçº
-                               DMãéã
-#### â¨ æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client()
-api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã")
-api.create_post("Hello with yaylib!") ``` #### â¨
+3994884d2ba3]](https://github.com/qvco) Quick Example  #### â¨
+æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client() api.login
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
+("Hello with yaylib!") ``` #### â¨
 åãè¾¼ã¿ãªã³ã¯ã®æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
 shared_url="https://github.com/qvco/yaylib") ``` #### â¨
 ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") filename = api.upload_image( image_type="post", #
```

### Comparing `yaylib-1.0.6/yaylib.egg-info/SOURCES.txt` & `yaylib-1.0.7/yaylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

