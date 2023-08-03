# Comparing `tmp/PySide6-Material-Widgets-0.0.2.tar.gz` & `tmp/PySide6-Material-Widgets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide6-Material-Widgets-0.0.2.tar", last modified: Tue Jul 25 23:55:14 2023, max compression
+gzip compressed data, was "dist\PySide6-Material-Widgets-0.1.1.tar", last modified: Thu Aug  3 03:15:29 2023, max compression
```

## Comparing `PySide6-Material-Widgets-0.0.2.tar` & `PySide6-Material-Widgets-0.1.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.973398 PySide6-Material-Widgets-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-07-24 00:28:48.000000 PySide6-Material-Widgets-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4104 2023-07-25 23:55:14.973398 PySide6-Material-Widgets-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.746503 PySide6-Material-Widgets-0.0.2/PySide6_Material_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4104 2023-07-25 23:55:14.000000 PySide6-Material-Widgets-0.0.2/PySide6_Material_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3899 2023-07-25 23:55:14.000000 PySide6-Material-Widgets-0.0.2/PySide6_Material_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 23:55:14.000000 PySide6-Material-Widgets-0.0.2/PySide6_Material_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-25 23:55:14.000000 PySide6-Material-Widgets-0.0.2/PySide6_Material_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-25 23:55:14.000000 PySide6-Material-Widgets-0.0.2/PySide6_Material_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3301 2023-07-25 13:10:35.000000 PySide6-Material-Widgets-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.746503 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/
--rw-rw-rw-   0        0        0      709 2023-07-25 13:06:27.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.753210 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  5932618 2023-07-25 04:06:55.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.806663 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/
--rw-rw-rw-   0        0        0      552 2023-07-22 14:31:29.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     7944 2023-07-24 03:57:05.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/animation.py
--rw-rw-rw-   0        0        0     3657 2023-06-26 15:48:09.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0     1189 2023-07-17 01:25:50.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/color.py
--rw-rw-rw-   0        0        0    10647 2023-07-17 01:37:12.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0     1306 2023-07-24 04:08:28.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/font.py
--rw-rw-rw-   0        0        0    12686 2023-07-24 04:37:39.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/icon.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.809179 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/
--rw-rw-rw-   0        0        0        0 2023-07-25 23:53:09.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.813291 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/blend/
--rw-rw-rw-   0        0        0        0 2023-07-25 23:53:17.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/blend/__init__.py
--rw-rw-rw-   0        0        0     4816 2023-07-17 01:35:35.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/blend/blend.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.825760 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/hct/
--rw-rw-rw-   0        0        0        0 2023-07-25 23:53:17.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/hct/__init__.py
--rw-rw-rw-   0        0        0    11533 2023-07-17 01:35:19.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/hct/cam16.py
--rw-rw-rw-   0        0        0     8397 2023-07-17 01:35:26.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/hct/hct.py
--rw-rw-rw-   0        0        0     5391 2023-07-17 01:35:30.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/hct/viewing_conditions.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.835661 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/palettes/
--rw-rw-rw-   0        0        0        0 2023-07-25 23:53:17.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/palettes/__init__.py
--rw-rw-rw-   0        0        0     1576 2023-07-17 01:35:03.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/palettes/core_palette.py
--rw-rw-rw-   0        0        0     1985 2023-07-17 01:35:12.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/palettes/tonal_palette.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.853691 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/
--rw-rw-rw-   0        0        0        0 2023-07-25 23:53:17.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/__init__.py
--rw-rw-rw-   0        0        0     1929 2023-07-17 01:34:35.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py
--rw-rw-rw-   0        0        0     2158 2023-07-17 01:34:38.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py
--rw-rw-rw-   0        0        0     1723 2023-07-17 01:34:42.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/quantizer_map.py
--rw-rw-rw-   0        0        0     8297 2023-07-17 01:34:46.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py
--rw-rw-rw-   0        0        0    14347 2023-07-17 01:34:55.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.859371 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/scheme/
--rw-rw-rw-   0        0        0        0 2023-07-25 23:53:17.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/scheme/__init__.py
--rw-rw-rw-   0        0        0     7792 2023-07-21 13:40:47.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/scheme/scheme.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.866002 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/score/
--rw-rw-rw-   0        0        0        0 2023-07-25 23:53:17.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/score/__init__.py
--rw-rw-rw-   0        0        0     6017 2023-07-17 01:34:16.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/score/score.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.884199 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/
--rw-rw-rw-   0        0        0        0 2023-07-25 23:53:17.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/__init__.py
--rw-rw-rw-   0        0        0     7656 2023-07-17 01:33:35.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/color_utils.py
--rw-rw-rw-   0        0        0     2850 2023-07-17 01:35:47.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/image_utils.py
--rw-rw-rw-   0        0        0     2854 2023-07-16 13:31:20.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/math_utils.py
--rw-rw-rw-   0        0        0     2325 2023-07-17 01:33:56.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/string_utils.py
--rw-rw-rw-   0        0        0     3857 2023-07-17 01:34:05.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/theme_utils.py
--rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3862 2023-07-15 10:05:17.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/router.py
--rw-rw-rw-   0        0        0     4874 2023-07-24 04:23:06.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0    12102 2023-07-25 07:18:19.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      460 2023-07-22 14:31:29.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.888606 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/
--rw-rw-rw-   0        0        0       72 2023-07-25 07:08:11.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.896462 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0       35 2023-07-22 09:35:54.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0     3233 2023-07-24 04:25:38.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     4660 2023-07-24 04:26:56.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/dialog_box/message_box.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.905756 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/layout/
--rw-rw-rw-   0        0        0       76 2023-07-18 06:23:37.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2658 2023-07-18 06:23:09.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5437 2023-07-18 06:23:09.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/layout/flow_layout.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:55:14.968307 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/
--rw-rw-rw-   0        0        0     2050 2023-07-25 07:08:20.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0    16812 2023-07-24 05:55:58.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     4932 2023-07-25 01:44:22.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     2437 2023-07-24 04:04:30.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0     5717 2023-07-24 04:16:27.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/floating_action_button.py
--rw-rw-rw-   0        0        0    16139 2023-07-24 04:05:24.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2049 2023-07-18 06:23:09.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1355 2023-07-24 04:02:29.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    16646 2023-07-24 04:20:31.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    21236 2023-07-24 06:04:00.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0     9136 2023-07-24 04:09:21.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    35500 2023-07-24 04:26:21.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0      711 2023-07-15 12:13:17.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/overlay_widget.py
--rw-rw-rw-   0        0        0     8210 2023-07-24 04:21:46.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     5562 2023-07-17 06:32:32.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     1354 2023-07-17 08:36:57.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/radio_button.py
--rw-rw-rw-   0        0        0     5707 2023-07-25 00:11:41.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/ripple.py
--rw-rw-rw-   0        0        0     2598 2023-07-24 04:10:29.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    18195 2023-07-24 04:22:47.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     6356 2023-07-24 04:13:26.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0    10489 2023-07-24 04:26:48.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0    22383 2023-07-24 04:14:13.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10242 2023-07-24 04:14:57.000000 PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0       42 2023-07-25 23:55:14.973398 PySide6-Material-Widgets-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1170 2023-07-25 23:54:46.000000 PySide6-Material-Widgets-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.627418 PySide6-Material-Widgets-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-24 00:28:48.000000 PySide6-Material-Widgets-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4523 2023-08-03 03:15:29.626413 PySide6-Material-Widgets-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.462463 PySide6-Material-Widgets-0.1.1/PySide6_Material_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4523 2023-08-03 03:15:29.000000 PySide6-Material-Widgets-0.1.1/PySide6_Material_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3899 2023-08-03 03:15:29.000000 PySide6-Material-Widgets-0.1.1/PySide6_Material_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 03:15:29.000000 PySide6-Material-Widgets-0.1.1/PySide6_Material_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-08-03 03:15:29.000000 PySide6-Material-Widgets-0.1.1/PySide6_Material_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-03 03:15:29.000000 PySide6-Material-Widgets-0.1.1/PySide6_Material_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3720 2023-08-03 03:14:22.000000 PySide6-Material-Widgets-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.463987 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/
+-rw-rw-rw-   0        0        0      709 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.468577 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  2184800 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.502890 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/
+-rw-rw-rw-   0        0        0      537 2023-08-03 03:14:31.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     7944 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     3657 2023-06-26 15:48:09.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0     1189 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/color.py
+-rw-rw-rw-   0        0        0    10647 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      866 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/font.py
+-rw-rw-rw-   0        0        0    12686 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/icon.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.504053 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.507777 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/blend/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/blend/__init__.py
+-rw-rw-rw-   0        0        0     4816 2023-07-17 01:35:35.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/blend/blend.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.516661 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/__init__.py
+-rw-rw-rw-   0        0        0    11533 2023-07-17 01:35:19.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/cam16.py
+-rw-rw-rw-   0        0        0     8397 2023-07-17 01:35:26.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/hct.py
+-rw-rw-rw-   0        0        0     5391 2023-07-17 01:35:30.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/viewing_conditions.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.523333 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/__init__.py
+-rw-rw-rw-   0        0        0     1576 2023-07-17 01:35:03.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/core_palette.py
+-rw-rw-rw-   0        0        0     1985 2023-07-17 01:35:12.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/tonal_palette.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.537595 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/__init__.py
+-rw-rw-rw-   0        0        0     1929 2023-07-17 01:34:35.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py
+-rw-rw-rw-   0        0        0     2158 2023-07-17 01:34:38.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py
+-rw-rw-rw-   0        0        0     1723 2023-07-17 01:34:42.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_map.py
+-rw-rw-rw-   0        0        0     8297 2023-07-17 01:34:46.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py
+-rw-rw-rw-   0        0        0    14347 2023-07-17 01:34:55.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.542477 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/scheme/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/scheme/__init__.py
+-rw-rw-rw-   0        0        0     7792 2023-07-21 13:40:47.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/scheme/scheme.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.546919 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/score/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/score/__init__.py
+-rw-rw-rw-   0        0        0     6017 2023-07-17 01:34:16.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/score/score.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.559239 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:48:21.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/__init__.py
+-rw-rw-rw-   0        0        0     7656 2023-07-17 01:33:35.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/color_utils.py
+-rw-rw-rw-   0        0        0     2850 2023-07-17 01:35:47.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/image_utils.py
+-rw-rw-rw-   0        0        0     2854 2023-07-16 13:31:20.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/math_utils.py
+-rw-rw-rw-   0        0        0     2325 2023-07-17 01:33:56.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/string_utils.py
+-rw-rw-rw-   0        0        0     3857 2023-07-17 01:34:05.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/theme_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3862 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/router.py
+-rw-rw-rw-   0        0        0     4874 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0    12102 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      460 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.561243 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/
+-rw-rw-rw-   0        0        0       72 2023-07-26 04:29:03.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.568039 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0       35 2023-07-22 09:35:54.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0     3233 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     4660 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/message_box.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.573349 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/
+-rw-rw-rw-   0        0        0       76 2023-07-18 06:23:37.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2658 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5437 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/flow_layout.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:15:29.623891 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     2225 2023-08-03 03:11:18.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0    19155 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     4932 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     2437 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0     5717 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/floating_action_button.py
+-rw-rw-rw-   0        0        0    16139 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2049 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1355 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    16646 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    21236 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0     9136 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    35500 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0      711 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/overlay_widget.py
+-rw-rw-rw-   0        0        0     8210 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     5562 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     1354 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/radio_button.py
+-rw-rw-rw-   0        0        0     5707 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/ripple.py
+-rw-rw-rw-   0        0        0     2598 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    18195 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     6356 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0    10489 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0    22383 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10242 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 03:15:29.627418 PySide6-Material-Widgets-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1170 2023-08-03 03:14:23.000000 PySide6-Material-Widgets-0.1.1/setup.py
```

### Comparing `PySide6-Material-Widgets-0.0.2/LICENSE` & `PySide6-Material-Widgets-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/PKG-INFO` & `PySide6-Material-Widgets-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Material-Widgets
-Version: 0.0.2
+Version: 0.1.1
 Summary: A material design widgets library based on PySide6
 Home-page: https://github.com/zhiyiYo/QMaterialWidgets/tree/master
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qmaterialwidgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/QMaterialWidgets/tree/master
@@ -24,20 +24,24 @@
   PySide6-Material-Widgets
 </h1>
 <p align="center">
   A material design widgets library based on PySide6
 </p>
 
 <p align="center">
+  <a href="https://pypi.org/project/PySide6-Material-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pyside6-material-widgets?color=%2334D058&label=Version" alt="Version">
+  </a>
+
   <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/Version-0.1.0-blue?color=#4ec820" alt="Version 0.1.0"/>
+    <img src="https://static.pepy.tech/personalized-badge/pyside6-material-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
   </a>
 
   <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="License GPLv3"/>
+    <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
   </a>
 </p>
 
@@ -56,27 +60,29 @@
 The Community version only provides basic components, while the more advanced ones are available in the [Premium version](https://afdian.net/a/zhiyiYo?tab=shop).
 
 > **Warning**
 > Don't install PySide6-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
 
 
 ## Run Example
+You can download the executable demo from the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases).
+
 After installing PySide6-Material-Widgets package using pip, you can run the demo in examples directory, for example:
 ```python
 cd examples/button
 python demo.py
 ```
 
 If you encounter `ImportError: cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the imported components are only available in the Premium version.
 
 ## Documentation
 Want to know more about PySide6-Material-Widgets? Please read the [help document](https://qmaterialwidgets.readthedocs.io/) 👈
 
 ## Video Demonstration
-Check out this [▶ example video](https://www.bilibili.com/video/BV12c411L73q) that shows off what PySide6-Material-Widgets are capable of 🎉
+Check out this [▶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off what PySide6-Material-Widgets are capable of 🎉
 
 ## Work with QtDesigner
 You can use PySide6-Material-Widgets in QtDesigner directly by running `python ./tools/designer.py`. If the operation is successful, you should be able to see the PySide6-Material-Widgets in the sidebar of QtDesigner.
 
 
 ## Support
 If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
```

#### html2text {}

```diff
@@ -1,47 +1,49 @@
-Metadata-Version: 2.1 Name: PySide6-Material-Widgets Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: PySide6-Material-Widgets Version: 0.1.1 Summary: A
 material design widgets library based on PySide6 Home-page: https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 qmaterialwidgets.readthedocs.io/ Project-URL: Source Code, https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/QMaterialWidgets/issues Keywords: pyside6 material widgets
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE
                                     [logo]
                     ****** PySide6-Material-Widgets ******
               A material design widgets library based on PySide6
-       [Version 0.1.0] [License GPLv3] [Platform Win32 | Linux | macOS]
+         [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/
 docs/source/_static/Interface.jpg) ## Install To install Community version:
 ```shell pip install PySide6-Material-Widgets -i https://pypi.org/simple/ ```
 The Community version only provides basic components, while the more advanced
 ones are available in the [Premium version](https://afdian.net/a/
 zhiyiYo?tab=shop). > **Warning** > Don't install PySide6-Material-Widgets and
 PySide2-Material-Widgets at the same time, because their package names are all
-`qmaterialwidgets`. ## Run Example After installing PySide6-Material-Widgets
-package using pip, you can run the demo in examples directory, for example:
-```python cd examples/button python demo.py ``` If you encounter `ImportError:
-cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the
-imported components are only available in the Premium version. ## Documentation
-Want to know more about PySide6-Material-Widgets? Please read the [help
-document](https://qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration
-Check out this [â¶ example video](https://www.bilibili.com/video/BV12c411L73q)
-that shows off what PySide6-Material-Widgets are capable of ð ## Work with
-QtDesigner You can use PySide6-Material-Widgets in QtDesigner directly by
-running `python ./tools/designer.py`. If the operation is successful, you
-should be able to see the PySide6-Material-Widgets in the sidebar of
-QtDesigner. ## Support If this project helps you a lot and you want to support
-the development and maintenance of this project, feel free to sponsor me via
-[ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/
-zhiyiYo). Your support is highly appreciated ð¥° ## Reference * [**Figma/
-Material 3 Design Kit**: Provides an introduction to the material design
-system](https://www.figma.com/community/file/1035203688168086460/Material-3-
-Design-Kit) * [**Google/Material Design**: A website demonstrates the controls
-available in Material Design 3 System](https://m3.material.io/get-started) ##
-License PySide6-Material-Widgets adopts dual licenses. Non-commercial usage is
-licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on
-[ç±åçµ](https://afdian.net/a/zhiyiYo?tab=shop) to support the development
-of this project. Copyright Â© 2021 by zhiyiYo.
+`qmaterialwidgets`. ## Run Example You can download the executable demo from
+the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases). After
+installing PySide6-Material-Widgets package using pip, you can run the demo in
+examples directory, for example: ```python cd examples/button python demo.py
+``` If you encounter `ImportError: cannot import name 'XXX' from
+'qmaterialwidgets'`, it indicates that the imported components are only
+available in the Premium version. ## Documentation Want to know more about
+PySide6-Material-Widgets? Please read the [help document](https://
+qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration Check out this
+[â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off
+what PySide6-Material-Widgets are capable of ð ## Work with QtDesigner You
+can use PySide6-Material-Widgets in QtDesigner directly by running `python ./
+tools/designer.py`. If the operation is successful, you should be able to see
+the PySide6-Material-Widgets in the sidebar of QtDesigner. ## Support If this
+project helps you a lot and you want to support the development and maintenance
+of this project, feel free to sponsor me via [ç±åçµ](https://afdian.net/a/
+zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly
+appreciated ð¥° ## Reference * [**Figma/Material 3 Design Kit**: Provides an
+introduction to the material design system](https://www.figma.com/community/
+file/1035203688168086460/Material-3-Design-Kit) * [**Google/Material Design**:
+A website demonstrates the controls available in Material Design 3 System]
+(https://m3.material.io/get-started) ## License PySide6-Material-Widgets adopts
+dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For
+commercial purposes, please purchase on [ç±åçµ](https://afdian.net/a/
+zhiyiYo?tab=shop) to support the development of this project. Copyright Â© 2021
+by zhiyiYo.
```

### Comparing `PySide6-Material-Widgets-0.0.2/PySide6_Material_Widgets.egg-info/PKG-INFO` & `PySide6-Material-Widgets-0.1.1/PySide6_Material_Widgets.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Material-Widgets
-Version: 0.0.2
+Version: 0.1.1
 Summary: A material design widgets library based on PySide6
 Home-page: https://github.com/zhiyiYo/QMaterialWidgets/tree/master
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qmaterialwidgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/QMaterialWidgets/tree/master
@@ -24,20 +24,24 @@
   PySide6-Material-Widgets
 </h1>
 <p align="center">
   A material design widgets library based on PySide6
 </p>
 
 <p align="center">
+  <a href="https://pypi.org/project/PySide6-Material-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pyside6-material-widgets?color=%2334D058&label=Version" alt="Version">
+  </a>
+
   <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/Version-0.1.0-blue?color=#4ec820" alt="Version 0.1.0"/>
+    <img src="https://static.pepy.tech/personalized-badge/pyside6-material-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
   </a>
 
   <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="License GPLv3"/>
+    <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
   </a>
 </p>
 
@@ -56,27 +60,29 @@
 The Community version only provides basic components, while the more advanced ones are available in the [Premium version](https://afdian.net/a/zhiyiYo?tab=shop).
 
 > **Warning**
 > Don't install PySide6-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
 
 
 ## Run Example
+You can download the executable demo from the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases).
+
 After installing PySide6-Material-Widgets package using pip, you can run the demo in examples directory, for example:
 ```python
 cd examples/button
 python demo.py
 ```
 
 If you encounter `ImportError: cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the imported components are only available in the Premium version.
 
 ## Documentation
 Want to know more about PySide6-Material-Widgets? Please read the [help document](https://qmaterialwidgets.readthedocs.io/) 👈
 
 ## Video Demonstration
-Check out this [▶ example video](https://www.bilibili.com/video/BV12c411L73q) that shows off what PySide6-Material-Widgets are capable of 🎉
+Check out this [▶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off what PySide6-Material-Widgets are capable of 🎉
 
 ## Work with QtDesigner
 You can use PySide6-Material-Widgets in QtDesigner directly by running `python ./tools/designer.py`. If the operation is successful, you should be able to see the PySide6-Material-Widgets in the sidebar of QtDesigner.
 
 
 ## Support
 If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
```

#### html2text {}

```diff
@@ -1,47 +1,49 @@
-Metadata-Version: 2.1 Name: PySide6-Material-Widgets Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: PySide6-Material-Widgets Version: 0.1.1 Summary: A
 material design widgets library based on PySide6 Home-page: https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 qmaterialwidgets.readthedocs.io/ Project-URL: Source Code, https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/QMaterialWidgets/issues Keywords: pyside6 material widgets
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE
                                     [logo]
                     ****** PySide6-Material-Widgets ******
               A material design widgets library based on PySide6
-       [Version 0.1.0] [License GPLv3] [Platform Win32 | Linux | macOS]
+         [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/
 docs/source/_static/Interface.jpg) ## Install To install Community version:
 ```shell pip install PySide6-Material-Widgets -i https://pypi.org/simple/ ```
 The Community version only provides basic components, while the more advanced
 ones are available in the [Premium version](https://afdian.net/a/
 zhiyiYo?tab=shop). > **Warning** > Don't install PySide6-Material-Widgets and
 PySide2-Material-Widgets at the same time, because their package names are all
-`qmaterialwidgets`. ## Run Example After installing PySide6-Material-Widgets
-package using pip, you can run the demo in examples directory, for example:
-```python cd examples/button python demo.py ``` If you encounter `ImportError:
-cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the
-imported components are only available in the Premium version. ## Documentation
-Want to know more about PySide6-Material-Widgets? Please read the [help
-document](https://qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration
-Check out this [â¶ example video](https://www.bilibili.com/video/BV12c411L73q)
-that shows off what PySide6-Material-Widgets are capable of ð ## Work with
-QtDesigner You can use PySide6-Material-Widgets in QtDesigner directly by
-running `python ./tools/designer.py`. If the operation is successful, you
-should be able to see the PySide6-Material-Widgets in the sidebar of
-QtDesigner. ## Support If this project helps you a lot and you want to support
-the development and maintenance of this project, feel free to sponsor me via
-[ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/
-zhiyiYo). Your support is highly appreciated ð¥° ## Reference * [**Figma/
-Material 3 Design Kit**: Provides an introduction to the material design
-system](https://www.figma.com/community/file/1035203688168086460/Material-3-
-Design-Kit) * [**Google/Material Design**: A website demonstrates the controls
-available in Material Design 3 System](https://m3.material.io/get-started) ##
-License PySide6-Material-Widgets adopts dual licenses. Non-commercial usage is
-licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on
-[ç±åçµ](https://afdian.net/a/zhiyiYo?tab=shop) to support the development
-of this project. Copyright Â© 2021 by zhiyiYo.
+`qmaterialwidgets`. ## Run Example You can download the executable demo from
+the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases). After
+installing PySide6-Material-Widgets package using pip, you can run the demo in
+examples directory, for example: ```python cd examples/button python demo.py
+``` If you encounter `ImportError: cannot import name 'XXX' from
+'qmaterialwidgets'`, it indicates that the imported components are only
+available in the Premium version. ## Documentation Want to know more about
+PySide6-Material-Widgets? Please read the [help document](https://
+qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration Check out this
+[â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off
+what PySide6-Material-Widgets are capable of ð ## Work with QtDesigner You
+can use PySide6-Material-Widgets in QtDesigner directly by running `python ./
+tools/designer.py`. If the operation is successful, you should be able to see
+the PySide6-Material-Widgets in the sidebar of QtDesigner. ## Support If this
+project helps you a lot and you want to support the development and maintenance
+of this project, feel free to sponsor me via [ç±åçµ](https://afdian.net/a/
+zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly
+appreciated ð¥° ## Reference * [**Figma/Material 3 Design Kit**: Provides an
+introduction to the material design system](https://www.figma.com/community/
+file/1035203688168086460/Material-3-Design-Kit) * [**Google/Material Design**:
+A website demonstrates the controls available in Material Design 3 System]
+(https://m3.material.io/get-started) ## License PySide6-Material-Widgets adopts
+dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For
+commercial purposes, please purchase on [ç±åçµ](https://afdian.net/a/
+zhiyiYo?tab=shop) to support the development of this project. Copyright Â© 2021
+by zhiyiYo.
```

### Comparing `PySide6-Material-Widgets-0.0.2/PySide6_Material_Widgets.egg-info/SOURCES.txt` & `PySide6-Material-Widgets-0.1.1/PySide6_Material_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/README.md` & `PySide6-Material-Widgets-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,24 @@
   PySide6-Material-Widgets
 </h1>
 <p align="center">
   A material design widgets library based on PySide6
 </p>
 
 <p align="center">
+  <a href="https://pypi.org/project/PySide6-Material-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pyside6-material-widgets?color=%2334D058&label=Version" alt="Version">
+  </a>
+
   <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/Version-0.1.0-blue?color=#4ec820" alt="Version 0.1.0"/>
+    <img src="https://static.pepy.tech/personalized-badge/pyside6-material-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
   </a>
 
   <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="License GPLv3"/>
+    <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
   </a>
 </p>
 
@@ -37,27 +41,29 @@
 The Community version only provides basic components, while the more advanced ones are available in the [Premium version](https://afdian.net/a/zhiyiYo?tab=shop).
 
 > **Warning**
 > Don't install PySide6-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
 
 
 ## Run Example
+You can download the executable demo from the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases).
+
 After installing PySide6-Material-Widgets package using pip, you can run the demo in examples directory, for example:
 ```python
 cd examples/button
 python demo.py
 ```
 
 If you encounter `ImportError: cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the imported components are only available in the Premium version.
 
 ## Documentation
 Want to know more about PySide6-Material-Widgets? Please read the [help document](https://qmaterialwidgets.readthedocs.io/) 👈
 
 ## Video Demonstration
-Check out this [▶ example video](https://www.bilibili.com/video/BV12c411L73q) that shows off what PySide6-Material-Widgets are capable of 🎉
+Check out this [▶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off what PySide6-Material-Widgets are capable of 🎉
 
 ## Work with QtDesigner
 You can use PySide6-Material-Widgets in QtDesigner directly by running `python ./tools/designer.py`. If the operation is successful, you should be able to see the PySide6-Material-Widgets in the sidebar of QtDesigner.
 
 
 ## Support
 If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
```

#### html2text {}

```diff
@@ -1,36 +1,38 @@
                                     [logo]
                     ****** PySide6-Material-Widgets ******
               A material design widgets library based on PySide6
-       [Version 0.1.0] [License GPLv3] [Platform Win32 | Linux | macOS]
+         [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/
 docs/source/_static/Interface.jpg) ## Install To install Community version:
 ```shell pip install PySide6-Material-Widgets -i https://pypi.org/simple/ ```
 The Community version only provides basic components, while the more advanced
 ones are available in the [Premium version](https://afdian.net/a/
 zhiyiYo?tab=shop). > **Warning** > Don't install PySide6-Material-Widgets and
 PySide2-Material-Widgets at the same time, because their package names are all
-`qmaterialwidgets`. ## Run Example After installing PySide6-Material-Widgets
-package using pip, you can run the demo in examples directory, for example:
-```python cd examples/button python demo.py ``` If you encounter `ImportError:
-cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the
-imported components are only available in the Premium version. ## Documentation
-Want to know more about PySide6-Material-Widgets? Please read the [help
-document](https://qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration
-Check out this [â¶ example video](https://www.bilibili.com/video/BV12c411L73q)
-that shows off what PySide6-Material-Widgets are capable of ð ## Work with
-QtDesigner You can use PySide6-Material-Widgets in QtDesigner directly by
-running `python ./tools/designer.py`. If the operation is successful, you
-should be able to see the PySide6-Material-Widgets in the sidebar of
-QtDesigner. ## Support If this project helps you a lot and you want to support
-the development and maintenance of this project, feel free to sponsor me via
-[ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/
-zhiyiYo). Your support is highly appreciated ð¥° ## Reference * [**Figma/
-Material 3 Design Kit**: Provides an introduction to the material design
-system](https://www.figma.com/community/file/1035203688168086460/Material-3-
-Design-Kit) * [**Google/Material Design**: A website demonstrates the controls
-available in Material Design 3 System](https://m3.material.io/get-started) ##
-License PySide6-Material-Widgets adopts dual licenses. Non-commercial usage is
-licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on
-[ç±åçµ](https://afdian.net/a/zhiyiYo?tab=shop) to support the development
-of this project. Copyright Â© 2021 by zhiyiYo.
+`qmaterialwidgets`. ## Run Example You can download the executable demo from
+the [release page](https://github.com/zhiyiYo/QMaterialWidgets/releases). After
+installing PySide6-Material-Widgets package using pip, you can run the demo in
+examples directory, for example: ```python cd examples/button python demo.py
+``` If you encounter `ImportError: cannot import name 'XXX' from
+'qmaterialwidgets'`, it indicates that the imported components are only
+available in the Premium version. ## Documentation Want to know more about
+PySide6-Material-Widgets? Please read the [help document](https://
+qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration Check out this
+[â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off
+what PySide6-Material-Widgets are capable of ð ## Work with QtDesigner You
+can use PySide6-Material-Widgets in QtDesigner directly by running `python ./
+tools/designer.py`. If the operation is successful, you should be able to see
+the PySide6-Material-Widgets in the sidebar of QtDesigner. ## Support If this
+project helps you a lot and you want to support the development and maintenance
+of this project, feel free to sponsor me via [ç±åçµ](https://afdian.net/a/
+zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly
+appreciated ð¥° ## Reference * [**Figma/Material 3 Design Kit**: Provides an
+introduction to the material design system](https://www.figma.com/community/
+file/1035203688168086460/Material-3-Design-Kit) * [**Google/Material Design**:
+A website demonstrates the controls available in Material Design 3 System]
+(https://m3.material.io/get-started) ## License PySide6-Material-Widgets adopts
+dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For
+commercial purposes, please purchase on [ç±åçµ](https://afdian.net/a/
+zhiyiYo?tab=shop) to support the development of this project. Copyright Â© 2021
+by zhiyiYo.
```

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/__init__.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 Examples are available at https://github.com/zhiyiYo/QMaterialWidgets/tree/master/examples.
 
 :copyright: (c) 2023 by zhiyiYo.
 :license: PySide6-Material-Widgets adopts dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE).
 For commercial purposes, please purchase on [爱发电](https://afdian.net/a/zhiyiYo?tab=shop) to support the development of this project.
 """
 
-__version__ = "0.0.1"
+__version__ = "0.1.1"
 
 from .components import *
 from .common import *
 from ._rc import resource
```

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/__init__.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/__init__.py`

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

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/animation.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/auto_wrap.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/color.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/color.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/config.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/exception_handler.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/icon.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/blend/blend.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/blend/blend.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/hct/cam16.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/cam16.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/hct/hct.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/hct.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/hct/viewing_conditions.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/hct/viewing_conditions.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/palettes/core_palette.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/core_palette.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/palettes/tonal_palette.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/palettes/tonal_palette.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/quantizer_map.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_map.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/scheme/scheme.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/scheme/scheme.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/score/score.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/score/score.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/color_utils.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/color_utils.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/image_utils.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/math_utils.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/string_utils.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/material_color/utils/theme_utils.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/material_color/utils/theme_utils.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/overload.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/router.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/smooth_scroll.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/common/style_sheet.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/dialog_box/mask_dialog_base.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/dialog_box/message_box.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/dialog_box/message_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/layout/expand_layout.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/layout/flow_layout.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/__init__.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/__init__.py`

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

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/button.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/button.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # coding:utf-8
 from typing import Union
 
 from PySide6.QtCore import Qt, QRectF, QSize, QPoint, Property, QEvent
-from PySide6.QtGui import QPainterPath, QIcon, QPainter, QColor, QPen
+from PySide6.QtGui import QPainterPath, QIcon, QPainter, QColor, QPen, QPalette
 from PySide6.QtWidgets import QPushButton, QToolButton, QApplication, QWidget
 
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

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/card_widget.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/check_box.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/floating_action_button.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/flyout.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/frameless_window.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/icon_widget.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/info_badge.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/info_badge.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/info_bar.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/label.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/menu.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/overlay_widget.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/overlay_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/progress_bar.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/progress_ring.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/radio_button.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/radio_button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/ripple.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/ripple.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/scroll_area.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/scroll_bar.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/stacked_widget.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/switch_button.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/teaching_tip.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/qmaterialwidgets/components/widgets/tool_tip.py` & `PySide6-Material-Widgets-0.1.1/qmaterialwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Material-Widgets-0.0.2/setup.py` & `PySide6-Material-Widgets-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide6-Material-Widgets",
-    version="0.0.2",
+    version="0.1.1",
     keywords="pyside6 material widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A material design widgets library based on PySide6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

