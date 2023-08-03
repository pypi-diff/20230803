# Comparing `tmp/sinetstream_cli-1.8.0.tar.gz` & `tmp/sinetstream_cli-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinetstream_cli-1.8.0.tar", last modified: Thu May 18 23:32:18 2023, max compression
+gzip compressed data, was "sinetstream_cli-1.8.1.tar", last modified: Thu Aug  3 07:55:30 2023, max compression
```

## Comparing `sinetstream_cli-1.8.0.tar` & `sinetstream_cli-1.8.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-18 23:32:18.449814 sinetstream_cli-1.8.0/
--rw-rw-r--   0 koie      (1004) koie      (1004)      535 2023-05-18 23:32:18.449814 sinetstream_cli-1.8.0/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)    12678 2023-05-16 06:28:56.000000 sinetstream_cli-1.8.0/README.md
--rw-rw-r--   0 koie      (1004) koie      (1004)     1817 2023-05-16 06:29:37.000000 sinetstream_cli-1.8.0/pyproject.toml
--rw-rw-r--   0 koie      (1004) koie      (1004)       38 2023-05-18 23:32:18.449814 sinetstream_cli-1.8.0/setup.cfg
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-18 23:32:18.441815 sinetstream_cli-1.8.0/src/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-18 23:32:18.445814 sinetstream_cli-1.8.0/src/sinetstream_cli/
--rw-rw-r--   0 koie      (1004) koie      (1004)       89 2023-01-12 00:12:25.000000 sinetstream_cli-1.8.0/src/sinetstream_cli/__main__.py
--rwxrwxr-x   0 koie      (1004) koie      (1004)     7850 2023-01-12 00:12:25.000000 sinetstream_cli-1.8.0/src/sinetstream_cli/sinetstream_cli.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-18 23:32:18.449814 sinetstream_cli-1.8.0/src/sinetstream_cli.egg-info/
--rw-rw-r--   0 koie      (1004) koie      (1004)      535 2023-05-18 23:32:18.000000 sinetstream_cli-1.8.0/src/sinetstream_cli.egg-info/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)      397 2023-05-18 23:32:18.000000 sinetstream_cli-1.8.0/src/sinetstream_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-05-18 23:32:18.000000 sinetstream_cli-1.8.0/src/sinetstream_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       73 2023-05-18 23:32:18.000000 sinetstream_cli-1.8.0/src/sinetstream_cli.egg-info/entry_points.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-05-18 23:32:18.000000 sinetstream_cli-1.8.0/src/sinetstream_cli.egg-info/not-zip-safe
--rw-rw-r--   0 koie      (1004) koie      (1004)       90 2023-05-18 23:32:18.000000 sinetstream_cli-1.8.0/src/sinetstream_cli.egg-info/requires.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       16 2023-05-18 23:32:18.000000 sinetstream_cli-1.8.0/src/sinetstream_cli.egg-info/top_level.txt
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:55:30.509379 sinetstream_cli-1.8.1/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      535 2023-08-03 07:55:30.509379 sinetstream_cli-1.8.1/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)    14050 2023-08-03 06:26:44.000000 sinetstream_cli-1.8.1/README.md
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1817 2023-08-03 07:54:32.000000 sinetstream_cli-1.8.1/pyproject.toml
+-rw-rw-r--   0 koie      (1004) koie      (1004)       38 2023-08-03 07:55:30.509379 sinetstream_cli-1.8.1/setup.cfg
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:55:30.509379 sinetstream_cli-1.8.1/src/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:55:30.509379 sinetstream_cli-1.8.1/src/sinetstream_cli/
+-rw-rw-r--   0 koie      (1004) koie      (1004)       89 2023-08-02 07:22:54.000000 sinetstream_cli-1.8.1/src/sinetstream_cli/__main__.py
+-rwxrwxr-x   0 koie      (1004) koie      (1004)     7838 2023-08-02 07:22:54.000000 sinetstream_cli-1.8.1/src/sinetstream_cli/sinetstream_cli.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:55:30.509379 sinetstream_cli-1.8.1/src/sinetstream_cli.egg-info/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      535 2023-08-03 07:55:30.000000 sinetstream_cli-1.8.1/src/sinetstream_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)      397 2023-08-03 07:55:30.000000 sinetstream_cli-1.8.1/src/sinetstream_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 07:55:30.000000 sinetstream_cli-1.8.1/src/sinetstream_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       73 2023-08-03 07:55:30.000000 sinetstream_cli-1.8.1/src/sinetstream_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 07:55:30.000000 sinetstream_cli-1.8.1/src/sinetstream_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 koie      (1004) koie      (1004)       90 2023-08-03 07:55:30.000000 sinetstream_cli-1.8.1/src/sinetstream_cli.egg-info/requires.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       16 2023-08-03 07:55:30.000000 sinetstream_cli-1.8.1/src/sinetstream_cli.egg-info/top_level.txt
```

### Comparing `sinetstream_cli-1.8.0/PKG-INFO` & `sinetstream_cli-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sinetstream_cli
-Version: 1.8.0
+Version: 1.8.1
 Summary: SINETStream Command Line Interface
 License: Apache License, Version 2.0
 Project-URL: homepage, https://github.com/nii-gakunin-cloud/sinetstream/tree/main/python/sample/cli
 Project-URL: repository, https://github.com/nii-gakunin-cloud/sinetstream
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Console
-Requires-Python: >=3.7
+Requires-Python: >=3.8
```

### Comparing `sinetstream_cli-1.8.0/README.md` & `sinetstream_cli-1.8.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+<!--
+Copyright (C) 2022 National Institute of Informatics
+
+Licensed to the Apache Software Foundation (ASF) under one
+or more contributor license agreements.  See the NOTICE file
+distributed with this work for additional information
+regarding copyright ownership.  The ASF licenses this file
+to you under the Apache License, Version 2.0 (the
+"License"); you may not use this file except in compliance
+with the License.  You may obtain a copy of the License at
+
+  http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing,
+software distributed under the License is distributed on an
+"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+KIND, either express or implied.  See the License for the
+specific language governing permissions and limitations
+under the License.
+-->
+
 # SINETStream CLI (Python版,Java版)
 
 ## 概要
 
 本ツールは
 Python版は
 [SINETStream Writer/ReaderAPI](https://www.sinetstream.net/docs/userguide/api-python.html)
@@ -12,18 +33,18 @@
 ブローカ等のオプション情報は `.sinetstream_config.yml` ファイルで指定できるが、
 コマンドラインからも指定できる。
 
 ## 前提条件
 
 * Python版
     * Python3.8以上
-    * SINETStream v1.7.0(Python)
+    * SINETStream v1.9.0(Python)
 * Java版
     * Java11以上
-    * SINETStream v1.7.3(Java)
+    * SINETStream v1.9.0(Java)
 * [SINETStream API 設定ファイル](https://github.com/nii-gakunin-cloud/sinetstream/blob/main/docs/userguide/config.md) (データ送受信先の接続情報等が記述されているもの)
 
 ## ビルド
 
 Python版ではビルドの必要はない。
 
 Java版では次のコマンドを実行してソースコードからビルドするか、SINETStream公式サイトからビルド生成物のzipファイルをダウンロードする。
@@ -64,65 +85,72 @@
 # 実行
 $ sinetstream_cli-*/bin/sinetstream_cli ...
 ```
 
 ## 書式
 
 sinetstream-cli write
-[--service *SERVICE*]
-[--config *CONFIG*]
-[--text]
-[--file *FILE*]
-[--message *MESSAGE*]
-[--line]
+[-nc|--no-config-file]
+[-s|--service *SERVICE*]
+[-c|--config *CONFIG*]
+[-t|--text]
+[-f|--file *FILE*]
+[-m|--message *MESSAGE*]
+[-l|--line]
+[-v|--verbose]
 [*KEY*=*VALUE* [*KEY*=*VALUE* ...]]
 
 sinetstream_cli read
-[--service *SERVICE*]
-[--config *CONFIG*]
-[--text]
-[--verbose]
-[--raw]
-[--file *DIR*]
-[--count *COUNT*]
+[-nc|--no-config-file]
+[-s|--service *SERVICE*]
+[-c|--config *CONFIG*]
+[-t|--text]
+[-v|--verbose]
+[-r|--raw]
+[-f|--file *DIR*]
+[-C|--count *COUNT*]
 [*KEY*=*VALUE* [*KEY*=*VALUE* ...]]
 
 ## 説明
 
 `sinetstream-cli write` を実行すると標準入力からメッセージを読み込んでSINETStream APIをつかってブローカーにメッセージを送信する。
 
 `sinetstream-cli read` を実行するとSINETStream APIをつかってブローカーからメッセージを受信して標準出力にメッセージを出力する。
 
 
 ## オプション
 
-* `--service` *SERVICE*
+* `-nc`, `--no-config-file`
+    * コンフィグファイルを読み込まない。
+    * コマンドラインだけから設定パラメータを指定する場合に指定する。
+* `-s` *SERVICE*, `--service` *SERVICE*
     * SINETStream API で使用するサービス名
     * CONFIGもSERVICEも指定されていない場合は実行時に `./.sinetstream_config.yml` が作成されダミーのサービスが定義される。
         * 終了時にこのファイルは削除される。
         * sinetstream_cliをおなじディレクトリで複数実行した場合は一時作成された `./.sinetstream_config.yml` は共有される。
-* --config *CONFIG*
+* `-c` *CONFIG*, `--config` *CONFIG*
     * SINETStream API で使用するコンフィグ名
     * 指定するとコンフィグサーバーから設定を取得する。
-* --text
+* `-t`, `--text`
     * value_typeをTEXTに設定して入出力はテキストとして扱われる。
-* --file *PATH*
+* `-f` *PATH*, `--file` *PATH*
     * writeのときは指定されたファイルからメッセージを読み込む。
     * readのときは指定されたディレクトリの下にメッセージを保存する。ファイル名は "トピック名-ランダム文字列-シリアル番号" である。
       (トピック名はパーセントエンコーディングされる。)
-* --message *MESSAGE*
+* `-m` *MESSAGE*, `--message` *MESSAGE*
     * writeのとき、コマンドラインから送信メッセージを指定する。
     * 省略時は標準入力から送信メッセージを読み込む。
-* --line
+* `-l`, `--line`
     * writeのとき、標準入力から送信メッセージを読み込むとき1行ごとに送信する。
-* --verbose
+* `-v`, `--verbose`
+    * ログレベルを上げる(複数回指定可)。
     * 受信メッセージを出力するときにトピック名とシリアル番号を表示する。
-* --raw
+* `-r`, `--raw`
     * 受信メッセージをだけを表示する。
-* --count *COUNT*
+* `-C` *COUNT*, `--count` *COUNT*
     * COUNT数のメッセージを受信したら終了する。
 * *KEY*=*VALUE*
     * SINETStreamの設定パラメータを個別に指定する。
     * 値はYAMLで書く。
     * 複数階層になるパラメータを指定するときは `.` で連結する。
     * 例:
         * ブローカーにmqtt.example.netを指定する: `brokers=mqtt.example.net`
@@ -134,24 +162,24 @@
 ### コマンドラインから1メッセージを送信
 
 #### <read側での入力内容>
 
 1メッセージを受信したらコマンドが終了するように `--count 1` を指定している。
 
 ```
-$ sinetstream_cli read --text type=mqtt brokers=mqtt topic=test --count 1
+$ sinetstream_cli read -nc --text type=mqtt brokers=mqtt topic=test --count 1
 
 ```
 
 #### <write側での入力内容>
 
 `--message` オプションをつかってコマンドラインで送信メッセージを指定している。
 
 ```
-$ sinetstream_cli write --text type=mqtt brokers=mqtt topic=test --message 'this is a test message.'
+$ sinetstream_cli write -nc --text type=mqtt brokers=mqtt topic=test --message 'this is a test message.'
 $
 ```
 
 #### <read側での出力内容>
 
 ```
 [#1] Received on "test"
@@ -169,24 +197,24 @@
 ```
 $ echo '{"test-1":{"value_type":"text","type":"mqtt","brokers":"mqtt","topic":"test"}}' >.sinetstream_config.yml
 ```
 
 #### <read側での入力内容>
 
 ```
-$ sinetstream_cli read --service test-1 --text --count 1
+$ sinetstream_cli read -nc --service test-1 --text --count 1
 [#1] Received on "test"
 this is a test message.
 
 ```
 
 #### <write側での入力内容>
 
 ```
-$ sinetstream_cli write --service test-1 --text --message 'this is a test message.'
+$ sinetstream_cli write -nc --service test-1 --text --message 'this is a test message.'
 $
 ```
 
 #### <read側での出力内容>
 
 ```
 [#1] Received on "test"
@@ -209,24 +237,24 @@
 $ echo 'this is a test message.' >message.txt
 $
 ```
 
 #### <read側での入力内容>
 
 ```
-$ sinetstream_cli read --text type=mqtt brokers=mqtt topic=test --count 1
+$ sinetstream_cli read -nc --text type=mqtt brokers=mqtt topic=test --count 1
 
 ```
 
 #### <write側での入力内容>
 
 `--file` オプションをつかって送信するファイルを指定している。
 
 ```
-$ sinetstream_cli write --text type=mqtt brokers=mqtt topic=test --file message.txt
+$ sinetstream_cli write -nc --text type=mqtt brokers=mqtt topic=test --file message.txt
 rm message.txt
 $
 ```
 
 #### <read側での出力内容>
 
 ```
@@ -245,22 +273,22 @@
 ### 受信時にメッセージ内容だけを表示
 
 #### <read側での入力内容>
 
 `--raw` オプションをつかって `[#1] Received on "test"` のようなメッセージのメタ情報表示を抑制している。
 
 ```
-$ sinetstream_cli read --text type=mqtt brokers=mqtt topic=test --count 1 --raw
+$ sinetstream_cli read -nc --text type=mqtt brokers=mqtt topic=test --count 1 --raw
 
 ```
 
 #### <write側での入力内容>
 
 ```
-$ sinetstream_cli write --text type=mqtt brokers=mqtt topic=test --message 'this is a test message.'
+$ sinetstream_cli write -nc --text type=mqtt brokers=mqtt topic=test --message 'this is a test message.'
 $
 ```
 
 #### <read側での出力内容>
 
 ```
 this is a test message.
@@ -282,24 +310,24 @@
 
 #### <read側での入力内容>
 
 
 `--raw` オプションをつけないと出力にメタ情報表示が含まれてバイナリデータが壊れる。
 
 ```
-$ sinetstream_cli read type=mqtt brokers=mqtt topic=test --count 1 --raw >receivd.bin
+$ sinetstream_cli read -nc type=mqtt brokers=mqtt topic=test --count 1 --raw >receivd.bin
 
 ```
 
 #### <write側での入力内容>
 
 テキストではなくバイナリメッセージを送るときは `--text` オプションをつけない。
 
 ```
-$ sinetstream_cli write type=mqtt brokers=mqtt topic=test <message.bin
+$ sinetstream_cli write -nc type=mqtt brokers=mqtt topic=test <message.bin
 $
 ```
 
 #### <read側での出力内容>
 
 ```
 
@@ -319,23 +347,23 @@
 ### 受信メッセージをファイルに保存
 
 #### <read側での入力内容>
 
 `--file` オプションをつかうと受信メッセージをファイルに保存できる。
 
 ```
-$ mkdir recved && sinetstream_cli read --text type=mqtt brokers=mqtt topic=test/sub --count 2 --file recved
+$ mkdir recved && sinetstream_cli read -nc --text type=mqtt brokers=mqtt topic=test/sub --count 2 --file recved
 
 ```
 
 #### <write側での入力内容>
 
 ```
-$ sinetstream_cli write --text type=mqtt brokers=mqtt topic=test/sub --message 'this is the first message.'
-$ sinetstream_cli write --text type=mqtt brokers=mqtt topic=test/sub --message 'this is the second message.'
+$ sinetstream_cli write -nc --text type=mqtt brokers=mqtt topic=test/sub --message 'this is the first message.'
+$ sinetstream_cli write -nc --text type=mqtt brokers=mqtt topic=test/sub --message 'this is the second message.'
 $
 ```
 
 #### <read側での出力内容>
 
 ```
 $
@@ -363,25 +391,25 @@
 ```
 
 ### パラメータ指定
 
 #### <read側での入力内容>
 
 ```
-$ sinetstream_cli read --text type=mqtt brokers=mqtt data_compression=true compression.algorithm=zstd topic=test --count 1
+$ sinetstream_cli read -nc --text type=mqtt brokers=mqtt data_compression=true compression.algorithm=zstd topic=test --count 1
 
 ```
 
 #### <write側での入力内容>
 
 深いところにあるパラメータを指定する場合は `.` でつなぐ。
 この例では圧縮アルゴリズムにzstdを指定している。
 
 ```
-$ sinetstream_cli write --text type=mqtt brokers=mqtt data_compression=true compression.algorithm=zstd topic=test --message 'this is a test message.'
+$ sinetstream_cli write -nc --text type=mqtt brokers=mqtt data_compression=true compression.algorithm=zstd topic=test --message 'this is a test message.'
 $
 ```
 
 #### <read側での出力内容>
 
 ```
 [#1] Received on "test"
@@ -403,25 +431,25 @@
 ```
 
 ### YAMLパラメータ
 
 #### <read側での入力内容>
 
 ```
-$ sinetstream_cli read --text type=kafka brokers='[kafka1,kafka2]' topic=test --count 1
+$ sinetstream_cli read -nc --text type=kafka brokers='[kafka1,kafka2]' topic=test --count 1
 
 ```
 
 #### <write側での入力内容>
 
 パラメータ指定で値は(SINETStream設定ファイルとおなじように)YAMLとして解釈される。
 この例ではKafkaのブローカ指定で2つのサーバーを指定している。
 
 ```
-$ sinetstream_cli write --text type=kafka brokers='[kafka1,kafka2]' topic=test --message 'this is a test message.'
+$ sinetstream_cli write -nc --text type=kafka brokers='[kafka1,kafka2]' topic=test --message 'this is a test message.'
 ...
 $
 ```
 
 #### <read側での出力内容>
 
 ```
@@ -433,26 +461,26 @@
 ```
 
 ### 1行ずつ送信
 
 #### <read側での入力内容>
 
 ```
-$ sinetstream_cli read --text type=mqtt brokers=mqtt topic=test --count 1
+$ sinetstream_cli read -nc --text type=mqtt brokers=mqtt topic=test --count 1
 
 ```
 
 #### <write側での入力内容>
 
 標準入力から複数行からなるデータを流し込んでも1メッセージとしてあつかわれる。
 
 ```
 $ echo 'aaa
 > bbb
-> ccc' | sinetstream_cli write --text type=mqtt brokers=mqtt topic=test
+> ccc' | sinetstream_cli write -nc --text type=mqtt brokers=mqtt topic=test
 $
 ```
 
 #### <read側での出力内容>
 
 ```
 [#1] Received on "test"
@@ -463,24 +491,24 @@
 ```
 
 `--line` オプションを指定すると1行ずつ送信できる。
 
 #### <read側での入力内容>
 
 ```
-$ sinetstream_cli read --text type=mqtt brokers=mqtt topic=test --count 3
+$ sinetstream_cli read -nc --text type=mqtt brokers=mqtt topic=test --count 3
 
 ```
 
 #### <write側での入力内容>
 
 ```
 $ echo 'aaa
 > bbb
-> ccc' | sinetstream_cli write --text type=mqtt brokers=mqtt topic=test --line
+> ccc' | sinetstream_cli write -nc --text type=mqtt brokers=mqtt topic=test --line
 $
 ```
 
 #### <read側での出力内容>
 
 ```
 [#1] Received on "test"
@@ -498,23 +526,23 @@
 受信側は行単位でJSONを処理できて都合がよい。
 
 * 参照 :  [jqコマンド](https://stedolan.github.io/jq/)
 
 #### <read側での入力内容>
 
 ```
-$ sinetstream_cli read --text type=mqtt brokers=mqtt topic=test --count 2 --raw | while read X; do echo "$X" | jq 'add'; done
+$ sinetstream_cli read -nc --text type=mqtt brokers=mqtt topic=test --count 2 --raw | while read X; do echo "$X" | jq 'add'; done
 
 ```
 
 #### <write側での入力内容>
 
 ```
-$ echo '[1,2,3]' | jq -c . | sinetstream_cli write --text type=mqtt brokers=mqtt topic=test
-$ echo '[10,20,30]' | jq -c . | sinetstream_cli write --text type=mqtt brokers=mqtt topic=test
+$ echo '[1,2,3]' | jq -c . | sinetstream_cli write -nc --text type=mqtt brokers=mqtt topic=test
+$ echo '[10,20,30]' | jq -c . | sinetstream_cli write -nc --text type=mqtt brokers=mqtt topic=test
 $
 ```
 
 #### <read側での出力内容>
 
 ```
 6
```

### Comparing `sinetstream_cli-1.8.0/pyproject.toml` & `sinetstream_cli-1.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sinetstream_cli"
 description = "SINETStream Command Line Interface"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {text = "Apache License, Version 2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3 :: Only",
     "Environment :: Console",
 ]
 dependencies = [
     "sinetstream>=1.7.0",
     "sinetstream-kafka>=1.7.0",
     "sinetstream-mqtt>=1.7.0",
     "sinetstream-s3>=1.7.0",
 ]
 #dynamic = ["version"]
-version = "1.8.0"
+version = "1.8.1"
 
 [project.scripts]
 sinetstream_cli = "sinetstream_cli.sinetstream_cli:main"
 
 [project.urls]
 homepage = "https://github.com/nii-gakunin-cloud/sinetstream/tree/main/python/sample/cli"
 repository = "https://github.com/nii-gakunin-cloud/sinetstream"
```

### Comparing `sinetstream_cli-1.8.0/src/sinetstream_cli/sinetstream_cli.py` & `sinetstream_cli-1.8.1/src/sinetstream_cli/sinetstream_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,67 +15,65 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-from logging import basicConfig, getLogger, INFO
-basicConfig(level=INFO)
+from logging import basicConfig, getLogger, WARNING, INFO, DEBUG
+basicConfig(level=WARNING)
 logger = getLogger(__name__)
 
-
-def make_temp_config():
-    import pathlib
-    import atexit
-    service = "tempserv"
-    path = pathlib.Path(".sinetstream_config.yml")
-    emptymap = "{}"
-    config = f"""\
-header:
-  version: 2
-config:
-  {service}: {emptymap}
-"""
-    try:
-        with path.open(mode="x") as f:
-            atexit.register(path.unlink)
-            f.write(config)
-        logger.info(f"the temporary config file {path} created")
-    except FileExistsError:
-        return None
-    return service
-
-
 sep1 = "."
 sep2 = "="
+loglvls = [WARNING, INFO, DEBUG]
+
+
+def increase_log_level(verbose_count):
+    basicConfig(level=loglvls[min(verbose_count, len(loglvls) - 1)])
 
 
 def make_parser(argv0, cmd):
     from argparse import ArgumentParser
     parser = ArgumentParser(
         prog=f"{argv0} {cmd}",
         description=f"SINETStream CLI: {cmd}",
         )
     parser.add_argument(
+        "-nc",
+        "--no-config-file",
+        action="store_true",
+        required=False,
+        help="don't load any sinetstream_config.yml")
+    parser.add_argument(
+        "-s",
         "--service",
         metavar="SERVICE",
         required=False,
         help="specify the service name")
     parser.add_argument(
+        "-c",
         "--config",
         metavar="CONFIG",
         required=False,
         help="specify the config name when using config service")
     parser.add_argument(
+        "-t",
         "--text",
         action="store_true",
         required=False,
         help="text mode")
     parser.add_argument(
+        "-v",
+        "--verbose",
+        default=0,
+        action="count",
+        required=False,
+        help="verbose mode")
+    parser.add_argument(
         "parameters",
         metavar=f"KEY{sep2}VALUE",
         type=str,
         nargs="*",
         help=("parameter for SINETStream "
               f"(ex: brokers{sep2}mqtt.example.net compression{sep1}algorithm{sep2}gzip)"))
     return parser
@@ -91,18 +89,21 @@
     return d
 
 
 def build_kwargs(args):
     from yaml import load, SafeLoader
     kwargs = {}
 
-    if args.config is None:
-        if args.service is None:
-            args.service = make_temp_config()
-    else:
+    if args.no_config_file is not None:
+        kwargs["no_config"] = args.no_config_file
+
+    if args.service is not None:
+        kwargs["service"] = args.service
+
+    if args.config is not None:
         kwargs["config"] = args.config
 
     for p in args.parameters:
         if sep2 not in p:
             logger.error(f"invalid parameter: {p}")
             exit(1)
         key, val = p.split(sep2, 1)
@@ -112,32 +113,37 @@
 
 
 def cmd_write(argv0, argv):
     from sinetstream import MessageWriter
 
     parser = make_parser(argv0, "write")
     parser.add_argument(
+        "-f",
         "--file",
         metavar="INPUT",
         type=str,
         required=False,
         help="write the contents of a file as the message")
     parser.add_argument(
+        "-m",
         "--message",
         metavar="MESSAGE",
         type=str,
         required=False,
         help="write a single message from the command line")
     parser.add_argument(
+        "-l",
         "--line",
         action="store_true",
         required=False,
         help="split separate lines into separate messages")
     args = parser.parse_args(argv)
 
+    increase_log_level(args.verbose)
+
     kwargs = build_kwargs(args)
 
     if args.text or args.message or args.line:
         setdict(kwargs, ["value_type"], "text")
     textmode = kwargs.get("value_type", "byte_array") == "text"
 
     if args.message is not None:
@@ -161,57 +167,53 @@
                 while True:
                     m = fp.read()
                     if len(m) == 0:
                         return
                     yield m
 
     try:
-        with MessageWriter(args.service, **kwargs) as writer:
+
+        with MessageWriter(**kwargs) as writer:
             for msg in get_message():
                 writer.publish(msg)
     except KeyboardInterrupt:
         pass
     exit()
 
 
 def cmd_read(argv0, argv):
     # from datetime import datetime
     from sinetstream import MessageReader
 
     parser = make_parser(argv0, "read")
     parser.add_argument(
-        "--verbose",
-        dest="ofmt",
-        default="verbose",
-        action="store_const",
-        const="verbose",
-        required=False,
-        help="print received messages verbosely")
-    parser.add_argument(
+        "-r",
         "--raw",
-        dest="ofmt",
-        action="store_const",
-        const="raw",
+        action="store_true",
         required=False,
         help="print just received messages")
     parser.add_argument(
+        "-f",
         "--file",
         metavar="DIR",
         required=False,
         type=str,
         help="save received messages under the specified directory")
     parser.add_argument(
+        "-C",
         "--count",
         metavar="N",
         required=False,
         type=int,
         default=0,
         help="exit after the given count of messages have been received")
     args = parser.parse_args(argv)
 
+    increase_log_level(args.verbose)
+
     kwargs = build_kwargs(args)
 
     if args.text:
         setdict(kwargs, ["value_type"], "text")
     textmode = kwargs.get("value_type", "byte_array") == "text"
 
     if args.file:
@@ -222,24 +224,24 @@
         import random
         import string
         rand = ''.join(random.choices(string.ascii_letters + string.digits, k=16))
         from urllib.parse import quote
 
     try:
         from sys import stdout
-        with MessageReader(args.service, **kwargs) as reader:
+        with MessageReader(**kwargs) as reader:
             n = 0
             for msg in reader:
                 n += 1
                 if args.file:
                     opath = Path(args.file, f"{quote(msg.topic, safe='')}-{rand}-{n}")
                     with open(opath, mode="w" if textmode else "wb") as f:
                         f.write(msg.value)
                 else:
-                    if args.ofmt == "verbose":
+                    if not args.raw:
                         # ts = datetime.fromtimestamp(msg.timestamp)
                         # output like "nats sub"
                         stdout.write(f'[#{n}] Received on "{msg.topic}"\n')
                     if textmode:
                         stdout.write(msg.value)
                         if msg.value[-1] != "\n":
                             stdout.write("\n")  # like nats sub
```

### Comparing `sinetstream_cli-1.8.0/src/sinetstream_cli.egg-info/PKG-INFO` & `sinetstream_cli-1.8.1/src/sinetstream_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sinetstream-cli
-Version: 1.8.0
+Version: 1.8.1
 Summary: SINETStream Command Line Interface
 License: Apache License, Version 2.0
 Project-URL: homepage, https://github.com/nii-gakunin-cloud/sinetstream/tree/main/python/sample/cli
 Project-URL: repository, https://github.com/nii-gakunin-cloud/sinetstream
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Console
-Requires-Python: >=3.7
+Requires-Python: >=3.8
```

