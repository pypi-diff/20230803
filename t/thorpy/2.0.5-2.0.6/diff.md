# Comparing `tmp/thorpy-2.0.5.tar.gz` & `tmp/thorpy-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thorpy-2.0.5.tar", last modified: Fri Jul  7 13:58:46 2023, max compression
+gzip compressed data, was "thorpy-2.0.6.tar", last modified: Thu Aug  3 21:07:42 2023, max compression
```

## Comparing `thorpy-2.0.5.tar` & `thorpy-2.0.6.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 13:58:46.786334 thorpy-2.0.5/
--rw-rw-rw-   0        0        0     1093 2023-04-18 20:35:49.000000 thorpy-2.0.5/LICENSE
--rw-rw-rw-   0        0        0      378 2023-07-07 13:58:46.785352 thorpy-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2768 2023-07-07 13:58:29.000000 thorpy-2.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 13:58:46.786334 thorpy-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0      596 2023-07-07 13:57:27.000000 thorpy-2.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:58:46.727809 thorpy-2.0.5/thorpy/
--rw-rw-rw-   0        0        0     3603 2023-07-07 13:58:24.000000 thorpy-2.0.5/thorpy/__init__.py
--rw-rw-rw-   0        0        0    53629 2023-07-07 13:25:05.000000 thorpy-2.0.5/thorpy/canonical.py
--rw-rw-rw-   0        0        0   124246 2023-07-07 13:42:31.000000 thorpy-2.0.5/thorpy/elements.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:58:46.785352 thorpy-2.0.5/thorpy/examples/
--rw-rw-rw-   0        0        0        0 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/__init__.py
--rw-rw-rw-   0        0        0     1132 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_alert.py
--rw-rw-rw-   0        0        0     1243 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_anim_move.py
--rw-rw-rw-   0        0        0     1703 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_animatedgif.py
--rw-rw-rw-   0        0        0      992 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_box.py
--rw-rw-rw-   0        0        0      861 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_button_helloworld.py
--rw-rw-rw-   0        0        0      868 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_color_gradient.py
--rw-rw-rw-   0        0        0     1183 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_colorpicker.py
--rw-rw-rw-   0        0        0     2400 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_colorpicker2.py
--rw-rw-rw-   0        0        0     2402 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_colorpicker_fine_tuning.py
--rw-rw-rw-   0        0        0     3284 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_create_style.py
--rw-rw-rw-   0        0        0     3425 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_create_style2.py
--rw-rw-rw-   0        0        0     2249 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_custom_theme.py
--rw-rw-rw-   0        0        0     2063 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_dropdownlist.py
--rw-rw-rw-   0        0        0     1790 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_events.py
--rw-rw-rw-   0        0        0     1177 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_filebrowser.py
--rw-rw-rw-   0        0        0     2245 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_fx_light_emitting_image.py
--rw-rw-rw-   0        0        0     3235 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_fx_lights.py
--rw-rw-rw-   0        0        0     1984 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_get_value_from_elements.py
--rw-rw-rw-   0        0        0     1376 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_grouping.py
--rw-rw-rw-   0        0        0     1112 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_grouping_without_sorting.py
--rw-rw-rw-   0        0        0     2575 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_groups_of_groups.py
--rw-rw-rw-   0        0        0     3731 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_guess_the_number.py
--rw-rw-rw-   0        0        0     1573 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_helper.py
--rw-rw-rw-   0        0        0      982 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_heterogeneous_texts.py
--rw-rw-rw-   0        0        0      685 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_image_with_text.py
--rw-rw-rw-   0        0        0     1322 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_imagebutton.py
--rw-rw-rw-   0        0        0     1532 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_integration_in_existing_code.py
--rw-rw-rw-   0        0        0     1316 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_labels.py
--rw-rw-rw-   0        0        0     3028 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_launch.py
--rw-rw-rw-   0        0        0     1287 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_lifebar.py
--rw-rw-rw-   0        0        0     1305 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_look_tune.py
--rw-rw-rw-   0        0        0     2297 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_rich_text.py
--rw-rw-rw-   0        0        0     1307 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_set_default_font.py
--rw-rw-rw-   0        0        0     2128 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_shadows.py
--rw-rw-rw-   0        0        0     3051 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_showcase_themes.py
--rw-rw-rw-   0        0        0     3184 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_showcase_themes2.py
--rw-rw-rw-   0        0        0     2119 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_showcase_themes_buttons.py
--rw-rw-rw-   0        0        0     1500 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_showfps.py
--rw-rw-rw-   0        0        0     1660 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_slider.py
--rw-rw-rw-   0        0        0     2460 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_text_input.py
--rw-rw-rw-   0        0        0     2765 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_text_width.py
--rw-rw-rw-   0        0        0     1431 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_togglables_pool.py
--rw-rw-rw-   0        0        0     1105 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_user_choices.py
--rw-rw-rw-   0        0        0     1431 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_user_choices2.py
--rw-rw-rw-   0        0        0     2051 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_user_chooses_font.py
--rw-rw-rw-   0        0        0     2219 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_waiting_bar.py
--rw-rw-rw-   0        0        0     4520 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/gametools.py
--rw-rw-rw-   0        0        0    32626 2023-07-07 13:18:26.000000 thorpy-2.0.5/thorpy/graphics.py
--rw-rw-rw-   0        0        0     6068 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/loops.py
--rw-rw-rw-   0        0        0     2257 2023-07-04 10:28:17.000000 thorpy-2.0.5/thorpy/monitoring.py
--rw-rw-rw-   0        0        0      467 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/parameters.py
--rw-rw-rw-   0        0        0      625 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/setup.py
--rw-rw-rw-   0        0        0     3727 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/shadows.py
--rw-rw-rw-   0        0        0     2540 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/sorting.py
--rw-rw-rw-   0        0        0     2307 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/sound.py
--rw-rw-rw-   0        0        0    35577 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/styles.py
--rw-rw-rw-   0        0        0    32875 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/themes.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:58:46.738812 thorpy-2.0.5/thorpy.egg-info/
--rw-rw-rw-   0        0        0      378 2023-07-07 13:58:46.000000 thorpy-2.0.5/thorpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2349 2023-07-07 13:58:46.000000 thorpy-2.0.5/thorpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:58:46.000000 thorpy-2.0.5/thorpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 13:58:46.000000 thorpy-2.0.5/thorpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 21:07:42.697409 thorpy-2.0.6/
+-rw-rw-rw-   0        0        0     1093 2023-04-18 20:35:49.000000 thorpy-2.0.6/LICENSE
+-rw-rw-rw-   0        0        0      378 2023-08-03 21:07:42.697409 thorpy-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2949 2023-08-03 21:06:58.000000 thorpy-2.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 21:07:42.697409 thorpy-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      596 2023-08-03 20:54:55.000000 thorpy-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:07:42.646262 thorpy-2.0.6/thorpy/
+-rw-rw-rw-   0        0        0     3603 2023-08-03 20:54:37.000000 thorpy-2.0.6/thorpy/__init__.py
+-rw-rw-rw-   0        0        0    56555 2023-08-03 20:49:03.000000 thorpy-2.0.6/thorpy/canonical.py
+-rw-rw-rw-   0        0        0   125340 2023-08-02 20:39:37.000000 thorpy-2.0.6/thorpy/elements.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:07:42.696410 thorpy-2.0.6/thorpy/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/__init__.py
+-rw-rw-rw-   0        0        0     1132 2023-08-03 20:52:52.000000 thorpy-2.0.6/thorpy/examples/_example_alert.py
+-rw-rw-rw-   0        0        0     1243 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_anim_move.py
+-rw-rw-rw-   0        0        0     1703 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_animatedgif.py
+-rw-rw-rw-   0        0        0      992 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_box.py
+-rw-rw-rw-   0        0        0      861 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_button_helloworld.py
+-rw-rw-rw-   0        0        0      868 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_color_gradient.py
+-rw-rw-rw-   0        0        0     1183 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_colorpicker.py
+-rw-rw-rw-   0        0        0     2400 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_colorpicker2.py
+-rw-rw-rw-   0        0        0     2402 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_colorpicker_fine_tuning.py
+-rw-rw-rw-   0        0        0     3284 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_create_style.py
+-rw-rw-rw-   0        0        0     3425 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_create_style2.py
+-rw-rw-rw-   0        0        0     2249 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_custom_theme.py
+-rw-rw-rw-   0        0        0     2063 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_dropdownlist.py
+-rw-rw-rw-   0        0        0     1790 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_events.py
+-rw-rw-rw-   0        0        0     1177 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_filebrowser.py
+-rw-rw-rw-   0        0        0     2245 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_fx_light_emitting_image.py
+-rw-rw-rw-   0        0        0     3235 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_fx_lights.py
+-rw-rw-rw-   0        0        0     1984 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_get_value_from_elements.py
+-rw-rw-rw-   0        0        0     1376 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_grouping.py
+-rw-rw-rw-   0        0        0     1112 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_grouping_without_sorting.py
+-rw-rw-rw-   0        0        0     2575 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_groups_of_groups.py
+-rw-rw-rw-   0        0        0     3731 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_guess_the_number.py
+-rw-rw-rw-   0        0        0     1573 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_helper.py
+-rw-rw-rw-   0        0        0      982 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_heterogeneous_texts.py
+-rw-rw-rw-   0        0        0      685 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_image_with_text.py
+-rw-rw-rw-   0        0        0     1322 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_imagebutton.py
+-rw-rw-rw-   0        0        0     1532 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_integration_in_existing_code.py
+-rw-rw-rw-   0        0        0     1316 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_labels.py
+-rw-rw-rw-   0        0        0     3028 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_launch.py
+-rw-rw-rw-   0        0        0     1287 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_lifebar.py
+-rw-rw-rw-   0        0        0     1305 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_look_tune.py
+-rw-rw-rw-   0        0        0     2297 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_rich_text.py
+-rw-rw-rw-   0        0        0     1555 2023-08-03 21:04:22.000000 thorpy-2.0.6/thorpy/examples/_example_rotations.py
+-rw-rw-rw-   0        0        0     1307 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_set_default_font.py
+-rw-rw-rw-   0        0        0     2128 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_shadows.py
+-rw-rw-rw-   0        0        0     3051 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_showcase_themes.py
+-rw-rw-rw-   0        0        0     3184 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_showcase_themes2.py
+-rw-rw-rw-   0        0        0     2119 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_showcase_themes_buttons.py
+-rw-rw-rw-   0        0        0     1500 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_showfps.py
+-rw-rw-rw-   0        0        0     1660 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_slider.py
+-rw-rw-rw-   0        0        0     2460 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_text_input.py
+-rw-rw-rw-   0        0        0     2765 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_text_width.py
+-rw-rw-rw-   0        0        0     1431 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_togglables_pool.py
+-rw-rw-rw-   0        0        0     1105 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_user_choices.py
+-rw-rw-rw-   0        0        0     1431 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_user_choices2.py
+-rw-rw-rw-   0        0        0     2051 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_user_chooses_font.py
+-rw-rw-rw-   0        0        0     2219 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/examples/_example_waiting_bar.py
+-rw-rw-rw-   0        0        0     4520 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/gametools.py
+-rw-rw-rw-   0        0        0    32626 2023-07-07 13:18:26.000000 thorpy-2.0.6/thorpy/graphics.py
+-rw-rw-rw-   0        0        0     6068 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/loops.py
+-rw-rw-rw-   0        0        0     2257 2023-07-04 10:28:17.000000 thorpy-2.0.6/thorpy/monitoring.py
+-rw-rw-rw-   0        0        0      467 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/parameters.py
+-rw-rw-rw-   0        0        0      625 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/setup.py
+-rw-rw-rw-   0        0        0     3727 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/shadows.py
+-rw-rw-rw-   0        0        0     2540 2023-08-02 20:37:54.000000 thorpy-2.0.6/thorpy/sorting.py
+-rw-rw-rw-   0        0        0     2307 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/sound.py
+-rw-rw-rw-   0        0        0    35577 2023-05-11 18:30:45.000000 thorpy-2.0.6/thorpy/styles.py
+-rw-rw-rw-   0        0        0    32896 2023-08-03 20:44:00.000000 thorpy-2.0.6/thorpy/themes.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:07:42.659263 thorpy-2.0.6/thorpy.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-08-03 21:07:42.000000 thorpy-2.0.6/thorpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2387 2023-08-03 21:07:42.000000 thorpy-2.0.6/thorpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 21:07:42.000000 thorpy-2.0.6/thorpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 21:07:42.000000 thorpy-2.0.6/thorpy.egg-info/top_level.txt
```

### Comparing `thorpy-2.0.5/LICENSE` & `thorpy-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/README.md` & `thorpy-2.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # ThorpyWebsite (c) Yann Thorimbert 2023
 
 How to generate site :
 * Set the root for Thorpy in generate_website.py
-    (in general, I copy/paste all the code from site-packages/thorpy to ../Thorpy2)
-* Copy paste the actual thorpy folder to ./thorpy/
+    For thorpy's core code, I copy/paste all the code from site-packages/thorpy to ../Thorpy2.
+    For the examples, it's often in ../Thorpy2. Be careful to use the right folder in any case !
+* Copy-paste the actual thorpy folder to ./thorpy/
     Attention /!\ : j'ai dû c/c aussi dans ./thorpy pour que ça marche...
 * Run generate_website.py
 
 How to update elements :
 * Nothing special to do for the doc description, it is automatic as long as you indicate things in docstrings
 * For the image, put an image with the same name as the class (but lowercase) in the doc folder
+* For the examples, don't forget to add tags so that it is referenced.
 
 Files to upload to server:
 * All things inside to_upload/ should be sent to ftp.thorpy.org/httpdocs/
 
 Upload on PyPi :
 1. Copy paste the actual thorpy folder (on my computer its 'Thorpy2') to ./thorpy/
 2. Change version number in both setup.py AND thorpy/__init__.py (and dont forget the actual thorpy git !)
```

### Comparing `thorpy-2.0.5/setup.py` & `thorpy-2.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 setup(name='thorpy',
-      version='2.0.5',
+      version='2.0.6',
       description='GUI library for pygame',
       long_description='ThorPy is a non-intrusive, straightforward GUI kit for Pygame.',
       author='Yann Thorimbert',
       author_email='yann.thorimbert@gmail.com',
       url='http://www.thorpy.org/',
       keywords=['pygame', 'gui', 'menus', 'buttons', 'widgets', 'user interface', 'toolkit'],
       packages=find_packages(),
```

### Comparing `thorpy-2.0.5/thorpy/__init__.py` & `thorpy-2.0.6/thorpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #Import styling functions
 from .themes import theme_classic, theme_human, theme_round, theme_simple, theme_text, theme_game2
 from .themes import theme_round_gradient, theme_round2
 from .themes import theme_text_dark, theme_game1, set_style_attr, refresh_all_elements_style, get_theme_bck_color, get_theme_main_bck_color
 from .styles import get_default_font, set_default_font, get_text_size, get_text_height
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 def set_screen(screen):
     """Set the default surface display for all elements that will be created after this call."""
     parameters.screen = screen
 
 def get_screen():
     """Get the default surface display for elements that will be created after this call."""
```

### Comparing `thorpy-2.0.5/thorpy/canonical.py` & `thorpy-2.0.6/thorpy/canonical.py`

 * *Files 3% similar despite different names*

```diff
@@ -355,19 +355,21 @@
         """
         dx = 0 if x is None else x-self.rect.centerx
         dy = 0 if y is None else y-self.rect.centery
         self.move(dx, dy)
 
     def center_on(self, what):
         """Centers the element on another, or on a pygame Surface or Rect.
-        <what> : either a pygame Rect, a pygame Surface or a thorpy element.
+        <what> : either a pygame Rect, a 2-tuple, a pygame Surface or a thorpy element.
         It is also possible to specify what = 'screen' as a shortcut for screen's rect.
         """
         if isinstance(what, str):
             rect = p.screen.get_rect()
+        elif isinstance(what, tuple):
+            rect = pygame.Rect(what, (0,0))
         elif not isinstance(what, pygame.Rect): #works both for surfaces and elements.
             rect = what.get_rect()
         else:
             rect = what
         self.set_center(*rect.center)
 
     def stick_to(self, other, self_side, other_side, delta=(0,0), move_x=True, move_y=True):
@@ -385,14 +387,15 @@
             other = p.screen
         if not isinstance(other, pygame.Rect):
             other = other.get_rect()
         x0,y0 = sorting.get_side_center(self.rect, self_side)
         x1,y1 = sorting.get_side_center(other, other_side)
         self.move((x1-x0+delta[0])*move_x, (y1-y0+delta[1])*move_y)
 
+
     def englobe_children(self, margins=(5,5), adapt_parent=True, size_limit=(float("inf"), float("inf"))):
         """Resizes the element so that its size englobes that of its children.
         ***Optional arguments***
         <margins> : space between self's border and its children.
         <adapt_parent> : (bool) if False, parent of self won't be adapted accordingly.
         <size_limit> : (2-tuple) specifying the maximum width and height of the new size.
         """
@@ -431,27 +434,61 @@
                     self.styles[key].font_auto_multilines_width = w
         if self.state != "unactive": #self.styles[self.state]: #e.g. ghost has no style
             self.generate_surfaces()
         self.rect.center = center
         if adapt_parent and self.parent:
             self.parent.resort()
 
-    def rotate(self, angle, states="all"):
-        """Rotate the images of the element.
+    def rotate(self, angle, also_children=True, states="all", reactivate_surface_copy=True):
+        """Rotate the images of the element. Experimental, be cautious !
+        In most cases, only angles that are multiple of 90 degrees will yield fancy results.
+        Important note: as for now, element's shadows are not rotated. 
         ***Mandatory arguments***
         <angle> : the angle of rotation in degrees.
-        <states> : the states affected (either a list of strings or a specific state name or 'all')"""
+        ***Optional arguments***
+        <also_children> : if True, recursively rotates the children elements (for grouping rotation).
+        <states> : the states affected (either a list of strings or a specific state name or 'all')
+        <reactivate_surface_copy> : if needed, reactivate surface copy (for memory savings) if True.
+        """
+        if also_children:
+            self.rotate_recursive(angle, states, reactivate_surface_copy)
+            return
+        ################################################################
+        deactivated_copy = False
+        if self.has_copied_normal_state:
+            self.copy_normal_state(False)
+            self.refresh_surfaces()
+            deactivated_copy = True
+        second_draw_reactivations = {}
+        # Actual function ##############################################
         states = self.get_states_names(states)
         for state in states:
+            style = self.get_style(state)
+            if style:
+                if style.has_second_draw:
+                    self.set_style_attr("has_second_draw",False,refresh=True)
+                    second_draw_reactivations[style] = True
             for i in range(len(self.surfaces[state])):
                 surface = self.surfaces[state][i]
                 new_surface = pygame.transform.rotate(surface, angle)
                 self.surfaces[state][i] = new_surface
-                print("rotating", state, new_surface.get_rect())
+        ################################################################
         self.rect = self.get_rect()
+        if deactivated_copy and reactivate_surface_copy:
+            self.copy_normal_state(True)
+        for state in second_draw_reactivations.keys():
+            self.set_style_attr("has_second_draw",True,refresh=False)
+
+
+    def rotate_recursive(self, angle, states, reactivate_surface_copy):
+        positions = [c.rect.center for c in self.get_all_descendants()]
+        new_positions = rotate_points(positions, positions[0], angle)
+        for i,c in enumerate(self.get_all_descendants()):
+            c.rotate(angle, False, states)
+            c.set_center(*new_positions[i])
 
     def get_current_width(self):
         """Returns the width of the element using its current state."""
         return self.get_current_frame().get_width()
 
     def get_current_height(self):
         """Returns the height of the element using its current state."""
@@ -697,15 +734,15 @@
         states = []
         for c in self.children:
             states += c.lock_all_and_get_states()
         states += [(self, self.state)]
         self.state = "locked"
         return states
     
-    def get_children_rect(self, margins):
+    def get_children_rect(self, margins=(0,0)):
         r = self.children[0].rect.unionall([e.rect for e in self.children if not e.ignore_for_sorting])
         r.inflate_ip((margins[0]*2, margins[1]*2))
         return r
 
     def get_rect_with_children(self):
         if self.children:
             return self.rect.unionall([e.rect for e in self.children if not e.ignore_for_sorting])
@@ -978,14 +1015,16 @@
         <only_normal> : (bool) if False, surfaces are build for each state separately.
         """
         if only_normal:
             self.refresh_surfaces = self.refresh_surfaces_copy
         else:
             self.refresh_surfaces = self.refresh_surfaces_build
 
+    def has_copied_normal_state(self):
+        return self.refresh_surfaces is self.refresh_surfaces_copy
 
     def generate_shadow(self, fast="auto", shadowgen=None, states="all", uniform=False):
         """Generates a shadow and binds it to the element. This function is not meant to be called within the app loop, but only at initialization.
         ***Optional arguments***
         <fast> : (bool) if True, will generate a rectangular shadow whatever the element's shape is. Otherwise,
         this may be slow. You can also pass 'auto' : in this case, you let Thorpy choose whether the computing time
         is acceptable and automatically set fast to False if needed.
@@ -1012,25 +1051,33 @@
         self.get_current_frame = self.get_current_frame_normal
                 
     "#--- Children management ---#"
 
     def add_child(self, element, i=-1):
         """Add a child to the element.
         ***Mandatory arguments***
-        <element> : the children element to add.
+        <element> : the child element to add.
         ***Optional arguments***
         <i> : (integer) where in the list of children the new one should be added.
         By default -1 : it goes to the end.
         """
         element.parent = self
         if i < 0:
             self.children.append(element)
         else:
             self.children.insert(i, element)
 
+    def add_children(self, elements):
+        """Add children to the element.
+        ***Mandatory arguments***
+        <elements> : (list) the children elements to add.
+        """
+        for e in elements:
+            self.add_child(e)
+
     def remove_child(self, element):
         """Remove a child to the element.
         <element> : the children element to add.
         """
         element.parent = None
         self.children.remove(element)
 
@@ -1058,15 +1105,15 @@
         Returns the element itself if it has no parent."""
         if self.parent:
             return self.parent.root()
         else:
             return self
     
     def get_all_descendants(self):
-        """Returns all the descendants of the elements,
+        """Returns all the descendants of the elements, including self,
         i.e. its children, the children of its children and so on."""
         d = [self]
         for e in self.children:
             d += e.get_all_descendants()
         return d
     
     
@@ -1168,8 +1215,30 @@
         <adapt_cursor_style> : (bool) if True, mouse cursor will appear as a hand when hovering the element.
         """
         self.draggable_x = x_axis
         self.draggable_y = y_axis
         self.cannot_drag_outside = cannot_drag_outside
         self.cannot_draw_outside = cannot_draw_outside
         if adapt_cursor_style and (self.draggable_x or self.draggable_y):
-            self.hand_cursor = True
+            self.hand_cursor = True
+
+
+import math
+
+def rotate_points(points, center, angle):
+    angle = math.radians(angle)  # convert degrees to radians
+    cos_val = math.cos(angle)
+    sin_val = math.sin(angle)
+    cx, cy = center
+    rotated_points = []
+    for (x, y) in points:
+        # Translate point back to origin:
+        x -= cx
+        y -= cy
+        # Rotate point
+        x_new = (x * cos_val) - (y * sin_val)
+        y_new = (x * sin_val) + (y * cos_val)
+        # Translate point back:
+        x = x_new + cx
+        y = y_new + cy
+        rotated_points.append((x, y))
+    return rotated_points
```

### Comparing `thorpy-2.0.5/thorpy/elements.py` & `thorpy-2.0.6/thorpy/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import os, sys, inspect
 import pygame
 from . import styles, loops
 from . import parameters as p
 from .graphics import darken, enlighten
 from . import graphics
 from .canonical import Element
+from . import sorting
 import pygame.gfxdraw as gfx
 from .styles import get_text_height, get_text_size
 from .shadows import auto_set_fast
 
 sys.path.insert(0, "./")
 
 cursor_ibeam = pygame.cursors.Cursor(pygame.SYSTEM_CURSOR_IBEAM)
@@ -184,14 +185,33 @@
     def __init__(self, elements, mode="v", margins=(5,0), gap=5, nx="auto", ny="auto", align="center"):
         super().__init__(elements)
         if mode is not None:
             self.sort_children(mode,margins=margins,gap=gap,nx=nx,ny=ny,align=align)
             self.center_on(p.screen)
         self.copy_normal_state(True)
 
+    def stick_to(self, other, self_side, other_side, delta=(0,0), move_x=True, move_y=True):
+        """Sticks the element to another.
+        ***Mandatory arguments***
+        <other> : another element or pygame surface.
+        <self_side> : side of the element beeing sticked. Can be 'left', 'right', 'top' or 'bottom'.
+        <other_side> : side of the other element. Can be 'left', 'right', 'top' or 'bottom'.
+        ***Optional arguments***
+        <delta> : 2-tuple delta (pixels) to apply after the element has been moved.
+        <move_x> : (bool) set to False if x-axis movement should be ignored.
+        <move_y> : (bool) set to False if y-axis movement should be ignored.
+        """
+        if isinstance(other, str):
+            other = p.screen
+        if not isinstance(other, pygame.Rect):
+            other = other.get_rect()
+        x0,y0 = sorting.get_side_center(self.get_children_rect(), self_side)
+        x1,y1 = sorting.get_side_center(other, other_side)
+        self.move((x1-x0+delta[0])*move_x, (y1-y0+delta[1])*move_y)
+
 class Text(Button):
     """Text that can be used as a GUI element taking all standard element states
     (normal, hover, pressed, locked) and actions.
     ***Mandatory arguments***
     <text> : the text content. Can include line breaks.
     ***Optional arguments***
     <font_size> : size of the font (integer).
```

### Comparing `thorpy-2.0.5/thorpy/examples/_example_alert.py` & `thorpy-2.0.6/thorpy/examples/_example_alert.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_anim_move.py` & `thorpy-2.0.6/thorpy/examples/_example_anim_move.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_animatedgif.py` & `thorpy-2.0.6/thorpy/examples/_example_animatedgif.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_box.py` & `thorpy-2.0.6/thorpy/examples/_example_box.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_button_helloworld.py` & `thorpy-2.0.6/thorpy/examples/_example_button_helloworld.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_color_gradient.py` & `thorpy-2.0.6/thorpy/examples/_example_color_gradient.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_colorpicker.py` & `thorpy-2.0.6/thorpy/examples/_example_colorpicker.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_colorpicker2.py` & `thorpy-2.0.6/thorpy/examples/_example_colorpicker2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_colorpicker_fine_tuning.py` & `thorpy-2.0.6/thorpy/examples/_example_colorpicker_fine_tuning.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_create_style.py` & `thorpy-2.0.6/thorpy/examples/_example_create_style.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_create_style2.py` & `thorpy-2.0.6/thorpy/examples/_example_create_style2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_custom_theme.py` & `thorpy-2.0.6/thorpy/examples/_example_custom_theme.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_dropdownlist.py` & `thorpy-2.0.6/thorpy/examples/_example_dropdownlist.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_events.py` & `thorpy-2.0.6/thorpy/examples/_example_events.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_filebrowser.py` & `thorpy-2.0.6/thorpy/examples/_example_filebrowser.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_fx_light_emitting_image.py` & `thorpy-2.0.6/thorpy/examples/_example_fx_light_emitting_image.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_fx_lights.py` & `thorpy-2.0.6/thorpy/examples/_example_fx_lights.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_get_value_from_elements.py` & `thorpy-2.0.6/thorpy/examples/_example_get_value_from_elements.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_grouping.py` & `thorpy-2.0.6/thorpy/examples/_example_grouping.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_grouping_without_sorting.py` & `thorpy-2.0.6/thorpy/examples/_example_grouping_without_sorting.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_groups_of_groups.py` & `thorpy-2.0.6/thorpy/examples/_example_groups_of_groups.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_guess_the_number.py` & `thorpy-2.0.6/thorpy/examples/_example_guess_the_number.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_helper.py` & `thorpy-2.0.6/thorpy/examples/_example_helper.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_heterogeneous_texts.py` & `thorpy-2.0.6/thorpy/examples/_example_heterogeneous_texts.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_image_with_text.py` & `thorpy-2.0.6/thorpy/examples/_example_image_with_text.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_imagebutton.py` & `thorpy-2.0.6/thorpy/examples/_example_imagebutton.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_integration_in_existing_code.py` & `thorpy-2.0.6/thorpy/examples/_example_integration_in_existing_code.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_labels.py` & `thorpy-2.0.6/thorpy/examples/_example_labels.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_launch.py` & `thorpy-2.0.6/thorpy/examples/_example_launch.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_lifebar.py` & `thorpy-2.0.6/thorpy/examples/_example_lifebar.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_look_tune.py` & `thorpy-2.0.6/thorpy/examples/_example_look_tune.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_rich_text.py` & `thorpy-2.0.6/thorpy/examples/_example_rich_text.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_set_default_font.py` & `thorpy-2.0.6/thorpy/examples/_example_set_default_font.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_shadows.py` & `thorpy-2.0.6/thorpy/examples/_example_shadows.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_showcase_themes.py` & `thorpy-2.0.6/thorpy/examples/_example_showcase_themes.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_showcase_themes2.py` & `thorpy-2.0.6/thorpy/examples/_example_showcase_themes2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_showcase_themes_buttons.py` & `thorpy-2.0.6/thorpy/examples/_example_showcase_themes_buttons.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_showfps.py` & `thorpy-2.0.6/thorpy/examples/_example_showfps.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_slider.py` & `thorpy-2.0.6/thorpy/examples/_example_slider.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_text_input.py` & `thorpy-2.0.6/thorpy/examples/_example_text_input.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_text_width.py` & `thorpy-2.0.6/thorpy/examples/_example_text_width.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_togglables_pool.py` & `thorpy-2.0.6/thorpy/examples/_example_togglables_pool.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_user_choices.py` & `thorpy-2.0.6/thorpy/examples/_example_user_choices.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_user_choices2.py` & `thorpy-2.0.6/thorpy/examples/_example_user_choices2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_user_chooses_font.py` & `thorpy-2.0.6/thorpy/examples/_example_user_chooses_font.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/examples/_example_waiting_bar.py` & `thorpy-2.0.6/thorpy/examples/_example_waiting_bar.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/gametools.py` & `thorpy-2.0.6/thorpy/gametools.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/graphics.py` & `thorpy-2.0.6/thorpy/graphics.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/loops.py` & `thorpy-2.0.6/thorpy/loops.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/monitoring.py` & `thorpy-2.0.6/thorpy/monitoring.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/setup.py` & `thorpy-2.0.6/thorpy/setup.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/shadows.py` & `thorpy-2.0.6/thorpy/shadows.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/sorting.py` & `thorpy-2.0.6/thorpy/sorting.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/sound.py` & `thorpy-2.0.6/thorpy/sound.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/styles.py` & `thorpy-2.0.6/thorpy/styles.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.5/thorpy/themes.py` & `thorpy-2.0.6/thorpy/themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -596,14 +596,15 @@
     #Colorpickers
     apply_default_colorpickers()
     #
     assign_styles()
 
 def theme_game2():
     p.current_theme = "game2"
+    theme_classic()
     #Button
     base_style = styles.RoundStyle
     Button.style_normal = base_style()
     Button.style_normal.radius = 0
     Button.style_normal.border_thickness = 2
     # Button.style_normal.bck_color = (220,220,220,127)
     alpha = 180
```

### Comparing `thorpy-2.0.5/thorpy.egg-info/SOURCES.txt` & `thorpy-2.0.6/thorpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 thorpy/examples/_example_imagebutton.py
 thorpy/examples/_example_integration_in_existing_code.py
 thorpy/examples/_example_labels.py
 thorpy/examples/_example_launch.py
 thorpy/examples/_example_lifebar.py
 thorpy/examples/_example_look_tune.py
 thorpy/examples/_example_rich_text.py
+thorpy/examples/_example_rotations.py
 thorpy/examples/_example_set_default_font.py
 thorpy/examples/_example_shadows.py
 thorpy/examples/_example_showcase_themes.py
 thorpy/examples/_example_showcase_themes2.py
 thorpy/examples/_example_showcase_themes_buttons.py
 thorpy/examples/_example_showfps.py
 thorpy/examples/_example_slider.py
```

