# Comparing `tmp/asammdf-7.3.8.tar.gz` & `tmp/asammdf-7.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asammdf-7.3.8.tar", last modified: Wed Mar 29 08:07:44 2023, max compression
+gzip compressed data, was "asammdf-7.3.9.tar", last modified: Fri Mar 31 05:54:19 2023, max compression
```

## Comparing `asammdf-7.3.8.tar` & `asammdf-7.3.9.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:44.342458 asammdf-7.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-03-29 08:07:30.000000 asammdf-7.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-29 08:07:30.000000 asammdf-7.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-03-29 08:07:44.342458 asammdf-7.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-03-29 08:07:30.000000 asammdf-7.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-29 08:07:30.000000 asammdf-7.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-29 08:07:30.000000 asammdf-7.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-29 08:07:44.342458 asammdf-7.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-03-29 08:07:30.000000 asammdf-7.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:44.294457 asammdf-7.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:44.298457 asammdf-7.3.8/src/asammdf/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:44.310457 asammdf-7.3.8/src/asammdf/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/bus_logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35487 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/cutils.c
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/mdf_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/mdf_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)   141470 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/mdf_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)   423467 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/mdf_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/source_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    70970 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   116192 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/v2_v3_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/v2_v3_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   235230 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/v4_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    20827 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/blocks/v4_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:44.310457 asammdf-7.3.8/src/asammdf/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/asammdfgui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:44.314457 asammdf-7.3.8/src/asammdf/gui/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/bus_database_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/channel_group_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/channel_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/conversion_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/define_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/error_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/functions_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/gps_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/multi_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/simple_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/dialogs/window_selection_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:44.334458 asammdf-7.3.8/src/asammdf/gui/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/attachment.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/bar.ui
--rw-r--r--   0 runner    (1001) docker     (123)    60675 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/batch_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    70050 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/batch_widget.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/bus_database_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/bus_database_manager.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/channel_bar_display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/channel_bar_display_widget.ui
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/channel_group_info_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/channel_group_info_widget.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/channel_info_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/channel_info_widget.ui
--rw-r--r--   0 runner    (1001) docker     (123)    39698 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/channel_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    44844 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/channel_stats.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/database_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/database_item.ui
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/define_channel_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/define_channel_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/define_conversion_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/define_conversion_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/error_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/error_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/fft_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/fft_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)    56553 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/file_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    66297 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/file_widget.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/functions_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/functions_manager.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/gps.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/gps_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/gps_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/multi_search_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/multi_search_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/numeric_offline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/numeric_offline.ui
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/numeric_online.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/range_editor_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/range_editor_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/range_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/range_widget.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/resource.qrc
--rw-r--r--   0 runner    (1001) docker     (123)   587997 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/resource_rc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/search_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/search_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/signal_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/signal_scale.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/simple_search_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/simple_search_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/tabular.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/tabular_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/tabular_filter.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/values_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/values_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/vrtt_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/vrtt_widget.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/vtt_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/vtt_widget.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/windows_selection_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/ui/windows_selection_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    35975 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:44.342458 asammdf-7.3.8/src/asammdf/gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    69922 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/bus_database_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/can_bus_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/channel_bar_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/channel_group_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/channel_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/channel_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/collapsiblebox.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/database_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/dict_to_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/fft_window.py
--rw-r--r--   0 runner    (1001) docker     (123)   110061 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/flexray_bus_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/formated_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/functions_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/lin_bus_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    20292 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/main.py
--rw-r--r--   0 runner    (1001) docker     (123)   155530 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/mdi_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    58171 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)   222324 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    23811 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/plot_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/python_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/range_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/signal_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    88016 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/tabular_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/tabular_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    78990 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/tree_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/tree_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/viewbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/vrtt_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/gui/widgets/vtt_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)   237064 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/mdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    54245 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-29 08:07:30.000000 asammdf-7.3.8/src/asammdf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:44.302457 asammdf-7.3.8/src/asammdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-03-29 08:07:44.000000 asammdf-7.3.8/src/asammdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-03-29 08:07:44.000000 asammdf-7.3.8/src/asammdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:07:44.000000 asammdf-7.3.8/src/asammdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-29 08:07:44.000000 asammdf-7.3.8/src/asammdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-29 08:07:44.000000 asammdf-7.3.8/src/asammdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-29 08:07:44.000000 asammdf-7.3.8/src/asammdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:07:44.342458 asammdf-7.3.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-03-29 08:07:30.000000 asammdf-7.3.8/test/test_CAN_bus_loogging.py
--rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-03-29 08:07:30.000000 asammdf-7.3.8/test/test_endianess.py
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-03-29 08:07:30.000000 asammdf-7.3.8/test/test_mdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-03-29 08:07:30.000000 asammdf-7.3.8/test/test_mdf23.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-03-29 08:07:30.000000 asammdf-7.3.8/test/test_mdf4.py
--rw-r--r--   0 runner    (1001) docker     (123)    20781 2023-03-29 08:07:30.000000 asammdf-7.3.8/test/test_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:19.672484 asammdf-7.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-03-31 05:54:06.000000 asammdf-7.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-31 05:54:06.000000 asammdf-7.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-03-31 05:54:19.672484 asammdf-7.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-03-31 05:54:06.000000 asammdf-7.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-31 05:54:06.000000 asammdf-7.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 05:54:06.000000 asammdf-7.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-31 05:54:19.676484 asammdf-7.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-03-31 05:54:06.000000 asammdf-7.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:19.596480 asammdf-7.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:19.604480 asammdf-7.3.9/src/asammdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:19.616481 asammdf-7.3.9/src/asammdf/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/bus_logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/conversion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35487 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/cutils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/mdf_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/mdf_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141470 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/mdf_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   423467 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/mdf_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/source_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71170 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116384 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/v2_v3_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/v2_v3_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)   235230 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/v4_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20827 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/blocks/v4_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:19.616481 asammdf-7.3.9/src/asammdf/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/asammdfgui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:19.624481 asammdf-7.3.9/src/asammdf/gui/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17983 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/bus_database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/channel_group_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/channel_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/conversion_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/define_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/error_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/functions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/gps_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/multi_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/simple_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/dialogs/window_selection_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:19.656483 asammdf-7.3.9/src/asammdf/gui/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/attachment.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/bar.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    60675 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/batch_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70050 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/batch_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/bus_database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/bus_database_manager.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/channel_bar_display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/channel_bar_display_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/channel_group_info_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/channel_group_info_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/channel_info_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/channel_info_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    39698 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/channel_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44844 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/channel_stats.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/database_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/database_item.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/define_channel_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/define_channel_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/define_conversion_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/define_conversion_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/error_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/error_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/fft_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/fft_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    56553 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/file_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66297 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/file_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/functions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/functions_manager.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/gps.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/gps_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/gps_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/multi_search_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/multi_search_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/numeric_offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/numeric_offline.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/numeric_online.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/range_editor_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/range_editor_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/range_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/range_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/resource.qrc
+-rw-r--r--   0 runner    (1001) docker     (123)   587997 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/resource_rc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/search_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/search_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/signal_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/signal_scale.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/simple_search_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/simple_search_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/tabular.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/tabular_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/tabular_filter.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/values_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/values_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/vrtt_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/vrtt_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/vtt_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/vtt_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/windows_selection_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/ui/windows_selection_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    35975 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:19.672484 asammdf-7.3.9/src/asammdf/gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69922 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/bus_database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/can_bus_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/channel_bar_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/channel_group_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/channel_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/channel_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/collapsiblebox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/database_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/dict_to_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/fft_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110061 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/flexray_bus_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/formated_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/functions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/lin_bus_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20292 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155530 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/mdi_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58171 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222324 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23811 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/plot_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/python_highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/range_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/signal_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88016 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/tabular_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/tabular_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78990 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/tree_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/tree_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/viewbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/vrtt_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/gui/widgets/vtt_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)   237064 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/mdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54245 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-31 05:54:06.000000 asammdf-7.3.9/src/asammdf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:19.608481 asammdf-7.3.9/src/asammdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-03-31 05:54:19.000000 asammdf-7.3.9/src/asammdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-03-31 05:54:19.000000 asammdf-7.3.9/src/asammdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 05:54:19.000000 asammdf-7.3.9/src/asammdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-31 05:54:19.000000 asammdf-7.3.9/src/asammdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-31 05:54:19.000000 asammdf-7.3.9/src/asammdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-31 05:54:19.000000 asammdf-7.3.9/src/asammdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:54:19.672484 asammdf-7.3.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-03-31 05:54:06.000000 asammdf-7.3.9/test/test_CAN_bus_loogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-03-31 05:54:06.000000 asammdf-7.3.9/test/test_endianess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-03-31 05:54:06.000000 asammdf-7.3.9/test/test_mdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-03-31 05:54:06.000000 asammdf-7.3.9/test/test_mdf23.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-03-31 05:54:06.000000 asammdf-7.3.9/test/test_mdf4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20781 2023-03-31 05:54:06.000000 asammdf-7.3.9/test/test_signal.py
```

### Comparing `asammdf-7.3.8/LICENSE` & `asammdf-7.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/PKG-INFO` & `asammdf-7.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asammdf
-Version: 7.3.8
+Version: 7.3.9
 Summary: ASAM MDF measurement data file parser
 Home-page: https://github.com/danielhrisca/asammdf
 Author: Daniel Hrisca
 Author-email: daniel.hrisca@gmail.com
 License: LGPLv3+
 Keywords: read reader edit editor parse parser asam mdf measurement
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `asammdf-7.3.8/README.md` & `asammdf-7.3.9/README.md`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/pyproject.toml` & `asammdf-7.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/setup.cfg` & `asammdf-7.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/setup.py` & `asammdf-7.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/__init__.py` & `asammdf-7.3.9/src/asammdf/__init__.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/bus_logging_utils.py` & `asammdf-7.3.9/src/asammdf/blocks/bus_logging_utils.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/conversion_utils.py` & `asammdf-7.3.9/src/asammdf/blocks/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/cutils.c` & `asammdf-7.3.9/src/asammdf/blocks/cutils.c`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/mdf_common.py` & `asammdf-7.3.9/src/asammdf/blocks/mdf_common.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/mdf_v2.py` & `asammdf-7.3.9/src/asammdf/blocks/mdf_v2.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/mdf_v3.py` & `asammdf-7.3.9/src/asammdf/blocks/mdf_v3.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/mdf_v4.py` & `asammdf-7.3.9/src/asammdf/blocks/mdf_v4.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/options.py` & `asammdf-7.3.9/src/asammdf/blocks/options.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/source_utils.py` & `asammdf-7.3.9/src/asammdf/blocks/source_utils.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/utils.py` & `asammdf-7.3.9/src/asammdf/blocks/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -468,14 +468,17 @@
         else:
             fmt = f"({size},)u1"
     else:
         if size > 64 and data_type in (
             v3c.DATA_TYPE_UNSIGNED_INTEL,
             v3c.DATA_TYPE_UNSIGNED,
             v3c.DATA_TYPE_UNSIGNED_MOTOROLA,
+            v3c.DATA_TYPE_SIGNED_INTEL,
+            v3c.DATA_TYPE_SIGNED,
+            v3c.DATA_TYPE_SIGNED_MOTOROLA,
         ):
             fmt = f"({size // 8},)u1"
         else:
             if size <= 8:
                 size = 1
             elif size <= 16:
                 size = 2
@@ -597,14 +600,16 @@
         elif data_type == v4c.DATA_TYPE_COMPLEX_MOTOROLA:
             fmt = ">c8"
 
     else:
         if size > 64 and data_type in (
             v4c.DATA_TYPE_UNSIGNED_INTEL,
             v4c.DATA_TYPE_UNSIGNED_MOTOROLA,
+            v4c.DATA_TYPE_SIGNED_INTEL,
+            v4c.DATA_TYPE_SIGNED_MOTOROLA,
         ):
             fmt = f"({size // 8},)u1"
         else:
             if size <= 8:
                 size = 1
             elif size <= 16:
                 size = 2
```

### Comparing `asammdf-7.3.8/src/asammdf/blocks/v2_v3_blocks.py` & `asammdf-7.3.9/src/asammdf/blocks/v2_v3_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -2946,45 +2946,48 @@
         Returns
         -------
         timestamp : datetime.datetime
             start timestamp
 
         """
 
-        if self.block_len > v23c.HEADER_COMMON_SIZE:
-            if self.abs_time:
-                timestamp = self.abs_time / 10**9
-
-                tz = timezone(timedelta(hours=self.tz_offset))
-
-                try:
-                    timestamp = datetime.fromtimestamp(timestamp, tz)
-                except OverflowError:
-                    timestamp = datetime.fromtimestamp(0, tz) + timedelta(
-                        seconds=timestamp
+        try:
+            if self.block_len > v23c.HEADER_COMMON_SIZE:
+                if self.abs_time:
+                    timestamp = self.abs_time / 10**9
+
+                    tz = timezone(timedelta(hours=self.tz_offset))
+
+                    try:
+                        timestamp = datetime.fromtimestamp(timestamp, tz)
+                    except OverflowError:
+                        timestamp = datetime.fromtimestamp(0, tz) + timedelta(
+                            seconds=timestamp
+                        )
+                    except OSError:
+                        timestamp = datetime.now(tz)
+                else:
+                    timestamp = "{} {}".format(
+                        self.date.decode("ascii"), self.time.decode("ascii")
                     )
-                except OSError:
-                    timestamp = datetime.now(tz)
+
+                    timestamp = datetime.strptime(
+                        timestamp, "%d:%m:%Y %H:%M:%S"
+                    ).astimezone(timezone.utc)
+
             else:
                 timestamp = "{} {}".format(
                     self.date.decode("ascii"), self.time.decode("ascii")
                 )
 
                 timestamp = datetime.strptime(
                     timestamp, "%d:%m:%Y %H:%M:%S"
                 ).astimezone(timezone.utc)
-
-        else:
-            timestamp = "{} {}".format(
-                self.date.decode("ascii"), self.time.decode("ascii")
-            )
-
-            timestamp = datetime.strptime(timestamp, "%d:%m:%Y %H:%M:%S").astimezone(
-                timezone.utc
-            )
+        except:
+            return datetime.now().astimezone(timezone.utc)
 
         return timestamp
 
     @start_time.setter
     def start_time(self, timestamp: datetime) -> None:
         if timestamp.tzinfo is None:
             # the user provided a naive datetime
```

### Comparing `asammdf-7.3.8/src/asammdf/blocks/v2_v3_constants.py` & `asammdf-7.3.9/src/asammdf/blocks/v2_v3_constants.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/v4_blocks.py` & `asammdf-7.3.9/src/asammdf/blocks/v4_blocks.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/blocks/v4_constants.py` & `asammdf-7.3.9/src/asammdf/blocks/v4_constants.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/asammdfgui.py` & `asammdf-7.3.9/src/asammdf/gui/asammdfgui.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/advanced_search.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/advanced_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                 pattern = re.compile(f"(?i){text}")
 
             try:
                 if extened_search:
                     matches = {}
 
                     for group_index, group in enumerate(self.mdf.groups):
-                        cg_source = group.channel_group.acq_source
+                        cg_source = getattr(group.channel_group, "acq_source", None)
 
                         # check channel group source name
 
                         if cg_source and (
                             match_kind == "Wildcard"
                             and (
                                 fnmatch((cg_source.name or "").casefold(), pattern)
@@ -253,15 +253,15 @@
                             if entry not in matches:
                                 (group_index, channel_index) = entry
                                 ch = self.mdf.groups[group_index].channels[
                                     channel_index
                                 ]
                                 cg = self.mdf.groups[group_index].channel_group
 
-                                source = ch.source or cg.acq_source
+                                source = ch.source or getattr(cg, "acq_source", None)
 
                                 matches[entry] = {
                                     "names": [],
                                     "comment": extract_xml_comment(ch.comment).strip(),
                                     "unit": ch.conversion
                                     and ch.conversion.unit
                                     or ch.unit,
```

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/bus_database_manager.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/bus_database_manager.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/channel_group_info.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/channel_group_info.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/channel_info.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/channel_info.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/conversion_editor.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/conversion_editor.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/define_channel.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/define_channel.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/error_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/error_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/functions_manager.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/functions_manager.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/gps_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/gps_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/multi_search.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/multi_search.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/range_editor.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/range_editor.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/simple_search.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/simple_search.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/dialogs/window_selection_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/dialogs/window_selection_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/plot.py` & `asammdf-7.3.9/src/asammdf/gui/plot.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/attachment.py` & `asammdf-7.3.9/src/asammdf/gui/ui/attachment.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/attachment.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/attachment.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/bar.py` & `asammdf-7.3.9/src/asammdf/gui/ui/bar.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/bar.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/bar.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/batch_widget.py` & `asammdf-7.3.9/src/asammdf/gui/ui/batch_widget.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/batch_widget.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/batch_widget.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/bus_database_manager.py` & `asammdf-7.3.9/src/asammdf/gui/ui/bus_database_manager.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/bus_database_manager.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/bus_database_manager.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/channel_bar_display_widget.py` & `asammdf-7.3.9/src/asammdf/gui/ui/channel_bar_display_widget.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/channel_bar_display_widget.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/channel_bar_display_widget.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/channel_group_info_widget.py` & `asammdf-7.3.9/src/asammdf/gui/ui/channel_group_info_widget.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/channel_group_info_widget.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/channel_group_info_widget.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/channel_info_widget.py` & `asammdf-7.3.9/src/asammdf/gui/ui/channel_info_widget.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/channel_info_widget.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/channel_info_widget.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/channel_stats.py` & `asammdf-7.3.9/src/asammdf/gui/ui/channel_stats.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/channel_stats.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/channel_stats.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/database_item.py` & `asammdf-7.3.9/src/asammdf/gui/ui/database_item.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/database_item.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/database_item.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/define_channel_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/ui/define_channel_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/define_channel_dialog.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/define_channel_dialog.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/define_conversion_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/ui/define_conversion_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/define_conversion_dialog.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/define_conversion_dialog.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/error_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/ui/error_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/error_dialog.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/error_dialog.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/fft_window.py` & `asammdf-7.3.9/src/asammdf/gui/ui/fft_window.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/fft_window.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/fft_window.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/file_widget.py` & `asammdf-7.3.9/src/asammdf/gui/ui/file_widget.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/file_widget.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/file_widget.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/functions_manager.py` & `asammdf-7.3.9/src/asammdf/gui/ui/functions_manager.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/functions_manager.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/functions_manager.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/gps.py` & `asammdf-7.3.9/src/asammdf/gui/ui/gps.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/gps.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/gps.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/gps_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/ui/gps_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/gps_dialog.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/gps_dialog.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/main_window.py` & `asammdf-7.3.9/src/asammdf/gui/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/main_window.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/multi_search_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/ui/multi_search_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/multi_search_dialog.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/multi_search_dialog.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/numeric.py` & `asammdf-7.3.9/src/asammdf/gui/ui/numeric.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/numeric_offline.py` & `asammdf-7.3.9/src/asammdf/gui/ui/numeric_offline.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/numeric_offline.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/numeric_offline.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/numeric_online.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/numeric_online.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/range_editor_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/ui/range_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/range_editor_dialog.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/range_editor_dialog.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/range_widget.py` & `asammdf-7.3.9/src/asammdf/gui/ui/range_widget.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/range_widget.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/range_widget.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/resource.qrc` & `asammdf-7.3.9/src/asammdf/gui/ui/resource.qrc`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/resource_rc.py` & `asammdf-7.3.9/src/asammdf/gui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/search_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/ui/search_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/search_dialog.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/search_dialog.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/signal_scale.py` & `asammdf-7.3.9/src/asammdf/gui/ui/signal_scale.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/signal_scale.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/signal_scale.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/simple_search_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/ui/simple_search_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/simple_search_dialog.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/simple_search_dialog.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/tabular.py` & `asammdf-7.3.9/src/asammdf/gui/ui/tabular.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/tabular.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/tabular.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/tabular_filter.py` & `asammdf-7.3.9/src/asammdf/gui/ui/tabular_filter.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/tabular_filter.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/tabular_filter.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/values_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/ui/values_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/values_dialog.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/values_dialog.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/vrtt_widget.py` & `asammdf-7.3.9/src/asammdf/gui/ui/vrtt_widget.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/vrtt_widget.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/vrtt_widget.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/vtt_widget.py` & `asammdf-7.3.9/src/asammdf/gui/ui/vtt_widget.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/vtt_widget.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/vtt_widget.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/windows_selection_dialog.py` & `asammdf-7.3.9/src/asammdf/gui/ui/windows_selection_dialog.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/ui/windows_selection_dialog.ui` & `asammdf-7.3.9/src/asammdf/gui/ui/windows_selection_dialog.ui`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/utils.py` & `asammdf-7.3.9/src/asammdf/gui/utils.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/attachment.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/attachment.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/bar.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/bar.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/batch.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/batch.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/bus_database_manager.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/bus_database_manager.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/can_bus_trace.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/can_bus_trace.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/channel_bar_display.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/channel_bar_display.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/channel_group_info.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/channel_group_info.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/channel_info.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/channel_info.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/channel_stats.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/channel_stats.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/collapsiblebox.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/collapsiblebox.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/cursor.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/cursor.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/dict_to_tree.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/dict_to_tree.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/fft_window.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/fft_window.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/file.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/file.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/flexray_bus_trace.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/flexray_bus_trace.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/formated_axis.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/formated_axis.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/functions_manager.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/functions_manager.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/gps.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/gps.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,27 +52,23 @@
         self._timestamp = self._min
 
         self.timestamp.setRange(self._min, self._max)
         self.timestamp.setValue(self._min)
         self.min_t.setText(f"{self._min:.6f}s")
         self.max_t.setText(f"{self._max:.6f}s")
 
-        leaflet.core.Evented.mapWidget = None
-
         self.mapWidget = MapWidget()
         self.map_layout.insertWidget(0, self.mapWidget)
         self.map_layout.setStretch(0, 1)
 
         self.map = L.map(self.mapWidget)
 
         self.map.setView([50.1364092, 8.5991296], zoom)
 
-        L.tileLayer("https://{s}.tile.openstreetmap.fr/osmfr/{z}/{x}/{y}.png").addTo(
-            self.map
-        )
+        L.tileLayer("https://{s}.tile.osm.org/{z}/{x}/{y}.png").addTo(self.map)
 
         # L.tileLayer("https://{s}.tile.opentopomap.org/{z}/{x}/{y}.png").addTo(self.map)
 
         if len(timebase):
             line = L.polyline(
                 np.column_stack(
                     [self.latitude_signal.samples, self.longitude_signal.samples]
```

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/lin_bus_trace.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/lin_bus_trace.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/list.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/list.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/loader.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/loader.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/main.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/main.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/mdi_area.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/mdi_area.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/numeric.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/numeric.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/plot.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/plot.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/plot_standalone.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/plot_standalone.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/python_highlighter.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/python_highlighter.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/range_widget.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/range_widget.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/search.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/search.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/signal_scale.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/signal_scale.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/tabular.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/tabular.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/tabular_base.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/tabular_base.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/tabular_filter.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/tabular_filter.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/tree.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/tree_item.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/tree_item.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/tree_numeric.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/tree_numeric.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/viewbox.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/viewbox.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/vrtt_widget.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/vrtt_widget.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/gui/widgets/vtt_widget.py` & `asammdf-7.3.9/src/asammdf/gui/widgets/vtt_widget.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/mdf.py` & `asammdf-7.3.9/src/asammdf/mdf.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/signal.py` & `asammdf-7.3.9/src/asammdf/signal.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf/types.py` & `asammdf-7.3.9/src/asammdf/types.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/src/asammdf.egg-info/PKG-INFO` & `asammdf-7.3.9/src/asammdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asammdf
-Version: 7.3.8
+Version: 7.3.9
 Summary: ASAM MDF measurement data file parser
 Home-page: https://github.com/danielhrisca/asammdf
 Author: Daniel Hrisca
 Author-email: daniel.hrisca@gmail.com
 License: LGPLv3+
 Keywords: read reader edit editor parse parser asam mdf measurement
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `asammdf-7.3.8/src/asammdf.egg-info/SOURCES.txt` & `asammdf-7.3.9/src/asammdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/test/test_CAN_bus_loogging.py` & `asammdf-7.3.9/test/test_CAN_bus_loogging.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/test/test_endianess.py` & `asammdf-7.3.9/test/test_endianess.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/test/test_mdf.py` & `asammdf-7.3.9/test/test_mdf.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/test/test_mdf23.py` & `asammdf-7.3.9/test/test_mdf23.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/test/test_mdf4.py` & `asammdf-7.3.9/test/test_mdf4.py`

 * *Files identical despite different names*

### Comparing `asammdf-7.3.8/test/test_signal.py` & `asammdf-7.3.9/test/test_signal.py`

 * *Files identical despite different names*

