# Comparing `tmp/uvdiviner-2.0.3.tar.gz` & `tmp/uvdiviner-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvdiviner-2.0.3.tar", last modified: Thu Aug  3 08:24:10 2023, max compression
+gzip compressed data, was "uvdiviner-2.1.0.tar", last modified: Thu Aug  3 09:33:49 2023, max compression
```

## Comparing `uvdiviner-2.0.3.tar` & `uvdiviner-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 08:24:10.378968 uvdiviner-2.0.3/
--rw-rw-rw-   0        0        0    11558 2023-08-03 07:38:11.000000 uvdiviner-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     1337 2023-08-03 08:24:10.377968 uvdiviner-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      753 2023-08-03 07:53:10.000000 uvdiviner-2.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-08-03 08:24:10.378968 uvdiviner-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-08-03 08:23:49.000000 uvdiviner-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:24:10.352800 uvdiviner-2.0.3/uvdiviner/
--rw-rw-rw-   0        0        0       21 2023-08-03 07:57:35.000000 uvdiviner-2.0.3/uvdiviner/__init__.py
--rw-rw-rw-   0        0        0      713 2023-08-03 07:04:10.000000 uvdiviner-2.0.3/uvdiviner/colorize.py
--rw-rw-rw-   0        0        0      881 2023-08-03 07:44:59.000000 uvdiviner-2.0.3/uvdiviner/divine.py
--rw-rw-rw-   0        0        0      902 2023-06-24 07:04:37.000000 uvdiviner-2.0.3/uvdiviner/errors.py
--rw-rw-rw-   0        0        0     2849 2023-07-31 12:34:56.000000 uvdiviner-2.0.3/uvdiviner/evolution.py
--rw-rw-rw-   0        0        0     6259 2023-08-03 07:36:20.000000 uvdiviner-2.0.3/uvdiviner/main.py
--rw-rw-rw-   0        0        0     1820 2023-08-03 06:31:01.000000 uvdiviner-2.0.3/uvdiviner/progressbar.py
--rw-rw-rw-   0        0        0    56165 2023-06-24 12:01:07.000000 uvdiviner-2.0.3/uvdiviner/trigrams.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:24:10.376987 uvdiviner-2.0.3/uvdiviner.egg-info/
--rw-rw-rw-   0        0        0     1337 2023-08-03 08:24:10.000000 uvdiviner-2.0.3/uvdiviner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-08-03 08:24:10.000000 uvdiviner-2.0.3/uvdiviner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 08:24:10.000000 uvdiviner-2.0.3/uvdiviner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 08:24:10.000000 uvdiviner-2.0.3/uvdiviner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-03 08:24:10.000000 uvdiviner-2.0.3/uvdiviner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 09:33:49.994577 uvdiviner-2.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-08-03 07:38:11.000000 uvdiviner-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1349 2023-08-03 09:33:49.994577 uvdiviner-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2023-08-03 08:25:04.000000 uvdiviner-2.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 09:33:49.994577 uvdiviner-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      963 2023-08-03 09:33:25.000000 uvdiviner-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 09:33:49.964492 uvdiviner-2.1.0/uvdiviner/
+-rw-rw-rw-   0        0        0       21 2023-08-03 09:32:08.000000 uvdiviner-2.1.0/uvdiviner/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-08-03 07:04:10.000000 uvdiviner-2.1.0/uvdiviner/colorize.py
+-rw-rw-rw-   0        0        0     2818 2023-08-03 09:31:46.000000 uvdiviner-2.1.0/uvdiviner/divine.py
+-rw-rw-rw-   0        0        0      902 2023-06-24 07:04:37.000000 uvdiviner-2.1.0/uvdiviner/errors.py
+-rw-rw-rw-   0        0        0     2849 2023-07-31 12:34:56.000000 uvdiviner-2.1.0/uvdiviner/evolution.py
+-rw-rw-rw-   0        0        0     6527 2023-08-03 09:12:09.000000 uvdiviner-2.1.0/uvdiviner/main.py
+-rw-rw-rw-   0        0        0     1820 2023-08-03 06:31:01.000000 uvdiviner-2.1.0/uvdiviner/progressbar.py
+-rw-rw-rw-   0        0        0       13 2023-08-03 09:32:16.000000 uvdiviner-2.1.0/uvdiviner/settings.py
+-rw-rw-rw-   0        0        0    56165 2023-06-24 12:01:07.000000 uvdiviner-2.1.0/uvdiviner/trigrams.py
+drwxrwxrwx   0        0        0        0 2023-08-03 09:33:49.993212 uvdiviner-2.1.0/uvdiviner.egg-info/
+-rw-rw-rw-   0        0        0     1349 2023-08-03 09:33:49.000000 uvdiviner-2.1.0/uvdiviner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-08-03 09:33:49.000000 uvdiviner-2.1.0/uvdiviner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 09:33:49.000000 uvdiviner-2.1.0/uvdiviner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 09:33:49.000000 uvdiviner-2.1.0/uvdiviner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-03 09:33:49.000000 uvdiviner-2.1.0/uvdiviner.egg-info/top_level.txt
```

### Comparing `uvdiviner-2.0.3/LICENSE` & `uvdiviner-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.0.3/PKG-INFO` & `uvdiviner-2.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uvdiviner
-Version: 2.0.3
+Version: 2.1.0
 Summary: 基于周易蓍草占卜原理实现的中国古占卜.
-Home-page: https://gitee.com/unvisitor/augur
+Home-page: https://gitee.com/unvisitor/diviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
-Project-URL: Bug Tracker, https://gitee.com/unvisitor/augur/issues
+Project-URL: Bug Tracker, https://gitee.com/unvisitor/diviner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,40 +18,40 @@
 基于周易蓍草占卜原理实现的中国古占卜.
 
 感谢熊逸先生的《周易江湖》对本项目提供的基本原理支持.
 
 ## 安装
 使用`pip`安装:
 ```sh
-pip install diviner
+pip install uvdiviner
 ```
 
 ## 使用
 ### 完整占卜
 ```python
-from diviner.main import main
+from uvdiviner.main import main
 
 if __name__ == "__main__":
     main()
 ```
 
 ### 快速占卜
 ```python
-from diviner.divine import divine
+from uvdiviner.divine import divine
 
 def main():
     diagram = divine()
     print("本卦: ", diagram.name)
     diagram.variate()
     print("变卦: ", diagram.name)
 
 if __name__ == "__main__":
     main()
 ```
 
 ### 快速检定
 执行以下代码进行快速吉凶检定:
 ```python
-from diviner.divine import quick_check
+from uvdiviner.divine import quick_check
 
 print(quick_check()) # 返回 True 或 False
 ```
```

### Comparing `uvdiviner-2.0.3/README.md` & `uvdiviner-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 基于周易蓍草占卜原理实现的中国古占卜.
 
 感谢熊逸先生的《周易江湖》对本项目提供的基本原理支持.
 
 ## 安装
 使用`pip`安装:
 ```sh
-pip install diviner
+pip install uvdiviner
 ```
 
 ## 使用
 ### 完整占卜
 ```python
-from diviner.main import main
+from uvdiviner.main import main
 
 if __name__ == "__main__":
     main()
 ```
 
 ### 快速占卜
 ```python
-from diviner.divine import divine
+from uvdiviner.divine import divine
 
 def main():
     diagram = divine()
     print("本卦: ", diagram.name)
     diagram.variate()
     print("变卦: ", diagram.name)
 
 if __name__ == "__main__":
     main()
 ```
 
 ### 快速检定
 执行以下代码进行快速吉凶检定:
 ```python
-from diviner.divine import quick_check
+from uvdiviner.divine import quick_check
 
 print(quick_check()) # 返回 True 或 False
 ```
```

### Comparing `uvdiviner-2.0.3/setup.py` & `uvdiviner-2.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     name = "uvdiviner",
     version = uvdiviner.__version__,
     author = "Night Resurgent <fu050409@163.com>",
     author_email = "fu050409@163.com",
     description = "基于周易蓍草占卜原理实现的中国古占卜.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://gitee.com/unvisitor/augur",
+    url = "https://gitee.com/unvisitor/diviner",
     project_urls = {
-        "Bug Tracker": "https://gitee.com/unvisitor/augur/issues",
+        "Bug Tracker": "https://gitee.com/unvisitor/diviner/issues",
     },
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     license = "Apache-2.0",
```

### Comparing `uvdiviner-2.0.3/uvdiviner/colorize.py` & `uvdiviner-2.1.0/uvdiviner/colorize.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.0.3/uvdiviner/errors.py` & `uvdiviner-2.1.0/uvdiviner/errors.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.0.3/uvdiviner/evolution.py` & `uvdiviner-2.1.0/uvdiviner/evolution.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.0.3/uvdiviner/main.py` & `uvdiviner-2.1.0/uvdiviner/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from evolution import diagram, trigram
-from trigrams import data
-from progressbar import ProgressBar
-from divine import make_trigram
-from colorize import bright, light_white, cyan, light_green, light_red, light_magenta, light_yellow
+try:
+    from uvdiviner.evolution import diagram, trigram
+    from uvdiviner.trigrams import data
+    from uvdiviner.progressbar import ProgressBar
+    from uvdiviner.divine import make_trigram
+    from uvdiviner.colorize import bright, light_white, cyan, light_green, light_red, light_magenta, light_yellow
+    from uvdiviner.settings import DEBUG
+except ImportError:
+    from evolution import diagram, trigram
+    from trigrams import data
+    from progressbar import ProgressBar
+    from divine import make_trigram, update_data
+    from colorize import bright, light_white, cyan, light_green, light_red, light_magenta, light_yellow
+    from settings import DEBUG
 
 import time
 import sys
 
-DEBUG = True
-
 def clear_output():
     sys.stdout.write('\033[1J')
     sys.stdout.write('\033[H')
     sys.stdout.flush()
 
-def update_data(diagram):
-    for d in data:
-        if diagram.property == data[d]["属性"]:
-            diagram.data = data[d]
-    return diagram
-
 def get_useful_data(diagram):
     result = ""
 
     update_data(diagram)
     static = diagram.data
     static["卦名"] = diagram.name + "卦"
     diagram.variate()
@@ -78,15 +79,15 @@
         else:
             result += light_magenta("本卦断解: \n    ")
             result += light_green(static["爻辞"][6])
             result += "\n\n"
             name = "用九" if static["卦名"][:-1] == "乾" else "用六"
             result += cyan("此卦为 " + static["卦名"][:-1] + "之" + variable["卦名"][:-1] + f", 六爻全动, 请以 {name} 的爻辞为核心断解此次卜筮结果.")
 
-    return (static, variable, result)
+    return static, variable, result
 
 def main():
     global DEBUG
 
     if not DEBUG:
         y = True if input(
             bright(light_white("警告: 不建议在短时间内执行大量卜筮行为, 这可能会导致气运大幅下降. (已知悉? y/n) "))
@@ -101,29 +102,29 @@
         "天何言哉，叩之即应；神之灵矣，感而遂通。\n"
         "今有某人，有事关心，罔知休咎，罔释厥疑，\n"
         "惟神惟灵，望垂昭报，若可若否，尚明告之。\n"
         ),
         flush = True,
         )
 
-    trigrams = [make_trigram(), make_trigram(), make_trigram(),] if not DEBUG else [trigram(9), trigram(8), trigram(8),]
+    trigrams = [make_trigram(), make_trigram(), make_trigram(),] if not DEBUG else [trigram(8), trigram(8), trigram(6),]
 
     for i in range(1, 28):
         ProgressBar(i/55, name="内卦")
         if not DEBUG:
             time.sleep(1)
 
     print(light_red("\n\n" "某宫三象，吉凶未判，再求外象三爻，以成一卦，以决忧疑。" "\n"))
 
     for i in range(28, 56):
         ProgressBar(i/55, name="外卦")
         if not DEBUG:
             time.sleep(1)
 
-    trigrams += [make_trigram(), make_trigram(), make_trigram()] if not DEBUG else [trigram(9), trigram(9), trigram(9)]
+    trigrams += [make_trigram(), make_trigram(), make_trigram()] if not DEBUG else [trigram(9), trigram(8), trigram(8)]
     print("\n")
 
     if not DEBUG: time.sleep(1)
 
     dia = diagram(trigrams)
 
     static, variable, result = get_useful_data(dia)
```

### Comparing `uvdiviner-2.0.3/uvdiviner/progressbar.py` & `uvdiviner-2.1.0/uvdiviner/progressbar.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.0.3/uvdiviner/trigrams.py` & `uvdiviner-2.1.0/uvdiviner/trigrams.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.0.3/uvdiviner.egg-info/PKG-INFO` & `uvdiviner-2.1.0/uvdiviner.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uvdiviner
-Version: 2.0.3
+Version: 2.1.0
 Summary: 基于周易蓍草占卜原理实现的中国古占卜.
-Home-page: https://gitee.com/unvisitor/augur
+Home-page: https://gitee.com/unvisitor/diviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
-Project-URL: Bug Tracker, https://gitee.com/unvisitor/augur/issues
+Project-URL: Bug Tracker, https://gitee.com/unvisitor/diviner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,40 +18,40 @@
 基于周易蓍草占卜原理实现的中国古占卜.
 
 感谢熊逸先生的《周易江湖》对本项目提供的基本原理支持.
 
 ## 安装
 使用`pip`安装:
 ```sh
-pip install diviner
+pip install uvdiviner
 ```
 
 ## 使用
 ### 完整占卜
 ```python
-from diviner.main import main
+from uvdiviner.main import main
 
 if __name__ == "__main__":
     main()
 ```
 
 ### 快速占卜
 ```python
-from diviner.divine import divine
+from uvdiviner.divine import divine
 
 def main():
     diagram = divine()
     print("本卦: ", diagram.name)
     diagram.variate()
     print("变卦: ", diagram.name)
 
 if __name__ == "__main__":
     main()
 ```
 
 ### 快速检定
 执行以下代码进行快速吉凶检定:
 ```python
-from diviner.divine import quick_check
+from uvdiviner.divine import quick_check
 
 print(quick_check()) # 返回 True 或 False
 ```
```

