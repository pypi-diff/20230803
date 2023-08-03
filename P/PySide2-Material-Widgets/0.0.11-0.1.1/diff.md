# Comparing `tmp/PySide2-Material-Widgets-0.0.11.tar.gz` & `tmp/PySide2-Material-Widgets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide2-Material-Widgets-0.0.11.tar", last modified: Wed Jul 26 04:50:53 2023, max compression
+gzip compressed data, was "dist\PySide2-Material-Widgets-0.1.1.tar", last modified: Thu Aug  3 03:13:36 2023, max compression
```

## Comparing `PySide2-Material-Widgets-0.0.11.tar` & `PySide2-Material-Widgets-0.1.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.363751 PySide2-Material-Widgets-0.0.11/
--rw-rw-rw-   0        0        0    35823 2023-07-24 00:28:48.000000 PySide2-Material-Widgets-0.0.11/LICENSE
--rw-rw-rw-   0        0        0     4405 2023-07-26 04:50:53.362333 PySide2-Material-Widgets-0.0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.160305 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4405 2023-07-26 04:50:52.000000 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3899 2023-07-26 04:50:53.000000 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 04:50:52.000000 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-26 04:50:53.000000 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 04:50:53.000000 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3601 2023-07-26 04:49:23.000000 PySide2-Material-Widgets-0.0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.162789 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/
--rw-rw-rw-   0        0        0      710 2023-07-26 04:50:02.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.167342 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  5933542 2023-07-26 03:47:15.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.210538 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/
--rw-rw-rw-   0        0        0      552 2023-07-22 14:31:29.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     7944 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/animation.py
--rw-rw-rw-   0        0        0     3657 2023-06-26 15:48:09.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0     1189 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/color.py
--rw-rw-rw-   0        0        0    10647 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0     1306 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/font.py
--rw-rw-rw-   0        0        0    12716 2023-07-26 03:51:09.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/icon.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.212625 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.217533 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/blend/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/blend/__init__.py
--rw-rw-rw-   0        0        0     4816 2023-07-17 01:35:35.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/blend/blend.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.228572 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/__init__.py
--rw-rw-rw-   0        0        0    11533 2023-07-17 01:35:19.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/cam16.py
--rw-rw-rw-   0        0        0     8397 2023-07-17 01:35:26.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/hct.py
--rw-rw-rw-   0        0        0     5391 2023-07-17 01:35:30.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/viewing_conditions.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.236201 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/__init__.py
--rw-rw-rw-   0        0        0     1576 2023-07-17 01:35:03.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/core_palette.py
--rw-rw-rw-   0        0        0     1985 2023-07-17 01:35:12.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/tonal_palette.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.254774 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/__init__.py
--rw-rw-rw-   0        0        0     1929 2023-07-17 01:34:35.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py
--rw-rw-rw-   0        0        0     2158 2023-07-17 01:34:38.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py
--rw-rw-rw-   0        0        0     1723 2023-07-17 01:34:42.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_map.py
--rw-rw-rw-   0        0        0     8297 2023-07-17 01:34:46.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py
--rw-rw-rw-   0        0        0    14347 2023-07-17 01:34:55.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.260477 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/scheme/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/scheme/__init__.py
--rw-rw-rw-   0        0        0     7792 2023-07-21 13:40:47.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/scheme/scheme.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.265841 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/score/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/score/__init__.py
--rw-rw-rw-   0        0        0     6017 2023-07-17 01:34:16.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/score/score.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.282364 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/__init__.py
--rw-rw-rw-   0        0        0     7656 2023-07-17 01:33:35.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/color_utils.py
--rw-rw-rw-   0        0        0     2850 2023-07-17 01:35:47.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/image_utils.py
--rw-rw-rw-   0        0        0     2854 2023-07-16 13:31:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/math_utils.py
--rw-rw-rw-   0        0        0     2325 2023-07-17 01:33:56.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/string_utils.py
--rw-rw-rw-   0        0        0     3857 2023-07-17 01:34:05.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/theme_utils.py
--rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3862 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/router.py
--rw-rw-rw-   0        0        0     4874 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0    12748 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      460 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.284371 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/
--rw-rw-rw-   0        0        0       72 2023-07-26 04:29:03.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.292140 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0       35 2023-07-22 09:35:54.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0     3194 2023-07-26 04:17:47.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     4660 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/message_box.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.300077 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/
--rw-rw-rw-   0        0        0       76 2023-07-18 06:23:37.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2658 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5437 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/flow_layout.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.359671 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/
--rw-rw-rw-   0        0        0     2050 2023-07-26 04:33:30.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0    16812 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     4932 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     2437 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0     5717 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/floating_action_button.py
--rw-rw-rw-   0        0        0    16139 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2049 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1355 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    16646 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    21236 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0     9136 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    35532 2023-07-26 03:51:47.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0      711 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/overlay_widget.py
--rw-rw-rw-   0        0        0     8210 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     5562 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     1346 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/radio_button.py
--rw-rw-rw-   0        0        0     5707 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/ripple.py
--rw-rw-rw-   0        0        0     2598 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    18195 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     6356 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0    10489 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0    22383 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10242 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0       42 2023-07-26 04:50:53.363751 PySide2-Material-Widgets-0.0.11/setup.cfg
--rw-rw-rw-   0        0        0     1170 2023-07-26 04:50:09.000000 PySide2-Material-Widgets-0.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.768362 PySide2-Material-Widgets-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-24 00:28:48.000000 PySide2-Material-Widgets-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4523 2023-08-03 03:13:36.768362 PySide2-Material-Widgets-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.598602 PySide2-Material-Widgets-0.1.1/PySide2_Material_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4523 2023-08-03 03:13:36.000000 PySide2-Material-Widgets-0.1.1/PySide2_Material_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3899 2023-08-03 03:13:36.000000 PySide2-Material-Widgets-0.1.1/PySide2_Material_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 03:13:36.000000 PySide2-Material-Widgets-0.1.1/PySide2_Material_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-08-03 03:13:36.000000 PySide2-Material-Widgets-0.1.1/PySide2_Material_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-03 03:13:36.000000 PySide2-Material-Widgets-0.1.1/PySide2_Material_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3720 2023-08-03 03:11:07.000000 PySide2-Material-Widgets-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.601128 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/
+-rw-rw-rw-   0        0        0      709 2023-08-03 03:11:56.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.605189 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  2185694 2023-08-03 03:12:18.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.639076 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/
+-rw-rw-rw-   0        0        0      537 2023-08-03 03:12:47.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     7944 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     3657 2023-06-26 15:48:09.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0     1189 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/color.py
+-rw-rw-rw-   0        0        0    10647 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      866 2023-08-03 03:11:18.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/font.py
+-rw-rw-rw-   0        0        0    12716 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/icon.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.641083 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.645554 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/blend/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/blend/__init__.py
+-rw-rw-rw-   0        0        0     4816 2023-07-17 01:35:35.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/blend/blend.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.653577 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/__init__.py
+-rw-rw-rw-   0        0        0    11533 2023-07-17 01:35:19.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/cam16.py
+-rw-rw-rw-   0        0        0     8397 2023-07-17 01:35:26.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/hct.py
+-rw-rw-rw-   0        0        0     5391 2023-07-17 01:35:30.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/viewing_conditions.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.660938 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/__init__.py
+-rw-rw-rw-   0        0        0     1576 2023-07-17 01:35:03.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/core_palette.py
+-rw-rw-rw-   0        0        0     1985 2023-07-17 01:35:12.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/tonal_palette.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.676185 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/__init__.py
+-rw-rw-rw-   0        0        0     1929 2023-07-17 01:34:35.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py
+-rw-rw-rw-   0        0        0     2158 2023-07-17 01:34:38.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py
+-rw-rw-rw-   0        0        0     1723 2023-07-17 01:34:42.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_map.py
+-rw-rw-rw-   0        0        0     8297 2023-07-17 01:34:46.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py
+-rw-rw-rw-   0        0        0    14347 2023-07-17 01:34:55.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.680615 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/scheme/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/scheme/__init__.py
+-rw-rw-rw-   0        0        0     7792 2023-07-21 13:40:47.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/scheme/scheme.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.683629 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/score/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/score/__init__.py
+-rw-rw-rw-   0        0        0     6017 2023-07-17 01:34:16.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/score/score.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.699038 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/__init__.py
+-rw-rw-rw-   0        0        0     7656 2023-07-17 01:33:35.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/color_utils.py
+-rw-rw-rw-   0        0        0     2850 2023-07-17 01:35:47.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/image_utils.py
+-rw-rw-rw-   0        0        0     2854 2023-07-16 13:31:20.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/math_utils.py
+-rw-rw-rw-   0        0        0     2325 2023-07-17 01:33:56.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/string_utils.py
+-rw-rw-rw-   0        0        0     3857 2023-07-17 01:34:05.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/theme_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3862 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/router.py
+-rw-rw-rw-   0        0        0     4874 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0    12748 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      460 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.701046 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/
+-rw-rw-rw-   0        0        0       72 2023-07-26 04:29:03.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.708438 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0       35 2023-07-22 09:35:54.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0     3194 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     4660 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/message_box.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.714813 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/
+-rw-rw-rw-   0        0        0       76 2023-07-18 06:23:37.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2658 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5437 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/flow_layout.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:13:36.765981 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     2225 2023-08-03 03:11:18.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0    19155 2023-08-03 03:11:59.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     4932 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     2437 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0     5717 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/floating_action_button.py
+-rw-rw-rw-   0        0        0    16139 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2049 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1355 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    16646 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    21236 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0     9136 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    35532 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0      711 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/overlay_widget.py
+-rw-rw-rw-   0        0        0     8210 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     5562 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     1346 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/radio_button.py
+-rw-rw-rw-   0        0        0     5707 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/ripple.py
+-rw-rw-rw-   0        0        0     2598 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    18195 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     6356 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0    10489 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0    22383 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10242 2023-08-03 03:11:08.000000 PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 03:13:36.768362 PySide2-Material-Widgets-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1169 2023-08-03 03:11:46.000000 PySide2-Material-Widgets-0.1.1/setup.py
```

### Comparing `PySide2-Material-Widgets-0.0.11/LICENSE` & `PySide2-Material-Widgets-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/PKG-INFO` & `PySide2-Material-Widgets-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Material-Widgets
-Version: 0.0.11
+Version: 0.1.1
 Summary: A material design widgets library based on PySide2
 Home-page: https://github.com/zhiyiYo/QMaterialWidgets/tree/master
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qmaterialwidgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/QMaterialWidgets/tree/master
@@ -60,14 +60,16 @@
 The Community version only provides basic components, while the more advanced ones are available in the [Premium version](https://afdian.net/a/zhiyiYo?tab=shop).
 
 > **Warning**
 > Don't install PySide2-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
 
 
 ## Run Example
+You can download the executable demo from the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases).
+
 After installing PySide2-Material-Widgets package using pip, you can run the demo in examples directory, for example:
 ```python
 cd examples/button
 python demo.py
 ```
 
 If you encounter `ImportError: cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the imported components are only available in the Premium version.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide2-Material-Widgets Version: 0.0.11 Summary: A
+Metadata-Version: 2.1 Name: PySide2-Material-Widgets Version: 0.1.1 Summary: A
 material design widgets library based on PySide2 Home-page: https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 qmaterialwidgets.readthedocs.io/ Project-URL: Source Code, https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/QMaterialWidgets/issues Keywords: pyside2 material widgets
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
@@ -17,31 +17,33 @@
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/
 docs/source/_static/Interface.jpg) ## Install To install Community version:
 ```shell pip install PySide2-Material-Widgets -i https://pypi.org/simple/ ```
 The Community version only provides basic components, while the more advanced
 ones are available in the [Premium version](https://afdian.net/a/
 zhiyiYo?tab=shop). > **Warning** > Don't install PySide2-Material-Widgets and
 PySide2-Material-Widgets at the same time, because their package names are all
-`qmaterialwidgets`. ## Run Example After installing PySide2-Material-Widgets
-package using pip, you can run the demo in examples directory, for example:
-```python cd examples/button python demo.py ``` If you encounter `ImportError:
-cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the
-imported components are only available in the Premium version. ## Documentation
-Want to know more about PySide2-Material-Widgets? Please read the [help
-document](https://qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration
-Check out this [â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o)
-that shows off what PySide2-Material-Widgets are capable of ð ## Work with
-QtDesigner You can use PySide2-Material-Widgets in QtDesigner directly by
-running `python ./tools/designer.py`. If the operation is successful, you
-should be able to see the PySide2-Material-Widgets in the sidebar of
-QtDesigner. ## Support If this project helps you a lot and you want to support
-the development and maintenance of this project, feel free to sponsor me via
-[ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/
-zhiyiYo). Your support is highly appreciated ð¥° ## Reference * [**Figma/
-Material 3 Design Kit**: Provides an introduction to the material design
-system](https://www.figma.com/community/file/1035203688168086460/Material-3-
-Design-Kit) * [**Google/Material Design**: A website demonstrates the controls
-available in Material Design 3 System](https://m3.material.io/get-started) ##
-License PySide2-Material-Widgets adopts dual licenses. Non-commercial usage is
-licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on
-[ç±åçµ](https://afdian.net/a/zhiyiYo?tab=shop) to support the development
-of this project. Copyright Â© 2021 by zhiyiYo.
+`qmaterialwidgets`. ## Run Example You can download the executable demo from
+the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases). After
+installing PySide2-Material-Widgets package using pip, you can run the demo in
+examples directory, for example: ```python cd examples/button python demo.py
+``` If you encounter `ImportError: cannot import name 'XXX' from
+'qmaterialwidgets'`, it indicates that the imported components are only
+available in the Premium version. ## Documentation Want to know more about
+PySide2-Material-Widgets? Please read the [help document](https://
+qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration Check out this
+[â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off
+what PySide2-Material-Widgets are capable of ð ## Work with QtDesigner You
+can use PySide2-Material-Widgets in QtDesigner directly by running `python ./
+tools/designer.py`. If the operation is successful, you should be able to see
+the PySide2-Material-Widgets in the sidebar of QtDesigner. ## Support If this
+project helps you a lot and you want to support the development and maintenance
+of this project, feel free to sponsor me via [ç±åçµ](https://afdian.net/a/
+zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly
+appreciated ð¥° ## Reference * [**Figma/Material 3 Design Kit**: Provides an
+introduction to the material design system](https://www.figma.com/community/
+file/1035203688168086460/Material-3-Design-Kit) * [**Google/Material Design**:
+A website demonstrates the controls available in Material Design 3 System]
+(https://m3.material.io/get-started) ## License PySide2-Material-Widgets adopts
+dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For
+commercial purposes, please purchase on [ç±åçµ](https://afdian.net/a/
+zhiyiYo?tab=shop) to support the development of this project. Copyright Â© 2021
+by zhiyiYo.
```

### Comparing `PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/PKG-INFO` & `PySide2-Material-Widgets-0.1.1/PySide2_Material_Widgets.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Material-Widgets
-Version: 0.0.11
+Version: 0.1.1
 Summary: A material design widgets library based on PySide2
 Home-page: https://github.com/zhiyiYo/QMaterialWidgets/tree/master
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qmaterialwidgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/QMaterialWidgets/tree/master
@@ -60,14 +60,16 @@
 The Community version only provides basic components, while the more advanced ones are available in the [Premium version](https://afdian.net/a/zhiyiYo?tab=shop).
 
 > **Warning**
 > Don't install PySide2-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
 
 
 ## Run Example
+You can download the executable demo from the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases).
+
 After installing PySide2-Material-Widgets package using pip, you can run the demo in examples directory, for example:
 ```python
 cd examples/button
 python demo.py
 ```
 
 If you encounter `ImportError: cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the imported components are only available in the Premium version.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide2-Material-Widgets Version: 0.0.11 Summary: A
+Metadata-Version: 2.1 Name: PySide2-Material-Widgets Version: 0.1.1 Summary: A
 material design widgets library based on PySide2 Home-page: https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 qmaterialwidgets.readthedocs.io/ Project-URL: Source Code, https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/QMaterialWidgets/issues Keywords: pyside2 material widgets
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
@@ -17,31 +17,33 @@
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/
 docs/source/_static/Interface.jpg) ## Install To install Community version:
 ```shell pip install PySide2-Material-Widgets -i https://pypi.org/simple/ ```
 The Community version only provides basic components, while the more advanced
 ones are available in the [Premium version](https://afdian.net/a/
 zhiyiYo?tab=shop). > **Warning** > Don't install PySide2-Material-Widgets and
 PySide2-Material-Widgets at the same time, because their package names are all
-`qmaterialwidgets`. ## Run Example After installing PySide2-Material-Widgets
-package using pip, you can run the demo in examples directory, for example:
-```python cd examples/button python demo.py ``` If you encounter `ImportError:
-cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the
-imported components are only available in the Premium version. ## Documentation
-Want to know more about PySide2-Material-Widgets? Please read the [help
-document](https://qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration
-Check out this [â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o)
-that shows off what PySide2-Material-Widgets are capable of ð ## Work with
-QtDesigner You can use PySide2-Material-Widgets in QtDesigner directly by
-running `python ./tools/designer.py`. If the operation is successful, you
-should be able to see the PySide2-Material-Widgets in the sidebar of
-QtDesigner. ## Support If this project helps you a lot and you want to support
-the development and maintenance of this project, feel free to sponsor me via
-[ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/
-zhiyiYo). Your support is highly appreciated ð¥° ## Reference * [**Figma/
-Material 3 Design Kit**: Provides an introduction to the material design
-system](https://www.figma.com/community/file/1035203688168086460/Material-3-
-Design-Kit) * [**Google/Material Design**: A website demonstrates the controls
-available in Material Design 3 System](https://m3.material.io/get-started) ##
-License PySide2-Material-Widgets adopts dual licenses. Non-commercial usage is
-licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on
-[ç±åçµ](https://afdian.net/a/zhiyiYo?tab=shop) to support the development
-of this project. Copyright Â© 2021 by zhiyiYo.
+`qmaterialwidgets`. ## Run Example You can download the executable demo from
+the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases). After
+installing PySide2-Material-Widgets package using pip, you can run the demo in
+examples directory, for example: ```python cd examples/button python demo.py
+``` If you encounter `ImportError: cannot import name 'XXX' from
+'qmaterialwidgets'`, it indicates that the imported components are only
+available in the Premium version. ## Documentation Want to know more about
+PySide2-Material-Widgets? Please read the [help document](https://
+qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration Check out this
+[â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off
+what PySide2-Material-Widgets are capable of ð ## Work with QtDesigner You
+can use PySide2-Material-Widgets in QtDesigner directly by running `python ./
+tools/designer.py`. If the operation is successful, you should be able to see
+the PySide2-Material-Widgets in the sidebar of QtDesigner. ## Support If this
+project helps you a lot and you want to support the development and maintenance
+of this project, feel free to sponsor me via [ç±åçµ](https://afdian.net/a/
+zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly
+appreciated ð¥° ## Reference * [**Figma/Material 3 Design Kit**: Provides an
+introduction to the material design system](https://www.figma.com/community/
+file/1035203688168086460/Material-3-Design-Kit) * [**Google/Material Design**:
+A website demonstrates the controls available in Material Design 3 System]
+(https://m3.material.io/get-started) ## License PySide2-Material-Widgets adopts
+dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For
+commercial purposes, please purchase on [ç±åçµ](https://afdian.net/a/
+zhiyiYo?tab=shop) to support the development of this project. Copyright Â© 2021
+by zhiyiYo.
```

### Comparing `PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/SOURCES.txt` & `PySide2-Material-Widgets-0.1.1/PySide2_Material_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/README.md` & `PySide2-Material-Widgets-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 The Community version only provides basic components, while the more advanced ones are available in the [Premium version](https://afdian.net/a/zhiyiYo?tab=shop).
 
 > **Warning**
 > Don't install PySide2-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
 
 
 ## Run Example
+You can download the executable demo from the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases).
+
 After installing PySide2-Material-Widgets package using pip, you can run the demo in examples directory, for example:
 ```python
 cd examples/button
 python demo.py
 ```
 
 If you encounter `ImportError: cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the imported components are only available in the Premium version.
```

#### html2text {}

```diff
@@ -6,31 +6,33 @@
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/
 docs/source/_static/Interface.jpg) ## Install To install Community version:
 ```shell pip install PySide2-Material-Widgets -i https://pypi.org/simple/ ```
 The Community version only provides basic components, while the more advanced
 ones are available in the [Premium version](https://afdian.net/a/
 zhiyiYo?tab=shop). > **Warning** > Don't install PySide2-Material-Widgets and
 PySide2-Material-Widgets at the same time, because their package names are all
-`qmaterialwidgets`. ## Run Example After installing PySide2-Material-Widgets
-package using pip, you can run the demo in examples directory, for example:
-```python cd examples/button python demo.py ``` If you encounter `ImportError:
-cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the
-imported components are only available in the Premium version. ## Documentation
-Want to know more about PySide2-Material-Widgets? Please read the [help
-document](https://qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration
-Check out this [â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o)
-that shows off what PySide2-Material-Widgets are capable of ð ## Work with
-QtDesigner You can use PySide2-Material-Widgets in QtDesigner directly by
-running `python ./tools/designer.py`. If the operation is successful, you
-should be able to see the PySide2-Material-Widgets in the sidebar of
-QtDesigner. ## Support If this project helps you a lot and you want to support
-the development and maintenance of this project, feel free to sponsor me via
-[ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/
-zhiyiYo). Your support is highly appreciated ð¥° ## Reference * [**Figma/
-Material 3 Design Kit**: Provides an introduction to the material design
-system](https://www.figma.com/community/file/1035203688168086460/Material-3-
-Design-Kit) * [**Google/Material Design**: A website demonstrates the controls
-available in Material Design 3 System](https://m3.material.io/get-started) ##
-License PySide2-Material-Widgets adopts dual licenses. Non-commercial usage is
-licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on
-[ç±åçµ](https://afdian.net/a/zhiyiYo?tab=shop) to support the development
-of this project. Copyright Â© 2021 by zhiyiYo.
+`qmaterialwidgets`. ## Run Example You can download the executable demo from
+the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases). After
+installing PySide2-Material-Widgets package using pip, you can run the demo in
+examples directory, for example: ```python cd examples/button python demo.py
+``` If you encounter `ImportError: cannot import name 'XXX' from
+'qmaterialwidgets'`, it indicates that the imported components are only
+available in the Premium version. ## Documentation Want to know more about
+PySide2-Material-Widgets? Please read the [help document](https://
+qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration Check out this
+[â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off
+what PySide2-Material-Widgets are capable of ð ## Work with QtDesigner You
+can use PySide2-Material-Widgets in QtDesigner directly by running `python ./
+tools/designer.py`. If the operation is successful, you should be able to see
+the PySide2-Material-Widgets in the sidebar of QtDesigner. ## Support If this
+project helps you a lot and you want to support the development and maintenance
+of this project, feel free to sponsor me via [ç±åçµ](https://afdian.net/a/
+zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly
+appreciated ð¥° ## Reference * [**Figma/Material 3 Design Kit**: Provides an
+introduction to the material design system](https://www.figma.com/community/
+file/1035203688168086460/Material-3-Design-Kit) * [**Google/Material Design**:
+A website demonstrates the controls available in Material Design 3 System]
+(https://m3.material.io/get-started) ## License PySide2-Material-Widgets adopts
+dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For
+commercial purposes, please purchase on [ç±åçµ](https://afdian.net/a/
+zhiyiYo?tab=shop) to support the development of this project. Copyright Â© 2021
+by zhiyiYo.
```

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/__init__.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 Examples are available at https://github.com/zhiyiYo/QMaterialWidgets/tree/master/examples.
 
 :copyright: (c) 2023 by zhiyiYo.
 :license: PySide2-Material-Widgets adopts dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE).
 For commercial purposes, please purchase on [爱发电](https://afdian.net/a/zhiyiYo?tab=shop) to support the development of this project.
 """
 
-__version__ = "0.0.11"
+__version__ = "0.1.1"
 
 from .components import *
 from .common import *
 from ._rc import resource
```

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/__init__.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .config import *
-from .font import setFont, getFont, registerFonts
+from .font import setFont, getFont
 from .auto_wrap import TextWrap
 from .icon import Action, Icon, getIconColor, drawSvgIcon, FluentIcon, drawIcon, MaterialIconBase, writeSvg
 from .style_sheet import (setStyleSheet, getStyleSheet, setTheme, ThemeColor, themeColor,
                           setThemeColor, applyThemeColor, MaterialStyleSheet, StyleSheetBase, palette, Palette)
 from .smooth_scroll import SmoothScroll, SmoothMode
 from .translator import MaterialTranslator
 from .router import qrouter, Router
```

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/animation.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/auto_wrap.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/color.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/color.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/config.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/exception_handler.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/icon.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/blend/blend.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/blend/blend.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/cam16.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/cam16.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/hct.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/hct.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/viewing_conditions.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/viewing_conditions.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/core_palette.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/core_palette.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/tonal_palette.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/tonal_palette.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_map.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_map.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/scheme/scheme.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/scheme/scheme.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/score/score.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/score/score.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/color_utils.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/color_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/image_utils.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/math_utils.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/string_utils.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/theme_utils.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/theme_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/overload.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/router.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/smooth_scroll.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/style_sheet.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/mask_dialog_base.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/message_box.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/message_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/expand_layout.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/flow_layout.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/__init__.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from .check_box import CheckBox
 from .card_widget import CardWidget, OutlinedCardWidget, ElevatedCardWidget
 from .button import (OutlinedPushButton, TextPushButton, FilledPushButton, ElevatedPushButton,
                      TonalPushButton, TransparentToolButton, FilledToolButton, TransparentToggleToolButton,
-                     TonalToolButton, OutlinedToolButton, FilledToggleToolButton, OutlinedToggleToolButton)
+                     TonalToolButton, OutlinedToolButton, FilledToggleToolButton, OutlinedToggleToolButton,
+                     OutlinedDropDownPushButton, FilledDropDownPushButton, TextDropDownPushButton,
+                     ElevatedDropDownPushButton, TonalDropDownPushButton)
 from .menu import (LineEditMenu, RoundMenu, MenuAnimationManager, MenuAnimationType, IndicatorMenuItemDelegate,
                    MenuItemDelegate, ShortcutMenuItemDelegate, CheckableMenu, MenuIndicatorType)
 from .radio_button import RadioButton
 from .ripple import RippleStyle
 from .icon_widget import IconWidget
 from .label import (CaptionLabel, StrongBodyLabel, BodyLabel, SubtitleLabel, TitleLabel,
                     LargeTitleLabel, DisplayLabel, MaterialLabelBase, ImageLabel)
```

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/button.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/button.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # coding:utf-8
 from typing import Union
 
 from PySide2.QtCore import Qt, QRectF, QSize, QPoint, Property, QEvent
-from PySide2.QtGui import QPainterPath, QIcon, QPainter, QColor, QPen
+from PySide2.QtGui import QPainterPath, QIcon, QPainter, QColor, QPen, QPalette
 from PySide2.QtWidgets import QPushButton, QToolButton, QApplication, QWidget
 
 from ...common.color import translucent, mixColor
 from ...common.icon import MaterialIconBase, drawIcon, isDarkTheme, Theme, toQIcon, Icon
 from ...common.font import setFont
 from ...common.style_sheet import (MaterialStyleSheet, themeColor, ThemeColor, palette,
                                    hoverMixPrimary, pressedMixPrimary)
 from ...common.animation import BackgroundAnimationWidget, DropShadowAnimation
 from ...common.overload import singledispatchmethod
 from .ripple import RippleOverlayWidget, RippleStyle
+from .menu import RoundMenu
 
 
 
 class PushButton(BackgroundAnimationWidget, QPushButton):
     """ push button """
 
     @singledispatchmethod
@@ -498,7 +499,87 @@
         drawIcon(icon, painter, rect, state)
 
     def _drawBackground(self, painter: QPainter):
         if self.isEnabled():
             painter.setPen('#938F99' if isDarkTheme() else '#79747E')
 
         ToolButton._drawBackground(self, painter)
+
+
+class DropDownIcon(MaterialIconBase):
+
+    def path(self, theme=Theme.AUTO) -> str:
+        return ":/qmaterialwidgets/images/button/ArrowDropDown.svg"
+
+
+
+class DropDownButtonBase:
+    """ Drop down button base class """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._menu = None
+        self.dropDownIcon = DropDownIcon()
+
+    def setMenu(self, menu: RoundMenu):
+        self._menu = menu
+
+    def menu(self) -> RoundMenu:
+        return self._menu
+
+    def mouseReleaseEvent(self, e):
+        super().mouseReleaseEvent(e)
+        self._showMenu()
+
+    def _showMenu(self):
+        if not self.menu():
+            return
+
+        menu = self.menu()
+        menu.view.setMinimumWidth(self.width())
+        menu.view.adjustSize()
+        menu.adjustSize()
+
+        # show menu
+        x = -menu.width()//2 + menu.layout().contentsMargins().left() + self.width()//2
+        y = self.height()
+        menu.exec(self.mapToGlobal(QPoint(x, y)))
+
+    def _hideMenu(self):
+        if self.menu():
+            self.menu().hide()
+
+    def _drawDropDownIcon(self, painter, rect):
+        color = self.palette().color(QPalette.WindowText).name()
+        self.dropDownIcon.render(painter, rect, fill=color)
+
+    def paintEvent(self, e):
+        super().paintEvent(e)
+
+        painter = QPainter(self)
+        painter.setRenderHints(QPainter.Antialiasing)
+        rect = QRectF(self.width()-36, self.height() / 2 - 12, 24, 24)
+        self._drawDropDownIcon(painter, rect)
+
+
+class OutlinedDropDownPushButton(DropDownButtonBase, OutlinedPushButton):
+    """ Drop down push button """
+
+
+class FilledDropDownPushButton(DropDownButtonBase, FilledPushButton):
+    """ Filled drop down push button """
+
+
+class ElevatedDropDownPushButton(DropDownButtonBase, ElevatedPushButton):
+    """ Elevated drop down push button """
+
+
+class TonalDropDownPushButton(DropDownButtonBase, TonalPushButton):
+    """ Tonal drop down push button """
+
+
+class TextDropDownPushButton(DropDownButtonBase, TextPushButton):
+    """ Text drop down push button """
+
+    def _drawDropDownIcon(self, painter, rect: QRectF):
+        rect.moveLeft(self.width() - 32)
+        return super()._drawDropDownIcon(painter, rect)
```

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/card_widget.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/check_box.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/floating_action_button.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/flyout.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/frameless_window.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/icon_widget.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/info_badge.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/info_badge.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/info_bar.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/label.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/menu.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/overlay_widget.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/overlay_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/progress_bar.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/progress_ring.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/radio_button.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/radio_button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/ripple.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/ripple.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/scroll_area.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/scroll_bar.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/stacked_widget.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/switch_button.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/teaching_tip.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/tool_tip.py` & `PySide2-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.11/setup.py` & `PySide2-Material-Widgets-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide2-Material-Widgets",
-    version="0.0.11",
+    version="0.1.1",
     keywords="pyside2 material widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A material design widgets library based on PySide2",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

