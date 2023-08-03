# Comparing `tmp/aa_structures-2.4.2.tar.gz` & `tmp/aa_structures-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_structures-2.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_structures-2.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_structures-2.4.2.tar` & `aa_structures-2.5.0.tar`

### file list

```diff
@@ -1,172 +1,186 @@
--rw-r--r--   0        0        0     1070 2023-07-27 19:21:52.362421 aa_structures-2.4.2/LICENSE
--rw-r--r--   0        0        0     4406 2023-07-27 19:21:52.362421 aa_structures-2.4.2/README.md
--rw-r--r--   0        0        0     2113 2023-07-27 19:21:52.366421 aa_structures-2.4.2/pyproject.toml
--rw-r--r--   0        0        0      170 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/__init__.py
--rw-r--r--   0        0        0    36110 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/admin.py
--rw-r--r--   0        0        0     6228 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/app_settings.py
--rw-r--r--   0        0        0      195 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/apps.py
--rw-r--r--   0        0        0      915 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/auth_hooks.py
--rw-r--r--   0        0        0      741 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/constants.py
--rw-r--r--   0        0        0        0 2023-07-27 19:48:00.999760 aa_structures-2.4.2/structures/core/__init__.py
--rw-r--r--   0        0        0    71519 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/core/notification_embeds.py
--rw-r--r--   0        0        0    16436 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/core/notification_timers.py
--rw-r--r--   0        0        0    19834 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/core/serializers.py
--rw-r--r--   0        0        0      623 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/core/sovereignty.py
--rw-r--r--   0        0        0     1613 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/core/starbases.py
--rw-r--r--   0        0        0      382 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/forms.py
--rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/helpers/__init__.py
--rw-r--r--   0        0        0      830 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/helpers/general.py
--rw-r--r--   0        0        0    13634 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    61204 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/django.pot
--rw-r--r--   0        0        0      380 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47274 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5784 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    55691 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47267 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47024 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ko/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      538 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47437 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47505 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11588 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    58962 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/management/commands/__init__.py
--rw-r--r--   0        0        0     1443 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/management/commands/structures_load_eve.py
--rw-r--r--   0        0        0     2398 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/management/commands/structures_preload_eveuniverse.py
--rw-r--r--   0        0        0    18114 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/managers.py
--rw-r--r--   0        0        0    59315 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     2274 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/migrations/0002_remove_eveuniverse_relation_names.py
--rw-r--r--   0        0        0    44042 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/migrations/0003_add_localization_and_unique_key.py
--rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/migrations/__init__.py
--rw-r--r--   0        0        0      505 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/models/__init__.py
--rw-r--r--   0        0        0     2073 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/models/eveuniverse.py
--rw-r--r--   0        0        0    42745 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/models/notifications.py
--rw-r--r--   0        0        0    53967 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/models/owners.py
--rw-r--r--   0        0        0    37256 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/models/structures.py
--rw-r--r--   0        0        0      274 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/providers.py
--rw-r--r--   0        0        0     1165 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/css/global.css
--rw-r--r--   0        0        0     1186 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/css/main.css
--rw-r--r--   0        0        0    43262 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0      908 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/eve_symbol_128.png
--rw-r--r--   0        0        0      805 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/0h.png
--rw-r--r--   0        0        0      805 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/0l.png
--rw-r--r--   0        0        0      805 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/0m.png
--rw-r--r--   0        0        0      805 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/0r.png
--rw-r--r--   0        0        0      805 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/0s.png
--rw-r--r--   0        0        0     2590 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/1h.png
--rw-r--r--   0        0        0     1976 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/1l.png
--rw-r--r--   0        0        0     2025 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/1m.png
--rw-r--r--   0        0        0     2512 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/1r.png
--rw-r--r--   0        0        0     3541 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/2h.png
--rw-r--r--   0        0        0     2570 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/2l.png
--rw-r--r--   0        0        0     2766 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/2m.png
--rw-r--r--   0        0        0     3497 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/2r.png
--rw-r--r--   0        0        0     4607 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/3h.png
--rw-r--r--   0        0        0     3523 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/3l.png
--rw-r--r--   0        0        0     3720 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/3m.png
--rw-r--r--   0        0        0     4886 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/3r.png
--rw-r--r--   0        0        0     5309 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/4h.png
--rw-r--r--   0        0        0     4628 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/4l.png
--rw-r--r--   0        0        0     4956 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/4m.png
--rw-r--r--   0        0        0     9490 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/4s.png
--rw-r--r--   0        0        0     6109 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/5h.png
--rw-r--r--   0        0        0     5888 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/5l.png
--rw-r--r--   0        0        0     6270 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/5m.png
--rw-r--r--   0        0        0     7399 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/5s.png
--rw-r--r--   0        0        0     7203 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/6h.png
--rw-r--r--   0        0        0     7014 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/6l.png
--rw-r--r--   0        0        0     7439 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/6m.png
--rw-r--r--   0        0        0     8288 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/7h.png
--rw-r--r--   0        0        0     8067 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/7l.png
--rw-r--r--   0        0        0     8580 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/7m.png
--rw-r--r--   0        0        0     9276 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/8h.png
--rw-r--r--   0        0        0     8972 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/8l.png
--rw-r--r--   0        0        0     9541 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/8m.png
--rw-r--r--   0        0        0      195 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/blank.png
--rw-r--r--   0        0        0    16840 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/circle.png
--rw-r--r--   0        0        0    33523 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/dustwheel.png
--rw-r--r--   0        0        0     1480 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/h.png
--rw-r--r--   0        0        0     1480 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/l.png
--rw-r--r--   0        0        0     1480 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/m.png
--rw-r--r--   0        0        0     8879 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/noship.png
--rw-r--r--   0        0        0     1480 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/r.png
--rw-r--r--   0        0        0    43642 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis.png
--rw-r--r--   0        0        0    43560 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_blue.png
--rw-r--r--   0        0        0    42833 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_darkred.png
--rw-r--r--   0        0        0    38343 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_default.png
--rw-r--r--   0        0        0    42868 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_revelations.png
--rw-r--r--   0        0        0      496 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/structures_logo.png
--rw-r--r--   0        0        0     8806 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/tasks.py
--rw-r--r--   0        0        0      298 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/base.html
--rw-r--r--   0        0        0    21200 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/main.html
--rw-r--r--   0        0        0      264 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/fitting_assets.html
--rw-r--r--   0        0        0     9530 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/fitting_gfx.html
--rw-r--r--   0        0        0     2705 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/poco_details.html
--rw-r--r--   0        0        0     4133 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/starbase_detail.html
--rw-r--r--   0        0        0     4070 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/structure_details.html
--rw-r--r--   0        0        0      998 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/tab_general_detail.html
--rw-r--r--   0        0        0     1501 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/partials/jump_gates_list.html
--rw-r--r--   0        0        0     1034 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/partials/poco_list.html
--rw-r--r--   0        0        0     5947 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/partials/structure_list.html
--rw-r--r--   0        0        0     1586 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/partials/structure_summary.html
--rw-r--r--   0        0        0      117 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/templatetags/detail_title.html
--rw-r--r--   0        0        0      375 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/templatetags/list_asset.html
--rw-r--r--   0        0        0      706 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/templatetags/list_item.html
--rw-r--r--   0        0        0      505 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/templatetags/list_tax_item.html
--rw-r--r--   0        0        0       68 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/templates/structures/templatetags/list_title.html
--rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/templatetags/__init__.py
--rw-r--r--   0        0        0     1601 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/templatetags/structures.py
--rw-r--r--   0        0        0       75 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/tests/core/__init__.py
--rw-r--r--   0        0        0    13532 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_notification_embeds.py
--rw-r--r--   0        0        0    10435 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_notification_structuretimers.py
--rw-r--r--   0        0        0     5515 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_notifications_timerboard.py
--rw-r--r--   0        0        0     3385 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_serializers.py
--rw-r--r--   0        0        0      825 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_sovereignty.py
--rw-r--r--   0        0        0     3163 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_starbases.py
--rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/tests/models/__init__.py
--rw-r--r--   0        0        0     1600 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_eveuniverse.py
--rw-r--r--   0        0        0    39346 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_notifications_1.py
--rw-r--r--   0        0        0    31553 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_notifications_2.py
--rw-r--r--   0        0        0     6004 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_notifications_3.py
--rw-r--r--   0        0        0     5318 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_notifications_discord.py
--rw-r--r--   0        0        0    26807 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_owners_1.py
--rw-r--r--   0        0        0    54158 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_owners_2.py
--rw-r--r--   0        0        0    37407 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_owners_3.py
--rw-r--r--   0        0        0    37744 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_structures.py
--rw-r--r--   0        0        0    21127 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_admin.py
--rw-r--r--   0        0        0     1861 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_helpers.py
--rw-r--r--   0        0        0    23524 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_integration.py
--rw-r--r--   0        0        0    27217 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_managers_1.py
--rw-r--r--   0        0        0     1567 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_managers_3.py
--rw-r--r--   0        0        0    18409 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_tasks.py
--rw-r--r--   0        0        0    36695 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_views.py
--rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/tests/testdata/__init__.py
--rw-r--r--   0        0        0     2601 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0    33188 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/entities.json
--rw-r--r--   0        0        0    13864 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/esi_data.json
--rw-r--r--   0        0        0   979813 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0     7827 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/factories.py
--rw-r--r--   0        0        0    10857 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/factories_2.py
--rw-r--r--   0        0        0     5746 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/generate_notifications.py
--rw-r--r--   0        0        0     1415 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/generate_notifications_2.py
--rw-r--r--   0        0        0     6238 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/generate_structures.py
--rw-r--r--   0        0        0    26820 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/helpers.py
--rw-r--r--   0        0        0      395 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0      963 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/tasks_loadtest.py
--rw-r--r--   0        0        0      414 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/test_generate_structures.py
--rw-r--r--   0        0        0     1057 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/urls.py
--rw-r--r--   0        0        0    21820 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/views.py
--rw-r--r--   0        0        0        0 2023-07-27 19:48:01.011759 aa_structures-2.4.2/structures/webhooks/__init__.py
--rw-r--r--   0        0        0     6587 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/webhooks/core.py
--rw-r--r--   0        0        0     1036 2023-07-27 19:21:52.390420 aa_structures-2.4.2/structures/webhooks/managers.py
--rw-r--r--   0        0        0     1641 2023-07-27 19:21:52.390420 aa_structures-2.4.2/structures/webhooks/models.py
--rw-r--r--   0        0        0        0 2023-07-27 19:48:01.011759 aa_structures-2.4.2/structures/webhooks/tests/__init__.py
--rw-r--r--   0        0        0     6395 2023-07-27 19:21:52.390420 aa_structures-2.4.2/structures/webhooks/tests/test_core.py
--rw-r--r--   0        0        0      459 2023-07-27 19:21:52.390420 aa_structures-2.4.2/structures/webhooks/tests/test_utils.py
--rw-r--r--   0        0        0     5929 1970-01-01 00:00:00.000000 aa_structures-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2020-10-22 17:29:44.465193 aa_structures-2.5.0/LICENSE
+-rw-r--r--   0        0        0     4406 2022-08-11 17:23:18.759898 aa_structures-2.5.0/README.md
+-rw-r--r--   0        0        0     2351 2023-08-01 12:33:06.795354 aa_structures-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-08-03 11:53:41.382294 aa_structures-2.5.0/structures/__init__.py
+-rw-r--r--   0        0        0    36334 2023-07-28 16:06:53.286038 aa_structures-2.5.0/structures/admin.py
+-rw-r--r--   0        0        0     6267 2023-07-28 01:22:06.039331 aa_structures-2.5.0/structures/app_settings.py
+-rw-r--r--   0        0        0      195 2023-07-27 19:27:24.171062 aa_structures-2.5.0/structures/apps.py
+-rw-r--r--   0        0        0      915 2022-03-01 14:58:19.767220 aa_structures-2.5.0/structures/auth_hooks.py
+-rw-r--r--   0        0        0      926 2023-07-28 01:22:06.039331 aa_structures-2.5.0/structures/constants.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:34:32.920442 aa_structures-2.5.0/structures/core/__init__.py
+-rw-r--r--   0        0        0      131 2023-07-28 01:22:06.039331 aa_structures-2.5.0/structures/core/notification_embeds/__init__.py
+-rw-r--r--   0        0        0     3742 2023-07-28 22:31:18.461156 aa_structures-2.5.0/structures/core/notification_embeds/billing_embeds.py
+-rw-r--r--   0        0        0     5607 2023-07-28 01:22:06.039331 aa_structures-2.5.0/structures/core/notification_embeds/character_embeds.py
+-rw-r--r--   0        0        0     2974 2023-08-01 13:22:15.295910 aa_structures-2.5.0/structures/core/notification_embeds/helpers.py
+-rw-r--r--   0        0        0    13488 2023-08-01 19:24:52.669709 aa_structures-2.5.0/structures/core/notification_embeds/main.py
+-rw-r--r--   0        0        0     7307 2023-07-28 22:31:18.461156 aa_structures-2.5.0/structures/core/notification_embeds/moonmining_embeds.py
+-rw-r--r--   0        0        0     2919 2023-07-28 22:31:18.465156 aa_structures-2.5.0/structures/core/notification_embeds/orbital_embeds.py
+-rw-r--r--   0        0        0     9128 2023-07-28 22:31:18.465156 aa_structures-2.5.0/structures/core/notification_embeds/sov_embeds.py
+-rw-r--r--   0        0        0    13201 2023-07-28 22:31:18.465156 aa_structures-2.5.0/structures/core/notification_embeds/structures_embeds.py
+-rw-r--r--   0        0        0     5741 2023-08-01 12:33:06.799354 aa_structures-2.5.0/structures/core/notification_embeds/tower_embeds.py
+-rw-r--r--   0        0        0     9208 2023-07-28 01:22:06.043331 aa_structures-2.5.0/structures/core/notification_embeds/war_embeds.py
+-rw-r--r--   0        0        0    15134 2023-07-28 22:31:18.465156 aa_structures-2.5.0/structures/core/notification_timers.py
+-rw-r--r--   0        0        0    11199 2023-08-01 17:39:30.150287 aa_structures-2.5.0/structures/core/notification_types.py
+-rw-r--r--   0        0        0    20065 2023-07-28 22:31:18.465156 aa_structures-2.5.0/structures/core/serializers.py
+-rw-r--r--   0        0        0      730 2023-07-28 01:22:06.043331 aa_structures-2.5.0/structures/core/sovereignty.py
+-rw-r--r--   0        0        0     1757 2023-07-28 01:22:06.043331 aa_structures-2.5.0/structures/core/starbases.py
+-rw-r--r--   0        0        0      392 2023-07-28 01:22:06.043331 aa_structures-2.5.0/structures/forms.py
+-rw-r--r--   0        0        0     1027 2023-08-01 19:24:52.669709 aa_structures-2.5.0/structures/helpers.py
+-rw-r--r--   0        0        0    13634 2020-10-22 17:29:44.473193 aa_structures-2.5.0/structures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    61204 2023-05-21 12:33:18.416466 aa_structures-2.5.0/structures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-05-21 12:33:18.416466 aa_structures-2.5.0/structures/locale/django.pot
+-rw-r--r--   0        0        0      380 2020-10-22 17:29:44.473193 aa_structures-2.5.0/structures/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47274 2023-05-21 12:33:18.416466 aa_structures-2.5.0/structures/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5784 2020-10-22 17:29:44.473193 aa_structures-2.5.0/structures/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    55691 2023-05-21 12:33:18.420466 aa_structures-2.5.0/structures/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-05-21 12:33:18.420466 aa_structures-2.5.0/structures/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-05-21 12:33:18.420466 aa_structures-2.5.0/structures/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47267 2023-05-21 12:33:18.424466 aa_structures-2.5.0/structures/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2020-10-22 17:29:44.473193 aa_structures-2.5.0/structures/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47024 2023-04-17 00:48:58.414803 aa_structures-2.5.0/structures/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-05-21 12:33:18.424466 aa_structures-2.5.0/structures/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      538 2020-10-22 17:29:44.473193 aa_structures-2.5.0/structures/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47437 2023-05-21 12:33:18.424466 aa_structures-2.5.0/structures/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47505 2023-05-21 12:33:18.428466 aa_structures-2.5.0/structures/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11588 2020-10-22 17:29:44.473193 aa_structures-2.5.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    58962 2023-05-21 12:33:18.428466 aa_structures-2.5.0/structures/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-08-03 12:34:32.924442 aa_structures-2.5.0/structures/management/commands/__init__.py
+-rw-r--r--   0        0        0     1507 2023-07-28 01:22:06.047331 aa_structures-2.5.0/structures/management/commands/structures_load_eve.py
+-rw-r--r--   0        0        0     2489 2023-07-28 01:22:06.047331 aa_structures-2.5.0/structures/management/commands/structures_preload_eveuniverse.py
+-rw-r--r--   0        0        0    19003 2023-07-28 16:06:53.294037 aa_structures-2.5.0/structures/managers.py
+-rw-r--r--   0        0        0    59315 2023-04-17 14:02:22.882798 aa_structures-2.5.0/structures/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     2274 2023-04-16 22:10:32.169268 aa_structures-2.5.0/structures/migrations/0002_remove_eveuniverse_relation_names.py
+-rw-r--r--   0        0        0    44042 2023-04-17 00:48:58.414803 aa_structures-2.5.0/structures/migrations/0003_add_localization_and_unique_key.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:34:32.924442 aa_structures-2.5.0/structures/migrations/__init__.py
+-rw-r--r--   0        0        0      916 2023-07-28 16:06:53.294037 aa_structures-2.5.0/structures/models/__init__.py
+-rw-r--r--   0        0        0     2103 2023-07-28 22:31:18.465156 aa_structures-2.5.0/structures/models/eveuniverse.py
+-rw-r--r--   0        0        0    35035 2023-08-01 19:24:52.673709 aa_structures-2.5.0/structures/models/notifications.py
+-rw-r--r--   0        0        0    53380 2023-07-28 22:31:18.465156 aa_structures-2.5.0/structures/models/owners.py
+-rw-r--r--   0        0        0    29438 2023-08-01 19:24:52.673709 aa_structures-2.5.0/structures/models/structures_1.py
+-rw-r--r--   0        0        0     9469 2023-07-28 22:31:18.465156 aa_structures-2.5.0/structures/models/structures_2.py
+-rw-r--r--   0        0        0      317 2023-07-28 01:22:06.051331 aa_structures-2.5.0/structures/providers.py
+-rw-r--r--   0        0        0     1165 2022-05-30 21:05:57.989637 aa_structures-2.5.0/structures/static/structures/css/global.css
+-rw-r--r--   0        0        0     1186 2021-12-14 22:54:11.485089 aa_structures-2.5.0/structures/static/structures/css/main.css
+-rw-r--r--   0        0        0    43262 2021-04-29 22:23:58.269246 aa_structures-2.5.0/structures/static/structures/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2021-04-29 22:23:58.269246 aa_structures-2.5.0/structures/static/structures/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0      908 2021-04-29 22:23:58.269246 aa_structures-2.5.0/structures/static/structures/img/eve_symbol_128.png
+-rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.5.0/structures/static/structures/img/panel/0h.png
+-rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.5.0/structures/static/structures/img/panel/0l.png
+-rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.5.0/structures/static/structures/img/panel/0m.png
+-rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.5.0/structures/static/structures/img/panel/0r.png
+-rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.5.0/structures/static/structures/img/panel/0s.png
+-rw-r--r--   0        0        0     2590 2023-04-16 23:43:18.808312 aa_structures-2.5.0/structures/static/structures/img/panel/1h.png
+-rw-r--r--   0        0        0     1976 2023-04-16 23:43:18.808312 aa_structures-2.5.0/structures/static/structures/img/panel/1l.png
+-rw-r--r--   0        0        0     2025 2023-04-16 23:43:18.812312 aa_structures-2.5.0/structures/static/structures/img/panel/1m.png
+-rw-r--r--   0        0        0     2512 2023-04-16 23:43:18.812312 aa_structures-2.5.0/structures/static/structures/img/panel/1r.png
+-rw-r--r--   0        0        0     3541 2023-04-16 23:43:18.812312 aa_structures-2.5.0/structures/static/structures/img/panel/2h.png
+-rw-r--r--   0        0        0     2570 2023-04-16 23:43:18.812312 aa_structures-2.5.0/structures/static/structures/img/panel/2l.png
+-rw-r--r--   0        0        0     2766 2023-04-16 23:43:18.812312 aa_structures-2.5.0/structures/static/structures/img/panel/2m.png
+-rw-r--r--   0        0        0     3497 2023-04-16 23:43:18.812312 aa_structures-2.5.0/structures/static/structures/img/panel/2r.png
+-rw-r--r--   0        0        0     4607 2023-04-16 23:43:18.812312 aa_structures-2.5.0/structures/static/structures/img/panel/3h.png
+-rw-r--r--   0        0        0     3523 2023-04-16 23:43:18.812312 aa_structures-2.5.0/structures/static/structures/img/panel/3l.png
+-rw-r--r--   0        0        0     3720 2023-04-16 23:43:18.812312 aa_structures-2.5.0/structures/static/structures/img/panel/3m.png
+-rw-r--r--   0        0        0     4886 2023-04-16 23:43:18.812312 aa_structures-2.5.0/structures/static/structures/img/panel/3r.png
+-rw-r--r--   0        0        0     5309 2023-04-16 23:43:18.816312 aa_structures-2.5.0/structures/static/structures/img/panel/4h.png
+-rw-r--r--   0        0        0     4628 2023-04-16 23:43:18.816312 aa_structures-2.5.0/structures/static/structures/img/panel/4l.png
+-rw-r--r--   0        0        0     4956 2023-04-16 23:43:18.816312 aa_structures-2.5.0/structures/static/structures/img/panel/4m.png
+-rw-r--r--   0        0        0     9490 2023-04-16 23:43:18.816312 aa_structures-2.5.0/structures/static/structures/img/panel/4s.png
+-rw-r--r--   0        0        0     6109 2023-04-16 23:43:18.816312 aa_structures-2.5.0/structures/static/structures/img/panel/5h.png
+-rw-r--r--   0        0        0     5888 2023-04-16 23:43:18.816312 aa_structures-2.5.0/structures/static/structures/img/panel/5l.png
+-rw-r--r--   0        0        0     6270 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/5m.png
+-rw-r--r--   0        0        0     7399 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/5s.png
+-rw-r--r--   0        0        0     7203 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/6h.png
+-rw-r--r--   0        0        0     7014 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/6l.png
+-rw-r--r--   0        0        0     7439 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/6m.png
+-rw-r--r--   0        0        0     8288 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/7h.png
+-rw-r--r--   0        0        0     8067 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/7l.png
+-rw-r--r--   0        0        0     8580 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/7m.png
+-rw-r--r--   0        0        0     9276 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/8h.png
+-rw-r--r--   0        0        0     8972 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/8l.png
+-rw-r--r--   0        0        0     9541 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/8m.png
+-rw-r--r--   0        0        0      195 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/blank.png
+-rw-r--r--   0        0        0    16840 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/circle.png
+-rw-r--r--   0        0        0    33523 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/dustwheel.png
+-rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/h.png
+-rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/l.png
+-rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/m.png
+-rw-r--r--   0        0        0     8879 2023-04-16 23:43:18.820312 aa_structures-2.5.0/structures/static/structures/img/panel/noship.png
+-rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.824312 aa_structures-2.5.0/structures/static/structures/img/panel/r.png
+-rw-r--r--   0        0        0    43642 2023-04-16 23:43:18.824312 aa_structures-2.5.0/structures/static/structures/img/panel/tyrannis.png
+-rw-r--r--   0        0        0    43560 2023-04-16 23:43:18.824312 aa_structures-2.5.0/structures/static/structures/img/panel/tyrannis_blue.png
+-rw-r--r--   0        0        0    42833 2023-04-16 23:43:18.824312 aa_structures-2.5.0/structures/static/structures/img/panel/tyrannis_darkred.png
+-rw-r--r--   0        0        0    38343 2023-04-16 23:43:18.824312 aa_structures-2.5.0/structures/static/structures/img/panel/tyrannis_default.png
+-rw-r--r--   0        0        0    42868 2023-04-16 23:43:18.824312 aa_structures-2.5.0/structures/static/structures/img/panel/tyrannis_revelations.png
+-rw-r--r--   0        0        0      496 2021-04-29 22:23:58.277247 aa_structures-2.5.0/structures/static/structures/img/structures_logo.png
+-rw-r--r--   0        0        0     9061 2023-07-28 16:06:53.298038 aa_structures-2.5.0/structures/tasks.py
+-rw-r--r--   0        0        0      298 2021-04-29 22:23:58.277247 aa_structures-2.5.0/structures/templates/structures/base.html
+-rw-r--r--   0        0        0    21200 2022-07-14 15:22:09.316257 aa_structures-2.5.0/structures/templates/structures/main.html
+-rw-r--r--   0        0        0      264 2022-06-01 20:12:19.043382 aa_structures-2.5.0/structures/templates/structures/modals/fitting_assets.html
+-rw-r--r--   0        0        0     9530 2023-04-16 23:43:18.824312 aa_structures-2.5.0/structures/templates/structures/modals/fitting_gfx.html
+-rw-r--r--   0        0        0     2705 2022-06-01 20:12:19.043382 aa_structures-2.5.0/structures/templates/structures/modals/poco_details.html
+-rw-r--r--   0        0        0     4133 2022-06-01 20:12:19.047382 aa_structures-2.5.0/structures/templates/structures/modals/starbase_detail.html
+-rw-r--r--   0        0        0     4070 2022-06-01 20:12:19.047382 aa_structures-2.5.0/structures/templates/structures/modals/structure_details.html
+-rw-r--r--   0        0        0      998 2022-06-01 20:12:19.047382 aa_structures-2.5.0/structures/templates/structures/modals/tab_general_detail.html
+-rw-r--r--   0        0        0     1501 2022-05-30 21:05:57.993637 aa_structures-2.5.0/structures/templates/structures/partials/jump_gates_list.html
+-rw-r--r--   0        0        0     1034 2021-05-22 14:22:35.353363 aa_structures-2.5.0/structures/templates/structures/partials/poco_list.html
+-rw-r--r--   0        0        0     5947 2022-05-30 21:05:57.993637 aa_structures-2.5.0/structures/templates/structures/partials/structure_list.html
+-rw-r--r--   0        0        0     1586 2023-04-16 22:10:32.185268 aa_structures-2.5.0/structures/templates/structures/partials/structure_summary.html
+-rw-r--r--   0        0        0      117 2022-05-31 14:09:14.519367 aa_structures-2.5.0/structures/templates/structures/templatetags/detail_title.html
+-rw-r--r--   0        0        0      375 2022-06-01 20:12:19.047382 aa_structures-2.5.0/structures/templates/structures/templatetags/list_asset.html
+-rw-r--r--   0        0        0      706 2022-06-01 15:59:29.634387 aa_structures-2.5.0/structures/templates/structures/templatetags/list_item.html
+-rw-r--r--   0        0        0      505 2023-04-16 22:10:32.185268 aa_structures-2.5.0/structures/templates/structures/templatetags/list_tax_item.html
+-rw-r--r--   0        0        0       68 2022-05-30 21:05:57.993637 aa_structures-2.5.0/structures/templates/structures/templatetags/list_title.html
+-rw-r--r--   0        0        0        0 2023-08-03 12:34:32.932442 aa_structures-2.5.0/structures/templatetags/__init__.py
+-rw-r--r--   0        0        0     1637 2023-07-28 01:22:06.051331 aa_structures-2.5.0/structures/templatetags/structures.py
+-rw-r--r--   0        0        0       75 2020-10-22 17:29:44.485193 aa_structures-2.5.0/structures/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:34:32.932442 aa_structures-2.5.0/structures/tests/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:34:32.932442 aa_structures-2.5.0/structures/tests/core/notification_embeds/__init__.py
+-rw-r--r--   0        0        0     1778 2023-08-01 13:22:15.295910 aa_structures-2.5.0/structures/tests/core/notification_embeds/test_helpers.py
+-rw-r--r--   0        0        0    13721 2023-08-01 12:33:06.799354 aa_structures-2.5.0/structures/tests/core/notification_embeds/test_main.py
+-rw-r--r--   0        0        0    10494 2023-07-28 22:31:18.469156 aa_structures-2.5.0/structures/tests/core/test_notification_structuretimers.py
+-rw-r--r--   0        0        0     9881 2023-07-28 16:06:53.302038 aa_structures-2.5.0/structures/tests/core/test_notification_types.py
+-rw-r--r--   0        0        0     5574 2023-07-28 22:31:18.469156 aa_structures-2.5.0/structures/tests/core/test_notifications_timerboard.py
+-rw-r--r--   0        0        0     3446 2023-07-28 22:31:18.469156 aa_structures-2.5.0/structures/tests/core/test_serializers.py
+-rw-r--r--   0        0        0      821 2023-07-28 01:22:06.051331 aa_structures-2.5.0/structures/tests/core/test_sovereignty.py
+-rw-r--r--   0        0        0     3186 2023-07-28 22:31:18.469156 aa_structures-2.5.0/structures/tests/core/test_starbases.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:34:32.932442 aa_structures-2.5.0/structures/tests/models/__init__.py
+-rw-r--r--   0        0        0     1623 2023-07-28 22:31:18.469156 aa_structures-2.5.0/structures/tests/models/test_eveuniverse.py
+-rw-r--r--   0        0        0    29798 2023-08-01 17:39:30.154287 aa_structures-2.5.0/structures/tests/models/test_notifications_1.py
+-rw-r--r--   0        0        0    36015 2023-08-01 17:39:30.154287 aa_structures-2.5.0/structures/tests/models/test_notifications_2.py
+-rw-r--r--   0        0        0     6081 2023-07-28 22:31:18.473156 aa_structures-2.5.0/structures/tests/models/test_notifications_3.py
+-rw-r--r--   0        0        0     5391 2023-07-28 22:31:18.473156 aa_structures-2.5.0/structures/tests/models/test_notifications_discord.py
+-rw-r--r--   0        0        0    26877 2023-07-28 22:31:18.473156 aa_structures-2.5.0/structures/tests/models/test_owners_1.py
+-rw-r--r--   0        0        0    54277 2023-07-28 22:31:18.473156 aa_structures-2.5.0/structures/tests/models/test_owners_2.py
+-rw-r--r--   0        0        0    37517 2023-07-28 22:31:18.477156 aa_structures-2.5.0/structures/tests/models/test_owners_3.py
+-rw-r--r--   0        0        0    37864 2023-07-28 22:31:18.477156 aa_structures-2.5.0/structures/tests/models/test_structures.py
+-rw-r--r--   0        0        0    21127 2023-04-25 14:58:07.639318 aa_structures-2.5.0/structures/tests/test_admin.py
+-rw-r--r--   0        0        0     2374 2023-08-01 19:24:52.673709 aa_structures-2.5.0/structures/tests/test_helpers.py
+-rw-r--r--   0        0        0    23588 2023-07-28 16:06:53.310037 aa_structures-2.5.0/structures/tests/test_integration.py
+-rw-r--r--   0        0        0    27287 2023-07-28 16:06:53.310037 aa_structures-2.5.0/structures/tests/test_managers_1.py
+-rw-r--r--   0        0        0     1623 2023-07-28 16:06:53.310037 aa_structures-2.5.0/structures/tests/test_managers_3.py
+-rw-r--r--   0        0        0    18512 2023-07-28 16:06:53.314037 aa_structures-2.5.0/structures/tests/test_tasks.py
+-rw-r--r--   0        0        0    36722 2023-07-28 22:31:18.477156 aa_structures-2.5.0/structures/tests/test_views.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:34:32.932442 aa_structures-2.5.0/structures/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     2610 2023-07-28 22:31:18.477156 aa_structures-2.5.0/structures/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    33188 2022-09-10 17:58:40.514747 aa_structures-2.5.0/structures/tests/testdata/entities.json
+-rw-r--r--   0        0        0    13864 2022-08-10 19:36:18.186258 aa_structures-2.5.0/structures/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0   979813 2022-09-10 17:58:40.522747 aa_structures-2.5.0/structures/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0     7843 2023-07-28 22:31:18.477156 aa_structures-2.5.0/structures/tests/testdata/factories.py
+-rw-r--r--   0        0        0    10907 2023-07-28 16:06:53.314037 aa_structures-2.5.0/structures/tests/testdata/factories_2.py
+-rw-r--r--   0        0        0     5746 2022-09-10 17:58:40.522747 aa_structures-2.5.0/structures/tests/testdata/generate_notifications.py
+-rw-r--r--   0        0        0     1415 2022-08-11 17:23:18.771898 aa_structures-2.5.0/structures/tests/testdata/generate_notifications_2.py
+-rw-r--r--   0        0        0     6238 2022-08-16 19:31:09.320517 aa_structures-2.5.0/structures/tests/testdata/generate_structures.py
+-rw-r--r--   0        0        0    26871 2023-07-28 16:06:53.318038 aa_structures-2.5.0/structures/tests/testdata/helpers.py
+-rw-r--r--   0        0        0      395 2022-08-10 15:32:14.940423 aa_structures-2.5.0/structures/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0      963 2021-03-24 18:47:30.630666 aa_structures-2.5.0/structures/tests/testdata/tasks_loadtest.py
+-rw-r--r--   0        0        0      414 2020-10-22 17:29:44.489193 aa_structures-2.5.0/structures/tests/testdata/test_generate_structures.py
+-rw-r--r--   0        0        0     1086 2023-07-28 01:22:06.055331 aa_structures-2.5.0/structures/urls.py
+-rw-r--r--   0        0        0    22302 2023-07-28 16:06:53.322038 aa_structures-2.5.0/structures/views.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:34:32.932442 aa_structures-2.5.0/structures/webhooks/__init__.py
+-rw-r--r--   0        0        0     6573 2023-08-01 12:33:06.799354 aa_structures-2.5.0/structures/webhooks/core.py
+-rw-r--r--   0        0        0     1117 2023-07-28 22:31:18.481156 aa_structures-2.5.0/structures/webhooks/managers.py
+-rw-r--r--   0        0        0     1790 2023-07-28 01:22:06.055331 aa_structures-2.5.0/structures/webhooks/models.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:34:32.932442 aa_structures-2.5.0/structures/webhooks/tests/__init__.py
+-rw-r--r--   0        0        0     6412 2023-07-28 16:06:53.326038 aa_structures-2.5.0/structures/webhooks/tests/test_core.py
+-rw-r--r--   0        0        0      459 2021-02-14 22:48:19.121024 aa_structures-2.5.0/structures/webhooks/tests/test_utils.py
+-rw-r--r--   0        0        0     5958 1970-01-01 00:00:00.000000 aa_structures-2.5.0/PKG-INFO
```

### Comparing `aa_structures-2.4.2/LICENSE` & `aa_structures-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/README.md` & `aa_structures-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/pyproject.toml` & `aa_structures-2.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "allianceauth>=3.0",
     "dhooks-lite>=1.0",
     "django-eveuniverse>=1.0",
     "django-multiselectfield",
     "django-navhelper",
     "pytz!=2022.2",
     "redis-simple-mq>=1.0",
+    "humanize>=4.7",
 ]
 
 [project.urls]
 Homepage = "https://gitlab.com/ErikKalkoken/aa-structures"
 Documentation = "https://aa-structures.readthedocs.io/en/latest/"
 Source = "https://gitlab.com/ErikKalkoken/aa-structures"
 Changelog = "https://gitlab.com/ErikKalkoken/aa-structures/-/blob/master/CHANGELOG.md"
@@ -57,18 +58,27 @@
     "FIRSTPARTY",
     "LOCALFOLDER",
 ]
 known_allianceauth = ["allianceauth", "app_utils"]
 known_django = ["django", "django_webtest", "esi", "eveuniverse"]
 
 [tool.pylint.'MASTER']
-ignore-patterns = ["__init__.py", "auth_hooks.py", "apps.py"]
+ignore-patterns = ["__init__.py", "auth_hooks.py", "apps.py", "admin.py"]
 ignore-paths = ["^.*/tests/.*$", "^.*/migrations/.*$"]
 
 [tool.pylint.'BASIC']
-good-names = ["i", "j", "k", "ex"]
+good-names = ["i", "j", "k", "x", "y", "z", "ex", "id"]
 
 [tool.pylint.'FORMAT']
 max-line-length = 120
 
 [tool.pylint.'MESSAGES CONTROL']
-disable = ["R0902", "R0903"]
+disable = [
+    "too-many-instance-attributes",
+    "too-few-public-methods",
+    "imported-auth-user",
+    "cyclic-import",
+    "fixme",
+    "import-outside-toplevel",
+    "redefined-builtin",
+    "no-member",
+]
```

### Comparing `aa_structures-2.4.2/structures/admin.py` & `aa_structures-2.5.0/structures/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Admin site for Structures."""
+
 import statistics
 from typing import Optional
 
 from django.conf import settings
 from django.contrib import admin
 from django.db import models
 from django.db.models import Prefetch
@@ -11,22 +13,22 @@
 
 from allianceauth.eveonline.models import EveAllianceInfo, EveCorporationInfo
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.django import admin_boolean_icon_html
 from app_utils.logging import LoggerAddTag
 
 from . import __title__, app_settings, tasks
+from .core.notification_types import NotificationType
 from .models import (
     FuelAlert,
     FuelAlertConfig,
     GeneratedNotification,
     JumpFuelAlert,
     JumpFuelAlertConfig,
     Notification,
-    NotificationType,
     Owner,
     OwnerCharacter,
     Structure,
     StructureItem,
     StructureService,
     StructureTag,
     Webhook,
@@ -176,18 +178,17 @@
             ("no", "No"),
         )
 
     def queryset(self, request, queryset):
         """Return the filtered queryset"""
         if self.value() == "yes":
             return queryset.annotate_can_be_rendered().filter(can_be_rendered_2=True)
-        elif self.value() == "no":
+        if self.value() == "no":
             return queryset.annotate_can_be_rendered().filter(can_be_rendered_2=False)
-        else:
-            return queryset
+        return queryset
 
 
 class NotificationBaseAdmin(admin.ModelAdmin):
     list_display = (
         "_notification_id",
         "timestamp",
         "owner",
@@ -269,24 +270,22 @@
     def _is_timer_added(self, obj):
         value = obj.is_timer_added if obj.can_have_timer else None
         return admin_boolean_icon_html(value)
 
     @admin.display(description=_("Mark selected notifications as sent"))
     def mark_as_sent(self, request, queryset):
         queryset.update(is_sent=True)
-        self.message_user(
-            request, "{} notifications marked as sent".format(queryset.count())
-        )
+        notif_count = queryset.count()
+        self.message_user(request, f"{notif_count} notifications marked as sent")
 
     @admin.display(description=_("Mark selected notifications as unsent"))
     def mark_as_unsent(self, request, queryset):
         queryset.update(is_sent=False)
-        self.message_user(
-            request, "{} notifications marked as unsent".format(queryset.count())
-        )
+        notif_count = queryset.count()
+        self.message_user(request, f"{notif_count} notifications marked as unsent")
 
     @admin.display(description=_("Send selected notifications to configured webhooks"))
     def send_to_configured_webhooks(self, request, queryset):
         notifs_queued = 0
         for obj in queryset:
             if obj.can_be_rendered and obj.relevant_webhooks().exists():
                 if obj.send_to_configured_webhooks():
@@ -470,17 +469,20 @@
         queryset.update(is_active=False)
         self.message_user(request, f"Deactivated {queryset.count()} owners")
 
     @admin.display(description=_("Update all from EVE server for selected owners"))
     def update_all(self, request, queryset):
         for obj in queryset:
             tasks.update_all_for_owner.delay(obj.pk, user_pk=request.user.pk)  # type: ignore
-            text = _(
-                "Started updating structures and notifications for %s. "
-                "You will receive a notification once it is completed." % obj
+            text = (
+                _(
+                    "Started updating structures and notifications for %s. "
+                    "You will receive a notification once it is completed."
+                )
+                % obj
             )
             self.message_user(request, text)
 
     @admin.display(
         description=_("Update structures from EVE server for selected owners")
     )
     def update_structures(self, request, queryset):
@@ -629,18 +631,18 @@
         "is_default",
         "style",
         "is_user_managed",
     )
     readonly_fields = ("is_user_managed",)
 
     def has_delete_permission(self, request, obj: Optional[StructureTag] = None):
-        return False if obj and not obj.is_user_managed else True
+        return not (obj and not obj.is_user_managed)
 
     def has_change_permission(self, request, obj: Optional[StructureTag] = None):
-        return False if obj and not obj.is_user_managed else True
+        return not (obj and not obj.is_user_managed)
 
 
 class StructureServiceAdminInline(admin.TabularInline):
     model = StructureService
 
     def has_add_permission(self, request, obj=None):
         return False
@@ -674,21 +676,21 @@
     def lookups(self, request, model_admin):
         qs = (
             EveCorporationInfo.objects.filter(structure_owner__isnull=False)
             .values("corporation_id", "corporation_name")
             .distinct()
             .order_by(Lower("corporation_name"))
         )
-        return tuple([(x["corporation_id"], x["corporation_name"]) for x in qs])
+        return tuple(((obj["corporation_id"], obj["corporation_name"]) for obj in qs))
 
     def queryset(self, request, queryset):
         if self.value() is None:
             return queryset.all()
-        else:
-            return queryset.filter(owner__corporation__corporation_id=self.value())
+
+        return queryset.filter(owner__corporation__corporation_id=self.value())
 
 
 class OwnerAllianceFilter(admin.SimpleListFilter):
     """Custom filter to filter on alliances from owners only"""
 
     title = "owner alliance"
     parameter_name = "owner_alliance_id__exact"
@@ -698,23 +700,21 @@
             EveAllianceInfo.objects.filter(
                 evecorporationinfo__structure_owner__isnull=False
             )
             .values("alliance_id", "alliance_name")
             .distinct()
             .order_by(Lower("alliance_name"))
         )
-        return tuple([(x["alliance_id"], x["alliance_name"]) for x in qs])
+        return tuple(((obj["alliance_id"], obj["alliance_name"]) for obj in qs))
 
     def queryset(self, request, queryset):
         if self.value() is None:
             return queryset.all()
-        else:
-            return queryset.filter(
-                owner__corporation__alliance__alliance_id=self.value()
-            )
+
+        return queryset.filter(owner__corporation__alliance__alliance_id=self.value())
 
 
 class HasWebhooksListFilter(admin.SimpleListFilter):
     title = "has webhooks"
     parameter_name = "has_webhooks"
 
     def lookups(self, request, model_admin):
@@ -724,14 +724,15 @@
         )
 
     def queryset(self, request, queryset):
         if self.value() == "y":
             return queryset.filter(webhooks__isnull=False)
         if self.value() == "n":
             return queryset.filter(webhooks__isnull=True)
+        return None
 
 
 @admin.register(Structure)
 class StructureAdmin(admin.ModelAdmin):
     show_full_result_count = True
     list_select_related = (
         "owner",
@@ -773,19 +774,19 @@
         ("eve_type__eve_group", admin.RelatedOnlyFieldListFilter),
         ("eve_type__eve_group__eve_category", admin.RelatedOnlyFieldListFilter),
         ("tags", admin.RelatedOnlyFieldListFilter),
         HasWebhooksListFilter,
     )
     actions = ("add_default_tags", "remove_user_tags", "update_generated_tags")
     readonly_fields = tuple(
-        [
+        (
             x.name
             for x in Structure._meta.get_fields()
             if isinstance(x, models.fields.Field) and x.name not in ["tags", "webhooks"]
-        ]
+        )
     )
     fieldsets = (
         (
             None,
             {
                 "fields": (
                     "name",
@@ -899,42 +900,41 @@
     def add_default_tags(self, request, queryset):
         structure_count = 0
         tags = StructureTag.objects.filter(is_default=True)
         for structure in queryset:
             for tag in tags:
                 structure.tags.add(tag)
             structure_count += 1
+        tags_count = tags.count()
         self.message_user(
             request,
-            "Added {:,} default tags to {:,} structures".format(
-                tags.count(), structure_count
-            ),
+            f"Added {tags_count:,} default tags to {structure_count:,} structures",
         )
 
     @admin.display(description=_("Remove user tags for selected structures"))
     def remove_user_tags(self, request, queryset):
         structure_count = 0
         for structure in queryset:
             for tag in structure.tags.filter(is_user_managed=True):
                 structure.tags.remove(tag)
             structure_count += 1
         self.message_user(
             request,
-            "Removed all user tags from {:,} structures".format(structure_count),
+            f"Removed all user tags from {structure_count:,} structures",
         )
 
     @admin.display(description=_("Update generated tags for selected structures"))
     def update_generated_tags(self, request, queryset):
         structure_count = 0
         for structure in queryset:
             structure.update_generated_tags(recreate_tags=True)
             structure_count += 1
         self.message_user(
             request,
-            "Updated all generated tags for {:,} structures".format(structure_count),
+            f"Updated all generated tags for {structure_count:,} structures",
         )
 
     def formfield_for_manytomany(self, db_field, request, **kwargs):
         """only show custom tags in dropdown"""
         if db_field.name == "tags":
             kwargs["queryset"] = StructureTag.objects.filter(is_user_managed=True)
 
@@ -990,15 +990,15 @@
         ),
     )
 
     def get_form(self, *args, **kwargs):
         form = super().get_form(*args, **kwargs)
         form.base_fields[
             "notification_types"
-        ].choices = NotificationType.choices_enabled
+        ].choices = NotificationType.choices_enabled()
         return form
 
     def get_queryset(self, request):
         qs = super().get_queryset(request)
         return qs.prefetch_related(
             "ping_groups",
             "owners",
@@ -1047,48 +1047,54 @@
     def test_notification(self, request, queryset):
         for obj in queryset:
             tasks.send_test_notifications_to_webhook.delay(
                 obj.pk, user_pk=request.user.pk
             )  # type: ignore
             self.message_user(
                 request,
-                'Initiated sending test notification to webhook "{}". '
-                "You will receive a report on completion.".format(obj),
+                _(
+                    "Initiated sending test notification to webhook %s. "
+                    "You will receive a report on completion."
+                )
+                % obj,
             )
 
     @admin.display(description=_("Activate selected webhook"))
     def activate(self, request, queryset):
         for obj in queryset:
             obj.is_active = True
             obj.save()
-            self.message_user(request, f'You have activated webhook "{obj}"')
+            self.message_user(request, _("You have activated webhook %s") % obj)
 
     @admin.display(description=_("Deactivate selected webhook"))
     def deactivate(self, request, queryset):
         for obj in queryset:
             obj.is_active = False
             obj.save()
-            self.message_user(request, f'You have de-activated webhook "{obj}"')
+            self.message_user(request, _("You have de-activated webhook %s") % obj)
 
     @admin.display(description=_("Purge queued messages from selected webhooks"))
     def purge_messages(self, request, queryset):
         actions_count = 0
         killmails_deleted = 0
         for webhook in queryset:
             killmails_deleted += webhook.clear_queue()
             actions_count += 1
         self.message_user(
             request,
-            f"Purged queued messages for {actions_count} webhooks, "
-            f"deleting a total of {killmails_deleted} messages.",
+            _(
+                "Purged queued messages for %(actions_count)s webhooks, "
+                "deleting a total of %(killmails_deleted)s messages."
+            )
+            % {"actions_count": actions_count, "killmails_deleted": killmails_deleted},
         )
 
     @admin.display(description=_("Send queued messages from selected webhooks"))
     def send_messages(self, request, queryset):
         items_count = 0
         for webhook in queryset:
             tasks.send_messages_for_webhook.delay(webhook.pk)  # type: ignore
             items_count += 1
 
         self.message_user(
-            request, f"Started sending queued messages for {items_count} webhooks."
+            request, _("Started sending queued messages for %d webhooks.") % items_count
         )
```

### Comparing `aa_structures-2.4.2/structures/app_settings.py` & `aa_structures-2.5.0/structures/app_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from app_utils.django import clean_setting
+"""Settings for Structures."""
+
+from app_utils.app_settings import clean_setting
 
 # Whether to automatically add timers for certain notifications
 # on the timerboard (will have no effect if aa-timerboard app is not installed)
 STRUCTURES_ADD_TIMERS = clean_setting("STRUCTURES_ADD_TIMERS", True)
 
 # whether admins will get notifications about import events like
 # when someone adds a structure owner
@@ -153,8 +155,10 @@
     "STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS", True
 )
 
 
 STRUCTURES_ESI_DIRECTOR_ERROR_MAX_RETRIES = clean_setting(
     "STRUCTURES_ESI_DIRECTOR_ERROR_MAX_RETRIES", 3
 )
-"""Max retries before a character is deleted when ESI claims the character is not a director (Since this sometimes is reported wrongly by ESI)."""
+"""Max retries before a character is deleted when ESI claims the character
+is not a director (Since this sometimes is reported wrongly by ESI).
+"""
```

### Comparing `aa_structures-2.4.2/structures/auth_hooks.py` & `aa_structures-2.5.0/structures/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/constants.py` & `aa_structures-2.5.0/structures/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,52 @@
+"""Constants for Structures."""
+
 from enum import IntEnum
 
 
 # Eve enums
 class EveAttributeId(IntEnum):
+    """An EVE attribute ID."""
+
     SQUADRON_SIZE = 2215
 
 
 class EveCategoryId(IntEnum):
+    """An EVE category ID."""
+
     ORBITAL = 46
     STARBASE = 23
     STRUCTURE = 65
 
 
 class EveGroupId(IntEnum):
+    """An EVE group ID."""
+
     CITADEL = 1657
     CONTROL_TOWER = 365
     ENGINEERING_COMPLEX = 1404
     FUEL_BLOCK = 1136
     ICE_PRODUCT = 423
     REFINERY = 1406
     PLANET = 7
     STRUCTURE_CITADEL_SERVICE_MODULE = 1321
     UNCOMMON_MOON_ASTEROIDS = 1921
     QUANTUM_CORES = 4086
 
 
 class EveTypeId(IntEnum):
+    """An EVE type ID."""
+
     CALDARI_CONTROL_TOWER = 16213
     CUSTOMS_OFFICE = 2233
     IHUB = 32458
     JUMP_GATE = 35841
     LIQUID_OZONE = 16273
     NITROGEN_FUEL_BLOCK = 4051
     STRONTIUM = 16275
     TCU = 32226
 
 
 class EveCorporationId(IntEnum):
+    """An EVE corporation ID."""
+
     DED = 1000137
```

### Comparing `aa_structures-2.4.2/structures/core/notification_timers.py` & `aa_structures-2.5.0/structures/core/notification_timers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,94 +1,98 @@
 """Creating or removing timers from notifications."""
 
+# pylint: disable = ungrouped-imports
+
 import datetime as dt
 
 from django.utils.translation import gettext
-from eveuniverse.models import EveMoon, EvePlanet, EveSolarSystem, EveType
+from eveuniverse.models import EveType
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.datetime import (
     DATETIME_FORMAT,
     ldap_time_2_datetime,
     ldap_timedelta_2_timedelta,
 )
 from app_utils.django import app_labels
 from app_utils.logging import LoggerAddTag
 
-from .. import __title__
-from ..app_settings import (
+from structures import __title__
+from structures.app_settings import (
     STRUCTURES_MOON_EXTRACTION_TIMERS_ENABLED,
     STRUCTURES_TIMERS_ARE_CORP_RESTRICTED,
 )
-from ..constants import EveTypeId
-from ..models import Notification, NotificationType, Structure
+from structures.constants import EveTypeId
+from structures.models import Notification, Structure
+
 from . import sovereignty, starbases
+from .notification_types import NotificationType
 
 if "timerboard" in app_labels():
     from allianceauth.timerboard.models import Timer as AuthTimer
 
-    has_auth_timers = True
+    HAS_AUTH_TIMERS = True
 else:
-    has_auth_timers = False
+    HAS_AUTH_TIMERS = False
 
 if "structuretimers" in app_labels():
     from structuretimers.models import Timer
 
-    has_structure_timers = True
+    HAS_STRUCTURE_TIMERS = True
 else:
-    has_structure_timers = False
+    HAS_STRUCTURE_TIMERS = False
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 def add_or_remove_timer(notif: Notification) -> bool:
     """Add/remove a timer related to this notification for some types.
 
     Returns True when timers where added or removed, else False
     """
-    parsed_text = notif.parsed_text()
     if notif.notif_type in [
         NotificationType.STRUCTURE_LOST_ARMOR,
         NotificationType.STRUCTURE_LOST_SHIELD,
     ]:
-        timer_processed = _gen_timer_structure_reinforcement(notif, parsed_text)
+        timer_processed = _gen_timer_structure_reinforcement(notif)
     elif notif.notif_type == NotificationType.SOV_STRUCTURE_REINFORCED:
-        timer_processed = _gen_timer_sov_reinforcements(notif, parsed_text)
+        timer_processed = _gen_timer_sov_reinforcements(notif)
     elif notif.notif_type == NotificationType.ORBITAL_REINFORCED:
-        timer_processed = _gen_timer_orbital_reinforcements(notif, parsed_text)
+        timer_processed = _gen_timer_orbital_reinforcements(notif)
     elif notif.notif_type in [
         NotificationType.MOONMINING_EXTRACTION_STARTED,
         NotificationType.MOONMINING_EXTRACTION_CANCELLED,
     ]:
         if not STRUCTURES_MOON_EXTRACTION_TIMERS_ENABLED:
             timer_processed = None
         else:
-            timer_processed = _gen_timer_moon_extraction(notif, parsed_text)
+            timer_processed = _gen_timer_moon_extraction(notif)
     elif notif.notif_type == NotificationType.TOWER_REINFORCED_EXTRA:
-        timer_processed = _gen_timer_tower_reinforcements(notif, parsed_text)
+        timer_processed = _gen_timer_tower_reinforcements(notif)
     else:
         raise NotImplementedError(
             f"Unsupported notification type for timers: {notif.notif_type}"
         )
     if timer_processed:
         logger.info("%s: Created timer for notification", notif.notification_id)
         notif.is_timer_added = True
         notif.save()
     return timer_processed
 
 
-def _gen_timer_structure_reinforcement(notif: Notification, parsed_text: str) -> bool:
+def _gen_timer_structure_reinforcement(notif: Notification) -> bool:
     """Generate timer for structure reinforcements"""
     token = notif.owner.fetch_token()
+    parsed_text = notif.parsed_text()
     structure_obj, _ = Structure.objects.get_or_create_esi(
         id=parsed_text["structureID"], token=token
     )
     eve_time = notif.timestamp + ldap_timedelta_2_timedelta(parsed_text["timeLeft"])
     timer_processed = False
-    if has_auth_timers:
+    if HAS_AUTH_TIMERS:
         details_map = {
             NotificationType.STRUCTURE_LOST_SHIELD: gettext("Armor timer"),
             NotificationType.STRUCTURE_LOST_ARMOR: gettext("Final timer"),
         }
         AuthTimer.objects.create(
             details=details_map.get(notif.notif_type, ""),
             system=structure_obj.eve_solar_system.name,
@@ -97,15 +101,15 @@
             objective="Friendly",
             eve_time=eve_time,
             eve_corp=notif.owner.corporation,
             corp_timer=STRUCTURES_TIMERS_ARE_CORP_RESTRICTED,
         )
         timer_processed = True
 
-    if has_structure_timers:
+    if HAS_STRUCTURE_TIMERS:
         timer_map = {
             NotificationType.STRUCTURE_LOST_SHIELD: Timer.Type.ARMOR,
             NotificationType.STRUCTURE_LOST_ARMOR: Timer.Type.HULL,
         }
         visibility = (
             Timer.Visibility.CORPORATION
             if STRUCTURES_TIMERS_ARE_CORP_RESTRICTED
@@ -125,54 +129,51 @@
             details_notes=_timer_details_notes(notif),
         )
         timer_processed = True
 
     return timer_processed
 
 
-def _gen_timer_sov_reinforcements(notif: Notification, parsed_text: str) -> bool:
+def _gen_timer_sov_reinforcements(notif: Notification) -> bool:
     """Generate timer for sov reinforcements."""
     if not notif.owner.is_alliance_main:
         return False
 
-    solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
-        id=parsed_text["solarSystemID"]
-    )
-    structure_type_name = sovereignty.structure_type_name_from_event_type(
+    parsed_text = notif.parsed_text()
+    solar_system = notif.eve_solar_system()
+    structure_type_name = sovereignty.event_type_to_structure_type_name(
         parsed_text["campaignEventType"]
     )
     eve_time = ldap_time_2_datetime(parsed_text["decloakTime"])
     timer_processed = False
-    if has_auth_timers:
+
+    if HAS_AUTH_TIMERS:
         AuthTimer.objects.create(
             details=gettext("Sov timer"),
             system=solar_system.name,
             planet_moon="",
             structure=structure_type_name,
             objective="Friendly",
             eve_time=eve_time,
             eve_corp=notif.owner.corporation,
             corp_timer=STRUCTURES_TIMERS_ARE_CORP_RESTRICTED,
         )
         timer_processed = True
 
-    if has_structure_timers:
-        eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
-            id=parsed_text["solarSystemID"]
-        )
+    if HAS_STRUCTURE_TIMERS:
         structure_type, _ = EveType.objects.get_or_create_esi(
-            id=sovereignty.type_id_from_event_type(parsed_text["campaignEventType"])
+            id=sovereignty.event_type_to_type_id(parsed_text["campaignEventType"])
         )
         visibility = (
             Timer.Visibility.CORPORATION
             if STRUCTURES_TIMERS_ARE_CORP_RESTRICTED
             else Timer.Visibility.UNRESTRICTED
         )
         Timer.objects.create(
-            eve_solar_system=eve_solar_system,
+            eve_solar_system=solar_system,
             structure_type=structure_type,
             timer_type=Timer.Type.FINAL,
             objective=Timer.Objective.FRIENDLY,
             date=eve_time,
             eve_corporation=notif.owner.corporation,
             eve_alliance=notif.owner.corporation.alliance,
             visibility=visibility,
@@ -180,49 +181,47 @@
             details_notes=_timer_details_notes(notif),
         )
         timer_processed = True
 
     return timer_processed
 
 
-def _gen_timer_orbital_reinforcements(notif: Notification, parsed_text: str) -> bool:
+def _gen_timer_orbital_reinforcements(notif: Notification) -> bool:
     """Generate timer for orbital reinforcements."""
-    solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
-        id=parsed_text["solarSystemID"]
-    )
-    planet, _ = EvePlanet.objects.get_or_create_esi(id=parsed_text["planetID"])
+
+    solar_system = notif.eve_solar_system()
+    planet = notif.eve_planet()
+    parsed_text = notif.parsed_text()
     eve_time = ldap_time_2_datetime(parsed_text["reinforceExitTime"])
     timer_processed = False
-    if has_auth_timers:
+
+    if HAS_AUTH_TIMERS:
         AuthTimer.objects.create(
             details=gettext("Final timer"),
             system=solar_system.name,
             planet_moon=planet.name,
             structure="POCO",
             objective="Friendly",
             eve_time=eve_time,
             eve_corp=notif.owner.corporation,
             corp_timer=STRUCTURES_TIMERS_ARE_CORP_RESTRICTED,
         )
         timer_processed = True
 
-    if has_structure_timers:
-        eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
-            id=parsed_text["solarSystemID"]
-        )
+    if HAS_STRUCTURE_TIMERS:
         structure_type, _ = EveType.objects.get_or_create_esi(
             id=EveTypeId.CUSTOMS_OFFICE
         )
         visibility = (
             Timer.Visibility.CORPORATION
             if STRUCTURES_TIMERS_ARE_CORP_RESTRICTED
             else Timer.Visibility.UNRESTRICTED
         )
         Timer.objects.create(
-            eve_solar_system=eve_solar_system,
+            eve_solar_system=solar_system,
             structure_type=structure_type,
             timer_type=Timer.Type.FINAL,
             objective=Timer.Objective.FRIENDLY,
             date=eve_time,
             location_details=planet.name,
             eve_corporation=notif.owner.corporation,
             eve_alliance=notif.owner.corporation.alliance,
@@ -232,146 +231,137 @@
             details_notes=_timer_details_notes(notif),
         )
         timer_processed = True
 
     return timer_processed
 
 
-def _gen_timer_moon_extraction(notif: Notification, parsed_text: str) -> bool:
+def _gen_timer_moon_extraction(notif: Notification) -> bool:
     """Generate timer for moon mining extractions."""
-    solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
-        id=parsed_text["solarSystemID"]
-    )
-    moon, _ = EveMoon.objects.get_or_create_esi(id=parsed_text["moonID"])
-    if "readyTime" in parsed_text:
-        eve_time = ldap_time_2_datetime(parsed_text["readyTime"])
-    else:
-        eve_time = None
-    details = gettext("Extraction ready")
-    system = solar_system.name
-    planet_moon = moon.name
+    solar_system = notif.eve_solar_system()
+    moon = notif.eve_moon()
+    parsed_text = notif.parsed_text()
+    eve_time = _extract_eve_time(parsed_text)
+
     structure_type_name = "Moon Mining Cycle"
     objective = "Friendly"
     timer_processed = False
-
-    if has_structure_timers:
-        eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
-            id=parsed_text["solarSystemID"]
-        )
-        structure_type, _ = EveType.objects.get_or_create_esi(
-            id=parsed_text["structureTypeID"]
-        )
-        visibility = (
-            Timer.Visibility.CORPORATION
-            if STRUCTURES_TIMERS_ARE_CORP_RESTRICTED
-            else Timer.Visibility.UNRESTRICTED
-        )
-    else:
-        eve_solar_system = None
-        structure_type = None
-        visibility = None
+    structure_type = notif.eve_structure_type()
 
     if notif.notif_type == NotificationType.MOONMINING_EXTRACTION_STARTED:
-        if has_auth_timers:
+        if HAS_AUTH_TIMERS:
             AuthTimer.objects.create(
-                details=details,
-                system=system,
-                planet_moon=planet_moon,
+                details=gettext("Extraction ready"),
+                system=solar_system.name,
+                planet_moon=moon.name,
                 structure=structure_type_name,
                 objective=objective,
                 eve_time=eve_time,
                 eve_corp=notif.owner.corporation,
                 corp_timer=STRUCTURES_TIMERS_ARE_CORP_RESTRICTED,
             )
             timer_processed = True
 
-        if has_structure_timers:
-            eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
-                id=parsed_text["solarSystemID"]
-            )
-            structure_type, _ = EveType.objects.get_or_create_esi(
-                id=parsed_text["structureTypeID"]
-            )
-            visibility = (
-                Timer.Visibility.CORPORATION
-                if STRUCTURES_TIMERS_ARE_CORP_RESTRICTED
-                else Timer.Visibility.UNRESTRICTED
-            )
+        if HAS_STRUCTURE_TIMERS:
             Timer.objects.create(
-                eve_solar_system=eve_solar_system,
+                eve_solar_system=solar_system,
                 structure_type=structure_type,
                 timer_type=Timer.Type.MOONMINING,
                 objective=Timer.Objective.FRIENDLY,
                 date=eve_time,
                 location_details=moon.name,
                 eve_corporation=notif.owner.corporation,
                 eve_alliance=notif.owner.corporation.alliance,
-                visibility=visibility,
+                visibility=_calc_visibility(),
                 structure_name=parsed_text["structureName"],
                 owner_name=notif.owner.corporation.corporation_name,
                 details_notes=_timer_details_notes(notif),
             )
             timer_processed = True
 
     elif notif.notif_type == NotificationType.MOONMINING_EXTRACTION_CANCELLED:
         timer_processed = True
-        notifications_qs = Notification.objects.filter(
+
+        for notification in Notification.objects.filter(
             notif_type=NotificationType.MOONMINING_EXTRACTION_STARTED,
             owner=notif.owner,
             is_timer_added=True,
             timestamp__lte=notif.timestamp,
-        ).order_by("-timestamp")
-        for notification in notifications_qs:
+        ).order_by("-timestamp"):
+            notification: Notification
             parsed_text_2 = notification.parsed_text()
             my_structure_type_id = parsed_text_2["structureTypeID"]
             if my_structure_type_id == parsed_text["structureTypeID"]:
-                eve_time = ldap_time_2_datetime(parsed_text_2["readyTime"])
-                if has_auth_timers:
+                eve_time_2 = _extract_eve_time(parsed_text_2)
+
+                if HAS_AUTH_TIMERS:
                     timer_query = AuthTimer.objects.filter(
-                        system=system,
-                        planet_moon=planet_moon,
+                        system=solar_system.name,
+                        planet_moon=moon.name,
                         structure=structure_type_name,
                         objective=objective,
-                        eve_time=eve_time,
+                        eve_time=eve_time_2,
                     )
                     deleted_count, _ = timer_query.delete()
                     logger.info(
-                        f"{notif.notification_id}: removed {deleted_count} "
-                        "obsolete Auth timers related to notification"
+                        "%s: removed %d obsolete Auth timers related to notification",
+                        notif.notification_id,
+                        deleted_count,
                     )
 
-                if has_structure_timers:
+                if HAS_STRUCTURE_TIMERS:
                     timer_query = Timer.objects.filter(
-                        eve_solar_system=eve_solar_system,
+                        eve_solar_system=solar_system,
                         structure_type=structure_type,
                         timer_type=Timer.Type.MOONMINING,
                         location_details=moon.name,
-                        date=eve_time,
+                        date=eve_time_2,
                         objective=Timer.Objective.FRIENDLY,
                         eve_corporation=notif.owner.corporation,
                         eve_alliance=notif.owner.corporation.alliance,
-                        visibility=visibility,
+                        visibility=_calc_visibility(),
                         structure_name=parsed_text["structureName"],
                         owner_name=notif.owner.corporation.corporation_name,
                     )
                     deleted_count, _ = timer_query.delete()
                     logger.info(
-                        f"{notif.notification_id}: removed {deleted_count} "
-                        "obsolete structure timers related to notification"
+                        "%s: removed %d obsolete structure timers "
+                        "related to notification",
+                        notif.notification_id,
+                        deleted_count,
                     )
 
     return timer_processed
 
 
-def _gen_timer_tower_reinforcements(notif: Notification, parsed_text: str) -> bool:
+def _calc_visibility():
+    if HAS_STRUCTURE_TIMERS:
+        return (
+            Timer.Visibility.CORPORATION
+            if STRUCTURES_TIMERS_ARE_CORP_RESTRICTED
+            else Timer.Visibility.UNRESTRICTED
+        )
+    return None
+
+
+def _extract_eve_time(parsed_text):
+    if "readyTime" in parsed_text:
+        return ldap_time_2_datetime(parsed_text["readyTime"])
+    return None
+
+
+def _gen_timer_tower_reinforcements(notif: Notification) -> bool:
     """Generate timer for tower reinforcements."""
-    structure = notif.structures.first()
+    structure = notif.structures.select_related(
+        "eve_solar_system", "eve_type", "eve_moon"
+    ).first()
     eve_time = dt.datetime.fromisoformat(notif.details["reinforced_until"])
     timer_processed = False
-    if has_auth_timers:
+
+    if HAS_AUTH_TIMERS:
         structure_type_map = {
             starbases.StarbaseSize.SMALL: "POS[S]",
             starbases.StarbaseSize.MEDIUM: "POS[M]",
             starbases.StarbaseSize.LARGE: "POS[L]",
         }
         structure_str = structure_type_map.get(
             starbases.starbase_size(structure.eve_type), "POS[M]"
@@ -384,27 +374,23 @@
             objective="Friendly",
             eve_time=eve_time,
             eve_corp=notif.owner.corporation,
             corp_timer=STRUCTURES_TIMERS_ARE_CORP_RESTRICTED,
         )
         timer_processed = True
 
-    if has_structure_timers:
-        eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
-            id=structure.eve_solar_system.id
-        )
-        structure_type, _ = EveType.objects.get_or_create_esi(id=structure.eve_type.id)
+    if HAS_STRUCTURE_TIMERS:
         visibility = (
             Timer.Visibility.CORPORATION
             if STRUCTURES_TIMERS_ARE_CORP_RESTRICTED
             else Timer.Visibility.UNRESTRICTED
         )
         Timer.objects.create(
-            eve_solar_system=eve_solar_system,
-            structure_type=structure_type,
+            eve_solar_system=structure.eve_solar_system,
+            structure_type=structure.eve_type,
             timer_type=Timer.Type.FINAL,
             objective=Timer.Objective.FRIENDLY,
             date=eve_time,
             location_details=structure.eve_moon.name,
             eve_corporation=notif.owner.corporation,
             eve_alliance=notif.owner.corporation.alliance,
             visibility=visibility,
```

### Comparing `aa_structures-2.4.2/structures/core/serializers.py` & `aa_structures-2.5.0/structures/core/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""JSON serializers for Structures."""
+
+# pylint: disable=missing-class-docstring
+
 import re
 from abc import ABC, abstractmethod
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.db.models import Q, Sum
 from django.urls import reverse
@@ -20,33 +24,35 @@
     image_html,
     link_html,
     no_wrap_html,
     yesno_str,
     yesnonone_str,
 )
 
-from ..app_settings import STRUCTURES_SHOW_FUEL_EXPIRES_RELATIVE
-from ..constants import EveTypeId
-from ..models import EveSpaceType, Structure, StructureItem, StructureService
+from structures.app_settings import STRUCTURES_SHOW_FUEL_EXPIRES_RELATIVE
+from structures.constants import EveTypeId
+from structures.models import EveSpaceType, Structure, StructureItem, StructureService
 
 
 class _AbstractStructureListSerializer(ABC):
     """Converting a list of structure objects into a dict for JSON."""
 
     ICON_RENDER_SIZE = 64
     ICON_OUTPUT_SIZE = 40
 
     def __init__(self, queryset: models.QuerySet, request=None):
         self.queryset = queryset
         self._request = request
 
     def has_data(self) -> bool:
+        """Return True if this query returns any data, else False."""
         return self.queryset.exists()
 
     def count(self) -> bool:
+        """Return number of objects in this query."""
         return self.queryset.count()
 
     def to_list(self) -> list:
         """Serialize all objects into a list."""
         return [self.serialize_object(obj) for obj in self.queryset]
 
     @abstractmethod
@@ -136,15 +142,15 @@
             tags += [x.html for x in structure.tags.all()]
             row["structure_name"] += format_html("<br>{}", mark_safe(" ".join(tags)))
 
     def _add_services(self, structure, row):
         if row["is_poco"] or row["is_starbase"]:
             row["services"] = "-"
             return
-        services = list()
+        services = []
         for service in structure.services.all():
             service_name_html = no_wrap_html(
                 format_html("<small>{}</small>", service.name)
             )
             if service.state == StructureService.State.OFFLINE:
                 service_name_html = format_html("<del>{}</del>", service_name_html)
             services.append({"name": service.name, "html": service_name_html})
@@ -159,15 +165,15 @@
     def _add_reinforcement_infos(self, structure, row):
         row["is_reinforced"] = structure.is_reinforced
         row["is_reinforced_str"] = yesno_str(structure.is_reinforced)
         if structure.is_starbase:
             row["reinforcement"] = "-"
         else:
             if structure.reinforce_hour is not None:
-                row["reinforcement"] = "{:02d}:00".format(structure.reinforce_hour)
+                row["reinforcement"] = f"{structure.reinforce_hour:02d}:00"
             else:
                 row["reinforcement"] = ""
 
     def _add_fuel_infos(self, structure, row):
         if structure.is_poco:
             fuel_expires_display = "-"
             fuel_expires_timestamp = None
@@ -263,16 +269,16 @@
             last_online_at_timestamp = None
         row["last_online_at"] = {
             "display": no_wrap_html(last_online_at_display),
             "timestamp": last_online_at_timestamp,
         }
 
     def _add_state(self, structure, row, request):
-        def cap_first(s: str) -> str:
-            return s[0].upper() + s[1::]
+        def cap_first(text: str) -> str:
+            return text[0].upper() + text[1::]
 
         row["state_str"] = (
             cap_first(structure.get_state_display()) if not structure.is_poco else "-"
         )
         row["state_details"] = row["state_str"]
         if structure.state_timer_end:
             row["state_details"] += format_html(
```

### Comparing `aa_structures-2.4.2/structures/core/sovereignty.py` & `aa_structures-2.5.0/structures/core/sovereignty.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Eve sovereignty related core logic."""
 
 from typing import Optional
 
-from ..constants import EveTypeId
+from structures.constants import EveTypeId
 
 _MAP_CAMPAIGN_EVENT_2_TYPE_ID = {
     1: EveTypeId.TCU,
     2: EveTypeId.IHUB,
 }
 _MAP_TYPE_ID_2_TIMER_STRUCTURE_NAME = {
     EveTypeId.CUSTOMS_OFFICE: "POCO",
     EveTypeId.TCU: "TCU",
     EveTypeId.IHUB: "I-HUB",
 }
 
 
-def type_id_from_event_type(event_type: int) -> Optional[int]:
+def event_type_to_type_id(event_type: int) -> Optional[int]:
+    """Convert an event type to a type ID."""
     return _MAP_CAMPAIGN_EVENT_2_TYPE_ID.get(event_type)
 
 
-def structure_type_name_from_event_type(event_type: int) -> str:
+def event_type_to_structure_type_name(event_type: int) -> str:
+    """Convert an event type to a structure type name."""
     return _MAP_TYPE_ID_2_TIMER_STRUCTURE_NAME.get(
-        type_id_from_event_type(event_type), "Other"
+        event_type_to_type_id(event_type), "Other"
     )
```

### Comparing `aa_structures-2.4.2/structures/core/starbases.py` & `aa_structures-2.5.0/structures/core/starbases.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,60 @@
+"""Core logic for starbases in Structures."""
+
 import math
 from enum import IntEnum, auto
 from typing import Optional
 
 from eveuniverse.models import EveType
 
-from ..constants import EveGroupId
+from structures.constants import EveGroupId
 
 
 class StarbaseSize(IntEnum):
+    """A starbase size."""
+
     SMALL = auto()
     MEDIUM = auto()
     LARGE = auto()
 
 
 def is_starbase(eve_type: EveType) -> bool:
+    """Return True if this type is a starbase, else False."""
     return eve_type.eve_group_id == EveGroupId.CONTROL_TOWER
 
 
 def starbase_size(eve_type: EveType) -> StarbaseSize:
-    """return the size of a starbase or None if this type is not a starbase"""
+    """Return the size of a starbase or None if this type is not a starbase."""
     if not is_starbase(eve_type):
         return None
-    elif "medium" in eve_type.name.lower():
+
+    if "medium" in eve_type.name.lower():
         return StarbaseSize.MEDIUM
-    elif "small" in eve_type.name.lower():
+
+    if "small" in eve_type.name.lower():
         return StarbaseSize.SMALL
+
     return StarbaseSize.LARGE
 
 
 def fuel_per_hour(eve_type: EveType) -> Optional[int]:
     """Calculate the number of fuel blocks consumed per hour.
 
-    Returns None if not a starbase.
+    Return None if not a starbase.
     """
     size = starbase_size(eve_type)
     if size is StarbaseSize.LARGE:
         return 40
-    elif size is StarbaseSize.MEDIUM:
+
+    if size is StarbaseSize.MEDIUM:
         return 20
-    elif size is StarbaseSize.SMALL:
+
+    if size is StarbaseSize.SMALL:
         return 10
+
     return None
 
 
 def fuel_duration(
     starbase_type: EveType,
     fuel_quantity: int,
     has_sov: bool = False,
```

### Comparing `aa_structures-2.4.2/structures/helpers/general.py` & `aa_structures-2.5.0/structures/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+"""Helpers for Structures."""
+
 import datetime as dt
 from typing import Optional
+from urllib.parse import urlparse
 
 from django.utils.timezone import now
 
 
 def hours_until_deadline(
     deadline: dt.datetime, start: Optional[dt.datetime] = None
 ) -> float:
@@ -21,7 +24,12 @@
     """True when first and second datetime are within threshold in seconds.
     False when first or second is None.
     """
     if not first or not second:
         return False
     dif = abs((first - second).total_seconds())
     return dif <= abs(threshold)
+
+
+def is_absolute_url(url: str) -> bool:
+    """Return True if URL is absolute else False."""
+    return bool(urlparse(url).netloc)
```

### Comparing `aa_structures-2.4.2/structures/locale/de/LC_MESSAGES/django.mo` & `aa_structures-2.5.0/structures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/de/LC_MESSAGES/django.po` & `aa_structures-2.5.0/structures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/django.pot` & `aa_structures-2.5.0/structures/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/en/LC_MESSAGES/django.po` & `aa_structures-2.5.0/structures/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/es/LC_MESSAGES/django.mo` & `aa_structures-2.5.0/structures/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/es/LC_MESSAGES/django.po` & `aa_structures-2.5.0/structures/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/fr_FR/LC_MESSAGES/django.po` & `aa_structures-2.5.0/structures/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/it_IT/LC_MESSAGES/django.po` & `aa_structures-2.5.0/structures/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/ja/LC_MESSAGES/django.po` & `aa_structures-2.5.0/structures/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/ko/LC_MESSAGES/django.po` & `aa_structures-2.5.0/structures/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/ko_KR/LC_MESSAGES/django.po` & `aa_structures-2.5.0/structures/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/ru/LC_MESSAGES/django.mo` & `aa_structures-2.5.0/structures/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/ru/LC_MESSAGES/django.po` & `aa_structures-2.5.0/structures/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/uk/LC_MESSAGES/django.po` & `aa_structures-2.5.0/structures/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_structures-2.5.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_structures-2.5.0/structures/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/management/commands/structures_load_eve.py` & `aa_structures-2.5.0/structures/management/commands/structures_load_eve.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+"""Command to load eve types for Structures."""
+
 from django.core.management import call_command
 from django.core.management.base import BaseCommand
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
-from ... import __title__
-from ...constants import EveCategoryId, EveGroupId, EveTypeId
+from structures import __title__
+from structures.constants import EveCategoryId, EveGroupId, EveTypeId
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class Command(BaseCommand):
     help = "Preloads data required for this app from ESI"
```

### Comparing `aa_structures-2.4.2/structures/management/commands/structures_preload_eveuniverse.py` & `aa_structures-2.5.0/structures/management/commands/structures_preload_eveuniverse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+"""Command to preload eveuniverse object for migration to Structures 2."""
+
 from django.core.management.base import BaseCommand, CommandError
 from eveuniverse.models import EveEntity, EveMoon, EvePlanet, EveSolarSystem, EveType
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.esi import fetch_esi_status
 from app_utils.logging import LoggerAddTag
 
-from ... import __title__
-from ...models import Notification, StarbaseDetailFuel, Structure, StructureItem
+from structures import __title__
+from structures.models import Notification, StarbaseDetailFuel, Structure, StructureItem
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class Command(BaseCommand):
     help = "Preload missing eveuniverse objects in preparation for migrating to eveuniverse with release 2."
```

### Comparing `aa_structures-2.4.2/structures/managers.py` & `aa_structures-2.5.0/structures/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+"""Managers for Structures."""
+
+# pylint: disable=missing-class-docstring
+
 import datetime as dt
 import itertools
-from typing import Optional, Set, Tuple, TypeVar
+from typing import Any, Optional, Set, Tuple
 
 from django.contrib.auth.models import User
 from django.db import models, transaction
 from django.db.models import Case, Count, Exists, OuterRef, Q, Value, When
 from django.utils.timezone import now
 from esi.models import Token
 from eveuniverse.models import EveMoon, EvePlanet, EveSolarSystem, EveType
@@ -12,28 +16,28 @@
 from allianceauth.eveonline.models import EveCorporationInfo
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
 from . import __title__
 from .app_settings import STRUCTURES_HOURS_UNTIL_STALE_NOTIFICATION
 from .constants import EveCategoryId, EveTypeId
+from .core.notification_types import NotificationType
 from .providers import esi
 from .webhooks.managers import WebhookBaseManager
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
-ModelType = TypeVar("ModelType", bound=models.Model)
-
 
 class EveSovereigntyMapManager(models.Manager):
-    def update_from_esi(self):
+    def update_or_create_all_from_esi(self):
+        """Update or create complete sovereignty map from ESI."""
         sov_map = esi.client.Sovereignty.get_sovereignty_map().results()
         logger.info("Retrieved sovereignty map from ESI")
         last_updated = now()
-        obj_list = list()
+        obj_list = []
         for solar_system in sov_map:
             obj_def = {
                 "solar_system_id": solar_system["system_id"],
                 "last_updated": last_updated,
             }
             for key in ["alliance_id", "corporation_id", "faction_id"]:
                 if key in solar_system and solar_system[key]:
@@ -58,21 +62,21 @@
         self, eve_solar_system, corporation: EveCorporationInfo
     ) -> bool:
         """returns true if given corporation has sov in this solar system
         else False
         """
         if not eve_solar_system.is_null_sec:
             return False
-        else:
-            alliance_id = (
-                int(corporation.alliance.alliance_id) if corporation.alliance else None
-            )
-            return bool(alliance_id) and (
-                self.solar_system_sov_alliance_id(eve_solar_system) == alliance_id
-            )
+
+        alliance_id = (
+            int(corporation.alliance.alliance_id) if corporation.alliance else None
+        )
+        return bool(alliance_id) and (
+            self.solar_system_sov_alliance_id(eve_solar_system) == alliance_id
+        )
 
     def solar_system_sov_alliance_id(self, eve_solar_system) -> Optional[int]:
         """returns ID of sov owning alliance for this system or None"""
         if not eve_solar_system.is_null_sec:
             return None
         try:
             sov_map = self.get(solar_system_id=eve_solar_system.id)
@@ -80,35 +84,33 @@
         except self.model.DoesNotExist:
             return None
 
 
 class NotificationBaseQuerySet(models.QuerySet):
     def annotate_can_be_rendered(self) -> models.QuerySet:
         """annotates field indicating if a notification can be rendered"""
-        from .models import NotificationType
 
         return self.annotate(
             can_be_rendered_2=Case(
                 When(notif_type__in=NotificationType.values, then=True),
                 default=Value(False),
                 output_field=models.BooleanField(),
             )
         )
 
 
 class NotificationBaseManagerBase(models.Manager):
     def add_or_remove_timers(self):
         """Add or remove timers from notifications."""
-        from .models import NotificationType
 
         cutoff_dt_for_stale = now() - dt.timedelta(
             hours=STRUCTURES_HOURS_UNTIL_STALE_NOTIFICATION
         )
         notifications = (
-            self.filter(notif_type__in=NotificationType.relevant_for_timerboard)
+            self.filter(notif_type__in=NotificationType.relevant_for_timerboard())
             .exclude(is_timer_added=True)
             .filter(timestamp__gte=cutoff_dt_for_stale)
             .select_related("owner")
             .order_by("timestamp")
         )
         if notifications.exists():
             for notification in notifications:
@@ -129,26 +131,23 @@
 class GeneratedNotificationQuerySet(NotificationBaseQuerySet):
     pass
 
 
 class GeneratedNotificationManagerBase(NotificationBaseManagerBase):
     def get_or_create_from_structure(
         self, structure: models.Model, notif_type: models.TextChoices
-    ) -> Tuple[ModelType, bool]:
+    ) -> Tuple[Any, bool]:
         """Get or create an object from given structure."""
-        from .models import NotificationType
 
         if notif_type not in {NotificationType.TOWER_REINFORCED_EXTRA}:
             raise ValueError(f"Unsupported notification type: {notif_type}")
 
         return self._get_or_create_tower_reinforced(structure)
 
-    def _get_or_create_tower_reinforced(self, structure) -> Tuple[ModelType, bool]:
-        from .models import NotificationType
-
+    def _get_or_create_tower_reinforced(self, structure) -> Tuple[Any, bool]:
         if not structure.is_starbase:
             raise ValueError(f"Structure is not a starbase: {structure}")
         if not structure.is_reinforced:
             raise ValueError(f"Starbase is not reinforced: {structure}")
         if not structure.state_timer_end:
             raise ValueError(f"Starbase has no reinforce time: {structure}")
         reinforced_until = structure.state_timer_end.isoformat()
@@ -174,14 +173,15 @@
 GeneratedNotificationManager = GeneratedNotificationManagerBase.from_queryset(
     GeneratedNotificationQuerySet
 )
 
 
 class OwnerQuerySet(models.QuerySet):
     def annotate_characters_count(self) -> models.QuerySet:
+        """Add character count annotation."""
         return self.annotate(
             x_characters_count=Count(
                 "characters",
                 filter=Q(characters__character_ownership__isnull=False),
                 distinct=True,
             )
         )
@@ -199,20 +199,23 @@
 
 
 OwnerManager = OwnerManagerBase.from_queryset(OwnerQuerySet)
 
 
 class StructureQuerySet(models.QuerySet):
     def filter_upwell_structures(self) -> models.QuerySet:
+        """Filter for upwell structures."""
         return self.filter(eve_type__eve_group__eve_category=EveCategoryId.STRUCTURE)
 
     def filter_customs_offices(self) -> models.QuerySet:
+        """Filter for custom offices."""
         return self.filter(eve_type=EveTypeId.CUSTOMS_OFFICE)
 
     def filter_starbases(self) -> models.QuerySet:
+        """Filter for starbases."""
         return self.filter(eve_type__eve_group__eve_category=EveCategoryId.STARBASE)
 
     def ids(self) -> Set[int]:
         """Return ids as set."""
         return set(self.values_list("id", flat=True))
 
     def select_related_defaults(self) -> models.QuerySet:
@@ -230,14 +233,15 @@
             "eve_type__eve_group__eve_category",
         )
 
     # TODO: Add specific tests
     def visible_for_user(
         self, user: User, tags: Optional[list] = None
     ) -> models.QuerySet:
+        """Return structures which the given user have permission to view."""
         if user.has_perm("structures.view_all_structures"):
             structures_query = self.select_related_defaults()
             if tags:
                 structures_query = structures_query.filter(
                     tags__name__in=tags
                 ).distinct()
 
@@ -270,34 +274,36 @@
 
             structures_query = self.select_related_defaults().filter(
                 owner__corporation__in=corporations
             )
         return structures_query
 
     def annotate_has_poco_details(self) -> models.QuerySet:
+        """Add annotation wether the structure has poco details."""
         from .models import PocoDetails
 
         return self.annotate(
             has_poco_details=Exists(
                 PocoDetails.objects.filter(structure_id=OuterRef("id"))
             )
         )
 
     def annotate_has_starbase_detail(self) -> models.QuerySet:
+        """Add annotation wether the structure has starbase details."""
         from .models import StarbaseDetail
 
         return self.annotate(
             has_starbase_detail=Exists(
                 StarbaseDetail.objects.filter(structure_id=OuterRef("id"))
             )
         )
 
 
 class StructureManagerBase(models.Manager):
-    def get_or_create_esi(self, *, id: int, token: Token) -> tuple:
+    def get_or_create_esi(self, *, id: int, token: Token) -> Tuple[Any, bool]:
         """get or create a structure with data from ESI if needed.
 
         Args:
             id: Structure ID of object in Eve Online
             token: ``esi.models.Token`` object with scope:
                 ``esi-universe.read_structures.v1``
 
@@ -307,15 +313,15 @@
         id = int(id)
         try:
             obj = self.get(id=id)
             return obj, False
         except self.model.DoesNotExist:
             return self.update_or_create_esi(id=id, token=token)
 
-    def update_or_create_esi(self, *, id: int, token: Token) -> tuple:
+    def update_or_create_esi(self, *, id: int, token: Token) -> Tuple[Any, bool]:
         """update or create a structure from ESI for given structure ID
         This will only fetch basic info about a structure
 
         Args:
             id: Structure ID of object in Eve Online
             token: ``esi.models.Token`` object with scope: ``esi-universe.read_structures.v1``
 
@@ -341,46 +347,32 @@
         }
         owner = Owner.objects.get(
             corporation__corporation_id=structure_info["corporation_id"]
         )
         obj, created = self.update_or_create_from_dict(structure=structure, owner=owner)
         return obj, created
 
-    def update_or_create_from_dict(self, structure: dict, owner) -> tuple:
+    def update_or_create_from_dict(self, structure: dict, owner) -> Tuple[Any, bool]:
         """update or create structure from given dict"""
 
-        from .models import StructureService
-
         eve_type, _ = EveType.objects.get_or_create_esi(id=structure["type_id"])
         eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
             id=structure["system_id"]
         )
-        if position := structure.get("position"):
-            position_x = position.get("x")
-            position_y = position.get("y")
-            position_z = position.get("z")
-        else:
-            position_x = position_y = position_z = None
-        if planet_id := structure.get("planet_id"):
-            eve_planet, _ = EvePlanet.objects.get_or_create_esi(id=planet_id)
-        else:
-            eve_planet = None
-        if moon_id := structure.get("moon_id"):
-            eve_moon, _ = EveMoon.objects.get_or_create_esi(id=moon_id)
-        else:
-            eve_moon = None
+        position_x, position_y, position_z = self._extract_position(structure)
+        eve_planet = self._extract_eve_planet(structure)
+        eve_moon = self._extract_eve_moon(structure)
 
-        structure_id = structure["structure_id"]
         try:
-            old_obj = self.get(id=structure_id)
+            old_obj = self.get(id=structure["structure_id"])
         except self.model.DoesNotExist:
             old_obj = None
 
         obj, created = self.update_or_create(
-            id=structure_id,
+            id=structure["structure_id"],
             defaults={
                 "owner": owner,
                 "eve_type": eve_type,
                 "name": structure.get("name", ""),
                 "eve_solar_system": eve_solar_system,
                 "eve_planet": eve_planet,
                 "eve_moon": eve_moon,
@@ -403,15 +395,37 @@
             obj.handle_fuel_notifications(old_obj)
 
         # Make sure we have dogmas loaded for this type for fittings
         EveType.objects.get_or_create_esi(
             id=structure["type_id"], enabled_sections=[EveType.Section.DOGMAS]
         )
 
-        # save related structure services
+        self._save_related_structure_services(structure, obj)
+
+        return obj, created
+
+    def _extract_eve_moon(self, structure):
+        if moon_id := structure.get("moon_id"):
+            return EveMoon.objects.get_or_create_esi(id=moon_id)[0]
+        return None
+
+    def _extract_eve_planet(self, structure):
+        if planet_id := structure.get("planet_id"):
+            return EvePlanet.objects.get_or_create_esi(id=planet_id)[0]
+        return None
+
+    def _extract_position(self, structure):
+        if position := structure.get("position"):
+            return position.get("x"), position.get("y"), position.get("z")
+        return None, None, None
+
+    @staticmethod
+    def _save_related_structure_services(structure, obj):
+        from .models import StructureService
+
         StructureService.objects.filter(structure=obj).delete()
         if "services" in structure and structure["services"]:
             for service in structure["services"]:
                 service_state = StructureService.State.from_esi_name(service["state"])
                 args = {
                     "structure": obj,
                     "name": service["name"],
@@ -419,35 +433,39 @@
                 }
                 StructureService.objects.create(**args)
 
         if obj.services.filter(state=StructureService.State.ONLINE).exists():
             obj.last_online_at = now()
             obj.save()
 
-        return obj, created
-
 
 StructureManager = StructureManagerBase.from_queryset(StructureQuerySet)
 
 
 class StructureTagManager(models.Manager):
-    def get_or_create_for_space_type(self, solar_system) -> tuple:
+    def get_or_create_for_space_type(
+        self, solar_system: EveSolarSystem
+    ) -> Tuple[Any, bool]:
+        """Get or create tag for a space type."""
         from .models import EveSpaceType
 
         space_type = EveSpaceType.from_solar_system(solar_system)
         params = self.model.SPACE_TYPE_MAP.get(space_type)
         if params:
             try:
                 obj = self.get(name=params["name"])
                 return obj, False
             except self.model.DoesNotExist:
                 return self.update_or_create_for_space_type(solar_system)
         return None, None
 
-    def update_or_create_for_space_type(self, solar_system) -> tuple:
+    def update_or_create_for_space_type(
+        self, solar_system: EveSolarSystem
+    ) -> Tuple[Any, bool]:
+        """Update or create tag for a space type."""
         from .models import EveSpaceType
 
         space_type = EveSpaceType.from_solar_system(solar_system)
         params = self.model.SPACE_TYPE_MAP.get(space_type)
         if params:
             return self.update_or_create(
                 name=params["name"],
@@ -459,22 +477,24 @@
                     "order": 50,
                     "is_user_managed": False,
                     "is_default": False,
                 },
             )
         return None, None
 
-    def get_or_create_for_sov(self) -> tuple:
+    def get_or_create_for_sov(self) -> Tuple[Any, bool]:
+        """Get or create sovereignty tag."""
         try:
             obj = self.get(name=self.model.NAME_SOV_TAG)
             return obj, False
         except self.model.DoesNotExist:
             return self.update_or_create_for_sov()
 
-    def update_or_create_for_sov(self) -> tuple:
+    def update_or_create_for_sov(self) -> Tuple[Any, bool]:
+        """Update or create sovereignty tag."""
         return self.update_or_create(
             name=self.model.NAME_SOV_TAG,
             defaults={
                 "style": self.model.Style.DARK_BLUE,
                 "description": (
                     "Owner of this structure has sovereignty. system generated."
                 ),
```

### Comparing `aa_structures-2.4.2/structures/migrations/0001_initial_new.py` & `aa_structures-2.5.0/structures/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/migrations/0002_remove_eveuniverse_relation_names.py` & `aa_structures-2.5.0/structures/migrations/0002_remove_eveuniverse_relation_names.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/migrations/0003_add_localization_and_unique_key.py` & `aa_structures-2.5.0/structures/migrations/0003_add_localization_and_unique_key.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/models/eveuniverse.py` & `aa_structures-2.5.0/structures/models/eveuniverse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Eve Universe models"""
+"""Eve Universe models for Structures."""
 
 from enum import Enum
 
 from django.db import models
 from eveuniverse.models import EveSolarSystem
 
-from ..managers import EveSovereigntyMapManager
+from structures.managers import EveSovereigntyMapManager
 
 
 class EveSovereigntyMap(models.Model):
     """Shows which alliance / corporation / faction owns a system
 
     Note: This model does not hold FKs to respective objects like
     EveSolarSystem to avoid having load all those object from ESI
@@ -44,31 +44,35 @@
 
     objects = EveSovereigntyMapManager()
 
     def __str__(self):
         return str(self.solar_system_id)
 
     def __repr__(self):
-        return "{}(solar_system_id='{}')".format(
-            self.__class__.__name__, self.solar_system_id
-        )
+        return f"{self.__class__.__name__}(solar_system_id='{self.solar_system_id}')"
 
 
 class EveSpaceType(str, Enum):
+    """A space type in Eve Online."""
+
     UNKNOWN = "unknown"
     HIGHSEC = "highsec"
     LOWSEC = "lowsec"
     NULLSEC = "nullsec"
     W_SPACE = "w-space"
 
     @classmethod
     def from_solar_system(cls, eve_solar_system: EveSolarSystem) -> "EveSpaceType":
         """returns the space type"""
         if eve_solar_system.is_null_sec:
             return cls.NULLSEC
-        elif eve_solar_system.is_low_sec:
+
+        if eve_solar_system.is_low_sec:
             return cls.LOWSEC
-        elif eve_solar_system.is_high_sec:
+
+        if eve_solar_system.is_high_sec:
             return cls.HIGHSEC
-        elif eve_solar_system.is_w_space:
+
+        if eve_solar_system.is_w_space:
             return cls.W_SPACE
+
         return cls.UNKNOWN
```

### Comparing `aa_structures-2.4.2/structures/models/notifications.py` & `aa_structures-2.5.0/structures/models/owners.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1157 +1,1356 @@
-"""Notification related models."""
+"""Owner related models for Structures."""
 
-import math
-from typing import List, Optional, Set, Tuple, Union
+# pylint: disable = duplicate-code,too-many-lines
 
-import dhooks_lite
-import yaml
-from multiselectfield import MultiSelectField
-from requests.exceptions import HTTPError
-
-from django.contrib.auth.models import Group
-from django.core.exceptions import ValidationError
-from django.db import models
-from django.db.models import Q
-from django.utils import translation
-from django.utils.functional import classproperty  # type: ignore
+import datetime as dt
+import json
+import os
+import re
+from email.utils import format_datetime, parsedate_to_datetime
+from typing import Any, Iterable, List, Optional
+
+from bravado.exception import HTTPForbidden, HTTPNotFound
+
+from django.contrib.auth.models import Group, User
+from django.core.exceptions import ObjectDoesNotExist
+from django.core.serializers.json import DjangoJSONEncoder
+from django.db import models, transaction
+from django.db.models import F
 from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
-from eveuniverse.models import EveEntity
-
+from esi.errors import TokenError
+from esi.models import Token
+from eveuniverse.models import EveMoon, EvePlanet, EveSolarSystem, EveType
+
+from allianceauth.authentication.models import CharacterOwnership
+from allianceauth.eveonline.models import EveCorporationInfo
+from allianceauth.notifications import notify
 from allianceauth.services.hooks import get_extension_logger
-from app_utils.django import app_labels
+from app_utils.allianceauth import notify_admins
+from app_utils.datetime import DATETIME_FORMAT
+from app_utils.helpers import chunks
 from app_utils.logging import LoggerAddTag
-from app_utils.urls import static_file_absolute_url
 
-from .. import __title__
-from ..app_settings import (  # STRUCTURES_NOTIFICATION_DISABLE_ESI_FUEL_ALERTS,
-    STRUCTURES_ADD_TIMERS,
-    STRUCTURES_DEFAULT_LANGUAGE,
-    STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS,
-    STRUCTURES_NOTIFICATION_SET_AVATAR,
-    STRUCTURES_REPORT_NPC_ATTACKS,
+from structures import __title__
+from structures.app_settings import (
+    STRUCTURES_ADMIN_NOTIFICATIONS_ENABLED,
+    STRUCTURES_DEVELOPER_MODE,
+    STRUCTURES_ESI_DIRECTOR_ERROR_MAX_RETRIES,
+    STRUCTURES_FEATURE_CUSTOMS_OFFICES,
+    STRUCTURES_FEATURE_STARBASES,
+    STRUCTURES_HOURS_UNTIL_STALE_NOTIFICATION,
+    STRUCTURES_NOTIFICATION_SYNC_GRACE_MINUTES,
+    STRUCTURES_NOTIFICATIONS_ARCHIVING_ENABLED,
+    STRUCTURES_STRUCTURE_SYNC_GRACE_MINUTES,
+)
+from structures.constants import EveGroupId, EveTypeId
+from structures.managers import OwnerManager
+from structures.providers import esi
+
+from .eveuniverse import EveSovereigntyMap
+from .notifications import (
+    EveEntity,
+    GeneratedNotification,
+    Notification,
+    NotificationType,
+    Webhook,
 )
-from ..constants import EveCategoryId, EveCorporationId, EveTypeId
-from ..managers import GeneratedNotificationManager, NotificationManager, WebhookManager
-from ..webhooks.models import WebhookBase
-from .structures import Structure
+from .structures_1 import Structure, StructureItem
+from .structures_2 import PocoDetails, StarbaseDetail, StarbaseDetailFuel
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
-# Supported languages
-LANGUAGES = (
-    ("en", _("English")),
-    ("de", _("German")),
-    ("es", _("Spanish")),
-    ("zh-hans", _("Chinese Simplified")),
-    ("ru", _("Russian")),
-    ("ko", _("Korean")),
-)
 
+class General(models.Model):
+    """Meta model for global app permissions"""
 
-class NotificationType(models.TextChoices):
-    """Definition of all supported notification types."""
+    class Meta:
+        managed = False
+        default_permissions = ()
+        permissions = (
+            ("basic_access", "Can access this app and view public pages"),
+            ("view_corporation_structures", "Can view corporation structures"),
+            ("view_alliance_structures", "Can view alliance structures"),
+            ("view_all_structures", "Can view all structures"),
+            ("add_structure_owner", "Can add new structure owner"),
+            (
+                "view_all_unanchoring_status",
+                "Can view unanchoring timers for all structures the user can see",
+            ),
+            ("view_structure_fit", "Can view structure fit"),
+        )
 
-    # upwell structures
-    STRUCTURE_ANCHORING = "StructureAnchoring", _("Upwell structure anchoring")
-    STRUCTURE_ONLINE = "StructureOnline", _("Upwell structure went online")
-    STRUCTURE_SERVICES_OFFLINE = "StructureServicesOffline", _(
-        "Upwell structure services went offline"
-    )
-    STRUCTURE_WENT_HIGH_POWER = "StructureWentHighPower", _(
-        "Upwell structure went high power"
-    )
-    STRUCTURE_WENT_LOW_POWER = "StructureWentLowPower", _(
-        "Upwell structure went low power"
-    )
-    STRUCTURE_UNANCHORING = "StructureUnanchoring", _("Upwell structure unanchoring")
-    STRUCTURE_FUEL_ALERT = "StructureFuelAlert", _("Upwell structure fuel alert")
-    STRUCTURE_REFUELED_EXTRA = "StructureRefueledExtra", _("Upwell structure refueled")
-    STRUCTURE_JUMP_FUEL_ALERT = "StructureJumpFuelAlert", _(
-        "Upwell structure jump fuel alert"
-    )
-    STRUCTURE_UNDER_ATTACK = "StructureUnderAttack", _(
-        "Upwell structure is under attack"
-    )
-    STRUCTURE_LOST_SHIELD = "StructureLostShields", _("Upwell structure lost shields")
-    STRUCTURE_LOST_ARMOR = "StructureLostArmor", _("Upwell structure lost armor")
-    STRUCTURE_DESTROYED = "StructureDestroyed", _("Upwell structure destroyed")
 
-    STRUCTURE_REINFORCE_CHANGED = "StructuresReinforcementChanged", _(
-        "Upwell structure reinforcement time changed"
-    )
-    OWNERSHIP_TRANSFERRED = "OwnershipTransferred", _(
-        "Upwell structure ownership transferred"
-    )
+class Owner(models.Model):
+    """A corporation that owns structures"""
 
-    # customs offices
-    ORBITAL_ATTACKED = "OrbitalAttacked", _("Customs office attacked")
-    ORBITAL_REINFORCED = "OrbitalReinforced", _("Customs office reinforced")
-
-    # starbases
-    TOWER_ALERT_MSG = "TowerAlertMsg", _("Starbase attacked")
-    TOWER_RESOURCE_ALERT_MSG = "TowerResourceAlertMsg", _("Starbase fuel alert")
-    TOWER_REFUELED_EXTRA = "TowerRefueledExtra", _("Starbase refueled (BETA)")
-    TOWER_REINFORCED_EXTRA = "TowerReinforcedExtra", _("Starbase reinforced (BETA)")
-
-    # moon mining
-    MOONMINING_EXTRACTION_STARTED = "MoonminingExtractionStarted", _(
-        "Moon mining extraction started"
-    )
-    MOONMINING_LASER_FIRED = "MoonminingLaserFired", _("Moonmining laser fired")
-    MOONMINING_EXTRACTION_CANCELLED = "MoonminingExtractionCancelled", _(
-        "Moon mining extraction cancelled"
-    )
-    MOONMINING_EXTRACTION_FINISHED = "MoonminingExtractionFinished", _(
-        "Moon mining extraction finished"
-    )
-    MOONMINING_AUTOMATIC_FRACTURE = "MoonminingAutomaticFracture", _(
-        "Moon mining automatic fracture triggered"
-    )
+    class RotateCharactersType(models.TextChoices):
+        """Type of sync to rotate characters for."""
 
-    # sov
-    SOV_STRUCTURE_REINFORCED = "SovStructureReinforced", _(
-        "Sovereignty structure reinforced"
-    )
-    SOV_STRUCTURE_DESTROYED = "SovStructureDestroyed", _(
-        "Sovereignty structure destroyed"
-    )
-    SOV_ENTOSIS_CAPTURE_STARTED = "EntosisCaptureStarted", _(
-        "Sovereignty entosis capture started"
-    )
-    SOV_COMMAND_NODE_EVENT_STARTED = "SovCommandNodeEventStarted", _(
-        "Sovereignty command node event started"
-    )
-    SOV_ALL_CLAIM_ACQUIRED_MSG = "SovAllClaimAquiredMsg", _(
-        "Sovereignty claim acknowledgment"  # SovAllClaimAquiredMsg [sic!]
-    )
-    SOV_ALL_CLAIM_LOST_MSG = "SovAllClaimLostMsg", _("Sovereignty lost")
-    SOV_ALL_ANCHORING_MSG = "AllAnchoringMsg", _(
-        "Structure anchoring in alliance space"
-    )
+        STRUCTURES = "structures"
+        NOTIFICATIONS = "notifications"
 
-    # wars
-    WAR_WAR_DECLARED = "WarDeclared", _("War declared")
-    WAR_ALLY_JOINED_WAR_AGGRESSOR_MSG = "AllyJoinedWarAggressorMsg", _(
-        "War ally joined aggressor"
-    )
-    WAR_ALLY_JOINED_WAR_AllY_MSG = "AllyJoinedWarAllyMsg", _("War ally joined ally")
-    WAR_ALLY_JOINED_WAR_DEFENDER_MSG = "AllyJoinedWarDefenderMsg", _(
-        "War ally joined defender"
-    )
-    WAR_WAR_ADOPTED = "WarAdopted", _("War adopted")
-    WAR_WAR_INHERITED = "WarInherited", _("War inherited")
-    WAR_CORP_WAR_SURRENDER_MSG = "CorpWarSurrenderMsg", _("War party surrendered")
-    WAR_WAR_RETRACTED_BY_CONCORD = "WarRetractedByConcord", _(
-        "War retracted by Concord"
-    )
-    WAR_CORPORATION_BECAME_ELIGIBLE = "CorpBecameWarEligible", _(
-        "War corporation became eligible"
-    )
-    WAR_CORPORATION_NO_LONGER_ELIGIBLE = "CorpNoLongerWarEligible", _(
-        "War corporation no longer eligible"
+        @property
+        def last_used_at_name(self) -> str:
+            """Name of last used at property."""
+            if self is self.STRUCTURES:
+                return "structures_last_used_at"
+            if self is self.NOTIFICATIONS:
+                return "notifications_last_used_at"
+            raise NotImplementedError(f"Not defined for: {self}")
+
+        @property
+        def esi_cache_duration(self) -> int:
+            """ESI cache duration in seconds."""
+            if self is self.STRUCTURES:
+                return 3600
+            if self is self.NOTIFICATIONS:
+                return 600
+            raise NotImplementedError(f"Not defined for: {self}")
+
+    # PK
+    corporation = models.OneToOneField(
+        EveCorporationInfo,
+        primary_key=True,
+        on_delete=models.CASCADE,
+        related_name="structure_owner",
+        verbose_name=_("corporation"),
+        help_text=_("Corporation owning structures"),
     )
-    WAR_WAR_SURRENDER_OFFER_MSG = "WarSurrenderOfferMsg", _("War surrender offered")
-
-    # corporation membership
-    CORP_APP_NEW_MSG = "CorpAppNewMsg", _("Character submitted application")
-    CORP_APP_INVITED_MSG = "CorpAppInvitedMsg", _(
-        "Character invited to join corporation"
+    # regular
+    are_pocos_public = models.BooleanField(
+        default=False,
+        verbose_name=_("are pocos public"),
+        help_text=_("whether pocos of this owner are shown on public POCO page"),
     )
-    CORP_APP_REJECT_CUSTOM_MSG = "CorpAppRejectCustomMsg", _(
-        "Corp application rejected"
+    assets_last_update_at = models.DateTimeField(
+        null=True,
+        default=None,
+        blank=True,
+        verbose_name=_("assets last update at"),
+        help_text=_("when the last successful update happened"),
     )
-    CHAR_APP_WITHDRAW_MSG = "CharAppWithdrawMsg", _("Character withdrew application")
-    CHAR_APP_ACCEPT_MSG = "CharAppAcceptMsg", _("Character joins corporation")
-    CHAR_LEFT_CORP_MSG = "CharLeftCorpMsg", _("Character leaves corporation")
-
-    # billing
-    BILLING_BILL_OUT_OF_MONEY_MSG = "BillOutOfMoneyMsg", _("Bill out of money")
-    BILLING_I_HUB_BILL_ABOUT_TO_EXPIRE = (
-        "InfrastructureHubBillAboutToExpire",
-        _("I-HUB bill about to expire"),
+    character_ownership = models.ForeignKey(
+        CharacterOwnership,
+        on_delete=models.SET_DEFAULT,
+        default=None,
+        null=True,
+        blank=True,
+        related_name="+",
+        help_text="OUTDATED. Has been replaced by OwnerCharacter",  # TODO: Remove
     )
-    BILLING_I_HUB_DESTROYED_BY_BILL_FAILURE = (
-        "IHubDestroyedByBillFailure",
-        _("I_HUB destroyed by bill failure"),
+    forwarding_last_update_at = models.DateTimeField(
+        null=True,
+        default=None,
+        blank=True,
+        verbose_name=_("forwarding last update at"),
+        help_text=_("when the last successful update happened"),
     )
-
-    @classproperty
-    def esi_notifications(cls) -> Set["NotificationType"]:
-        return set(cls.values) - cls.generated_notifications  # type: ignore
-
-    @classproperty
-    def generated_notifications(cls) -> Set["NotificationType"]:
-        return {
-            cls.STRUCTURE_JUMP_FUEL_ALERT,
-            cls.STRUCTURE_REFUELED_EXTRA,
-            cls.TOWER_REFUELED_EXTRA,
-            cls.TOWER_REINFORCED_EXTRA,
-        }
-
-    @classproperty
-    def webhook_defaults(cls) -> List["NotificationType"]:
-        """List of default notifications for new webhooks."""
-        return [
-            cls.STRUCTURE_ANCHORING,
-            cls.STRUCTURE_DESTROYED,
-            cls.STRUCTURE_FUEL_ALERT,
-            cls.STRUCTURE_LOST_ARMOR,
-            cls.STRUCTURE_LOST_SHIELD,
-            cls.STRUCTURE_ONLINE,
-            cls.STRUCTURE_SERVICES_OFFLINE,
-            cls.STRUCTURE_UNDER_ATTACK,
-            cls.STRUCTURE_WENT_HIGH_POWER,
-            cls.STRUCTURE_WENT_LOW_POWER,
-            cls.ORBITAL_ATTACKED,
-            cls.ORBITAL_REINFORCED,
-            cls.TOWER_ALERT_MSG,
-            cls.TOWER_RESOURCE_ALERT_MSG,
-            cls.SOV_STRUCTURE_REINFORCED,
-            cls.SOV_STRUCTURE_DESTROYED,
-        ]
-
-    @classproperty
-    def relevant_for_timerboard(cls) -> Set["NotificationType"]:
-        """Notification types that can create timers."""
-        return {
-            cls.STRUCTURE_LOST_SHIELD,
-            cls.STRUCTURE_LOST_ARMOR,
-            cls.ORBITAL_REINFORCED,
-            cls.MOONMINING_EXTRACTION_STARTED,
-            cls.MOONMINING_EXTRACTION_CANCELLED,
-            cls.SOV_STRUCTURE_REINFORCED,
-            cls.TOWER_REINFORCED_EXTRA,
-        }
-
-    @classproperty
-    def relevant_for_alliance_level(cls) -> Set["NotificationType"]:
-        """Notification types that require the alliance level flag."""
-        return {
-            # billing
-            cls.BILLING_BILL_OUT_OF_MONEY_MSG,
-            cls.BILLING_I_HUB_DESTROYED_BY_BILL_FAILURE,
-            cls.BILLING_I_HUB_BILL_ABOUT_TO_EXPIRE,
-            # sov
-            cls.SOV_ENTOSIS_CAPTURE_STARTED,
-            cls.SOV_COMMAND_NODE_EVENT_STARTED,
-            cls.SOV_ALL_CLAIM_ACQUIRED_MSG,
-            cls.SOV_STRUCTURE_REINFORCED,
-            cls.SOV_STRUCTURE_DESTROYED,
-            cls.SOV_ALL_CLAIM_LOST_MSG,
-            # cls.SOV_ALL_ANCHORING_MSG, # This notif is not broadcasted to all corporations
-            # wars
-            cls.WAR_ALLY_JOINED_WAR_AGGRESSOR_MSG,
-            cls.WAR_ALLY_JOINED_WAR_AllY_MSG,
-            cls.WAR_ALLY_JOINED_WAR_DEFENDER_MSG,
-            cls.WAR_CORP_WAR_SURRENDER_MSG,
-            cls.WAR_CORPORATION_BECAME_ELIGIBLE,
-            cls.WAR_CORPORATION_NO_LONGER_ELIGIBLE,
-            cls.WAR_WAR_ADOPTED,
-            cls.WAR_WAR_DECLARED,
-            cls.WAR_WAR_INHERITED,
-            cls.WAR_WAR_RETRACTED_BY_CONCORD,
-            cls.WAR_WAR_SURRENDER_OFFER_MSG,
-        }
-
-    @classproperty
-    def relevant_for_moonmining(cls) -> Set["NotificationType"]:
-        """Notification types about moon mining."""
-        return {
-            cls.MOONMINING_EXTRACTION_STARTED,
-            cls.MOONMINING_EXTRACTION_CANCELLED,
-            cls.MOONMINING_LASER_FIRED,
-            cls.MOONMINING_EXTRACTION_FINISHED,
-            cls.MOONMINING_AUTOMATIC_FRACTURE,
-        }
-
-    @classproperty
-    def structure_related(cls) -> Set["NotificationType"]:
-        """Notification types that are related to a structure."""
-        return {
-            cls.STRUCTURE_ONLINE,
-            cls.STRUCTURE_FUEL_ALERT,
-            cls.STRUCTURE_JUMP_FUEL_ALERT,
-            cls.STRUCTURE_REFUELED_EXTRA,
-            cls.STRUCTURE_SERVICES_OFFLINE,
-            cls.STRUCTURE_WENT_LOW_POWER,
-            cls.STRUCTURE_WENT_HIGH_POWER,
-            cls.STRUCTURE_UNANCHORING,
-            cls.STRUCTURE_UNDER_ATTACK,
-            cls.STRUCTURE_LOST_SHIELD,
-            cls.STRUCTURE_LOST_ARMOR,
-            cls.STRUCTURE_DESTROYED,
-            cls.OWNERSHIP_TRANSFERRED,
-            cls.STRUCTURE_ANCHORING,
-            cls.MOONMINING_EXTRACTION_STARTED,
-            cls.MOONMINING_EXTRACTION_FINISHED,
-            cls.MOONMINING_AUTOMATIC_FRACTURE,
-            cls.MOONMINING_EXTRACTION_CANCELLED,
-            cls.MOONMINING_LASER_FIRED,
-            cls.STRUCTURE_REINFORCE_CHANGED,
-            cls.ORBITAL_ATTACKED,
-            cls.ORBITAL_REINFORCED,
-            cls.TOWER_ALERT_MSG,
-            cls.TOWER_RESOURCE_ALERT_MSG,
-            cls.TOWER_REFUELED_EXTRA,
-            cls.TOWER_REINFORCED_EXTRA,
-        }
-
-    @classproperty
-    def relevant_for_forwarding(cls) -> Set["NotificationType"]:
-        """Notification types that are forwarded to Discord."""
-        my_set = set(cls.values_enabled)  # type: ignore
-        # if STRUCTURES_NOTIFICATION_DISABLE_ESI_FUEL_ALERTS:
-        #     my_set.discard(cls.STRUCTURE_FUEL_ALERT)
-        #     my_set.discard(cls.TOWER_RESOURCE_ALERT_MSG)
-        return my_set
-
-    @classproperty
-    def values_enabled(cls) -> Set["NotificationType"]:
-        """Values of enabled notif types only."""
-        my_set = set(cls.values)  # type: ignore
-        if not STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS:
-            my_set.discard(cls.STRUCTURE_REFUELED_EXTRA)
-            my_set.discard(cls.TOWER_REFUELED_EXTRA)
-        return my_set
-
-    @classproperty
-    def choices_enabled(cls) -> list:
-        """Choices list containing enabled notif types only."""
-        return [choice for choice in cls.choices if choice[0] in cls.values_enabled]
-
-
-def get_default_notification_types():
-    """DEPRECATED: generates a set of all existing notification types as default.
-    Required to support older migrations."""
-    return tuple(sorted([str(x[0]) for x in NotificationType.values]))
-
-
-class Webhook(WebhookBase):
-    """A destination for forwarding notification alerts."""
-
-    notification_types = MultiSelectField(
-        choices=NotificationType.choices,
-        default=NotificationType.webhook_defaults,
-        verbose_name=_("notification types"),
+    has_default_pings_enabled = models.BooleanField(
+        default=True,
+        verbose_name=_("has default pings enabled"),
         help_text=_(
-            "Select which type of notifications should be forwarded to this webhook"
+            "to enable or disable pinging of notifications for this owner "
+            "e.g. with @everyone and @here"
         ),
     )
-    language_code = models.CharField(
-        max_length=8,
-        choices=LANGUAGES,
-        default=None,
-        null=True,
-        blank=True,
-        verbose_name=_("language"),
-        help_text=_("language of notifications send to this webhook"),
+    is_active = models.BooleanField(
+        default=True,
+        verbose_name=_("is active"),
+        help_text=_("whether this owner is currently included in the sync process"),
     )
-    is_default = models.BooleanField(
+    is_alliance_main = models.BooleanField(
         default=False,
-        verbose_name=_("is default"),
+        verbose_name=_("is alliance main"),
         help_text=_(
-            "Whether owners have this webhook automatically pre-set when created"
+            "whether alliance wide notifications "
+            "are forwarded for this owner (e.g. sov notifications)"
         ),
     )
-    has_default_pings_enabled = models.BooleanField(
+    is_included_in_service_status = models.BooleanField(
         default=True,
-        verbose_name=_("has default pings enabled"),
-        help_text=(
-            "To enable or disable pinging of notifications for this webhook "
-            "e.g. with @everyone and @here"
+        verbose_name=_("is included in service status"),
+        help_text=_(
+            "whether the sync status of this owner is included in "
+            "the overall status of this services"
         ),
     )
+    is_up = models.BooleanField(
+        null=True,
+        default=None,
+        editable=False,
+        verbose_name=_("is up"),
+        help_text=_("whether all services for this owner are currently up"),
+    )
+    notifications_last_update_at = models.DateTimeField(
+        null=True,
+        default=None,
+        blank=True,
+        verbose_name=_("notifications last update at"),
+        help_text=_("when the last successful update happened"),
+    )
     ping_groups = models.ManyToManyField(
         Group,
         default=None,
         blank=True,
         related_name="+",
         verbose_name=_("ping groups"),
-        help_text=_("Groups to be pinged for each notification - "),
+        help_text=_("Groups to be pinged for each notification. "),
     )
-    objects = WebhookManager()
-
-    class Meta:
-        verbose_name = _("webhook")
-        verbose_name_plural = _("webhooks")
-
-    @staticmethod
-    def text_bold(text) -> str:
-        """Format the given text in bold."""
-        return f"**{text}**" if text else ""
-
-
-class NotificationBase(models.Model):
-    """Base model for a notification."""
-
-    is_sent = models.BooleanField(
-        default=False,
-        verbose_name=_("is sent"),
-        help_text=_("True when this notification has been forwarded to Discord"),
-    )
-    is_timer_added = models.BooleanField(
+    structures_last_update_at = models.DateTimeField(
         null=True,
-        default=False,
-        verbose_name=_("is timer added"),
-        help_text=_("True when a timer has been added for this notification"),
-    )
-    notif_type = models.CharField(
-        max_length=100,
-        default="",
-        db_index=True,
-        verbose_name=_("type"),
-        help_text=_("type of this notification"),
-    )
-    owner = models.ForeignKey(
-        "Owner",
-        on_delete=models.CASCADE,
-        verbose_name=_("owner"),
-        help_text=_("Corporation that owns this notification"),
+        default=None,
+        blank=True,
+        verbose_name=_("structures last update at"),
+        help_text=_("when the last successful update happened"),
     )
-    structures = models.ManyToManyField(
-        Structure,
-        verbose_name=_("structures"),
-        help_text=_("Structures this notification is about (if any)"),
+    webhooks = models.ManyToManyField(
+        "Webhook",
+        default=None,
+        blank=True,
+        related_name="owners",
+        verbose_name=_("webhooks"),
+        help_text=_("Notifications are sent to these webhooks."),
     )
 
-    class Meta:
-        abstract = True
+    objects = OwnerManager()
 
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-        self._ping_type_override = None
-        self._color_override = None
+    class Meta:
+        verbose_name = _("owner")
+        verbose_name_plural = _("owners")
 
     def __str__(self) -> str:
-        return f"{self.notification_id}:{self.notif_type}"
+        return str(self.corporation.corporation_name)
 
-    def __repr__(self) -> str:
-        return "%s(notification_id=%d, owner='%s', notif_type='%s')" % (
-            self.__class__.__name__,
-            self.notification_id,
-            self.owner,
-            self.notif_type,
+    def __repr__(self):
+        return (
+            f"{self.__class__.__name__}(pk={self.pk}, corporation='{self.corporation}')"
         )
 
-    @property
-    def is_alliance_level(self) -> bool:
-        """Whether this is an alliance level notification."""
-        return self.notif_type in NotificationType.relevant_for_alliance_level
+    def save(self, *args, **kwargs) -> None:
+        if self.is_alliance_main:
+            Owner.objects.filter(
+                corporation__alliance_id=self.corporation.alliance_id
+            ).exclude(corporation__alliance_id__isnull=True).update(
+                is_alliance_main=False
+            )
+            if "update_fields" in kwargs:
+                kwargs["update_fields"].append("is_alliance_main")
+        super().save(*args, **kwargs)
 
     @property
-    def can_be_rendered(self) -> bool:
-        """Whether this notification can be rendered in Discord."""
-        return self.notif_type in NotificationType.values
+    def is_structure_sync_fresh(self) -> bool:
+        """True if last sync happened with grace time, else False."""
+        return bool(
+            self.structures_last_update_at
+        ) and self.structures_last_update_at > (
+            now() - dt.timedelta(minutes=STRUCTURES_STRUCTURE_SYNC_GRACE_MINUTES)
+        )
 
     @property
-    def can_have_timer(self) -> bool:
-        """Whether this notification can have a timer."""
-        return self.notif_type in NotificationType.relevant_for_timerboard
+    def is_notification_sync_fresh(self) -> bool:
+        """True if last sync happened with grace time, else False."""
+        return bool(
+            self.notifications_last_update_at
+        ) and self.notifications_last_update_at > (
+            now() - dt.timedelta(minutes=STRUCTURES_NOTIFICATION_SYNC_GRACE_MINUTES)
+        )
 
     @property
-    def is_structure_related(self) -> bool:
-        """Weather this notification related to a structure."""
-        return self.notif_type in NotificationType.structure_related
+    def is_forwarding_sync_fresh(self) -> bool:
+        """True if last sync happened with grace time, else False."""
+        return bool(
+            self.forwarding_last_update_at
+        ) and self.forwarding_last_update_at > (
+            now() - dt.timedelta(minutes=STRUCTURES_NOTIFICATION_SYNC_GRACE_MINUTES)
+        )
 
     @property
-    def is_temporary(self) -> bool:
-        raise NotImplementedError()
-
-    def is_npc_attacking(self) -> bool:
-        raise NotImplementedError()
-
-    def parsed_text(self) -> dict:
-        raise NotImplementedError()
+    def is_assets_sync_fresh(self) -> bool:
+        """True if last sync happened with grace time, else False."""
+        return bool(self.assets_last_update_at) and self.assets_last_update_at > (
+            now() - dt.timedelta(minutes=STRUCTURES_STRUCTURE_SYNC_GRACE_MINUTES)
+        )
 
-    def send_to_configured_webhooks(
-        self,
-        ping_type_override: Optional[Union[Webhook.PingType, str]] = None,
-        use_color_override: bool = False,
-        color_override: Optional[int] = None,
-    ) -> Optional[bool]:
-        """Send this notification to all active webhooks which have this
-        notification type configured
-        and apply filter for NPC attacks and alliance level if needed.
-
-        Returns True, if notifications has been successfully send to webhooks
-        Returns None, if owner has no fitting webhook
-        Returns False, if sending to any webhooks failed
+    @property
+    def are_all_syncs_ok(self) -> bool:
+        """returns true if they have been no errors
+        and last syncing occurred within alloted time for all sync categories
         """
-        if self.filter_for_npc_attacks():
-            logger.debug("%s: Will not send NPC attacks", self)
-            return None
-        if self.filter_for_alliance_level():
-            logger.debug(
-                "%s: Alliance level notifications are not enabled for this owner", self
-            )
-            return None
-        webhooks_qs = self.relevant_webhooks()
-        if not webhooks_qs.exists():
-            logger.debug("%s: No relevant webhook found", self)
-            return None
-        if ping_type_override:
-            self._ping_type_override = Webhook.PingType(ping_type_override)
-        if use_color_override:
-            self._color_override = color_override
-        success = True
-        for webhook in webhooks_qs:
-            success &= self.send_to_webhook(webhook)
-        return success
-
-    def filter_for_npc_attacks(self) -> bool:
-        """True when notification to be filtered out due to npc attacks."""
-        return not STRUCTURES_REPORT_NPC_ATTACKS and self.is_npc_attacking()
-
-    def filter_for_alliance_level(self) -> bool:
-        """True when notification to be filtered out due to alliance level."""
         return (
-            self.is_alliance_level
-            and self.owner.corporation.alliance is not None
-            and not self.owner.is_alliance_main
+            self.is_structure_sync_fresh
+            and self.is_notification_sync_fresh
+            and self.is_forwarding_sync_fresh
+            and self.is_assets_sync_fresh
         )
 
-    def relevant_webhooks(self) -> models.QuerySet:
-        """Determine relevant webhooks matching this notification type."""
-        if not self.is_structure_related:
-            structures_qs = Structure.objects.none()
-        else:
-            structures_qs = self.calc_related_structures()
+    def update_is_up(self) -> bool:
+        """Check if all services for this owner are up, notify admins if necessary
+        and store result.
+        """
+
+        def fresh_str(value: bool) -> str:
+            return "up" if value else "down"
+
+        is_up = self.are_all_syncs_ok
         if (
-            structures_qs.exists()
-            and structures_qs.filter(webhooks__isnull=False).count() == 1
+            STRUCTURES_ADMIN_NOTIFICATIONS_ENABLED
+            and self.is_included_in_service_status
         ):
-            webhooks_qs = structures_qs.first().webhooks.filter(
-                notification_types__contains=self.notif_type, is_active=True
-            )
-        else:
-            webhooks_qs = self.owner.webhooks.filter(
-                notification_types__contains=self.notif_type, is_active=True
+            if self.is_up and is_up is False:
+                title = f"{__title__}: Services are down for {self}"
+                msg = (
+                    f"Structure services for {self} are down. "
+                    "Admin action is likely required to restore services.\n"
+                    f"- Structures: {fresh_str(self.is_structure_sync_fresh)}\n"
+                    f"- Notifications: {fresh_str(self.is_notification_sync_fresh)}\n"
+                    f"- Forwarding: {fresh_str(self.is_forwarding_sync_fresh)}\n"
+                    f"- Assets: {fresh_str(self.is_assets_sync_fresh)}\n"
+                )
+                notify_admins(message=msg, title=title, level="danger")
+            elif self.is_up is False and is_up:
+                title = f"{__title__}: Services restored for {self}"
+                msg = f"Structure services for {self} have been restored. "
+                notify_admins(message=msg, title=title, level="success")
+            elif self.is_up is None and is_up:
+                title = f"{__title__}: Services enabled {self}"
+                msg = f"Structure services for {self} have been enabled. "
+                notify_admins(message=msg, title=title, level="success")
+        if self.is_up != is_up:
+            self.is_up = is_up
+            self.save(update_fields=["is_up"])
+        return is_up
+
+    def add_character(
+        self, character_ownership: CharacterOwnership
+    ) -> "OwnerCharacter":
+        """Add character to this owner.
+
+        Raises ValueError when character does not belong to owner's corporation.
+        """
+        if (
+            character_ownership.character.corporation_id
+            != self.corporation.corporation_id
+        ):
+            raise ValueError(
+                f"Character {character_ownership.character} does not belong "
+                "to owner corporation."
             )
-        return webhooks_qs
+        obj, _ = self.characters.get_or_create(character_ownership=character_ownership)
+        return obj
 
-    def calc_related_structures(self) -> models.QuerySet[Structure]:
-        """Identify structures this notification is related to.
+    def characters_count(self) -> int:
+        """Count of valid owner characters."""
+        return self.characters.count()
+
+    def has_sov(self, eve_solar_system: EveSolarSystem) -> bool:
+        """Determine whether this owner has sov in the given solar system."""
+        return EveSovereigntyMap.objects.corporation_has_sov(
+            eve_solar_system=eve_solar_system, corporation=self.corporation
+        )
 
-        Returns:
-        - structures if any found or empty list if there are no related structures
+    def delete_character(
+        self,
+        character: "OwnerCharacter",
+        error: str,
+        level: str = "warning",
+        max_allowed_errors: int = 0,
+    ) -> None:
+        """Delete character and notify it's owner and admin about the reason
+
+        Args:
+        - character: Character this error refers to
+        - error: Error text
+        - level: context level for the notification
+        - max_error: how many errors are permitted before character is deleted
         """
-        parsed_text = self.parsed_text()
-        if not parsed_text:
-            return Structure.objects.none()
-        if self.notif_type in {
-            NotificationType.STRUCTURE_ONLINE,
-            NotificationType.STRUCTURE_FUEL_ALERT,
-            NotificationType.STRUCTURE_JUMP_FUEL_ALERT,
-            NotificationType.STRUCTURE_REFUELED_EXTRA,
-            NotificationType.STRUCTURE_SERVICES_OFFLINE,
-            NotificationType.STRUCTURE_WENT_LOW_POWER,
-            NotificationType.STRUCTURE_WENT_HIGH_POWER,
-            NotificationType.STRUCTURE_UNANCHORING,
-            NotificationType.STRUCTURE_UNDER_ATTACK,
-            NotificationType.STRUCTURE_LOST_SHIELD,
-            NotificationType.STRUCTURE_LOST_ARMOR,
-            NotificationType.STRUCTURE_DESTROYED,
-            NotificationType.OWNERSHIP_TRANSFERRED,
-            NotificationType.STRUCTURE_ANCHORING,
-            NotificationType.MOONMINING_EXTRACTION_STARTED,
-            NotificationType.MOONMINING_EXTRACTION_FINISHED,
-            NotificationType.MOONMINING_AUTOMATIC_FRACTURE,
-            NotificationType.MOONMINING_EXTRACTION_CANCELLED,
-            NotificationType.MOONMINING_LASER_FIRED,
-        }:
-            structure_id = parsed_text.get("structureID")
-            return Structure.objects.filter(id=structure_id)
-        elif self.notif_type == NotificationType.STRUCTURE_REINFORCE_CHANGED:
-            structure_ids = [
-                structure_info[0] for structure_info in parsed_text["allStructureInfo"]
-            ]
-            return Structure.objects.filter(id__in=structure_ids)
-
-        elif self.notif_type in {
-            NotificationType.ORBITAL_ATTACKED,
-            NotificationType.ORBITAL_REINFORCED,
-        }:
-            return Structure.objects.filter(
-                eve_planet_id=parsed_text["planetID"], eve_type_id=parsed_text["typeID"]
-            )
-
-        elif self.notif_type in {
-            NotificationType.TOWER_ALERT_MSG,
-            NotificationType.TOWER_RESOURCE_ALERT_MSG,
-            NotificationType.TOWER_REFUELED_EXTRA,
-        }:
-            return Structure.objects.filter(
-                eve_moon_id=parsed_text["moonID"], eve_type_id=parsed_text["typeID"]
+        if character.error_count < max_allowed_errors:
+            logger.warning(
+                (
+                    "%s: Character encountered an error and will be deleted "
+                    "if this occurs more often (%d/%d): %s"
+                ),
+                character,
+                character.error_count + 1,
+                max_allowed_errors,
+                error,
             )
-        return Structure.objects.none()
-
-    def send_to_webhook(self, webhook: Webhook) -> bool:
-        """Sends this notification to the configured webhook.
+            with transaction.atomic():
+                character.error_count = F("error_count") + 1
+                character.save(update_fields=["error_count"])
+            return
+
+        title = f"{__title__}: {self}: Invalid character has been removed"
+        message = (
+            f"{character.character_ownership}: {error}\n"
+            "The character has been removed. "
+            "Please add a new character to restore the previous service level."
+        )
+        notify(
+            user=character.character_ownership.user,
+            title=title,
+            message=message,
+            level=level,
+        )
+        if self.characters.count() == 1:
+            message += (
+                " This owner has no configured characters anymore "
+                "and it's services are now down."
+            )
+            level = "danger"
+        notify_admins(title=f"FYI: {title}", message=message, level=level)
+        character.delete()
 
-        returns True if successful, else False
+    def _rotate_character(
+        self,
+        character: "OwnerCharacter",
+        ignore_schedule: bool,
+        rotate_characters: RotateCharactersType,
+    ) -> None:
+        """Rotate this character such that all are spread evenly
+        across the ESI cache duration for each ESI call.
         """
-        logger.info("%s: Trying to sent to webhook: %s", self, webhook)
+        time_since_last_used = (
+            (
+                now() - getattr(character, rotate_characters.last_used_at_name)
+            ).total_seconds()
+            if getattr(character, rotate_characters.last_used_at_name)
+            else None
+        )
         try:
-            embed, ping_type = self._generate_embed(webhook.language_code)
-        except (OSError, NotImplementedError) as ex:
-            logger.warning("%s: Failed to generate embed: %s", self, ex, exc_info=True)
-            return False
-        if webhook.has_default_pings_enabled and self.owner.has_default_pings_enabled:
-            if ping_type == Webhook.PingType.EVERYONE:
-                content = "@everyone"
-            elif ping_type == Webhook.PingType.HERE:
-                content = "@here"
-            else:
-                content = ""
-        else:
-            content = ""
-        if webhook.ping_groups.count() > 0 or self.owner.ping_groups.count() > 0:
-            if "discord" in app_labels():
-                DiscordUser = self._import_discord()
+            minimum_time_between_rotations = max(
+                rotate_characters.esi_cache_duration / self.characters.count(),
+                60,
+            )
+        except ZeroDivisionError:
+            minimum_time_between_rotations = rotate_characters.esi_cache_duration
+        if (
+            ignore_schedule
+            or not time_since_last_used
+            or time_since_last_used >= minimum_time_between_rotations
+        ):
+            setattr(character, rotate_characters.last_used_at_name, now())
+            character.save()
+
+    def fetch_token(
+        self,
+        rotate_characters: Optional[RotateCharactersType] = None,
+        ignore_schedule: bool = False,
+    ) -> Token:
+        """Fetch a valid token for the owner and return it.
+
+        Args:
+            rotate_characters: For which sync type to rotate through characters \
+                with every new call
+            ignore_schedule: Ignore current schedule when rotating
 
-                groups = set(self.owner.ping_groups.all()) | set(
-                    webhook.ping_groups.all()
+        Raises TokenError when no valid token can be provided.
+        """
+        order_by_last_used = (
+            rotate_characters.last_used_at_name
+            if rotate_characters
+            else "notifications_last_used_at"
+        )
+        for character in self.characters.order_by(order_by_last_used):
+            if (
+                character.character_ownership.character.corporation_id
+                != self.corporation.corporation_id
+            ):
+                self.delete_character(
+                    character=character,
+                    error="Character does no longer belong to the owner's corporation.",
                 )
-                for group in groups:
-                    try:
-                        role = DiscordUser.objects.group_to_role(group)
-                    except HTTPError:
-                        logger.warning("Failed to get Discord roles", exc_info=True)
-                    else:
-                        if role:
-                            content += f" <@&{role['id']}>"
-
-        username, avatar_url = self._gen_avatar()
-        new_queue_size = webhook.send_message(
-            content=content, embeds=[embed], username=username, avatar_url=avatar_url
-        )
-        success = new_queue_size > 0
-        if success and not self.is_temporary:
-            self.is_sent = True
-            self.save()
-        return success
-
-    def _generate_embed(
-        self, language_code: Optional[str]
-    ) -> Tuple[dhooks_lite.Embed, Optional[Webhook.PingType]]:
-        """Generates a Discord embed for this notification."""
-        from ..core.notification_embeds import NotificationBaseEmbed
-
-        logger.info("Creating embed with language = %s" % language_code)
-        with translation.override(language_code):
-            notification_embed = NotificationBaseEmbed.create(self)
-            embed = notification_embed.generate_embed()
-            return embed, notification_embed.ping_type
+                continue
 
-    @staticmethod
-    def _import_discord() -> object:
-        from allianceauth.services.modules.discord.models import DiscordUser
+            if not character.character_ownership.user.has_perm(
+                "structures.add_structure_owner"
+            ):
+                self.delete_character(
+                    character=character,
+                    error="Character does not have sufficient permission to sync.",
+                )
+                continue
 
-        return DiscordUser
+            token = character.valid_token()
+            if not token:
+                self.delete_character(
+                    character=character,
+                    error="Character has no valid token for sync.",
+                )
+                continue
+            found_character = character
+            break  # leave the for loop if we have found a valid token
 
-    def _gen_avatar(self) -> Tuple[Optional[str], Optional[str]]:
-        if STRUCTURES_NOTIFICATION_SET_AVATAR:
-            username = "Notifications"
-            avatar_url = static_file_absolute_url("structures/img/structures_logo.png")
         else:
-            username = None
-            avatar_url = None
-        return username, avatar_url
+            raise TokenError(
+                f"{self}: No valid character found for sync. "
+                "Service down for this owner."
+            )
 
-    def add_or_remove_timer(self) -> bool:
-        """Add/remove a timer related to this notification for some types.
+        if rotate_characters:
+            self._rotate_character(
+                character=found_character,
+                ignore_schedule=ignore_schedule,
+                rotate_characters=rotate_characters,
+            )
+        return token
 
-        Returns True when timers where added or removed, else False
-        """
-        if (
-            not STRUCTURES_ADD_TIMERS
-            or self.notif_type not in NotificationType.relevant_for_timerboard
-        ):
-            return False
+    def _report_esi_issue(self, action: str, ex: Exception, token: Token):
+        """Report an ESI issue to admins."""
+        message = f"{self}: Failed to {action} from ESI with token {token} due to {ex}"
+        logger.warning(message, exc_info=True)
+
+    def update_structures_esi(self, user: Optional[User] = None):
+        """Updates all structures from ESI."""
+        token = self.fetch_token(rotate_characters=self.RotateCharactersType.STRUCTURES)
+        is_ok = self._fetch_upwell_structures(token)
+        if STRUCTURES_FEATURE_CUSTOMS_OFFICES:
+            is_ok &= self._fetch_custom_offices(token)
+        if STRUCTURES_FEATURE_STARBASES:
+            is_ok &= self._fetch_starbases(token)
+
+        if is_ok:
+            self.structures_last_update_at = now()
+            self.save(update_fields=["structures_last_update_at"])
+            if user:
+                self._send_report_to_user(
+                    topic="structures", topic_count=self.structures.count(), user=user
+                )
 
-        from ..core import notification_timers
+    def _remove_structures_not_returned_from_esi(
+        self, structures_qs: models.QuerySet, new_structures: Iterable
+    ):
+        """Remove structures no longer returned from ESI."""
+        ids_local = {x.id for x in structures_qs}
+        ids_from_esi = {x["structure_id"] for x in new_structures}
+        ids_to_remove = ids_local - ids_from_esi
+        if len(ids_to_remove) > 0:
+            structures_qs.filter(id__in=ids_to_remove).delete()
+            logger.info(
+                "Removed %d structures which apparently no longer exist.",
+                len(ids_to_remove),
+            )
 
+    def _fetch_locations_for_assets(
+        self, item_ids: Iterable[int], token: Token
+    ) -> dict:
+        """Fetch locations for given asset items from ESI."""
+        item_ids = list(item_ids)
+        logger.info(
+            "%s: Fetching locations for %d assets from ESI", self, len(item_ids)
+        )
+        locations_data = []
+        for item_ids_chunk in chunks(item_ids, 999):
+            try:
+                locations_data_chunk = (
+                    esi.client.Assets.post_corporations_corporation_id_assets_locations(
+                        corporation_id=self.corporation.corporation_id,
+                        item_ids=item_ids_chunk,
+                        token=token.valid_access_token(),
+                    )
+                ).results()
+            except HTTPNotFound:
+                pass
+            else:
+                locations_data += locations_data_chunk
+        positions = {x["item_id"]: x["position"] for x in locations_data}
+        return positions
+
+    def _fetch_upwell_structures(self, token: Token) -> bool:
+        """Fetch Upwell structures from ESI for self.
+
+        Return True if successful, else False.
+        """
+        is_ok = True
+        # fetch main list of structure for this corporation
         try:
-            with translation.override(STRUCTURES_DEFAULT_LANGUAGE):
-                return notification_timers.add_or_remove_timer(self)
+            structures = (
+                esi.client.Corporation.get_corporations_corporation_id_structures(
+                    corporation_id=self.corporation.corporation_id,
+                    token=token.valid_access_token(),
+                ).results()
+            )
         except OSError as ex:
-            logger.warning(
-                "%s: Failed to add timer from notification: %s",
+            self._report_esi_issue("fetch corporation structures", ex, token)
+            return False
+
+        # fetch additional information for structures
+        if not structures:
+            logger.info("%s: No Upwell structures retrieved from ESI", self)
+        else:
+            logger.info(
+                "%s: Fetching additional infos for %d Upwell structures from ESI",
                 self,
-                ex,
-                exc_info=True,
+                len(structures),
             )
-        return False
+            for structure in structures:
+                try:
+                    structure_info = (
+                        esi.client.Universe.get_universe_structures_structure_id(
+                            structure_id=structure["structure_id"],
+                            token=token.valid_access_token(),
+                        )
+                    ).results()
+                except OSError as ex:
+                    self._report_esi_issue(
+                        f"fetch structure #{structure['structure_id']}", ex, token
+                    )
+                    structure["name"] = "(no data)"
+                    is_ok = False
+                else:
+                    structure["name"] = Structure.extract_name_from_esi_response(
+                        structure_info["name"]
+                    )
+                    structure["position"] = structure_info["position"]
 
+            logger.info(
+                "%s: Storing updates for %d upwell structures",
+                self,
+                len(structures),
+            )
+            for structure in structures:
+                try:
+                    Structure.objects.update_or_create_from_dict(structure, self)
+                except OSError:
+                    logger.warning(
+                        "%s: Failed to store update for structure with ID %s",
+                        self,
+                        structure["structure_id"],
+                    )
+                    is_ok = False
 
-class Notification(NotificationBase):
-    """A notification in Eve Online.
+        if STRUCTURES_DEVELOPER_MODE:
+            self._store_raw_data("structures", structures)
 
-    Notifications are usually created from Eve Online notifications received from ESI,
-    but they can also be generated directly by Structures.
-    """
+        self._remove_structures_not_returned_from_esi(
+            structures_qs=self.structures.filter_upwell_structures(),
+            new_structures=structures,
+        )
+        return is_ok
 
-    TEMPORARY_NOTIFICATION_ID = 999999999999
+    def _fetch_custom_offices(self, token: Token) -> bool:
+        """Fetch custom offices from ESI for this owner.
 
-    notification_id = models.PositiveBigIntegerField(verbose_name=_("id"))
-    created = models.DateTimeField(
-        null=True,
-        default=None,
-        verbose_name=_("created"),
-        help_text=_("Date when this notification was first received from ESI"),
-    )
-    is_read = models.BooleanField(
-        null=True,
-        default=None,
-        verbose_name=_("is read"),
-        help_text=_("True when this notification has read in the eve client"),
-    )
-    last_updated = models.DateTimeField(
-        verbose_name=_("last updated"),
-        help_text=_("Date when this notification has last been updated from ESI"),
-    )
-    sender = models.ForeignKey(
-        EveEntity,
-        on_delete=models.SET_NULL,
-        null=True,
-        related_name="+",
-        verbose_name=_("sender"),
-    )
+        Return True when successful, else False.
+        """
+        structures = {}
+        try:
+            pocos = esi.client.Planetary_Interaction.get_corporations_corporation_id_customs_offices(
+                corporation_id=self.corporation.corporation_id,
+                token=token.valid_access_token(),
+            ).results()
 
-    text = models.TextField(
-        null=True,
-        default=None,
-        blank=True,
-        verbose_name=_("text"),
-        help_text=_("Notification details in YAML"),
-    )
-    timestamp = models.DateTimeField(db_index=True, verbose_name=_("timestamp"))
+            if not pocos:
+                logger.info("%s: No custom offices retrieved from ESI", self)
 
-    objects = NotificationManager()
+            else:
+                pocos_2 = {row["office_id"]: row for row in pocos}
+                office_ids = list(pocos_2.keys())
+                positions = self._fetch_locations_for_assets(office_ids, token)
+                names = self._fetch_names_for_pocos(office_ids, token)
+
+                # making sure we have all solar systems loaded
+                # incl. their planets for later name matching
+                for solar_system_id in {int(x["system_id"]) for x in pocos}:
+                    EveSolarSystem.objects.get_or_create_esi(id=solar_system_id)
 
-    class Meta:
-        verbose_name = _("eve notification")
-        verbose_name_plural = _("eve notifications")
-        unique_together = (("notification_id", "owner"),)
+                structures.update(
+                    self._compile_pocos_for_structures(pocos_2, positions, names)
+                )
 
-    def save(self, *args, **kwargs) -> None:
-        if self.is_temporary:
-            raise ValueError("Temporary notifications can not be saved")
-        super().save(*args, **kwargs)
+                self._store_poco_details(structures, pocos_2)
 
-    @property
-    def is_temporary(self) -> bool:
-        """True when this notification is temporary."""
-        return self.notification_id == self.TEMPORARY_NOTIFICATION_ID
+            if STRUCTURES_DEVELOPER_MODE:
+                self._store_raw_data("customs_offices", structures)
 
-    @property
-    def is_generated(self) -> bool:
-        return self.is_temporary
+        except OSError as ex:
+            self._report_esi_issue("fetch custom offices", ex, token)
+            return False
 
-    # @classmethod
-    # def get_all_types(cls) -> Set[int]:
-    #     """returns a set with all supported notification types"""
-    #     return {x[0] for x in NotificationType.choices}
-
-    def parsed_text(self) -> dict:
-        """Returns the notifications's text as dict."""
-        return yaml.safe_load(self.text) if self.text else {}
-
-    def is_npc_attacking(self) -> bool:
-        """Whether this notification is about a NPC attacking."""
-        if self.notif_type in [
-            NotificationType.ORBITAL_ATTACKED,
-            NotificationType.STRUCTURE_UNDER_ATTACK,
-        ]:
-            parsed_text = self.parsed_text()
-            corporation_id = None
-            if self.notif_type == NotificationType.STRUCTURE_UNDER_ATTACK:
-                if (
-                    "corpLinkData" in parsed_text
-                    and len(parsed_text["corpLinkData"]) >= 3
-                ):
-                    corporation_id = int(parsed_text["corpLinkData"][2])
-            if self.notif_type == NotificationType.ORBITAL_ATTACKED:
-                if "aggressorCorpID" in parsed_text:
-                    corporation_id = int(parsed_text["aggressorCorpID"])
-            if corporation_id:
-                corporation = EveEntity(
-                    category=EveEntity.CATEGORY_CORPORATION, id=corporation_id
+        self._remove_structures_not_returned_from_esi(
+            structures_qs=self.structures.filter_customs_offices(),
+            new_structures=structures.values(),
+        )
+        return True
+
+    def _store_poco_details(self, structures: dict, pocos_2: dict):
+        logger.info("%s: Storing updates for %d customs offices", self, len(structures))
+        for office_id, structure in structures.items():
+            try:
+                poco = pocos_2[office_id]
+            except KeyError:
+                logger.warning(
+                    "%s: No details found for this POCO: %d", self, office_id
                 )
-                return corporation.is_npc and not corporation.is_npc_starter_corporation
-        return False
+                continue
 
-    def update_related_structures(self) -> bool:
-        """Update related structure for this notification.
+            standing_level = PocoDetails.StandingLevel.from_esi(
+                poco.get("standing_level")
+            )
+            structure_obj, _ = Structure.objects.update_or_create_from_dict(
+                structure, self
+            )
+            PocoDetails.objects.update_or_create(
+                structure=structure_obj,
+                defaults={
+                    "alliance_tax_rate": poco.get("alliance_tax_rate"),
+                    "allow_access_with_standings": poco.get(
+                        "allow_access_with_standings"
+                    ),
+                    "allow_alliance_access": poco.get("allow_alliance_access"),
+                    "bad_standing_tax_rate": poco.get("bad_standing_tax_rate"),
+                    "corporation_tax_rate": poco.get("corporation_tax_rate"),
+                    "excellent_standing_tax_rate": poco.get(
+                        "excellent_standing_tax_rate"
+                    ),
+                    "good_standing_tax_rate": poco.get("good_standing_tax_rate"),
+                    "neutral_standing_tax_rate": poco.get("neutral_standing_tax_rate"),
+                    "reinforce_exit_end": poco.get("reinforce_exit_end"),
+                    "reinforce_exit_start": poco.get("reinforce_exit_start"),
+                    "standing_level": standing_level,
+                    "terrible_standing_tax_rate": poco.get(
+                        "terrible_standing_tax_rate"
+                    ),
+                },
+            )
 
-        Returns True if structures where updated, else False.
-        """
-        structures_qs = self.calc_related_structures()
-        self.structures.clear()
-        if structures_qs.exists():
-            objs = [obj for obj in structures_qs.all()]
-            self.structures.add(*objs)
-            return True
-        return False
-
-    @classmethod
-    def create_from_structure(
-        cls, structure: Structure, notif_type: NotificationType, **kwargs
-    ) -> "Notification":
-        """Create new notification from given structure."""
-        if "timestamp" not in kwargs:
-            kwargs["timestamp"] = now()
-        if "last_updated" not in kwargs:
-            kwargs["last_updated"] = now()
-        threshold = kwargs.pop("threshold") if "threshold" in kwargs else None
-        if "text" not in kwargs:
-            if notif_type in {
-                NotificationType.STRUCTURE_FUEL_ALERT,
-                NotificationType.STRUCTURE_REFUELED_EXTRA,
-                NotificationType.STRUCTURE_JUMP_FUEL_ALERT,
-            }:
-                data = {
-                    "solarsystemID": structure.eve_solar_system_id,
-                    "structureID": structure.id,
-                    "structureTypeID": structure.eve_type_id,
-                    "threshold": threshold,
-                }
-            elif notif_type in {
-                NotificationType.TOWER_RESOURCE_ALERT_MSG,
-                NotificationType.TOWER_REFUELED_EXTRA,
-            }:
-                data = {
-                    "moonID": structure.eve_moon_id,
-                    "typeID": structure.eve_type_id,
-                    "structureID": structure.id,
-                }
+    def _compile_pocos_for_structures(self, pocos_2, positions, names) -> dict:
+        structures = {}
+        for office_id, poco in pocos_2.items():
+            planet_name = names.get(office_id, "")
+            if planet_name:
+                try:
+                    eve_planet = EvePlanet.objects.get(name=planet_name)
+                except EvePlanet.DoesNotExist:
+                    name = ""
+                    planet_id = None
+                else:
+                    planet_id = eve_planet.id
+                    name = eve_planet.eve_type.name
             else:
-                raise ValueError("text property not provided and can not be generated.")
-            kwargs["text"] = yaml.dump(data)
-        if "sender" not in kwargs:
-            sender, _ = EveEntity.objects.get_or_create_esi(id=EveCorporationId.DED)
-            kwargs["sender"] = sender
-        kwargs["notification_id"] = cls.TEMPORARY_NOTIFICATION_ID
-        kwargs["owner"] = structure.owner
-        kwargs["notif_type"] = notif_type
-        return cls(**kwargs)
-
-
-class GeneratedNotification(NotificationBase):
-    """A notification generated by the Structures app, not by Eve Online."""
-
-    details = models.JSONField(default=dict, verbose_name=_("details"))
-    last_updated = models.DateTimeField(auto_now=True, verbose_name=_("last_updated"))
-    timestamp = models.DateTimeField(auto_now_add=True, verbose_name=_("timestamp"))
+                name = None
+                planet_id = None
 
-    objects = GeneratedNotificationManager()
-
-    class Meta:
-        verbose_name = _("generated notification")
-        verbose_name_plural = _("generated  notifications")
+            reinforce_exit_start = dt.datetime(
+                year=2000, month=1, day=1, hour=poco["reinforce_exit_start"]
+            )
+            reinforce_hour = reinforce_exit_start + dt.timedelta(hours=1)
+            structure = {
+                "structure_id": office_id,
+                "type_id": EveTypeId.CUSTOMS_OFFICE,
+                "corporation_id": self.corporation.corporation_id,
+                "name": name if name else "",
+                "system_id": poco["system_id"],
+                "reinforce_hour": reinforce_hour.hour,
+                "state": Structure.State.UNKNOWN,
+            }
+            if planet_id:
+                structure["planet_id"] = planet_id
+
+            if office_id in positions:
+                structure["position"] = positions[office_id]
+
+            structures[office_id] = structure
+
+        return structures
+
+    def _fetch_names_for_pocos(self, item_ids: list, token: Token) -> dict:
+        logger.info(
+            "%s: Fetching names for %d custom office names from ESI",
+            self,
+            len(item_ids),
+        )
+        names_data = []
+        for item_ids_chunk in chunks(item_ids, 999):
+            try:
+                names_data_chunk = (
+                    esi.client.Assets.post_corporations_corporation_id_assets_names(
+                        corporation_id=self.corporation.corporation_id,
+                        item_ids=item_ids_chunk,
+                        token=token.valid_access_token(),
+                    )
+                ).results()
+            except HTTPNotFound:
+                pass
+            else:
+                names_data += names_data_chunk
+        names = {x["item_id"]: self._extract_planet_name(x["name"]) for x in names_data}
+        return names
 
-    @property
-    def notification_id(self) -> int:
-        return self.pk
+    @staticmethod
+    def _extract_planet_name(text: str) -> str:
+        """Extract name of planet from assert name for a customs office."""
+        reg_ex = re.compile(r"Customs Office \((.+)\)")
+        matches = reg_ex.match(text)
+        return matches.group(1) if matches else ""
 
-    @property
-    def is_temporary(self) -> bool:
-        return False
+    def _fetch_starbases(self, token: Token) -> bool:
+        """Fetch starbases from ESI for this owner.
 
-    @property
-    def is_generated(self) -> bool:
-        return True
+        Return True when successful, else False.
+        """
+        structures = []
+        try:
+            starbases_data = (
+                esi.client.Corporation.get_corporations_corporation_id_starbases(
+                    corporation_id=self.corporation.corporation_id,
+                    token=token.valid_access_token(),
+                )
+            ).results()
+            if not starbases_data:
+                logger.info("%s: This corporation has no starbases.", self)
 
-    def is_npc_attacking(self) -> bool:
-        return False
+            else:
+                starbases_data = {obj["starbase_id"]: obj for obj in starbases_data}
+                names = self._fetch_starbases_names(starbases_data.keys(), token)
+                locations = self._fetch_locations_for_assets(
+                    starbases_data.keys(), token
+                )
+                structures += self._convert_starbases_to_structures(
+                    starbases_data, names, locations
+                )
 
-    def parsed_text(self) -> dict:
-        """Adopting to Notification API."""
-        return self.details
-
-
-class BaseFuelAlertConfig(models.Model):
-    """Configuration of structure fuel notifications."""
-
-    channel_ping_type = models.CharField(
-        max_length=2,
-        choices=Webhook.PingType.choices,
-        default=Webhook.PingType.HERE,
-        verbose_name=_("channel pings"),
-        help_text=_(
-            "Option to ping every member of the channel. "
-            "This setting can be overruled by the respective owner "
-            "or webhook configuration"
-        ),
-    )
-    color = models.IntegerField(
-        choices=Webhook.Color.choices,
-        default=Webhook.Color.WARNING,
-        blank=True,
-        null=True,
-        verbose_name=_("color"),
-        help_text=_("Context color of these notification on Discord"),
-    )
-    is_enabled = models.BooleanField(
-        default=True,
-        verbose_name=_("is_enabled"),
-        help_text=_("Disabled configurations will not create any new alerts."),
-    )
+                self._store_updates_for_starbases(token, structures)
 
-    class Meta:
-        abstract = True
+            if STRUCTURES_DEVELOPER_MODE:
+                self._store_raw_data("starbases", structures)
 
-    def __str__(self) -> str:
-        return f"#{self.pk}"
+        except HTTPForbidden:
+            try:
+                character = self.characters.get(
+                    character_ownership__character__character_id=token.character_id
+                )
+            except ObjectDoesNotExist:
+                pass
+            else:
+                self.delete_character(
+                    character=character,
+                    error=(
+                        "Character is not a director or CEO and therefore "
+                        "can not fetch starbases."
+                    ),
+                    max_allowed_errors=STRUCTURES_ESI_DIRECTOR_ERROR_MAX_RETRIES,
+                )
+            return False
 
-    def send_new_notifications(self, force: bool = False) -> None:
-        """Send new fuel notifications based on this config."""
-        raise NotImplementedError()
+        except OSError as ex:
+            self._report_esi_issue("fetch starbases", ex, token)
+            return False
 
-    @staticmethod
-    def relevant_webhooks() -> models.QuerySet:
-        """Webhooks relevant for processing fuel notifications based on this config."""
-        raise NotImplementedError()
+        self._remove_structures_not_returned_from_esi(
+            structures_qs=self.structures.filter_starbases(),
+            new_structures=structures,
+        )
+        return True
 
+    def _store_updates_for_starbases(self, token, structures):
+        logger.info("%s: Storing updates for %d starbases", self, len(structures))
+        for structure in structures:
+            structure_obj, _ = Structure.objects.update_or_create_from_dict(
+                structure, self
+            )
+            detail = self._update_starbase_detail(structure=structure_obj, token=token)
+            fuel_expires_at = detail.calc_fuel_expires()
+            if fuel_expires_at:
+                structure_obj.fuel_expires_at = fuel_expires_at
+                structure_obj.save()
+            if (
+                structure_obj.state == Structure.State.POS_REINFORCED
+                and structure_obj.state_timer_end
+            ):
+                GeneratedNotification.objects.get_or_create_from_structure(
+                    structure=structure_obj,
+                    notif_type=NotificationType.TOWER_REINFORCED_EXTRA,
+                )
 
-class FuelAlertConfig(BaseFuelAlertConfig):
-    """Configuration of structure fuel notifications."""
+    def _convert_starbases_to_structures(
+        self, starbases_data, names, locations
+    ) -> List[dict]:
+        structures = []
+        for structure_id, starbase in starbases_data.items():
+            try:
+                name = names[structure_id]
+            except KeyError:
+                name = "Starbase"
+            structure = {
+                "structure_id": structure_id,
+                "type_id": starbase["type_id"],
+                "corporation_id": self.corporation.corporation_id,
+                "name": name,
+                "system_id": starbase["system_id"],
+            }
+            if structure_id in locations:
+                structure["position"] = locations[structure_id]
+            if "state" in starbase:
+                structure["state"] = starbase["state"]
+            if "moon_id" in starbase:
+                structure["moon_id"] = starbase["moon_id"]
+            if "fuel_expires" in starbase:
+                structure["fuel_expires"] = starbase["fuel_expires"]
+            if "reinforced_until" in starbase:
+                structure["state_timer_end"] = starbase["reinforced_until"]
+            if "unanchors_at" in starbase:
+                structure["unanchors_at"] = starbase["unanchors_at"]
+            structures.append(structure)
+
+        return structures
+
+    def _fetch_starbases_names(self, item_ids: Iterable, token: Token) -> dict:
+        item_ids = list(item_ids)
+        logger.info("%s: Fetching names for %d starbases from ESI", self, len(item_ids))
+        names_data = []
+        for item_ids_chunk in chunks(item_ids, 999):
+            try:
+                names_data_chunk = (
+                    esi.client.Assets.post_corporations_corporation_id_assets_names(
+                        corporation_id=self.corporation.corporation_id,
+                        item_ids=item_ids_chunk,
+                        token=token.valid_access_token(),
+                    )
+                ).results()
+            except HTTPNotFound:
+                pass
+            else:
+                names_data += names_data_chunk
+        names = {x["item_id"]: x["name"] for x in names_data}
+        return names
+
+    def _update_starbase_detail(self, structure, token: Token) -> StarbaseDetail:
+        """Update detail for the starbase from ESI."""
+        operation = esi.client.Corporation.get_corporations_corporation_id_starbases_starbase_id(
+            corporation_id=structure.owner.corporation.corporation_id,
+            starbase_id=structure.id,
+            system_id=structure.eve_solar_system.id,
+            token=token.valid_access_token(),
+        )
+        operation.request_config.also_return_response = True
+        data, response = operation.results()
+        last_modified_at = parsedate_to_datetime(
+            response.headers.get("Last-Modified", format_datetime(now()))
+        )
+        defaults = {
+            "allow_alliance_members": data["allow_alliance_members"],
+            "allow_corporation_members": data["allow_corporation_members"],
+            "anchor_role": StarbaseDetail.Role.from_esi(data["anchor"]),
+            "attack_if_at_war": data["attack_if_at_war"],
+            "attack_if_other_security_status_dropping": data.get(
+                "attack_if_other_security_status_dropping"
+            ),
+            "attack_security_status_threshold": data.get(
+                "attack_security_status_threshold"
+            ),
+            "attack_standing_threshold": data.get("attack_standing_threshold"),
+            "fuel_bay_take_role": StarbaseDetail.Role.from_esi(data["fuel_bay_take"]),
+            "fuel_bay_view_role": StarbaseDetail.Role.from_esi(data["fuel_bay_view"]),
+            "last_modified_at": last_modified_at,
+            "offline_role": StarbaseDetail.Role.from_esi(data["offline"]),
+            "online_role": StarbaseDetail.Role.from_esi(data["online"]),
+            "unanchor_role": StarbaseDetail.Role.from_esi(data["unanchor"]),
+            "use_alliance_standings": data["use_alliance_standings"],
+        }
+        for fuel in data["fuels"]:
+            EveType.objects.get_or_create_esi(id=fuel["type_id"])
+        with transaction.atomic():
+            detail, _ = StarbaseDetail.objects.update_or_create(
+                structure=structure, defaults=defaults
+            )
+            detail.fuels.all().delete()
+            for fuel in data["fuels"]:
+                StarbaseDetailFuel.objects.create(
+                    eve_type_id=fuel["type_id"],
+                    detail=detail,
+                    quantity=fuel["quantity"],
+                )
+        return detail
 
-    end = models.PositiveIntegerField(
-        verbose_name=_("end"), help_text=_("End of alerts in hours before fuel expires")
-    )
-    repeat = models.PositiveIntegerField(
-        verbose_name=_("repeat"),
-        help_text=_(
-            "Notifications will be repeated every x hours. Set to 0 for no repeats"
-        ),
-    )
-    start = models.PositiveIntegerField(
-        verbose_name=_("start"),
-        help_text=_("Start of alerts in hours before fuel expires"),
-    )
+    def add_or_remove_timers_from_notifications(self):
+        """Add/remove timers from esi and generated notification of this owner."""
+        self.notification_set.add_or_remove_timers()
+        self.generatednotification_set.add_or_remove_timers()
+
+    def fetch_notifications_esi(self, user: Optional[User] = None) -> None:
+        """Fetch notifications for this owner from ESI and process them."""
+        notifications_count_all = 0
+        token = self.fetch_token(
+            rotate_characters=self.RotateCharactersType.NOTIFICATIONS
+        )
+        notifications = self._fetch_notifications_from_esi(token)
+        notifications_count_new = self._store_notifications(notifications)
+        self._process_moon_notifications()
+        if notifications_count_new > 0:
+            logger.info(
+                "%s: Received %d new notifications from ESI",
+                self,
+                notifications_count_new,
+            )
+            notifications_count_all += notifications_count_new
+        else:
+            logger.info("%s: No new notifications received from ESI", self)
 
-    class Meta:
-        verbose_name = _("structure fuel alert config")
-        verbose_name_plural = _("structure fuel alert configs")
+        self.notifications_last_update_at = now()
+        self.save(update_fields=["notifications_last_update_at"])
+        if user:
+            self._send_report_to_user(
+                topic="notifications",
+                topic_count=notifications_count_all,
+                user=user,
+            )
 
-    def clean(self) -> None:
-        if self.start is None or self.end is None or self.repeat is None:  # Fixes #83
-            return  # these will be caught by the form validation later
-        if self.start <= self.end:
-            raise ValidationError(
-                _("Start must be before end, i.e. have a larger value.")
-            )
-        if self.repeat >= self.start - self.end:
-            raise ValidationError(
-                {"repeat": _("Repeat can not be larger that the interval size.")}
-            )
-        new = range(self.end, self.start)
-        for config in FuelAlertConfig.objects.exclude(pk=self.pk):
-            current = range(config.end, config.start)
-            overlap = range(max(new[0], current[0]), min(new[-1], current[-1]) + 1)
-            if len(overlap) > 0:
-                raise ValidationError(
-                    _(
-                        "This configuration may not overlap with an "
-                        "existing configuration."
-                    )
-                )
+    def _fetch_notifications_from_esi(self, token: Token) -> List[dict]:
+        """fetching all notifications from ESI for current owner"""
+        notifications = esi.client.Character.get_characters_character_id_notifications(
+            character_id=token.character_id, token=token.valid_access_token()
+        ).results()
+        if STRUCTURES_DEVELOPER_MODE:
+            self._store_raw_data("notifications", notifications)
+        if STRUCTURES_NOTIFICATIONS_ARCHIVING_ENABLED:
+            self._store_raw_notifications(notifications)
+        logger.debug(
+            "%s: Processing %d notifications received from ESI",
+            self,
+            len(notifications),
+        )
+        return notifications
 
-    def save(self, *args, **kwargs) -> None:
-        try:
-            old_instance = FuelAlertConfig.objects.get(pk=self.pk)
-        except FuelAlertConfig.DoesNotExist:
-            old_instance = None
-        super().save(*args, **kwargs)
-        if old_instance and (
-            old_instance.start != self.start
-            or old_instance.end != self.end
-            or old_instance.repeat != self.repeat
-        ):
-            self.structure_fuel_alerts.all().delete()
+    def _store_raw_notifications(self, notifications):
+        """Store notifications to disk in continuous file per corp."""
+        folder_name = "structures_notifications_archive"
+        os.makedirs(folder_name, exist_ok=True)
+        corporation_id = self.corporation.corporation_id
+        now_str = now().date().isoformat()
+        filename = f"{folder_name}/notifications_{corporation_id}_{now_str}.txt"
+        logger.info(
+            "%s: Storing notifications into archive file: %s", self, format(filename)
+        )
+        with open(file=filename, mode="a", encoding="utf-8") as file:
+            now_str_2 = now().strftime(DATETIME_FORMAT)
+            file.write(f"[{now_str_2}] {self.corporation.corporation_ticker}:\n")
+            json.dump(
+                notifications, file, cls=DjangoJSONEncoder, sort_keys=True, indent=4
+            )
+            file.write("\n")
 
-    def send_new_notifications(self, force: bool = False) -> None:
-        """Send new fuel notifications based on this config."""
-        structures = Structure.objects.filter(
-            eve_type__eve_group__eve_category_id__in=[
-                EveCategoryId.STARBASE,
-                EveCategoryId.STRUCTURE,
-            ],
-            fuel_expires_at__isnull=False,
+    def _store_notifications(self, notifications: List[dict]) -> int:
+        """Store new notifications in database.
+        Returns number of newly created objects.
+        """
+        # identify new notifications
+        existing_notification_ids = set(
+            self.notification_set.values_list("notification_id", flat=True)
         )
-        for structure in structures:
-            if not structure.is_burning_fuel:
-                continue
-            hours_left = structure.hours_fuel_expires
-            if self.start >= hours_left >= self.end:
-                hours_last_alert = (
-                    self.start
-                    - (
-                        math.floor((self.start - hours_left) / self.repeat)
-                        * self.repeat
-                    )
-                    if self.repeat
-                    else self.start
-                )
-                notif, created = FuelAlert.objects.get_or_create(
-                    structure=structure, config=self, hours=hours_last_alert
+        new_notifications = [
+            obj
+            for obj in notifications
+            if obj["notification_id"] not in existing_notification_ids
+        ]
+        # create new notification objects
+        for notification in new_notifications:
+            if notification["sender_type"] == "other":
+                sender = None
+            else:
+                sender, _ = EveEntity.objects.get_or_create_esi(
+                    id=notification["sender_id"]
                 )
-                if created or force:
-                    notif.send_generated_notification()
+            text = notification["text"] if "text" in notification else None
+            is_read = notification["is_read"] if "is_read" in notification else None
+            # at least one type has a trailing white space
+            # which we need to remove
+            notif_type = notification["type"].strip()
+            Notification.objects.create(
+                notification_id=notification["notification_id"],
+                owner=self,
+                sender=sender,
+                timestamp=notification["timestamp"],
+                notif_type=notif_type,
+                text=text,
+                is_read=is_read,
+                last_updated=now(),
+                created=now(),
+            )
+        return len(new_notifications)
 
-    @staticmethod
-    def relevant_webhooks() -> models.QuerySet:
-        """Webhooks relevant for processing fuel notifications based on this config."""
-        return (
-            Webhook.objects.filter(is_active=True)
-            .filter(Q(owners__isnull=False) | Q(structures__isnull=False))
-            .filter(
-                Q(notification_types__contains=NotificationType.STRUCTURE_FUEL_ALERT)
-                | Q(
-                    notification_types__contains=NotificationType.TOWER_RESOURCE_ALERT_MSG
+    def _process_moon_notifications(self):
+        """processes notifications for timers if any"""
+        empty_refineries = Structure.objects.filter(
+            owner=self,
+            eve_type__eve_group_id=EveGroupId.REFINERY,
+            eve_moon__isnull=True,
+        )
+        if empty_refineries.exists():
+            logger.info(
+                "%s: Trying to find moons for up to %d refineries which have no moon.",
+                self,
+                empty_refineries.count(),
+            )
+            notifications = (
+                self.notification_set.filter(
+                    notif_type__in=NotificationType.relevant_for_moonmining()
                 )
+                .select_related("owner", "sender")
+                .order_by("timestamp")
             )
-            .distinct()
+            structure_id_2_moon_id = {}
+            for notification in notifications:
+                parsed_text = notification.parsed_text()
+                moon_id = parsed_text["moonID"]
+                structure_id = parsed_text["structureID"]
+                structure_id_2_moon_id[structure_id] = moon_id
+            for refinery in empty_refineries:
+                if refinery.id in structure_id_2_moon_id:
+                    logger.info("%s: Updating moon for structure %s", self, refinery)
+                    eve_moon, _ = EveMoon.objects.get_or_create_esi(
+                        id=structure_id_2_moon_id[refinery.id]
+                    )
+                    refinery.eve_moon = eve_moon
+                    refinery.save()
+
+    def send_new_notifications(self, user: Optional[User] = None):
+        """Forward all new notification of this owner to configured webhooks."""
+        notifications_count = 0
+        cutoff_dt_for_stale = now() - dt.timedelta(
+            hours=STRUCTURES_HOURS_UNTIL_STALE_NOTIFICATION
+        )
+        my_filter = {
+            "notif_type__in": (
+                Webhook.objects.enabled_notification_types()
+                & NotificationType.relevant_for_forwarding()
+            ),
+            "is_sent": False,
+            "timestamp__gte": cutoff_dt_for_stale,
+        }
+        new_eve_notifications = (
+            self.notification_set.filter(**my_filter)
+            .select_related("owner", "sender", "owner__corporation")
+            .order_by("timestamp")
         )
+        for notif in new_eve_notifications:
+            notif.send_to_configured_webhooks()
+        new_generated_notifications = (
+            self.generatednotification_set.filter(**my_filter)
+            .select_related("owner", "owner__corporation")
+            .order_by("timestamp")
+        )
+        for notif in new_generated_notifications:
+            notif.send_to_configured_webhooks()
+        if (
+            not new_eve_notifications.exists()
+            and not new_generated_notifications.exists()
+        ):
+            logger.info("%s: No new notifications found for forwarding", self)
+        self.forwarding_last_update_at = now()
+        self.save(update_fields=["forwarding_last_update_at"])
+        if user:
+            self._send_report_to_user(
+                topic="notifications", topic_count=notifications_count, user=user
+            )
 
+    def _send_report_to_user(self, topic: str, topic_count: int, user: User):
+        message_details = "%(count)s %(topic)s synced." % {
+            "count": topic_count,
+            "topic": topic,
+        }
+        message = _(
+            "Syncing of %(topic)s for %(owner)s %(result)s.\n %(message_details)s"
+        ) % {
+            "topic": topic,
+            "owner": self.corporation.corporation_name,
+            "result": _("completed successfully"),
+            "message_details": message_details,
+        }
+        notify(
+            user,
+            title=_("%(title)s: %(topic)s updated for %(owner)s: %(result)s")
+            % {
+                "title": _(__title__),
+                "topic": topic,
+                "owner": self.corporation.corporation_name,
+                "result": _("OK"),
+            },
+            message=message,
+            level="success",
+        )
 
-class JumpFuelAlertConfig(BaseFuelAlertConfig):
-    """Configuration of jump fuel notifications."""
+    def _store_raw_data(self, name: str, data: Any):
+        """store raw data for debug purposes"""
+        with open(
+            f"{name}_raw_{self.corporation.corporation_id}.json", "w", encoding="utf-8"
+        ) as file:
+            json.dump(data, file, cls=DjangoJSONEncoder, sort_keys=True, indent=4)
+
+    def update_asset_esi(self, user: Optional[User] = None):
+        """Update assets from ESI."""
+        token = self.fetch_token()
+        assets_data = self._fetch_structure_assets_from_esi(token)
+        self._store_items_for_upwell_structures(assets_data)
+        self._store_items_for_starbases(assets_data)
+        if user:
+            self._send_report_to_user(
+                topic="assets", topic_count=self.structures.count(), user=user
+            )
 
-    threshold = models.PositiveIntegerField(
-        verbose_name=_("threshold"),
-        help_text=_(
-            "Notifications will be sent once fuel level in units reaches this threshold"
-        ),
-    )
+    def _fetch_structure_assets_from_esi(self, token: Token) -> dict:
+        assets_raw = esi.client.Assets.get_corporations_corporation_id_assets(
+            corporation_id=self.corporation.corporation_id,
+            token=token.valid_access_token(),
+        ).results()
+        assets = {asset["item_id"]: asset for asset in assets_raw}
+        positions = self._fetch_locations_for_assets(assets.keys(), token)
+        for item_id, asset in assets.items():
+            asset["position"] = positions[item_id] if item_id in positions else None
+        return assets
+
+    def _store_items_for_upwell_structures(self, assets_data: dict):
+        structure_ids = set(
+            self.structures.filter_upwell_structures().values_list("id", flat=True)
+        )
+        assets_in_structures = {id: {} for id in structure_ids}
+        for item_id, item in assets_data.items():
+            location_id = item["location_id"]
+            if location_id in structure_ids and item["location_flag"] not in [
+                StructureItem.LocationFlag.CORP_DELIVERIES,
+                StructureItem.LocationFlag.OFFICE_FOLDER,
+                StructureItem.LocationFlag.SECONDARY_STORAGE,
+                StructureItem.LocationFlag.AUTOFIT,
+            ]:
+                assets_in_structures[location_id][item_id] = item
+        for structure in self.structures.all():
+            structure_items = []
+            if structure.id in assets_in_structures.keys():
+                structure_assets = assets_in_structures[structure.id]
+                has_fitting = [
+                    asset
+                    for asset in structure_assets.values()
+                    if asset["location_flag"]
+                    != StructureItem.LocationFlag.QUANTUM_CORE_ROOM
+                ]
+                has_core = [
+                    asset
+                    for asset in structure_assets.values()
+                    if asset["location_flag"]
+                    == StructureItem.LocationFlag.QUANTUM_CORE_ROOM
+                ]
+                structure.has_fitting = bool(has_fitting)
+                structure.has_core = bool(has_core)
+                structure.save()
+
+                for asset in structure_assets.values():
+                    structure_items.append(
+                        StructureItem.from_esi_asset(asset, structure)
+                    )
 
-    class Meta:
-        verbose_name = _("jump fuel alert config")
-        verbose_name_plural = _("jump fuel alert configs")
+            structure.update_items(structure_items)
+            structure.reevaluate_jump_fuel_alerts()
 
-    def save(self, *args, **kwargs) -> None:
-        try:
-            old_instance = JumpFuelAlertConfig.objects.get(pk=self.pk)
-        except JumpFuelAlertConfig.DoesNotExist:
-            old_instance = None
-        super().save(*args, **kwargs)
-        if old_instance and (old_instance.threshold != self.threshold):
-            self.jump_fuel_alerts.all().delete()
+        self.assets_last_update_at = now()
+        self.save(update_fields=["assets_last_update_at"])
 
-    def send_new_notifications(self, force: bool = False) -> None:
-        """Send new fuel notifications based on this config."""
-        jump_gates = Structure.objects.filter(eve_type_id=EveTypeId.JUMP_GATE)
-        for jump_gate in jump_gates:
-            if not jump_gate.is_burning_fuel:
-                continue
-            fuel_quantity = jump_gate.jump_fuel_quantity()
-            if fuel_quantity and fuel_quantity < self.threshold:
-                notif, created = JumpFuelAlert.objects.get_or_create(
-                    structure=jump_gate, config=self
-                )
-                if created or force:
-                    notif.send_generated_notification()
+    def _store_items_for_starbases(self, assets_raw: dict):
+        relevant_assets = {
+            item_id: item
+            for item_id, item in assets_raw.items()
+            if item["location_type"] == "solar_system"
+            and item["location_flag"] == "AutoFit"
+            and item["position"]
+        }
+        for structure in self.structures.filter_starbases().filter(
+            position_x__isnull=False, position_y__isnull=False, position_z__isnull=False
+        ):
+            structure_items = []
+            for item_id, item in relevant_assets.items():
+                if (
+                    item["location_id"] == structure.eve_solar_system_id
+                    and item_id != structure.id
+                    and structure.distance_to_object(
+                        item["position"]["x"],
+                        item["position"]["y"],
+                        item["position"]["z"],
+                    )
+                    < 100_000
+                ):
+                    structure_items.append(
+                        StructureItem.from_esi_asset(item, structure)
+                    )
+            structure.update_items(structure_items)
 
     @staticmethod
-    def relevant_webhooks() -> models.QuerySet:
-        """Webhooks relevant for processing jump fuel notifications based on this config."""
-        return Webhook.objects.filter(
-            is_active=True,
-            notification_types__contains=NotificationType.STRUCTURE_JUMP_FUEL_ALERT,
-        ).filter(Q(owners__isnull=False) | Q(structures__isnull=False))
-
-
-class BaseFuelAlert(models.Model):
-    class Meta:
-        abstract = True
-
-    def send_generated_notification(self):
-        raise NotImplementedError()
+    def get_esi_scopes() -> List[str]:
+        """Return all required ESI scopes."""
+        scopes = [
+            "esi-corporations.read_structures.v1",
+            "esi-universe.read_structures.v1",
+            "esi-characters.read_notifications.v1",
+            "esi-assets.read_corporation_assets.v1",
+        ]
+        if STRUCTURES_FEATURE_CUSTOMS_OFFICES:
+            scopes += ["esi-planets.read_customs_offices.v1"]
+        if STRUCTURES_FEATURE_STARBASES:
+            scopes += ["esi-corporations.read_starbases.v1"]
+        return scopes
 
 
-class FuelAlert(BaseFuelAlert):
-    """A generated notification alerting about fuel getting low in structures."""
+class OwnerCharacter(models.Model):
+    """Character for syncing owner data with ESI."""
 
-    structure = models.ForeignKey(
-        Structure,
+    owner = models.ForeignKey(
+        Owner,
         on_delete=models.CASCADE,
-        related_name="structure_fuel_alerts",
-        verbose_name=_("structure"),
+        related_name="characters",
+        verbose_name=_("owner"),
     )
-    config = models.ForeignKey(
-        FuelAlertConfig,
+    character_ownership = models.ForeignKey(
+        CharacterOwnership,
         on_delete=models.CASCADE,
-        related_name="structure_fuel_alerts",
-        verbose_name=_("configuration"),
+        related_name="+",
+        verbose_name=_("character_ownership"),
+        help_text="character used for syncing",
+    )
+    structures_last_used_at = models.DateTimeField(
+        null=True,
+        default=None,
+        editable=False,
+        db_index=True,
+        verbose_name=_("structures last used at"),
+        help_text="when this character was last used for syncing structures",
     )
-    hours = models.PositiveIntegerField(
+    notifications_last_used_at = models.DateTimeField(
+        null=True,
+        default=None,
+        editable=False,
         db_index=True,
-        verbose_name=_("hours"),
-        help_text=_("number of hours before fuel expiration this alert was sent"),
+        verbose_name=_("notifications last used at"),
+        help_text="when this character was last used for syncing notifications",
     )
+    error_count = models.PositiveIntegerField(
+        default=0,
+        editable=False,
+        verbose_name=_("error count"),
+        help_text="Count of ESI errors which happened with this character.",
+    )
+    created_at = models.DateTimeField(auto_now_add=True)
 
     class Meta:
-        verbose_name = _("structure fuel alert")
-        verbose_name_plural = _("structure fuel alerts")
+        verbose_name = _("owner character")
+        verbose_name_plural = _("owner characters")
         constraints = [
             models.UniqueConstraint(
-                fields=["structure", "config", "hours"],
-                name="functional_pk_fuelalert",
+                fields=["owner", "character_ownership"], name="functional_pk_ownertoken"
             )
         ]
 
     def __str__(self) -> str:
-        return f"{self.structure}-{self.config}-{self.hours}"
-
-    def send_generated_notification(self):
-        notif_type = (
-            NotificationType.TOWER_RESOURCE_ALERT_MSG
-            if self.structure.is_starbase
-            else NotificationType.STRUCTURE_FUEL_ALERT
-        )
-        notif = Notification.create_from_structure(
-            structure=self.structure, notif_type=notif_type
-        )
-        notif.send_to_configured_webhooks(
-            ping_type_override=self.config.channel_ping_type,
-            use_color_override=True,
-            color_override=self.config.color,
+        return (
+            f"{self.owner.corporation.corporation_name}-"
+            f"{self.character_ownership.character.character_name}"
         )
 
-
-class JumpFuelAlert(BaseFuelAlert):
-    """A generated notification alerting about jump fuel getting low."""
-
-    structure = models.ForeignKey(
-        Structure,
-        on_delete=models.CASCADE,
-        related_name="jump_fuel_alerts",
-        verbose_name=_("structure"),
-    )
-    config = models.ForeignKey(
-        JumpFuelAlertConfig,
-        on_delete=models.CASCADE,
-        related_name="jump_fuel_alerts",
-        verbose_name=_("configuration"),
-    )
-
-    class Meta:
-        verbose_name = _("jump fuel alert")
-        verbose_name_plural = _("jump fuel alerts")
-
-    def __str__(self) -> str:
-        return f"{self.structure}-{self.config}"
-
-    def send_generated_notification(self) -> None:
-        notif = Notification.create_from_structure(
-            structure=self.structure,
-            notif_type=NotificationType.STRUCTURE_JUMP_FUEL_ALERT,
-            threshold=self.config.threshold,
-        )
-        notif.send_to_configured_webhooks(
-            ping_type_override=self.config.channel_ping_type,
-            use_color_override=True,
-            color_override=self.config.color,
+    def valid_token(self) -> Optional[Token]:
+        """Provide a valid token or None if none can be found."""
+        return (
+            Token.objects.filter(
+                user=self.character_ownership.user,
+                character_id=self.character_ownership.character.character_id,
+            )
+            .require_scopes(Owner.get_esi_scopes())
+            .require_valid()
+            .first()
         )
```

### Comparing `aa_structures-2.4.2/structures/models/structures.py` & `aa_structures-2.5.0/structures/models/structures_1.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Structure related models."""
+"""Structure related models for Structures."""
 
 import datetime as dt
 import math
 import re
 from typing import List, Optional
 
 from django.core.validators import MaxValueValidator, MinValueValidator
@@ -11,25 +11,25 @@
 from django.utils.functional import cached_property
 from django.utils.html import escape
 from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
 from django.utils.translation import gettext_noop
 from eveuniverse.models import EveMoon, EvePlanet, EveSolarSystem, EveType
 
-from allianceauth.eveonline.models import EveCharacter
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 from app_utils.views import bootstrap_label_html
 
-from .. import __title__
-from ..app_settings import STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS
-from ..constants import EveCategoryId, EveGroupId, EveTypeId
-from ..core import starbases
-from ..helpers.general import datetime_almost_equal, hours_until_deadline
-from ..managers import StructureManager, StructureTagManager
+from structures import __title__
+from structures.app_settings import STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS
+from structures.constants import EveCategoryId, EveGroupId, EveTypeId
+from structures.core import starbases
+from structures.helpers import datetime_almost_equal, hours_until_deadline
+from structures.managers import StructureManager, StructureTagManager
+
 from .eveuniverse import EveSpaceType
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class StructureTag(models.Model):
     """Tag for organizing structures."""
@@ -38,14 +38,16 @@
     NAME_SOV_TAG = gettext_noop("sov")
     NAME_HIGHSEC_TAG = gettext_noop("highsec")
     NAME_LOWSEC_TAG = gettext_noop("lowsec")
     NAME_NULLSEC_TAG = gettext_noop("nullsec")
     NAME_W_SPACE_TAG = gettext_noop("w_space")
 
     class Style(models.TextChoices):
+        """A boostrap like style."""
+
         GREY = "default", _("grey")
         DARK_BLUE = "primary", _("dark blue")
         GREEN = "success", _("green")
         LIGHT_BLUE = "info", _("light blue")
         ORANGE = "warning", _("orange")
         RED = "danger", _("red")
 
@@ -110,39 +112,42 @@
         verbose_name_plural = _("structure tags")
         ordering = ["order", "name"]
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self):
-        return "{}(name='{}')".format(self.__class__.__name__, self.name)
+        return f"{self.__class__.__name__}(name='{self.name}')"
 
     @property
     def html(self) -> str:
+        """Return HTML for this tag."""
         if self.is_user_managed:
             name = escape(self.name)
         else:
             name = _(self.name)
         return bootstrap_label_html(name, self.style)
 
     @classmethod
     def sorted(cls, tags: list, reverse: bool = False) -> list:
         """returns a sorted copy of the provided list of tags"""
         return sorted(tags, key=lambda x: x.name.lower(), reverse=reverse)
 
 
-class Structure(models.Model):
+class Structure(models.Model):  # pylint: disable = too-many-public-methods
     """A structure in Eve Online."""
 
-    # Threshold in seconds when two fuel expiry dates will be judged as different
     FUEL_DATES_EQUAL_THRESHOLD_UPWELL = 1800
-    FUEL_DATES_EQUAL_THRESHOLD_STARBASE = 7200  # high fluctuation due to estimating
+    """Threshold in seconds when two fuel expiry dates will be judged as different."""
+
+    FUEL_DATES_EQUAL_THRESHOLD_STARBASE = 7200
+    """high fluctuation due to estimating."""
 
     class State(models.IntegerChoices):
-        """State of a structure"""
+        """A state of a structure."""
 
         # states Upwell structures
         ANCHOR_VULNERABLE = 1, _("anchor vulnerable")
         ANCHORING = 2, _("anchoring")
         ARMOR_REINFORCE = 3, _("armor reinforce")
         ARMOR_VULNERABLE = 4, _("armor vulnerable")
         DEPLOY_VULNERABLE = 5, _("deploy vulnerable")
@@ -162,15 +167,15 @@
         # other
         NA = 0, _("N/A")
         UNKNOWN = 13, _("unknown")
 
         @classmethod
         def from_esi_name(cls, esi_state_name: str) -> "Structure.State":
             """returns matching state for esi state name of Upwell structures"""
-            STATES_ESI_MAP = {
+            states_esi_map = {
                 "anchor_vulnerable": cls.ANCHOR_VULNERABLE,
                 "anchoring": cls.ANCHORING,
                 "armor_reinforce": cls.ARMOR_REINFORCE,
                 "armor_vulnerable": cls.ARMOR_VULNERABLE,
                 "deploy_vulnerable": cls.DEPLOY_VULNERABLE,
                 "fitting_invulnerable": cls.FITTING_INVULNERABLE,
                 "hull_reinforce": cls.HULL_REINFORCE,
@@ -182,20 +187,22 @@
                 "offline": cls.POS_OFFLINE,
                 "online": cls.POS_ONLINE,
                 "onlining": cls.POS_ONLINING,
                 "reinforced": cls.POS_REINFORCED,
                 "unanchoring ": cls.POS_UNANCHORING,
             }
             return (
-                STATES_ESI_MAP[esi_state_name]
-                if esi_state_name in STATES_ESI_MAP
+                states_esi_map[esi_state_name]
+                if esi_state_name in states_esi_map
                 else cls.UNKNOWN
             )
 
     class PowerMode(models.TextChoices):
+        """A power mode of a structure."""
+
         FULL_POWER = "FU", _("Full Power")
         LOW_POWER = "LO", _("Low Power")
         ABANDONED = "AB", _("Abandoned")
         LOW_ABANDONED = "LA", _("Abandoned?")
         UNKNOWN = "UN", _("Unknown")
 
     id = models.BigIntegerField(
@@ -440,42 +447,47 @@
             for tag in StructureTag.objects.filter(is_default=True):
                 self.tags.add(tag)
         # make sure related objects are saved whenever structure is saved
         self.update_generated_tags()
 
     @property
     def is_jump_gate(self) -> bool:
+        """Return True if this structure is a jump gate, else False."""
         return self.eve_type_id == EveTypeId.JUMP_GATE
 
     @property
     def is_poco(self) -> bool:
+        """Return True if this structure is a customs office, else False."""
         return self.eve_type_id == EveTypeId.CUSTOMS_OFFICE
 
     @cached_property
     def is_starbase(self) -> bool:
+        """Return True if this structure is a starbase, else False."""
         return starbases.is_starbase(self.eve_type)
 
     @cached_property
     def is_upwell_structure(self) -> bool:
+        """Return True if this structure is an upwell structure, else False."""
         return self.eve_type.eve_group.eve_category_id == EveCategoryId.STRUCTURE
 
     @property
     def is_full_power(self) -> Optional[bool]:
-        """return True if structure is full power, False if not.
+        """Return True if structure is full power, False if not.
 
         Returns None if state can not be determined
         """
         power_mode = self.power_mode
         if not power_mode:
             return None
+
         return power_mode == self.PowerMode.FULL_POWER
 
     @property
     def is_low_power(self) -> Optional[bool]:
-        """return True if structure is low power, False if not.
+        """Return True if structure is low power, False if not.
 
         Returns None if state can not be determined
         """
         power_mode = self.power_mode
         if not power_mode:
             return None
         return power_mode == self.PowerMode.LOW_POWER
@@ -505,27 +517,31 @@
     @property
     def power_mode(self) -> Optional["PowerMode"]:
         """returns the calculated power mode of this structure, e.g. low power
         returns None for non upwell structures
         """
         if not self.is_upwell_structure:
             return None
+
         if self.fuel_expires_at and self.fuel_expires_at > now():
             return self.PowerMode.FULL_POWER
-        elif self.last_online_at:
+
+        if self.last_online_at:
             if self.last_online_at >= now() - dt.timedelta(days=7):
                 return self.PowerMode.LOW_POWER
-            else:
-                return self.PowerMode.ABANDONED
-        elif self.state in {self.State.ANCHORING, self.State.ANCHOR_VULNERABLE}:
+            return self.PowerMode.ABANDONED
+
+        if self.state in {self.State.ANCHORING, self.State.ANCHOR_VULNERABLE}:
             return self.PowerMode.LOW_POWER
+
         return self.PowerMode.LOW_ABANDONED
 
     @property
     def is_reinforced(self) -> bool:
+        """Return True if this structure is reinforced, else False."""
         return self.state in [
             self.State.ARMOR_REINFORCE,
             self.State.HULL_REINFORCE,
             self.State.ANCHOR_VULNERABLE,
             self.State.HULL_VULNERABLE,
             self.State.POS_REINFORCED,
         ]
@@ -550,14 +566,17 @@
             self.position_x is not None
             and self.position_y is not None
             and self.position_z is not None
         )
 
     @cached_property
     def owner_has_sov(self) -> bool:
+        """Return True if the owner of this structure has sov in this solar system,
+        else False.
+        """
         return self.owner.has_sov(self.eve_solar_system)
 
     @cached_property
     def location_name(self) -> str:
         """Name of this structures's location."""
         try:
             return self.eve_moon.name
@@ -643,15 +662,15 @@
         )
 
     def handle_fuel_notifications(self, old_instance: "Structure"):
         """Remove fuel notifications if fuel levels have changed
         and sent refueled notifications if structure has been refueled.
         """
         if self.fuel_expires_at and old_instance and self.pk == old_instance.pk:
-            logger_tag = "%s: Fuel notifications" % self
+            logger_tag = f"{self}: Fuel notifications"
             if self.fuel_expires_at != old_instance.fuel_expires_at:
                 logger.info(
                     "%s: Fuel expiry dates changed: old|current|delta: %s|%s|%s",
                     logger_tag,
                     old_instance.fuel_expires_at.isoformat()
                     if old_instance.fuel_expires_at
                     else None,
@@ -703,14 +722,17 @@
         jump_fuel_quantity = self.jump_fuel_quantity()
         if jump_fuel_quantity:
             self.jump_fuel_alerts.filter(
                 config__threshold__lt=jump_fuel_quantity
             ).delete()
 
     def get_power_mode_display(self) -> str:
+        """Return this structure's power mode as label for display.
+        Or return an empty string for structures that have no power mode.
+        """
         return self.PowerMode(self.power_mode).label if self.power_mode else ""
 
     def update_generated_tags(self, recreate_tags=False):
         """updates all generated tags for this structure
 
         recreate_tags: when set true all tags will be re-created,
         otherwise just re-added if they are missing
@@ -798,250 +820,25 @@
         verbose_name = _("structure item")
         verbose_name_plural = _("structure items")
 
     def __str__(self) -> str:
         return str(self.eve_type.name)
 
     def __repr__(self):
-        return "{}(pk={}, structure=<{}>, eve_type=<{}>)".format(
-            self.__class__.__name__, self.pk, self.structure, self.eve_type
+        return (
+            f"{self.__class__.__name__}("
+            f"pk={self.pk}, structure=<{self.structure}>, eve_type=<{self.eve_type}>"
+            ")"
         )
 
     @classmethod
     def from_esi_asset(cls, item: dict, structure: "Structure") -> "StructureItem":
         """Create new object from ESI asset item."""
         eve_type, _ = EveType.objects.get_or_create_esi(id=item["type_id"])
         return StructureItem(
             id=item["item_id"],
             structure=structure,
             eve_type=eve_type,
             is_singleton=item["is_singleton"],
             location_flag=item["location_flag"],
             quantity=item["quantity"],
         )
-
-
-class StructureService(models.Model):
-    """Service of a Structure."""
-
-    class State(models.IntegerChoices):
-        OFFLINE = 1, _("offline")
-        ONLINE = 2, _("online")
-
-        @classmethod
-        def from_esi_name(cls, esi_state_name: str) -> "StructureService.State":
-            """returns matching state for given ESI state name"""
-            STATES_ESI_MAP = {"offline": cls.OFFLINE, "online": cls.ONLINE}
-            return (
-                STATES_ESI_MAP[esi_state_name]
-                if esi_state_name in STATES_ESI_MAP
-                else cls.OFFLINE
-            )
-
-    structure = models.ForeignKey(
-        Structure,
-        on_delete=models.CASCADE,
-        related_name="services",
-        verbose_name=_("structure"),
-        help_text=_("Structure this service is installed to"),
-    )
-    name = models.CharField(
-        max_length=100, verbose_name=_("name"), help_text=_("Name of the service")
-    )
-
-    state = models.IntegerField(
-        choices=State.choices,
-        verbose_name=_("state"),
-        help_text=_("Current state of this service"),
-    )
-
-    class Meta:
-        verbose_name = _("structure service")
-        verbose_name_plural = _("structure services")
-        unique_together = (("structure", "name"),)
-
-    def __str__(self):
-        return "{} - {}".format(str(self.structure), self.name)
-
-    def __repr__(self):
-        return "{}(structure_id={}, name='{}')".format(
-            self.__class__.__name__, self.structure.id, self.name
-        )
-
-
-class PocoDetails(models.Model):
-    """Additional information about a POCO."""
-
-    class StandingLevel(models.IntegerChoices):
-        NONE = -99, _("none")
-        TERRIBLE = -10, _("terrible")
-        BAD = -5, _("bad")
-        NEUTRAL = 0, _("neutral")
-        GOOD = 5, _("good")
-        EXCELLENT = 10, _("excellent")
-
-        @classmethod
-        def from_esi(cls, value) -> "PocoDetails.StandingLevel":
-            """Return match from ESI value or NONE"""
-            my_map = {
-                "bad": cls.BAD,
-                "excellent": cls.EXCELLENT,
-                "good": cls.GOOD,
-                "neutral": cls.NEUTRAL,
-                "terrible": cls.TERRIBLE,
-            }
-            try:
-                return my_map[value]
-            except KeyError:
-                return cls.NONE
-
-    alliance_tax_rate = models.FloatField(null=True, default=None)
-    allow_access_with_standings = models.BooleanField()
-    allow_alliance_access = models.BooleanField()
-    bad_standing_tax_rate = models.FloatField(null=True, default=None)
-    corporation_tax_rate = models.FloatField(null=True, default=None)
-    excellent_standing_tax_rate = models.FloatField(null=True, default=None)
-    good_standing_tax_rate = models.FloatField(null=True, default=None)
-    neutral_standing_tax_rate = models.FloatField(null=True, default=None)
-    reinforce_exit_end = models.PositiveIntegerField()
-    reinforce_exit_start = models.PositiveIntegerField()
-    standing_level = models.IntegerField(
-        choices=StandingLevel.choices, default=StandingLevel.NONE
-    )
-    structure = models.OneToOneField(
-        Structure, on_delete=models.CASCADE, related_name="poco_details"
-    )
-    terrible_standing_tax_rate = models.FloatField(null=True, default=None)
-
-    def __str__(self):
-        return f"{self.structure}"
-
-    @property
-    def reinforce_exit_end_str(self) -> str:
-        return f"{self.reinforce_exit_end}:00"
-
-    @property
-    def reinforce_exit_start_str(self) -> str:
-        return f"{self.reinforce_exit_start}:00"
-
-    def tax_for_character(self, character: EveCharacter) -> Optional[float]:
-        """Return the effective tax for this character or None if unknown."""
-        owner_corporation = self.structure.owner.corporation
-        if character.corporation_id == owner_corporation.corporation_id:
-            return self.corporation_tax_rate
-        if (
-            owner_corporation.alliance
-            and owner_corporation.alliance.alliance_id == character.alliance_id
-        ):
-            return self.alliance_tax_rate
-        else:
-            return None
-
-    def has_character_access(self, character: EveCharacter) -> Optional[bool]:
-        """Return Tru if this has access else False."""
-        owner_corporation = self.structure.owner.corporation
-        if character.corporation_id == owner_corporation.corporation_id:
-            return True
-        if (
-            owner_corporation.alliance
-            and owner_corporation.alliance.alliance_id == character.alliance_id
-        ):
-            return self.allow_alliance_access
-        else:
-            return None
-
-    def standing_level_access_map(self) -> dict:
-        """Return map of access per standing level with standing level names as key."""
-        names_map = {
-            self.StandingLevel.NONE: "NONE",
-            self.StandingLevel.TERRIBLE: "TERRIBLE",
-            self.StandingLevel.BAD: "BAD",
-            self.StandingLevel.NEUTRAL: "NEUTRAL",
-            self.StandingLevel.GOOD: "GOOD",
-            self.StandingLevel.EXCELLENT: "EXCELLENT",
-        }
-        return {
-            names_map[self.StandingLevel(level)]: (
-                self.allow_access_with_standings and level >= self.standing_level
-            )
-            for level in self.StandingLevel.values
-        }
-
-
-class StarbaseDetail(models.Model):
-    """Additional information about a starbase."""
-
-    class Role(models.TextChoices):
-        ALLIANCE_MEMBER = "AL", _("alliance member")
-        CONFIG_STARBASE_EQUIPMENT_ROLE = "CE", _("config starbase equipment role")
-        CORPORATION_MEMBER = "CO", _("corporation member")
-        STARBASE_FUEL_TECHNICIAN_ROLE = "FT", _("starbase fuel technician role")
-
-        @classmethod
-        def from_esi(cls, name) -> "StarbaseDetail.Role":
-            my_map = {
-                "alliance_member": cls.ALLIANCE_MEMBER,
-                "config_starbase_equipment_role": cls.CONFIG_STARBASE_EQUIPMENT_ROLE,
-                "corporation_member": cls.CORPORATION_MEMBER,
-                "starbase_fuel_technician_role": cls.STARBASE_FUEL_TECHNICIAN_ROLE,
-            }
-            return my_map[name]
-
-    allow_alliance_members = models.BooleanField()
-    allow_corporation_members = models.BooleanField()
-    anchor_role = models.CharField(max_length=2, choices=Role.choices)
-    attack_if_at_war = models.BooleanField()
-    attack_if_other_security_status_dropping = models.BooleanField()
-    attack_security_status_threshold = models.FloatField(default=None, null=True)
-    attack_standing_threshold = models.FloatField(default=None, null=True)
-    fuel_bay_take_role = models.CharField(max_length=2, choices=Role.choices)
-    fuel_bay_view_role = models.CharField(max_length=2, choices=Role.choices)
-    last_modified_at = models.DateTimeField(
-        help_text="When data was modified on the server."
-    )
-    offline_role = models.CharField(max_length=2, choices=Role.choices)
-    online_role = models.CharField(max_length=2, choices=Role.choices)
-    structure = models.OneToOneField(
-        Structure, on_delete=models.CASCADE, related_name="starbase_detail"
-    )
-    unanchor_role = models.CharField(max_length=2, choices=Role.choices)
-    use_alliance_standings = models.BooleanField()
-
-    def __str__(self) -> str:
-        return str(self.structure)
-
-    def calc_fuel_expires(self) -> Optional[dt.datetime]:
-        """Estimate when fuel will expire for this starbase.
-
-        Estimate will vary due to server caching of remaining fuel blocks.
-        """
-        if self.structure.state is Structure.State.POS_OFFLINE:
-            return None
-        fuel = self.fuels.filter(eve_type__eve_group_id=EveGroupId.FUEL_BLOCK).first()
-        if not fuel:
-            return None
-        seconds = starbases.fuel_duration(
-            starbase_type=self.structure.eve_type,
-            fuel_quantity=fuel.quantity,
-            has_sov=self.structure.owner.has_sov(self.structure.eve_solar_system),
-        )
-        return self.last_modified_at + dt.timedelta(seconds=seconds)
-
-
-class StarbaseDetailFuel(models.Model):
-    """Fuel for a starbase detail."""
-
-    eve_type = models.ForeignKey(EveType, on_delete=models.CASCADE, related_name="+")
-    detail = models.ForeignKey(
-        StarbaseDetail, on_delete=models.CASCADE, related_name="fuels"
-    )
-    quantity = models.IntegerField()
-
-    class Meta:
-        constraints = [
-            models.UniqueConstraint(
-                fields=["detail", "eve_type"], name="functional_pk_starbasedetailfuel"
-            )
-        ]
-
-    def __str__(self) -> str:
-        return f"{self.detail}-{self.eve_type}"
```

### Comparing `aa_structures-2.4.2/structures/static/structures/css/global.css` & `aa_structures-2.5.0/structures/static/structures/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/css/main.css` & `aa_structures-2.5.0/structures/static/structures/css/main.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/Spinner-1s-64px-dark.gif` & `aa_structures-2.5.0/structures/static/structures/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/Spinner-1s-64px-light.gif` & `aa_structures-2.5.0/structures/static/structures/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/eve_symbol_128.png` & `aa_structures-2.5.0/structures/static/structures/img/eve_symbol_128.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/0h.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/0h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/0l.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/0l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/0m.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/0m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/0r.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/0r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/0s.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/0s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/1h.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/1h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/1l.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/1l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/1m.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/1m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/1r.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/1r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/2h.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/2h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/2l.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/2l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/2m.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/2m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/2r.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/2r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/3h.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/3h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/3l.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/3l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/3m.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/3m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/3r.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/3r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/4h.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/4h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/4l.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/4l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/4m.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/4m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/4s.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/4s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/5h.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/5h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/5l.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/5l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/5m.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/5m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/5s.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/5s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/6h.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/6h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/6l.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/6l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/6m.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/6m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/7h.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/7h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/7l.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/7l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/7m.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/7m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/8h.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/8h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/8l.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/8l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/8m.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/8m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/circle.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/circle.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/dustwheel.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/dustwheel.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/h.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/l.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/m.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/noship.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/noship.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/r.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/tyrannis.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_blue.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/tyrannis_blue.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_darkred.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/tyrannis_darkred.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_default.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/tyrannis_default.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_revelations.png` & `aa_structures-2.5.0/structures/static/structures/img/panel/tyrannis_revelations.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/tasks.py` & `aa_structures-2.5.0/structures/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+"""Tasks for Structures."""
+
 from typing import Iterable, Optional
 
 from celery import chain, shared_task
 
 from django.contrib.auth.models import User
 
 from allianceauth.notifications import notify
 from allianceauth.services.hooks import get_extension_logger
 from allianceauth.services.tasks import QueueOnce
 from app_utils.esi import fetch_esi_status
 from app_utils.logging import LoggerAddTag
 
 from . import __title__
 from .app_settings import STRUCTURES_TASKS_TIME_LIMIT
+from .core.notification_types import NotificationType
 from .models import (
     EveSovereigntyMap,
     FuelAlertConfig,
     JumpFuelAlertConfig,
-    NotificationType,
     Owner,
     Webhook,
 )
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 TASK_PRIORITY_HIGH = 2
@@ -38,15 +40,15 @@
         return
     chain(update_sov_map.si(), update_structures.si()).delay()
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
 def update_sov_map():
     """Update sovereignty map from ESI."""
-    EveSovereigntyMap.objects.update_from_esi()
+    EveSovereigntyMap.objects.update_or_create_all_from_esi()
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
 def update_structures():
     """Update all structures for all active owners from ESI."""
     for owner in Owner.objects.all():
         if owner.is_active:
@@ -149,15 +151,15 @@
 def update_existing_notifications(owner_pk: int) -> int:
     """Update structure relation for existing notifications if needed.
 
     Returns number of updated notifications.
     """
     owner = Owner.objects.get(pk=owner_pk)
     notif_need_update_qs = owner.notification_set.filter(
-        notif_type__in=NotificationType.structure_related, structures__isnull=True
+        notif_type__in=NotificationType.structure_related(), structures__isnull=True
     )
     notif_need_update_count = notif_need_update_qs.count()
     updated_count = 0
     if notif_need_update_count > 0:
         for notif in notif_need_update_qs:
             if notif.update_related_structures():
                 updated_count += 1
@@ -168,34 +170,37 @@
             notif_need_update_count,
         )
     return updated_count
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
 def generate_new_timers_for_owner(owner_pk: int):
+    """Generate new timers for given owner."""
     owner = Owner.objects.get(pk=owner_pk)
     owner.add_or_remove_timers_from_notifications()
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
 def send_new_notifications_for_owner(owner_pk: int):
     """Send new notifications to Discord."""
     owner = Owner.objects.get(pk=owner_pk)
     owner.send_new_notifications()
     send_queued_messages_for_webhooks(owner.webhooks.filter(is_active=True))
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
 def send_structure_fuel_notifications_for_config(config_pk: int):
+    """Send structure fuel notifications for a config."""
     FuelAlertConfig.objects.get(pk=config_pk).send_new_notifications()
     send_queued_messages_for_webhooks(FuelAlertConfig.relevant_webhooks())
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
 def send_jump_fuel_notifications_for_config(config_pk: int):
+    """Send jump fuel notifications for a config."""
     JumpFuelAlertConfig.objects.get(pk=config_pk).send_new_notifications()
     send_queued_messages_for_webhooks(JumpFuelAlertConfig.relevant_webhooks())
 
 
 def send_queued_messages_for_webhooks(webhooks: Iterable[Webhook]):
     """Send queued message for given webhooks."""
     for webhook in webhooks:
@@ -216,26 +221,28 @@
     webhook_pk, user_pk: Optional[int] = None
 ) -> None:
     """Send test notification to given webhook."""
     webhook = Webhook.objects.get(pk=webhook_pk)
     user = _get_user(user_pk)
     send_report, send_success = webhook.send_test_message(user)
     if user:
-        message = 'Test notification to webhook "{}" {}.\n'.format(
-            webhook, "completed successfully" if send_success else "has failed"
-        )
-        if not send_success:
-            message += "Error: {}".format(send_report)
+        result_text = "completed successfully" if send_success else "has failed"
+        message = f"Test notification to webhook {webhook} {result_text}.\n"
+        if send_success:
+            user_text = "OK"
+            level = "success"
+        else:
+            user_text = "FAILED"
+            level = "danger"
+            message += f"Error: {send_report}"
         notify(
             user=user,
-            title='{}: Test notification to "{}": {}'.format(
-                __title__, webhook, "OK" if send_success else "FAILED"
-            ),
+            title=f"{__title__}: Test notification to {webhook}: {user_text}",
             message=message,
-            level="success" if send_success else "danger",
+            level=level,
         )
 
 
 def _get_user(user_pk: Optional[int]) -> Optional[User]:
     """Fetch the user or return None."""
     if not user_pk:
         return None
```

### Comparing `aa_structures-2.4.2/structures/templates/structures/main.html` & `aa_structures-2.5.0/structures/templates/structures/main.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/templates/structures/modals/fitting_gfx.html` & `aa_structures-2.5.0/structures/templates/structures/modals/fitting_gfx.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/templates/structures/modals/poco_details.html` & `aa_structures-2.5.0/structures/templates/structures/modals/poco_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/templates/structures/modals/starbase_detail.html` & `aa_structures-2.5.0/structures/templates/structures/modals/starbase_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/templates/structures/modals/structure_details.html` & `aa_structures-2.5.0/structures/templates/structures/modals/structure_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/templates/structures/modals/tab_general_detail.html` & `aa_structures-2.5.0/structures/templates/structures/modals/tab_general_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/templates/structures/partials/jump_gates_list.html` & `aa_structures-2.5.0/structures/templates/structures/partials/jump_gates_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/templates/structures/partials/poco_list.html` & `aa_structures-2.5.0/structures/templates/structures/partials/poco_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/templates/structures/partials/structure_list.html` & `aa_structures-2.5.0/structures/templates/structures/partials/structure_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/templates/structures/partials/structure_summary.html` & `aa_structures-2.5.0/structures/templates/structures/partials/structure_summary.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/templates/structures/templatetags/list_item.html` & `aa_structures-2.5.0/structures/templates/structures/templatetags/list_item.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/templatetags/structures.py` & `aa_structures-2.5.0/structures/templatetags/structures.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Templatetags for Structures."""
+
 from django import template
 from eveuniverse.models import EveType
 
 register = template.Library()
 
 
 @register.inclusion_tag("structures/templatetags/detail_title.html")
```

### Comparing `aa_structures-2.4.2/structures/tests/core/test_notification_embeds.py` & `aa_structures-2.5.0/structures/tests/core/notification_embeds/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,58 +4,56 @@
 
 from django.test import TestCase, override_settings
 from django.utils.timezone import now
 from eveuniverse.models import EveEntity
 
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
-from structures.core import notification_embeds as ne
-from structures.core.notification_embeds import (
-    NotificationBaseEmbed,
-    NotificationTowerReinforcedExtra,
+from structures.core.notification_embeds import NotificationBaseEmbed
+from structures.core.notification_embeds.billing_embeds import BillType
+from structures.core.notification_embeds.moonmining_embeds import (
+    NotificationMoonminningExtractionFinished,
 )
-from structures.models.notifications import (
-    Notification,
-    NotificationType,
-    Structure,
-    Webhook,
+from structures.core.notification_embeds.tower_embeds import (
+    NotificationTowerReinforcedExtra,
 )
-
-from ..testdata.factories import (
+from structures.core.notification_types import NotificationType
+from structures.models.notifications import Notification, Structure, Webhook
+from structures.tests.testdata.factories import (
     create_notification,
     create_owner_from_user,
     create_starbase,
 )
-from ..testdata.factories_2 import (
+from structures.tests.testdata.factories_2 import (
     EveEntityAllianceFactory,
     GeneratedNotificationFactory,
     NotificationFactory,
     OwnerFactory,
     WebhookFactory,
 )
-from ..testdata.helpers import (
+from structures.tests.testdata.helpers import (
     create_structures,
     load_entities,
     load_notification_entities,
     markdown_to_plain,
     set_owner_character,
 )
-from ..testdata.load_eveuniverse import load_eveuniverse
+from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
 MODULE_PATH = "structures.core.notification_embeds"
 
 
 class TestBilType(TestCase):
     def test_should_create_from_valid_id(self):
-        self.assertEqual(ne.BillType.to_enum(7), ne.BillType.INFRASTRUCTURE_HUB)
+        self.assertEqual(BillType.to_enum(7), BillType.INFRASTRUCTURE_HUB)
 
     def test_should_create_from_invalid_id(self):
         for bill_id in range(7):
             with self.subTest(bill_id=bill_id):
-                self.assertEqual(ne.BillType.to_enum(bill_id), ne.BillType.UNKNOWN)
+                self.assertEqual(BillType.to_enum(bill_id), BillType.UNKNOWN)
 
 
 class TestNotificationEmbeds(TestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
@@ -63,18 +61,18 @@
         _, cls.owner = set_owner_character(character_id=1001)
         load_notification_entities(cls.owner)
 
     def test_should_create_obj_from_notification(self):
         # given
         notification = Notification.objects.get(notification_id=1000000403)
         # when
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         # then
         self.assertIsInstance(
-            notification_embed, ne.NotificationMoonminningExtractionFinished
+            notification_embed, NotificationMoonminningExtractionFinished
         )
         self.assertEqual(
             str(notification_embed), "1000000403:MoonminingExtractionFinished"
         )
         self.assertEqual(
             repr(notification_embed),
             "NotificationMoonminningExtractionFinished(notification=Notification("
@@ -90,23 +88,23 @@
             sender=EveEntity.objects.get(id=2001),
             timestamp=now(),
             notif_type="XXXUnsupportedNotificationTypeXXX",
             last_updated=now(),
         )
         # when / then
         with self.assertRaises(NotImplementedError):
-            ne.NotificationBaseEmbed.create(notification)
+            NotificationBaseEmbed.create(notification)
 
     def test_should_require_notification_for_init(self):
         with self.assertRaises(TypeError):
-            ne.NotificationBaseEmbed(notification="dummy")
+            NotificationBaseEmbed(notification="dummy")
 
     def test_should_require_notification_for_factory(self):
         with self.assertRaises(TypeError):
-            ne.NotificationBaseEmbed.create(notification="dummy")
+            NotificationBaseEmbed.create(notification="dummy")
 
 
 class TestNotificationEmbedsGenerate(TestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
@@ -115,125 +113,125 @@
         load_notification_entities(cls.owner)
         cls.webhook = WebhookFactory()
         cls.owner.webhooks.add(cls.webhook)
 
     def test_should_generate_embed_from_notification(self):
         # given
         notification = Notification.objects.get(notification_id=1000000403)
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         # when
         discord_embed = notification_embed.generate_embed()
         # then
         self.assertIsInstance(discord_embed, dhooks_lite.Embed)
         self.assertEqual(discord_embed.footer.text, "Eve Online")
         self.assertIn("eve_symbol_128.png", discord_embed.footer.icon_url)
 
     def test_should_generate_embed_from_notification_with_custom_color(self):
         # given
         notification = Notification.objects.get(notification_id=1000000403)
         notification._color_override = Webhook.Color.SUCCESS
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         # when
         discord_embed = notification_embed.generate_embed()
         # then
         self.assertIsInstance(discord_embed, dhooks_lite.Embed)
         self.assertEqual(discord_embed.color, Webhook.Color.SUCCESS)
 
     def test_should_generate_embed_from_notification_without_custom_color(self):
         # given
         notification = Notification.objects.get(notification_id=1000000403)
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         # when
         discord_embed = notification_embed.generate_embed()
         # then
         self.assertIsInstance(discord_embed, dhooks_lite.Embed)
         self.assertNotEqual(discord_embed.color, Webhook.Color.SUCCESS)
 
     def test_should_generate_embed_from_notification_with_ping_type_override(self):
         # given
         notification = Notification.objects.get(notification_id=1000000403)
         notification._ping_type_override = Webhook.PingType.EVERYONE
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         # when
         notification_embed.generate_embed()
         # then
         self.assertEqual(notification_embed.ping_type, Webhook.PingType.EVERYONE)
 
     def test_should_generate_embed_for_all_supported_esi_notification_types(self):
-        types_tested = set()
-        for notification in Notification.objects.select_related(
-            "owner", "sender"
-        ).all():
-            if notification.notif_type in NotificationType.values:
+        for notif_type in NotificationType.esi_notifications():
+            with self.subTest(notif_type=notif_type):
                 # given
-                notification_embed = ne.NotificationBaseEmbed.create(notification)
+                notification = (
+                    Notification.objects.select_related("owner", "sender")
+                    .filter(notif_type=notif_type)
+                    .first()
+                )
+                notification_embed = NotificationBaseEmbed.create(notification)
                 # when
                 discord_embed = notification_embed.generate_embed()
                 # then
                 self.assertIsInstance(discord_embed, dhooks_lite.Embed)
-                types_tested.add(notification.notif_type)
-        self.assertSetEqual(NotificationType.esi_notifications, types_tested)
 
     def test_should_set_ping_everyone_for_color_danger(self):
         # given
         notification = Notification.objects.get(notification_id=1000000513)
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         notification_embed._color = Webhook.Color.DANGER
         # when
         notification_embed.generate_embed()
         # then
         self.assertEqual(notification_embed.ping_type, Webhook.PingType.EVERYONE)
 
     def test_should_set_ping_everyone_for_color_warning(self):
         # given
         notification = Notification.objects.get(notification_id=1000000513)
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         notification_embed._color = Webhook.Color.WARNING
         # when
         notification_embed.generate_embed()
         # then
         self.assertEqual(notification_embed.ping_type, Webhook.PingType.HERE)
 
     def test_should_not_set_ping_everyone_for_color_info(self):
         # given
         notification = Notification.objects.get(notification_id=1000000513)
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         notification_embed._color = Webhook.Color.INFO
         # when
         notification_embed.generate_embed()
         # then
         self.assertEqual(notification_embed.ping_type, Webhook.PingType.NONE)
 
     def test_should_not_set_ping_everyone_for_color_success(self):
         # given
         notification = Notification.objects.get(notification_id=1000000513)
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         notification_embed._color = Webhook.Color.SUCCESS
         # when
         notification_embed.generate_embed()
         # then
         self.assertEqual(notification_embed.ping_type, Webhook.PingType.NONE)
 
     @override_settings(DEBUG=True)
     def test_should_set_footer_in_developer_mode(self):
         # given
         notification = Notification.objects.get(notification_id=1000000403)
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         # when
         discord_embed = notification_embed.generate_embed()
         # then
         self.assertTrue(discord_embed.footer)
 
     def test_should_set_special_footer_for_generated_notifications(self):
         # given
         structure = Structure.objects.get(id=1000000000001)
         notification = Notification.create_from_structure(
             structure, notif_type=NotificationType.STRUCTURE_FUEL_ALERT
         )
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         # when
         discord_embed = notification_embed.generate_embed()
         # then
         self.assertEqual(discord_embed.footer.text, "Structures")
         self.assertIn("structures_logo.png", discord_embed.footer.icon_url)
 
 
@@ -267,15 +265,15 @@
             "wants": [{"quantity": 120, "typeID": 4051}],
         }
         notification = create_notification(
             owner=self.owner,
             notif_type=NotificationType.TOWER_RESOURCE_ALERT_MSG,
             data=data,
         )
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         # when
         discord_embed = notification_embed.generate_embed()
         # then
         description = markdown_to_plain(discord_embed.description)
         self.assertIn("is running out of fuel in 3 hours", description)
 
     def test_should_generate_embed_for_generated_tower_resource_alert(self):
@@ -286,15 +284,15 @@
             eve_solar_system_id=self.solar_system_id,
             eve_type_id=self.type_id,
             fuel_expires_at=now() + dt.timedelta(hours=2, seconds=20),
         )
         notification = Notification.create_from_structure(
             structure=structure, notif_type=NotificationType.TOWER_RESOURCE_ALERT_MSG
         )
-        notification_embed = ne.NotificationBaseEmbed.create(notification)
+        notification_embed = NotificationBaseEmbed.create(notification)
         # when
         discord_embed = notification_embed.generate_embed()
         # then
         description = markdown_to_plain(discord_embed.description)
         self.assertIn("is running out of fuel in 2 hours", description)
```

### Comparing `aa_structures-2.4.2/structures/tests/core/test_notification_structuretimers.py` & `aa_structures-2.5.0/structures/tests/core/test_notification_structuretimers.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,22 @@
     from eveuniverse.models import EveSolarSystem, EveType
 
     from allianceauth.eveonline.models import EveAllianceInfo, EveCorporationInfo
     from app_utils.testing import NoSocketsTestCase
 
     from structures.core import notification_timers
     from structures.models import Notification
-
-    from ..testdata.factories import create_webhook
-    from ..testdata.factories_2 import GeneratedNotificationFactory
-    from ..testdata.helpers import (
+    from structures.tests.testdata.factories import create_webhook
+    from structures.tests.testdata.factories_2 import GeneratedNotificationFactory
+    from structures.tests.testdata.helpers import (
         create_structures,
         load_notification_entities,
         set_owner_character,
     )
-    from ..testdata.load_eveuniverse import load_eveuniverse
+    from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
     MODULE_PATH = "structures.core.notification_timers"
 
     @patch(
         "structuretimers.models._task_calc_timer_distances_for_all_staging_systems",
         Mock(),
     )
```

### Comparing `aa_structures-2.4.2/structures/tests/core/test_notifications_timerboard.py` & `aa_structures-2.5.0/structures/tests/core/test_notifications_timerboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,22 @@
     from unittest.mock import Mock, patch
 
     from allianceauth.timerboard.models import Timer as AuthTimer
     from app_utils.testing import NoSocketsTestCase
 
     from structures.core import notification_timers
     from structures.models import Notification
-
-    from ..testdata.factories import create_webhook
-    from ..testdata.factories_2 import GeneratedNotificationFactory
-    from ..testdata.helpers import (
+    from structures.tests.testdata.factories import create_webhook
+    from structures.tests.testdata.factories_2 import GeneratedNotificationFactory
+    from structures.tests.testdata.helpers import (
         create_structures,
         load_notification_entities,
         set_owner_character,
     )
-    from ..testdata.load_eveuniverse import load_eveuniverse
+    from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
     MODULE_PATH = "structures.core.notification_timers"
 
     @patch(
         "structuretimers.models._task_calc_timer_distances_for_all_staging_systems",
         Mock(),
     )
```

### Comparing `aa_structures-2.4.2/structures/tests/core/test_serializers.py` & `aa_structures-2.5.0/structures/tests/core/test_serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import List
 
 from django.test import RequestFactory
 
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
-from ...core.serializers import PocoListSerializer, StructureListSerializer
-from ...models import Structure
-from ..testdata.factories import (
+from structures.core.serializers import PocoListSerializer, StructureListSerializer
+from structures.models import Structure
+from structures.tests.testdata.factories import (
     create_owner_from_user,
     create_poco,
     create_starbase,
     create_upwell_structure,
 )
-from ..testdata.helpers import load_entities
-from ..testdata.load_eveuniverse import load_eveuniverse
+from structures.tests.testdata.helpers import load_entities
+from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
 
 def to_dict(lst: List[dict], key="id"):
     return {obj[key]: obj for obj in lst}
 
 
 class TestStructureListSerializer(NoSocketsTestCase):
```

### Comparing `aa_structures-2.4.2/structures/tests/core/test_sovereignty.py` & `aa_structures-2.5.0/structures/tests/core/test_sovereignty.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 
 class TestSovereignty(NoSocketsTestCase):
     def test_should_return_type_id_or_none(self):
         my_map = [(1, EveTypeId.TCU), (2, EveTypeId.IHUB), (3, None), (0, None)]
         for input, expected in my_map:
             with self.subTest(input=input):
-                self.assertEqual(sovereignty.type_id_from_event_type(input), expected)
+                self.assertEqual(sovereignty.event_type_to_type_id(input), expected)
 
     def test_should_return_structure_type_names(self):
         my_map = [(1, "TCU"), (2, "I-HUB"), (3, "Other"), (0, "Other")]
         for input, expected in my_map:
             with self.subTest(input=input):
                 self.assertEqual(
-                    sovereignty.structure_type_name_from_event_type(input), expected
+                    sovereignty.event_type_to_structure_type_name(input), expected
                 )
```

### Comparing `aa_structures-2.4.2/structures/tests/core/test_starbases.py` & `aa_structures-2.5.0/structures/tests/core/test_starbases.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from eveuniverse.models import EveType
 
 from app_utils.testing import NoSocketsTestCase
 
-from ...core import starbases
-from ..testdata.load_eveuniverse import load_eveuniverse
+from structures.core import starbases
+from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
 
 class TestStarbases(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
```

### Comparing `aa_structures-2.4.2/structures/tests/models/test_eveuniverse.py` & `aa_structures-2.5.0/structures/tests/models/test_eveuniverse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from eveuniverse.models import EveSolarSystem
 
 from app_utils.testing import NoSocketsTestCase
 
-from ...models import EveSovereigntyMap, EveSpaceType
-from ..testdata.load_eveuniverse import load_eveuniverse
+from structures.models import EveSovereigntyMap, EveSpaceType
+from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
 MODULE_PATH = "structures.models.eveuniverse"
 
 
 class TestEveSovereigntyMap(NoSocketsTestCase):
     def test_str(self):
         obj = EveSovereigntyMap(solar_system_id=99)
```

### Comparing `aa_structures-2.4.2/structures/tests/models/test_notifications_1.py` & `aa_structures-2.5.0/structures/tests/models/test_notifications_1.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 from unittest.mock import patch
 
 from django.utils.timezone import now
 from eveuniverse.models import EveEntity
 
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
-from ...models import Notification, NotificationType, Structure, Webhook
-from ..testdata.factories import (
+from structures.core.notification_types import NotificationType
+from structures.models import Notification, Structure, Webhook
+from structures.tests.testdata.factories import (
     create_notification,
     create_owner_from_user,
     create_upwell_structure,
     create_webhook,
 )
-from ..testdata.helpers import (
+from structures.tests.testdata.helpers import (
     create_structures,
     load_entities,
     load_notification_entities,
     set_owner_character,
 )
-from ..testdata.load_eveuniverse import load_eveuniverse
+from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
 MODULE_PATH = "structures.models.notifications"
 
 
 class TestNotification(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
@@ -118,75 +119,75 @@
         load_notification_entities(cls.owner)
 
     def test_should_not_filter_non_alliance_notifications_1(self):
         # given
         self.owner.is_alliance_main = False
         self.owner.save()
         notifs = self.owner.notification_set.exclude(
-            notif_type__in=NotificationType.relevant_for_alliance_level
+            notif_type__in=NotificationType.relevant_for_alliance_level()
         )
         # when/then
         for notif in notifs:
             with self.subTest(notif=str(notif)):
                 self.assertFalse(notif.filter_for_alliance_level())
 
     def test_should_not_filter_non_alliance_notifications_2(self):
         # given
         self.owner.is_alliance_main = True
         self.owner.save()
         notifs = self.owner.notification_set.exclude(
-            notif_type__in=NotificationType.relevant_for_alliance_level
+            notif_type__in=NotificationType.relevant_for_alliance_level()
         )
         # when/then
         for notif in notifs:
             with self.subTest(notif=str(notif)):
                 self.assertFalse(notif.filter_for_alliance_level())
 
     def test_should_filter_alliance_notifications(self):
         # given
         self.owner.is_alliance_main = False
         self.owner.save()
         notifs = self.owner.notification_set.filter(
-            notif_type__in=NotificationType.relevant_for_alliance_level
+            notif_type__in=NotificationType.relevant_for_alliance_level()
         )
         # when/then
         for notif in notifs:
             with self.subTest(notif=str(notif)):
                 self.assertTrue(notif.filter_for_alliance_level())
 
     def test_should_not_filter_alliance_notifications_1(self):
         # given
         self.owner.is_alliance_main = True
         self.owner.save()
         notifs = self.owner.notification_set.filter(
-            notif_type__in=NotificationType.relevant_for_alliance_level
+            notif_type__in=NotificationType.relevant_for_alliance_level()
         )
         # when/then
         for notif in notifs:
             with self.subTest(notif=str(notif)):
                 self.assertFalse(notif.filter_for_alliance_level())
 
     def test_should_not_filter_alliance_notifications_2(self):
         # given
         self.owner.is_alliance_main = True
         self.owner.save()
         notifs = self.owner.notification_set.filter(
-            notif_type__in=NotificationType.relevant_for_alliance_level
+            notif_type__in=NotificationType.relevant_for_alliance_level()
         )
         # when/then
         for notif in notifs:
             with self.subTest(notif=str(notif)):
                 self.assertFalse(notif.filter_for_alliance_level())
 
     def test_should_not_filter_alliance_notifications_3(self):
         # given
         _, owner = set_owner_character(character_id=1102)  # corp with no alliance
         load_notification_entities(owner)
         notifs = self.owner.notification_set.filter(
-            notif_type__in=NotificationType.relevant_for_alliance_level
+            notif_type__in=NotificationType.relevant_for_alliance_level()
         )
         # when/then
         for notif in notifs:
             with self.subTest(notif=str(notif)):
                 self.assertFalse(notif.filter_for_alliance_level())
 
 
@@ -331,30 +332,30 @@
         self.assertQuerysetEqual(
             result_qs, Webhook.objects.filter(pk=webhook_structure.pk)
         )
 
     def test_should_return_owner_webhooks_when_notif_has_multiple_structures(self):
         # given
         webhook_owner = create_webhook(
-            notification_types=[NotificationType.STRUCTURE_UNDER_ATTACK]
+            notification_types=[NotificationType.STRUCTURE_REINFORCEMENT_CHANGED]
         )
         self.owner.webhooks.add(webhook_owner)
         structure_1 = create_upwell_structure(owner=self.owner)
         webhook_structure = create_webhook(
-            notification_types=[NotificationType.STRUCTURE_UNDER_ATTACK]
+            notification_types=[NotificationType.STRUCTURE_REINFORCEMENT_CHANGED]
         )
         structure_1.webhooks.add(webhook_structure)
         structure_2 = create_upwell_structure(owner=self.owner)
         webhook_structure = create_webhook(
-            notification_types=[NotificationType.STRUCTURE_UNDER_ATTACK]
+            notification_types=[NotificationType.STRUCTURE_REINFORCEMENT_CHANGED]
         )
         structure_2.webhooks.add(webhook_structure)
         notif = create_notification(
             owner=self.owner,
-            notif_type=NotificationType.STRUCTURE_UNDER_ATTACK,
+            notif_type=NotificationType.STRUCTURE_REINFORCEMENT_CHANGED,
             text=f"allStructureInfo:\n- - {structure_1.id}\n  - {structure_1}\n  - 35825\n- - {structure_2.id}\n  - {structure_2}\n  - 35825\nhour: 19\nnumStructures: 1\ntimestamp: 132141703753688216\nweekday: 255\n",
         )
         # when
         result_qs = notif.relevant_webhooks()
         # then
         self.assertQuerysetEqual(result_qs, Webhook.objects.filter(pk=webhook_owner.pk))
 
@@ -601,15 +602,15 @@
             with self.subTest(notif_type=notif.notif_type):
                 if notif.notif_type in NotificationType.values:
                     self.assertFalse(notif.is_sent)
                     self.assertTrue(notif.send_to_webhook(self.webhook))
                     types_tested.add(notif.notif_type)
 
         # make sure we have tested all existing esi notification types
-        self.assertSetEqual(NotificationType.esi_notifications, types_tested)
+        self.assertSetEqual(NotificationType.esi_notifications(), types_tested)
 
     def test_should_create_notification_for_structure_refueled(self, mock_send_message):
         # given
         mock_send_message.return_value = 1
         structure = Structure.objects.get(id=1000000000001)
         notif = Notification.create_from_structure(
             structure, NotificationType.STRUCTURE_REFUELED_EXTRA
@@ -728,270 +729,7 @@
         obj = Notification.objects.get(notification_id=1000000509)
         # when
         result = obj.send_to_webhook(webhook_normal)
         # then
         self.assertTrue(result)
         _, kwargs = mock_send_message.call_args
         self.assertNotIn("@everyone", kwargs["content"])
-
-
-class TestNotificationType(NoSocketsTestCase):
-    def test_should_return_enabled_values_only(self):
-        # when
-        with patch(MODULE_PATH + ".STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS", False):
-            values = NotificationType.values_enabled
-        # then
-        self.assertNotIn(NotificationType.STRUCTURE_REFUELED_EXTRA, values)
-        self.assertNotIn(NotificationType.TOWER_REFUELED_EXTRA, values)
-
-    def test_should_return_all_values(self):
-        # when
-        with patch(MODULE_PATH + ".STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS", True):
-            values = NotificationType.values_enabled
-        # then
-        self.assertIn(NotificationType.STRUCTURE_REFUELED_EXTRA, values)
-        self.assertIn(NotificationType.TOWER_REFUELED_EXTRA, values)
-
-    def test_should_return_enabled_choices_only(self):
-        # when
-        with patch(MODULE_PATH + ".STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS", False):
-            choices = NotificationType.choices_enabled
-        # then
-        types = {choice[0] for choice in choices}
-        self.assertNotIn(NotificationType.STRUCTURE_REFUELED_EXTRA, types)
-        self.assertNotIn(NotificationType.TOWER_REFUELED_EXTRA, types)
-
-    def test_should_return_all_choices(self):
-        # when
-        with patch(MODULE_PATH + ".STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS", True):
-            choices = NotificationType.choices_enabled
-        # then
-        types = {choice[0] for choice in choices}
-        self.assertIn(NotificationType.STRUCTURE_REFUELED_EXTRA, types)
-        self.assertIn(NotificationType.TOWER_REFUELED_EXTRA, types)
-
-    def test_has_correct_esi_values(self):
-        # given
-        esi_valid_notification_types = {
-            "AcceptedAlly",
-            "AcceptedSurrender",
-            "AgentRetiredTrigravian",
-            "AllAnchoringMsg",
-            "AllMaintenanceBillMsg",
-            "AllStrucInvulnerableMsg",
-            "AllStructVulnerableMsg",
-            "AllWarCorpJoinedAllianceMsg",
-            "AllWarDeclaredMsg",
-            "AllWarInvalidatedMsg",
-            "AllWarRetractedMsg",
-            "AllWarSurrenderMsg",
-            "AllianceCapitalChanged",
-            "AllianceWarDeclaredV2",
-            "AllyContractCancelled",
-            "AllyJoinedWarAggressorMsg",
-            "AllyJoinedWarAllyMsg",
-            "AllyJoinedWarDefenderMsg",
-            "BattlePunishFriendlyFire",
-            "BillOutOfMoneyMsg",
-            "BillPaidCorpAllMsg",
-            "BountyClaimMsg",
-            "BountyESSShared",
-            "BountyESSTaken",
-            "BountyPlacedAlliance",
-            "BountyPlacedChar",
-            "BountyPlacedCorp",
-            "BountyYourBountyClaimed",
-            "BuddyConnectContactAdd",
-            "CharAppAcceptMsg",
-            "CharAppRejectMsg",
-            "CharAppWithdrawMsg",
-            "CharLeftCorpMsg",
-            "CharMedalMsg",
-            "CharTerminationMsg",
-            "CloneActivationMsg",
-            "CloneActivationMsg2",
-            "CloneMovedMsg",
-            "CloneRevokedMsg1",
-            "CloneRevokedMsg2",
-            "CombatOperationFinished",
-            "ContactAdd",
-            "ContactEdit",
-            "ContainerPasswordMsg",
-            "ContractRegionChangedToPochven",
-            "CorpAllBillMsg",
-            "CorpAppAcceptMsg",
-            "CorpAppInvitedMsg",
-            "CorpAppNewMsg",
-            "CorpAppRejectCustomMsg",
-            "CorpAppRejectMsg",
-            "CorpBecameWarEligible",
-            "CorpDividendMsg",
-            "CorpFriendlyFireDisableTimerCompleted",
-            "CorpFriendlyFireDisableTimerStarted",
-            "CorpFriendlyFireEnableTimerCompleted",
-            "CorpFriendlyFireEnableTimerStarted",
-            "CorpKicked",
-            "CorpLiquidationMsg",
-            "CorpNewCEOMsg",
-            "CorpNewsMsg",
-            "CorpNoLongerWarEligible",
-            "CorpOfficeExpirationMsg",
-            "CorpStructLostMsg",
-            "CorpTaxChangeMsg",
-            "CorpVoteCEORevokedMsg",
-            "CorpVoteMsg",
-            "CorpWarDeclaredMsg",
-            "CorpWarDeclaredV2",
-            "CorpWarFightingLegalMsg",
-            "CorpWarInvalidatedMsg",
-            "CorpWarRetractedMsg",
-            "CorpWarSurrenderMsg",
-            "CustomsMsg",
-            "DeclareWar",
-            "DistrictAttacked",
-            "DustAppAcceptedMsg",
-            "ESSMainBankLink",
-            "EntosisCaptureStarted",
-            "ExpertSystemExpired",
-            "ExpertSystemExpiryImminent",
-            "FWAllianceKickMsg",
-            "FWAllianceWarningMsg",
-            "FWCharKickMsg",
-            "FWCharRankGainMsg",
-            "FWCharRankLossMsg",
-            "FWCharWarningMsg",
-            "FWCorpJoinMsg",
-            "FWCorpKickMsg",
-            "FWCorpLeaveMsg",
-            "FWCorpWarningMsg",
-            "FacWarCorpJoinRequestMsg",
-            "FacWarCorpJoinWithdrawMsg",
-            "FacWarCorpLeaveRequestMsg",
-            "FacWarCorpLeaveWithdrawMsg",
-            "FacWarLPDisqualifiedEvent",
-            "FacWarLPDisqualifiedKill",
-            "FacWarLPPayoutEvent",
-            "FacWarLPPayoutKill",
-            "GameTimeAdded",
-            "GameTimeReceived",
-            "GameTimeSent",
-            "GiftReceived",
-            "IHubDestroyedByBillFailure",
-            "IncursionCompletedMsg",
-            "IndustryOperationFinished",
-            "IndustryTeamAuctionLost",
-            "IndustryTeamAuctionWon",
-            "InfrastructureHubBillAboutToExpire",
-            "InsuranceExpirationMsg",
-            "InsuranceFirstShipMsg",
-            "InsuranceInvalidatedMsg",
-            "InsuranceIssuedMsg",
-            "InsurancePayoutMsg",
-            "InvasionCompletedMsg",
-            "InvasionSystemLogin",
-            "InvasionSystemStart",
-            "JumpCloneDeletedMsg1",
-            "JumpCloneDeletedMsg2",
-            "KillReportFinalBlow",
-            "KillReportVictim",
-            "KillRightAvailable",
-            "KillRightAvailableOpen",
-            "KillRightEarned",
-            "KillRightUnavailable",
-            "KillRightUnavailableOpen",
-            "KillRightUsed",
-            "LocateCharMsg",
-            "MadeWarMutual",
-            "MercOfferRetractedMsg",
-            "MercOfferedNegotiationMsg",
-            "MissionCanceledTriglavian",
-            "MissionOfferExpirationMsg",
-            "MissionTimeoutMsg",
-            "MoonminingAutomaticFracture",
-            "MoonminingExtractionCancelled",
-            "MoonminingExtractionFinished",
-            "MoonminingExtractionStarted",
-            "MoonminingLaserFired",
-            "MutualWarExpired",
-            "MutualWarInviteAccepted",
-            "MutualWarInviteRejected",
-            "MutualWarInviteSent",
-            "NPCStandingsGained",
-            "NPCStandingsLost",
-            "OfferToAllyRetracted",
-            "OfferedSurrender",
-            "OfferedToAlly",
-            "OfficeLeaseCanceledInsufficientStandings",
-            "OldLscMessages",
-            "OperationFinished",
-            "OrbitalAttacked",
-            "OrbitalReinforced",
-            "OwnershipTransferred",
-            "RaffleCreated",
-            "RaffleExpired",
-            "RaffleFinished",
-            "ReimbursementMsg",
-            "ResearchMissionAvailableMsg",
-            "RetractsWar",
-            "SeasonalChallengeCompleted",
-            "SovAllClaimAquiredMsg",
-            "SovAllClaimLostMsg",
-            "SovCommandNodeEventStarted",
-            "SovCorpBillLateMsg",
-            "SovCorpClaimFailMsg",
-            "SovDisruptorMsg",
-            "SovStationEnteredFreeport",
-            "SovStructureDestroyed",
-            "SovStructureReinforced",
-            "SovStructureSelfDestructCancel",
-            "SovStructureSelfDestructFinished",
-            "SovStructureSelfDestructRequested",
-            "SovereigntyIHDamageMsg",
-            "SovereigntySBUDamageMsg",
-            "SovereigntyTCUDamageMsg",
-            "StationAggressionMsg1",
-            "StationAggressionMsg2",
-            "StationConquerMsg",
-            "StationServiceDisabled",
-            "StationServiceEnabled",
-            "StationStateChangeMsg",
-            "StoryLineMissionAvailableMsg",
-            "StructureAnchoring",
-            "StructureCourierContractChanged",
-            "StructureDestroyed",
-            "StructureFuelAlert",
-            "StructureImpendingAbandonmentAssetsAtRisk",
-            "StructureItemsDelivered",
-            "StructureItemsMovedToSafety",
-            "StructureLostArmor",
-            "StructureLostShields",
-            "StructureOnline",
-            "StructureServicesOffline",
-            "StructureUnanchoring",
-            "StructureUnderAttack",
-            "StructureWentHighPower",
-            "StructureWentLowPower",
-            "StructuresJobsCancelled",
-            "StructuresJobsPaused",
-            "StructuresReinforcementChanged",
-            "TowerAlertMsg",
-            "TowerResourceAlertMsg",
-            "TransactionReversalMsg",
-            "TutorialMsg",
-            "WarAdopted",
-            "WarAllyInherited",
-            "WarAllyOfferDeclinedMsg",
-            "WarConcordInvalidates",
-            "WarDeclared",
-            "WarEndedHqSecurityDrop",
-            "WarHQRemovedFromSpace",
-            "WarInherited",
-            "WarInvalid",
-            "WarRetracted",
-            "WarRetractedByConcord",
-            "WarSurrenderDeclinedMsg",
-            "WarSurrenderOfferMsg",
-        }
-        # when
-        for ntype in NotificationType.esi_notifications:
-            with self.subTest(notification_type=ntype):
-                self.assertIn(ntype, esi_valid_notification_types)
```

### Comparing `aa_structures-2.4.2/structures/tests/models/test_notifications_2.py` & `aa_structures-2.5.0/structures/tests/models/test_notifications_2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import datetime as dt
 from unittest.mock import patch
 
 from django.utils.timezone import now
 
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
-from ...constants import EveTypeId
-from ...models import (
+from structures.constants import EveTypeId
+from structures.core.notification_types import NotificationType
+from structures.models import (
     FuelAlert,
     FuelAlertConfig,
     JumpFuelAlert,
     JumpFuelAlertConfig,
     Notification,
-    NotificationType,
     Structure,
     StructureItem,
     Webhook,
 )
-from ..testdata.factories import (
+from structures.tests.testdata.factories import (
     create_jump_gate,
     create_notification,
     create_owner_from_user,
     create_poco,
     create_starbase,
     create_structure_item,
     create_upwell_structure,
     create_webhook,
 )
-from ..testdata.helpers import (
+from structures.tests.testdata.factories_2 import (
+    EveEntityCorporationFactory,
+    NotificationFactory,
+)
+from structures.tests.testdata.helpers import (
     create_structures,
     load_entities,
     load_notification_by_type,
     load_notification_entities,
     set_owner_character,
 )
-from ..testdata.load_eveuniverse import load_eveuniverse
+from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
 MODULE_PATH = "structures.models.notifications"
 
 
 @patch(MODULE_PATH + ".Webhook.send_message", spec=True)
 class TestStructureFuelAlerts(NoSocketsTestCase):
     @classmethod
@@ -800,7 +804,129 @@
         notif = create_notification(owner=self.owner)
         # when
         with patch(MODULE_PATH + ".Notification.calc_related_structures") as m:
             m.return_value = Structure.objects.none()
             result = notif.update_related_structures()
         # then
         self.assertFalse(result)
+
+    def test_should_return_empty_qs_when_structure_id_is_missing(self):
+        # given
+        sender = EveEntityCorporationFactory()
+        notif = NotificationFactory(
+            sender=sender,
+            notif_type=NotificationType.OWNERSHIP_TRANSFERRED.value,
+            text_from_dict={
+                "charID": 1001,
+                "newOwnerCorpID": 2002,
+                "oldOwnerCorpID": 2001,
+                "solarSystemID": 30002537,
+                "structureName": "Test Structure Alpha",
+                "structureTypeID": 35832,
+            },
+        )
+        # when
+        result_qs = notif.calc_related_structures()
+        # then
+        self.assertEqual(list(result_qs), [])
+
+    def test_should_return_empty_qs_when_all_structure_info_is_missing(self):
+        # given
+        sender = EveEntityCorporationFactory()
+        notif = NotificationFactory(
+            sender=sender,
+            notif_type=NotificationType.STRUCTURE_REINFORCEMENT_CHANGED.value,
+            text_from_dict={
+                "hour": 19,
+                "numStructures": 1,
+                "timestamp": 132141703753688216,
+                "weekday": 255,
+            },
+        )
+        # when
+        result_qs = notif.calc_related_structures()
+        # then
+        self.assertEqual(list(result_qs), [])
+
+    def test_should_return_empty_qs_when_planet_id_is_missing(self):
+        # given
+        sender = EveEntityCorporationFactory()
+        notif = NotificationFactory(
+            sender=sender,
+            notif_type=NotificationType.ORBITAL_ATTACKED.value,
+            text_from_dict={
+                "aggressorCorpID": 2011,
+                "aggressorID": 1011,
+                "planetTypeID": 2016,
+                "shieldLevel": 0.9821850015653375,
+                "solarSystemID": 30002537,
+                "typeID": 2233,
+            },
+        )
+        # when
+        result_qs = notif.calc_related_structures()
+        # then
+        self.assertEqual(list(result_qs), [])
+
+    def test_should_return_empty_qs_when_type_id_is_missing(self):
+        # given
+        sender = EveEntityCorporationFactory()
+        notif = NotificationFactory(
+            sender=sender,
+            notif_type=NotificationType.ORBITAL_ATTACKED.value,
+            text_from_dict={
+                "aggressorCorpID": 2011,
+                "aggressorID": 1011,
+                "planetID": 40161469,
+                "planetTypeID": 2016,
+                "shieldLevel": 0.9821850015653375,
+                "solarSystemID": 30002537,
+            },
+        )
+        # when
+        result_qs = notif.calc_related_structures()
+        # then
+        self.assertEqual(list(result_qs), [])
+
+    def test_should_return_empty_qs_when_moon_id_is_missing(self):
+        # given
+        sender = EveEntityCorporationFactory()
+        notif = NotificationFactory(
+            sender=sender,
+            notif_type=NotificationType.TOWER_ALERT_MSG.value,
+            text_from_dict={
+                "aggressorAllianceID": 3011,
+                "aggressorCorpID": 2011,
+                "aggressorID": 1011,
+                "armorValue": 0.6950949076033535,
+                "hullValue": 1.0,
+                "shieldValue": 0.3950949076033535,
+                "solarSystemID": 30002537,
+                "typeID": 16213,
+            },
+        )
+        # when
+        result_qs = notif.calc_related_structures()
+        # then
+        self.assertEqual(list(result_qs), [])
+
+    def test_should_return_empty_qs_when_moon_type_id_is_missing(self):
+        # given
+        sender = EveEntityCorporationFactory()
+        notif = NotificationFactory(
+            sender=sender,
+            notif_type=NotificationType.TOWER_ALERT_MSG.value,
+            text_from_dict={
+                "aggressorAllianceID": 3011,
+                "aggressorCorpID": 2011,
+                "aggressorID": 1011,
+                "armorValue": 0.6950949076033535,
+                "hullValue": 1.0,
+                "moonID": 40161465,
+                "shieldValue": 0.3950949076033535,
+                "solarSystemID": 30002537,
+            },
+        )
+        # when
+        result_qs = notif.calc_related_structures()
+        # then
+        self.assertEqual(list(result_qs), [])
```

### Comparing `aa_structures-2.4.2/structures/tests/models/test_notifications_3.py` & `aa_structures-2.5.0/structures/tests/models/test_notifications_3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime as dt
 from unittest import mock
 
 from django.utils.timezone import now
 
 from app_utils.testing import NoSocketsTestCase
 
-from structures.models import GeneratedNotification, NotificationType, Structure
-
-from ..testdata.factories_2 import (
+from structures.core.notification_types import NotificationType
+from structures.models import GeneratedNotification, Structure
+from structures.tests.testdata.factories_2 import (
     GeneratedNotificationFactory,
     NotificationFactory,
     OwnerFactory,
     StarbaseFactory,
     StructureFactory,
 )
-from ..testdata.load_eveuniverse import load_eveuniverse
+from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
 MODULE_PATH = "structures.models.notifications"
 
 
 class TestGeneratedNotification(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
@@ -144,15 +144,15 @@
     @mock.patch(MODULE_PATH + ".STRUCTURES_ADD_TIMERS", True)
     def test_should_not_process_timers_for_non_supported_notification_types(
         self, mock_add_or_remove_timer
     ):
         mock_add_or_remove_timer.return_value = True
         unsupported_notif_types = {
             obj for obj in NotificationType
-        } - NotificationType.relevant_for_timerboard
+        } - NotificationType.relevant_for_timerboard()
         for notif_type in unsupported_notif_types:
             with self.subTest(notif_type=notif_type):
                 notif = NotificationFactory(owner=self.owner, notif_type=notif_type)
                 self.assertFalse(notif.add_or_remove_timer())
 
     def test_should_not_process_timers_when_disabled(self, mock_add_or_remove_timer):
         # given
```

### Comparing `aa_structures-2.4.2/structures/tests/models/test_notifications_discord.py` & `aa_structures-2.5.0/structures/tests/models/test_notifications_discord.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
     from requests.exceptions import HTTPError
 
     from django.contrib.auth.models import Group
 
     from app_utils.testing import NoSocketsTestCase
 
-    from ...models import Notification
-    from ..testdata.factories import create_webhook
-    from ..testdata.helpers import (
+    from structures.models import Notification
+    from structures.tests.testdata.factories import create_webhook
+    from structures.tests.testdata.helpers import (
         create_structures,
         load_entities,
         load_notification_entities,
         set_owner_character,
     )
-    from ..testdata.load_eveuniverse import load_eveuniverse
+    from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
     MODULE_PATH = "structures.models.notifications"
 
     @patch(MODULE_PATH + ".Notification._import_discord")
     @patch(MODULE_PATH + ".Webhook.send_message", spec=True)
     class TestGroupPings(NoSocketsTestCase):
         @classmethod
@@ -75,14 +75,15 @@
             # then
             self.assertTrue(result)
             self.assertTrue(mock_import_discord.called)
             _, kwargs = mock_send_message.call_args
             self.assertIn(f"<@&{self.group_2.pk}>", kwargs["content"])
 
         def test_can_ping_both(self, mock_send_message, mock_import_discord):
+            # given
             mock_send_message.return_value = 1
             mock_import_discord.return_value.objects.group_to_role.side_effect = (
                 self._my_group_to_role
             )
             webhook = create_webhook()
             webhook.ping_groups.add(self.group_1)
             self.owner.ping_groups.add(self.group_2)
```

### Comparing `aa_structures-2.4.2/structures/tests/models/test_owners_1.py` & `aa_structures-2.5.0/structures/tests/models/test_owners_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 from esi.errors import TokenError
 from esi.models import Token
 from eveuniverse.models import EveSolarSystem
 
 from allianceauth.eveonline.models import EveCharacter, EveCorporationInfo
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
-from ...models import Owner, OwnerCharacter
-from ..testdata.factories import create_owner_from_user
-from ..testdata.helpers import create_structures, load_entities, set_owner_character
-from ..testdata.load_eveuniverse import load_eveuniverse
+from structures.models import Owner, OwnerCharacter
+from structures.tests.testdata.factories import create_owner_from_user
+from structures.tests.testdata.helpers import (
+    create_structures,
+    load_entities,
+    set_owner_character,
+)
+from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
 MODULE_PATH = "structures.models.owners"
 
 
 class TestOwner(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
```

### Comparing `aa_structures-2.4.2/structures/tests/models/test_owners_2.py` & `aa_structures-2.5.0/structures/tests/models/test_owners_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 
 from django.utils.timezone import now, utc
 from eveuniverse.models import EvePlanet
 
 from app_utils.esi_testing import EsiClientStub, EsiEndpoint
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
-from ...models import (
+from structures.core.notification_types import NotificationType
+from structures.models import (
     FuelAlertConfig,
-    NotificationType,
     Owner,
     PocoDetails,
     StarbaseDetail,
     Structure,
     StructureService,
     StructureTag,
     Webhook,
 )
-from .. import to_json
-from ..testdata.factories import (
+from structures.tests import to_json
+from structures.tests.testdata.factories import (
     create_owner_from_user,
     create_poco,
     create_starbase,
     create_structure_service,
     create_upwell_structure,
 )
-from ..testdata.helpers import load_entities
-from ..testdata.load_eveuniverse import load_eveuniverse
+from structures.tests.testdata.helpers import load_entities
+from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
 MODULE_PATH = "structures.models.owners"
 
 
 @patch(MODULE_PATH + ".esi")
 class TestUpdateStructuresEsi(NoSocketsTestCase):
     @classmethod
@@ -1174,15 +1174,15 @@
         structure = Structure.objects.get(id=1200000000003)
         self.assertEqual(structure.eve_planet_id, 40161472)
         self.assertEqual(structure.name, "Planet (Barren)")
 
     @patch(MODULE_PATH + ".STRUCTURES_FEATURE_STARBASES", False)
     @patch(MODULE_PATH + ".STRUCTURES_FEATURE_CUSTOMS_OFFICES", False)
     @patch(
-        "structures.models.structures.STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS", True
+        "structures.models.structures_1.STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS", True
     )
     @patch("structures.models.notifications.Webhook.send_message")
     def test_should_send_refueled_notification_when_fuel_level_increased(
         self, mock_send_message, mock_esi
     ):
         # given
         mock_esi.client = self.esi_client_stub
@@ -1196,24 +1196,24 @@
         owner = create_owner_from_user(self.user)
         owner.webhooks.add(webhook)
         owner.update_structures_esi()
         structure = Structure.objects.get(id=1000000000001)
         structure.fuel_expires_at = dt.datetime(2020, 3, 3, 0, 0, tzinfo=utc)
         structure.save()
         # when
-        with patch("structures.models.structures.now") as now:
+        with patch("structures.models.structures_1.now") as now:
             now.return_value = dt.datetime(2020, 3, 2, 0, 0, tzinfo=utc)
             owner.update_structures_esi()
         # then
         self.assertTrue(mock_send_message.called)
 
     @patch(MODULE_PATH + ".STRUCTURES_FEATURE_STARBASES", False)
     @patch(MODULE_PATH + ".STRUCTURES_FEATURE_CUSTOMS_OFFICES", False)
     @patch(
-        "structures.models.structures.STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS", True
+        "structures.models.structures_1.STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS", True
     )
     @patch("structures.models.notifications.Webhook.send_message")
     def test_should_not_send_refueled_notification_when_fuel_level_unchanged(
         self, mock_send_message, mock_esi
     ):
         # given
         mock_esi.client = self.esi_client_stub
@@ -1222,15 +1222,15 @@
             name="Webhook 1",
             url="webhook-1",
             notification_types=[NotificationType.STRUCTURE_REFUELED_EXTRA],
             is_active=True,
         )
         owner = create_owner_from_user(self.user)
         owner.webhooks.add(webhook)
-        with patch("structures.models.structures.now") as now:
+        with patch("structures.models.structures_1.now") as now:
             now.return_value = dt.datetime(2020, 3, 2, 0, 0, tzinfo=utc)
             owner.update_structures_esi()
             # when
             owner.update_structures_esi()
         # then
         self.assertFalse(mock_send_message.called)
 
@@ -1254,15 +1254,15 @@
         owner.update_structures_esi()
         structure = Structure.objects.get(id=1000000000001)
         structure.fuel_expires_at = dt.datetime(2020, 3, 3, 0, 0, tzinfo=utc)
         structure.save()
         config = FuelAlertConfig.objects.create(start=48, end=0, repeat=12)
         structure.structure_fuel_alerts.create(config=config, hours=12)
         # when
-        with patch("structures.models.structures.now") as now:
+        with patch("structures.models.structures_1.now") as now:
             now.return_value = dt.datetime(2020, 3, 2, 0, 0, tzinfo=utc)
             owner.update_structures_esi()
         # then
         self.assertEqual(structure.structure_fuel_alerts.count(), 0)
 
     @patch(MODULE_PATH + ".STRUCTURES_FEATURE_STARBASES", True)
     @patch(MODULE_PATH + ".STRUCTURES_FEATURE_CUSTOMS_OFFICES", False)
```

### Comparing `aa_structures-2.4.2/structures/tests/models/test_owners_3.py` & `aa_structures-2.5.0/structures/tests/models/test_owners_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,41 +14,41 @@
 from app_utils.testing import (
     BravadoResponseStub,
     NoSocketsTestCase,
     create_user_from_evecharacter,
     queryset_pks,
 )
 
-from ...models import (
+from structures.core.notification_types import NotificationType
+from structures.models import (
     JumpFuelAlertConfig,
     Notification,
-    NotificationType,
     Owner,
     StructureItem,
     Webhook,
 )
-from ..testdata.factories import (
+from structures.tests.testdata.factories import (
     create_owner_from_user,
     create_starbase,
     create_structure_item,
     create_upwell_structure,
     create_webhook,
 )
-from ..testdata.factories_2 import (
+from structures.tests.testdata.factories_2 import (
     EveEntityCorporationFactory,
     OwnerFactory,
     datetime_to_esi,
 )
-from ..testdata.helpers import (
+from structures.tests.testdata.helpers import (
     create_structures,
     load_entities,
     load_notification_entities,
     set_owner_character,
 )
-from ..testdata.load_eveuniverse import load_eveuniverse
+from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
 OWNERS_PATH = "structures.models.owners"
 NOTIFICATIONS_PATH = "structures.models.notifications"
 
 
 @patch(OWNERS_PATH + ".esi")
 class TestFetchNotificationsEsi(NoSocketsTestCase):
```

### Comparing `aa_structures-2.4.2/structures/tests/models/test_structures.py` & `aa_structures-2.5.0/structures/tests/models/test_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,43 +7,46 @@
 from django.utils.timezone import now
 from eveuniverse.models import EveSolarSystem
 
 from allianceauth.eveonline.models import EveCharacter, EveCorporationInfo
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
 from structures.constants import EveTypeId
+from structures.core.notification_types import NotificationType
 from structures.models import (
     EveSovereigntyMap,
     FuelAlertConfig,
     JumpFuelAlertConfig,
-    NotificationType,
     PocoDetails,
     Structure,
     StructureItem,
     StructureService,
     StructureTag,
 )
-
-from ..testdata.factories import (
+from structures.tests.testdata.factories import (
     create_owner_from_user,
     create_starbase,
     create_upwell_structure,
 )
-from ..testdata.factories_2 import (
+from structures.tests.testdata.factories_2 import (
     JumpGateFactory,
     OwnerFactory,
     PocoFactory,
     StarbaseFactory,
     StructureFactory,
     StructureTagFactory,
 )
-from ..testdata.helpers import create_structures, load_entities, set_owner_character
-from ..testdata.load_eveuniverse import load_eveuniverse
+from structures.tests.testdata.helpers import (
+    create_structures,
+    load_entities,
+    set_owner_character,
+)
+from structures.tests.testdata.load_eveuniverse import load_eveuniverse
 
-STRUCTURES_PATH = "structures.models.structures"
+STRUCTURES_PATH = "structures.models.structures_1"
 NOTIFICATIONS_PATH = "structures.models.notifications"
 
 EVE_ID_HELIUM_FUEL_BLOCK = 4247
 EVE_ID_NITROGEN_FUEL_BLOCK = 4051
 
 
 class TestStructureTag(NoSocketsTestCase):
```

### Comparing `aa_structures-2.4.2/structures/tests/test_admin.py` & `aa_structures-2.5.0/structures/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/tests/test_integration.py` & `aa_structures-2.5.0/structures/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 from django.utils.timezone import now
 from eveuniverse.models import EveSolarSystem
 
 from app_utils.django import app_labels
 from app_utils.esi import EsiStatus
 from app_utils.esi_testing import EsiClientStub, EsiEndpoint
 
-from .. import tasks
-from ..models import NotificationType, Structure
+from structures import tasks
+from structures.core.notification_types import NotificationType
+from structures.models import Structure
+
 from .testdata.factories_2 import (
     EveEntityAllianceFactory,
     EveEntityCorporationFactory,
     NotificationFactory,
     OwnerFactory,
     RawNotificationFactory,
     StarbaseFactory,
```

### Comparing `aa_structures-2.4.2/structures/tests/test_managers_1.py` & `aa_structures-2.5.0/structures/tests/test_managers_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from django.utils.timezone import now
 from eveuniverse.models import EveSolarSystem
 
 from allianceauth.eveonline.models import EveCharacter, EveCorporationInfo
 from app_utils.esi_testing import EsiClientStub, EsiEndpoint
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
+from structures.core.notification_types import NotificationType
 from structures.models import (
     EveSovereigntyMap,
-    NotificationType,
     Owner,
     Structure,
     StructureService,
     StructureTag,
     Webhook,
 )
 
@@ -69,28 +69,28 @@
         cls.esi_client_stub = EsiClientStub.create_from_endpoints(endpoints)
 
     @patch(MODULE_PATH + ".esi")
     def test_should_create_sov_map_from_scratch(self, mock_esi):
         # given
         mock_esi.client = self.esi_client_stub
         # when
-        EveSovereigntyMap.objects.update_from_esi()
+        EveSovereigntyMap.objects.update_or_create_all_from_esi()
         # then
         solar_system_ids = EveSovereigntyMap.objects.values_list(
             "solar_system_id", flat=True
         )
         self.assertSetEqual(set(solar_system_ids), {30000726, 30000474, 30000728})
 
     @patch(MODULE_PATH + ".esi")
     def test_should_update_existing_map(self, mock_esi):
         # given
         mock_esi.client = self.esi_client_stub
         create_eve_sovereignty_map(solar_system_id=30000726, alliance_id=3001)
         # when
-        EveSovereigntyMap.objects.update_from_esi()
+        EveSovereigntyMap.objects.update_or_create_all_from_esi()
         # then
         solar_system_ids = EveSovereigntyMap.objects.values_list(
             "solar_system_id", flat=True
         )
         self.assertSetEqual(set(solar_system_ids), {30000726, 30000474, 30000728})
         structure = EveSovereigntyMap.objects.get(solar_system_id=30000726)
         self.assertEqual(structure.corporation_id, 2011)
```

### Comparing `aa_structures-2.4.2/structures/tests/test_managers_3.py` & `aa_structures-2.5.0/structures/tests/test_managers_3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from unittest.mock import patch
 
 from app_utils.testing import NoSocketsTestCase
 
-from ..models import GeneratedNotification, Notification, NotificationType
+from structures.core.notification_types import NotificationType
+from structures.models import GeneratedNotification, Notification
+
 from .testdata.factories_2 import (
     GeneratedNotificationFactory,
     NotificationFactory,
     OwnerFactory,
 )
 from .testdata.load_eveuniverse import load_eveuniverse
```

### Comparing `aa_structures-2.4.2/structures/tests/test_tasks.py` & `aa_structures-2.5.0/structures/tests/test_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 from app_utils.testdata_factories import UserFactory
 from app_utils.testing import (
     NoSocketsTestCase,
     create_user_from_evecharacter,
     generate_invalid_pk,
 )
 
-from .. import tasks
-from ..models import FuelAlertConfig, NotificationType, Owner, Webhook
+from structures import tasks
+from structures.core.notification_types import NotificationType
+from structures.models import FuelAlertConfig, Owner, Webhook
+
 from .testdata.factories import create_notification, create_owner_from_user
 from .testdata.factories_2 import (
     FuelAlertConfigFactory,
     JumpFuelAlertConfigFactory,
     OwnerFactory,
     WebhookFactory,
 )
@@ -239,15 +241,15 @@
 #         self.owner.webhooks.first().clear_queue()
 #         # when
 #         tasks.process_notifications_for_owner.delay(owner_pk=self.owner.pk)
 #         # then
 #         self.assertTrue(mock_fetch_notifications_esi.called)
 #         self.assertEqual(mock_send_messages_for_webhook.apply_async.call_count, 1)
 #         for notif in self.owner.notifications.filter(
-#             notif_type__in=[NotificationType.structure_related]
+#             notif_type__in=[NotificationType.structure_related()]
 #         ):
 #             structure_ids = notif.structures.values_list("id", flat=True)
 #             self.assertTrue(
 #                 1000000000001 in set(structure_ids)
 #                 or 1000000000002 in set(structure_ids)
 #             )
 
@@ -338,15 +340,18 @@
         # when
         result = tasks.update_existing_notifications(owner.pk)
         # then
         self.assertEqual(result, 0)
 
 
 class TestOtherTasks(NoSocketsTestCase):
-    @patch(MODULE_PATH + ".EveSovereigntyMap.objects.update_from_esi", spec=True)
+    @patch(
+        MODULE_PATH + ".EveSovereigntyMap.objects.update_or_create_all_from_esi",
+        spec=True,
+    )
     def test_should_call_update_sov_map_from_esi(self, mock_update_from_esi):
         # when
         tasks.update_sov_map()
         # then
         self.assertTrue(mock_update_from_esi.called)
 
     @patch(MODULE_PATH + ".Owner.fetch_notifications_esi", spec=True)
```

### Comparing `aa_structures-2.4.2/structures/tests/test_views.py` & `aa_structures-2.5.0/structures/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,18 @@
     EveAllianceInfo,
     EveCharacter,
     EveCorporationInfo,
 )
 from allianceauth.tests.auth_utils import AuthUtils
 from app_utils.testing import create_user_from_evecharacter, json_response_to_python
 
-from .. import views
-from ..constants import EveTypeId
-from ..models import Owner, PocoDetails, Structure, StructureItem, Webhook
+from structures import views
+from structures.constants import EveTypeId
+from structures.models import Owner, PocoDetails, Structure, StructureItem, Webhook
+
 from .testdata.factories import create_owner_from_user, create_poco, create_starbase
 from .testdata.helpers import (
     create_structures,
     load_entities,
     load_entity,
     set_owner_character,
 )
```

### Comparing `aa_structures-2.4.2/structures/tests/testdata/create_eveuniverse.py` & `aa_structures-2.5.0/structures/tests/testdata/create_eveuniverse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.test import TestCase
 from eveuniverse.models import EveType
 from eveuniverse.tools.testdata import ModelSpec, create_testdata
 
-from ...constants import EveCategoryId, EveGroupId, EveTypeId
+from structures.constants import EveCategoryId, EveGroupId, EveTypeId
+
 from .helpers import test_data_filename
 
 
 class CreateEveUniverseTestData(TestCase):
     def test_create_testdata(self):
         testdata_spec = [
             ModelSpec(
```

### Comparing `aa_structures-2.4.2/structures/tests/testdata/entities.json` & `aa_structures-2.5.0/structures/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/tests/testdata/esi_data.json` & `aa_structures-2.5.0/structures/tests/testdata/esi_data.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/tests/testdata/eveuniverse.json` & `aa_structures-2.5.0/structures/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/tests/testdata/factories.py` & `aa_structures-2.5.0/structures/tests/testdata/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 from django.contrib.auth.models import User
 from django.utils.text import slugify
 from django.utils.timezone import now
 
 from allianceauth.eveonline.models import EveCorporationInfo
 
-from ...constants import EveTypeId
-from ...models import (
+from structures.constants import EveTypeId
+from structures.models import (
     EveSovereigntyMap,
     Notification,
     Owner,
     OwnerCharacter,
     PocoDetails,
     StarbaseDetail,
     StarbaseDetailFuel,
```

### Comparing `aa_structures-2.4.2/structures/tests/testdata/factories_2.py` & `aa_structures-2.5.0/structures/tests/testdata/factories_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 from app_utils.testdata_factories import (
     EveAllianceInfoFactory,
     EveCharacterFactory,
     EveCorporationInfoFactory,
     UserMainFactory,
 )
 
-from ...models import (
+from structures.core.notification_types import NotificationType
+from structures.models import (
     FuelAlertConfig,
     GeneratedNotification,
     JumpFuelAlertConfig,
     Notification,
-    NotificationType,
     Owner,
     OwnerCharacter,
     Structure,
     StructureTag,
     Webhook,
 )
```

### Comparing `aa_structures-2.4.2/structures/tests/testdata/generate_notifications.py` & `aa_structures-2.5.0/structures/tests/testdata/generate_notifications.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/tests/testdata/generate_notifications_2.py` & `aa_structures-2.5.0/structures/tests/testdata/generate_notifications_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/tests/testdata/generate_structures.py` & `aa_structures-2.5.0/structures/tests/testdata/generate_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/tests/testdata/helpers.py` & `aa_structures-2.5.0/structures/tests/testdata/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,24 +23,25 @@
     EveAllianceInfo,
     EveCharacter,
     EveCorporationInfo,
 )
 from app_utils.esi_testing import BravadoOperationStub, BravadoResponseStub
 from app_utils.testing import create_user_from_evecharacter
 
-from ...models import (
+from structures.core.notification_types import NotificationType
+from structures.models import (
     EveSovereigntyMap,
     Notification,
-    NotificationType,
     Owner,
     Structure,
     StructureService,
     StructureTag,
     Webhook,
 )
+
 from .factories import create_notification
 
 ESI_CORP_STRUCTURES_PAGE_SIZE = 2
 
 _current_folder = Path(__file__).parent
 _FILENAME_EVEUNIVERSE_TESTDATA = "eveuniverse.json"
```

### Comparing `aa_structures-2.4.2/structures/tests/testdata/tasks_loadtest.py` & `aa_structures-2.5.0/structures/tests/testdata/tasks_loadtest.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.2/structures/urls.py` & `aa_structures-2.5.0/structures/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Tasks for Structures."""
+
 from django.urls import path
 
 from . import views
 
 app_name = "structures"
 
 urlpatterns = [
```

### Comparing `aa_structures-2.4.2/structures/views.py` & `aa_structures-2.5.0/structures/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Views for Structures."""
+
 import functools
 from collections import defaultdict
 from enum import IntEnum
 from typing import Dict
 from urllib.parse import urlencode
 
 from django.contrib.auth.decorators import login_required, permission_required
@@ -54,41 +56,44 @@
         return default
     return value
 
 
 @login_required
 @permission_required("structures.basic_access")
 def index(request):
+    """Redirect from index view to main."""
     url = reverse("structures:main")
     if STRUCTURES_DEFAULT_TAGS_FILTER_ENABLED:
         params = {
             QUERY_PARAM_TAGS: ",".join(
                 [x.name for x in StructureTag.objects.filter(is_default=True)]
             )
         }
-        url += "?{}".format(urlencode(params))
+        params_encoded = urlencode(params)
+        url += f"?{params_encoded}"
     return redirect(url)
 
 
 @login_required
 @permission_required("structures.basic_access")
 def main(request):
     """Main view"""
-    active_tags = list()
+    active_tags = []
     if request.method == "POST":
         form = TagsFilterForm(data=request.POST)
         if form.is_valid():
             for name, activated in form.cleaned_data.items():
                 if activated:
                     active_tags.append(get_object_or_404(StructureTag, name=name))
 
             url = reverse("structures:main")
             if active_tags:
                 params = {QUERY_PARAM_TAGS: ",".join([x.name for x in active_tags])}
-                url += "?{}".format(urlencode(params))
+                params_encoded = urlencode(params)
+                url += f"?{params_encoded}"
             return redirect(url)
     else:
         tags_raw = request.GET.get(QUERY_PARAM_TAGS)
         if tags_raw:
             tags_parsed = tags_raw.split(",")
             active_tags = [
                 x for x in StructureTag.objects.all() if x.name in tags_parsed
@@ -107,207 +112,236 @@
     }
     return render(request, "structures/main.html", context)
 
 
 @login_required
 @permission_required("structures.basic_access")
 def structure_list_data(request) -> JsonResponse:
-    """returns structure list in JSON for AJAX call in structure_list view"""
+    """Return structure list in JSON for AJAX call in structure_list view."""
     tags_raw = request.GET.get(QUERY_PARAM_TAGS)
     tags = tags_raw.split(",") if tags_raw else None
     structures = Structure.objects.visible_for_user(request.user, tags)
     serializer = StructureListSerializer(queryset=structures, request=request)
     return JsonResponse({"data": serializer.to_list()})
 
 
+class FakeEveType:
+    """A faked eve type."""
+
+    def __init__(self, id, name):
+        self.id = id
+        self.name = name
+        self.profile_url = ""
+
+    def icon_url(self, size=64) -> str:
+        """Return icon url for an EveType."""
+        return eveimageserver.type_icon_url(self.id, size)
+
+
+class FakeAsset:
+    """Fake asset object for showing additional information in the asset list."""
+
+    def __init__(self, name, quantity, eve_type_id):
+        self.name = name
+        self.quantity = quantity
+        self.eve_type_id = eve_type_id
+        self.eve_type = FakeEveType(eve_type_id, name)
+        self.is_singleton = False
+
+
+class Slot(IntEnum):
+    """A slot type in a fitting."""
+
+    HIGH = 14
+    MEDIUM = 13
+    LOW = 12
+    RIG = 1137
+    SERVICE = 2056
+
+    def image_url(self, type_attributes: dict) -> str:
+        """Return url to image file for this slot variant"""
+        id_map = {
+            self.HIGH: "h",
+            self.MEDIUM: "m",
+            self.LOW: "l",
+            self.RIG: "r",
+            self.SERVICE: "s",
+        }
+        try:
+            slot_num = type_attributes[self.value]
+            my_id = id_map[Slot(self.value)]
+            return staticfiles_storage.url(
+                f"structures/img/panel/{slot_num}{my_id}.png"
+            )
+        except KeyError:
+            return ""
+
+
 @login_required
 @permission_required("structures.view_structure_fit")
 def structure_details(request, structure_id):
     """Main view of the structure fit"""
 
-    class Slot(IntEnum):
-        HIGH = 14
-        MEDIUM = 13
-        LOW = 12
-        RIG = 1137
-        SERVICE = 2056
-
-        def image_url(self) -> str:
-            """Return url to image file for this slot variant"""
-            id_map = {
-                self.HIGH: "h",
-                self.MEDIUM: "m",
-                self.LOW: "l",
-                self.RIG: "r",
-                self.SERVICE: "s",
-            }
-            try:
-                slot_num = type_attributes[self.value]
-                my_id = id_map[Slot(self.value)]
-                return staticfiles_storage.url(
-                    f"structures/img/panel/{slot_num}{my_id}.png"
-                )
-            except KeyError:
-                return ""
-
-    class FakeEveType:
-        def __init__(self, id, name):
-            self.id = id
-            self.name = name
-            self.profile_url = ""
-
-        def icon_url(self, size=64) -> str:
-            return eveimageserver.type_icon_url(self.id, size)
-
-    class FakeAsset:
-        """Fake asset object for showing additional information in the asset list."""
-
-        def __init__(self, name, quantity, eve_type_id):
-            self.name = name
-            self.quantity = quantity
-            self.eve_type_id = eve_type_id
-            self.eve_type = FakeEveType(eve_type_id, name)
-            self.is_singleton = False
-
-    def extract_slot_assets(fittings: list, slot_name: str) -> list:
-        """Return assets for slot sorted by slot number"""
-        return [
-            asset[0]
-            for asset in sorted(
-                [
-                    (asset, asset.location_flag[-1])
-                    for asset in fittings
-                    if asset.location_flag.startswith(slot_name)
-                ],
-                key=lambda x: x[1],
-            )
-        ]
-
-    def patch_fighter_tube_quantities(fighter_tubes):
-        eve_type_ids = {item.eve_type_id for item in fighter_tubes}
-        eve_types = [
-            EveType.objects.get_or_create_esi(
-                id=eve_type_id, enabled_sections=[EveType.Section.DOGMAS]
-            )[0]
-            for eve_type_id in eve_type_ids
-        ]
-        squadron_sizes = {
-            eve_type.id: int(
-                eve_type.dogma_attributes.get(
-                    eve_dogma_attribute=EveAttributeId.SQUADRON_SIZE.value
-                ).value
-            )
-            for eve_type in eve_types
-        }
-        for item in fighter_tubes:
-            try:
-                squadron_size = squadron_sizes[item.eve_type_id]
-            except KeyError:
-                pass
-            else:
-                item.quantity = squadron_size
-                item.is_singleton = False
-
     structure = get_object_or_404(
         Structure.objects.select_related(
             "owner",
             "owner__corporation",
             "owner__corporation__alliance",
             "eve_type",
             "eve_type__eve_group",
             "eve_solar_system",
             "eve_solar_system__eve_constellation",
             "eve_solar_system__eve_constellation__eve_region",
         ),
         id=structure_id,
     )
-    type_attributes = {
-        obj["eve_dogma_attribute_id"]: int(obj["value"])
-        for obj in EveTypeDogmaAttribute.objects.filter(
-            eve_type_id=structure.eve_type_id
-        ).values("eve_dogma_attribute_id", "value")
-    }
-    slot_image_urls = {
-        "high": Slot.HIGH.image_url(),
-        "med": Slot.MEDIUM.image_url(),
-        "low": Slot.LOW.image_url(),
-        "rig": Slot.RIG.image_url(),
-        "service": Slot.SERVICE.image_url(),
-    }
     assets = structure.items.select_related("eve_type")
-    high_slots = extract_slot_assets(assets, "HiSlot")
-    med_slots = extract_slot_assets(assets, "MedSlot")
-    low_slots = extract_slot_assets(assets, "LoSlot")
-    rig_slots = extract_slot_assets(assets, "RigSlot")
-    service_slots = extract_slot_assets(assets, "ServiceSlot")
-    fighter_tubes = extract_slot_assets(assets, "FighterTube")
-    patch_fighter_tube_quantities(fighter_tubes)
-    assets_grouped = {"ammo_hold": [], "fighter_bay": [], "fuel_bay": []}
-    for asset in assets:
-        if asset.location_flag == StructureItem.LocationFlag.CARGO:
-            assets_grouped["ammo_hold"].append(asset)
-        elif asset.location_flag == StructureItem.LocationFlag.FIGHTER_BAY:
-            assets_grouped["fighter_bay"].append(asset)
-        elif asset.location_flag == StructureItem.LocationFlag.STRUCTURE_FUEL:
-            assets_grouped["fuel_bay"].append(asset)
-        else:
-            assets_grouped[asset.location_flag] = asset
+    high_slots = _extract_slot_assets(assets, "HiSlot")
+    med_slots = _extract_slot_assets(assets, "MedSlot")
+    low_slots = _extract_slot_assets(assets, "LoSlot")
+    rig_slots = _extract_slot_assets(assets, "RigSlot")
+    service_slots = _extract_slot_assets(assets, "ServiceSlot")
+    fighter_tubes = _extract_slot_assets(assets, "FighterTube")
+    _patch_fighter_tube_quantities(fighter_tubes)
+
+    assets_grouped = _init_assets_grouped(assets)
+
     if structure.is_upwell_structure:
         assets_grouped["fuel_usage"] = [
             FakeAsset(
                 name=_("Fuel blocks per day (est.)"),
                 quantity=structure.structure_fuel_usage(),
                 eve_type_id=24756,
             )
         ]
-    modules_count = len(high_slots + med_slots + low_slots + rig_slots + service_slots)
+
     fuel_blocks_total = (
         functools.reduce(
             lambda x, y: x + y, [obj.quantity for obj in assets_grouped["fuel_bay"]]
         )
         if assets_grouped["fuel_bay"]
         else 0
     )
     ammo_total = (
         functools.reduce(
             lambda x, y: x + y, [obj.quantity for obj in assets_grouped["ammo_hold"]]
         )
         if assets_grouped["ammo_hold"]
         else 0
     )
-    fighters_consolidated = assets_grouped["fighter_bay"] + fighter_tubes
-    fighters_total = (
-        functools.reduce(
-            lambda x, y: x + y, [obj.quantity for obj in fighters_consolidated]
-        )
-        if fighters_consolidated
-        else 0
-    )
     context = {
         "fitting": assets,
-        "slots": slot_image_urls,
+        "slots": _generate_slot_image_urls(structure),
         "slot_assets": {
             "high_slots": high_slots,
             "med_slots": med_slots,
             "low_slots": low_slots,
             "rig_slots": rig_slots,
             "service_slots": service_slots,
             "fighter_tubes": fighter_tubes,
         },
         "assets_grouped": assets_grouped,
         "structure": structure,
-        "modules_count": modules_count,
+        "modules_count": len(
+            high_slots + med_slots + low_slots + rig_slots + service_slots
+        ),
         "fuel_blocks_total": fuel_blocks_total,
-        "fighters_total": fighters_total,
+        "fighters_total": _calc_fighters_total(fighter_tubes, assets_grouped),
         "ammo_total": ammo_total,
         "last_updated": structure.owner.assets_last_update_at,
     }
     return render(request, "structures/modals/structure_details.html", context)
 
 
+def _init_assets_grouped(assets):
+    assets_grouped = {"ammo_hold": [], "fighter_bay": [], "fuel_bay": []}
+    for asset in assets:
+        if asset.location_flag == StructureItem.LocationFlag.CARGO:
+            assets_grouped["ammo_hold"].append(asset)
+        elif asset.location_flag == StructureItem.LocationFlag.FIGHTER_BAY:
+            assets_grouped["fighter_bay"].append(asset)
+        elif asset.location_flag == StructureItem.LocationFlag.STRUCTURE_FUEL:
+            assets_grouped["fuel_bay"].append(asset)
+        else:
+            assets_grouped[asset.location_flag] = asset
+    return assets_grouped
+
+
+def _calc_fighters_total(fighter_tubes, assets_grouped):
+    fighters_consolidated = assets_grouped["fighter_bay"] + fighter_tubes
+    fighters_total = (
+        functools.reduce(
+            lambda x, y: x + y, [obj.quantity for obj in fighters_consolidated]
+        )
+        if fighters_consolidated
+        else 0
+    )
+
+    return fighters_total
+
+
+def _generate_slot_image_urls(structure):
+    type_attributes = {
+        obj["eve_dogma_attribute_id"]: int(obj["value"])
+        for obj in EveTypeDogmaAttribute.objects.filter(
+            eve_type_id=structure.eve_type_id
+        ).values("eve_dogma_attribute_id", "value")
+    }
+    slot_image_urls = {
+        "high": Slot.HIGH.image_url(type_attributes),
+        "med": Slot.MEDIUM.image_url(type_attributes),
+        "low": Slot.LOW.image_url(type_attributes),
+        "rig": Slot.RIG.image_url(type_attributes),
+        "service": Slot.SERVICE.image_url(type_attributes),
+    }
+
+    return slot_image_urls
+
+
+def _extract_slot_assets(fittings: list, slot_name: str) -> list:
+    """Return assets for slot sorted by slot number"""
+    return [
+        asset[0]
+        for asset in sorted(
+            [
+                (asset, asset.location_flag[-1])
+                for asset in fittings
+                if asset.location_flag.startswith(slot_name)
+            ],
+            key=lambda x: x[1],
+        )
+    ]
+
+
+def _patch_fighter_tube_quantities(fighter_tubes):
+    eve_type_ids = {item.eve_type_id for item in fighter_tubes}
+    eve_types = [
+        EveType.objects.get_or_create_esi(
+            id=eve_type_id, enabled_sections=[EveType.Section.DOGMAS]
+        )[0]
+        for eve_type_id in eve_type_ids
+    ]
+    squadron_sizes = {
+        eve_type.id: int(
+            eve_type.dogma_attributes.get(
+                eve_dogma_attribute=EveAttributeId.SQUADRON_SIZE.value
+            ).value
+        )
+        for eve_type in eve_types
+    }
+    for item in fighter_tubes:
+        try:
+            squadron_size = squadron_sizes[item.eve_type_id]
+        except KeyError:
+            pass
+        else:
+            item.quantity = squadron_size
+            item.is_singleton = False
+
+
 @login_required
 @permission_required("structures.basic_access")
 def poco_details(request, structure_id):
     """Shows details modal for a POCO."""
 
     structure = get_object_or_404(
         Structure.objects.select_related(
@@ -390,14 +424,15 @@
     return render(request, "structures/modals/starbase_detail.html", context)
 
 
 @login_required
 @permission_required("structures.add_structure_owner")
 @token_required(scopes=Owner.get_esi_scopes())  # type: ignore
 def add_structure_owner(request, token):
+    """View for adding or replacing a structure owner."""
     token_char = get_object_or_404(EveCharacter, character_id=token.character_id)
     try:
         character_ownership = CharacterOwnership.objects.get(
             user=request.user, character=token_char
         )
     except CharacterOwnership.DoesNotExist:
         character_ownership = None
@@ -504,16 +539,15 @@
     """
     status_ok = True
     for owner in Owner.objects.filter(is_included_in_service_status=True):
         status_ok = status_ok and owner.are_all_syncs_ok
 
     if status_ok:
         return HttpResponse(_("service is up"))
-    else:
-        return HttpResponseServerError(_("service is down"))
+    return HttpResponseServerError(_("service is down"))
 
 
 def poco_list_data(request) -> JsonResponse:
     """List of public POCOs for DataTables."""
     pocos = Structure.objects.filter(
         eve_type__eve_group__eve_category_id=EveCategoryId.ORBITAL,
         owner__are_pocos_public=True,
@@ -521,14 +555,15 @@
     serializer = PocoListSerializer(queryset=pocos, request=request)
     return JsonResponse({"data": serializer.to_list()})
 
 
 @login_required
 @permission_required("structures.basic_access")
 def structure_summary_data(request) -> JsonResponse:
+    """View returning data for structure summary page."""
     summary_qs = (
         Structure.objects.values(
             "owner__corporation__corporation_id",
             "owner__corporation__corporation_name",
             "owner__corporation__alliance__alliance_name",
         )
         .annotate(
@@ -553,15 +588,15 @@
         .annotate(poco_count=Count("id", filter=Q(eve_type=EveTypeId.CUSTOMS_OFFICE)))
         .annotate(
             starbase_count=Count(
                 "id", filter=Q(eve_type__eve_group__eve_category=EveCategoryId.STARBASE)
             )
         )
     )
-    data = list()
+    data = []
     for row in summary_qs:
         other_count = (
             row["upwell_count"]
             - row["ec_count"]
             - row["refinery_count"]
             - row["citadel_count"]
         )
```

### Comparing `aa_structures-2.4.2/structures/webhooks/core.py` & `aa_structures-2.5.0/structures/webhooks/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Core logic for webhooks."""
+
 import json
 from time import sleep
 from typing import List, Optional, Tuple
 from urllib.parse import urlparse
 
 import dhooks_lite
 from simple_mq import SimpleMQ
@@ -9,15 +11,15 @@
 from django.contrib.auth.models import User
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.allianceauth import get_redis_client
 from app_utils.json import JSONDateTimeDecoder, JSONDateTimeEncoder
 from app_utils.logging import LoggerAddTag
 
-from .. import __title__
+from structures import __title__
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class DiscordWebhookMixin:
     """Mixing adding a queued Discord webhook to a model
 
@@ -38,34 +40,32 @@
             redis_client, f"{__title__}_webhook_{self.pk}_errors"
         )
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
-        return "{}(pk={}, name='{}')".format(
-            self.__class__.__name__, self.pk, self.name
-        )
+        return f"{self.__class__.__name__}(pk={self.pk}, name='{self.name}')"
 
     def queue_size(self) -> int:
         """returns current size of the queue"""
         return self._main_queue.size()
 
     def clear_queue(self) -> int:
         """deletes all messages from the queue. Returns number of cleared messages."""
         counter = 0
         while True:
-            y = self._main_queue.dequeue()
-            if y is None:
+            message = self._main_queue.dequeue()
+            if message is None:
                 break
-            else:
-                counter += 1
+            counter += 1
 
         return counter
 
+    # pylint: disable = too-many-arguments
     def send_message(
         self,
         content: Optional[str] = None,
         embeds: Optional[List[dhooks_lite.Embed]] = None,
         tts: Optional[bool] = None,
         username: Optional[str] = None,
         avatar_url: Optional[str] = None,
@@ -79,15 +79,15 @@
             raise ValueError("Message must have content or embeds to be valid")
 
         if embeds:
             embeds_list = [obj.asdict() for obj in embeds]
         else:
             embeds_list = None
 
-        message = dict()
+        message = {}
         if content:
             message["content"] = content
         if embeds_list:
             message["embeds"] = embeds_list
         if tts:
             message["tts"] = tts
         if username:
@@ -100,16 +100,15 @@
     @staticmethod
     def _url_has_scheme(avatar_url) -> bool:
         """Return True if URL is valid and has a scheme else return False."""
         try:
             parts = urlparse(avatar_url)
         except ValueError:
             return False
-        else:
-            return bool(parts.scheme)
+        return bool(parts.scheme)
 
     def send_queued_messages(self) -> int:
         """sends all messages in the queue to this webhook
 
         returns number of successfully sent messages
 
         Messages that could not be sent are put back into the queue for later retry
@@ -161,20 +160,21 @@
             wait_for_response=True,
         )
         logger.debug("headers: %s", response.headers)
         logger.debug("status_code: %s", response.status_code)
         logger.debug("content: %s", response.content)
         if response.status_ok:
             return True
+
         msg = (
-            f"Webhook {self} failed to send message to Discord.\n"
-            f"HTTP status code: {response.status_code}\n"
+            f"Webhook {self} failed to send message to Discord. "
+            f"HTTP status code: {response.status_code}. "
             f"API response: {response.content}"
         )
-        logger.warning(msg, exc_info=True)
+        logger.warning(msg)
         return False
 
     @classmethod
     def create_link(cls, name: str, url: str) -> str:
         """creates a link for messages of this webhook"""
         return f"[{str(name)}]({str(url)})"
 
@@ -183,22 +183,23 @@
         user_text = f" sent by **{user}**" if user else ""
         message = {
             "content": f"Test message for webhook **{self.name}**{user_text}",
             "username": __title__,
         }
         try:
             success = self._send_message_to_webhook(message)
+
         except OSError as ex:
             logger.warning(
                 "Failed to send test notification to webhook %s: %s",
                 self,
                 ex,
                 exc_info=True,
             )
             return type(ex).__name__, False
-        else:
-            return "(no info)", success
+
+        return "(no info)", success
 
     @staticmethod
     def default_username() -> str:
         """sets the apps title as username for all messages"""
         return __title__
```

### Comparing `aa_structures-2.4.2/structures/webhooks/managers.py` & `aa_structures-2.5.0/structures/webhooks/managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+"""Managers for webhooks."""
+
+# pylint: disable=missing-class-docstring
+
 from django.db import models
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
-from .. import __title__
+from structures import __title__
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class WebhookBaseManager(models.Manager):
     def send_queued_messages_for_webhook(self, webhook_pk: int) -> None:
         """sends all currently queued messages to given webhook
```

### Comparing `aa_structures-2.4.2/structures/webhooks/models.py` & `aa_structures-2.5.0/structures/webhooks/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,37 @@
+"""Models for webhooks."""
+
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from .core import DiscordWebhookMixin
 from .managers import WebhookBaseManager
 
 
 class WebhookBase(DiscordWebhookMixin, models.Model):
     """Base model for a Webhook"""
 
     class PingType(models.TextChoices):
+        """A ping type for webhooks."""
+
         NONE = "NO", _("none")
         HERE = "HE", _("here")
         EVERYONE = "EV", _("everyone")
 
     class Color(models.IntegerChoices):
+        """A color for embeds."""
+
         DANGER = 0xD9534F, _("danger")
         INFO = 0x5BC0DE, _("info")
         SUCCESS = 0x5CB85C, _("success")
         WARNING = 0xF0AD4E, _("warning")
 
         @property
         def css_color(self) -> str:
+            """Return color as CSS value."""
             return f"#{self.value:X}"
 
     TYPE_DISCORD = 1
 
     TYPE_CHOICES = [
         (TYPE_DISCORD, _("Discord Webhook")),
     ]
```

### Comparing `aa_structures-2.4.2/structures/webhooks/tests/test_core.py` & `aa_structures-2.5.0/structures/webhooks/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import dhooks_lite
 
 from django.test import TestCase
 
 from allianceauth.tests.auth_utils import AuthUtils
 from app_utils.json import JSONDateTimeDecoder
 
-from .. import core
+from structures.webhooks import core
 
 MODULE_PATH = core.__package__ + ".core"
 
 
 class Webhook(core.DiscordWebhookMixin):
     """Fake Webhook model used for testing
```

### Comparing `aa_structures-2.4.2/PKG-INFO` & `aa_structures-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-structures
-Version: 2.4.2
+Version: 2.5.0
 Summary: App for managing Eve Online structures with Alliance Auth.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
@@ -22,14 +22,15 @@
 Requires-Dist: allianceauth>=3.0
 Requires-Dist: dhooks-lite>=1.0
 Requires-Dist: django-eveuniverse>=1.0
 Requires-Dist: django-multiselectfield
 Requires-Dist: django-navhelper
 Requires-Dist: pytz!=2022.2
 Requires-Dist: redis-simple-mq>=1.0
+Requires-Dist: humanize>=4.7
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-structures/-/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://aa-structures.readthedocs.io/en/latest/
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-structures
 Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-structures
 Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-structures/-/issues
 
 # Structures
```

