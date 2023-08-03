# Comparing `tmp/nonebot_plugin_bawiki-0.8.2.tar.gz` & `tmp/nonebot_plugin_bawiki-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bawiki-0.8.2.tar", last modified: Fri Jul 21 07:53:24 2023, max compression
+gzip compressed data, was "nonebot_plugin_bawiki-0.8.3.tar", last modified: Thu Aug  3 11:01:01 2023, max compression
```

## Comparing `nonebot_plugin_bawiki-0.8.2.tar` & `nonebot_plugin_bawiki-0.8.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1068 2023-07-21 07:52:55.471583 nonebot_plugin_bawiki-0.8.2/LICENSE
--rw-r--r--   0        0        0     9655 2023-07-21 07:52:55.471583 nonebot_plugin_bawiki-0.8.2/README.md
--rw-r--r--   0        0        0      734 2023-07-21 07:52:55.471583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/__init__.py
--rw-r--r--   0        0        0      947 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/__init__.py
--rw-r--r--   0        0        0     3758 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/arona.py
--rw-r--r--   0        0        0     2330 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/calender.py
--rw-r--r--   0        0        0     1265 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/clear_cache.py
--rw-r--r--   0        0        0     1228 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/craft.py
--rw-r--r--   0        0        0     1013 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/emoji.py
--rw-r--r--   0        0        0     2600 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/event.py
--rw-r--r--   0        0        0      986 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/furniture.py
--rw-r--r--   0        0        0     6372 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/gacha.py
--rw-r--r--   0        0        0     3555 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/global_future.py
--rw-r--r--   0        0        0     1795 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/level_guide.py
--rw-r--r--   0        0        0     1438 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/manga.py
--rw-r--r--   0        0        0     4376 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/raid.py
--rw-r--r--   0        0        0     3617 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_fav.py
--rw-r--r--   0        0        0     1878 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_rank.py
--rw-r--r--   0        0        0     1635 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py
--rw-r--r--   0        0        0     2031 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_wiki_schale.py
--rw-r--r--   0        0        0     3395 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/time_atk.py
--rw-r--r--   0        0        0     4201 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/voice.py
--rw-r--r--   0        0        0     1152 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/config.py
--rw-r--r--   0        0        0        0 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/__init__.py
--rw-r--r--   0        0        0     1541 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/arona.py
--rw-r--r--   0        0        0     5814 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/bawiki.py
--rw-r--r--   0        0        0     7398 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/gacha.py
--rw-r--r--   0        0        0    11340 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/gamekee.py
--rw-r--r--   0        0        0    18840 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/schaledb.py
--rw-r--r--   0        0        0     1358 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/__init__.py
--rw-r--r--   0        0        0     1784 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/manual.py
--rw-r--r--   0        0        0     2226 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/pic_menu.py
--rw-r--r--   0        0        0      919 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/__init__.py
--rw-r--r--   0        0        0    21514 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/calender_banner.png
--rw-r--r--   0        0        0  1685142 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_bg.png
--rw-r--r--   0        0        0    13956 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png
--rw-r--r--   0        0        0     2408 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png
--rw-r--r--   0        0        0     4391 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_new.png
--rw-r--r--   0        0        0    10375 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_pickup.png
--rw-r--r--   0        0        0     2022 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_star.png
--rw-r--r--   0        0        0    14652 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png
--rw-r--r--   0        0        0  1764190 2023-07-21 07:52:55.483583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gradient.png
--rw-r--r--   0        0        0     4668 2023-07-21 07:52:55.483583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/util.py
--rw-r--r--   0        0        0     1481 2023-07-21 07:53:24.712021 nonebot_plugin_bawiki-0.8.2/pyproject.toml
--rw-r--r--   0        0        0    11106 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/LICENSE
+-rw-r--r--   0        0        0     9687 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/README.md
+-rw-r--r--   0        0        0      734 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/__init__.py
+-rw-r--r--   0        0        0      947 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/__init__.py
+-rw-r--r--   0        0        0     3758 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/arona.py
+-rw-r--r--   0        0        0     2330 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/calender.py
+-rw-r--r--   0        0        0     1265 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/clear_cache.py
+-rw-r--r--   0        0        0     1228 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/craft.py
+-rw-r--r--   0        0        0     1013 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/emoji.py
+-rw-r--r--   0        0        0     2600 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/event.py
+-rw-r--r--   0        0        0      986 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/furniture.py
+-rw-r--r--   0        0        0     6372 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/gacha.py
+-rw-r--r--   0        0        0     3555 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/global_future.py
+-rw-r--r--   0        0        0     1795 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/level_guide.py
+-rw-r--r--   0        0        0     1438 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/manga.py
+-rw-r--r--   0        0        0     4376 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/raid.py
+-rw-r--r--   0        0        0     3617 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_fav.py
+-rw-r--r--   0        0        0     1878 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_rank.py
+-rw-r--r--   0        0        0     1635 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py
+-rw-r--r--   0        0        0     2031 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_wiki_schale.py
+-rw-r--r--   0        0        0     3395 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/time_atk.py
+-rw-r--r--   0        0        0     4201 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/voice.py
+-rw-r--r--   0        0        0     1152 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/config.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/__init__.py
+-rw-r--r--   0        0        0     1541 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/arona.py
+-rw-r--r--   0        0        0     5814 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/bawiki.py
+-rw-r--r--   0        0        0     7398 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/gacha.py
+-rw-r--r--   0        0        0    11340 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/gamekee.py
+-rw-r--r--   0        0        0    18840 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/schaledb.py
+-rw-r--r--   0        0        0     1358 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/__init__.py
+-rw-r--r--   0        0        0     1784 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/manual.py
+-rw-r--r--   0        0        0     2226 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/pic_menu.py
+-rw-r--r--   0        0        0     1251 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/__init__.py
+-rw-r--r--   0        0        0    21514 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/calender_banner.png
+-rw-r--r--   0        0        0  1685142 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_bg.png
+-rw-r--r--   0        0        0    13956 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png
+-rw-r--r--   0        0        0     2408 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png
+-rw-r--r--   0        0        0     4391 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_new.png
+-rw-r--r--   0        0        0    10375 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_pickup.png
+-rw-r--r--   0        0        0     2022 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_star.png
+-rw-r--r--   0        0        0    14652 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png
+-rw-r--r--   0        0        0  1764190 2023-08-03 11:00:38.576594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gradient.png
+-rw-r--r--   0        0        0     4668 2023-08-03 11:00:38.576594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/util.py
+-rw-r--r--   0        0        0     1481 2023-08-03 11:01:01.006585 nonebot_plugin_bawiki-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0    11138 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.8.3/PKG-INFO
```

### Comparing `nonebot_plugin_bawiki-0.8.2/LICENSE` & `nonebot_plugin_bawiki-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/README.md` & `nonebot_plugin_bawiki-0.8.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+## 0.8.3
+
+- 修改缓存路径
+
 ### 0.8.2
 
 - 修改了 `ba语音` 指令的特性，兼容了有中配语音的学生，请查看该指令帮助获取详细信息
 - 删除了 `arona` 指令模糊搜索展示类别的功能，因为模糊搜索时 `type` 固定为 `0` 了
 
 ### 0.8.1
```

#### html2text {}

```diff
@@ -51,16 +51,16 @@
 126.com> ## ð¡ é¸£è°¢ ### [GameKee](https://ba.gamekee.com/) & [SchaleDB]
 (https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
 doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
-lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.8.2 - ä¿®æ¹äº `baè¯­é³`
+lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ##
+0.8.3 - ä¿®æ¹ç¼å­è·¯å¾ ### 0.8.2 - ä¿®æ¹äº `baè¯­é³`
 æä»¤çç¹æ§ï¼å¼å®¹äºæä¸­éè¯­é³çå­¦çï¼è¯·æ¥çè¯¥æä»¤å¸®å©è·åè¯¦ç»ä¿¡æ¯
 - å é¤äº `arona`
 æä»¤æ¨¡ç³æç´¢å±ç¤ºç±»å«çåè½ï¼å ä¸ºæ¨¡ç³æç´¢æ¶ `type`
 åºå®ä¸º `0` äº ### 0.8.1 - ä½¿ç¨ `arona`
 æä»¤æ¨¡ç³æç´¢çæ¶åä¼æ¾ç¤ºå¾çç±»å«äº ### 0.8.0 -
 æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona Bot
 æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
```

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/__init__.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 
 from .command import load_commands  # noqa: E402
 from .config import Cfg as Cfg  # noqa: E402
 from .help import extra, register_help_cmd, usage  # noqa: E402
 
-__version__ = "0.8.2"
+__version__ = "0.8.3"
 __plugin_meta__ = PluginMetadata(
     name="BAWiki",
     description="碧蓝档案Wiki插件",
     usage=usage,
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-bawiki",
     type="application",
     config=Cfg,
```

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/__init__.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/arona.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/arona.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/calender.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/calender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/clear_cache.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/clear_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/craft.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/craft.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/emoji.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/emoji.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/event.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/furniture.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/furniture.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/gacha.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/gacha.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/global_future.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/global_future.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/level_guide.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/level_guide.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/manga.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/manga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/raid.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/raid.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_fav.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_fav.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_rank.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_wiki_schale.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_wiki_schale.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/time_atk.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/time_atk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/voice.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/voice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/config.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/arona.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/arona.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/bawiki.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/bawiki.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/gacha.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/gacha.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/gamekee.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/gamekee.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/schaledb.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/schaledb.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/__init__.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/manual.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/manual.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/pic_menu.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/pic_menu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/calender_banner.png` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/calender_banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_bg.png` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_new.png` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_new.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_pickup.png` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_pickup.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_star.png` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_star.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gradient.png` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gradient.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/util.py` & `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.2/pyproject.toml` & `nonebot_plugin_bawiki-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bawiki"
-version = "0.8.2"
+version = "0.8.3"
 description = "A nonebot2 plugin for Blue Archive."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.1",
```

### Comparing `nonebot_plugin_bawiki-0.8.2/PKG-INFO` & `nonebot_plugin_bawiki-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bawiki
-Version: 0.8.2
+Version: 0.8.3
 Summary: A nonebot2 plugin for Blue Archive.
 Keywords: blue archive nonebot nonebot2 bot qq
 Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications
@@ -206,14 +206,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+## 0.8.3
+
+- 修改缓存路径
+
 ### 0.8.2
 
 - 修改了 `ba语音` 指令的特性，兼容了有中配语音的学生，请查看该指令帮助获取详细信息
 - 删除了 `arona` 指令模糊搜索展示类别的功能，因为模糊搜索时 `type` 固定为 `0` 了
 
 ### 0.8.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.8.2 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.8.3 Summary: A
 nonebot2 plugin for Blue Archive. Keywords: blue archive nonebot nonebot2 bot
 qq Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/ Author-Email:
 student_2333
 126.com> License: MIT Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Chat :: ICQ Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Board Games
@@ -71,16 +71,16 @@
 126.com> ## ð¡ é¸£è°¢ ### [GameKee](https://ba.gamekee.com/) & [SchaleDB]
 (https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
 doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
-lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.8.2 - ä¿®æ¹äº `baè¯­é³`
+lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ##
+0.8.3 - ä¿®æ¹ç¼å­è·¯å¾ ### 0.8.2 - ä¿®æ¹äº `baè¯­é³`
 æä»¤çç¹æ§ï¼å¼å®¹äºæä¸­éè¯­é³çå­¦çï¼è¯·æ¥çè¯¥æä»¤å¸®å©è·åè¯¦ç»ä¿¡æ¯
 - å é¤äº `arona`
 æä»¤æ¨¡ç³æç´¢å±ç¤ºç±»å«çåè½ï¼å ä¸ºæ¨¡ç³æç´¢æ¶ `type`
 åºå®ä¸º `0` äº ### 0.8.1 - ä½¿ç¨ `arona`
 æä»¤æ¨¡ç³æç´¢çæ¶åä¼æ¾ç¤ºå¾çç±»å«äº ### 0.8.0 -
 æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona Bot
 æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
```

