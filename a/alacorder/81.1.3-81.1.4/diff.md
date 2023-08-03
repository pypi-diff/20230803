# Comparing `tmp/alacorder-81.1.3.tar.gz` & `tmp/alacorder-81.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-81.1.3.tar", max compression
+gzip compressed data, was "alacorder-81.1.4.tar", max compression
```

## Comparing `alacorder-81.1.3.tar` & `alacorder-81.1.4.tar`

### file list

```diff
@@ -1,9 +1,1958 @@
--rw-r--r--   0        0        0     1067 2023-04-18 14:01:34.633926 alacorder-81.1.3/LICENSE
--rw-r--r--   0        0        0     4865 2023-07-25 18:33:12.479611 alacorder-81.1.3/README.md
--rw-r--r--   0        0        0       72 2023-07-29 19:00:48.870558 alacorder-81.1.3/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0       72 2023-07-31 16:52:36.121455 alacorder-81.1.3/alacorder/.ipynb_checkpoints/Untitled1-checkpoint.ipynb
--rw-r--r--   0        0        0       19 2023-07-25 19:20:19.054678 alacorder-81.1.3/alacorder/__init__.py
--rw-r--r--   0        0        0       59 2023-07-25 19:23:49.408885 alacorder-81.1.3/alacorder/__main__.py
--rw-r--r--   0        0        0   251145 2023-08-02 20:05:43.081253 alacorder-81.1.3/alacorder/alac.py
--rw-r--r--   0        0        0      557 2023-08-02 20:05:57.027823 alacorder-81.1.3/pyproject.toml
--rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 alacorder-81.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-18 14:01:34.633926 alacorder-81.1.4/LICENSE
+-rw-r--r--   0        0        0     4865 2023-07-25 18:33:12.479611 alacorder-81.1.4/README.md
+-rw-r--r--   0        0        0     6148 2023-07-31 22:32:12.260014 alacorder-81.1.4/alacorder/.DS_Store
+-rw-r--r--   0        0        0       72 2023-07-29 19:00:48.870558 alacorder-81.1.4/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2023-07-31 16:52:36.121455 alacorder-81.1.4/alacorder/.ipynb_checkpoints/Untitled1-checkpoint.ipynb
+-rw-r--r--   0        0        0       34 2023-07-27 22:51:55.510100 alacorder-81.1.4/alacorder/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-27 22:51:55.505923 alacorder-81.1.4/alacorder/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0     1517 2023-07-27 22:51:51.106830 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/__init__.data.json
+-rw-r--r--   0        0        0     1523 2023-07-27 22:51:51.107009 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/__init__.meta.json
+-rw-r--r--   0        0        0    12784 2023-07-27 22:51:54.008525 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/alias.data.json
+-rw-r--r--   0        0        0     1812 2023-07-27 22:51:54.008789 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/alias.meta.json
+-rw-r--r--   0        0        0     7684 2023-07-27 22:51:53.985250 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/async_helpers.data.json
+-rw-r--r--   0        0        0     1737 2023-07-27 22:51:53.985468 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/async_helpers.meta.json
+-rw-r--r--   0        0        0     5470 2023-07-27 22:51:51.070650 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/autocall.data.json
+-rw-r--r--   0        0        0     1535 2023-07-27 22:51:51.070836 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/autocall.meta.json
+-rw-r--r--   0        0        0     8029 2023-07-27 22:51:54.006284 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/builtin_trap.data.json
+-rw-r--r--   0        0        0     1796 2023-07-27 22:51:54.006485 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/builtin_trap.meta.json
+-rw-r--r--   0        0        0     8169 2023-07-27 22:51:52.060293 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/compilerop.data.json
+-rw-r--r--   0        0        0     1757 2023-07-27 22:51:52.060539 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/compilerop.meta.json
+-rw-r--r--   0        0        0    48003 2023-07-27 22:51:53.817532 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/display.data.json
+-rw-r--r--   0        0        0     2184 2023-07-27 22:51:53.817844 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/display.meta.json
+-rw-r--r--   0        0        0     7549 2023-07-27 22:51:52.106470 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/display_functions.data.json
+-rw-r--r--   0        0        0     1651 2023-07-27 22:51:52.106660 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/display_functions.meta.json
+-rw-r--r--   0        0        0     4730 2023-07-27 22:51:54.004764 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/display_trap.data.json
+-rw-r--r--   0        0        0     1810 2023-07-27 22:51:54.004977 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/display_trap.meta.json
+-rw-r--r--   0        0        0    14219 2023-07-27 22:51:54.003051 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/displayhook.data.json
+-rw-r--r--   0        0        0     1893 2023-07-27 22:51:54.003279 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/displayhook.meta.json
+-rw-r--r--   0        0        0     7067 2023-07-27 22:51:53.997223 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/displaypub.data.json
+-rw-r--r--   0        0        0     1831 2023-07-27 22:51:53.997450 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/displaypub.meta.json
+-rw-r--r--   0        0        0     5369 2023-07-27 22:51:51.069563 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/error.data.json
+-rw-r--r--   0        0        0     1529 2023-07-27 22:51:51.069739 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/error.meta.json
+-rw-r--r--   0        0        0     7907 2023-07-27 22:51:51.068642 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/events.data.json
+-rw-r--r--   0        0        0     1546 2023-07-27 22:51:51.068833 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/events.meta.json
+-rw-r--r--   0        0        0     2006 2023-07-27 22:51:52.009009 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/excolors.data.json
+-rw-r--r--   0        0        0     1576 2023-07-27 22:51:52.009209 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/excolors.meta.json
+-rw-r--r--   0        0        0     9526 2023-07-27 22:51:54.726747 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/extensions.data.json
+-rw-r--r--   0        0        0     1919 2023-07-27 22:51:54.726988 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/extensions.meta.json
+-rw-r--r--   0        0        0    93018 2023-07-27 22:51:53.995908 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/formatters.data.json
+-rw-r--r--   0        0        0     2167 2023-07-27 22:51:53.996171 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/formatters.meta.json
+-rw-r--r--   0        0        0     1613 2023-07-27 22:51:51.109642 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/getipython.data.json
+-rw-r--r--   0        0        0     1538 2023-07-27 22:51:51.109835 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/getipython.meta.json
+-rw-r--r--   0        0        0   121070 2023-07-27 22:51:51.992241 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/guarded_eval.data.json
+-rw-r--r--   0        0        0     1813 2023-07-27 22:51:51.992536 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/guarded_eval.meta.json
+-rw-r--r--   0        0        0     6332 2023-07-27 22:51:51.715857 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/hooks.data.json
+-rw-r--r--   0        0        0     1597 2023-07-27 22:51:51.716041 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/hooks.meta.json
+-rw-r--r--   0        0        0    39122 2023-07-27 22:51:52.057959 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/inputtransformer2.data.json
+-rw-r--r--   0        0        0     1680 2023-07-27 22:51:52.058218 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/inputtransformer2.meta.json
+-rw-r--r--   0        0        0     1995 2023-07-27 22:51:51.000758 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/latex_symbols.data.json
+-rw-r--r--   0        0        0     1570 2023-07-27 22:51:51.001016 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/latex_symbols.meta.json
+-rw-r--r--   0        0        0     8470 2023-07-27 22:51:51.714594 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/logger.data.json
+-rw-r--r--   0        0        0     1657 2023-07-27 22:51:51.714795 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/logger.meta.json
+-rw-r--r--   0        0        0     4028 2023-07-27 22:51:53.725231 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/macro.data.json
+-rw-r--r--   0        0        0     1638 2023-07-27 22:51:53.725414 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/macro.meta.json
+-rw-r--r--   0        0        0    17783 2023-07-27 22:51:54.037057 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/magic_arguments.data.json
+-rw-r--r--   0        0        0     1849 2023-07-27 22:51:54.037285 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/magic_arguments.meta.json
+-rw-r--r--   0        0        0     3558 2023-07-27 22:51:53.987117 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/payload.data.json
+-rw-r--r--   0        0        0     1786 2023-07-27 22:51:53.987339 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/payload.meta.json
+-rw-r--r--   0        0        0     5686 2023-07-27 22:51:53.910293 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/pylabtools.data.json
+-rw-r--r--   0        0        0     1741 2023-07-27 22:51:53.910534 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/pylabtools.meta.json
+-rw-r--r--   0        0        0     5245 2023-07-27 22:51:51.109111 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/release.data.json
+-rw-r--r--   0        0        0     1558 2023-07-27 22:51:51.109289 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/release.meta.json
+-rw-r--r--   0        0        0     2940 2023-07-27 22:51:51.712023 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/usage.data.json
+-rw-r--r--   0        0        0     1617 2023-07-27 22:51:51.712204 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/core/usage.meta.json
+-rw-r--r--   0        0        0     5353 2023-07-27 22:51:54.009461 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/display.data.json
+-rw-r--r--   0        0        0     1764 2023-07-27 22:51:54.009655 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/display.meta.json
+-rw-r--r--   0        0        0     1565 2023-07-27 22:51:50.964240 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/extensions/__init__.data.json
+-rw-r--r--   0        0        0     1536 2023-07-27 22:51:50.964419 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/extensions/__init__.meta.json
+-rw-r--r--   0        0        0     1509 2023-07-27 22:51:51.098691 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/lib/__init__.data.json
+-rw-r--r--   0        0        0     1523 2023-07-27 22:51:51.098861 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/lib/__init__.meta.json
+-rw-r--r--   0        0        0    30393 2023-07-27 22:51:53.948912 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/lib/display.data.json
+-rw-r--r--   0        0        0     2005 2023-07-27 22:51:53.949133 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/lib/display.meta.json
+-rw-r--r--   0        0        0    46626 2023-07-27 22:51:53.800804 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/lib/pretty.data.json
+-rw-r--r--   0        0        0     1866 2023-07-27 22:51:53.801055 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/lib/pretty.meta.json
+-rw-r--r--   0        0        0     1549 2023-07-27 22:51:51.071651 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/__init__.data.json
+-rw-r--r--   0        0        0     1531 2023-07-27 22:51:51.071816 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/__init__.meta.json
+-rw-r--r--   0        0        0     9601 2023-07-27 22:51:55.227200 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/prompts.data.json
+-rw-r--r--   0        0        0     2295 2023-07-27 22:51:55.227393 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/prompts.meta.json
+-rw-r--r--   0        0        0     5382 2023-07-27 22:51:51.010414 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/pt_inputhooks/__init__.data.json
+-rw-r--r--   0        0        0     1589 2023-07-27 22:51:51.010696 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/pt_inputhooks/__init__.meta.json
+-rw-r--r--   0        0        0    30671 2023-07-27 22:51:55.336828 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/__init__.data.json
+-rw-r--r--   0        0        0     2469 2023-07-27 22:51:55.337025 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/__init__.meta.json
+-rw-r--r--   0        0        0    12059 2023-07-27 22:51:55.220382 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/auto_match.data.json
+-rw-r--r--   0        0        0     1818 2023-07-27 22:51:55.220588 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/auto_match.meta.json
+-rw-r--r--   0        0        0    32296 2023-07-27 22:51:55.335922 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/auto_suggest.data.json
+-rw-r--r--   0        0        0     2341 2023-07-27 22:51:55.336138 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/auto_suggest.meta.json
+-rw-r--r--   0        0        0    22567 2023-07-27 22:51:55.334867 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/filters.data.json
+-rw-r--r--   0        0        0     2394 2023-07-27 22:51:55.335190 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/filters.meta.json
+-rw-r--r--   0        0        0     1872 2023-07-27 22:51:51.051438 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/testing/__init__.data.json
+-rw-r--r--   0        0        0     1567 2023-07-27 22:51:51.051652 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1652 2023-07-27 22:51:51.103448 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/testing/skipdoctest.data.json
+-rw-r--r--   0        0        0     1546 2023-07-27 22:51:51.103634 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/testing/skipdoctest.meta.json
+-rw-r--r--   0        0        0    10833 2023-07-27 22:51:54.033890 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/PyColorize.data.json
+-rw-r--r--   0        0        0     1918 2023-07-27 22:51:54.034174 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/PyColorize.meta.json
+-rw-r--r--   0        0        0     1525 2023-07-27 22:51:51.065804 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/__init__.data.json
+-rw-r--r--   0        0        0     1525 2023-07-27 22:51:51.065980 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3502 2023-07-27 22:51:53.784143 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/_process_common.data.json
+-rw-r--r--   0        0        0     1704 2023-07-27 22:51:53.784350 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/_process_common.meta.json
+-rw-r--r--   0        0        0     7297 2023-07-27 22:51:53.837922 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/_process_posix.data.json
+-rw-r--r--   0        0        0     1730 2023-07-27 22:51:53.838110 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/_process_posix.meta.json
+-rw-r--r--   0        0        0     6826 2023-07-27 22:51:53.913712 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/_process_win32.data.json
+-rw-r--r--   0        0        0     1849 2023-07-27 22:51:53.913927 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/_process_win32.meta.json
+-rw-r--r--   0        0        0     1559 2023-07-27 22:51:51.054593 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/_sysinfo.data.json
+-rw-r--r--   0        0        0     1535 2023-07-27 22:51:51.054777 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/_sysinfo.meta.json
+-rw-r--r--   0        0        0    16110 2023-07-27 22:51:54.022274 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/capture.data.json
+-rw-r--r--   0        0        0     1954 2023-07-27 22:51:54.022542 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/capture.meta.json
+-rw-r--r--   0        0        0     3860 2023-07-27 22:51:53.983836 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/colorable.data.json
+-rw-r--r--   0        0        0     1807 2023-07-27 22:51:53.984068 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/colorable.meta.json
+-rw-r--r--   0        0        0    17827 2023-07-27 22:51:51.695006 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/coloransi.data.json
+-rw-r--r--   0        0        0     1605 2023-07-27 22:51:51.695233 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/coloransi.meta.json
+-rw-r--r--   0        0        0     4124 2023-07-27 22:51:51.964177 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/contexts.data.json
+-rw-r--r--   0        0        0     1553 2023-07-27 22:51:51.964356 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/contexts.meta.json
+-rw-r--r--   0        0        0     1830 2023-07-27 22:51:51.008723 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/data.data.json
+-rw-r--r--   0        0        0     1529 2023-07-27 22:51:51.008891 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/data.meta.json
+-rw-r--r--   0        0        0     2993 2023-07-27 22:51:51.711130 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/decorators.data.json
+-rw-r--r--   0        0        0     1567 2023-07-27 22:51:51.711317 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/decorators.meta.json
+-rw-r--r--   0        0        0     2259 2023-07-27 22:51:52.211405 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/dir2.data.json
+-rw-r--r--   0        0        0     1600 2023-07-27 22:51:52.211591 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/dir2.meta.json
+-rw-r--r--   0        0        0     1636 2023-07-27 22:51:51.001813 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/docs.data.json
+-rw-r--r--   0        0        0     1537 2023-07-27 22:51:51.001989 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/docs.meta.json
+-rw-r--r--   0        0        0     2447 2023-07-27 22:51:52.994411 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/encoding.data.json
+-rw-r--r--   0        0        0     1624 2023-07-27 22:51:52.994626 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/encoding.meta.json
+-rw-r--r--   0        0        0     2505 2023-07-27 22:51:51.107542 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/frame.data.json
+-rw-r--r--   0        0        0     1543 2023-07-27 22:51:51.107725 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/frame.meta.json
+-rw-r--r--   0        0        0     4049 2023-07-27 22:51:51.685794 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/generics.data.json
+-rw-r--r--   0        0        0     1577 2023-07-27 22:51:51.686084 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/generics.meta.json
+-rw-r--r--   0        0        0     1644 2023-07-27 22:51:51.016394 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/importstring.data.json
+-rw-r--r--   0        0        0     1545 2023-07-27 22:51:51.016728 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/importstring.meta.json
+-rw-r--r--   0        0        0     6675 2023-07-27 22:51:54.729212 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/io.data.json
+-rw-r--r--   0        0        0     1806 2023-07-27 22:51:54.729429 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/io.meta.json
+-rw-r--r--   0        0        0     6854 2023-07-27 22:51:51.067249 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/ipstruct.data.json
+-rw-r--r--   0        0        0     1538 2023-07-27 22:51:51.067427 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/ipstruct.meta.json
+-rw-r--r--   0        0        0     1788 2023-07-27 22:51:50.961045 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/module_paths.data.json
+-rw-r--r--   0        0        0     1575 2023-07-27 22:51:50.961225 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/module_paths.meta.json
+-rw-r--r--   0        0        0     3647 2023-07-27 22:51:52.052956 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/openpy.data.json
+-rw-r--r--   0        0        0     1639 2023-07-27 22:51:52.053196 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/openpy.meta.json
+-rw-r--r--   0        0        0     8481 2023-07-27 22:51:54.038709 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/path.data.json
+-rw-r--r--   0        0        0     1765 2023-07-27 22:51:54.038925 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/path.meta.json
+-rw-r--r--   0        0        0     3617 2023-07-27 22:51:53.986191 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/process.data.json
+-rw-r--r--   0        0        0     1773 2023-07-27 22:51:53.986410 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/process.meta.json
+-rw-r--r--   0        0        0     5236 2023-07-27 22:51:53.726191 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/py3compat.data.json
+-rw-r--r--   0        0        0     1628 2023-07-27 22:51:53.726369 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/py3compat.meta.json
+-rw-r--r--   0        0        0     3147 2023-07-27 22:51:51.005130 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/sentinel.data.json
+-rw-r--r--   0        0        0     1536 2023-07-27 22:51:51.005309 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/sentinel.meta.json
+-rw-r--r--   0        0        0     4816 2023-07-27 22:51:52.051938 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/strdispatch.data.json
+-rw-r--r--   0        0        0     1621 2023-07-27 22:51:52.052163 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/strdispatch.meta.json
+-rw-r--r--   0        0        0     3272 2023-07-27 22:51:53.726889 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/sysinfo.data.json
+-rw-r--r--   0        0        0     1786 2023-07-27 22:51:53.727067 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/sysinfo.meta.json
+-rw-r--r--   0        0        0     5984 2023-07-27 22:51:52.050794 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/syspathcontext.data.json
+-rw-r--r--   0        0        0     1638 2023-07-27 22:51:52.051024 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/syspathcontext.meta.json
+-rw-r--r--   0        0        0     5217 2023-07-27 22:51:52.008359 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/terminal.data.json
+-rw-r--r--   0        0        0     1616 2023-07-27 22:51:52.008610 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/terminal.meta.json
+-rw-r--r--   0        0        0    20894 2023-07-27 22:51:51.710329 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/text.data.json
+-rw-r--r--   0        0        0     1629 2023-07-27 22:51:51.710553 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/text.meta.json
+-rw-r--r--   0        0        0     3274 2023-07-27 22:51:51.653668 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/timing.data.json
+-rw-r--r--   0        0        0     1576 2023-07-27 22:51:51.653899 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/timing.meta.json
+-rw-r--r--   0        0        0    25950 2023-07-27 22:51:51.970706 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/tokenutil.data.json
+-rw-r--r--   0        0        0     1597 2023-07-27 22:51:51.970891 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/tokenutil.meta.json
+-rw-r--r--   0        0        0     4095 2023-07-27 22:51:52.965660 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/wildcard.data.json
+-rw-r--r--   0        0        0     1631 2023-07-27 22:51:52.965854 alacorder-81.1.4/alacorder/.mypy_cache/3.10/IPython/utils/wildcard.meta.json
+-rw-r--r--   0        0        0     7816 2023-07-27 22:51:51.358108 alacorder-81.1.4/alacorder/.mypy_cache/3.10/__future__.data.json
+-rw-r--r--   0        0        0     1558 2023-07-27 22:51:51.358287 alacorder-81.1.4/alacorder/.mypy_cache/3.10/__future__.meta.json
+-rw-r--r--   0        0        0   177662 2023-07-27 22:51:50.849508 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1575 2023-07-27 22:51:50.849704 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    49905 2023-07-27 22:51:50.895186 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_bisect.data.json
+-rw-r--r--   0        0        0     1577 2023-07-27 22:51:50.895365 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_bisect.meta.json
+-rw-r--r--   0        0        0    51291 2023-07-27 22:51:50.846213 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1615 2023-07-27 22:51:50.846382 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    21942 2023-07-27 22:51:50.844903 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1610 2023-07-27 22:51:50.845080 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0    10060 2023-07-27 22:51:51.046081 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_compression.data.json
+-rw-r--r--   0        0        0     1609 2023-07-27 22:51:51.046266 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_compression.meta.json
+-rw-r--r--   0        0        0    19625 2023-07-27 22:51:51.078424 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_csv.data.json
+-rw-r--r--   0        0        0     1584 2023-07-27 22:51:51.078651 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_csv.meta.json
+-rw-r--r--   0        0        0    90550 2023-07-27 22:51:51.318998 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1626 2023-07-27 22:51:51.319243 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0   174451 2023-07-27 22:51:51.745607 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_decimal.data.json
+-rw-r--r--   0        0        0     1632 2023-07-27 22:51:51.745908 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_decimal.meta.json
+-rw-r--r--   0        0        0   126511 2023-07-27 22:51:51.384611 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_operator.data.json
+-rw-r--r--   0        0        0     1605 2023-07-27 22:51:51.384927 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_operator.meta.json
+-rw-r--r--   0        0        0     6090 2023-07-27 22:51:51.374940 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_random.data.json
+-rw-r--r--   0        0        0     1552 2023-07-27 22:51:51.375137 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_random.meta.json
+-rw-r--r--   0        0        0    90355 2023-07-27 22:51:51.131629 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_socket.data.json
+-rw-r--r--   0        0        0     1602 2023-07-27 22:51:51.131855 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_socket.meta.json
+-rw-r--r--   0        0        0    19698 2023-07-27 22:51:51.083324 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_stat.data.json
+-rw-r--r--   0        0        0     1560 2023-07-27 22:51:51.083555 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_stat.meta.json
+-rw-r--r--   0        0        0    23856 2023-07-27 22:51:51.505473 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_thread.data.json
+-rw-r--r--   0        0        0     1629 2023-07-27 22:51:51.505671 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_thread.meta.json
+-rw-r--r--   0        0        0   108216 2023-07-27 22:51:50.844144 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1640 2023-07-27 22:51:50.844321 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0     4930 2023-07-27 22:51:51.090466 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_typeshed/xml.data.json
+-rw-r--r--   0        0        0     1539 2023-07-27 22:51:51.090649 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_typeshed/xml.meta.json
+-rw-r--r--   0        0        0    13073 2023-07-27 22:51:51.386353 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_warnings.data.json
+-rw-r--r--   0        0        0     1532 2023-07-27 22:51:51.386600 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_warnings.meta.json
+-rw-r--r--   0        0        0    30627 2023-07-27 22:51:51.118471 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_weakref.data.json
+-rw-r--r--   0        0        0     1616 2023-07-27 22:51:51.118687 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_weakref.meta.json
+-rw-r--r--   0        0        0    61659 2023-07-27 22:51:51.115333 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_weakrefset.data.json
+-rw-r--r--   0        0        0     1622 2023-07-27 22:51:51.115682 alacorder-81.1.4/alacorder/.mypy_cache/3.10/_weakrefset.meta.json
+-rw-r--r--   0        0        0    26853 2023-07-27 22:51:50.842000 alacorder-81.1.4/alacorder/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1582 2023-07-27 22:51:50.842168 alacorder-81.1.4/alacorder/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0   159707 2023-07-27 22:51:51.403679 alacorder-81.1.4/alacorder/.mypy_cache/3.10/argparse.data.json
+-rw-r--r--   0        0        0     1614 2023-07-27 22:51:51.403968 alacorder-81.1.4/alacorder/.mypy_cache/3.10/argparse.meta.json
+-rw-r--r--   0        0        0    70967 2023-07-27 22:51:51.342187 alacorder-81.1.4/alacorder/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1597 2023-07-27 22:51:51.342460 alacorder-81.1.4/alacorder/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0   136485 2023-07-27 22:51:51.355576 alacorder-81.1.4/alacorder/.mypy_cache/3.10/ast.data.json
+-rw-r--r--   0        0        0     1627 2023-07-27 22:51:51.355831 alacorder-81.1.4/alacorder/.mypy_cache/3.10/ast.meta.json
+-rw-r--r--   0        0        0     2314 2023-07-27 22:51:52.177814 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/__init__.data.json
+-rw-r--r--   0        0        0     1619 2023-07-27 22:51:52.177986 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/__init__.meta.json
+-rw-r--r--   0        0        0     2439 2023-07-27 22:51:50.896918 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/astroid_compat.data.json
+-rw-r--r--   0        0        0     1600 2023-07-27 22:51:50.897093 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/astroid_compat.meta.json
+-rw-r--r--   0        0        0    38518 2023-07-27 22:51:52.176018 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/asttokens.data.json
+-rw-r--r--   0        0        0     1819 2023-07-27 22:51:52.176266 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/asttokens.meta.json
+-rw-r--r--   0        0        0     6907 2023-07-27 22:51:51.918180 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/line_numbers.data.json
+-rw-r--r--   0        0        0     1575 2023-07-27 22:51:51.918377 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/line_numbers.meta.json
+-rw-r--r--   0        0        0    56358 2023-07-27 22:51:52.177402 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/mark_tokens.data.json
+-rw-r--r--   0        0        0     1771 2023-07-27 22:51:52.177608 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/mark_tokens.meta.json
+-rw-r--r--   0        0        0    61889 2023-07-27 22:51:51.953737 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/util.data.json
+-rw-r--r--   0        0        0     1710 2023-07-27 22:51:51.953985 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asttokens/util.meta.json
+-rw-r--r--   0        0        0    14446 2023-07-27 22:51:53.906554 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     2012 2023-07-27 22:51:53.906762 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0    98976 2023-07-27 22:51:53.905889 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     1869 2023-07-27 22:51:53.906107 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    28169 2023-07-27 22:51:50.968963 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1624 2023-07-27 22:51:50.969190 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   196507 2023-07-27 22:51:53.903714 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/events.data.json
+-rw-r--r--   0        0        0     1891 2023-07-27 22:51:53.903960 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/events.meta.json
+-rw-r--r--   0        0        0     9023 2023-07-27 22:51:50.966765 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1579 2023-07-27 22:51:50.967056 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    42232 2023-07-27 22:51:53.899932 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1789 2023-07-27 22:51:53.900163 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    27160 2023-07-27 22:51:53.898772 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1743 2023-07-27 22:51:53.899009 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/locks.meta.json
+-rw-r--r--   0        0        0    17206 2023-07-27 22:51:53.890571 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1673 2023-07-27 22:51:53.890776 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    25758 2023-07-27 22:51:53.897834 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1646 2023-07-27 22:51:53.898066 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/queues.meta.json
+-rw-r--r--   0        0        0     5002 2023-07-27 22:51:53.896992 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1699 2023-07-27 22:51:53.897202 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     3818 2023-07-27 22:51:53.888825 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1684 2023-07-27 22:51:53.889138 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    35284 2023-07-27 22:51:53.896508 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1785 2023-07-27 22:51:53.896708 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    23927 2023-07-27 22:51:53.889839 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1805 2023-07-27 22:51:53.890073 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0   123121 2023-07-27 22:51:53.895477 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1804 2023-07-27 22:51:53.895683 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     6472 2023-07-27 22:51:50.965018 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1589 2023-07-27 22:51:50.965185 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/threads.meta.json
+-rw-r--r--   0        0        0    27481 2023-07-27 22:51:53.892931 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1698 2023-07-27 22:51:53.893143 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    61503 2023-07-27 22:51:53.892056 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1776 2023-07-27 22:51:53.892272 alacorder-81.1.4/alacorder/.mypy_cache/3.10/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0     9226 2023-07-27 22:51:51.072636 alacorder-81.1.4/alacorder/.mypy_cache/3.10/atexit.data.json
+-rw-r--r--   0        0        0     1571 2023-07-27 22:51:51.072804 alacorder-81.1.4/alacorder/.mypy_cache/3.10/atexit.meta.json
+-rw-r--r--   0        0        0   222149 2023-07-27 22:51:51.817359 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/__init__.data.json
+-rw-r--r--   0        0        0     1735 2023-07-27 22:51:51.817908 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/__init__.meta.json
+-rw-r--r--   0        0        0     3906 2023-07-27 22:51:51.172863 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/_cmp.data.json
+-rw-r--r--   0        0        0     1510 2023-07-27 22:51:51.173074 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/_cmp.meta.json
+-rw-r--r--   0        0        0     3015 2023-07-27 22:51:51.172138 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/_typing_compat.data.json
+-rw-r--r--   0        0        0     1530 2023-07-27 22:51:51.172310 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/_typing_compat.meta.json
+-rw-r--r--   0        0        0     7004 2023-07-27 22:51:51.171436 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/_version_info.data.json
+-rw-r--r--   0        0        0     1529 2023-07-27 22:51:51.171646 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/_version_info.meta.json
+-rw-r--r--   0        0        0     9115 2023-07-27 22:51:51.820373 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/converters.data.json
+-rw-r--r--   0        0        0     1533 2023-07-27 22:51:51.820540 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/converters.meta.json
+-rw-r--r--   0        0        0    10237 2023-07-27 22:51:51.174362 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/exceptions.data.json
+-rw-r--r--   0        0        0     1522 2023-07-27 22:51:51.174713 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/exceptions.meta.json
+-rw-r--r--   0        0        0     3538 2023-07-27 22:51:51.819897 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/filters.data.json
+-rw-r--r--   0        0        0     1527 2023-07-27 22:51:51.820057 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/filters.meta.json
+-rw-r--r--   0        0        0     8130 2023-07-27 22:51:51.819496 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/setters.data.json
+-rw-r--r--   0        0        0     1527 2023-07-27 22:51:51.819668 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/setters.meta.json
+-rw-r--r--   0        0        0    50838 2023-07-27 22:51:51.818976 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/validators.data.json
+-rw-r--r--   0        0        0     1563 2023-07-27 22:51:51.819178 alacorder-81.1.4/alacorder/.mypy_cache/3.10/attr/validators.meta.json
+-rw-r--r--   0        0        0    15383 2023-07-27 22:51:51.420330 alacorder-81.1.4/alacorder/.mypy_cache/3.10/base64.data.json
+-rw-r--r--   0        0        0     1578 2023-07-27 22:51:51.420575 alacorder-81.1.4/alacorder/.mypy_cache/3.10/base64.meta.json
+-rw-r--r--   0        0        0    50167 2023-07-27 22:51:51.065258 alacorder-81.1.4/alacorder/.mypy_cache/3.10/bdb.data.json
+-rw-r--r--   0        0        0     1605 2023-07-27 22:51:51.065464 alacorder-81.1.4/alacorder/.mypy_cache/3.10/bdb.meta.json
+-rw-r--r--   0        0        0    13515 2023-07-27 22:51:51.106259 alacorder-81.1.4/alacorder/.mypy_cache/3.10/binascii.data.json
+-rw-r--r--   0        0        0     1582 2023-07-27 22:51:51.106478 alacorder-81.1.4/alacorder/.mypy_cache/3.10/binascii.meta.json
+-rw-r--r--   0        0        0    12852 2023-07-27 22:51:51.638171 alacorder-81.1.4/alacorder/.mypy_cache/3.10/bisect.data.json
+-rw-r--r--   0        0        0     1556 2023-07-27 22:51:51.638351 alacorder-81.1.4/alacorder/.mypy_cache/3.10/bisect.meta.json
+-rw-r--r--   0        0        0  1188395 2023-07-27 22:51:50.871530 alacorder-81.1.4/alacorder/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1666 2023-07-27 22:51:50.872179 alacorder-81.1.4/alacorder/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0    21585 2023-07-27 22:51:50.989155 alacorder-81.1.4/alacorder/.mypy_cache/3.10/cProfile.data.json
+-rw-r--r--   0        0        0     1640 2023-07-27 22:51:50.989407 alacorder-81.1.4/alacorder/.mypy_cache/3.10/cProfile.meta.json
+-rw-r--r--   0        0        0     2288 2023-07-27 22:51:52.107041 alacorder-81.1.4/alacorder/.mypy_cache/3.10/certifi/__init__.data.json
+-rw-r--r--   0        0        0     1576 2023-07-27 22:51:52.107214 alacorder-81.1.4/alacorder/.mypy_cache/3.10/certifi/__init__.meta.json
+-rw-r--r--   0        0        0     3056 2023-07-27 22:51:51.725906 alacorder-81.1.4/alacorder/.mypy_cache/3.10/certifi/core.data.json
+-rw-r--r--   0        0        0     1572 2023-07-27 22:51:51.726087 alacorder-81.1.4/alacorder/.mypy_cache/3.10/certifi/core.meta.json
+-rw-r--r--   0        0        0     7747 2023-07-27 22:51:52.501152 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/__init__.data.json
+-rw-r--r--   0        0        0     1743 2023-07-27 22:51:52.501315 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/__init__.meta.json
+-rw-r--r--   0        0        0    47172 2023-07-27 22:51:52.115219 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/_compat.data.json
+-rw-r--r--   0        0        0     1657 2023-07-27 22:51:52.115436 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/_compat.meta.json
+-rw-r--r--   0        0        0    47953 2023-07-27 22:51:52.491303 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     1893 2023-07-27 22:51:52.491543 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0   182167 2023-07-27 22:51:52.498292 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/core.data.json
+-rw-r--r--   0        0        0     2003 2023-07-27 22:51:52.498501 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/core.meta.json
+-rw-r--r--   0        0        0    60248 2023-07-27 22:51:52.499757 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/decorators.data.json
+-rw-r--r--   0        0        0     1684 2023-07-27 22:51:52.499929 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/decorators.meta.json
+-rw-r--r--   0        0        0    27635 2023-07-27 22:51:52.489172 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/exceptions.data.json
+-rw-r--r--   0        0        0     1649 2023-07-27 22:51:52.489344 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17497 2023-07-27 22:51:52.492061 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/formatting.data.json
+-rw-r--r--   0        0        0     1681 2023-07-27 22:51:52.492257 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/formatting.meta.json
+-rw-r--r--   0        0        0     7042 2023-07-27 22:51:52.487116 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/globals.data.json
+-rw-r--r--   0        0        0     1621 2023-07-27 22:51:52.487411 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/globals.meta.json
+-rw-r--r--   0        0        0    28765 2023-07-27 22:51:52.490043 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/parser.data.json
+-rw-r--r--   0        0        0     1682 2023-07-27 22:51:52.490231 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/parser.meta.json
+-rw-r--r--   0        0        0    33752 2023-07-27 22:51:52.500683 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1691 2023-07-27 22:51:52.500863 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    24205 2023-07-27 22:51:52.494746 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/termui.data.json
+-rw-r--r--   0        0        0     1786 2023-07-27 22:51:52.494924 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/termui.meta.json
+-rw-r--r--   0        0        0    80652 2023-07-27 22:51:52.493910 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/types.data.json
+-rw-r--r--   0        0        0     1815 2023-07-27 22:51:52.494098 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/types.meta.json
+-rw-r--r--   0        0        0    32709 2023-07-27 22:51:52.488263 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/utils.data.json
+-rw-r--r--   0        0        0     1736 2023-07-27 22:51:52.488475 alacorder-81.1.4/alacorder/.mypy_cache/3.10/click/utils.meta.json
+-rw-r--r--   0        0        0    20259 2023-07-27 22:51:50.963753 alacorder-81.1.4/alacorder/.mypy_cache/3.10/cmd.data.json
+-rw-r--r--   0        0        0     1566 2023-07-27 22:51:50.963930 alacorder-81.1.4/alacorder/.mypy_cache/3.10/cmd.meta.json
+-rw-r--r--   0        0        0   125751 2023-07-27 22:51:50.841182 alacorder-81.1.4/alacorder/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1626 2023-07-27 22:51:50.841359 alacorder-81.1.4/alacorder/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0     5706 2023-07-27 22:51:51.012986 alacorder-81.1.4/alacorder/.mypy_cache/3.10/codeop.data.json
+-rw-r--r--   0        0        0     1538 2023-07-27 22:51:51.013183 alacorder-81.1.4/alacorder/.mypy_cache/3.10/codeop.meta.json
+-rw-r--r--   0        0        0   504131 2023-07-27 22:51:50.838514 alacorder-81.1.4/alacorder/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1655 2023-07-27 22:51:50.838743 alacorder-81.1.4/alacorder/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3726 2023-07-27 22:51:50.829692 alacorder-81.1.4/alacorder/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1566 2023-07-27 22:51:50.829856 alacorder-81.1.4/alacorder/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0     7539 2023-07-27 22:51:51.356823 alacorder-81.1.4/alacorder/.mypy_cache/3.10/colorsys.data.json
+-rw-r--r--   0        0        0     1530 2023-07-27 22:51:51.357005 alacorder-81.1.4/alacorder/.mypy_cache/3.10/colorsys.meta.json
+-rw-r--r--   0        0        0     1522 2023-07-27 22:51:50.920915 alacorder-81.1.4/alacorder/.mypy_cache/3.10/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1541 2023-07-27 22:51:50.921112 alacorder-81.1.4/alacorder/.mypy_cache/3.10/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4537 2023-07-27 22:51:53.783285 alacorder-81.1.4/alacorder/.mypy_cache/3.10/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1728 2023-07-27 22:51:53.783501 alacorder-81.1.4/alacorder/.mypy_cache/3.10/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    81175 2023-07-27 22:51:51.943387 alacorder-81.1.4/alacorder/.mypy_cache/3.10/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1678 2023-07-27 22:51:51.943627 alacorder-81.1.4/alacorder/.mypy_cache/3.10/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    61157 2023-07-27 22:51:53.717973 alacorder-81.1.4/alacorder/.mypy_cache/3.10/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     1928 2023-07-27 22:51:53.718230 alacorder-81.1.4/alacorder/.mypy_cache/3.10/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    22719 2023-07-27 22:51:52.183745 alacorder-81.1.4/alacorder/.mypy_cache/3.10/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1760 2023-07-27 22:51:52.183952 alacorder-81.1.4/alacorder/.mypy_cache/3.10/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0   129001 2023-07-27 22:51:51.333449 alacorder-81.1.4/alacorder/.mypy_cache/3.10/configparser.data.json
+-rw-r--r--   0        0        0     1631 2023-07-27 22:51:51.333711 alacorder-81.1.4/alacorder/.mypy_cache/3.10/configparser.meta.json
+-rw-r--r--   0        0        0   118047 2023-07-27 22:51:50.829279 alacorder-81.1.4/alacorder/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1618 2023-07-27 22:51:50.829454 alacorder-81.1.4/alacorder/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    44294 2023-07-27 22:51:50.925013 alacorder-81.1.4/alacorder/.mypy_cache/3.10/contextvars.data.json
+-rw-r--r--   0        0        0     1622 2023-07-27 22:51:50.925216 alacorder-81.1.4/alacorder/.mypy_cache/3.10/contextvars.meta.json
+-rw-r--r--   0        0        0     6048 2023-07-27 22:51:51.424567 alacorder-81.1.4/alacorder/.mypy_cache/3.10/copy.data.json
+-rw-r--r--   0        0        0     1521 2023-07-27 22:51:51.424816 alacorder-81.1.4/alacorder/.mypy_cache/3.10/copy.meta.json
+-rw-r--r--   0        0        0    13035 2023-07-27 22:51:50.874118 alacorder-81.1.4/alacorder/.mypy_cache/3.10/copyreg.data.json
+-rw-r--r--   0        0        0     1590 2023-07-27 22:51:50.874297 alacorder-81.1.4/alacorder/.mypy_cache/3.10/copyreg.meta.json
+-rw-r--r--   0        0        0    32138 2023-07-27 22:51:51.749239 alacorder-81.1.4/alacorder/.mypy_cache/3.10/csv.data.json
+-rw-r--r--   0        0        0     1609 2023-07-27 22:51:51.749473 alacorder-81.1.4/alacorder/.mypy_cache/3.10/csv.meta.json
+-rw-r--r--   0        0        0    56033 2023-07-27 22:51:51.320430 alacorder-81.1.4/alacorder/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1616 2023-07-27 22:51:51.320615 alacorder-81.1.4/alacorder/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    54630 2023-07-27 22:51:51.782530 alacorder-81.1.4/alacorder/.mypy_cache/3.10/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1598 2023-07-27 22:51:51.782751 alacorder-81.1.4/alacorder/.mypy_cache/3.10/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0    64231 2023-07-27 22:51:50.826916 alacorder-81.1.4/alacorder/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1633 2023-07-27 22:51:50.827075 alacorder-81.1.4/alacorder/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   155471 2023-07-27 22:51:51.854126 alacorder-81.1.4/alacorder/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1593 2023-07-27 22:51:51.854457 alacorder-81.1.4/alacorder/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0     4906 2023-07-27 22:51:52.108299 alacorder-81.1.4/alacorder/.mypy_cache/3.10/decimal.data.json
+-rw-r--r--   0        0        0     1586 2023-07-27 22:51:52.108480 alacorder-81.1.4/alacorder/.mypy_cache/3.10/decimal.meta.json
+-rw-r--r--   0        0        0    63990 2023-07-27 22:51:51.089355 alacorder-81.1.4/alacorder/.mypy_cache/3.10/difflib.data.json
+-rw-r--r--   0        0        0     1590 2023-07-27 22:51:51.089631 alacorder-81.1.4/alacorder/.mypy_cache/3.10/difflib.meta.json
+-rw-r--r--   0        0        0    42382 2023-07-27 22:51:51.776718 alacorder-81.1.4/alacorder/.mypy_cache/3.10/dis.data.json
+-rw-r--r--   0        0        0     1620 2023-07-27 22:51:51.776945 alacorder-81.1.4/alacorder/.mypy_cache/3.10/dis.meta.json
+-rw-r--r--   0        0        0     7433 2023-07-27 22:51:50.825421 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1618 2023-07-27 22:51:50.825592 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    12195 2023-07-27 22:51:50.824960 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1563 2023-07-27 22:51:50.825123 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7244 2023-07-27 22:51:50.824401 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1595 2023-07-27 22:51:50.824574 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25068 2023-07-27 22:51:50.823934 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1567 2023-07-27 22:51:50.824109 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9149 2023-07-27 22:51:50.823229 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1580 2023-07-27 22:51:50.823405 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    84152 2023-07-27 22:51:50.822708 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1683 2023-07-27 22:51:50.822890 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    30852 2023-07-27 22:51:50.820848 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1644 2023-07-27 22:51:50.821031 alacorder-81.1.4/alacorder/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0    68559 2023-07-27 22:51:50.819926 alacorder-81.1.4/alacorder/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1608 2023-07-27 22:51:50.820098 alacorder-81.1.4/alacorder/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    19378 2023-07-27 22:51:51.213863 alacorder-81.1.4/alacorder/.mypy_cache/3.10/errno.data.json
+-rw-r--r--   0        0        0     1575 2023-07-27 22:51:51.214046 alacorder-81.1.4/alacorder/.mypy_cache/3.10/errno.meta.json
+-rw-r--r--   0        0        0    22917 2023-07-27 22:51:53.720757 alacorder-81.1.4/alacorder/.mypy_cache/3.10/executing/__init__.data.json
+-rw-r--r--   0        0        0     1675 2023-07-27 22:51:53.721016 alacorder-81.1.4/alacorder/.mypy_cache/3.10/executing/__init__.meta.json
+-rw-r--r--   0        0        0    78088 2023-07-27 22:51:52.947887 alacorder-81.1.4/alacorder/.mypy_cache/3.10/executing/executing.data.json
+-rw-r--r--   0        0        0     1938 2023-07-27 22:51:52.948150 alacorder-81.1.4/alacorder/.mypy_cache/3.10/executing/executing.meta.json
+-rw-r--r--   0        0        0     1534 2023-07-27 22:51:50.896208 alacorder-81.1.4/alacorder/.mypy_cache/3.10/executing/version.data.json
+-rw-r--r--   0        0        0     1525 2023-07-27 22:51:50.896378 alacorder-81.1.4/alacorder/.mypy_cache/3.10/executing/version.meta.json
+-rw-r--r--   0        0        0     7007 2023-07-27 22:51:50.957821 alacorder-81.1.4/alacorder/.mypy_cache/3.10/fnmatch.data.json
+-rw-r--r--   0        0        0     1549 2023-07-27 22:51:50.958081 alacorder-81.1.4/alacorder/.mypy_cache/3.10/fnmatch.meta.json
+-rw-r--r--   0        0        0    90541 2023-07-27 22:51:52.406608 alacorder-81.1.4/alacorder/.mypy_cache/3.10/fractions.data.json
+-rw-r--r--   0        0        0     1693 2023-07-27 22:51:52.406844 alacorder-81.1.4/alacorder/.mypy_cache/3.10/fractions.meta.json
+-rw-r--r--   0        0        0   152418 2023-07-27 22:51:51.464360 alacorder-81.1.4/alacorder/.mypy_cache/3.10/functools.data.json
+-rw-r--r--   0        0        0     1617 2023-07-27 22:51:51.464661 alacorder-81.1.4/alacorder/.mypy_cache/3.10/functools.meta.json
+-rw-r--r--   0        0        0    15955 2023-07-27 22:51:51.007267 alacorder-81.1.4/alacorder/.mypy_cache/3.10/gc.data.json
+-rw-r--r--   0        0        0     1592 2023-07-27 22:51:51.007450 alacorder-81.1.4/alacorder/.mypy_cache/3.10/gc.meta.json
+-rw-r--r--   0        0        0    23498 2023-07-27 22:51:50.818293 alacorder-81.1.4/alacorder/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1608 2023-07-27 22:51:50.818501 alacorder-81.1.4/alacorder/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0     6277 2023-07-27 22:51:51.011873 alacorder-81.1.4/alacorder/.mypy_cache/3.10/getopt.data.json
+-rw-r--r--   0        0        0     1526 2023-07-27 22:51:51.012066 alacorder-81.1.4/alacorder/.mypy_cache/3.10/getopt.meta.json
+-rw-r--r--   0        0        0     3734 2023-07-27 22:51:51.453852 alacorder-81.1.4/alacorder/.mypy_cache/3.10/getpass.data.json
+-rw-r--r--   0        0        0     1527 2023-07-27 22:51:51.454035 alacorder-81.1.4/alacorder/.mypy_cache/3.10/getpass.meta.json
+-rw-r--r--   0        0        0    55134 2023-07-27 22:51:51.220060 alacorder-81.1.4/alacorder/.mypy_cache/3.10/gettext.data.json
+-rw-r--r--   0        0        0     1611 2023-07-27 22:51:51.220348 alacorder-81.1.4/alacorder/.mypy_cache/3.10/gettext.meta.json
+-rw-r--r--   0        0        0    10955 2023-07-27 22:51:51.532527 alacorder-81.1.4/alacorder/.mypy_cache/3.10/glob.data.json
+-rw-r--r--   0        0        0     1571 2023-07-27 22:51:51.532708 alacorder-81.1.4/alacorder/.mypy_cache/3.10/glob.meta.json
+-rw-r--r--   0        0        0    45664 2023-07-27 22:51:51.724994 alacorder-81.1.4/alacorder/.mypy_cache/3.10/gzip.data.json
+-rw-r--r--   0        0        0     1624 2023-07-27 22:51:51.725207 alacorder-81.1.4/alacorder/.mypy_cache/3.10/gzip.meta.json
+-rw-r--r--   0        0        0    26918 2023-07-27 22:51:51.207472 alacorder-81.1.4/alacorder/.mypy_cache/3.10/hashlib.data.json
+-rw-r--r--   0        0        0     1601 2023-07-27 22:51:51.207680 alacorder-81.1.4/alacorder/.mypy_cache/3.10/hashlib.meta.json
+-rw-r--r--   0        0        0     4718 2023-07-27 22:51:51.452697 alacorder-81.1.4/alacorder/.mypy_cache/3.10/html/__init__.data.json
+-rw-r--r--   0        0        0     1530 2023-07-27 22:51:51.453173 alacorder-81.1.4/alacorder/.mypy_cache/3.10/html/__init__.meta.json
+-rw-r--r--   0        0        0     2715 2023-07-27 22:51:50.897521 alacorder-81.1.4/alacorder/.mypy_cache/3.10/html/entities.data.json
+-rw-r--r--   0        0        0     1540 2023-07-27 22:51:50.897688 alacorder-81.1.4/alacorder/.mypy_cache/3.10/html/entities.meta.json
+-rw-r--r--   0        0        0    19478 2023-07-27 22:51:51.223671 alacorder-81.1.4/alacorder/.mypy_cache/3.10/http/__init__.data.json
+-rw-r--r--   0        0        0     1595 2023-07-27 22:51:51.223892 alacorder-81.1.4/alacorder/.mypy_cache/3.10/http/__init__.meta.json
+-rw-r--r--   0        0        0    67147 2023-07-27 22:51:52.395234 alacorder-81.1.4/alacorder/.mypy_cache/3.10/http/client.data.json
+-rw-r--r--   0        0        0     1737 2023-07-27 22:51:52.395462 alacorder-81.1.4/alacorder/.mypy_cache/3.10/http/client.meta.json
+-rw-r--r--   0        0        0    58566 2023-07-27 22:51:53.073704 alacorder-81.1.4/alacorder/.mypy_cache/3.10/http/cookiejar.data.json
+-rw-r--r--   0        0        0     1706 2023-07-27 22:51:53.073962 alacorder-81.1.4/alacorder/.mypy_cache/3.10/http/cookiejar.meta.json
+-rw-r--r--   0        0        0     6120 2023-07-27 22:51:50.817513 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1595 2023-07-27 22:51:50.817676 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    69978 2023-07-27 22:51:50.817040 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1688 2023-07-27 22:51:50.817248 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64518 2023-07-27 22:51:50.815376 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1702 2023-07-27 22:51:50.815604 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    92848 2023-07-27 22:51:50.813846 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1739 2023-07-27 22:51:50.814059 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12298 2023-07-27 22:51:50.811888 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1583 2023-07-27 22:51:50.812059 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    10969 2023-07-27 22:51:51.075403 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/resources/__init__.data.json
+-rw-r--r--   0        0        0     1709 2023-07-27 22:51:51.075706 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/resources/__init__.meta.json
+-rw-r--r--   0        0        0    22943 2023-07-27 22:51:51.141569 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/util.data.json
+-rw-r--r--   0        0        0     1682 2023-07-27 22:51:51.141766 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib/util.meta.json
+-rw-r--r--   0        0        0    94512 2023-07-27 22:51:52.963883 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/__init__.data.json
+-rw-r--r--   0        0        0     2173 2023-07-27 22:51:52.964083 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/__init__.meta.json
+-rw-r--r--   0        0        0     6489 2023-07-27 22:51:52.181063 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_adapters.data.json
+-rw-r--r--   0        0        0     1791 2023-07-27 22:51:52.181354 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_adapters.meta.json
+-rw-r--r--   0        0        0    24163 2023-07-27 22:51:50.899748 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_collections.data.json
+-rw-r--r--   0        0        0     1573 2023-07-27 22:51:50.899935 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_collections.meta.json
+-rw-r--r--   0        0        0     5220 2023-07-27 22:51:51.630671 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_compat.data.json
+-rw-r--r--   0        0        0     1598 2023-07-27 22:51:51.630854 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_compat.meta.json
+-rw-r--r--   0        0        0     2108 2023-07-27 22:51:51.629672 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_functools.data.json
+-rw-r--r--   0        0        0     1581 2023-07-27 22:51:51.629837 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_functools.meta.json
+-rw-r--r--   0        0        0     2083 2023-07-27 22:51:51.629119 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_itertools.data.json
+-rw-r--r--   0        0        0     1592 2023-07-27 22:51:51.629294 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_itertools.meta.json
+-rw-r--r--   0        0        0    24956 2023-07-27 22:51:50.901918 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_meta.data.json
+-rw-r--r--   0        0        0     1540 2023-07-27 22:51:50.902103 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_meta.meta.json
+-rw-r--r--   0        0        0     3280 2023-07-27 22:51:52.961498 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_py39compat.data.json
+-rw-r--r--   0        0        0     1621 2023-07-27 22:51:52.961771 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_py39compat.meta.json
+-rw-r--r--   0        0        0     5393 2023-07-27 22:51:51.919410 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_text.data.json
+-rw-r--r--   0        0        0     1587 2023-07-27 22:51:51.919607 alacorder-81.1.4/alacorder/.mypy_cache/3.10/importlib_metadata/_text.meta.json
+-rw-r--r--   0        0        0   363821 2023-07-27 22:51:52.159840 alacorder-81.1.4/alacorder/.mypy_cache/3.10/inspect.data.json
+-rw-r--r--   0        0        0     1701 2023-07-27 22:51:52.160352 alacorder-81.1.4/alacorder/.mypy_cache/3.10/inspect.meta.json
+-rw-r--r--   0        0        0    87436 2023-07-27 22:51:50.811293 alacorder-81.1.4/alacorder/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1628 2023-07-27 22:51:50.811463 alacorder-81.1.4/alacorder/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0   154066 2023-07-27 22:51:51.032942 alacorder-81.1.4/alacorder/.mypy_cache/3.10/ipaddress.data.json
+-rw-r--r--   0        0        0     1606 2023-07-27 22:51:51.033233 alacorder-81.1.4/alacorder/.mypy_cache/3.10/ipaddress.meta.json
+-rw-r--r--   0        0        0   343687 2023-07-27 22:51:51.494975 alacorder-81.1.4/alacorder/.mypy_cache/3.10/itertools.data.json
+-rw-r--r--   0        0        0     1619 2023-07-27 22:51:51.495270 alacorder-81.1.4/alacorder/.mypy_cache/3.10/itertools.meta.json
+-rw-r--r--   0        0        0    15484 2023-07-27 22:51:51.823228 alacorder-81.1.4/alacorder/.mypy_cache/3.10/json/__init__.data.json
+-rw-r--r--   0        0        0     1618 2023-07-27 22:51:51.823467 alacorder-81.1.4/alacorder/.mypy_cache/3.10/json/__init__.meta.json
+-rw-r--r--   0        0        0    14499 2023-07-27 22:51:51.186668 alacorder-81.1.4/alacorder/.mypy_cache/3.10/json/decoder.data.json
+-rw-r--r--   0        0        0     1560 2023-07-27 22:51:51.186926 alacorder-81.1.4/alacorder/.mypy_cache/3.10/json/decoder.meta.json
+-rw-r--r--   0        0        0    10879 2023-07-27 22:51:51.184567 alacorder-81.1.4/alacorder/.mypy_cache/3.10/json/encoder.data.json
+-rw-r--r--   0        0        0     1569 2023-07-27 22:51:51.184881 alacorder-81.1.4/alacorder/.mypy_cache/3.10/json/encoder.meta.json
+-rw-r--r--   0        0        0     3653 2023-07-27 22:51:51.008157 alacorder-81.1.4/alacorder/.mypy_cache/3.10/keyword.data.json
+-rw-r--r--   0        0        0     1602 2023-07-27 22:51:51.008341 alacorder-81.1.4/alacorder/.mypy_cache/3.10/keyword.meta.json
+-rw-r--r--   0        0        0     9293 2023-07-27 22:51:51.304910 alacorder-81.1.4/alacorder/.mypy_cache/3.10/linecache.data.json
+-rw-r--r--   0        0        0     1583 2023-07-27 22:51:51.305098 alacorder-81.1.4/alacorder/.mypy_cache/3.10/linecache.meta.json
+-rw-r--r--   0        0        0    31946 2023-07-27 22:51:52.200440 alacorder-81.1.4/alacorder/.mypy_cache/3.10/locale.data.json
+-rw-r--r--   0        0        0     1651 2023-07-27 22:51:52.200640 alacorder-81.1.4/alacorder/.mypy_cache/3.10/locale.meta.json
+-rw-r--r--   0        0        0   144612 2023-07-27 22:51:51.801496 alacorder-81.1.4/alacorder/.mypy_cache/3.10/logging/__init__.data.json
+-rw-r--r--   0        0        0     1694 2023-07-27 22:51:51.801773 alacorder-81.1.4/alacorder/.mypy_cache/3.10/logging/__init__.meta.json
+-rw-r--r--   0        0        0    51570 2023-07-27 22:51:52.015911 alacorder-81.1.4/alacorder/.mypy_cache/3.10/logging/config.data.json
+-rw-r--r--   0        0        0     1684 2023-07-27 22:51:52.016127 alacorder-81.1.4/alacorder/.mypy_cache/3.10/logging/config.meta.json
+-rw-r--r--   0        0        0     2404 2023-07-27 22:51:53.051800 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/__init__.data.json
+-rw-r--r--   0        0        0     1589 2023-07-27 22:51:53.051964 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/__init__.meta.json
+-rw-r--r--   0        0        0     2022 2023-07-27 22:51:51.706703 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/_compat.data.json
+-rw-r--r--   0        0        0     1596 2023-07-27 22:51:51.706888 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/_compat.meta.json
+-rw-r--r--   0        0        0     4657 2023-07-27 22:51:50.929885 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/_punycode.data.json
+-rw-r--r--   0        0        0     1561 2023-07-27 22:51:50.930064 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/_punycode.meta.json
+-rw-r--r--   0        0        0     1565 2023-07-27 22:51:50.982674 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/__init__.data.json
+-rw-r--r--   0        0        0     1535 2023-07-27 22:51:50.983013 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/__init__.meta.json
+-rw-r--r--   0        0        0     1736 2023-07-27 22:51:51.644376 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/entities.data.json
+-rw-r--r--   0        0        0     1603 2023-07-27 22:51:51.644586 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/entities.meta.json
+-rw-r--r--   0        0        0     1685 2023-07-27 22:51:50.890049 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/html_blocks.data.json
+-rw-r--r--   0        0        0     1552 2023-07-27 22:51:50.890232 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/html_blocks.meta.json
+-rw-r--r--   0        0        0     4972 2023-07-27 22:51:50.889368 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/html_re.data.json
+-rw-r--r--   0        0        0     1554 2023-07-27 22:51:50.889572 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/html_re.meta.json
+-rw-r--r--   0        0        0     5733 2023-07-27 22:51:53.050494 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/normalize_url.data.json
+-rw-r--r--   0        0        0     1729 2023-07-27 22:51:53.050660 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/normalize_url.meta.json
+-rw-r--r--   0        0        0    14161 2023-07-27 22:51:51.973027 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/utils.data.json
+-rw-r--r--   0        0        0     1609 2023-07-27 22:51:51.973209 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/common/utils.meta.json
+-rw-r--r--   0        0        0     2565 2023-07-27 22:51:53.049057 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/helpers/__init__.data.json
+-rw-r--r--   0        0        0     1717 2023-07-27 22:51:53.049254 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/helpers/__init__.meta.json
+-rw-r--r--   0        0        0     5233 2023-07-27 22:51:52.185659 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/helpers/parse_link_destination.data.json
+-rw-r--r--   0        0        0     1651 2023-07-27 22:51:52.185852 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/helpers/parse_link_destination.meta.json
+-rw-r--r--   0        0        0     2318 2023-07-27 22:51:53.048224 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/helpers/parse_link_label.data.json
+-rw-r--r--   0        0        0     1709 2023-07-27 22:51:53.048393 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/helpers/parse_link_label.meta.json
+-rw-r--r--   0        0        0     5369 2023-07-27 22:51:52.184786 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/helpers/parse_link_title.data.json
+-rw-r--r--   0        0        0     1639 2023-07-27 22:51:52.184990 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/helpers/parse_link_title.meta.json
+-rw-r--r--   0        0        0    25144 2023-07-27 22:51:53.051442 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/main.data.json
+-rw-r--r--   0        0        0     2242 2023-07-27 22:51:53.051608 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/main.meta.json
+-rw-r--r--   0        0        0     5869 2023-07-27 22:51:53.050047 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/parser_block.data.json
+-rw-r--r--   0        0        0     2230 2023-07-27 22:51:53.050220 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/parser_block.meta.json
+-rw-r--r--   0        0        0     4913 2023-07-27 22:51:53.048654 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/parser_core.data.json
+-rw-r--r--   0        0        0     1934 2023-07-27 22:51:53.048845 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/parser_core.meta.json
+-rw-r--r--   0        0        0     7118 2023-07-27 22:51:53.049576 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/parser_inline.data.json
+-rw-r--r--   0        0        0     2331 2023-07-27 22:51:53.049770 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/parser_inline.meta.json
+-rw-r--r--   0        0        0     4147 2023-07-27 22:51:51.683963 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/presets/__init__.data.json
+-rw-r--r--   0        0        0     1657 2023-07-27 22:51:51.684158 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/presets/__init__.meta.json
+-rw-r--r--   0        0        0     1648 2023-07-27 22:51:50.928851 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/presets/commonmark.data.json
+-rw-r--r--   0        0        0     1553 2023-07-27 22:51:50.929031 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/presets/commonmark.meta.json
+-rw-r--r--   0        0        0     1624 2023-07-27 22:51:50.928342 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/presets/default.data.json
+-rw-r--r--   0        0        0     1547 2023-07-27 22:51:50.928508 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/presets/default.meta.json
+-rw-r--r--   0        0        0     1600 2023-07-27 22:51:50.927801 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/presets/zero.data.json
+-rw-r--r--   0        0        0     1541 2023-07-27 22:51:50.927987 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/presets/zero.meta.json
+-rw-r--r--   0        0        0    20478 2023-07-27 22:51:52.196626 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/renderer.data.json
+-rw-r--r--   0        0        0     1740 2023-07-27 22:51:52.196839 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/renderer.meta.json
+-rw-r--r--   0        0        0    24213 2023-07-27 22:51:53.030286 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/ruler.data.json
+-rw-r--r--   0        0        0     1726 2023-07-27 22:51:53.030602 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/ruler.meta.json
+-rw-r--r--   0        0        0     3634 2023-07-27 22:51:53.047452 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/__init__.data.json
+-rw-r--r--   0        0        0     2058 2023-07-27 22:51:53.047639 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/__init__.meta.json
+-rw-r--r--   0        0        0     2877 2023-07-27 22:51:53.043775 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/blockquote.data.json
+-rw-r--r--   0        0        0     1734 2023-07-27 22:51:53.043966 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/blockquote.meta.json
+-rw-r--r--   0        0        0     2592 2023-07-27 22:51:53.043359 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/code.data.json
+-rw-r--r--   0        0        0     1673 2023-07-27 22:51:53.043549 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/code.meta.json
+-rw-r--r--   0        0        0     2605 2023-07-27 22:51:53.042941 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/fence.data.json
+-rw-r--r--   0        0        0     1676 2023-07-27 22:51:53.043134 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/fence.meta.json
+-rw-r--r--   0        0        0     2838 2023-07-27 22:51:53.042522 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/heading.data.json
+-rw-r--r--   0        0        0     1728 2023-07-27 22:51:53.042718 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/heading.meta.json
+-rw-r--r--   0        0        0     2666 2023-07-27 22:51:53.042083 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/hr.data.json
+-rw-r--r--   0        0        0     1701 2023-07-27 22:51:53.042290 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/hr.meta.json
+-rw-r--r--   0        0        0     3868 2023-07-27 22:51:53.041657 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/html_block.data.json
+-rw-r--r--   0        0        0     1795 2023-07-27 22:51:53.041858 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/html_block.meta.json
+-rw-r--r--   0        0        0     2733 2023-07-27 22:51:53.041189 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/lheading.data.json
+-rw-r--r--   0        0        0     1681 2023-07-27 22:51:53.041393 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/lheading.meta.json
+-rw-r--r--   0        0        0     5071 2023-07-27 22:51:53.040763 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/list.data.json
+-rw-r--r--   0        0        0     1705 2023-07-27 22:51:53.040962 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/list.meta.json
+-rw-r--r--   0        0        0     2746 2023-07-27 22:51:53.040273 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/paragraph.data.json
+-rw-r--r--   0        0        0     1683 2023-07-27 22:51:53.040465 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/paragraph.meta.json
+-rw-r--r--   0        0        0     3187 2023-07-27 22:51:53.039829 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/reference.data.json
+-rw-r--r--   0        0        0     1715 2023-07-27 22:51:53.040032 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/reference.meta.json
+-rw-r--r--   0        0        0    13892 2023-07-27 22:51:53.032171 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/state_block.data.json
+-rw-r--r--   0        0        0     1752 2023-07-27 22:51:53.032358 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/state_block.meta.json
+-rw-r--r--   0        0        0     4172 2023-07-27 22:51:53.039363 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/table.data.json
+-rw-r--r--   0        0        0     1702 2023-07-27 22:51:53.039584 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_block/table.meta.json
+-rw-r--r--   0        0        0     3019 2023-07-27 22:51:53.047847 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/__init__.data.json
+-rw-r--r--   0        0        0     1865 2023-07-27 22:51:53.048010 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/__init__.meta.json
+-rw-r--r--   0        0        0     2213 2023-07-27 22:51:53.046595 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/block.data.json
+-rw-r--r--   0        0        0     1680 2023-07-27 22:51:53.046792 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/block.meta.json
+-rw-r--r--   0        0        0     2136 2023-07-27 22:51:53.046156 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/inline.data.json
+-rw-r--r--   0        0        0     1658 2023-07-27 22:51:53.046363 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/inline.meta.json
+-rw-r--r--   0        0        0     5040 2023-07-27 22:51:53.045726 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/linkify.data.json
+-rw-r--r--   0        0        0     1738 2023-07-27 22:51:53.045926 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/linkify.meta.json
+-rw-r--r--   0        0        0     2789 2023-07-27 22:51:53.045238 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/normalize.data.json
+-rw-r--r--   0        0        0     1674 2023-07-27 22:51:53.045435 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/normalize.meta.json
+-rw-r--r--   0        0        0     8155 2023-07-27 22:51:53.044320 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/replacements.data.json
+-rw-r--r--   0        0        0     1754 2023-07-27 22:51:53.044518 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/replacements.meta.json
+-rw-r--r--   0        0        0     5219 2023-07-27 22:51:53.044797 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/smartquotes.data.json
+-rw-r--r--   0        0        0     1751 2023-07-27 22:51:53.045005 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/smartquotes.meta.json
+-rw-r--r--   0        0        0     4487 2023-07-27 22:51:53.032919 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/state_core.data.json
+-rw-r--r--   0        0        0     1731 2023-07-27 22:51:53.033216 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_core/state_core.meta.json
+-rw-r--r--   0        0        0     3921 2023-07-27 22:51:53.047034 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/__init__.data.json
+-rw-r--r--   0        0        0     2175 2023-07-27 22:51:53.047223 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/__init__.meta.json
+-rw-r--r--   0        0        0     2844 2023-07-27 22:51:53.037799 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/autolink.data.json
+-rw-r--r--   0        0        0     1681 2023-07-27 22:51:53.038014 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/autolink.meta.json
+-rw-r--r--   0        0        0     2561 2023-07-27 22:51:53.037365 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/backticks.data.json
+-rw-r--r--   0        0        0     1683 2023-07-27 22:51:53.037557 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/backticks.meta.json
+-rw-r--r--   0        0        0     3197 2023-07-27 22:51:53.036923 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/balance_pairs.data.json
+-rw-r--r--   0        0        0     1681 2023-07-27 22:51:53.037129 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/balance_pairs.meta.json
+-rw-r--r--   0        0        0     3419 2023-07-27 22:51:53.038820 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/emphasis.data.json
+-rw-r--r--   0        0        0     1717 2023-07-27 22:51:53.039063 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/emphasis.meta.json
+-rw-r--r--   0        0        0     3216 2023-07-27 22:51:53.036502 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/entity.data.json
+-rw-r--r--   0        0        0     1754 2023-07-27 22:51:53.036680 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/entity.meta.json
+-rw-r--r--   0        0        0     2814 2023-07-27 22:51:53.036055 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/escape.data.json
+-rw-r--r--   0        0        0     1723 2023-07-27 22:51:53.036260 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/escape.meta.json
+-rw-r--r--   0        0        0     3100 2023-07-27 22:51:53.035624 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/html_inline.data.json
+-rw-r--r--   0        0        0     1710 2023-07-27 22:51:53.035828 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/html_inline.meta.json
+-rw-r--r--   0        0        0     2670 2023-07-27 22:51:53.035171 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/image.data.json
+-rw-r--r--   0        0        0     1737 2023-07-27 22:51:53.035364 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/image.meta.json
+-rw-r--r--   0        0        0     2462 2023-07-27 22:51:53.034721 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/link.data.json
+-rw-r--r--   0        0        0     1694 2023-07-27 22:51:53.034924 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/link.meta.json
+-rw-r--r--   0        0        0     2820 2023-07-27 22:51:53.034268 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/newline.data.json
+-rw-r--r--   0        0        0     1710 2023-07-27 22:51:53.034478 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/newline.meta.json
+-rw-r--r--   0        0        0    36701 2023-07-27 22:51:53.031512 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/state_inline.data.json
+-rw-r--r--   0        0        0     1835 2023-07-27 22:51:53.031730 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/state_inline.meta.json
+-rw-r--r--   0        0        0     4140 2023-07-27 22:51:53.038281 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/strikethrough.data.json
+-rw-r--r--   0        0        0     1698 2023-07-27 22:51:53.038490 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/strikethrough.meta.json
+-rw-r--r--   0        0        0     2626 2023-07-27 22:51:53.033869 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/text.data.json
+-rw-r--r--   0        0        0     1663 2023-07-27 22:51:53.034044 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/text.meta.json
+-rw-r--r--   0        0        0     2410 2023-07-27 22:51:53.033461 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/text_collapse.data.json
+-rw-r--r--   0        0        0     1681 2023-07-27 22:51:53.033645 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/rules_inline/text_collapse.meta.json
+-rw-r--r--   0        0        0    23355 2023-07-27 22:51:52.078901 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/token.data.json
+-rw-r--r--   0        0        0     1686 2023-07-27 22:51:52.079130 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/token.meta.json
+-rw-r--r--   0        0        0    29602 2023-07-27 22:51:51.683145 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/utils.data.json
+-rw-r--r--   0        0        0     1590 2023-07-27 22:51:51.683343 alacorder-81.1.4/alacorder/.mypy_cache/3.10/markdown_it/utils.meta.json
+-rw-r--r--   0        0        0     6291 2023-07-27 22:51:51.409955 alacorder-81.1.4/alacorder/.mypy_cache/3.10/marshal.data.json
+-rw-r--r--   0        0        0     1581 2023-07-27 22:51:51.410191 alacorder-81.1.4/alacorder/.mypy_cache/3.10/marshal.meta.json
+-rw-r--r--   0        0        0    53668 2023-07-27 22:51:51.518768 alacorder-81.1.4/alacorder/.mypy_cache/3.10/math.data.json
+-rw-r--r--   0        0        0     1596 2023-07-27 22:51:51.519032 alacorder-81.1.4/alacorder/.mypy_cache/3.10/math.meta.json
+-rw-r--r--   0        0        0     3261 2023-07-27 22:51:52.186300 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/__init__.data.json
+-rw-r--r--   0        0        0     1655 2023-07-27 22:51:52.186491 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/__init__.meta.json
+-rw-r--r--   0        0        0     4593 2023-07-27 22:51:51.628464 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/_decode.data.json
+-rw-r--r--   0        0        0     1585 2023-07-27 22:51:51.628645 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/_decode.meta.json
+-rw-r--r--   0        0        0     4260 2023-07-27 22:51:51.627619 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/_encode.data.json
+-rw-r--r--   0        0        0     1590 2023-07-27 22:51:51.627807 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/_encode.meta.json
+-rw-r--r--   0        0        0     2182 2023-07-27 22:51:51.937583 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/_format.data.json
+-rw-r--r--   0        0        0     1552 2023-07-27 22:51:51.937772 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/_format.meta.json
+-rw-r--r--   0        0        0    12471 2023-07-27 22:51:51.936860 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/_parse.data.json
+-rw-r--r--   0        0        0     1638 2023-07-27 22:51:51.937098 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/_parse.meta.json
+-rw-r--r--   0        0        0    27630 2023-07-27 22:51:51.626724 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/_url.data.json
+-rw-r--r--   0        0        0     1528 2023-07-27 22:51:51.626909 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mdurl/_url.meta.json
+-rw-r--r--   0        0        0    15230 2023-07-27 22:51:51.102901 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mimetypes.data.json
+-rw-r--r--   0        0        0     1591 2023-07-27 22:51:51.103089 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mimetypes.meta.json
+-rw-r--r--   0        0        0    28224 2023-07-27 22:51:51.511502 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1595 2023-07-27 22:51:51.511715 alacorder-81.1.4/alacorder/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0     1501 2023-07-27 22:51:51.157711 alacorder-81.1.4/alacorder/.mypy_cache/3.10/msvcrt.data.json
+-rw-r--r--   0        0        0     1561 2023-07-27 22:51:51.157906 alacorder-81.1.4/alacorder/.mypy_cache/3.10/msvcrt.meta.json
+-rw-r--r--   0        0        0    33072 2023-07-27 22:51:52.904754 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     2008 2023-07-27 22:51:52.904940 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    31335 2023-07-27 22:51:51.922946 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1681 2023-07-27 22:51:51.923149 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0    99036 2023-07-27 22:51:52.903777 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2158 2023-07-27 22:51:52.903975 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   170589 2023-07-27 22:51:52.900646 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1822 2023-07-27 22:51:52.900996 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    58315 2023-07-27 22:51:50.887243 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1640 2023-07-27 22:51:50.887497 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9013 2023-07-27 22:51:52.162412 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1676 2023-07-27 22:51:52.162623 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     5736 2023-07-27 22:51:52.539269 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1715 2023-07-27 22:51:52.539447 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     6406 2023-07-27 22:51:52.538829 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1717 2023-07-27 22:51:52.539017 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     1972 2023-07-27 22:51:52.160910 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1690 2023-07-27 22:51:52.161122 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    17681 2023-07-27 22:51:50.881864 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1610 2023-07-27 22:51:50.882066 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    26379 2023-07-27 22:51:50.892865 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1598 2023-07-27 22:51:50.893067 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    28828 2023-07-27 22:51:52.538286 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1794 2023-07-27 22:51:52.538549 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    32117 2023-07-27 22:51:50.878238 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1658 2023-07-27 22:51:50.878437 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    74911 2023-07-27 22:51:52.540897 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1781 2023-07-27 22:51:52.541071 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0     9817 2023-07-27 22:51:50.879637 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1589 2023-07-27 22:51:50.879809 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    25542 2023-07-27 22:51:52.901683 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1734 2023-07-27 22:51:52.901872 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    23499 2023-07-27 22:51:51.916626 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1647 2023-07-27 22:51:51.916841 alacorder-81.1.4/alacorder/.mypy_cache/3.10/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0     5893 2023-07-27 22:51:53.804581 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/__init__.data.json
+-rw-r--r--   0        0        0     1828 2023-07-27 22:51:53.804760 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/__init__.meta.json
+-rw-r--r--   0        0        0     1572 2023-07-27 22:51:50.953182 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/_imports.data.json
+-rw-r--r--   0        0        0     1527 2023-07-27 22:51:50.953361 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/_imports.meta.json
+-rw-r--r--   0        0        0     6692 2023-07-27 22:51:50.954735 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/_struct.data.json
+-rw-r--r--   0        0        0     1526 2023-07-27 22:51:50.954918 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/_struct.meta.json
+-rw-r--r--   0        0        0     2966 2023-07-27 22:51:53.723075 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/_version.data.json
+-rw-r--r--   0        0        0     1700 2023-07-27 22:51:53.723307 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/_version.meta.json
+-rw-r--r--   0        0        0     1878 2023-07-27 22:51:53.804147 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/converter.data.json
+-rw-r--r--   0        0        0     1634 2023-07-27 22:51:53.804313 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/converter.meta.json
+-rw-r--r--   0        0        0     1541 2023-07-27 22:51:50.898017 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/corpus/__init__.data.json
+-rw-r--r--   0        0        0     1529 2023-07-27 22:51:50.898190 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/corpus/__init__.meta.json
+-rw-r--r--   0        0        0     1687 2023-07-27 22:51:51.644986 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/corpus/words.data.json
+-rw-r--r--   0        0        0     1546 2023-07-27 22:51:51.645196 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/corpus/words.meta.json
+-rw-r--r--   0        0        0    10823 2023-07-27 22:51:50.952510 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/json_compat.data.json
+-rw-r--r--   0        0        0     1582 2023-07-27 22:51:50.952728 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/json_compat.meta.json
+-rw-r--r--   0        0        0     3210 2023-07-27 22:51:51.684768 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/notebooknode.data.json
+-rw-r--r--   0        0        0     1580 2023-07-27 22:51:51.684957 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/notebooknode.meta.json
+-rw-r--r--   0        0        0     3256 2023-07-27 22:51:51.975930 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/reader.data.json
+-rw-r--r--   0        0        0     1560 2023-07-27 22:51:51.976100 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/reader.meta.json
+-rw-r--r--   0        0        0     3072 2023-07-27 22:51:50.983995 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/sentinel.data.json
+-rw-r--r--   0        0        0     1526 2023-07-27 22:51:50.984241 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/sentinel.meta.json
+-rw-r--r--   0        0        0     2513 2023-07-27 22:51:52.201682 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v1/__init__.data.json
+-rw-r--r--   0        0        0     1645 2023-07-27 22:51:52.201862 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v1/__init__.meta.json
+-rw-r--r--   0        0        0     1591 2023-07-27 22:51:50.956256 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v1/convert.data.json
+-rw-r--r--   0        0        0     1530 2023-07-27 22:51:50.956615 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v1/convert.meta.json
+-rw-r--r--   0        0        0     3339 2023-07-27 22:51:51.646988 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v1/nbbase.data.json
+-rw-r--r--   0        0        0     1553 2023-07-27 22:51:51.647196 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v1/nbbase.meta.json
+-rw-r--r--   0        0        0     8410 2023-07-27 22:51:51.963222 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v1/nbjson.data.json
+-rw-r--r--   0        0        0     1665 2023-07-27 22:51:51.963412 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v1/nbjson.meta.json
+-rw-r--r--   0        0        0     3854 2023-07-27 22:51:50.904016 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v1/rwbase.data.json
+-rw-r--r--   0        0        0     1529 2023-07-27 22:51:50.904222 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v1/rwbase.meta.json
+-rw-r--r--   0        0        0     4545 2023-07-27 22:51:52.201160 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/__init__.data.json
+-rw-r--r--   0        0        0     1706 2023-07-27 22:51:52.201345 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/__init__.meta.json
+-rw-r--r--   0        0        0     2268 2023-07-27 22:51:51.962136 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/convert.data.json
+-rw-r--r--   0        0        0     1557 2023-07-27 22:51:51.962309 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/convert.meta.json
+-rw-r--r--   0        0        0     4774 2023-07-27 22:51:51.646142 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/nbbase.data.json
+-rw-r--r--   0        0        0     1553 2023-07-27 22:51:51.646351 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/nbbase.meta.json
+-rw-r--r--   0        0        0     9799 2023-07-27 22:51:51.961563 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/nbjson.data.json
+-rw-r--r--   0        0        0     1698 2023-07-27 22:51:51.961737 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/nbjson.meta.json
+-rw-r--r--   0        0        0    10643 2023-07-27 22:51:51.960324 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/nbpy.data.json
+-rw-r--r--   0        0        0     1672 2023-07-27 22:51:51.960515 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/nbpy.meta.json
+-rw-r--r--   0        0        0     2306 2023-07-27 22:51:50.955396 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/nbxml.data.json
+-rw-r--r--   0        0        0     1526 2023-07-27 22:51:50.955580 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/nbxml.meta.json
+-rw-r--r--   0        0        0     5647 2023-07-27 22:51:51.632935 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/rwbase.data.json
+-rw-r--r--   0        0        0     1543 2023-07-27 22:51:51.633113 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v2/rwbase.meta.json
+-rw-r--r--   0        0        0     4675 2023-07-27 22:51:52.964717 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/__init__.data.json
+-rw-r--r--   0        0        0     1681 2023-07-27 22:51:52.964912 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/__init__.meta.json
+-rw-r--r--   0        0        0     2844 2023-07-27 22:51:52.189882 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/convert.data.json
+-rw-r--r--   0        0        0     1599 2023-07-27 22:51:52.190103 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/convert.meta.json
+-rw-r--r--   0        0        0     6734 2023-07-27 22:51:51.958854 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/nbbase.data.json
+-rw-r--r--   0        0        0     1570 2023-07-27 22:51:51.959062 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/nbbase.meta.json
+-rw-r--r--   0        0        0     9803 2023-07-27 22:51:52.189088 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/nbjson.data.json
+-rw-r--r--   0        0        0     1738 2023-07-27 22:51:52.189292 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/nbjson.meta.json
+-rw-r--r--   0        0        0    10970 2023-07-27 22:51:52.187810 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/nbpy.data.json
+-rw-r--r--   0        0        0     1758 2023-07-27 22:51:52.187998 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/nbpy.meta.json
+-rw-r--r--   0        0        0     6182 2023-07-27 22:51:51.631873 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/rwbase.data.json
+-rw-r--r--   0        0        0     1542 2023-07-27 22:51:51.632059 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v3/rwbase.meta.json
+-rw-r--r--   0        0        0     5758 2023-07-27 22:51:53.803765 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v4/__init__.data.json
+-rw-r--r--   0        0        0     1645 2023-07-27 22:51:53.803948 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v4/__init__.meta.json
+-rw-r--r--   0        0        0     5427 2023-07-27 22:51:53.803236 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v4/convert.data.json
+-rw-r--r--   0        0        0     1706 2023-07-27 22:51:53.803466 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v4/convert.meta.json
+-rw-r--r--   0        0        0     4548 2023-07-27 22:51:51.957493 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v4/nbbase.data.json
+-rw-r--r--   0        0        0     1587 2023-07-27 22:51:51.957700 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v4/nbbase.meta.json
+-rw-r--r--   0        0        0     9806 2023-07-27 22:51:51.956002 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v4/nbjson.data.json
+-rw-r--r--   0        0        0     1627 2023-07-27 22:51:51.956215 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v4/nbjson.meta.json
+-rw-r--r--   0        0        0     5780 2023-07-27 22:51:50.903108 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v4/rwbase.data.json
+-rw-r--r--   0        0        0     1529 2023-07-27 22:51:50.903291 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/v4/rwbase.meta.json
+-rw-r--r--   0        0        0    15803 2023-07-27 22:51:51.975527 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/validator.data.json
+-rw-r--r--   0        0        0     1740 2023-07-27 22:51:51.975709 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/validator.meta.json
+-rw-r--r--   0        0        0     2959 2023-07-27 22:51:50.930648 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/warnings.data.json
+-rw-r--r--   0        0        0     1526 2023-07-27 22:51:50.930830 alacorder-81.1.4/alacorder/.mypy_cache/3.10/nbformat/warnings.meta.json
+-rw-r--r--   0        0        0    78977 2023-07-27 22:51:51.181611 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numbers.data.json
+-rw-r--r--   0        0        0     1527 2023-07-27 22:51:51.181803 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numbers.meta.json
+-rw-r--r--   0        0        0  2406345 2023-07-27 22:51:53.642049 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3090 2023-07-27 22:51:53.642646 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     4935 2023-07-27 22:51:51.080791 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1552 2023-07-27 22:51:51.080977 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0    21339 2023-07-27 22:51:53.537525 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/__init__.data.json
+-rw-r--r--   0        0        0     1938 2023-07-27 22:51:53.537699 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/__init__.meta.json
+-rw-r--r--   0        0        0     3522 2023-07-27 22:51:53.679017 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1711 2023-07-27 22:51:53.679181 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    27411 2023-07-27 22:51:53.531660 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_array_like.data.json
+-rw-r--r--   0        0        0     1727 2023-07-27 22:51:53.531834 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_array_like.meta.json
+-rw-r--r--   0        0        0   301493 2023-07-27 22:51:53.594526 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_callable.data.json
+-rw-r--r--   0        0        0     1767 2023-07-27 22:51:53.594732 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_callable.meta.json
+-rw-r--r--   0        0        0    41701 2023-07-27 22:51:51.041027 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1542 2023-07-27 22:51:51.041241 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    31693 2023-07-27 22:51:53.526166 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1721 2023-07-27 22:51:53.526346 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     5739 2023-07-27 22:51:53.589362 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1636 2023-07-27 22:51:53.589541 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    34355 2023-07-27 22:51:53.524681 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1772 2023-07-27 22:51:53.524972 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4343 2023-07-27 22:51:51.041714 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_nbit.data.json
+-rw-r--r--   0        0        0     1529 2023-07-27 22:51:51.041897 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_nbit.meta.json
+-rw-r--r--   0        0        0    18772 2023-07-27 22:51:51.703648 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1594 2023-07-27 22:51:51.703843 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     5855 2023-07-27 22:51:53.525261 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_scalars.data.json
+-rw-r--r--   0        0        0     1591 2023-07-27 22:51:53.525439 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2295 2023-07-27 22:51:51.037089 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_shape.data.json
+-rw-r--r--   0        0        0     1531 2023-07-27 22:51:51.037300 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_shape.meta.json
+-rw-r--r--   0        0        0   305870 2023-07-27 22:51:53.684563 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1773 2023-07-27 22:51:53.684819 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_typing/_ufunc.meta.json
+-rw-r--r--   0        0        0     1836 2023-07-27 22:51:52.016515 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_version.data.json
+-rw-r--r--   0        0        0     1532 2023-07-27 22:51:52.016806 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/_version.meta.json
+-rw-r--r--   0        0        0     5029 2023-07-27 22:51:51.954611 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/compat/__init__.data.json
+-rw-r--r--   0        0        0     1579 2023-07-27 22:51:51.954839 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/compat/__init__.meta.json
+-rw-r--r--   0        0        0     5809 2023-07-27 22:51:50.982147 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/compat/_inspect.data.json
+-rw-r--r--   0        0        0     1573 2023-07-27 22:51:50.982359 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/compat/_inspect.meta.json
+-rw-r--r--   0        0        0    11833 2023-07-27 22:51:51.624985 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/compat/py3k.data.json
+-rw-r--r--   0        0        0     1661 2023-07-27 22:51:51.625190 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/compat/py3k.meta.json
+-rw-r--r--   0        0        0     1501 2023-07-27 22:51:51.079869 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1522 2023-07-27 22:51:51.080048 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    14278 2023-07-27 22:51:53.580593 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1694 2023-07-27 22:51:53.580757 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    25007 2023-07-27 22:51:53.595381 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1639 2023-07-27 22:51:53.595558 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     4809 2023-07-27 22:51:53.580014 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1595 2023-07-27 22:51:53.580175 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    11206 2023-07-27 22:51:53.579593 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1618 2023-07-27 22:51:53.579774 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    27989 2023-07-27 22:51:53.579062 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1662 2023-07-27 22:51:53.579229 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   169925 2023-07-27 22:51:53.663445 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1740 2023-07-27 22:51:53.663648 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    37234 2023-07-27 22:51:53.578188 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1737 2023-07-27 22:51:53.578358 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0   358922 2023-07-27 22:51:53.587593 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1756 2023-07-27 22:51:53.587819 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    52023 2023-07-27 22:51:53.588918 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1721 2023-07-27 22:51:53.589088 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   319951 2023-07-27 22:51:53.577123 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1802 2023-07-27 22:51:53.577335 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   206356 2023-07-27 22:51:53.571011 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1758 2023-07-27 22:51:53.571199 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    49543 2023-07-27 22:51:53.567050 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1815 2023-07-27 22:51:53.567227 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    26497 2023-07-27 22:51:51.700807 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/overrides.data.json
+-rw-r--r--   0        0        0     1683 2023-07-27 22:51:51.701003 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/overrides.meta.json
+-rw-r--r--   0        0        0    53616 2023-07-27 22:51:53.660111 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1767 2023-07-27 22:51:53.660290 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    58993 2023-07-27 22:51:53.565805 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1736 2023-07-27 22:51:53.565976 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3045 2023-07-27 22:51:51.701683 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1577 2023-07-27 22:51:51.701864 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0   115848 2023-07-27 22:51:53.536809 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1850 2023-07-27 22:51:53.537004 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     4272 2023-07-27 22:51:53.673361 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1640 2023-07-27 22:51:53.673540 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    18731 2023-07-27 22:51:53.655626 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1701 2023-07-27 22:51:53.655794 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    22898 2023-07-27 22:51:53.654915 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1671 2023-07-27 22:51:53.655098 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    24294 2023-07-27 22:51:53.534312 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2208 2023-07-27 22:51:53.534504 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     8937 2023-07-27 22:51:51.035085 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1529 2023-07-27 22:51:51.035330 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    19247 2023-07-27 22:51:53.564413 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1676 2023-07-27 22:51:53.564589 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   163450 2023-07-27 22:51:53.563694 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1682 2023-07-27 22:51:53.563883 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    29500 2023-07-27 22:51:53.560644 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1668 2023-07-27 22:51:53.560815 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7021 2023-07-27 22:51:51.036321 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1524 2023-07-27 22:51:51.036545 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   234869 2023-07-27 22:51:53.559744 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1856 2023-07-27 22:51:53.559946 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0     8889 2023-07-27 22:51:53.555050 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1688 2023-07-27 22:51:53.555256 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    67747 2023-07-27 22:51:53.554480 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1769 2023-07-27 22:51:53.554700 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    47352 2023-07-27 22:51:53.654103 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1579 2023-07-27 22:51:53.654299 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    95419 2023-07-27 22:51:53.552803 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1783 2023-07-27 22:51:53.553021 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0   102217 2023-07-27 22:51:53.550679 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1875 2023-07-27 22:51:53.550895 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0    97284 2023-07-27 22:51:53.548364 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1681 2023-07-27 22:51:53.548562 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0    62206 2023-07-27 22:51:53.652650 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1673 2023-07-27 22:51:53.652902 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    96026 2023-07-27 22:51:53.546204 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1782 2023-07-27 22:51:53.546421 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    25234 2023-07-27 22:51:53.544114 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1707 2023-07-27 22:51:53.544320 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    82317 2023-07-27 22:51:53.543297 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1737 2023-07-27 22:51:53.543472 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0   106963 2023-07-27 22:51:53.541436 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1736 2023-07-27 22:51:53.541616 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    26587 2023-07-27 22:51:53.539220 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1677 2023-07-27 22:51:53.539392 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    27399 2023-07-27 22:51:53.538393 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1654 2023-07-27 22:51:53.538568 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5299 2023-07-27 22:51:53.658707 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1622 2023-07-27 22:51:53.658890 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   108226 2023-07-27 22:51:53.658254 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1721 2023-07-27 22:51:53.658445 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    27656 2023-07-27 22:51:53.533531 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1630 2023-07-27 22:51:53.533725 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   139753 2023-07-27 22:51:53.530003 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1649 2023-07-27 22:51:53.530209 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    23307 2023-07-27 22:51:53.530823 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1632 2023-07-27 22:51:53.531001 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    15179 2023-07-27 22:51:53.532281 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1618 2023-07-27 22:51:53.532449 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     2740 2023-07-27 22:51:53.532656 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1645 2023-07-27 22:51:53.532874 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6169 2023-07-27 22:51:53.526657 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1743 2023-07-27 22:51:53.526830 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4067 2023-07-27 22:51:53.672977 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1798 2023-07-27 22:51:53.673138 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    26978 2023-07-27 22:51:50.980624 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1545 2023-07-27 22:51:50.980865 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    16455 2023-07-27 22:51:53.651108 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1666 2023-07-27 22:51:53.651278 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    14167 2023-07-27 22:51:53.650456 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1662 2023-07-27 22:51:53.650644 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    14231 2023-07-27 22:51:53.649873 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1666 2023-07-27 22:51:53.650037 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    14006 2023-07-27 22:51:53.649271 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1664 2023-07-27 22:51:53.649455 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    14006 2023-07-27 22:51:53.648668 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1664 2023-07-27 22:51:53.648849 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    13085 2023-07-27 22:51:53.648060 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1668 2023-07-27 22:51:53.648245 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4630 2023-07-27 22:51:50.976742 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1545 2023-07-27 22:51:50.976915 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0     9795 2023-07-27 22:51:53.678629 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1796 2023-07-27 22:51:53.678796 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   253099 2023-07-27 22:51:53.678130 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1796 2023-07-27 22:51:53.678327 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    10568 2023-07-27 22:51:53.672088 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1713 2023-07-27 22:51:53.672267 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    15447 2023-07-27 22:51:53.671575 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1698 2023-07-27 22:51:53.671740 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    11379 2023-07-27 22:51:53.670941 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1711 2023-07-27 22:51:53.671132 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     8959 2023-07-27 22:51:53.670381 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1709 2023-07-27 22:51:53.670558 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    70001 2023-07-27 22:51:53.647408 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1764 2023-07-27 22:51:53.647632 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   323838 2023-07-27 22:51:53.669800 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1768 2023-07-27 22:51:53.670034 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     8688 2023-07-27 22:51:53.672574 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1648 2023-07-27 22:51:53.672749 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1597 2023-07-27 22:51:50.975817 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1543 2023-07-27 22:51:50.975985 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   124768 2023-07-27 22:51:53.645711 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1916 2023-07-27 22:51:53.645937 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0     2818 2023-07-27 22:51:53.679424 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     1656 2023-07-27 22:51:53.679589 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0     3241 2023-07-27 22:51:52.213510 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/version.data.json
+-rw-r--r--   0        0        0     1624 2023-07-27 22:51:52.213689 alacorder-81.1.4/alacorder/.mypy_cache/3.10/numpy/version.meta.json
+-rw-r--r--   0        0        0     6089 2023-07-27 22:51:51.170416 alacorder-81.1.4/alacorder/.mypy_cache/3.10/opcode.data.json
+-rw-r--r--   0        0        0     1579 2023-07-27 22:51:51.170620 alacorder-81.1.4/alacorder/.mypy_cache/3.10/opcode.meta.json
+-rw-r--r--   0        0        0    50523 2023-07-27 22:51:51.839925 alacorder-81.1.4/alacorder/.mypy_cache/3.10/operator.data.json
+-rw-r--r--   0        0        0     1600 2023-07-27 22:51:51.840142 alacorder-81.1.4/alacorder/.mypy_cache/3.10/operator.meta.json
+-rw-r--r--   0        0        0   335737 2023-07-27 22:51:50.809278 alacorder-81.1.4/alacorder/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1680 2023-07-27 22:51:50.809493 alacorder-81.1.4/alacorder/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     4903 2023-07-27 22:51:50.803018 alacorder-81.1.4/alacorder/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1555 2023-07-27 22:51:50.803190 alacorder-81.1.4/alacorder/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0    95861 2023-07-27 22:51:50.802568 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1637 2023-07-27 22:51:50.802757 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    94625 2023-07-27 22:51:52.210683 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pdb.data.json
+-rw-r--r--   0        0        0     1721 2023-07-27 22:51:52.210910 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pdb.meta.json
+-rw-r--r--   0        0        0    45593 2023-07-27 22:51:51.138862 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1599 2023-07-27 22:51:51.139113 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    33234 2023-07-27 22:51:51.423456 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pkgutil.data.json
+-rw-r--r--   0        0        0     1614 2023-07-27 22:51:51.423700 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pkgutil.meta.json
+-rw-r--r--   0        0        0    36327 2023-07-27 22:51:51.471250 alacorder-81.1.4/alacorder/.mypy_cache/3.10/platform.data.json
+-rw-r--r--   0        0        0     1558 2023-07-27 22:51:51.471448 alacorder-81.1.4/alacorder/.mypy_cache/3.10/platform.meta.json
+-rw-r--r--   0        0        0    19050 2023-07-27 22:51:54.406905 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/__init__.data.json
+-rw-r--r--   0        0        0     2203 2023-07-27 22:51:54.407100 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/__init__.meta.json
+-rw-r--r--   0        0        0     2077 2023-07-27 22:51:54.405791 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/_reexport.data.json
+-rw-r--r--   0        0        0     1756 2023-07-27 22:51:54.405997 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/_reexport.meta.json
+-rw-r--r--   0        0        0    16847 2023-07-27 22:51:54.353792 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/api.data.json
+-rw-r--r--   0        0        0     2074 2023-07-27 22:51:54.353993 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/api.meta.json
+-rw-r--r--   0        0        0    42714 2023-07-27 22:51:54.353089 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/config.data.json
+-rw-r--r--   0        0        0     1880 2023-07-27 22:51:54.353289 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/config.meta.json
+-rw-r--r--   0        0        0    19289 2023-07-27 22:51:54.404211 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/convert.data.json
+-rw-r--r--   0        0        0     2137 2023-07-27 22:51:54.404415 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/convert.meta.json
+-rw-r--r--   0        0        0     2062 2023-07-27 22:51:54.400969 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/dataframe/__init__.data.json
+-rw-r--r--   0        0        0     1709 2023-07-27 22:51:54.401170 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/dataframe/__init__.meta.json
+-rw-r--r--   0        0        0    14215 2023-07-27 22:51:54.332890 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/dataframe/_html.data.json
+-rw-r--r--   0        0        0     1826 2023-07-27 22:51:54.333074 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/dataframe/_html.meta.json
+-rw-r--r--   0        0        0   334582 2023-07-27 22:51:54.398673 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/dataframe/frame.data.json
+-rw-r--r--   0        0        0     3440 2023-07-27 22:51:54.398963 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/dataframe/frame.meta.json
+-rw-r--r--   0        0        0    42815 2023-07-27 22:51:54.374718 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/dataframe/groupby.data.json
+-rw-r--r--   0        0        0     2326 2023-07-27 22:51:54.374907 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/dataframe/groupby.meta.json
+-rw-r--r--   0        0        0     8892 2023-07-27 22:51:54.339208 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/datatypes/__init__.data.json
+-rw-r--r--   0        0        0     1842 2023-07-27 22:51:54.339381 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/datatypes/__init__.meta.json
+-rw-r--r--   0        0        0    80178 2023-07-27 22:51:54.337339 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/datatypes/classes.data.json
+-rw-r--r--   0        0        0     1912 2023-07-27 22:51:54.337533 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/datatypes/classes.meta.json
+-rw-r--r--   0        0        0     6904 2023-07-27 22:51:54.338731 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/datatypes/constants.data.json
+-rw-r--r--   0        0        0     1808 2023-07-27 22:51:54.338904 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/datatypes/constants.meta.json
+-rw-r--r--   0        0        0    10548 2023-07-27 22:51:54.335575 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/datatypes/constructor.data.json
+-rw-r--r--   0        0        0     1958 2023-07-27 22:51:54.335764 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/datatypes/constructor.meta.json
+-rw-r--r--   0        0        0    32809 2023-07-27 22:51:54.338298 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/datatypes/convert.data.json
+-rw-r--r--   0        0        0     1945 2023-07-27 22:51:54.338472 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/datatypes/convert.meta.json
+-rw-r--r--   0        0        0    16033 2023-07-27 22:51:53.741625 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/dependencies.data.json
+-rw-r--r--   0        0        0     1916 2023-07-27 22:51:53.741850 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/dependencies.meta.json
+-rw-r--r--   0        0        0    11480 2023-07-27 22:51:51.436442 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/exceptions.data.json
+-rw-r--r--   0        0        0     1546 2023-07-27 22:51:51.436635 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/exceptions.meta.json
+-rw-r--r--   0        0        0     2001 2023-07-27 22:51:54.400555 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/__init__.data.json
+-rw-r--r--   0        0        0     1693 2023-07-27 22:51:54.400758 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/__init__.meta.json
+-rw-r--r--   0        0        0     6313 2023-07-27 22:51:54.348044 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/array.data.json
+-rw-r--r--   0        0        0     1754 2023-07-27 22:51:54.348236 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/array.meta.json
+-rw-r--r--   0        0        0     7533 2023-07-27 22:51:54.347541 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/binary.data.json
+-rw-r--r--   0        0        0     1784 2023-07-27 22:51:54.347749 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/binary.meta.json
+-rw-r--r--   0        0        0     5364 2023-07-27 22:51:54.347029 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/categorical.data.json
+-rw-r--r--   0        0        0     1793 2023-07-27 22:51:54.347230 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/categorical.meta.json
+-rw-r--r--   0        0        0    34926 2023-07-27 22:51:54.365355 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/datetime.data.json
+-rw-r--r--   0        0        0     1993 2023-07-27 22:51:54.365530 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/datetime.meta.json
+-rw-r--r--   0        0        0   346368 2023-07-27 22:51:54.391556 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/expr.data.json
+-rw-r--r--   0        0        0     2579 2023-07-27 22:51:54.391785 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/expr.meta.json
+-rw-r--r--   0        0        0    30885 2023-07-27 22:51:54.364433 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/list.data.json
+-rw-r--r--   0        0        0     2044 2023-07-27 22:51:54.364603 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/list.meta.json
+-rw-r--r--   0        0        0    21541 2023-07-27 22:51:54.346551 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/meta.data.json
+-rw-r--r--   0        0        0     1803 2023-07-27 22:51:54.346750 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/meta.meta.json
+-rw-r--r--   0        0        0    34082 2023-07-27 22:51:54.363547 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/string.data.json
+-rw-r--r--   0        0        0     1981 2023-07-27 22:51:54.363726 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/string.meta.json
+-rw-r--r--   0        0        0     6012 2023-07-27 22:51:54.345781 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/struct.data.json
+-rw-r--r--   0        0        0     1756 2023-07-27 22:51:54.345978 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/expr/struct.meta.json
+-rw-r--r--   0        0        0     8755 2023-07-27 22:51:54.400150 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/__init__.data.json
+-rw-r--r--   0        0        0     1906 2023-07-27 22:51:54.400319 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/__init__.meta.json
+-rw-r--r--   0        0        0     3484 2023-07-27 22:51:54.385278 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/aggregation/__init__.data.json
+-rw-r--r--   0        0        0     1795 2023-07-27 22:51:54.385440 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/aggregation/__init__.meta.json
+-rw-r--r--   0        0        0     8041 2023-07-27 22:51:54.362583 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/aggregation/horizontal.data.json
+-rw-r--r--   0        0        0     1968 2023-07-27 22:51:54.362763 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/aggregation/horizontal.meta.json
+-rw-r--r--   0        0        0    32178 2023-07-27 22:51:54.362105 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/aggregation/vertical.data.json
+-rw-r--r--   0        0        0     2056 2023-07-27 22:51:54.362288 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/aggregation/vertical.meta.json
+-rw-r--r--   0        0        0    19317 2023-07-27 22:51:54.371724 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/as_datatype.data.json
+-rw-r--r--   0        0        0     2090 2023-07-27 22:51:54.371897 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/as_datatype.meta.json
+-rw-r--r--   0        0        0     8294 2023-07-27 22:51:54.350440 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/eager.data.json
+-rw-r--r--   0        0        0     2099 2023-07-27 22:51:54.350642 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/eager.meta.json
+-rw-r--r--   0        0        0    77857 2023-07-27 22:51:54.370999 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/lazy.data.json
+-rw-r--r--   0        0        0     2271 2023-07-27 22:51:54.371186 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/lazy.meta.json
+-rw-r--r--   0        0        0    46134 2023-07-27 22:51:54.369144 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/range.data.json
+-rw-r--r--   0        0        0     2214 2023-07-27 22:51:54.369325 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/range.meta.json
+-rw-r--r--   0        0        0    23392 2023-07-27 22:51:54.372901 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/repeat.data.json
+-rw-r--r--   0        0        0     2111 2023-07-27 22:51:54.373093 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/repeat.meta.json
+-rw-r--r--   0        0        0    14372 2023-07-27 22:51:54.367972 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/whenthen.data.json
+-rw-r--r--   0        0        0     1974 2023-07-27 22:51:54.368134 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/functions/whenthen.meta.json
+-rw-r--r--   0        0        0     3929 2023-07-27 22:51:54.403457 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/__init__.data.json
+-rw-r--r--   0        0        0     1900 2023-07-27 22:51:54.403656 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/__init__.meta.json
+-rw-r--r--   0        0        0    12787 2023-07-27 22:51:54.349404 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/_utils.data.json
+-rw-r--r--   0        0        0     1821 2023-07-27 22:51:54.349610 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/_utils.meta.json
+-rw-r--r--   0        0        0     2916 2023-07-27 22:51:54.342204 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/avro.data.json
+-rw-r--r--   0        0        0     1801 2023-07-27 22:51:54.342400 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/avro.meta.json
+-rw-r--r--   0        0        0     2252 2023-07-27 22:51:54.384899 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/csv/__init__.data.json
+-rw-r--r--   0        0        0     1705 2023-07-27 22:51:54.385060 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/csv/__init__.meta.json
+-rw-r--r--   0        0        0     3259 2023-07-27 22:51:54.331597 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/csv/_utils.data.json
+-rw-r--r--   0        0        0     1765 2023-07-27 22:51:54.331891 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/csv/_utils.meta.json
+-rw-r--r--   0        0        0     9045 2023-07-27 22:51:54.344186 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/csv/batched_reader.data.json
+-rw-r--r--   0        0        0     2151 2023-07-27 22:51:54.344392 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/csv/batched_reader.meta.json
+-rw-r--r--   0        0        0    13573 2023-07-27 22:51:54.361171 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/csv/functions.data.json
+-rw-r--r--   0        0        0     2111 2023-07-27 22:51:54.361342 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/csv/functions.meta.json
+-rw-r--r--   0        0        0     6520 2023-07-27 22:51:54.403007 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/database.data.json
+-rw-r--r--   0        0        0     1827 2023-07-27 22:51:54.403210 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/database.meta.json
+-rw-r--r--   0        0        0     8141 2023-07-27 22:51:54.402499 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/delta.data.json
+-rw-r--r--   0        0        0     1923 2023-07-27 22:51:54.402701 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/delta.meta.json
+-rw-r--r--   0        0        0     2058 2023-07-27 22:51:54.392376 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/excel/__init__.data.json
+-rw-r--r--   0        0        0     1710 2023-07-27 22:51:54.392539 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/excel/__init__.meta.json
+-rw-r--r--   0        0        0    34730 2023-07-27 22:51:54.341317 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/excel/_write_utils.data.json
+-rw-r--r--   0        0        0     2087 2023-07-27 22:51:54.341529 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/excel/_write_utils.meta.json
+-rw-r--r--   0        0        0    17852 2023-07-27 22:51:54.373605 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/excel/functions.data.json
+-rw-r--r--   0        0        0     1856 2023-07-27 22:51:54.373774 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/excel/functions.meta.json
+-rw-r--r--   0        0        0     2250 2023-07-27 22:51:54.384525 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/ipc/__init__.data.json
+-rw-r--r--   0        0        0     1705 2023-07-27 22:51:54.384698 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/ipc/__init__.meta.json
+-rw-r--r--   0        0        0     4215 2023-07-27 22:51:54.360118 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/ipc/anonymous_scan.data.json
+-rw-r--r--   0        0        0     1945 2023-07-27 22:51:54.360290 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/ipc/anonymous_scan.meta.json
+-rw-r--r--   0        0        0     6753 2023-07-27 22:51:54.360573 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/ipc/functions.data.json
+-rw-r--r--   0        0        0     2017 2023-07-27 22:51:54.360745 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/ipc/functions.meta.json
+-rw-r--r--   0        0        0     2972 2023-07-27 22:51:54.341773 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/json.data.json
+-rw-r--r--   0        0        0     1918 2023-07-27 22:51:54.341972 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/json.meta.json
+-rw-r--r--   0        0        0     4614 2023-07-27 22:51:54.349881 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/ndjson.data.json
+-rw-r--r--   0        0        0     2036 2023-07-27 22:51:54.350085 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/ndjson.meta.json
+-rw-r--r--   0        0        0     2322 2023-07-27 22:51:54.401947 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/parquet/__init__.data.json
+-rw-r--r--   0        0        0     1717 2023-07-27 22:51:54.402143 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/parquet/__init__.meta.json
+-rw-r--r--   0        0        0     4283 2023-07-27 22:51:54.359695 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/parquet/anonymous_scan.data.json
+-rw-r--r--   0        0        0     1957 2023-07-27 22:51:54.359866 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/parquet/anonymous_scan.meta.json
+-rw-r--r--   0        0        0     7704 2023-07-27 22:51:54.401521 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/parquet/functions.data.json
+-rw-r--r--   0        0        0     2047 2023-07-27 22:51:54.401734 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/parquet/functions.meta.json
+-rw-r--r--   0        0        0     2289 2023-07-27 22:51:54.367360 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/pyarrow_dataset/__init__.data.json
+-rw-r--r--   0        0        0     1741 2023-07-27 22:51:54.367546 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/pyarrow_dataset/__init__.meta.json
+-rw-r--r--   0        0        0     4103 2023-07-27 22:51:54.339650 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/pyarrow_dataset/anonymous_scan.data.json
+-rw-r--r--   0        0        0     1908 2023-07-27 22:51:54.339826 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/pyarrow_dataset/anonymous_scan.meta.json
+-rw-r--r--   0        0        0     3767 2023-07-27 22:51:54.345262 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/pyarrow_dataset/functions.data.json
+-rw-r--r--   0        0        0     1898 2023-07-27 22:51:54.345469 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/io/pyarrow_dataset/functions.meta.json
+-rw-r--r--   0        0        0     2062 2023-07-27 22:51:54.399616 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/lazyframe/__init__.data.json
+-rw-r--r--   0        0        0     1709 2023-07-27 22:51:54.399820 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/lazyframe/__init__.meta.json
+-rw-r--r--   0        0        0   160119 2023-07-27 22:51:54.384081 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/lazyframe/frame.data.json
+-rw-r--r--   0        0        0     2769 2023-07-27 22:51:54.384325 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/lazyframe/frame.meta.json
+-rw-r--r--   0        0        0    15823 2023-07-27 22:51:54.359253 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/lazyframe/groupby.data.json
+-rw-r--r--   0        0        0     2123 2023-07-27 22:51:54.359429 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/lazyframe/groupby.meta.json
+-rw-r--r--   0        0        0    40543 2023-07-27 22:51:54.408956 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/selectors.data.json
+-rw-r--r--   0        0        0     2020 2023-07-27 22:51:54.409163 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/selectors.meta.json
+-rw-r--r--   0        0        0     2027 2023-07-27 22:51:54.399211 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/__init__.data.json
+-rw-r--r--   0        0        0     1701 2023-07-27 22:51:54.399399 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/__init__.meta.json
+-rw-r--r--   0        0        0     5857 2023-07-27 22:51:54.332231 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/_numpy.data.json
+-rw-r--r--   0        0        0     1820 2023-07-27 22:51:54.332414 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/_numpy.meta.json
+-rw-r--r--   0        0        0     6655 2023-07-27 22:51:54.358623 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/array.data.json
+-rw-r--r--   0        0        0     1783 2023-07-27 22:51:54.358787 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/array.meta.json
+-rw-r--r--   0        0        0     7876 2023-07-27 22:51:54.358183 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/binary.data.json
+-rw-r--r--   0        0        0     1813 2023-07-27 22:51:54.358357 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/binary.meta.json
+-rw-r--r--   0        0        0     5728 2023-07-27 22:51:54.357734 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/categorical.data.json
+-rw-r--r--   0        0        0     1823 2023-07-27 22:51:54.357896 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/categorical.meta.json
+-rw-r--r--   0        0        0    38564 2023-07-27 22:51:54.357291 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/datetime.data.json
+-rw-r--r--   0        0        0     2005 2023-07-27 22:51:54.357472 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/datetime.meta.json
+-rw-r--r--   0        0        0    30305 2023-07-27 22:51:54.356293 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/list.data.json
+-rw-r--r--   0        0        0     1970 2023-07-27 22:51:54.356469 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/list.meta.json
+-rw-r--r--   0        0        0   312466 2023-07-27 22:51:54.380798 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/series.data.json
+-rw-r--r--   0        0        0     2898 2023-07-27 22:51:54.381046 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/series.meta.json
+-rw-r--r--   0        0        0    33023 2023-07-27 22:51:54.355361 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/string.data.json
+-rw-r--r--   0        0        0     2041 2023-07-27 22:51:54.355574 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/string.meta.json
+-rw-r--r--   0        0        0    11229 2023-07-27 22:51:54.354379 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/struct.data.json
+-rw-r--r--   0        0        0     1918 2023-07-27 22:51:54.354583 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/struct.meta.json
+-rw-r--r--   0        0        0    12290 2023-07-27 22:51:54.344823 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/utils.data.json
+-rw-r--r--   0        0        0     1960 2023-07-27 22:51:54.345024 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/series/utils.meta.json
+-rw-r--r--   0        0        0    12986 2023-07-27 22:51:54.340247 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/slice.data.json
+-rw-r--r--   0        0        0     1901 2023-07-27 22:51:54.340452 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/slice.meta.json
+-rw-r--r--   0        0        0     2006 2023-07-27 22:51:54.406212 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/sql/__init__.data.json
+-rw-r--r--   0        0        0     1693 2023-07-27 22:51:54.406407 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/sql/__init__.meta.json
+-rw-r--r--   0        0        0    42035 2023-07-27 22:51:54.405362 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/sql/context.data.json
+-rw-r--r--   0        0        0     2204 2023-07-27 22:51:54.405571 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/sql/context.meta.json
+-rw-r--r--   0        0        0     7280 2023-07-27 22:51:54.351944 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/string_cache.data.json
+-rw-r--r--   0        0        0     1774 2023-07-27 22:51:54.352139 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/string_cache.meta.json
+-rw-r--r--   0        0        0    33570 2023-07-27 22:51:54.335020 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/type_aliases.data.json
+-rw-r--r--   0        0        0     1901 2023-07-27 22:51:54.335204 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/type_aliases.meta.json
+-rw-r--r--   0        0        0     4100 2023-07-27 22:51:54.392018 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/__init__.data.json
+-rw-r--r--   0        0        0     1843 2023-07-27 22:51:54.392188 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/__init__.meta.json
+-rw-r--r--   0        0        0    67688 2023-07-27 22:51:54.366963 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/_construction.data.json
+-rw-r--r--   0        0        0     2262 2023-07-27 22:51:54.367153 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/_construction.meta.json
+-rw-r--r--   0        0        0     8976 2023-07-27 22:51:54.351434 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/_parse_expr_input.data.json
+-rw-r--r--   0        0        0     2036 2023-07-27 22:51:54.351634 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/_parse_expr_input.meta.json
+-rw-r--r--   0        0        0     2677 2023-07-27 22:51:54.334071 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/_scan.data.json
+-rw-r--r--   0        0        0     1760 2023-07-27 22:51:54.334235 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/_scan.meta.json
+-rw-r--r--   0        0        0     5994 2023-07-27 22:51:54.343625 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/_wrap.data.json
+-rw-r--r--   0        0        0     1950 2023-07-27 22:51:54.343822 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/_wrap.meta.json
+-rw-r--r--   0        0        0     2704 2023-07-27 22:51:52.417427 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/build_info.data.json
+-rw-r--r--   0        0        0     1650 2023-07-27 22:51:52.417606 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/build_info.meta.json
+-rw-r--r--   0        0        0    22153 2023-07-27 22:51:54.333689 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/convert.data.json
+-rw-r--r--   0        0        0     1878 2023-07-27 22:51:54.333871 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/convert.meta.json
+-rw-r--r--   0        0        0    19053 2023-07-27 22:51:54.348771 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/decorators.data.json
+-rw-r--r--   0        0        0     1762 2023-07-27 22:51:54.348975 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/decorators.meta.json
+-rw-r--r--   0        0        0     4356 2023-07-27 22:51:54.350894 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/meta.data.json
+-rw-r--r--   0        0        0     1813 2023-07-27 22:51:54.351089 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/meta.meta.json
+-rw-r--r--   0        0        0     2921 2023-07-27 22:51:52.131513 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/polars_version.data.json
+-rw-r--r--   0        0        0     1641 2023-07-27 22:51:52.131691 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/polars_version.meta.json
+-rw-r--r--   0        0        0     3719 2023-07-27 22:51:54.372113 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/show_versions.data.json
+-rw-r--r--   0        0        0     1768 2023-07-27 22:51:54.372290 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/show_versions.meta.json
+-rw-r--r--   0        0        0    31640 2023-07-27 22:51:54.407872 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/udfs.data.json
+-rw-r--r--   0        0        0     1804 2023-07-27 22:51:54.408077 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/udfs.meta.json
+-rw-r--r--   0        0        0    27562 2023-07-27 22:51:54.343124 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/various.data.json
+-rw-r--r--   0        0        0     2033 2023-07-27 22:51:54.343335 alacorder-81.1.4/alacorder/.mypy_cache/3.10/polars/utils/various.meta.json
+-rw-r--r--   0        0        0    88451 2023-07-27 22:51:50.800538 alacorder-81.1.4/alacorder/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1635 2023-07-27 22:51:50.800709 alacorder-81.1.4/alacorder/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0    12007 2023-07-27 22:51:51.054035 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pprint.data.json
+-rw-r--r--   0        0        0     1554 2023-07-27 22:51:51.054244 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pprint.meta.json
+-rw-r--r--   0        0        0    20165 2023-07-27 22:51:50.906732 alacorder-81.1.4/alacorder/.mypy_cache/3.10/profile.data.json
+-rw-r--r--   0        0        0     1600 2023-07-27 22:51:50.906951 alacorder-81.1.4/alacorder/.mypy_cache/3.10/profile.meta.json
+-rw-r--r--   0        0        0     3591 2023-07-27 22:51:55.222067 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/__init__.data.json
+-rw-r--r--   0        0        0     1894 2023-07-27 22:51:55.222274 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/__init__.meta.json
+-rw-r--r--   0        0        0     3557 2023-07-27 22:51:55.156828 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/application/__init__.data.json
+-rw-r--r--   0        0        0     1894 2023-07-27 22:51:55.157030 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/application/__init__.meta.json
+-rw-r--r--   0        0        0   108451 2023-07-27 22:51:55.155321 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/application/application.data.json
+-rw-r--r--   0        0        0     3625 2023-07-27 22:51:55.155519 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/application/application.meta.json
+-rw-r--r--   0        0        0    16606 2023-07-27 22:51:55.099937 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/application/current.data.json
+-rw-r--r--   0        0        0     2009 2023-07-27 22:51:55.100111 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/application/current.meta.json
+-rw-r--r--   0        0        0     9063 2023-07-27 22:51:55.155877 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/application/dummy.data.json
+-rw-r--r--   0        0        0     1899 2023-07-27 22:51:55.156092 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/application/dummy.meta.json
+-rw-r--r--   0        0        0     6851 2023-07-27 22:51:55.100385 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/application/run_in_terminal.data.json
+-rw-r--r--   0        0        0     2092 2023-07-27 22:51:55.100559 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/application/run_in_terminal.meta.json
+-rw-r--r--   0        0        0    24216 2023-07-27 22:51:55.110126 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/auto_suggest.data.json
+-rw-r--r--   0        0        0     1907 2023-07-27 22:51:55.110297 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/auto_suggest.meta.json
+-rw-r--r--   0        0        0   109590 2023-07-27 22:51:55.123898 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/buffer.data.json
+-rw-r--r--   0        0        0     2609 2023-07-27 22:51:55.124089 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/buffer.meta.json
+-rw-r--r--   0        0        0    23616 2023-07-27 22:51:51.676563 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/cache.data.json
+-rw-r--r--   0        0        0     1583 2023-07-27 22:51:51.676850 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/cache.meta.json
+-rw-r--r--   0        0        0     2759 2023-07-27 22:51:52.948651 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/__init__.data.json
+-rw-r--r--   0        0        0     1686 2023-07-27 22:51:52.948851 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/__init__.meta.json
+-rw-r--r--   0        0        0    19002 2023-07-27 22:51:51.925304 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/base.data.json
+-rw-r--r--   0        0        0     1609 2023-07-27 22:51:51.925494 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/base.meta.json
+-rw-r--r--   0        0        0     6990 2023-07-27 22:51:52.163843 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/in_memory.data.json
+-rw-r--r--   0        0        0     1674 2023-07-27 22:51:52.164066 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/in_memory.meta.json
+-rw-r--r--   0        0        0     4201 2023-07-27 22:51:55.121628 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/__init__.data.json
+-rw-r--r--   0        0        0     1979 2023-07-27 22:51:55.121790 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/__init__.meta.json
+-rw-r--r--   0        0        0    43769 2023-07-27 22:51:55.118424 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/base.data.json
+-rw-r--r--   0        0        0     2059 2023-07-27 22:51:55.118605 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/base.meta.json
+-rw-r--r--   0        0        0     5620 2023-07-27 22:51:55.118852 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/deduplicate.data.json
+-rw-r--r--   0        0        0     1798 2023-07-27 22:51:55.119021 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/deduplicate.meta.json
+-rw-r--r--   0        0        0     9975 2023-07-27 22:51:55.121238 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/filesystem.data.json
+-rw-r--r--   0        0        0     1883 2023-07-27 22:51:55.121415 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/filesystem.meta.json
+-rw-r--r--   0        0        0    32629 2023-07-27 22:51:55.120724 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/fuzzy_completer.data.json
+-rw-r--r--   0        0        0     2112 2023-07-27 22:51:55.120906 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/fuzzy_completer.meta.json
+-rw-r--r--   0        0        0     9637 2023-07-27 22:51:55.119851 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/nested.data.json
+-rw-r--r--   0        0        0     1869 2023-07-27 22:51:55.120012 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/nested.meta.json
+-rw-r--r--   0        0        0    10014 2023-07-27 22:51:55.119349 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/word_completer.data.json
+-rw-r--r--   0        0        0     1969 2023-07-27 22:51:55.119530 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/word_completer.meta.json
+-rw-r--r--   0        0        0    18940 2023-07-27 22:51:55.096402 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/cursor_shapes.data.json
+-rw-r--r--   0        0        0     1873 2023-07-27 22:51:55.096580 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/cursor_shapes.meta.json
+-rw-r--r--   0        0        0    31144 2023-07-27 22:51:51.634570 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/data_structures.data.json
+-rw-r--r--   0        0        0     1568 2023-07-27 22:51:51.634762 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/data_structures.meta.json
+-rw-r--r--   0        0        0    83671 2023-07-27 22:51:55.107102 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/document.data.json
+-rw-r--r--   0        0        0     1916 2023-07-27 22:51:55.107283 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/document.meta.json
+-rw-r--r--   0        0        0     3702 2023-07-27 22:51:51.695764 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/enums.data.json
+-rw-r--r--   0        0        0     1560 2023-07-27 22:51:51.695961 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/enums.meta.json
+-rw-r--r--   0        0        0     3423 2023-07-27 22:51:54.725049 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/__init__.data.json
+-rw-r--r--   0        0        0     1840 2023-07-27 22:51:54.725261 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/__init__.meta.json
+-rw-r--r--   0        0        0    11172 2023-07-27 22:51:54.017551 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/async_generator.data.json
+-rw-r--r--   0        0        0     1863 2023-07-27 22:51:54.017786 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/async_generator.meta.json
+-rw-r--r--   0        0        0    18200 2023-07-27 22:51:53.965323 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/inputhook.data.json
+-rw-r--r--   0        0        0     1859 2023-07-27 22:51:53.965528 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/inputhook.meta.json
+-rw-r--r--   0        0        0     7762 2023-07-27 22:51:53.962609 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/utils.data.json
+-rw-r--r--   0        0        0     1796 2023-07-27 22:51:53.962795 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/utils.meta.json
+-rw-r--r--   0        0        0    10046 2023-07-27 22:51:55.102326 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/__init__.data.json
+-rw-r--r--   0        0        0     1851 2023-07-27 22:51:55.102503 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/__init__.meta.json
+-rw-r--r--   0        0        0    29547 2023-07-27 22:51:55.101200 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/app.data.json
+-rw-r--r--   0        0        0     2026 2023-07-27 22:51:55.101381 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/app.meta.json
+-rw-r--r--   0        0        0    31877 2023-07-27 22:51:51.669826 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/base.data.json
+-rw-r--r--   0        0        0     1562 2023-07-27 22:51:51.670072 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/base.meta.json
+-rw-r--r--   0        0        0    19629 2023-07-27 22:51:55.101846 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/cli.data.json
+-rw-r--r--   0        0        0     1954 2023-07-27 22:51:55.102020 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/cli.meta.json
+-rw-r--r--   0        0        0     4761 2023-07-27 22:51:51.965194 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/utils.data.json
+-rw-r--r--   0        0        0     1598 2023-07-27 22:51:51.965383 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/utils.meta.json
+-rw-r--r--   0        0        0     4079 2023-07-27 22:51:55.117331 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/__init__.data.json
+-rw-r--r--   0        0        0     1941 2023-07-27 22:51:55.117499 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/__init__.meta.json
+-rw-r--r--   0        0        0    16522 2023-07-27 22:51:55.116934 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/ansi.data.json
+-rw-r--r--   0        0        0     1926 2023-07-27 22:51:55.117112 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/ansi.meta.json
+-rw-r--r--   0        0        0    14880 2023-07-27 22:51:55.095093 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/base.data.json
+-rw-r--r--   0        0        0     1832 2023-07-27 22:51:55.095284 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/base.meta.json
+-rw-r--r--   0        0        0     9923 2023-07-27 22:51:55.097365 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/html.data.json
+-rw-r--r--   0        0        0     1954 2023-07-27 22:51:55.097540 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/html.meta.json
+-rw-r--r--   0        0        0     6363 2023-07-27 22:51:55.096850 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/pygments.data.json
+-rw-r--r--   0        0        0     1867 2023-07-27 22:51:55.097035 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/pygments.meta.json
+-rw-r--r--   0        0        0     6724 2023-07-27 22:51:55.098797 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/utils.data.json
+-rw-r--r--   0        0        0     1832 2023-07-27 22:51:55.098973 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/utils.meta.json
+-rw-r--r--   0        0        0    26319 2023-07-27 22:51:53.982754 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/history.data.json
+-rw-r--r--   0        0        0     1799 2023-07-27 22:51:53.983023 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/history.meta.json
+-rw-r--r--   0        0        0     2674 2023-07-27 22:51:55.128406 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/__init__.data.json
+-rw-r--r--   0        0        0     1774 2023-07-27 22:51:55.128599 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/__init__.meta.json
+-rw-r--r--   0        0        0     4005 2023-07-27 22:51:51.913479 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/ansi_escape_sequences.data.json
+-rw-r--r--   0        0        0     1660 2023-07-27 22:51:51.913765 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/ansi_escape_sequences.meta.json
+-rw-r--r--   0        0        0    29599 2023-07-27 22:51:55.113832 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/base.data.json
+-rw-r--r--   0        0        0     1805 2023-07-27 22:51:55.114026 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/base.meta.json
+-rw-r--r--   0        0        0     4257 2023-07-27 22:51:55.114254 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/defaults.data.json
+-rw-r--r--   0        0        0     1775 2023-07-27 22:51:55.114430 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/defaults.meta.json
+-rw-r--r--   0        0        0     5111 2023-07-27 22:51:55.126904 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/typeahead.data.json
+-rw-r--r--   0        0        0     1870 2023-07-27 22:51:55.127073 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/typeahead.meta.json
+-rw-r--r--   0        0        0    16680 2023-07-27 22:51:55.124542 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/vt100_parser.data.json
+-rw-r--r--   0        0        0     1935 2023-07-27 22:51:55.124715 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/input/vt100_parser.meta.json
+-rw-r--r--   0        0        0     3098 2023-07-27 22:51:55.112116 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/__init__.data.json
+-rw-r--r--   0        0        0     1812 2023-07-27 22:51:55.112285 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/__init__.meta.json
+-rw-r--r--   0        0        0     1701 2023-07-27 22:51:50.969634 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/__init__.data.json
+-rw-r--r--   0        0        0     1569 2023-07-27 22:51:50.969842 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/__init__.meta.json
+-rw-r--r--   0        0        0     3850 2023-07-27 22:51:55.131178 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/auto_suggest.data.json
+-rw-r--r--   0        0        0     1935 2023-07-27 22:51:55.131362 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/auto_suggest.meta.json
+-rw-r--r--   0        0        0     5321 2023-07-27 22:51:55.141458 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/basic.data.json
+-rw-r--r--   0        0        0     2006 2023-07-27 22:51:55.141671 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/basic.meta.json
+-rw-r--r--   0        0        0     7615 2023-07-27 22:51:55.131660 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/completion.data.json
+-rw-r--r--   0        0        0     2297 2023-07-27 22:51:55.131866 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/completion.meta.json
+-rw-r--r--   0        0        0     3357 2023-07-27 22:51:55.125996 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/cpr.data.json
+-rw-r--r--   0        0        0     1870 2023-07-27 22:51:55.126182 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/cpr.meta.json
+-rw-r--r--   0        0        0     7770 2023-07-27 22:51:55.140997 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/emacs.data.json
+-rw-r--r--   0        0        0     2098 2023-07-27 22:51:55.141199 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/emacs.meta.json
+-rw-r--r--   0        0        0     3816 2023-07-27 22:51:55.130088 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/focus.data.json
+-rw-r--r--   0        0        0     1802 2023-07-27 22:51:55.130289 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/focus.meta.json
+-rw-r--r--   0        0        0    12770 2023-07-27 22:51:55.125568 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/mouse.data.json
+-rw-r--r--   0        0        0     1959 2023-07-27 22:51:55.125767 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/mouse.meta.json
+-rw-r--r--   0        0        0    74910 2023-07-27 22:51:55.139551 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/named_commands.data.json
+-rw-r--r--   0        0        0     2173 2023-07-27 22:51:55.139768 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/named_commands.meta.json
+-rw-r--r--   0        0        0     5283 2023-07-27 22:51:55.141928 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/open_in_editor.data.json
+-rw-r--r--   0        0        0     1890 2023-07-27 22:51:55.142131 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/open_in_editor.meta.json
+-rw-r--r--   0        0        0     6591 2023-07-27 22:51:55.132145 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/page_navigation.data.json
+-rw-r--r--   0        0        0     1885 2023-07-27 22:51:55.132346 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/page_navigation.meta.json
+-rw-r--r--   0        0        0     8159 2023-07-27 22:51:55.125017 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/scroll.data.json
+-rw-r--r--   0        0        0     1806 2023-07-27 22:51:55.125185 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/scroll.meta.json
+-rw-r--r--   0        0        0    30649 2023-07-27 22:51:55.140473 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/vi.data.json
+-rw-r--r--   0        0        0     2408 2023-07-27 22:51:55.140685 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/vi.meta.json
+-rw-r--r--   0        0        0     4588 2023-07-27 22:51:55.145968 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/defaults.data.json
+-rw-r--r--   0        0        0     2044 2023-07-27 22:51:55.146145 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/defaults.meta.json
+-rw-r--r--   0        0        0     2688 2023-07-27 22:51:51.620818 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/digraphs.data.json
+-rw-r--r--   0        0        0     1581 2023-07-27 22:51:51.621683 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/digraphs.meta.json
+-rw-r--r--   0        0        0     8025 2023-07-27 22:51:55.126497 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/emacs_state.data.json
+-rw-r--r--   0        0        0     1779 2023-07-27 22:51:55.126656 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/emacs_state.meta.json
+-rw-r--r--   0        0        0    61537 2023-07-27 22:51:55.103712 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_bindings.data.json
+-rw-r--r--   0        0        0     1970 2023-07-27 22:51:55.103895 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_bindings.meta.json
+-rw-r--r--   0        0        0    39549 2023-07-27 22:51:55.108938 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_processor.data.json
+-rw-r--r--   0        0        0     2451 2023-07-27 22:51:55.109125 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_processor.meta.json
+-rw-r--r--   0        0        0    17210 2023-07-27 22:51:55.095754 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/vi_state.data.json
+-rw-r--r--   0        0        0     1929 2023-07-27 22:51:55.095932 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/vi_state.meta.json
+-rw-r--r--   0        0        0    65652 2023-07-27 22:51:51.643564 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/keys.data.json
+-rw-r--r--   0        0        0     1583 2023-07-27 22:51:51.643803 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/keys.meta.json
+-rw-r--r--   0        0        0     7077 2023-07-27 22:51:55.156381 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/__init__.data.json
+-rw-r--r--   0        0        0     1980 2023-07-27 22:51:55.156587 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/__init__.meta.json
+-rw-r--r--   0        0        0   175820 2023-07-27 22:51:55.145520 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/containers.data.json
+-rw-r--r--   0        0        0     2649 2023-07-27 22:51:55.145724 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/containers.meta.json
+-rw-r--r--   0        0        0    97155 2023-07-27 22:51:55.137029 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/controls.data.json
+-rw-r--r--   0        0        0     2818 2023-07-27 22:51:55.137256 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/controls.meta.json
+-rw-r--r--   0        0        0    14639 2023-07-27 22:51:51.637330 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dimension.data.json
+-rw-r--r--   0        0        0     1597 2023-07-27 22:51:51.637517 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dimension.meta.json
+-rw-r--r--   0        0        0     3767 2023-07-27 22:51:55.150943 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dummy.data.json
+-rw-r--r--   0        0        0     1997 2023-07-27 22:51:55.151113 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dummy.meta.json
+-rw-r--r--   0        0        0    33603 2023-07-27 22:51:55.148753 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/layout.data.json
+-rw-r--r--   0        0        0     2334 2023-07-27 22:51:55.148934 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/layout.meta.json
+-rw-r--r--   0        0        0    26691 2023-07-27 22:51:55.137900 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/margins.data.json
+-rw-r--r--   0        0        0     1994 2023-07-27 22:51:55.138108 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/margins.meta.json
+-rw-r--r--   0        0        0    39889 2023-07-27 22:51:55.147812 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/menus.data.json
+-rw-r--r--   0        0        0     2611 2023-07-27 22:51:55.148004 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/menus.meta.json
+-rw-r--r--   0        0        0     6556 2023-07-27 22:51:55.094424 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/mouse_handlers.data.json
+-rw-r--r--   0        0        0     1845 2023-07-27 22:51:55.094622 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/mouse_handlers.meta.json
+-rw-r--r--   0        0        0    77084 2023-07-27 22:51:55.134978 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/processors.data.json
+-rw-r--r--   0        0        0     2229 2023-07-27 22:51:55.135195 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/processors.meta.json
+-rw-r--r--   0        0        0    25505 2023-07-27 22:51:55.093793 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/screen.data.json
+-rw-r--r--   0        0        0     1881 2023-07-27 22:51:55.094110 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/screen.meta.json
+-rw-r--r--   0        0        0    23316 2023-07-27 22:51:55.153190 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/scrollable_pane.data.json
+-rw-r--r--   0        0        0     2343 2023-07-27 22:51:55.153367 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/scrollable_pane.meta.json
+-rw-r--r--   0        0        0    37076 2023-07-27 22:51:55.098344 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/utils.data.json
+-rw-r--r--   0        0        0     1812 2023-07-27 22:51:55.098527 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/utils.meta.json
+-rw-r--r--   0        0        0     2912 2023-07-27 22:51:55.133357 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/__init__.data.json
+-rw-r--r--   0        0        0     1778 2023-07-27 22:51:55.133546 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/__init__.meta.json
+-rw-r--r--   0        0        0    13556 2023-07-27 22:51:55.130735 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/base.data.json
+-rw-r--r--   0        0        0     1815 2023-07-27 22:51:55.130931 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/base.meta.json
+-rw-r--r--   0        0        0    23436 2023-07-27 22:51:55.132947 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/pygments.data.json
+-rw-r--r--   0        0        0     2130 2023-07-27 22:51:55.133135 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/pygments.meta.json
+-rw-r--r--   0        0        0    13274 2023-07-27 22:51:51.944909 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/mouse_events.data.json
+-rw-r--r--   0        0        0     1615 2023-07-27 22:51:51.945103 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/mouse_events.meta.json
+-rw-r--r--   0        0        0     2577 2023-07-27 22:51:55.115014 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/__init__.data.json
+-rw-r--r--   0        0        0     1818 2023-07-27 22:51:55.115170 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/__init__.meta.json
+-rw-r--r--   0        0        0    74663 2023-07-27 22:51:55.111717 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/base.data.json
+-rw-r--r--   0        0        0     1897 2023-07-27 22:51:55.111909 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/base.meta.json
+-rw-r--r--   0        0        0     9667 2023-07-27 22:51:55.099298 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/color_depth.data.json
+-rw-r--r--   0        0        0     1773 2023-07-27 22:51:55.099466 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/color_depth.meta.json
+-rw-r--r--   0        0        0     4080 2023-07-27 22:51:55.114653 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/defaults.data.json
+-rw-r--r--   0        0        0     1859 2023-07-27 22:51:55.114824 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/defaults.meta.json
+-rw-r--r--   0        0        0     4753 2023-07-27 22:51:51.622804 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/flush_stdout.data.json
+-rw-r--r--   0        0        0     1628 2023-07-27 22:51:51.623007 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/flush_stdout.meta.json
+-rw-r--r--   0        0        0    30328 2023-07-27 22:51:55.112973 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/plain_text.data.json
+-rw-r--r--   0        0        0     1983 2023-07-27 22:51:55.113148 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/plain_text.meta.json
+-rw-r--r--   0        0        0    53319 2023-07-27 22:51:55.116298 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/vt100.data.json
+-rw-r--r--   0        0        0     2074 2023-07-27 22:51:55.116483 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/output/vt100.meta.json
+-rw-r--r--   0        0        0    22260 2023-07-27 22:51:55.225450 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/patch_stdout.data.json
+-rw-r--r--   0        0        0     2030 2023-07-27 22:51:55.225657 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/patch_stdout.meta.json
+-rw-r--r--   0        0        0    39943 2023-07-27 22:51:55.127964 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/renderer.data.json
+-rw-r--r--   0        0        0     2628 2023-07-27 22:51:55.128180 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/renderer.meta.json
+-rw-r--r--   0        0        0    12747 2023-07-27 22:51:55.105299 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/search.data.json
+-rw-r--r--   0        0        0     2003 2023-07-27 22:51:55.105470 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/search.meta.json
+-rw-r--r--   0        0        0     9459 2023-07-27 22:51:51.639503 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/selection.data.json
+-rw-r--r--   0        0        0     1569 2023-07-27 22:51:51.639716 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/selection.meta.json
+-rw-r--r--   0        0        0     4456 2023-07-27 22:51:55.162515 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/__init__.data.json
+-rw-r--r--   0        0        0     1875 2023-07-27 22:51:55.162724 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/__init__.meta.json
+-rw-r--r--   0        0        0    21855 2023-07-27 22:51:55.159479 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/dialogs.data.json
+-rw-r--r--   0        0        0     2503 2023-07-27 22:51:55.159701 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/dialogs.meta.json
+-rw-r--r--   0        0        0     3948 2023-07-27 22:51:55.162051 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/__init__.data.json
+-rw-r--r--   0        0        0     1844 2023-07-27 22:51:55.162257 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/__init__.meta.json
+-rw-r--r--   0        0        0    51515 2023-07-27 22:51:55.158081 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/base.data.json
+-rw-r--r--   0        0        0     3081 2023-07-27 22:51:55.158308 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/base.meta.json
+-rw-r--r--   0        0        0    47588 2023-07-27 22:51:55.129637 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/formatters.data.json
+-rw-r--r--   0        0        0     2146 2023-07-27 22:51:55.129850 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/formatters.meta.json
+-rw-r--r--   0        0        0   100034 2023-07-27 22:51:55.161551 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/prompt.data.json
+-rw-r--r--   0        0        0     3582 2023-07-27 22:51:55.161789 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/prompt.meta.json
+-rw-r--r--   0        0        0    10368 2023-07-27 22:51:55.158683 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/utils.data.json
+-rw-r--r--   0        0        0     2326 2023-07-27 22:51:55.158903 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/utils.meta.json
+-rw-r--r--   0        0        0     5472 2023-07-27 22:51:55.109373 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/__init__.data.json
+-rw-r--r--   0        0        0     1945 2023-07-27 22:51:55.109549 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/__init__.meta.json
+-rw-r--r--   0        0        0    50758 2023-07-27 22:51:51.660977 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/base.data.json
+-rw-r--r--   0        0        0     1584 2023-07-27 22:51:51.661205 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/base.meta.json
+-rw-r--r--   0        0        0     6981 2023-07-27 22:51:52.192698 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/defaults.data.json
+-rw-r--r--   0        0        0     1749 2023-07-27 22:51:52.192907 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/defaults.meta.json
+-rw-r--r--   0        0        0     2366 2023-07-27 22:51:51.656427 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/named_colors.data.json
+-rw-r--r--   0        0        0     1577 2023-07-27 22:51:51.656654 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/named_colors.meta.json
+-rw-r--r--   0        0        0     5579 2023-07-27 22:51:52.212278 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/pygments.data.json
+-rw-r--r--   0        0        0     1727 2023-07-27 22:51:52.212473 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/pygments.meta.json
+-rw-r--r--   0        0        0    27026 2023-07-27 22:51:51.969231 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style.data.json
+-rw-r--r--   0        0        0     1755 2023-07-27 22:51:51.969445 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style.meta.json
+-rw-r--r--   0        0        0    41607 2023-07-27 22:51:55.104736 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style_transformation.data.json
+-rw-r--r--   0        0        0     2047 2023-07-27 22:51:55.104913 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style_transformation.meta.json
+-rw-r--r--   0        0        0    33441 2023-07-27 22:51:51.673779 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/utils.data.json
+-rw-r--r--   0        0        0     1681 2023-07-27 22:51:51.674003 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/utils.meta.json
+-rw-r--r--   0        0        0    27585 2023-07-27 22:51:55.107925 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/validation.data.json
+-rw-r--r--   0        0        0     1870 2023-07-27 22:51:55.108104 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/validation.meta.json
+-rw-r--r--   0        0        0     4475 2023-07-27 22:51:55.152487 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/__init__.data.json
+-rw-r--r--   0        0        0     1859 2023-07-27 22:51:55.152661 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/__init__.meta.json
+-rw-r--r--   0        0        0    85417 2023-07-27 22:51:55.150530 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/base.data.json
+-rw-r--r--   0        0        0     2926 2023-07-27 22:51:55.150721 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/base.meta.json
+-rw-r--r--   0        0        0     8064 2023-07-27 22:51:55.151402 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/dialogs.data.json
+-rw-r--r--   0        0        0     2363 2023-07-27 22:51:55.151585 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/dialogs.meta.json
+-rw-r--r--   0        0        0    19258 2023-07-27 22:51:55.152093 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/menus.data.json
+-rw-r--r--   0        0        0     2573 2023-07-27 22:51:55.152263 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/menus.meta.json
+-rw-r--r--   0        0        0    28557 2023-07-27 22:51:55.146799 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/toolbars.data.json
+-rw-r--r--   0        0        0     2844 2023-07-27 22:51:55.146997 alacorder-81.1.4/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/toolbars.meta.json
+-rw-r--r--   0        0        0    43338 2023-07-27 22:51:51.652157 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pstats.data.json
+-rw-r--r--   0        0        0     1668 2023-07-27 22:51:51.652397 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pstats.meta.json
+-rw-r--r--   0        0        0     7505 2023-07-27 22:51:51.182846 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pty.data.json
+-rw-r--r--   0        0        0     1587 2023-07-27 22:51:51.183022 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pty.meta.json
+-rw-r--r--   0        0        0     2138 2023-07-27 22:51:53.836542 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pure_eval/__init__.data.json
+-rw-r--r--   0        0        0     1641 2023-07-27 22:51:53.836722 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pure_eval/__init__.meta.json
+-rw-r--r--   0        0        0    16397 2023-07-27 22:51:53.782372 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pure_eval/core.data.json
+-rw-r--r--   0        0        0     1708 2023-07-27 22:51:53.782602 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pure_eval/core.meta.json
+-rw-r--r--   0        0        0     7413 2023-07-27 22:51:53.711358 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pure_eval/my_getattr_static.data.json
+-rw-r--r--   0        0        0     1650 2023-07-27 22:51:53.711605 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pure_eval/my_getattr_static.meta.json
+-rw-r--r--   0        0        0    13740 2023-07-27 22:51:52.512216 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pure_eval/utils.data.json
+-rw-r--r--   0        0        0     1731 2023-07-27 22:51:52.512431 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pure_eval/utils.meta.json
+-rw-r--r--   0        0        0     1534 2023-07-27 22:51:50.895708 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pure_eval/version.data.json
+-rw-r--r--   0        0        0     1525 2023-07-27 22:51:50.895884 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pure_eval/version.meta.json
+-rw-r--r--   0        0        0    23456 2023-07-27 22:51:52.386202 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/__init__.data.json
+-rw-r--r--   0        0        0     1938 2023-07-27 22:51:52.386402 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/__init__.meta.json
+-rw-r--r--   0        0        0     5109 2023-07-27 22:51:52.383151 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/annotated_types.data.json
+-rw-r--r--   0        0        0     1722 2023-07-27 22:51:52.383349 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/annotated_types.meta.json
+-rw-r--r--   0        0        0    29499 2023-07-27 22:51:52.366720 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/class_validators.data.json
+-rw-r--r--   0        0        0     1883 2023-07-27 22:51:52.366893 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/class_validators.meta.json
+-rw-r--r--   0        0        0    30801 2023-07-27 22:51:52.364912 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/color.data.json
+-rw-r--r--   0        0        0     1740 2023-07-27 22:51:52.365116 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/color.meta.json
+-rw-r--r--   0        0        0    30661 2023-07-27 22:51:52.365839 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/config.data.json
+-rw-r--r--   0        0        0     1781 2023-07-27 22:51:52.366016 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/config.meta.json
+-rw-r--r--   0        0        0    46856 2023-07-27 22:51:52.384349 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/dataclasses.data.json
+-rw-r--r--   0        0        0     1911 2023-07-27 22:51:52.384551 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/dataclasses.meta.json
+-rw-r--r--   0        0        0    10258 2023-07-27 22:51:52.367251 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/datetime_parse.data.json
+-rw-r--r--   0        0        0     1692 2023-07-27 22:51:52.367416 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/datetime_parse.meta.json
+-rw-r--r--   0        0        0    41091 2023-07-27 22:51:52.385455 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/decorator.data.json
+-rw-r--r--   0        0        0     1860 2023-07-27 22:51:52.385647 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/decorator.meta.json
+-rw-r--r--   0        0        0    38920 2023-07-27 22:51:52.382667 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/env_settings.data.json
+-rw-r--r--   0        0        0     1763 2023-07-27 22:51:52.382875 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/env_settings.meta.json
+-rw-r--r--   0        0        0    23197 2023-07-27 22:51:52.376542 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/error_wrappers.data.json
+-rw-r--r--   0        0        0     1779 2023-07-27 22:51:52.376747 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/error_wrappers.meta.json
+-rw-r--r--   0        0        0   146844 2023-07-27 22:51:52.362235 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/errors.data.json
+-rw-r--r--   0        0        0     1642 2023-07-27 22:51:52.362460 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/errors.meta.json
+-rw-r--r--   0        0        0    79459 2023-07-27 22:51:52.378376 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/fields.data.json
+-rw-r--r--   0        0        0     2040 2023-07-27 22:51:52.378589 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/fields.meta.json
+-rw-r--r--   0        0        0     9307 2023-07-27 22:51:52.374577 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/json.data.json
+-rw-r--r--   0        0        0     1825 2023-07-27 22:51:52.374761 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/json.meta.json
+-rw-r--r--   0        0        0    85357 2023-07-27 22:51:52.381557 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/main.data.json
+-rw-r--r--   0        0        0     2003 2023-07-27 22:51:52.381770 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/main.meta.json
+-rw-r--r--   0        0        0   105861 2023-07-27 22:51:52.374041 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/networks.data.json
+-rw-r--r--   0        0        0     1808 2023-07-27 22:51:52.374233 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/networks.meta.json
+-rw-r--r--   0        0        0     6098 2023-07-27 22:51:52.375037 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/parse.data.json
+-rw-r--r--   0        0        0     1665 2023-07-27 22:51:52.375239 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/parse.meta.json
+-rw-r--r--   0        0        0    46316 2023-07-27 22:51:52.379636 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/schema.data.json
+-rw-r--r--   0        0        0     1966 2023-07-27 22:51:52.379851 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/schema.meta.json
+-rw-r--r--   0        0        0    16626 2023-07-27 22:51:52.375730 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/tools.data.json
+-rw-r--r--   0        0        0     1711 2023-07-27 22:51:52.375929 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/tools.meta.json
+-rw-r--r--   0        0        0   160004 2023-07-27 22:51:52.371852 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/types.data.json
+-rw-r--r--   0        0        0     2008 2023-07-27 22:51:52.372050 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/types.meta.json
+-rw-r--r--   0        0        0    43060 2023-07-27 22:51:52.359369 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/typing.data.json
+-rw-r--r--   0        0        0     1744 2023-07-27 22:51:52.359642 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/typing.meta.json
+-rw-r--r--   0        0        0    70966 2023-07-27 22:51:52.363953 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/utils.data.json
+-rw-r--r--   0        0        0     1936 2023-07-27 22:51:52.364150 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/utils.meta.json
+-rw-r--r--   0        0        0    58764 2023-07-27 22:51:52.368606 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/validators.data.json
+-rw-r--r--   0        0        0     1976 2023-07-27 22:51:52.368794 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/validators.meta.json
+-rw-r--r--   0        0        0     3175 2023-07-27 22:51:51.079326 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/version.data.json
+-rw-r--r--   0        0        0     1538 2023-07-27 22:51:51.079523 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydantic/version.meta.json
+-rw-r--r--   0        0        0   105041 2023-07-27 22:51:52.073680 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydoc.data.json
+-rw-r--r--   0        0        0     1666 2023-07-27 22:51:52.074032 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pydoc.meta.json
+-rw-r--r--   0        0        0    35897 2023-07-27 22:51:51.680569 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pyexpat/__init__.data.json
+-rw-r--r--   0        0        0     1642 2023-07-27 22:51:51.680860 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pyexpat/__init__.meta.json
+-rw-r--r--   0        0        0    10324 2023-07-27 22:51:50.927128 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pyexpat/errors.data.json
+-rw-r--r--   0        0        0     1571 2023-07-27 22:51:50.927373 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pyexpat/errors.meta.json
+-rw-r--r--   0        0        0     3246 2023-07-27 22:51:50.925686 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pyexpat/model.data.json
+-rw-r--r--   0        0        0     1540 2023-07-27 22:51:50.925854 alacorder-81.1.4/alacorder/.mypy_cache/3.10/pyexpat/model.meta.json
+-rw-r--r--   0        0        0    34247 2023-07-27 22:51:51.664952 alacorder-81.1.4/alacorder/.mypy_cache/3.10/queue.data.json
+-rw-r--r--   0        0        0     1580 2023-07-27 22:51:51.665274 alacorder-81.1.4/alacorder/.mypy_cache/3.10/queue.meta.json
+-rw-r--r--   0        0        0    43152 2023-07-27 22:51:53.706565 alacorder-81.1.4/alacorder/.mypy_cache/3.10/random.data.json
+-rw-r--r--   0        0        0     1664 2023-07-27 22:51:53.706829 alacorder-81.1.4/alacorder/.mypy_cache/3.10/random.meta.json
+-rw-r--r--   0        0        0   181054 2023-07-27 22:51:50.798636 alacorder-81.1.4/alacorder/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1656 2023-07-27 22:51:50.798842 alacorder-81.1.4/alacorder/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    16527 2023-07-27 22:51:51.705967 alacorder-81.1.4/alacorder/.mypy_cache/3.10/reprlib.data.json
+-rw-r--r--   0        0        0     1632 2023-07-27 22:51:51.706155 alacorder-81.1.4/alacorder/.mypy_cache/3.10/reprlib.meta.json
+-rw-r--r--   0        0        0    41286 2023-07-27 22:51:50.910382 alacorder-81.1.4/alacorder/.mypy_cache/3.10/resource.data.json
+-rw-r--r--   0        0        0     1581 2023-07-27 22:51:50.910602 alacorder-81.1.4/alacorder/.mypy_cache/3.10/resource.meta.json
+-rw-r--r--   0        0        0     8279 2023-07-27 22:51:54.679773 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/__init__.data.json
+-rw-r--r--   0        0        0     1717 2023-07-27 22:51:54.679975 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/__init__.meta.json
+-rw-r--r--   0        0        0     7609 2023-07-27 22:51:54.684439 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/__main__.data.json
+-rw-r--r--   0        0        0     2045 2023-07-27 22:51:54.684615 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/__main__.meta.json
+-rw-r--r--   0        0        0     1754 2023-07-27 22:51:51.296535 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_cell_widths.data.json
+-rw-r--r--   0        0        0     1528 2023-07-27 22:51:51.296729 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_cell_widths.meta.json
+-rw-r--r--   0        0        0     1578 2023-07-27 22:51:51.373417 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_emoji_codes.data.json
+-rw-r--r--   0        0        0     1529 2023-07-27 22:51:51.373680 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_emoji_codes.meta.json
+-rw-r--r--   0        0        0     4072 2023-07-27 22:51:51.837458 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_emoji_replace.data.json
+-rw-r--r--   0        0        0     1564 2023-07-27 22:51:51.837635 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_emoji_replace.meta.json
+-rw-r--r--   0        0        0     2309 2023-07-27 22:51:51.473013 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_export_format.data.json
+-rw-r--r--   0        0        0     1531 2023-07-27 22:51:51.473188 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_export_format.meta.json
+-rw-r--r--   0        0        0     2079 2023-07-27 22:51:51.417672 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_extension.data.json
+-rw-r--r--   0        0        0     1521 2023-07-27 22:51:51.417902 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_extension.meta.json
+-rw-r--r--   0        0        0     2245 2023-07-27 22:51:51.836313 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_fileno.data.json
+-rw-r--r--   0        0        0     1532 2023-07-27 22:51:51.836557 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_fileno.meta.json
+-rw-r--r--   0        0        0     8184 2023-07-27 22:51:54.701717 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_log_render.data.json
+-rw-r--r--   0        0        0     1836 2023-07-27 22:51:54.701932 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_log_render.meta.json
+-rw-r--r--   0        0        0     6621 2023-07-27 22:51:51.407943 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_loop.data.json
+-rw-r--r--   0        0        0     1512 2023-07-27 22:51:51.408176 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_loop.meta.json
+-rw-r--r--   0        0        0    15349 2023-07-27 22:51:51.476825 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_null_file.data.json
+-rw-r--r--   0        0        0     1534 2023-07-27 22:51:51.477014 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_null_file.meta.json
+-rw-r--r--   0        0        0     2074 2023-07-27 22:51:54.684802 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_palettes.data.json
+-rw-r--r--   0        0        0     1688 2023-07-27 22:51:54.684971 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_palettes.meta.json
+-rw-r--r--   0        0        0     1988 2023-07-27 22:51:51.407068 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_pick.data.json
+-rw-r--r--   0        0        0     1511 2023-07-27 22:51:51.407260 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_pick.meta.json
+-rw-r--r--   0        0        0    10129 2023-07-27 22:51:53.698021 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_ratio.data.json
+-rw-r--r--   0        0        0     1632 2023-07-27 22:51:53.698271 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_ratio.meta.json
+-rw-r--r--   0        0        0     1639 2023-07-27 22:51:51.415168 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_spinners.data.json
+-rw-r--r--   0        0        0     1522 2023-07-27 22:51:51.415386 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_spinners.meta.json
+-rw-r--r--   0        0        0     6390 2023-07-27 22:51:51.092288 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_stack.data.json
+-rw-r--r--   0        0        0     1513 2023-07-27 22:51:51.092464 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_stack.meta.json
+-rw-r--r--   0        0        0     2777 2023-07-27 22:51:51.821220 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_timer.data.json
+-rw-r--r--   0        0        0     1542 2023-07-27 22:51:51.821400 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_timer.meta.json
+-rw-r--r--   0        0        0    54946 2023-07-27 22:51:54.718524 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_win32_console.data.json
+-rw-r--r--   0        0        0     1801 2023-07-27 22:51:54.718727 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_win32_console.meta.json
+-rw-r--r--   0        0        0     6780 2023-07-27 22:51:54.724228 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_windows.data.json
+-rw-r--r--   0        0        0     1755 2023-07-27 22:51:54.724422 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_windows.meta.json
+-rw-r--r--   0        0        0     3006 2023-07-27 22:51:54.721454 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_windows_renderer.data.json
+-rw-r--r--   0        0        0     1759 2023-07-27 22:51:54.721672 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_windows_renderer.meta.json
+-rw-r--r--   0        0        0     3953 2023-07-27 22:51:54.686033 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_wrap.data.json
+-rw-r--r--   0        0        0     1820 2023-07-27 22:51:54.686196 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/_wrap.meta.json
+-rw-r--r--   0        0        0     4453 2023-07-27 22:51:54.683964 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/abc.data.json
+-rw-r--r--   0        0        0     1727 2023-07-27 22:51:54.684129 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/abc.meta.json
+-rw-r--r--   0        0        0    22676 2023-07-27 22:51:54.701165 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/align.data.json
+-rw-r--r--   0        0        0     1937 2023-07-27 22:51:54.701371 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/align.meta.json
+-rw-r--r--   0        0        0    25645 2023-07-27 22:51:54.716658 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/ansi.data.json
+-rw-r--r--   0        0        0     1934 2023-07-27 22:51:54.716828 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/ansi.meta.json
+-rw-r--r--   0        0        0    20151 2023-07-27 22:51:54.687311 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/box.data.json
+-rw-r--r--   0        0        0     1887 2023-07-27 22:51:54.687484 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/box.meta.json
+-rw-r--r--   0        0        0     8431 2023-07-27 22:51:51.835483 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/cells.data.json
+-rw-r--r--   0        0        0     1604 2023-07-27 22:51:51.835690 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/cells.meta.json
+-rw-r--r--   0        0        0    55007 2023-07-27 22:51:54.700309 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/color.data.json
+-rw-r--r--   0        0        0     2025 2023-07-27 22:51:54.700516 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/color.meta.json
+-rw-r--r--   0        0        0    21553 2023-07-27 22:51:51.416955 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/color_triplet.data.json
+-rw-r--r--   0        0        0     1528 2023-07-27 22:51:51.417229 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/color_triplet.meta.json
+-rw-r--r--   0        0        0    10143 2023-07-27 22:51:54.688614 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/columns.data.json
+-rw-r--r--   0        0        0     2049 2023-07-27 22:51:54.688787 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/columns.meta.json
+-rw-r--r--   0        0        0   173517 2023-07-27 22:51:54.715381 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/console.data.json
+-rw-r--r--   0        0        0     2702 2023-07-27 22:51:54.715598 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/console.meta.json
+-rw-r--r--   0        0        0     5731 2023-07-27 22:51:54.685238 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/constrain.data.json
+-rw-r--r--   0        0        0     1776 2023-07-27 22:51:54.685402 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/constrain.meta.json
+-rw-r--r--   0        0        0    19516 2023-07-27 22:51:54.681393 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/containers.data.json
+-rw-r--r--   0        0        0     1833 2023-07-27 22:51:54.681568 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/containers.meta.json
+-rw-r--r--   0        0        0    21755 2023-07-27 22:51:54.698899 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/control.data.json
+-rw-r--r--   0        0        0     1859 2023-07-27 22:51:54.699108 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/control.meta.json
+-rw-r--r--   0        0        0     3592 2023-07-27 22:51:54.685624 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/default_styles.data.json
+-rw-r--r--   0        0        0     2002 2023-07-27 22:51:54.685794 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/default_styles.meta.json
+-rw-r--r--   0        0        0    10485 2023-07-27 22:51:54.698099 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/emoji.data.json
+-rw-r--r--   0        0        0     1936 2023-07-27 22:51:54.698306 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/emoji.meta.json
+-rw-r--r--   0        0        0     8024 2023-07-27 22:51:51.474204 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/errors.data.json
+-rw-r--r--   0        0        0     1514 2023-07-27 22:51:51.474388 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/errors.meta.json
+-rw-r--r--   0        0        0     8405 2023-07-27 22:51:54.720994 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/file_proxy.data.json
+-rw-r--r--   0        0        0     1732 2023-07-27 22:51:54.721202 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/file_proxy.meta.json
+-rw-r--r--   0        0        0     4786 2023-07-27 22:51:51.519831 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/filesize.data.json
+-rw-r--r--   0        0        0     1519 2023-07-27 22:51:51.520030 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/filesize.meta.json
+-rw-r--r--   0        0        0    14454 2023-07-27 22:51:54.711723 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/highlighter.data.json
+-rw-r--r--   0        0        0     1802 2023-07-27 22:51:54.711892 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/highlighter.meta.json
+-rw-r--r--   0        0        0     9625 2023-07-27 22:51:54.720420 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/json.data.json
+-rw-r--r--   0        0        0     1905 2023-07-27 22:51:54.720626 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/json.meta.json
+-rw-r--r--   0        0        0     9674 2023-07-27 22:51:54.711117 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/jupyter.data.json
+-rw-r--r--   0        0        0     1770 2023-07-27 22:51:54.711290 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/jupyter.meta.json
+-rw-r--r--   0        0        0    27500 2023-07-27 22:51:54.722400 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/live.data.json
+-rw-r--r--   0        0        0     2293 2023-07-27 22:51:54.722638 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/live.meta.json
+-rw-r--r--   0        0        0     8926 2023-07-27 22:51:54.717163 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/live_render.data.json
+-rw-r--r--   0        0        0     1834 2023-07-27 22:51:54.717352 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/live_render.meta.json
+-rw-r--r--   0        0        0    65179 2023-07-27 22:51:54.682990 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/markdown.data.json
+-rw-r--r--   0        0        0     2149 2023-07-27 22:51:54.683198 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/markdown.meta.json
+-rw-r--r--   0        0        0    26190 2023-07-27 22:51:54.697493 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/markup.data.json
+-rw-r--r--   0        0        0     1882 2023-07-27 22:51:54.697703 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/markup.meta.json
+-rw-r--r--   0        0        0    24314 2023-07-27 22:51:54.680640 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/measure.data.json
+-rw-r--r--   0        0        0     1750 2023-07-27 22:51:54.680844 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/measure.meta.json
+-rw-r--r--   0        0        0    12251 2023-07-27 22:51:54.686592 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/padding.data.json
+-rw-r--r--   0        0        0     1787 2023-07-27 22:51:54.686761 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/padding.meta.json
+-rw-r--r--   0        0        0     5855 2023-07-27 22:51:54.696563 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/pager.data.json
+-rw-r--r--   0        0        0     1806 2023-07-27 22:51:54.696781 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/pager.meta.json
+-rw-r--r--   0        0        0     8799 2023-07-27 22:51:54.683546 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/palette.data.json
+-rw-r--r--   0        0        0     1894 2023-07-27 22:51:54.683721 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/palette.meta.json
+-rw-r--r--   0        0        0    16891 2023-07-27 22:51:54.705150 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/panel.data.json
+-rw-r--r--   0        0        0     1912 2023-07-27 22:51:54.705406 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/panel.meta.json
+-rw-r--r--   0        0        0   124507 2023-07-27 22:51:54.696015 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/pretty.data.json
+-rw-r--r--   0        0        0     2087 2023-07-27 22:51:54.696245 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/pretty.meta.json
+-rw-r--r--   0        0        0   166552 2023-07-27 22:51:55.218332 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/progress.data.json
+-rw-r--r--   0        0        0     2214 2023-07-27 22:51:55.218644 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/progress.meta.json
+-rw-r--r--   0        0        0    15415 2023-07-27 22:51:54.735850 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/progress_bar.data.json
+-rw-r--r--   0        0        0     1922 2023-07-27 22:51:54.736079 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/progress_bar.meta.json
+-rw-r--r--   0        0        0     3348 2023-07-27 22:51:54.679067 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/protocol.data.json
+-rw-r--r--   0        0        0     1700 2023-07-27 22:51:54.679385 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/protocol.meta.json
+-rw-r--r--   0        0        0    16641 2023-07-27 22:51:51.472465 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/region.data.json
+-rw-r--r--   0        0        0     1513 2023-07-27 22:51:51.472643 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/region.meta.json
+-rw-r--r--   0        0        0    22715 2023-07-27 22:51:54.688075 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/repr.data.json
+-rw-r--r--   0        0        0     1782 2023-07-27 22:51:54.688254 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/repr.meta.json
+-rw-r--r--   0        0        0     8266 2023-07-27 22:51:54.704276 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/rule.data.json
+-rw-r--r--   0        0        0     1892 2023-07-27 22:51:54.704560 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/rule.meta.json
+-rw-r--r--   0        0        0     4139 2023-07-27 22:51:54.693316 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/scope.data.json
+-rw-r--r--   0        0        0     1826 2023-07-27 22:51:54.693518 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/scope.meta.json
+-rw-r--r--   0        0        0     5279 2023-07-27 22:51:54.692886 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/screen.data.json
+-rw-r--r--   0        0        0     1747 2023-07-27 22:51:54.693077 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/screen.meta.json
+-rw-r--r--   0        0        0    97194 2023-07-27 22:51:54.692403 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/segment.data.json
+-rw-r--r--   0        0        0     1870 2023-07-27 22:51:54.692607 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/segment.meta.json
+-rw-r--r--   0        0        0     9990 2023-07-27 22:51:54.723042 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/spinner.data.json
+-rw-r--r--   0        0        0     1981 2023-07-27 22:51:54.723262 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/spinner.meta.json
+-rw-r--r--   0        0        0    12259 2023-07-27 22:51:54.723705 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/status.data.json
+-rw-r--r--   0        0        0     1828 2023-07-27 22:51:54.723927 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/status.meta.json
+-rw-r--r--   0        0        0    55357 2023-07-27 22:51:54.710594 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/style.data.json
+-rw-r--r--   0        0        0     1871 2023-07-27 22:51:54.710770 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/style.meta.json
+-rw-r--r--   0        0        0     5938 2023-07-27 22:51:54.690123 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/styled.data.json
+-rw-r--r--   0        0        0     1832 2023-07-27 22:51:54.690289 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/styled.meta.json
+-rw-r--r--   0        0        0    75721 2023-07-27 22:51:54.703588 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/syntax.data.json
+-rw-r--r--   0        0        0     2216 2023-07-27 22:51:54.703808 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/syntax.meta.json
+-rw-r--r--   0        0        0    77259 2023-07-27 22:51:54.709164 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/table.data.json
+-rw-r--r--   0        0        0     2092 2023-07-27 22:51:54.709361 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/table.meta.json
+-rw-r--r--   0        0        0     6379 2023-07-27 22:51:54.689675 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/terminal_theme.data.json
+-rw-r--r--   0        0        0     1722 2023-07-27 22:51:54.689847 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/terminal_theme.meta.json
+-rw-r--r--   0        0        0    86670 2023-07-27 22:51:54.707310 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/text.data.json
+-rw-r--r--   0        0        0     2061 2023-07-27 22:51:54.707513 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/text.meta.json
+-rw-r--r--   0        0        0    14036 2023-07-27 22:51:54.689224 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/theme.data.json
+-rw-r--r--   0        0        0     1821 2023-07-27 22:51:54.689397 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/theme.meta.json
+-rw-r--r--   0        0        0     1658 2023-07-27 22:51:54.715786 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/themes.data.json
+-rw-r--r--   0        0        0     1723 2023-07-27 22:51:54.715958 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/themes.meta.json
+-rw-r--r--   0        0        0    47952 2023-07-27 22:51:54.719828 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/traceback.data.json
+-rw-r--r--   0        0        0     2246 2023-07-27 22:51:54.720043 alacorder-81.1.4/alacorder/.mypy_cache/3.10/rich/traceback.meta.json
+-rw-r--r--   0        0        0    11172 2023-07-27 22:51:51.058986 alacorder-81.1.4/alacorder/.mypy_cache/3.10/runpy.data.json
+-rw-r--r--   0        0        0     1575 2023-07-27 22:51:51.059244 alacorder-81.1.4/alacorder/.mypy_cache/3.10/runpy.meta.json
+-rw-r--r--   0        0        0    24062 2023-07-27 22:51:50.920263 alacorder-81.1.4/alacorder/.mypy_cache/3.10/select.data.json
+-rw-r--r--   0        0        0     1611 2023-07-27 22:51:50.920534 alacorder-81.1.4/alacorder/.mypy_cache/3.10/select.meta.json
+-rw-r--r--   0        0        0    57297 2023-07-27 22:51:50.916460 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selectors.data.json
+-rw-r--r--   0        0        0     1604 2023-07-27 22:51:50.916681 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selectors.meta.json
+-rw-r--r--   0        0        0     1699 2023-07-27 22:51:51.525745 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/__init__.data.json
+-rw-r--r--   0        0        0     1517 2023-07-27 22:51:51.525924 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/__init__.meta.json
+-rw-r--r--   0        0        0     6503 2023-07-27 22:51:51.833322 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/common/__init__.data.json
+-rw-r--r--   0        0        0     1566 2023-07-27 22:51:51.833548 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/common/__init__.meta.json
+-rw-r--r--   0        0        0    41541 2023-07-27 22:51:51.524691 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/common/exceptions.data.json
+-rw-r--r--   0        0        0     1546 2023-07-27 22:51:51.524901 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/common/exceptions.meta.json
+-rw-r--r--   0        0        0     2370 2023-07-27 22:51:51.520521 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/types.data.json
+-rw-r--r--   0        0        0     1522 2023-07-27 22:51:51.520709 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/types.meta.json
+-rw-r--r--   0        0        0     4536 2023-07-27 22:51:54.409909 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/__init__.data.json
+-rw-r--r--   0        0        0     2506 2023-07-27 22:51:54.410104 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/__init__.meta.json
+-rw-r--r--   0        0        0     1621 2023-07-27 22:51:51.290691 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/__init__.data.json
+-rw-r--r--   0        0        0     1551 2023-07-27 22:51:51.290868 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/__init__.meta.json
+-rw-r--r--   0        0        0     5452 2023-07-27 22:51:52.503666 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/options.data.json
+-rw-r--r--   0        0        0     1808 2023-07-27 22:51:52.503847 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/options.meta.json
+-rw-r--r--   0        0        0     4030 2023-07-27 22:51:53.951302 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/service.data.json
+-rw-r--r--   0        0        0     1862 2023-07-27 22:51:53.951482 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/service.meta.json
+-rw-r--r--   0        0        0     4090 2023-07-27 22:51:54.014844 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/webdriver.data.json
+-rw-r--r--   0        0        0     2251 2023-07-27 22:51:54.015079 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/webdriver.meta.json
+-rw-r--r--   0        0        0     1637 2023-07-27 22:51:51.169272 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/__init__.data.json
+-rw-r--r--   0        0        0     1555 2023-07-27 22:51:51.169439 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/__init__.meta.json
+-rw-r--r--   0        0        0    23167 2023-07-27 22:51:52.124378 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/options.data.json
+-rw-r--r--   0        0        0     1794 2023-07-27 22:51:52.124570 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/options.meta.json
+-rw-r--r--   0        0        0     3738 2023-07-27 22:51:53.689745 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/remote_connection.data.json
+-rw-r--r--   0        0        0     1711 2023-07-27 22:51:53.689984 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/remote_connection.meta.json
+-rw-r--r--   0        0        0     4971 2023-07-27 22:51:53.807701 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/service.data.json
+-rw-r--r--   0        0        0     1683 2023-07-27 22:51:53.807971 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/service.meta.json
+-rw-r--r--   0        0        0    14628 2023-07-27 22:51:53.832728 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/webdriver.data.json
+-rw-r--r--   0        0        0     1905 2023-07-27 22:51:53.832995 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/webdriver.meta.json
+-rw-r--r--   0        0        0     1621 2023-07-27 22:51:51.525244 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/__init__.data.json
+-rw-r--r--   0        0        0     1551 2023-07-27 22:51:51.525425 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/__init__.meta.json
+-rw-r--r--   0        0        0    13766 2023-07-27 22:51:53.961525 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/action_chains.data.json
+-rw-r--r--   0        0        0     2147 2023-07-27 22:51:53.961734 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/action_chains.meta.json
+-rw-r--r--   0        0        0     1685 2023-07-27 22:51:51.168772 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/__init__.data.json
+-rw-r--r--   0        0        0     1567 2023-07-27 22:51:51.168957 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/__init__.meta.json
+-rw-r--r--   0        0        0    20173 2023-07-27 22:51:53.829139 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/action_builder.data.json
+-rw-r--r--   0        0        0     2180 2023-07-27 22:51:53.829413 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/action_builder.meta.json
+-rw-r--r--   0        0        0     4226 2023-07-27 22:51:51.751864 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/input_device.data.json
+-rw-r--r--   0        0        0     1598 2023-07-27 22:51:51.752111 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/input_device.meta.json
+-rw-r--r--   0        0        0     8761 2023-07-27 22:51:51.168261 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/interaction.data.json
+-rw-r--r--   0        0        0     1584 2023-07-27 22:51:51.168473 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/interaction.meta.json
+-rw-r--r--   0        0        0     5444 2023-07-27 22:51:52.387700 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_actions.data.json
+-rw-r--r--   0        0        0     1841 2023-07-27 22:51:52.387923 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_actions.meta.json
+-rw-r--r--   0        0        0    10528 2023-07-27 22:51:52.121610 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_input.data.json
+-rw-r--r--   0        0        0     1771 2023-07-27 22:51:52.121801 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_input.meta.json
+-rw-r--r--   0        0        0     3685 2023-07-27 22:51:51.091287 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/mouse_button.data.json
+-rw-r--r--   0        0        0     1584 2023-07-27 22:51:51.091472 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/mouse_button.meta.json
+-rw-r--r--   0        0        0     8595 2023-07-27 22:51:53.729497 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_actions.data.json
+-rw-r--r--   0        0        0     1936 2023-07-27 22:51:53.729752 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_actions.meta.json
+-rw-r--r--   0        0        0     8606 2023-07-27 22:51:53.695767 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_input.data.json
+-rw-r--r--   0        0        0     1872 2023-07-27 22:51:53.696015 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_input.meta.json
+-rw-r--r--   0        0        0     4617 2023-07-27 22:51:53.727774 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_actions.data.json
+-rw-r--r--   0        0        0     1790 2023-07-27 22:51:53.727966 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_actions.meta.json
+-rw-r--r--   0        0        0    16869 2023-07-27 22:51:53.694162 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_input.data.json
+-rw-r--r--   0        0        0     1853 2023-07-27 22:51:53.694421 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_input.meta.json
+-rw-r--r--   0        0        0     4692 2023-07-27 22:51:52.504572 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/alert.data.json
+-rw-r--r--   0        0        0     1678 2023-07-27 22:51:52.504760 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/alert.meta.json
+-rw-r--r--   0        0        0     4120 2023-07-27 22:51:51.533761 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/by.data.json
+-rw-r--r--   0        0        0     1549 2023-07-27 22:51:51.533965 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/by.meta.json
+-rw-r--r--   0        0        0     6232 2023-07-27 22:51:51.451729 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/desired_capabilities.data.json
+-rw-r--r--   0        0        0     1585 2023-07-27 22:51:51.451916 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/desired_capabilities.meta.json
+-rw-r--r--   0        0        0     5335 2023-07-27 22:51:53.830157 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/driver_finder.data.json
+-rw-r--r--   0        0        0     1826 2023-07-27 22:51:53.830365 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/driver_finder.meta.json
+-rw-r--r--   0        0        0     1669 2023-07-27 22:51:51.203250 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/__init__.data.json
+-rw-r--r--   0        0        0     1563 2023-07-27 22:51:51.203462 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/__init__.meta.json
+-rw-r--r--   0        0        0     5987 2023-07-27 22:51:52.129612 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/application_cache.data.json
+-rw-r--r--   0        0        0     1709 2023-07-27 22:51:52.129799 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/application_cache.meta.json
+-rw-r--r--   0        0        0    18376 2023-07-27 22:51:51.450533 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/keys.data.json
+-rw-r--r--   0        0        0     1553 2023-07-27 22:51:51.450725 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/keys.meta.json
+-rw-r--r--   0        0        0    41319 2023-07-27 22:51:51.832468 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/options.data.json
+-rw-r--r--   0        0        0     1633 2023-07-27 22:51:51.832712 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/options.meta.json
+-rw-r--r--   0        0        0    44609 2023-07-27 22:51:51.431729 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/print_page_options.data.json
+-rw-r--r--   0        0        0     1610 2023-07-27 22:51:51.431951 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/print_page_options.meta.json
+-rw-r--r--   0        0        0    39687 2023-07-27 22:51:51.448935 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/proxy.data.json
+-rw-r--r--   0        0        0     1556 2023-07-27 22:51:51.449150 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/proxy.meta.json
+-rw-r--r--   0        0        0     7313 2023-07-27 22:51:52.104945 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/selenium_manager.data.json
+-rw-r--r--   0        0        0     1769 2023-07-27 22:51:52.105153 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/selenium_manager.meta.json
+-rw-r--r--   0        0        0    18666 2023-07-27 22:51:53.739306 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/service.data.json
+-rw-r--r--   0        0        0     1966 2023-07-27 22:51:53.739531 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/service.meta.json
+-rw-r--r--   0        0        0    14572 2023-07-27 22:51:51.427575 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/timeouts.data.json
+-rw-r--r--   0        0        0     1590 2023-07-27 22:51:51.427786 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/timeouts.meta.json
+-rw-r--r--   0        0        0     7519 2023-07-27 22:51:52.130790 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/utils.data.json
+-rw-r--r--   0        0        0     1673 2023-07-27 22:51:52.130975 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/utils.meta.json
+-rw-r--r--   0        0        0    32524 2023-07-27 22:51:51.828660 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/virtual_authenticator.data.json
+-rw-r--r--   0        0        0     1657 2023-07-27 22:51:51.828913 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/common/virtual_authenticator.meta.json
+-rw-r--r--   0        0        0     1605 2023-07-27 22:51:51.290211 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/__init__.data.json
+-rw-r--r--   0        0        0     1547 2023-07-27 22:51:51.290387 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/__init__.meta.json
+-rw-r--r--   0        0        0     9095 2023-07-27 22:51:52.502732 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/options.data.json
+-rw-r--r--   0        0        0     1804 2023-07-27 22:51:52.502926 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/options.meta.json
+-rw-r--r--   0        0        0     4119 2023-07-27 22:51:53.950302 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/service.data.json
+-rw-r--r--   0        0        0     1876 2023-07-27 22:51:53.950509 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/service.meta.json
+-rw-r--r--   0        0        0     4186 2023-07-27 22:51:54.013470 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/webdriver.data.json
+-rw-r--r--   0        0        0     2243 2023-07-27 22:51:54.013686 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/webdriver.meta.json
+-rw-r--r--   0        0        0     1629 2023-07-27 22:51:51.289686 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/__init__.data.json
+-rw-r--r--   0        0        0     1553 2023-07-27 22:51:51.289877 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/__init__.meta.json
+-rw-r--r--   0        0        0     9300 2023-07-27 22:51:52.397539 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_binary.data.json
+-rw-r--r--   0        0        0     1880 2023-07-27 22:51:52.397747 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_binary.meta.json
+-rw-r--r--   0        0        0    20936 2023-07-27 22:51:53.835923 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_profile.data.json
+-rw-r--r--   0        0        0     1983 2023-07-27 22:51:53.836128 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_profile.meta.json
+-rw-r--r--   0        0        0    25302 2023-07-27 22:51:53.959165 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/options.data.json
+-rw-r--r--   0        0        0     1954 2023-07-27 22:51:53.959371 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/options.meta.json
+-rw-r--r--   0        0        0     4116 2023-07-27 22:51:53.692158 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/remote_connection.data.json
+-rw-r--r--   0        0        0     1795 2023-07-27 22:51:53.692394 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/remote_connection.meta.json
+-rw-r--r--   0        0        0     5190 2023-07-27 22:51:53.826508 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/service.data.json
+-rw-r--r--   0        0        0     1730 2023-07-27 22:51:53.826758 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/service.meta.json
+-rw-r--r--   0        0        0    13608 2023-07-27 22:51:54.012015 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/webdriver.data.json
+-rw-r--r--   0        0        0     2200 2023-07-27 22:51:54.012259 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/webdriver.meta.json
+-rw-r--r--   0        0        0     1589 2023-07-27 22:51:51.224777 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/__init__.data.json
+-rw-r--r--   0        0        0     1543 2023-07-27 22:51:51.224952 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/__init__.meta.json
+-rw-r--r--   0        0        0    66756 2023-07-27 22:51:52.138417 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/options.data.json
+-rw-r--r--   0        0        0     1735 2023-07-27 22:51:52.138616 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/options.meta.json
+-rw-r--r--   0        0        0     4872 2023-07-27 22:51:53.824955 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/service.data.json
+-rw-r--r--   0        0        0     1670 2023-07-27 22:51:53.825191 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/service.meta.json
+-rw-r--r--   0        0        0     5908 2023-07-27 22:51:53.956243 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/webdriver.data.json
+-rw-r--r--   0        0        0     2066 2023-07-27 22:51:53.956426 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/webdriver.meta.json
+-rw-r--r--   0        0        0     1621 2023-07-27 22:51:51.432275 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/__init__.data.json
+-rw-r--r--   0        0        0     1551 2023-07-27 22:51:51.432453 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/__init__.meta.json
+-rw-r--r--   0        0        0     4196 2023-07-27 22:51:51.425474 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/bidi_connection.data.json
+-rw-r--r--   0        0        0     1574 2023-07-27 22:51:51.425685 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/bidi_connection.meta.json
+-rw-r--r--   0        0        0    23955 2023-07-27 22:51:51.434288 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/command.data.json
+-rw-r--r--   0        0        0     1559 2023-07-27 22:51:51.434498 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/command.meta.json
+-rw-r--r--   0        0        0    21125 2023-07-27 22:51:52.128710 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/errorhandler.data.json
+-rw-r--r--   0        0        0     1661 2023-07-27 22:51:52.128913 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/errorhandler.meta.json
+-rw-r--r--   0        0        0     8036 2023-07-27 22:51:52.413192 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/file_detector.data.json
+-rw-r--r--   0        0        0     1686 2023-07-27 22:51:52.413388 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/file_detector.meta.json
+-rw-r--r--   0        0        0    13316 2023-07-27 22:51:52.125898 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/mobile.data.json
+-rw-r--r--   0        0        0     1673 2023-07-27 22:51:52.126088 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/mobile.meta.json
+-rw-r--r--   0        0        0    17165 2023-07-27 22:51:52.411888 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/remote_connection.data.json
+-rw-r--r--   0        0        0     2044 2023-07-27 22:51:52.412128 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/remote_connection.meta.json
+-rw-r--r--   0        0        0     4743 2023-07-27 22:51:51.825635 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/script_key.data.json
+-rw-r--r--   0        0        0     1578 2023-07-27 22:51:51.825864 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/script_key.meta.json
+-rw-r--r--   0        0        0     7947 2023-07-27 22:51:51.824633 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/shadowroot.data.json
+-rw-r--r--   0        0        0     1690 2023-07-27 22:51:51.824856 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/shadowroot.meta.json
+-rw-r--r--   0        0        0    10338 2023-07-27 22:51:53.699484 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/switch_to.data.json
+-rw-r--r--   0        0        0     1865 2023-07-27 22:51:53.699731 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/switch_to.meta.json
+-rw-r--r--   0        0        0     3026 2023-07-27 22:51:52.107708 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/utils.data.json
+-rw-r--r--   0        0        0     1610 2023-07-27 22:51:52.107900 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/utils.meta.json
+-rw-r--r--   0        0        0    86571 2023-07-27 22:51:53.779608 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webdriver.data.json
+-rw-r--r--   0        0        0     2659 2023-07-27 22:51:53.779883 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webdriver.meta.json
+-rw-r--r--   0        0        0    38535 2023-07-27 22:51:52.416637 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webelement.data.json
+-rw-r--r--   0        0        0     1953 2023-07-27 22:51:52.416836 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webelement.meta.json
+-rw-r--r--   0        0        0     1621 2023-07-27 22:51:51.224259 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/__init__.data.json
+-rw-r--r--   0        0        0     1551 2023-07-27 22:51:51.224446 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/__init__.meta.json
+-rw-r--r--   0        0        0    21535 2023-07-27 22:51:52.117497 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/options.data.json
+-rw-r--r--   0        0        0     1731 2023-07-27 22:51:52.117699 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/options.meta.json
+-rw-r--r--   0        0        0     3894 2023-07-27 22:51:53.691288 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/remote_connection.data.json
+-rw-r--r--   0        0        0     1793 2023-07-27 22:51:53.691502 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/remote_connection.meta.json
+-rw-r--r--   0        0        0    11250 2023-07-27 22:51:53.823114 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/service.data.json
+-rw-r--r--   0        0        0     1719 2023-07-27 22:51:53.823350 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/service.meta.json
+-rw-r--r--   0        0        0     6946 2023-07-27 22:51:53.954917 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/webdriver.data.json
+-rw-r--r--   0        0        0     2225 2023-07-27 22:51:53.955115 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/webdriver.meta.json
+-rw-r--r--   0        0        0     1629 2023-07-27 22:51:51.533043 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/__init__.data.json
+-rw-r--r--   0        0        0     1553 2023-07-27 22:51:51.533224 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/__init__.meta.json
+-rw-r--r--   0        0        0    43134 2023-07-27 22:51:54.739722 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/expected_conditions.data.json
+-rw-r--r--   0        0        0     2437 2023-07-27 22:51:54.739937 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/expected_conditions.meta.json
+-rw-r--r--   0        0        0    12491 2023-07-27 22:51:53.701220 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/relative_locator.data.json
+-rw-r--r--   0        0        0     1802 2023-07-27 22:51:53.701469 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/relative_locator.meta.json
+-rw-r--r--   0        0        0    16482 2023-07-27 22:51:53.709063 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/select.data.json
+-rw-r--r--   0        0        0     1772 2023-07-27 22:51:53.709294 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/select.meta.json
+-rw-r--r--   0        0        0     1621 2023-07-27 22:51:53.780280 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/ui.data.json
+-rw-r--r--   0        0        0     1673 2023-07-27 22:51:53.780508 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/ui.meta.json
+-rw-r--r--   0        0        0     7542 2023-07-27 22:51:51.859591 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/wait.data.json
+-rw-r--r--   0        0        0     1690 2023-07-27 22:51:51.859811 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/support/wait.meta.json
+-rw-r--r--   0        0        0     1645 2023-07-27 22:51:51.221272 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/__init__.data.json
+-rw-r--r--   0        0        0     1557 2023-07-27 22:51:51.221452 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/__init__.meta.json
+-rw-r--r--   0        0        0    10920 2023-07-27 22:51:52.133995 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/options.data.json
+-rw-r--r--   0        0        0     1736 2023-07-27 22:51:52.134175 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/options.meta.json
+-rw-r--r--   0        0        0     5051 2023-07-27 22:51:53.821141 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/service.data.json
+-rw-r--r--   0        0        0     1695 2023-07-27 22:51:53.821343 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/service.meta.json
+-rw-r--r--   0        0        0     4009 2023-07-27 22:51:53.953319 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/webdriver.data.json
+-rw-r--r--   0        0        0     2076 2023-07-27 22:51:53.953521 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/webdriver.meta.json
+-rw-r--r--   0        0        0     1645 2023-07-27 22:51:51.220755 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/__init__.data.json
+-rw-r--r--   0        0        0     1557 2023-07-27 22:51:51.220952 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/__init__.meta.json
+-rw-r--r--   0        0        0     8817 2023-07-27 22:51:52.132750 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/options.data.json
+-rw-r--r--   0        0        0     1736 2023-07-27 22:51:52.132936 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/options.meta.json
+-rw-r--r--   0        0        0     5051 2023-07-27 22:51:53.819635 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/service.data.json
+-rw-r--r--   0        0        0     1695 2023-07-27 22:51:53.819873 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/service.meta.json
+-rw-r--r--   0        0        0     4140 2023-07-27 22:51:53.952307 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/webdriver.data.json
+-rw-r--r--   0        0        0     2130 2023-07-27 22:51:53.952499 alacorder-81.1.4/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/webdriver.meta.json
+-rw-r--r--   0        0        0    16870 2023-07-27 22:51:51.160269 alacorder-81.1.4/alacorder/.mypy_cache/3.10/shlex.data.json
+-rw-r--r--   0        0        0     1598 2023-07-27 22:51:51.160490 alacorder-81.1.4/alacorder/.mypy_cache/3.10/shlex.meta.json
+-rw-r--r--   0        0        0    74731 2023-07-27 22:51:51.442973 alacorder-81.1.4/alacorder/.mypy_cache/3.10/shutil.data.json
+-rw-r--r--   0        0        0     1609 2023-07-27 22:51:51.443218 alacorder-81.1.4/alacorder/.mypy_cache/3.10/shutil.meta.json
+-rw-r--r--   0        0        0    31654 2023-07-27 22:51:50.973756 alacorder-81.1.4/alacorder/.mypy_cache/3.10/signal.data.json
+-rw-r--r--   0        0        0     1622 2023-07-27 22:51:50.973971 alacorder-81.1.4/alacorder/.mypy_cache/3.10/signal.meta.json
+-rw-r--r--   0        0        0    15355 2023-07-27 22:51:51.056782 alacorder-81.1.4/alacorder/.mypy_cache/3.10/site.data.json
+-rw-r--r--   0        0        0     1571 2023-07-27 22:51:51.057152 alacorder-81.1.4/alacorder/.mypy_cache/3.10/site.meta.json
+-rw-r--r--   0        0        0    81904 2023-07-27 22:51:51.772321 alacorder-81.1.4/alacorder/.mypy_cache/3.10/socket.data.json
+-rw-r--r--   0        0        0     1646 2023-07-27 22:51:51.772637 alacorder-81.1.4/alacorder/.mypy_cache/3.10/socket.meta.json
+-rw-r--r--   0        0        0     9454 2023-07-27 22:51:52.006338 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sqlite3/__init__.data.json
+-rw-r--r--   0        0        0     1557 2023-07-27 22:51:52.006514 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sqlite3/__init__.meta.json
+-rw-r--r--   0        0        0   125428 2023-07-27 22:51:52.005796 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sqlite3/dbapi2.data.json
+-rw-r--r--   0        0        0     1668 2023-07-27 22:51:52.006024 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sqlite3/dbapi2.meta.json
+-rw-r--r--   0        0        0    14126 2023-07-27 22:51:50.795141 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1580 2023-07-27 22:51:50.795298 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    28376 2023-07-27 22:51:50.794575 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1592 2023-07-27 22:51:50.794751 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    49437 2023-07-27 22:51:50.793738 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1635 2023-07-27 22:51:50.793918 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   194734 2023-07-27 22:51:52.103506 alacorder-81.1.4/alacorder/.mypy_cache/3.10/ssl.data.json
+-rw-r--r--   0        0        0     1688 2023-07-27 22:51:52.103803 alacorder-81.1.4/alacorder/.mypy_cache/3.10/ssl.meta.json
+-rw-r--r--   0        0        0     3103 2023-07-27 22:51:54.028115 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/__init__.data.json
+-rw-r--r--   0        0        0     1773 2023-07-27 22:51:54.028278 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/__init__.meta.json
+-rw-r--r--   0        0        0   105961 2023-07-27 22:51:53.976749 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/core.data.json
+-rw-r--r--   0        0        0     1941 2023-07-27 22:51:53.977000 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/core.meta.json
+-rw-r--r--   0        0        0    18186 2023-07-27 22:51:54.027716 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/formatting.data.json
+-rw-r--r--   0        0        0     1852 2023-07-27 22:51:54.027907 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/formatting.meta.json
+-rw-r--r--   0        0        0    17765 2023-07-27 22:51:54.026999 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/serializing.data.json
+-rw-r--r--   0        0        0     1906 2023-07-27 22:51:54.027229 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/serializing.meta.json
+-rw-r--r--   0        0        0    17975 2023-07-27 22:51:52.951051 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/utils.data.json
+-rw-r--r--   0        0        0     1681 2023-07-27 22:51:52.951343 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/utils.meta.json
+-rw-r--r--   0        0        0     1542 2023-07-27 22:51:50.974330 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/version.data.json
+-rw-r--r--   0        0        0     1527 2023-07-27 22:51:50.974514 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stack_data/version.meta.json
+-rw-r--r--   0        0        0     6525 2023-07-27 22:51:51.749944 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stat.data.json
+-rw-r--r--   0        0        0     1533 2023-07-27 22:51:51.750160 alacorder-81.1.4/alacorder/.mypy_cache/3.10/stat.meta.json
+-rw-r--r--   0        0        0    27389 2023-07-27 22:51:51.190660 alacorder-81.1.4/alacorder/.mypy_cache/3.10/string.data.json
+-rw-r--r--   0        0        0     1620 2023-07-27 22:51:51.190881 alacorder-81.1.4/alacorder/.mypy_cache/3.10/string.meta.json
+-rw-r--r--   0        0        0    14908 2023-07-27 22:51:51.100652 alacorder-81.1.4/alacorder/.mypy_cache/3.10/struct.data.json
+-rw-r--r--   0        0        0     1589 2023-07-27 22:51:51.100834 alacorder-81.1.4/alacorder/.mypy_cache/3.10/struct.meta.json
+-rw-r--r--   0        0        0   160689 2023-07-27 22:51:50.792484 alacorder-81.1.4/alacorder/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1630 2023-07-27 22:51:50.792668 alacorder-81.1.4/alacorder/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   146609 2023-07-27 22:51:50.789156 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1668 2023-07-27 22:51:50.789348 alacorder-81.1.4/alacorder/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0   149722 2023-07-27 22:51:51.288856 alacorder-81.1.4/alacorder/.mypy_cache/3.10/tempfile.data.json
+-rw-r--r--   0        0        0     1636 2023-07-27 22:51:51.289195 alacorder-81.1.4/alacorder/.mypy_cache/3.10/tempfile.meta.json
+-rw-r--r--   0        0        0    47304 2023-07-27 22:51:51.155435 alacorder-81.1.4/alacorder/.mypy_cache/3.10/termios.data.json
+-rw-r--r--   0        0        0     1579 2023-07-27 22:51:51.155783 alacorder-81.1.4/alacorder/.mypy_cache/3.10/termios.meta.json
+-rw-r--r--   0        0        0    19548 2023-07-27 22:51:51.406435 alacorder-81.1.4/alacorder/.mypy_cache/3.10/textwrap.data.json
+-rw-r--r--   0        0        0     1562 2023-07-27 22:51:51.406642 alacorder-81.1.4/alacorder/.mypy_cache/3.10/textwrap.meta.json
+-rw-r--r--   0        0        0    65078 2023-07-27 22:51:51.507212 alacorder-81.1.4/alacorder/.mypy_cache/3.10/threading.data.json
+-rw-r--r--   0        0        0     1632 2023-07-27 22:51:51.507424 alacorder-81.1.4/alacorder/.mypy_cache/3.10/threading.meta.json
+-rw-r--r--   0        0        0    42804 2023-07-27 22:51:51.530923 alacorder-81.1.4/alacorder/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1573 2023-07-27 22:51:51.531147 alacorder-81.1.4/alacorder/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0    11963 2023-07-27 22:51:50.960311 alacorder-81.1.4/alacorder/.mypy_cache/3.10/timeit.data.json
+-rw-r--r--   0        0        0     1572 2023-07-27 22:51:50.960547 alacorder-81.1.4/alacorder/.mypy_cache/3.10/timeit.meta.json
+-rw-r--r--   0        0        0    14908 2023-07-27 22:51:51.004277 alacorder-81.1.4/alacorder/.mypy_cache/3.10/token.data.json
+-rw-r--r--   0        0        0     1553 2023-07-27 22:51:51.004463 alacorder-81.1.4/alacorder/.mypy_cache/3.10/token.meta.json
+-rw-r--r--   0        0        0    50645 2023-07-27 22:51:51.691535 alacorder-81.1.4/alacorder/.mypy_cache/3.10/tokenize.data.json
+-rw-r--r--   0        0        0     1634 2023-07-27 22:51:51.691795 alacorder-81.1.4/alacorder/.mypy_cache/3.10/tokenize.meta.json
+-rw-r--r--   0        0        0    52276 2023-07-27 22:51:51.303153 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traceback.data.json
+-rw-r--r--   0        0        0     1617 2023-07-27 22:51:51.303379 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traceback.meta.json
+-rw-r--r--   0        0        0    10743 2023-07-27 22:51:53.805666 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/__init__.data.json
+-rw-r--r--   0        0        0     1779 2023-07-27 22:51:53.805881 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/__init__.meta.json
+-rw-r--r--   0        0        0     2729 2023-07-27 22:51:51.015011 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/_version.data.json
+-rw-r--r--   0        0        0     1579 2023-07-27 22:51:51.015189 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/_version.meta.json
+-rw-r--r--   0        0        0     9740 2023-07-27 22:51:53.943469 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/config/__init__.data.json
+-rw-r--r--   0        0        0     1809 2023-07-27 22:51:53.943671 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/config/__init__.meta.json
+-rw-r--r--   0        0        0    52790 2023-07-27 22:51:53.942834 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/config/application.data.json
+-rw-r--r--   0        0        0     2190 2023-07-27 22:51:53.943056 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/config/application.meta.json
+-rw-r--r--   0        0        0     9820 2023-07-27 22:51:51.697920 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/config/argcomplete_config.data.json
+-rw-r--r--   0        0        0     1632 2023-07-27 22:51:51.698124 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/config/argcomplete_config.meta.json
+-rw-r--r--   0        0        0    25129 2023-07-27 22:51:53.941417 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/config/configurable.data.json
+-rw-r--r--   0        0        0     1927 2023-07-27 22:51:53.941614 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/config/configurable.meta.json
+-rw-r--r--   0        0        0    59616 2023-07-27 22:51:53.940471 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/config/loader.data.json
+-rw-r--r--   0        0        0     2089 2023-07-27 22:51:53.940781 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/config/loader.meta.json
+-rw-r--r--   0        0        0     1808 2023-07-27 22:51:52.009566 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/log.data.json
+-rw-r--r--   0        0        0     1533 2023-07-27 22:51:52.009739 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/log.meta.json
+-rw-r--r--   0        0        0   176934 2023-07-27 22:51:52.993488 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/traitlets.data.json
+-rw-r--r--   0        0        0     1949 2023-07-27 22:51:52.993804 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/traitlets.meta.json
+-rw-r--r--   0        0        0     2477 2023-07-27 22:51:51.017274 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/__init__.data.json
+-rw-r--r--   0        0        0     1557 2023-07-27 22:51:51.017500 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3168 2023-07-27 22:51:51.015862 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/bunch.data.json
+-rw-r--r--   0        0        0     1534 2023-07-27 22:51:51.016033 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/bunch.meta.json
+-rw-r--r--   0        0        0     4087 2023-07-27 22:51:53.723915 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/decorators.data.json
+-rw-r--r--   0        0        0     1639 2023-07-27 22:51:53.724142 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/decorators.meta.json
+-rw-r--r--   0        0        0     2995 2023-07-27 22:51:52.194020 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/descriptions.data.json
+-rw-r--r--   0        0        0     1630 2023-07-27 22:51:52.194204 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/descriptions.meta.json
+-rw-r--r--   0        0        0     1801 2023-07-27 22:51:52.193301 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/getargspec.data.json
+-rw-r--r--   0        0        0     1621 2023-07-27 22:51:52.193489 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/getargspec.meta.json
+-rw-r--r--   0        0        0     1660 2023-07-27 22:51:51.071193 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/importstring.data.json
+-rw-r--r--   0        0        0     1549 2023-07-27 22:51:51.071371 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/importstring.meta.json
+-rw-r--r--   0        0        0     1683 2023-07-27 22:51:51.017868 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/nested_update.data.json
+-rw-r--r--   0        0        0     1550 2023-07-27 22:51:51.018081 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/nested_update.meta.json
+-rw-r--r--   0        0        0     3734 2023-07-27 22:51:50.975271 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/sentinel.data.json
+-rw-r--r--   0        0        0     1540 2023-07-27 22:51:50.975450 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/sentinel.meta.json
+-rw-r--r--   0        0        0     2671 2023-07-27 22:51:51.698616 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/text.data.json
+-rw-r--r--   0        0        0     1557 2023-07-27 22:51:51.698799 alacorder-81.1.4/alacorder/.mypy_cache/3.10/traitlets/utils/text.meta.json
+-rw-r--r--   0        0        0     4821 2023-07-27 22:51:51.156975 alacorder-81.1.4/alacorder/.mypy_cache/3.10/tty.data.json
+-rw-r--r--   0        0        0     1554 2023-07-27 22:51:51.157219 alacorder-81.1.4/alacorder/.mypy_cache/3.10/tty.meta.json
+-rw-r--r--   0        0        0     4681 2023-07-27 22:51:55.194723 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/__init__.data.json
+-rw-r--r--   0        0        0     1814 2023-07-27 22:51:55.194890 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/__init__.meta.json
+-rw-r--r--   0        0        0     1986 2023-07-27 22:51:53.690410 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1585 2023-07-27 22:51:53.690617 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0    11451 2023-07-27 22:51:53.686897 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1689 2023-07-27 22:51:53.687130 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    34919 2023-07-27 22:51:51.150348 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/_typing.data.json
+-rw-r--r--   0        0        0     1618 2023-07-27 22:51:51.150587 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4838 2023-07-27 22:51:51.443867 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/colors.data.json
+-rw-r--r--   0        0        0     1516 2023-07-27 22:51:51.444081 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/colors.meta.json
+-rw-r--r--   0        0        0     8891 2023-07-27 22:51:55.191676 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/completion.data.json
+-rw-r--r--   0        0        0     1898 2023-07-27 22:51:55.191860 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/completion.meta.json
+-rw-r--r--   0        0        0    47497 2023-07-27 22:51:55.192930 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/core.data.json
+-rw-r--r--   0        0        0     1986 2023-07-27 22:51:55.193124 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/core.meta.json
+-rw-r--r--   0        0        0    53328 2023-07-27 22:51:55.194287 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/main.data.json
+-rw-r--r--   0        0        0     2017 2023-07-27 22:51:55.194476 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/main.meta.json
+-rw-r--r--   0        0        0    68816 2023-07-27 22:51:55.188906 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/models.data.json
+-rw-r--r--   0        0        0     1849 2023-07-27 22:51:55.189193 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/models.meta.json
+-rw-r--r--   0        0        0    56950 2023-07-27 22:51:55.191171 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/params.data.json
+-rw-r--r--   0        0        0     1764 2023-07-27 22:51:55.191365 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/params.meta.json
+-rw-r--r--   0        0        0    31605 2023-07-27 22:51:54.732943 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2064 2023-07-27 22:51:54.733163 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    17435 2023-07-27 22:51:55.189678 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/utils.data.json
+-rw-r--r--   0        0        0     1751 2023-07-27 22:51:55.189873 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typer/utils.meta.json
+-rw-r--r--   0        0        0   247729 2023-07-27 22:51:50.786255 alacorder-81.1.4/alacorder/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1646 2023-07-27 22:51:50.786463 alacorder-81.1.4/alacorder/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   497098 2023-07-27 22:51:50.781539 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1644 2023-07-27 22:51:50.781805 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0   109900 2023-07-27 22:51:50.771349 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1653 2023-07-27 22:51:50.771664 alacorder-81.1.4/alacorder/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    46483 2023-07-27 22:51:50.993991 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unicodedata.data.json
+-rw-r--r--   0        0        0     1587 2023-07-27 22:51:50.994210 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unicodedata.meta.json
+-rw-r--r--   0        0        0     5970 2023-07-27 22:51:52.048611 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1751 2023-07-27 22:51:52.048815 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    25995 2023-07-27 22:51:52.039640 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/_log.data.json
+-rw-r--r--   0        0        0     1614 2023-07-27 22:51:52.039820 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/_log.meta.json
+-rw-r--r--   0        0        0     8253 2023-07-27 22:51:52.045018 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1645 2023-07-27 22:51:52.045219 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   229952 2023-07-27 22:51:52.044393 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/case.data.json
+-rw-r--r--   0        0        0     1744 2023-07-27 22:51:52.044664 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/case.meta.json
+-rw-r--r--   0        0        0    14613 2023-07-27 22:51:52.047491 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/loader.data.json
+-rw-r--r--   0        0        0     1670 2023-07-27 22:51:52.047704 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11721 2023-07-27 22:51:52.048109 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/main.data.json
+-rw-r--r--   0        0        0     1679 2023-07-27 22:51:52.048315 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/main.meta.json
+-rw-r--r--   0        0        0    20941 2023-07-27 22:51:52.038701 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/result.data.json
+-rw-r--r--   0        0        0     1632 2023-07-27 22:51:52.038976 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/result.meta.json
+-rw-r--r--   0        0        0    10740 2023-07-27 22:51:52.046839 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/runner.data.json
+-rw-r--r--   0        0        0     1672 2023-07-27 22:51:52.047022 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12915 2023-07-27 22:51:52.046241 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/signals.data.json
+-rw-r--r--   0        0        0     1630 2023-07-27 22:51:52.046445 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11245 2023-07-27 22:51:52.045621 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/suite.data.json
+-rw-r--r--   0        0        0     1648 2023-07-27 22:51:52.045825 alacorder-81.1.4/alacorder/.mypy_cache/3.10/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1490 2023-07-27 22:51:51.187283 alacorder-81.1.4/alacorder/.mypy_cache/3.10/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1533 2023-07-27 22:51:51.187509 alacorder-81.1.4/alacorder/.mypy_cache/3.10/urllib/__init__.meta.json
+-rw-r--r--   0        0        0    11898 2023-07-27 22:51:51.719915 alacorder-81.1.4/alacorder/.mypy_cache/3.10/urllib/error.data.json
+-rw-r--r--   0        0        0     1592 2023-07-27 22:51:51.720109 alacorder-81.1.4/alacorder/.mypy_cache/3.10/urllib/error.meta.json
+-rw-r--r--   0        0        0   208725 2023-07-27 22:51:51.201986 alacorder-81.1.4/alacorder/.mypy_cache/3.10/urllib/parse.data.json
+-rw-r--r--   0        0        0     1624 2023-07-27 22:51:51.202790 alacorder-81.1.4/alacorder/.mypy_cache/3.10/urllib/parse.meta.json
+-rw-r--r--   0        0        0   151899 2023-07-27 22:51:53.077195 alacorder-81.1.4/alacorder/.mypy_cache/3.10/urllib/request.data.json
+-rw-r--r--   0        0        0     1817 2023-07-27 22:51:53.077420 alacorder-81.1.4/alacorder/.mypy_cache/3.10/urllib/request.meta.json
+-rw-r--r--   0        0        0    29044 2023-07-27 22:51:51.049901 alacorder-81.1.4/alacorder/.mypy_cache/3.10/urllib/response.data.json
+-rw-r--r--   0        0        0     1662 2023-07-27 22:51:51.050338 alacorder-81.1.4/alacorder/.mypy_cache/3.10/urllib/response.meta.json
+-rw-r--r--   0        0        0    33581 2023-07-27 22:51:51.211502 alacorder-81.1.4/alacorder/.mypy_cache/3.10/uuid.data.json
+-rw-r--r--   0        0        0     1585 2023-07-27 22:51:51.211703 alacorder-81.1.4/alacorder/.mypy_cache/3.10/uuid.meta.json
+-rw-r--r--   0        0        0    22600 2023-07-27 22:51:51.857381 alacorder-81.1.4/alacorder/.mypy_cache/3.10/warnings.data.json
+-rw-r--r--   0        0        0     1632 2023-07-27 22:51:51.857632 alacorder-81.1.4/alacorder/.mypy_cache/3.10/warnings.meta.json
+-rw-r--r--   0        0        0    55688 2023-07-27 22:51:51.098135 alacorder-81.1.4/alacorder/.mypy_cache/3.10/wave.data.json
+-rw-r--r--   0        0        0     1573 2023-07-27 22:51:51.098336 alacorder-81.1.4/alacorder/.mypy_cache/3.10/wave.meta.json
+-rw-r--r--   0        0        0   180578 2023-07-27 22:51:51.761773 alacorder-81.1.4/alacorder/.mypy_cache/3.10/weakref.data.json
+-rw-r--r--   0        0        0     1638 2023-07-27 22:51:51.762034 alacorder-81.1.4/alacorder/.mypy_cache/3.10/weakref.meta.json
+-rw-r--r--   0        0        0     2145 2023-07-27 22:51:51.160956 alacorder-81.1.4/alacorder/.mypy_cache/3.10/winreg.data.json
+-rw-r--r--   0        0        0     1573 2023-07-27 22:51:51.161164 alacorder-81.1.4/alacorder/.mypy_cache/3.10/winreg.meta.json
+-rw-r--r--   0        0        0     1545 2023-07-27 22:51:53.687471 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/__init__.data.json
+-rw-r--r--   0        0        0     1590 2023-07-27 22:51:53.687676 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/__init__.meta.json
+-rw-r--r--   0        0        0    25169 2023-07-27 22:51:52.120132 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/__init__.data.json
+-rw-r--r--   0        0        0     1601 2023-07-27 22:51:52.120340 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/__init__.meta.json
+-rw-r--r--   0        0        0     4698 2023-07-27 22:51:51.750850 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/domreg.data.json
+-rw-r--r--   0        0        0     1601 2023-07-27 22:51:51.751066 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/domreg.meta.json
+-rw-r--r--   0        0        0    62343 2023-07-27 22:51:53.764737 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/expatbuilder.data.json
+-rw-r--r--   0        0        0     1685 2023-07-27 22:51:53.764990 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/expatbuilder.meta.json
+-rw-r--r--   0        0        0    14690 2023-07-27 22:51:51.166923 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/minicompat.data.json
+-rw-r--r--   0        0        0     1595 2023-07-27 22:51:51.167160 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/minicompat.meta.json
+-rw-r--r--   0        0        0   162063 2023-07-27 22:51:53.768945 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/minidom.data.json
+-rw-r--r--   0        0        0     1754 2023-07-27 22:51:53.769156 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/minidom.meta.json
+-rw-r--r--   0        0        0    33641 2023-07-27 22:51:53.765751 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/xmlbuilder.data.json
+-rw-r--r--   0        0        0     1717 2023-07-27 22:51:53.765948 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/dom/xmlbuilder.meta.json
+-rw-r--r--   0        0        0     1613 2023-07-27 22:51:52.214001 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/parsers/__init__.data.json
+-rw-r--r--   0        0        0     1612 2023-07-27 22:51:52.214178 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/parsers/__init__.meta.json
+-rw-r--r--   0        0        0     2970 2023-07-27 22:51:52.049337 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/parsers/expat/__init__.data.json
+-rw-r--r--   0        0        0     1613 2023-07-27 22:51:52.049565 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/parsers/expat/__init__.meta.json
+-rw-r--r--   0        0        0    18023 2023-07-27 22:51:51.718221 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/sax/__init__.data.json
+-rw-r--r--   0        0        0     1667 2023-07-27 22:51:51.718419 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/sax/__init__.meta.json
+-rw-r--r--   0        0        0    18675 2023-07-27 22:51:51.044454 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/sax/handler.data.json
+-rw-r--r--   0        0        0     1572 2023-07-27 22:51:51.044639 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/sax/handler.meta.json
+-rw-r--r--   0        0        0    24713 2023-07-27 22:51:51.165066 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/sax/xmlreader.data.json
+-rw-r--r--   0        0        0     1571 2023-07-27 22:51:51.165297 alacorder-81.1.4/alacorder/.mypy_cache/3.10/xml/sax/xmlreader.meta.json
+-rw-r--r--   0        0        0    68729 2023-07-27 22:51:51.234427 alacorder-81.1.4/alacorder/.mypy_cache/3.10/zipfile.data.json
+-rw-r--r--   0        0        0     1632 2023-07-27 22:51:51.234697 alacorder-81.1.4/alacorder/.mypy_cache/3.10/zipfile.meta.json
+-rw-r--r--   0        0        0    13202 2023-07-27 22:51:50.986235 alacorder-81.1.4/alacorder/.mypy_cache/3.10/zipimport.data.json
+-rw-r--r--   0        0        0     1645 2023-07-27 22:51:50.986455 alacorder-81.1.4/alacorder/.mypy_cache/3.10/zipimport.meta.json
+-rw-r--r--   0        0        0    16688 2023-07-27 22:51:51.467483 alacorder-81.1.4/alacorder/.mypy_cache/3.10/zlib.data.json
+-rw-r--r--   0        0        0     1590 2023-07-27 22:51:51.467722 alacorder-81.1.4/alacorder/.mypy_cache/3.10/zlib.meta.json
+-rw-r--r--   0        0        0    21070 2023-07-27 22:51:52.081296 alacorder-81.1.4/alacorder/.mypy_cache/3.10/zoneinfo/__init__.data.json
+-rw-r--r--   0        0        0     1669 2023-07-27 22:51:52.081504 alacorder-81.1.4/alacorder/.mypy_cache/3.10/zoneinfo/__init__.meta.json
+-rw-r--r--   0        0        0      190 2023-07-27 22:51:55.510225 alacorder-81.1.4/alacorder/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-07-27 22:51:55.510310 alacorder-81.1.4/alacorder/.mypy_cache/missing_stubs
+-rw-r--r--   0        0        0       19 2023-07-25 19:20:19.054678 alacorder-81.1.4/alacorder/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-25 19:23:49.408885 alacorder-81.1.4/alacorder/__main__.py
+-rw-r--r--   0        0        0   255545 2023-08-03 21:08:45.413859 alacorder-81.1.4/alacorder/alac.py
+-rw-r--r--   0        0        0      557 2023-08-03 21:08:41.736077 alacorder-81.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 alacorder-81.1.4/PKG-INFO
```

### Comparing `alacorder-81.1.3/LICENSE` & `alacorder-81.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-81.1.3/README.md` & `alacorder-81.1.4/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-81.1.3/alacorder/alac.py` & `alacorder-81.1.4/alacorder/alac.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 ┣┫┃ ┣┫┃ ┃┃┣┫┃┃┣ ┣┫
 ┛┗┗┛┛┗┗┛┗┛┛┗┻┛┗┛┛┗
 (c) 2023 Sam Robson
 
 Dependencies: Python 3.9+, Google Chrome, brotli 1.0.9+, polars 0.18.1+, pymupdf 1.21.1+, rich 13.3.3+, selenium 4.8.3+, typer 0.9.0+, xlsx2csv 0.8.1+, xlsxwriter 3.0.9+
 """
 
-__version__ = "81.1.3"
+__version__ = "81.1.4"
 
 import os
 import re
 import glob
 import time
 from datetime import datetime
-import typer
-from typing_extensions import Annotated
 from pathlib import Path
+from typing_extensions import Annotated
+import typer
 from rich.progress import Progress, MofNCompleteColumn
 from rich.console import Console
 import fitz
 import polars as pl
 import xlsxwriter
 from bs4 import BeautifulSoup
 from selenium import webdriver
@@ -77,15 +77,15 @@
                 output.write_parquet(path, compression="brotli")
             if ext == ".json":
                 output.write_json(path),
             if ext == ".csv":
                 output.write_csv(path)
 
     if log:
-        with console.status("Writing to output path..."):
+        with console.status("Writing to output path…"):
             _write(output, path)
     else:
         _write(output, path)
 
 
 def read(source, all_sheets=False):
     """
@@ -143,24 +143,24 @@
         if os.path.isdir(source):
             paths = glob.glob(source + "**/*.pdf", recursive=True)
             all_text = []
             progress_bar = Progress(
                 *Progress.get_default_columns(), MofNCompleteColumn()
             )
             with progress_bar as p:
-                for path in p.track(paths, description="Reading PDFs..."):
+                for path in p.track(paths, description="Reading PDFs…"):
                     all_text += [extract_text(path)]
             output = pl.DataFrame(
                 {"Timestamp": time.time(), "AllPagesText": all_text, "Path": paths}
             )
     if isinstance(source, list):
         all_text = []
         progress_bar = Progress(*Progress.get_default_columns(), MofNCompleteColumn())
         with progress_bar as p:
-            for path in p.track(source, description="Reading PDFs..."):
+            for path in p.track(source, description="Reading PDFs…"):
                 all_text += [extract_text(path)]
         output = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": all_text, "Path": paths}
         )
     if isinstance(source, pl.DataFrame):
         output = source
     if isinstance(output, pl.DataFrame):
@@ -216,15 +216,15 @@
                 },
             )
         if dirpath != None:
             self.dirpath = os.path.abspath(dirpath)
         else:
             self.dirpath = None
         self.headless = headless
-        with console.status("Starting WebDriver (requires Google Chrome)..."):
+        with console.status("Starting WebDriver (requires Google Chrome)…"):
             self.driver = webdriver.Chrome(options=opt)
         self.party_search_queue = None
         self.case_number_queue = None
         self.output = None
         self.cID = cID
         self.uID = uID
         self.pwd = pwd
@@ -273,15 +273,15 @@
         if pwd != None:
             self.pwd = pwd
 
         if self.cID == None or self.uID == None or self.pwd == None:
             raise Exception("Must enter Alacourt credentials to login.")
 
         if log:
-            with console.status("Logging in to Alacourt..."):
+            with console.status("Logging in to Alacourt…"):
                 return _login(self.driver, self.cID, self.uID, self.pwd)
         else:
             return _login(self.driver, self.cID, self.uID, self.pwd)
 
 
     # party search
     def set_party_search_queue(self, queue) -> None:
@@ -539,15 +539,15 @@
         except:
             results_df = pl.DataFrame()
         progress_bar = Progress(*Progress.get_default_columns(), MofNCompleteColumn())
         with progress_bar as p:
             for i, r in enumerate(
                 p.track(
                     self.party_search_queue.rows(named=True),
-                    description="Party searching...",
+                    description="Party searching…",
                 )
             ):
                 if r["Retrieved"] in ("", None):
                     if verbose:
                         p.console.log(f"#{i+1}: {r['TEMP_NAME']}")
                     self.party_search(
                         name=r["TEMP_NAME"],
@@ -981,15 +981,48 @@
         county_select.send_keys(county)
         division_select.send_keys(division)
         case_year_select.send_keys(case_year)
         case_number_input.send_keys(six_digit)
         case_extension_select.select_by_visible_text(extension)
         search_button = self.driver.find_element(by=By.ID, value="searchButton")
         search_button.click()
-        WebDriverWait(self.driver, 20).until(EC.staleness_of(search_button))
+        try:
+            WebDriverWait(self.driver, 20).until(EC.staleness_of(search_button))
+        except:
+            print("The search button never went stale. Trying to login again and restart. (991)")
+            self.login(log=False)
+            self.driver.get("https://v2.alacourt.com/frmcaselookupform.aspx")
+            county_select = self.driver.find_element(
+                by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCounty"
+            )
+            division_select = self.driver.find_element(
+                by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlDivision"
+            )
+            case_year_select = self.driver.find_element(
+                by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCaseYear"
+            )
+            case_number_input = self.driver.find_element(
+                by=By.NAME, value="ctl00$ContentPlaceHolder1$txtCaseNumber"
+            )
+            case_extension_select = Select(
+                self.driver.find_element(
+                    by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlExt"
+                )
+            )
+            number_of_cases_select = self.driver.find_element(
+                by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlNumberOfCases"
+            )
+            county_select.send_keys(county)
+            division_select.send_keys(division)
+            case_year_select.send_keys(case_year)
+            case_number_input.send_keys(six_digit)
+            case_extension_select.select_by_visible_text(extension)
+            search_button = self.driver.find_element(by=By.ID, value="searchButton")
+            search_button.click()
+            WebDriverWait(self.driver, 10).until(EC.staleness_of(search_button))
         if download:
             if "NoCaseDetails" in self.driver.current_url:
                 return False
             else:
                 try:
                     WebDriverWait(self.driver, 10).until(
                         EC.visibility_of_element_located(
@@ -1006,14 +1039,17 @@
                 )
                 self.driver.find_element(by=By.ID, value="btnPrintCase").click()
                 return True
 
     def start_case_number_queue(
         self, queue=None, verbose=False, verify=True, pre_verify=False
     ):
+        """
+        From a table with 'Case Number' or 'CaseNumber' column, download cases to `AlacourtDriver.dirpath`. 
+        """
         if pre_verify:
             if isinstance(queue, pl.DataFrame) or isinstance(queue, str):
                 self.set_case_number_queue(queue)
             elif self.case_number_queue == None:
                 raise Exception("Must set case number queue to start.")
             self.verify_downloads()
         loop = True
@@ -1025,21 +1061,26 @@
             progress_bar = Progress(
                 *Progress.get_default_columns(), MofNCompleteColumn()
             )
             with progress_bar as p:
                 for i, r in enumerate(
                     p.track(
                         self.case_number_queue.rows(named=True),
-                        description="Fetching cases...",
+                        description="Fetching cases…",
                     )
                 ):
                     if r["Retrieved"] in ("", None):
                         if verbose:
                             p.console.log(f"#{i+1}: {r['CaseNumber']}")
-                        if self.case_number_search(r["CaseNumber"]):
+                        try:
+                            success = self.case_number_search(r["CaseNumber"])
+                        except:
+                            self.reconnect()
+                            success = self.case_number_search(r["CaseNumber"])
+                        if success:
                             self.case_number_queue[i, "Retrieved"] = "Y"
                             self.case_number_queue[i, "Timestamp"] = time.time()
                             self.case_number_queue[i, "Destination"] = self.dirpath
                         else:
                             self.case_number_queue[i, "Retrieved"] = "PDF Not Available"
                             self.case_number_queue[i, "Timestamp"] = time.time()
                         if self.case_number_queue_path != None and i % 10 == 0:
@@ -1057,22 +1098,43 @@
                     pl.col("Retrieved").is_null() | pl.col("Retrieved").eq("")
                 ).shape[0]
                 if remaining == 0:
                     loop = False
             else:
                 loop = False
 
+    def reconnect(self, wait=20, max_attempt=10):
+        """
+        Attempt to reconnect to Alacourt after `wait` seconds, up to `max_attempt` times before raising an exception.
+        """
+        successfully_reconnected = False
+        i = 0
+        while not successfully_reconnected:
+            try:
+                successfully_reconnected = self.login()
+            except:
+                i += 1
+                if i == max_attempt:
+                    break
+                with console.status(f"Connection error. Waiting {wait} seconds to attempt to reconnect…"):
+                    time.sleep(wait)
+        if not successfully_reconnected:
+            raise Exception(f"Failed to reconnect to Alacourt after {max_attempt} attempts.")
+
     def verify_downloads(self, queue=None):
+        """
+        Read case numbers from all cases in `dirpath`, and correct `queue_path` to accurately reflect progress.
+        """
         if isinstance(queue, pl.DataFrame) or isinstance(queue, str):
             self.set_case_number_queue(queue)
         elif not isinstance(self.case_number_queue, pl.DataFrame):
             raise Exception("Must set case number queue to verify.")
         if self.dirpath == None:
             raise Exception("Must set download directory to verify.")
-        with console.status("Verifying downloads..."):
+        with console.status("Verifying downloads…"):
             time.sleep(3)
             pdfs = glob.glob(self.dirpath + "**/*.pdf", recursive=True)
             case_numbers = []
             for pdf in pdfs:
                 doc = fitz.open(pdf)
                 text = " \n ".join(
                     x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks")
@@ -1118,15 +1180,15 @@
 class ADOCDriver:
     def __init__(self, output_path=None, headless=True):
         if output_path != None:
             self.output = os.path.abspath(output_path)
         opt = webdriver.ChromeOptions()
         if headless:
             opt.add_argument("--headless=new")
-        with console.status("Starting WebDriver (requires Google Chrome)..."):
+        with console.status("Starting WebDriver (requires Google Chrome)…"):
             self.driver = webdriver.Chrome(options=opt)
         self.driver.get("https://doc.alabama.gov/inmatesearch")
 
     def crawl(self, output_path=None) -> pl.DataFrame:
         """
         Collect all results in ADOC Inmate Search by searching last name by letter.
         """
@@ -1159,15 +1221,15 @@
             "X",
             "Y",
             "Z",
         ]
         results = pl.DataFrame()
         progress_bar = Progress(*Progress.get_default_columns(), MofNCompleteColumn())
         with progress_bar as p:
-            for letter in p.track(alphabet, description="Crawling ADOC..."):
+            for letter in p.track(alphabet, description="Crawling ADOC…"):
                 self.driver.get("https://doc.alabama.gov/inmatesearch")
                 self.driver.find_element(
                     by=By.ID, value="MainContent_txtLName"
                 ).send_keys(letter)
                 self.driver.find_element(
                     by=By.ID, value="MainContent_btnSearch"
                 ).click()
@@ -1529,15 +1591,15 @@
         except:
             inmate_details = pl.DataFrame()
             blue_tables = pl.DataFrame()
             black_tables = pl.DataFrame()
         progress_bar = Progress(*Progress.get_default_columns(), MofNCompleteColumn())
         with progress_bar as p:
             for i, r in enumerate(
-                p.track(self.queue.rows(named=True), description="Searching ADOC...")
+                p.track(self.queue.rows(named=True), description="Searching ADOC…")
             ):
                 if r["Retrieved"] in (None, ""):
                     if verbose:
                         p.console.log(
                             f"#{i+1}: {r['TEMP_AIS']} {r['TEMP_FIRST_NAME']} {r['TEMP_LAST_NAME']}"
                         )
                     self.search(
@@ -1618,25 +1680,31 @@
         self._attorneys = None
         self._images = None
         self._restitution = None
         self._linked_cases = None
         self._continuances = None
 
     def read(self):
+        """
+        Read input into pl.DataFrame. If directory, reads PDFs into archive df. 
+        """
         self.archive = read(self.archive)
         self.is_read = True
         return self.archive
 
     def cases(self):
+        """
+        Make case information table.
+        """
         if isinstance(self._cases, pl.DataFrame):
             return self._cases
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing cases table..."):
+            with console.status("Parsing cases table…"):
                 cases = self.archive.with_columns(
                     [
                         pl.col("AllPagesText")
                         .str.extract(
                             r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
                             group_index=1,
                         )
@@ -2482,20 +2550,23 @@
                     "ContinuanceDescription",
                     "NumberOfPreviousContinuances",
                 )
             self._cases = cases
             return self._cases
 
     def fees(self):
+        """
+        Make fee sheets table.
+        """
         if isinstance(self._fees, pl.DataFrame):
             return self._fees
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing fee sheets..."):
+            with console.status("Parsing fee sheets…"):
                 df = self.archive.select("CaseNumber", "AllPagesText")
                 df = df.select(
                     [
                         pl.col("CaseNumber"),
                         pl.col("AllPagesText")
                         .str.extract(r"(?s)Fee Sheet (.+Total:[^\n]+)")
                         .str.replace(
@@ -2771,14 +2842,17 @@
                     "AmountHold",
                 )
                 df = df.filter(pl.col("Balance").is_null().is_not())
             self._fees = df
             return self._fees
 
     def filing_charges(self, log=True):
+        """
+        Make filing charges table.
+        """
         def make_fc(archive):
             df = archive.select("CaseNumber", "AllPagesText")
             df = df.select(
                 [
                     pl.col("CaseNumber"),
                     pl.col("AllPagesText")
                     .str.extract(r"(?s)Filing Charges(.+?)Disposition Charges")
@@ -2997,27 +3071,30 @@
 
         if isinstance(self._filing_charges, pl.DataFrame):
             return self._filing_charges
         else:
             if not self.is_read:
                 self.read()
             if log:
-                with console.status("Parsing filing charges..."):
+                with console.status("Parsing filing charges…"):
                     self._filing_charges = make_fc(self.archive)
             else:
                 self._filing_charges = make_fc(self.archive)
             return self._filing_charges
 
     def disposition_charges(self):
+        """
+        Make disposition charges table.
+        """
         if isinstance(self._disposition_charges, pl.DataFrame):
             return self._disposition_charges
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing disposition charges..."):
+            with console.status("Parsing disposition charges…"):
                 df = self.archive.select("AllPagesText", "CaseNumber")
                 df = df.select(
                     [
                         pl.col("CaseNumber"),
                         pl.col("AllPagesText")
                         .str.extract(
                             r"(?s)Disposition Charges (.+?) (Sentences|Enforcement)"
@@ -3306,20 +3383,23 @@
                         ]
                     ).alias("ChargesSummary")
                 )
             self._disposition_charges = df
             return self._disposition_charges
 
     def sentences(self):
+        """
+        Make sentences table.
+        """
         if isinstance(self._sentences, pl.DataFrame):
             return self._sentences
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing sentences..."):
+            with console.status("Parsing sentences…"):
                 sent = self.archive.select(
                     [
                         pl.col("CaseNumber"),
                         pl.col("AllPagesTextNoNewLine")
                         .str.extract_all(r"Sentence\s\d+\s.+?(Linked Cases)")
                         .alias("Sentence"),
                     ]
@@ -3696,20 +3776,23 @@
                 )
                 sent = sent.drop_nulls("Number")
                 sent = sent.fill_null("")
             self._sentences = sent
             return self._sentences
 
     def settings(self):
+        """
+        Make settings table.
+        """
         if isinstance(self._settings, pl.DataFrame):
             return self._settings
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing settings..."):
+            with console.status("Parsing settings…"):
                 df = self.archive.select(
                     [
                         pl.col("CaseNumber"),
                         pl.col("AllPagesText")
                         .str.extract(
                             r"Description\:\s*\n\s*(?s)Settings(.+?)Court Action"
                         )
@@ -3748,20 +3831,23 @@
                         .alias("Description"),
                     ]
                 )
             self._settings = df
             return self._settings
 
     def case_action_summary(self):
+        """
+        Make case action summary table.
+        """
         if isinstance(self._case_action_summary, pl.DataFrame):
             return self._case_action_summary
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing case action summaries..."):
+            with console.status("Parsing case action summaries…"):
                 df = self.archive.select("AllPagesText", "CaseNumber")
                 df = df.select(
                     pl.col("CaseNumber"),
                     pl.col("AllPagesText")
                     .str.extract(r"(?s)Case Action Summary(.+) Date")
                     .str.replace(r"\s*\n\s*Operator\s*", "")
                     .alias("CAS"),
@@ -3815,20 +3901,23 @@
                     ]
                 )
                 df = df.filter(pl.col("Description").is_null().is_not())
             self._case_action_summary = df
             return self._case_action_summary
 
     def financial_history(self):
+        """
+        Make financial history table.
+        """
         if isinstance(self._financial_history, pl.DataFrame):
             return self._financial_history
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing financial history..."):
+            with console.status("Parsing financial history…"):
                 df = self.archive.select("CaseNumber", "AllPagesText")
                 df = df.select(
                     pl.col("CaseNumber"),
                     pl.col("AllPagesText")
                     .str.extract(r"(?s)Financial History(.+)Requesting Party")
                     .str.replace(
                         r"(\s*\n\s*Description From Party To Party Admin Fee\s*)", ""
@@ -3909,20 +3998,23 @@
                     ]
                 )
                 df = df.drop_nulls("Operator")
             self._financial_history = df
             return self._financial_history
 
     def witnesses(self):
+        """
+        Make witnesses table.
+        """
         if isinstance(self._witnesses, pl.DataFrame):
             return self._witnesses
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing witnesses tables..."):
+            with console.status("Parsing witnesses tables…"):
                 df = self.archive.select(
                     pl.col("CaseNumber"),
                     pl.col("AllPagesText")
                     .str.extract(
                         r"(?s)SJIS Witness List\s*\n\s*Date Issued\s*\n\s*Subpoena(.+?)Date"
                     )
                     .str.replace(r"..Alacourt\.com \d\d?/\d\d?/\d\d\d\d \d+", "")
@@ -3995,20 +4087,23 @@
                     "DateServed",
                     "ServiceType",
                 )
             self._witnesses = df
             return self._witnesses
 
     def attorneys(self):
+        """
+        Make attorneys table.
+        """
         if isinstance(self._attorneys, pl.DataFrame):
             return self._attorneys
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing attorneys tables..."):
+            with console.status("Parsing attorneys tables…"):
                 df = self.archive.select(
                     [
                         pl.col("CaseNumber"),
                         pl.col("AllPagesText")
                         .str.extract(r"(?s)Attorney Code\s*\n\s*(.+?)Warrant")
                         .alias("Attorneys"),
                     ]
@@ -4058,20 +4153,23 @@
                         .alias("Phone"),
                     ]
                 )
             self._attorneys = df
             return self._attorneys
 
     def images(self):
+        """
+        Make images table.
+        """
         if isinstance(self._images, pl.DataFrame):
             return self._images
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing images tables..."):
+            with console.status("Parsing images tables…"):
                 df = self.archive.with_columns(
                     [
                         pl.col("AllPagesText")
                         .str.extract(r"(?s)Images(.+)END OF THE REPORT")
                         .str.replace(r"\n Pages\s*", "")
                         .alias("Images")
                     ]
@@ -4116,20 +4214,23 @@
                     ]
                 )
                 df = df.drop_nulls("Date")
             self._images = df
             return self._images
 
     def restitution(self):
+        """
+        Make restitution table.
+        """
         if isinstance(self._restitution, pl.DataFrame):
             return self._restitution
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing restitution tables..."):
+            with console.status("Parsing restitution tables…"):
                 df = self.archive.select("CaseNumber", "AllPagesText")
                 df = df.select(
                     [
                         pl.col("CaseNumber"),
                         pl.col("AllPagesText")
                         .str.extract_all(r"(?s)Restitution (.+?) (Programs|Split)")
                         .alias("Restitution"),
@@ -4173,20 +4274,23 @@
                         .alias("Recipient"),
                     ]
                 )
             self._restitution = df
             return self._restitution
 
     def linked_cases(self):
+        """
+        Make linked cases table.
+        """
         if isinstance(self._linked_cases, pl.DataFrame):
             return self._linked_cases
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing linked cases tables..."):
+            with console.status("Parsing linked cases tables…"):
                 df = self.archive.select("CaseNumber", "AllPagesText")
                 df = df.select(
                     [
                         pl.col("CaseNumber"),
                         pl.col("AllPagesText")
                         .str.extract_all(
                             r"(?s)Linked Cases\s*\n\s*Sentencing Number Case Type Case Type Description CaseNumber(.+?)Enforcement|Sentence"
@@ -4235,20 +4339,23 @@
                     ]
                 )
                 df = df.drop_nulls("LinkedCaseNumber")
             self._linked_cases = df
             return self._linked_cases
 
     def continuances(self):
+        """
+        Make continuances table.
+        """
         if isinstance(self._continuances, pl.DataFrame):
             return self._continuances
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing continuances tables..."):
+            with console.status("Parsing continuances tables…"):
                 df = self.archive.select(
                     [
                         pl.col("CaseNumber"),
                         pl.col("AllPagesText")
                         .str.extract(
                             r"(?s)Continuances.+?Comments\s*\n(.+?)\s*\n\s*Court Action"
                         )
@@ -4286,14 +4393,17 @@
                     ]
                 )
                 df = df.filter(pl.col("Code").is_null().is_not())
             self._continuances = df
             return self._continuances
 
     def tables(self):
+        """
+        Make all tables and return dict.
+        """
         return {
             "cases": self.cases(),
             "filing-charges": self.filing_charges(),
             "disposition-charges": self.disposition_charges(),
             "fees": self.fees(),
             "sentences": self.sentences(),
             "financial-history": self.financial_history(),
@@ -4303,27 +4413,30 @@
             "case-action-summary": self.case_action_summary(),
             "restitution": self.restitution(),
             "linked-cases": self.linked_cases(),
             "continuances": self.continuances(),
         }
 
     def summary(self, pairs):
+        """
+        Summarize charges and fees by impact on voting rights using a filled pairs template. 
+        """
         if isinstance(pairs, str):
             self._pairs = read(pairs)
         if "Search" in self._pairs.columns:
             self._pairs = self._pairs.select(
                 [pl.col("Name"), pl.col("Search").alias("AIS / Unique ID")]
             )
             self._pairs = self._pairs.unique()
         if not self.is_read:
             self.read()
         cases = self.cases()
         dch = self.disposition_charges()
         fch = self.filing_charges()
-        with console.status("Creating summary..."):
+        with console.status("Creating summary…"):
             cases = cases.select("CaseNumber", "Name", "DOB", "Race", "Sex")
             cases = cases.with_columns(
                 [
                     pl.col("Race").cast(pl.Utf8, strict=False),
                     pl.col("Sex").cast(pl.Utf8, strict=False),
                 ]
             )
@@ -4491,17 +4604,20 @@
                 ]
             )
             cases = cases.sort("Name")
         self._summary = cases
         return self._summary
 
     def pairs_template(self):
+        """
+        Create empty pairs template for summary() pairs parameter.
+        """
         if not self.is_read:
             self.read()
-        with console.status("Creating template..."):
+        with console.status("Creating template…"):
             names = self.archive.with_columns(
                 [
                     pl.col("AllPagesText")
                     .str.extract(
                         r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
                         group_index=1,
                     )
@@ -4540,14 +4656,17 @@
             )
             names = names.sort("Name")
             names = names.filter(pl.col("Name") != "")
         self._pairs_template = names
         return self._pairs_template
 
     def write_tables(self, path):
+        """
+        Write all made tables to output path. If multiple tables, file extension must be .xlsx or .xls. Otherwise, .csv, .parquet, and .json are also supported.
+        """
         all_tables = {
             "cases": self._cases,
             "filing-charges": self._filing_charges,
             "disposition-charges": self._disposition_charges,
             "fees": self._fees,
             "sentences": self._sentences,
             "financial-history": self._financial_history,
@@ -4563,14 +4682,17 @@
         for x in all_tables:
             if isinstance(all_tables[x], pl.dataframe.frame.DataFrame):
                 only_df_vars.update({x: all_tables[x]})
         write(only_df_vars, path, log=True)
         return only_df_vars
 
     def write_archive(self, path):
+        """
+        Write case archive to output path. Supports .xls, .xlsx, .parquet, and .csv. Parquet export recommended.
+        """
         if not self.is_read:
             self.read()
         cols = [
             col
             for col in ["CaseNumber", "Path", "Timestamp", "AllPagesText"]
             if col in self.archive.columns
         ]
@@ -4753,15 +4875,15 @@
         bool,
         typer.Option(
             "--verbose", help="Print detailed logs while working.", show_default=False
         ),
     ] = False,
 ):
     """
-    From a queue table with `CaseNumber` column, download case detail PDFs to directory at `output_path`.
+    From a queue table with 'Case Number' or 'CaseNumber' column, download case detail PDFs to directory at `output_path`.
     """
     queue_path = os.path.abspath(queue_path)
     output_path = os.path.abspath(output_path)
     headless = not show_browser
 
     if os.path.splitext(queue_path)[1] not in (
         ".xls",
@@ -5021,15 +5143,15 @@
     """
     Rename all cases in a directory to full case number. Duplicates will be removed.
     """
     input_directory = os.path.abspath(input_directory)
     pdfs = glob.glob(input_directory + "**/*.pdf", recursive=True)
     progress_bar = Progress(*Progress.get_default_columns(), MofNCompleteColumn())
     with progress_bar as p:
-        for pdf in p.track(pdfs, description="Renaming PDFs..."):
+        for pdf in p.track(pdfs, description="Renaming PDFs…"):
             doc = fitz.open(pdf)
             text = " \n ".join(
                 x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks")
             )
             cnum = (
                 re.search(r"County: (\d\d)", str(text)).group(1)
                 + "-"
@@ -5053,14 +5175,15 @@
 ):
     pass
 
 
 if __name__ == "__main__":
     app()
 
+
 ## GETTERS
 
 
 def getName(text):
     try:
         return (
             re.sub(
```

### Comparing `alacorder-81.1.3/pyproject.toml` & `alacorder-81.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "81.1.3"
+version = "81.1.4"
 description = "Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
```

### Comparing `alacorder-81.1.3/PKG-INFO` & `alacorder-81.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 81.1.3
+Version: 81.1.4
 Summary: Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes.
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

