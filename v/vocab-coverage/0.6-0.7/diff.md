# Comparing `tmp/vocab-coverage-0.6.tar.gz` & `tmp/vocab-coverage-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocab-coverage-0.6.tar", last modified: Sun Jul  2 04:56:24 2023, max compression
+gzip compressed data, was "vocab-coverage-0.7.tar", last modified: Thu Aug  3 06:47:10 2023, max compression
```

## Comparing `vocab-coverage-0.6.tar` & `vocab-coverage-0.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-07-02 04:56:24.030416 vocab-coverage-0.6/
--rw-r--r--   0 tao        (502) staff       (20)    11357 2023-06-15 09:34:29.000000 vocab-coverage-0.6/LICENSE
--rw-r--r--   0 tao        (502) staff       (20)       30 2023-07-01 17:33:36.000000 vocab-coverage-0.6/MANIFEST.in
--rw-r--r--   0 tao        (502) staff       (20)    35485 2023-07-02 04:56:24.030252 vocab-coverage-0.6/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)    34660 2023-07-02 04:32:24.000000 vocab-coverage-0.6/README.md
--rw-r--r--   0 tao        (502) staff       (20)       38 2023-07-02 04:56:24.030466 vocab-coverage-0.6/setup.cfg
--rw-r--r--   0 tao        (502) staff       (20)     1556 2023-07-02 04:54:38.000000 vocab-coverage-0.6/setup.py
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-07-02 04:56:24.029027 vocab-coverage-0.6/vocab_coverage/
--rw-r--r--   0 tao        (502) staff       (20)      179 2023-07-01 16:39:12.000000 vocab-coverage-0.6/vocab_coverage/__init__.py
--rw-r--r--   0 tao        (502) staff       (20)   319549 2023-06-16 08:24:01.000000 vocab-coverage-0.6/vocab_coverage/charsets.json
--rw-r--r--   0 tao        (502) staff       (20)    11679 2023-06-26 16:57:52.000000 vocab-coverage-0.6/vocab_coverage/charsets.py
--rw-r--r--   0 tao        (502) staff       (20)     5327 2023-07-01 16:39:15.000000 vocab-coverage-0.6/vocab_coverage/coverage.py
--rw-r--r--   0 tao        (502) staff       (20)     7782 2023-06-26 18:05:18.000000 vocab-coverage-0.6/vocab_coverage/draw.py
--rw-r--r--   0 tao        (502) staff       (20)    19432 2023-07-01 16:07:09.000000 vocab-coverage-0.6/vocab_coverage/embedding.py
--rw-r--r--   0 tao        (502) staff       (20)    16153 2023-07-02 04:31:08.000000 vocab-coverage-0.6/vocab_coverage/generate.py
--rw-r--r--   0 tao        (502) staff       (20)     3606 2023-07-01 17:52:08.000000 vocab-coverage-0.6/vocab_coverage/main.py
--rw-r--r--   0 tao        (502) staff       (20)     3833 2023-07-01 17:17:46.000000 vocab-coverage-0.6/vocab_coverage/models.json
--rw-r--r--   0 tao        (502) staff       (20)     2733 2023-07-02 04:32:04.000000 vocab-coverage-0.6/vocab_coverage/models_readme.json
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-07-02 04:56:24.029981 vocab-coverage-0.6/vocab_coverage.egg-info/
--rw-r--r--   0 tao        (502) staff       (20)    35485 2023-07-02 04:56:23.000000 vocab-coverage-0.6/vocab_coverage.egg-info/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)      540 2023-07-02 04:56:24.000000 vocab-coverage-0.6/vocab_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 tao        (502) staff       (20)        1 2023-07-02 04:56:23.000000 vocab-coverage-0.6/vocab_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 tao        (502) staff       (20)       55 2023-07-02 04:56:23.000000 vocab-coverage-0.6/vocab_coverage.egg-info/entry_points.txt
--rw-r--r--   0 tao        (502) staff       (20)      146 2023-07-02 04:56:23.000000 vocab-coverage-0.6/vocab_coverage.egg-info/requires.txt
--rw-r--r--   0 tao        (502) staff       (20)       15 2023-07-02 04:56:23.000000 vocab-coverage-0.6/vocab_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-08-03 06:47:10.407049 vocab-coverage-0.7/
+-rw-r--r--   0 tao        (502) staff       (20)    11357 2023-07-26 03:19:02.000000 vocab-coverage-0.7/LICENSE
+-rw-r--r--   0 tao        (502) staff       (20)       30 2023-07-26 03:19:02.000000 vocab-coverage-0.7/MANIFEST.in
+-rw-r--r--   0 tao        (502) staff       (20)    51255 2023-08-03 06:47:10.406895 vocab-coverage-0.7/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)    50409 2023-08-01 15:20:38.000000 vocab-coverage-0.7/README.md
+-rw-r--r--   0 tao        (502) staff       (20)       38 2023-08-03 06:47:10.407090 vocab-coverage-0.7/setup.cfg
+-rw-r--r--   0 tao        (502) staff       (20)     1650 2023-08-03 06:35:32.000000 vocab-coverage-0.7/setup.py
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-08-03 06:47:10.405814 vocab-coverage-0.7/vocab_coverage/
+-rw-r--r--   0 tao        (502) staff       (20)      226 2023-07-26 03:19:03.000000 vocab-coverage-0.7/vocab_coverage/__init__.py
+-rw-r--r--   0 tao        (502) staff       (20)   319549 2023-07-26 03:19:03.000000 vocab-coverage-0.7/vocab_coverage/charsets.json
+-rw-r--r--   0 tao        (502) staff       (20)    11462 2023-07-27 18:14:41.000000 vocab-coverage-0.7/vocab_coverage/charsets.py
+-rw-r--r--   0 tao        (502) staff       (20)     4152 2023-07-27 18:08:33.000000 vocab-coverage-0.7/vocab_coverage/coverage.py
+-rw-r--r--   0 tao        (502) staff       (20)     8890 2023-07-27 18:09:17.000000 vocab-coverage-0.7/vocab_coverage/draw.py
+-rw-r--r--   0 tao        (502) staff       (20)    15766 2023-07-27 18:09:49.000000 vocab-coverage-0.7/vocab_coverage/embedding.py
+-rw-r--r--   0 tao        (502) staff       (20)    16861 2023-08-01 15:20:10.000000 vocab-coverage-0.7/vocab_coverage/generate.py
+-rw-r--r--   0 tao        (502) staff       (20)     6801 2023-07-27 18:13:44.000000 vocab-coverage-0.7/vocab_coverage/loader.py
+-rw-r--r--   0 tao        (502) staff       (20)     4556 2023-08-01 15:36:42.000000 vocab-coverage-0.7/vocab_coverage/main.py
+-rw-r--r--   0 tao        (502) staff       (20)     5588 2023-07-27 21:21:09.000000 vocab-coverage-0.7/vocab_coverage/reducer.py
+-rw-r--r--   0 tao        (502) staff       (20)     2825 2023-07-27 18:23:25.000000 vocab-coverage-0.7/vocab_coverage/utils.py
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-08-03 06:47:10.406654 vocab-coverage-0.7/vocab_coverage.egg-info/
+-rw-r--r--   0 tao        (502) staff       (20)    51255 2023-08-03 06:47:10.000000 vocab-coverage-0.7/vocab_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)      554 2023-08-03 06:47:10.000000 vocab-coverage-0.7/vocab_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 tao        (502) staff       (20)        1 2023-08-03 06:47:10.000000 vocab-coverage-0.7/vocab_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 tao        (502) staff       (20)       55 2023-08-03 06:47:10.000000 vocab-coverage-0.7/vocab_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 tao        (502) staff       (20)      185 2023-08-03 06:47:10.000000 vocab-coverage-0.7/vocab_coverage.egg-info/requires.txt
+-rw-r--r--   0 tao        (502) staff       (20)       15 2023-08-03 06:47:10.000000 vocab-coverage-0.7/vocab_coverage.egg-info/top_level.txt
```

### Comparing `vocab-coverage-0.6/LICENSE` & `vocab-coverage-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.6/setup.py` & `vocab-coverage-0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vocab-coverage',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     install_requires=[
         'Pillow',
         'protobuf==3.20.0',
         'sentencepiece',
         'tiktoken',
         'torch',
@@ -15,15 +15,19 @@
         'bs4',
         'pandas',
         'requests',
         'scikit-learn',
         'accelerate',
         'openai',
         'python-dotenv',
+        'umap-learn',
     ],
+    extras_require={
+        'cuml': ['cudf-cu12', 'cuml-cu12'],
+    },
     description='语言模型中文识字率分析\nA Python package designed to perform coverage analysis on Chinese vocabulary for language models.',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     include_package_data=True,
     author='Tao Wang',
     author_email='twang2218@gmail.com',
     url='https://github.com/twang2218/vocab-coverage',
```

### Comparing `vocab-coverage-0.6/vocab_coverage/charsets.json` & `vocab-coverage-0.7/vocab_coverage/charsets.json`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.6/vocab_coverage/charsets.py` & `vocab-coverage-0.7/vocab_coverage/charsets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import argparse
 import json
 from bs4 import BeautifulSoup
 import requests
+from vocab_coverage.utils import lighten_color, logger
 
 def get_chinese_chars():
     urls = [
         'https://www.zwbk2009.com/index.php?title=%E9%80%9A%E7%94%A8%E8%A7%84%E8%8C%83%E6%B1%89%E5%AD%97%E8%A1%A8%EF%BC%88%E4%B8%80%E7%BA%A7%E5%AD%97%E8%A1%A8%EF%BC%89',
         'https://www.zwbk2009.com/index.php?title=%E9%80%9A%E7%94%A8%E8%A7%84%E8%8C%83%E6%B1%89%E5%AD%97%E8%A1%A8%EF%BC%88%E4%BA%8C%E7%BA%A7%E5%AD%97%E8%A1%A8%EF%BC%89',
         'https://www.zwbk2009.com/index.php?title=%E9%80%9A%E7%94%A8%E8%A7%84%E8%8C%83%E6%B1%89%E5%AD%97%E8%A1%A8%EF%BC%88%E4%B8%89%E7%BA%A7%E5%AD%97%E8%A1%A8%EF%BC%89',
     ]
@@ -57,67 +58,55 @@
     charset = {}
     # 获取《通用规范汉字表》中一级、二级、三级字表'
     s1 = get_chinese_chars()
     charset['《通用规范汉字表》一级汉字'] = s1[0]
     charset['《通用规范汉字表》二级汉字'] = s1[1]
     charset['《通用规范汉字表》三级汉字'] = s1[2]
     for k, v in charset.items():
-        print(f"{k}共有{len(v)}个汉字")
+        logger.info(f"{k}共有{len(v)}个汉字")
 
     base_chars = set()
     for cc in charset.values():
         base_chars.update(cc)
-    print(f"《通用规范汉字表》共有{len(base_chars)}个汉字")
+    logger.info(f"《通用规范汉字表》共有{len(base_chars)}个汉字")
     s2 = generate_cnc_chars()
 
     extra_chars = []
     for c in s2[0]:
         if c not in base_chars:
             extra_chars.append(c)
     charset['《常用國字標準字體表》甲表(增)'] = extra_chars
-    print(f"《常用國字標準字體表》甲表共有{len(s2[0])}个汉字，其中{len(extra_chars)}个汉字不在《通用规范汉字表》中")
+    logger.info(f"《常用國字標準字體表》甲表共有{len(s2[0])}个汉字，其中{len(extra_chars)}个汉字不在《通用规范汉字表》中")
     for c in extra_chars:
         base_chars.update(c)
 
     extra_chars = []
     for c in s2[1]:
         if c not in base_chars:
             extra_chars.append(c)
     charset['《常用國字標準字體表》乙表(增)'] = extra_chars
-    print(f"《常用國字標準字體表》乙表共有{len(s2[1])}个汉字，其中{len(extra_chars)}个汉字不在《通用规范汉字表》中")
+    logger.info(f"《常用國字標準字體表》乙表共有{len(s2[1])}个汉字，其中{len(extra_chars)}个汉字不在《通用规范汉字表》中")
     for c in extra_chars:
         base_chars.update(c)
 
     chars = generate_unicode_chinese_chars()
     extra_chars = []
     for c in chars:
         if c not in base_chars:
             extra_chars.append(c)
-    print(f"《Unicode中日韩统一表意文字》共有{len(chars)}个汉字，其中{len(extra_chars)}个汉字不在《通用规范汉字表》和《常用國字標準字體表》中")
+    logger.info(f"《Unicode中日韩统一表意文字》共有{len(chars)}个汉字，其中{len(extra_chars)}个汉字不在《通用规范汉字表》和《常用國字標準字體表》中")
     charset['《Unicode中日韩统一表意文字》(增)'] = extra_chars
 
-    print(f"共有{sum([len(c) for c in charset.values()])}个汉字")
+    logger.info(f"共有{sum([len(c) for c in charset.values()])}个汉字")
 
     # 保存到JSON文件
     with open(filename, 'w') as f:
         json.dump(charset, f, ensure_ascii=False, indent=4)
 
 
-from PIL import ImageColor
-
-def lighten_color(color, amount=0.2):
-    if isinstance(color, str):
-        color = ImageColor.getrgb(color)
-
-    white = 255
-    adjusted_color = tuple(
-        int(round(old_value * (1 - amount) + white * amount))
-        for old_value in color
-    )
-    return adjusted_color
 
 class CharsetClassifier:
     def __init__(self, charsets:dict, is_detailed=False):
         self.charsets = charsets
         self.is_detailed = is_detailed
         self.palette = None
```

### Comparing `vocab-coverage-0.6/vocab_coverage/draw.py` & `vocab-coverage-0.7/vocab_coverage/draw.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import random
 from typing import List
 from PIL import Image, ImageDraw, ImageColor, ImageFont
 from sklearn.preprocessing import MinMaxScaler
+from vocab_coverage.utils import lighten_color, logger
 
 default_palette = [
     '#B04759', '#E76161','#F99B7D',
     '#146C94', '#19A7CE', '#E893CF',
 ]
 
 # apt install fonts-noto-cjk fonts-anonymous-pro fonts-noto-color-emoji
@@ -38,88 +39,109 @@
     font_paths = [
         "Anonymous Pro",
         "DejaVuSansMono",
         "Arial",
     ]
     return get_available_font_from_list(font_paths, size=size)
 
-def draw_vocab_graph(model_name: str, charset_stats:dict, vocab_size:int, filename: str, width=100, height=100, cell_size=10, margin=40, palette=default_palette):
+def draw_vocab_graph(model_name: str, charset_stats:dict, vocab_size:int, width=100, height=100, cell_size=60, margin=300, palette=default_palette):
     total_chars = sum([s['total'] for s in charset_stats.values()])
 
     # 定义图像大小
     image_width = width * cell_size + 1 + margin * 2
     height = total_chars // width + 1
-    image_height = height * cell_size + 1 + margin * 6
+    image_height = height * cell_size + 1 + margin * 8
 
     # 创建新的空白图像
-    image = Image.new("RGBA", (image_width, image_height), "#EEEEEE")
+    image = Image.new("RGB", (image_width, image_height), "#FFFFFF")
 
     # 获取图像的像素访问对象
     pixels = image.load()
 
     grid_color = (255,255,255, 40)
 
     # 根据map绘制栅格
     draw = ImageDraw.Draw(image)
+    # 画上底图
+    draw.rectangle((margin, margin, width * cell_size + margin, height * cell_size + margin), fill='#EEEEEE')
+    # 画每一个方块
     i = 0
     level = 0
+    zh_font = get_chinese_font(int(cell_size*0.7))
     for name, stats in charset_stats.items():
         for j, m in enumerate(stats['map']):
             x = i % width
             y = i // width
             c = ImageColor.getrgb(palette[level])
-            alpha = int(30 + m * 225)
-            c = c[:3] + (alpha,)
+            # 画方块
             draw.rectangle((x * cell_size + 1 + margin,
                 y * cell_size + 1 + margin,
                 x * cell_size + (cell_size-1) + margin,
                 y * cell_size + (cell_size-1) + margin
-                ), fill=c)
+                ), fill=lighten_color(c, 0.7-m))
+            ch = stats['chars'][j]
+            # 方块内填入文字
+            draw.text(
+                (x * cell_size + int(0.15*cell_size) + margin, y * cell_size - int(0.05*cell_size) + margin),
+                ch,
+                font=zh_font,
+                fill=lighten_color(c, 0.5-m))
             i += 1
         level += 1
     
     # 在图片左下角写入模型名称
     draw.text(
-        (margin + 10, image_height - margin - 60),
+        (margin + int(margin/4), image_height - margin - int(4.5*margin)),
         "[ {} ]".format(model_name),
         fill="#000000",
         align="right",
-        font=get_english_font(30))
+        font=get_english_font(int(margin*0.75)))
     # 在模型名称下方写入字表大小
     draw.text(
-        (margin + 40, image_height - margin - 20),
-        "vocab size: {:,} ".format(vocab_size),
+        (margin + int(0.3*margin), image_height - margin - int(3.5*margin)),
+        "[ vocab size: {:,} ]".format(vocab_size),
         fill="#000000",
         align="right",
-        font=get_english_font(20))
+        font=get_english_font(int(margin/2)))
 
     # 在图片右下角写入字表统计信息
-    zh_font = get_chinese_font(25)
+    zh_font = get_chinese_font(int(margin*0.5))
+
+    # 画字符集图例方块
+    legend_y = image_height - margin - int(3.5*margin)
+    box_width = int(margin / 2)
+    box_start_x = image_width - margin - int(15.5*margin)
+    box_start_y = legend_y + int(0.1*margin)
+    box_margin = int(0.2*box_width)
+    for i, color in enumerate(palette):
+        x = box_start_x
+        y = box_start_y + i * (box_width + box_margin)
+        draw.rectangle((x, y, x+box_width, y+box_width), fill=color)
+    # 画字符集名称
     stats_name = ""
     for name in charset_stats.keys():
         stats_name += "{}:\n".format(name)
     draw.text(
-        (image_width - margin - 700, image_height - margin - 140),
+        (image_width - margin - int(15*margin), legend_y),
         stats_name,
         fill="#000000",
         align="left",
         font=zh_font)
-    
+    # 画字符集统计信息
     stats_value = ""
     for s in charset_stats.values():
         stats_value += "{:4} / {:4}  ({:.2%})\n".format(s['known'], s['total'], float(s['known'])/s['total'])
     draw.text(
-        (image_width - margin - 270, image_height - margin - 140),
+        (image_width - margin - 6*margin, legend_y),
         stats_value,
         fill="#000000",
         align="right",
         font=zh_font)
 
-    # 保存图像
-    image.save(filename)
+    return image
 
 
 from vocab_coverage.charsets import CharsetClassifier
 import math
 
 # model: {model_name, model, tokenizer, vocab, embeddings, embeddings_2d}
 # def draw_vocab_embeddings(model, charsets, width=8000, height=8000, is_detail=False, debug=False):
@@ -143,24 +165,24 @@
 
     # CharsetClassifier
     classifier = CharsetClassifier(charsets=charsets, is_detailed=is_detailed)
     word_type_count = {k: 0 for k in classifier.get_types()}
     palette = classifier.get_palette(with_prefix_palette=True)
 
     if debug:
-        # print(f"palette: {palette}")
-        print(f"[{model_name}]: draw embedding point: {vocab_size}")
+        # logger.debug(f"palette: {palette}")
+        logger.debug(f"[{model_name}]: draw embedding point: {vocab_size}")
 
     # draw embedding point
     # clip font size to [12, margin]
     font_size = int(margin * 2000 / vocab_size)
     font_size = int(min(max(font_size, 12), margin))
     zh_font = get_chinese_font(font_size)
     if debug:
-        print(f"font size: {font_size}, font: {zh_font.getname()}")
+        logger.debug(f"font size: {font_size}, font: {zh_font.getname()}")
     for i, (x, y) in enumerate(embeddings_2d_norm):
         word = vocab[i]
         word_type = classifier.get_word_type(word)
         word_type_count[word_type] += 1
 
         if word.startswith('##'):
             word_type = '##' + word_type
@@ -169,18 +191,18 @@
 
         # draw text
         x = x * width + margin * 2
         y = y * height + margin * 2
         try:
             draw.text((x, y), word, fill=c, stroke_width=1, stroke_fill='#F0F0F0', font=zh_font)
         except Exception as e:
-            print(f"[{model_name}]: warning: draw text error: {e}")
+            logger.error(f"[{model_name}]: warning: draw text error: {e}")
 
     if debug:
-        print(f"[{model_name}]: token type counts: {word_type_count}")
+        logger.debug(f"[{model_name}]: token type counts: {word_type_count}")
     # draw model name
     font_size = int(margin / 2)
     draw.text((margin, image_height - (3*margin)),
         f'[ {model_name} ]',
         fill='#000000',
         font=get_english_font(font_size))
 
@@ -206,19 +228,19 @@
     font_count = get_chinese_font(int(font_size/1.7))
     for i, word_type in enumerate(word_type_count.keys()):
         row = int(i % column_size)
         col = int(i / column_size)
         x = image_width - ((column)*column_width) + (col * column_width)
         y = image_height - ((column_size-row)*(box_width*1.4)) - (margin)
         color = palette[word_type]
-        # print(i, row, col, x, y, word_type, color)
+        # logger.debug(i, row, col, x, y, word_type, color)
 
         # draw box
         draw.rectangle((x, y, x+box_width, y+box_width), fill=color)
-        # print(word_type, color)
+        # logger.debug(word_type, color)
 
         # draw label
         draw.text((x+box_width*1.5, int(y - font_size*0.3)),
             f'{word_type}',
             fill='#000000',
             font=font_label)
         # draw count
```

### Comparing `vocab-coverage-0.6/vocab_coverage/generate.py` & `vocab-coverage-0.7/vocab_coverage/generate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,72 @@
 # -*- coding: utf-8 -*-
 
 import argparse
+import io
 import json
+import logging
 import os
 import sys
 import traceback
 from typing import List
+import yaml
 
 if __name__ == "__main__":
     sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 from vocab_coverage import coverage_analysis, embedding_analysis
+from vocab_coverage.utils import logger
 
 DEFAULT_IMAGE_FOLDER = "images"
 
-def load_model_list(filename:str="models.json") -> List[dict]:
-    base_dir = os.path.dirname(os.path.abspath(__file__))
-    filename = os.path.join(base_dir, filename)
-    try:
-        with open(filename, "r") as f:
-            models = json.load(f)
-        return models
-    except Exception as e:
-        print(f"Cannot load model list from {filename}")
-        traceback.print_exc()
-        exit(1)
-
 def get_model_basename(model_name:str):
     basename = model_name.replace("/", "_")
     return basename
 
 def get_standard_coverage_filename(model_name:str, folder:str=DEFAULT_IMAGE_FOLDER):
-    folder = os.path.join(folder, "coverage")
+    folder = os.path.join(folder, "assets", "coverage")
     basename = get_model_basename(model_name)
-    filename = f"{folder}/{basename}.coverage.png"
+    filename = f"{folder}/{basename}.coverage.jpg"
     return filename
 
 def get_standard_embedding_filename(model_name:str, embedding_type:str, folder:str=DEFAULT_IMAGE_FOLDER):
-    folder = os.path.join(folder, "embeddings")
+    folder = os.path.join(folder, "assets", "embeddings")
     basename = get_model_basename(model_name)
     filename = f"{folder}/{basename}.embeddings.{embedding_type}.jpg"
     return filename
 
 def find_coverage_file(model_name:str, folder:str=DEFAULT_IMAGE_FOLDER):
-    folder = os.path.join(folder, "coverage")
+    folder = os.path.join(folder, "assets", "coverage")
     basename = get_model_basename(model_name)
     candidates = [
         get_standard_coverage_filename(model_name),
         f"{folder}/{basename}.png",
         f"{folder}/{basename}_coverage.png",
         f"{folder}/coverage.{basename}.png",
         f"{folder}/{basename}.coverage.png",
     ]
     for filename in candidates:
-        # print(filename)
+        # logger.debug(filename)
         if os.path.exists(filename):
             return filename
     return None
 
 def find_embedding_file(model_name:str, embedding_type:str, folder:str=DEFAULT_IMAGE_FOLDER):
-    folder = os.path.join(folder, "embeddings")
+    folder = os.path.join(folder, "assets", "embeddings")
     basename = get_model_basename(model_name)
     candidates = [
         get_standard_embedding_filename(model_name, embedding_type),
         f"{folder}/embeddings_{basename}.{embedding_type}.jpg",
         f"{folder}/embeddings.{basename}.{embedding_type}.jpg",
     ]
     if embedding_type == "input":
         candidates.append(f"{folder}/embeddings_{basename}.jpg")
         candidates.append(f"{folder}/embeddings.{basename}.jpg")
     for filename in candidates:
-        # print(filename)
+        # logger.debug(filename)
         if os.path.exists(filename):
             return filename
     return None
 
 def get_thumbnail_filename(filename:str, folder:str=DEFAULT_IMAGE_FOLDER):
     basename = os.path.basename(filename)
     basename = basename.replace(".jpg", ".thumbnail.jpg")
@@ -83,183 +75,215 @@
 
 def find_thumbnail_file(filename:str):
     thumbnail = get_thumbnail_filename(filename)
     if os.path.exists(thumbnail):
         return thumbnail
     return None
 
-def generate_markdown(models:List[dict], output:str="graphs.md", section_level:int=2):
-    with open(output, "w") as f:
-        section_mark = "#" * section_level
-        for section in models:
-            f.write(f"{section_mark} {section['name']}\n\n")
-            # Table header
-            f.write("| 名称| ![](images/empty.png) 中文覆盖率 | ![](images/empty.png) 输入词向量分布 | ![](images/empty.png) 输出词向量分布 |\n")
-            f.write("| :---: | :---: | :---: | :---: |\n")
-            # Table body
-            for model_name in section["models"]:
-                basename = get_model_basename(model_name)
-                coverage = find_coverage_file(model_name)
-                if coverage is None:
-                    print(f"Cannot find coverage file for {model_name}")
-                input_embedding = find_embedding_file(model_name, "input")
-                if input_embedding is None and not 'openai' in model_name.lower():
-                    print(f"Cannot find input embedding file for {model_name}")
-                output_embedding = find_embedding_file(model_name, "output")
-                if output_embedding is None and not 'openai' in model_name.lower():
-                    print(f"Cannot find output embedding file for {model_name}")
-                if coverage is None and input_embedding is None and output_embedding is None:
-                    print(f"Cannot find any file for {model_name}")
-                    continue
-                else:
-                    # Name
-                    # model_name = f'<b style="display: inline-block; transform: rotate(-90deg);">{model_name}</b>'
-                    if "/" in model_name:
-                        org, name = model_name.split("/")
-                        model_name = f'<p>{org}</p><p>/</p><p>{name}</p>'
-                    model_name = f'<b>{model_name}</b>'
-                    # Coverage
-                    if coverage is None or len(coverage) == 0:
-                        coverage = " "
-                    else:
-                        coverage = f"![Vocab Coverage for {model_name}]({coverage})"
-                    # Input Embedding
-                    if input_embedding is None or len(input_embedding) == 0:
-                        input_embedding = " "
-                    else:
-                        input_embedding_thumbnail = find_thumbnail_file(input_embedding)
-                        if input_embedding_thumbnail is None:
-                            print(f"Cannot find thumbnail file for {input_embedding}, use the full image instead.")
-                            input_embedding_thumbnail = input_embedding
-                        input_embedding = f"[![input embedding image for {model_name}]({input_embedding_thumbnail})]({input_embedding})"
-                    # Output Embedding
-                    if output_embedding is None or len(output_embedding) == 0:
-                        output_embedding = " "
-                    else:
-                        output_embedding_thumbnail = find_thumbnail_file(output_embedding)
-                        if output_embedding_thumbnail is None:
-                            print(f"Cannot find thumbnail file for {output_embedding}, use the full image instead.")
-                            output_embedding_thumbnail = output_embedding
-                        output_embedding = f"[![output embedding image for {model_name}]({output_embedding_thumbnail})]({output_embedding})"
-                    f.write(f"| {model_name} | {coverage} | {input_embedding} | {output_embedding} |\n")
-                # print(f"* {model_name}")
-                # print("\n")
-            f.write("\n\n")
-
-
 def generate_coverage(models:List[dict], charsets:dict, group:str='', folder=DEFAULT_IMAGE_FOLDER, debug:bool=False):
     for section in models:
         if group != '' and section['group'] != group:
             if debug:
-                print(f"Skip group {section['group']}")
+                logger.debug(f"Skip group {section['group']}")
             continue
         for model_name in section["models"]:
             try:
                 coverage = find_coverage_file(model_name)
                 if coverage is not None:
                     # fix coverage filename
                     standard_coverage = get_standard_coverage_filename(model_name)
                     if standard_coverage != coverage:
-                        print(f"Renaming {coverage} => {standard_coverage}")
+                        logger.info(f"Renaming {coverage} => {standard_coverage}")
                         os.rename(coverage, standard_coverage)
                         coverage = standard_coverage
                     if debug:
-                        print(f"Nothing to generate for {model_name} coverage. ({coverage}).")
+                        logger.debug(f"Nothing to generate for {model_name} coverage. ({coverage}).")
                     continue
                 # generate coverage
                 coverage_analysis(model_name, charsets, folder, debug)
-                print(f"Generated coverage for {model_name}")
+                logger.info(f"Generated coverage for {model_name}")
             except Exception as e:
-                print(f"Error in {model_name}")
+                logger.error(f"Error in {model_name}")
                 traceback.print_exc()
 
 def generate_embedding(models:List[dict], charsets:dict, group:str='', folder=DEFAULT_IMAGE_FOLDER, debug:bool=False):
     for section in models:
         if group != '' and section['group'] != group:
             if debug:
-                print(f"Skip group {section['group']}")
+                logger.debug(f"Skip group {section['group']}")
             continue
         for model_name in section["models"]:
             try:
                 embedding_types = []
                 # Input Embedding
                 input_embedding = find_embedding_file(model_name, "input")
                 if input_embedding is None and (not 'openai' in model_name.lower()):
                     embedding_types.append("input")
                 # fix the embedding filename
                 standard_input_embedding = get_standard_embedding_filename(model_name, "input")
                 if input_embedding is not None and input_embedding != standard_input_embedding:
-                    print(f"Renaming {input_embedding} => {standard_input_embedding}")
+                    logger.info(f"Renaming {input_embedding} => {standard_input_embedding}")
                     os.rename(input_embedding, standard_input_embedding)
                     input_embedding = standard_input_embedding
                 # Output Embedding
                 output_embedding = find_embedding_file(model_name, "output")
                 if output_embedding is None:
                     embedding_types.append("output")
                 # fix the embedding filename
                 standard_output_embedding = get_standard_embedding_filename(model_name, "output")
                 if output_embedding is not None and output_embedding != standard_output_embedding:
-                    print(f"Renaming {output_embedding} => {standard_output_embedding}")
+                    logger.info(f"Renaming {output_embedding} => {standard_output_embedding}")
                     os.rename(output_embedding, standard_output_embedding)
                     output_embedding = standard_output_embedding
                 # check if we need to generate embedding
                 if len(embedding_types) == 0:
                     if debug:
-                        print(f"Nothing to generate for {model_name} embedding. ({input_embedding}, {output_embedding}))")
+                        logger.debug(f"Nothing to generate for {model_name} embedding. ({input_embedding}, {output_embedding}))")
                     continue
                 # check special case for OpenAI
-                if "openai" not in model_name.lower() or "/text-embedding-ada-002" not in model_name.lower():
+                if "openai" in model_name.lower() and "text-embedding-ada-002" not in model_name.lower():
                     if debug:
-                        print(f"Do not support embedding analysis for {model_name}")
+                        logger.debug(f"Do not support embedding analysis for {model_name}")
                     continue
                 if 'openai' in model_name.lower():
-                    print(f'embedding_types: {embedding_types}')
+                    logger.info(f'embedding_types: {embedding_types}')
                 # generate embedding
                 embedding_analysis(model_name=model_name,
                                 charsets=charsets,
                                 output_dir=folder,
                                 embedding_type=embedding_types,
+                                clear_cache=True,
                                 debug=debug)
-                print(f"Generated embedding for {model_name}")
+                logger.info(f"Generated embedding for {model_name}")
             except Exception as e:
-                print(f"Error in {model_name}")
+                logger.error(f"Error in {model_name}")
                 traceback.print_exc()
 
 def generate_thumbnail(filename:str, folder=DEFAULT_IMAGE_FOLDER, debug:bool=False):
     if filename is None or len(filename) == 0 or not os.path.exists(filename):
-        print(f"Cannot find file {filename}")
+        logger.error(f"Cannot find file {filename}")
         return
     thumbnail_filename = get_thumbnail_filename(filename, folder=folder)
     if not os.path.exists(thumbnail_filename):
         basedir = os.path.dirname(thumbnail_filename)
         if not os.path.exists(basedir):
             os.makedirs(basedir, exist_ok=True)
-        print(f"Creating thumbnail for {filename}")
-        ret = os.system(f"convert {filename} -quality 20 -resize 30% {thumbnail_filename}")
+        logger.info(f"Creating thumbnail for {filename}")
+        ret = os.system(f"convert {filename} -quality 50 -resize 20% {thumbnail_filename}")
         if ret != 0:
-            print(f"Failed to create thumbnail for {filename}")
-            exit(1)
+            logger.error(f"Failed to create thumbnail for {filename}")
+            raise Exception(f"Failed to create thumbnail for {filename}")
 
 def generate_embedding_thumbnails(models:List[dict], folder=DEFAULT_IMAGE_FOLDER, debug:bool=False):
     for section in models:
         for model_name in section["models"]:
             try:
                 input_embedding = find_embedding_file(model_name, "input", folder=folder)
                 if input_embedding is not None:
                     generate_thumbnail(input_embedding, folder=folder, debug=debug)
                 output_embedding = find_embedding_file(model_name, "output", folder=folder)
                 if output_embedding is not None:
                     generate_thumbnail(output_embedding, folder=folder, debug=debug)
             except Exception as e:
-                print(f"Error in {model_name}")
+                logger.error(f"Error in {model_name}")
                 traceback.print_exc()
 
-def main():
-    models = load_model_list()
+def generate_coverage_thumbnails(models:List[dict], folder=DEFAULT_IMAGE_FOLDER, debug:bool=False):
+    for section in models:
+        for model_name in section["models"]:
+            try:
+                coverage = find_coverage_file(model_name, folder=folder)
+                if coverage is not None:
+                    generate_thumbnail(coverage, folder=folder, debug=debug)
+            except Exception as e:
+                logger.error(f"Error in {model_name}")
+                traceback.print_exc()
+
+def get_oss_url(image) -> str:
+    # base_url = "https://lab99-syd-pub.oss-accelerate.aliyuncs.com/vocab-coverage/"
+    # base_url = "https://lab99-syd-pub.oss-ap-southeast-2.aliyuncs.com/vocab-coverage/"
+    base_url = "http://syd.jiefu.org/vocab-coverage/"
+    if image.startswith("images/assets/"):
+        image = image.replace("images/assets/", "")
+    elif image.startswith("images/"):
+        image = image.replace("images/", "")
+    return base_url + image
+
+def generate_markdown_for_model_graph(image_file) -> str:
+    content = " "
+    if image_file is None or len(image_file) == 0:
+        content = " "
+    else:
+        thumbnail_file = find_thumbnail_file(image_file)
+        if thumbnail_file is None:
+            logger.warning(f"Cannot find thumbnail file for {image_file}, use the full size instead.")
+            thumbnail_file = image_file
+        # use OSS for image
+        image_file = get_oss_url(image_file)
+        thumbnail_file = get_oss_url(thumbnail_file)
+        content = f"[![]({thumbnail_file})]({image_file})"
+    return content
+
+def generate_markdown_for_model(model_name:str) -> str:
+    coverage = find_coverage_file(model_name)
+    if coverage is None:
+        logger.warning(f"Cannot find coverage file for {model_name}")
+    input_embedding = find_embedding_file(model_name, "input")
+    if input_embedding is None and not 'openai' in model_name.lower():
+        logger.warning(f"Cannot find input embedding file for {model_name}")
+    output_embedding = find_embedding_file(model_name, "output")
+    if output_embedding is None and not 'openai' in model_name.lower():
+        logger.warning(f"Cannot find output embedding file for {model_name}")
+    if coverage is None and input_embedding is None and output_embedding is None:
+        logger.error(f"Cannot find any file for {model_name}")
+        return ""
+    else:
+        # Name
+        # model_name = f'<b style="display: inline-block; transform: rotate(-90deg);">{model_name}</b>'
+        if "/" in model_name:
+            org, name = model_name.split("/")
+            model_name = f'<p>{org}</p><p>/</p><p>{name}</p>'
+        model_name = f'<b>{model_name}</b>'
+        coverage = generate_markdown_for_model_graph(coverage)
+        input_embedding = generate_markdown_for_model_graph(input_embedding)
+        output_embedding = generate_markdown_for_model_graph(output_embedding)
+        return f"| {model_name} | {coverage} | {input_embedding} | {output_embedding} |\n"
+
+def generate_markdown_for_models(models:List[str]) -> str:
+    content = ""
+    with io.StringIO() as f:
+        f.write("| 名称| 汉字覆盖率分析 | 输入词向量分布 | 输出词向量分布 |\n")
+        f.write("| :---: | :---: | :---: | :---: |\n")
+        # Table body
+        for model_name in models:
+            f.write(generate_markdown_for_model(model_name))
+        content = f.getvalue()
+    return content
+
+def generate_markdown_for_all(models:List[dict], output:str="graphs.md", section_level:int=2):
+    with open(output, "w") as f:
+        section_mark = "#" * section_level
+        for section in models:
+            f.write(f"{section_mark} {section['name']}\n\n")
+            f.write(generate_markdown_for_models(section["models"]))
+            f.write("\n\n")
+
+def generate_markdown_from_template(template_file:str, model_list_file:str, output:str="README.md"):
+    with open(template_file, "r") as f:
+        template = f.read()
+    with open(model_list_file, "r") as f:
+        models = yaml.load(f, Loader=yaml.FullLoader)
+    for tag, section in models.items():
+        content = generate_markdown_for_models(section["models"])
+        if len(content) > 0:
+            template = template.replace(f"{{{tag}}}", content)
+    with open(output, "w") as f:
+        f.write(template)
 
+def main():
     parser = argparse.ArgumentParser()
     subcommands = parser.add_subparsers(dest='command')
 
     cmdCoverage = subcommands.add_parser('coverage', help='Generate coverage graphs')
     cmdCoverage.add_argument("--group", type=str, default="", help="要生成的模型组（默认为全部），组名称见 models.json 中的 key")
     cmdCoverage.add_argument("--charset_file", type=str, default="", help="用以统计识字率的字表文件（默认为使用内置字符集文件）")
     cmdCoverage.add_argument("--debug", action="store_true", help="是否输出调试信息")
@@ -277,37 +301,41 @@
 
     cmdMarkdown = subcommands.add_parser('markdown', help='Generate markdown file for graphs')
     cmdMarkdown.add_argument("--charset_file", type=str, default="", help="用以统计识字率的字表文件（默认为使用内置字符集文件）")
     cmdMarkdown.add_argument("--markdown", type=str, default="graphs.md")
 
     args = parser.parse_args()
 
+    if hasattr(args, "debug") and args.debug:
+        logger.setLevel(logging.DEBUG)
+
     if hasattr(args, "charset_file") and len(args.charset_file) == 0:
         # 使用内置字符集文件
         args.charset_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'charsets.json')
 
+    models_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'models.yaml')
+    with open(models_file, "r") as f:
+        models = yaml.load(f, Loader=yaml.FullLoader)
+
     if args.command == "coverage":
         charsets = json.load(open(args.charset_file, 'r'))
         generate_coverage(models, charsets, group=args.group, folder=args.folder, debug=args.debug)
     elif args.command == "embedding":
         charsets = json.load(open(args.charset_file, 'r'))
         generate_embedding(models, charsets, group=args.group, folder=args.folder, debug=args.debug)
     elif args.command == "thumbnails":
+        generate_coverage_thumbnails(models, folder=args.folder, debug=args.debug)
         generate_embedding_thumbnails(models, folder=args.folder, debug=args.debug)
     elif args.command == "markdown":
-        generate_markdown(models, output=args.markdown)
-        # for models in readme
-        models_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'models_readme.json')
-        models = load_model_list(models_file)
-        generate_markdown(models, output='README.models.md', section_level=3)
-        if os.path.exists('README.md.template'):
-            print("Generating README.md")
-            content = open('README.md.template', 'r').read()
-            models_content = open('README.models.md', 'r').read()
-            content = content.replace('{MODEL_LIST}', models_content)
-            open('README.md', 'w').write(content)
-            print("生成后，请在 VSCode 中打开保存一下 `README.md` 文件，触发目录的更新。")
+        # markdown for all models
+        logger.info(f"Generating markdown for all models to {args.markdown}")
+        generate_markdown_for_all(models, output=args.markdown)
+        # markdown for readme
+        template_file = os.path.join('docs', 'README.template.md')
+        models_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'models_readme.yaml')
+        logger.info(f"Generating markdown for readme by {template_file} and {models_file}")
+        generate_markdown_from_template(template_file=template_file, model_list_file=models_file, output='README.md')
     else:
         parser.print_help()
 
 if __name__ == "__main__":
     main()
```

### Comparing `vocab-coverage-0.6/vocab_coverage/main.py` & `vocab-coverage-0.7/vocab_coverage/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,61 @@
+# -*- coding: utf-8 -*-
+
+import logging
 import os
 import sys
 import argparse
 import json
 from dotenv import load_dotenv
 
 if __name__ == "__main__":
     sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 from vocab_coverage import coverage_analysis, embedding_analysis
+from vocab_coverage.utils import logger
 
 def main():
     parser = argparse.ArgumentParser()
 
     subcommands = parser.add_subparsers(dest='command')
 
     cmdCoverage = subcommands.add_parser('coverage', help='模型汉字识字率分析')
     cmdCoverage.add_argument("--model_name", type=str, default="shibing624/text2vec-base-chinese", help="模型在 HuggingFace Hub 上的名称（默认为 shibing624/text2vec-base-chinese）")
     cmdCoverage.add_argument("--charset_file", type=str, default="", help="用以统计识字率的字表文件（默认为内置字符集文件）")
-    cmdCoverage.add_argument("--output_dir", type=str, default="images", help="生成的图像文件的输出目录（默认为 images）")
+    cmdCoverage.add_argument("--output_dir", type=str, default="images", help="生成的图像文件的输出目录（默认为 images/assets）")
     cmdCoverage.add_argument("--debug", action='store_true', help="是否打印调试信息")
 
     cmdEmbedding = subcommands.add_parser('embedding', help='词向量可视化分析')
     cmdEmbedding.add_argument("--model_name", type=str, default="shibing624/text2vec-base-chinese", help="模型在 HuggingFace Hub 上的名称（默认为 shibing624/text2vec-base-chinese）")
     cmdEmbedding.add_argument("--charset_file", type=str, default="", help="用以统计识字率的字表文件（默认为内置字符集文件）")
-    cmdEmbedding.add_argument("--output_dir", type=str, default="images", help="生成的图像文件的输出目录（默认为 images）")
+    cmdEmbedding.add_argument("--output_dir", type=str, default="images", help="生成的图像文件的输出目录（默认为 images/assets）")
+    cmdEmbedding.add_argument("--postfix", type=str, default=None, help="图像文件名可选后缀，用以控制生成的文件名")
+    cmdEmbedding.add_argument("--flat", action='store_true', help="控制是否将图像文件直接输出到 output_dir 目录下（默认为 False）") 
+    cmdEmbedding.add_argument("--override", action='store_true', help="是否覆盖已存在的图像文件（默认为 False）")
     cmdEmbedding.add_argument("--is_detailed", action='store_true', help="是否对汉字进行详细分类（默认为 False）")
     cmdEmbedding.add_argument("--debug", action='store_true', help="是否打印调试信息（默认为 False）")
     cmdEmbedding.add_argument("--skip_input_embeddings", action='store_true', help="不计算输入层的词向量")
     cmdEmbedding.add_argument("--output_embeddings", action='store_true', help="计算输出层的词向量")
-
+    cmdEmbedding.add_argument("--reducer_method", type=str, default="tsne", help="降维算法（默认为 tsne），可选值为 tsne, umap, tsne_cuml, umap_cuml, umap_tsne, umap_tsne_cuml")
     cmdCharset = subcommands.add_parser('charset', help='生成用以统计识字率的字表文件')
     cmdCharset.add_argument("--charset_file", type=str, default="", help="用以统计识字率的字表文件（默认为内置字符集文件）")
 
     args = parser.parse_args()
 
+    # if hasattr(args, "debug") and args.debug:
+    #     logger.setLevel(logging.DEBUG)
+
     if len(args.charset_file) == 0:
         # 使用内置字符集文件
         charset_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'charsets.json')
 
     if args.command == 'charsets':
         from vocab_coverage import generate_charsets
         if len(args.charset_file) == 0:
-            print(f'请指定 --charset_file 参数')
+            logger.error(f'请指定 --charset_file 参数')
             exit(1)
         generate_charsets(args.charset_file)
         return
     elif args.command == 'coverage':
         charsets = json.load(open(charset_file, 'r'))
         coverage_analysis(args.model_name, charsets, args.output_dir, args.debug)
         return
@@ -56,16 +66,20 @@
             etypes.append('input')
         if args.output_embeddings:
             etypes.append('output')
         embedding_analysis(
             model_name=args.model_name,
             charsets=charsets,
             output_dir=args.output_dir,
+            postfix=args.postfix,
+            flat=args.flat,
+            override=args.override,
             embedding_type=etypes,
             is_detailed=args.is_detailed,
+            reducer_method=args.reducer_method,
             debug=args.debug)
     else:
         parser.print_help()
         return
 
 if __name__ == "__main__":
     load_dotenv()
```

### Comparing `vocab-coverage-0.6/vocab_coverage.egg-info/SOURCES.txt` & `vocab-coverage-0.7/vocab_coverage.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 vocab_coverage/__init__.py
 vocab_coverage/charsets.json
 vocab_coverage/charsets.py
 vocab_coverage/coverage.py
 vocab_coverage/draw.py
 vocab_coverage/embedding.py
 vocab_coverage/generate.py
+vocab_coverage/loader.py
 vocab_coverage/main.py
-vocab_coverage/models.json
-vocab_coverage/models_readme.json
+vocab_coverage/reducer.py
+vocab_coverage/utils.py
 vocab_coverage.egg-info/PKG-INFO
 vocab_coverage.egg-info/SOURCES.txt
 vocab_coverage.egg-info/dependency_links.txt
 vocab_coverage.egg-info/entry_points.txt
 vocab_coverage.egg-info/requires.txt
 vocab_coverage.egg-info/top_level.txt
```

