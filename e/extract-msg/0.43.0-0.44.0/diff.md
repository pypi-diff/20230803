# Comparing `tmp/extract_msg-0.43.0.tar.gz` & `tmp/extract_msg-0.44.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extract_msg-0.43.0.tar", last modified: Thu Aug  3 03:36:00 2023, max compression
+gzip compressed data, was "extract_msg-0.44.0.tar", last modified: Thu Aug  3 21:39:54 2023, max compression
```

## Comparing `extract_msg-0.43.0.tar` & `extract_msg-0.44.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.203290 extract_msg-0.43.0/
--rw-rw-rw-   0        0        0    84772 2023-08-03 03:35:57.000000 extract_msg-0.43.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.43.0/LICENSE.txt
--rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.43.0/MANIFEST.in
--rw-rw-rw-   0        0        0    12250 2023-08-03 03:36:00.204274 extract_msg-0.43.0/PKG-INFO
--rw-rw-rw-   0        0        0    11428 2023-08-03 03:35:57.000000 extract_msg-0.43.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.090577 extract_msg-0.43.0/extract_msg/
--rw-rw-rw-   0        0        0     1937 2023-08-03 03:35:57.000000 extract_msg-0.43.0/extract_msg/__init__.py
--rw-rw-rw-   0        0        0     3629 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/__main__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.118505 extract_msg-0.43.0/extract_msg/_rtf/
--rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.43.0/extract_msg/_rtf/__init__.py
--rw-rw-rw-   0        0        0      845 2023-05-09 19:54:43.000000 extract_msg-0.43.0/extract_msg/_rtf/create_doc.py
--rw-rw-rw-   0        0        0     6250 2023-05-09 19:54:43.000000 extract_msg-0.43.0/extract_msg/_rtf/inject_rtf.py
--rw-rw-rw-   0        0        0      856 2023-05-09 19:54:43.000000 extract_msg-0.43.0/extract_msg/_rtf/token.py
--rw-rw-rw-   0        0        0     8932 2023-05-09 19:54:43.000000 extract_msg-0.43.0/extract_msg/_rtf/tokenize_rtf.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.130471 extract_msg-0.43.0/extract_msg/attachments/
--rw-rw-rw-   0        0        0     5756 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/attachments/__init__.py
--rw-rw-rw-   0        0        0     7338 2023-07-31 13:37:55.000000 extract_msg-0.43.0/extract_msg/attachments/attachment.py
--rw-rw-rw-   0        0        0    23038 2023-08-03 03:03:26.000000 extract_msg-0.43.0/extract_msg/attachments/attachment_base.py
--rw-rw-rw-   0        0        0     1188 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/attachments/broken_att.py
--rw-rw-rw-   0        0        0     6051 2023-07-31 13:37:55.000000 extract_msg-0.43.0/extract_msg/attachments/custom_att.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.135459 extract_msg-0.43.0/extract_msg/attachments/custom_att_handler/
--rw-rw-rw-   0        0        0     2591 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/attachments/custom_att_handler/__init__.py
--rw-rw-rw-   0        0        0     1766 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/attachments/custom_att_handler/custom_handler.py
--rw-rw-rw-   0        0        0     4754 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/attachments/custom_att_handler/outlook_image_dib.py
--rw-rw-rw-   0        0        0     5004 2023-07-31 13:37:55.000000 extract_msg-0.43.0/extract_msg/attachments/emb_msg_att.py
--rw-rw-rw-   0        0        0     9052 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/attachments/signed_att.py
--rw-rw-rw-   0        0        0     1162 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/attachments/unsupported_att.py
--rw-rw-rw-   0        0        0     2442 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/attachments/web_att.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.140444 extract_msg-0.43.0/extract_msg/constants/
--rw-rw-rw-   0        0        0     5670 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/constants/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/constants/ps.py
--rw-rw-rw-   0        0        0      874 2023-07-31 13:37:55.000000 extract_msg-0.43.0/extract_msg/constants/re.py
--rw-rw-rw-   0        0        0     3237 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/constants/st.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.055672 extract_msg-0.43.0/extract_msg/data/
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.142439 extract_msg-0.43.0/extract_msg/data/logging-config/
--rw-rw-rw-   0        0        0     2082 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/data/logging-config/logging-nt.json
--rw-rw-rw-   0        0        0     2058 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/data/logging-config/logging-posix.json
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.144433 extract_msg-0.43.0/extract_msg/encoding/
--rw-rw-rw-   0        0        0    12602 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/encoding/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.154417 extract_msg-0.43.0/extract_msg/encoding/_dt/
--rw-rw-rw-   0        0        0      116 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/encoding/_dt/__init__.py
--rw-rw-rw-   0        0        0     2743 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/encoding/_dt/_mac_ce.py
--rw-rw-rw-   0        0        0     2785 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/encoding/_dt/_mac_cyrillic.py
--rw-rw-rw-   0        0        0     2721 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/encoding/_dt/_mac_greek.py
--rw-rw-rw-   0        0        0     2627 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/encoding/_dt/_mac_iceland.py
--rw-rw-rw-   0        0        0     2628 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/encoding/_dt/_mac_turkish.py
--rw-rw-rw-   0        0        0     2422 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/encoding/_dt/_win874_dec.py
--rw-rw-rw-   0        0        0   298022 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/encoding/_dt/_win950_dec.py
--rw-rw-rw-   0        0        0    12122 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/encoding/utils.py
--rw-rw-rw-   0        0        0    58987 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/enums.py
--rw-rw-rw-   0        0        0     4048 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.181335 extract_msg-0.43.0/extract_msg/msg_classes/
--rw-rw-rw-   0        0        0     1249 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/__init__.py
--rw-rw-rw-   0        0        0     6722 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/appointment.py
--rw-rw-rw-   0        0        0     2930 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/calendar.py
--rw-rw-rw-   0        0        0    19319 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/calendar_base.py
--rw-rw-rw-   0        0        0    46043 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/contact.py
--rw-rw-rw-   0        0        0     3590 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/meeting_cancellation.py
--rw-rw-rw-   0        0        0     1630 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/meeting_exception.py
--rw-rw-rw-   0        0        0     3737 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/meeting_forward.py
--rw-rw-rw-   0        0        0     1900 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/meeting_related.py
--rw-rw-rw-   0        0        0     6577 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/meeting_request.py
--rw-rw-rw-   0        0        0     2223 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/meeting_response.py
--rw-rw-rw-   0        0        0      163 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/message.py
--rw-rw-rw-   0        0        0    58319 2023-08-03 03:35:57.000000 extract_msg-0.43.0/extract_msg/msg_classes/message_base.py
--rw-rw-rw-   0        0        0      201 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/message_signed.py
--rw-rw-rw-   0        0        0     5016 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/message_signed_base.py
--rw-rw-rw-   0        0        0    37987 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/msg.py
--rw-rw-rw-   0        0        0     2610 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/post.py
--rw-rw-rw-   0        0        0     1675 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/sticky_note.py
--rw-rw-rw-   0        0        0    12686 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/task.py
--rw-rw-rw-   0        0        0     4017 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/msg_classes/task_request.py
--rw-rw-rw-   0        0        0    41660 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/ole_writer.py
--rw-rw-rw-   0        0        0     8558 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/open_msg.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.188316 extract_msg-0.43.0/extract_msg/properties/
--rw-rw-rw-   0        0        0      549 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/properties/__init__.py
--rw-rw-rw-   0        0        0    15147 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/properties/named.py
--rw-rw-rw-   0        0        0     6806 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/properties/prop.py
--rw-rw-rw-   0        0        0     7627 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/properties/properties_store.py
--rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.43.0/extract_msg/py.typed
--rw-rw-rw-   0        0        0    13687 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/recipient.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.202279 extract_msg-0.43.0/extract_msg/structures/
--rw-rw-rw-   0        0        0      336 2023-05-09 19:54:43.000000 extract_msg-0.43.0/extract_msg/structures/__init__.py
--rw-rw-rw-   0        0        0    11737 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/structures/_helpers.py
--rw-rw-rw-   0        0        0     6682 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/structures/business_card.py
--rw-rw-rw-   0        0        0    19050 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/structures/entry_id.py
--rw-rw-rw-   0        0        0     6179 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/structures/misc_id.py
--rw-rw-rw-   0        0        0     7352 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/structures/recurrence_pattern.py
--rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.43.0/extract_msg/structures/report_tag.py
--rw-rw-rw-   0        0        0     1397 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/structures/system_time.py
--rw-rw-rw-   0        0        0     1616 2023-05-09 19:54:43.000000 extract_msg-0.43.0/extract_msg/structures/time_zone_definition.py
--rw-rw-rw-   0        0        0     2443 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/structures/time_zone_struct.py
--rw-rw-rw-   0        0        0     3254 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/structures/tz_rule.py
--rw-rw-rw-   0        0        0    48405 2023-07-29 23:17:08.000000 extract_msg-0.43.0/extract_msg/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:36:00.110525 extract_msg-0.43.0/extract_msg.egg-info/
--rw-rw-rw-   0        0        0    12250 2023-08-03 03:35:59.000000 extract_msg-0.43.0/extract_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3136 2023-08-03 03:35:59.000000 extract_msg-0.43.0/extract_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 03:35:59.000000 extract_msg-0.43.0/extract_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-08-03 03:35:59.000000 extract_msg-0.43.0/extract_msg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      270 2023-08-03 03:35:59.000000 extract_msg-0.43.0/extract_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-03 03:35:59.000000 extract_msg-0.43.0/extract_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      193 2023-07-29 23:17:08.000000 extract_msg-0.43.0/requirements.txt
--rw-rw-rw-   0        0        0      218 2023-08-03 03:36:00.205271 extract_msg-0.43.0/setup.cfg
--rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.43.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.696140 extract_msg-0.44.0/
+-rw-rw-rw-   0        0        0    85189 2023-08-03 21:39:50.000000 extract_msg-0.44.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.44.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.44.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12474 2023-08-03 21:39:54.696140 extract_msg-0.44.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11647 2023-08-03 21:39:50.000000 extract_msg-0.44.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.415504 extract_msg-0.44.0/extract_msg/
+-rw-rw-rw-   0        0        0     1937 2023-08-03 21:39:50.000000 extract_msg-0.44.0/extract_msg/__init__.py
+-rw-rw-rw-   0        0        0     3629 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.450917 extract_msg-0.44.0/extract_msg/_rtf/
+-rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.44.0/extract_msg/_rtf/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-05-09 19:54:43.000000 extract_msg-0.44.0/extract_msg/_rtf/create_doc.py
+-rw-rw-rw-   0        0        0     6250 2023-05-09 19:54:43.000000 extract_msg-0.44.0/extract_msg/_rtf/inject_rtf.py
+-rw-rw-rw-   0        0        0      856 2023-05-09 19:54:43.000000 extract_msg-0.44.0/extract_msg/_rtf/token.py
+-rw-rw-rw-   0        0        0     8932 2023-05-09 19:54:43.000000 extract_msg-0.44.0/extract_msg/_rtf/tokenize_rtf.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.487506 extract_msg-0.44.0/extract_msg/attachments/
+-rw-rw-rw-   0        0        0     5756 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/attachments/__init__.py
+-rw-rw-rw-   0        0        0     7338 2023-07-31 13:37:55.000000 extract_msg-0.44.0/extract_msg/attachments/attachment.py
+-rw-rw-rw-   0        0        0    23038 2023-08-03 03:03:26.000000 extract_msg-0.44.0/extract_msg/attachments/attachment_base.py
+-rw-rw-rw-   0        0        0     1188 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/attachments/broken_att.py
+-rw-rw-rw-   0        0        0     6051 2023-07-31 13:37:55.000000 extract_msg-0.44.0/extract_msg/attachments/custom_att.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.496494 extract_msg-0.44.0/extract_msg/attachments/custom_att_handler/
+-rw-rw-rw-   0        0        0     2591 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/attachments/custom_att_handler/__init__.py
+-rw-rw-rw-   0        0        0     1766 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/attachments/custom_att_handler/custom_handler.py
+-rw-rw-rw-   0        0        0     4754 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/attachments/custom_att_handler/outlook_image_dib.py
+-rw-rw-rw-   0        0        0     5004 2023-07-31 13:37:55.000000 extract_msg-0.44.0/extract_msg/attachments/emb_msg_att.py
+-rw-rw-rw-   0        0        0     9052 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/attachments/signed_att.py
+-rw-rw-rw-   0        0        0     1162 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/attachments/unsupported_att.py
+-rw-rw-rw-   0        0        0     2442 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/attachments/web_att.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.506461 extract_msg-0.44.0/extract_msg/constants/
+-rw-rw-rw-   0        0        0     5670 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/constants/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/constants/ps.py
+-rw-rw-rw-   0        0        0      874 2023-07-31 13:37:55.000000 extract_msg-0.44.0/extract_msg/constants/re.py
+-rw-rw-rw-   0        0        0     3237 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/constants/st.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.343454 extract_msg-0.44.0/extract_msg/data/
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.511019 extract_msg-0.44.0/extract_msg/data/logging-config/
+-rw-rw-rw-   0        0        0     2082 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/data/logging-config/logging-nt.json
+-rw-rw-rw-   0        0        0     2058 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/data/logging-config/logging-posix.json
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.529969 extract_msg-0.44.0/extract_msg/encoding/
+-rw-rw-rw-   0        0        0    12602 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/encoding/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.561053 extract_msg-0.44.0/extract_msg/encoding/_dt/
+-rw-rw-rw-   0        0        0      116 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/encoding/_dt/__init__.py
+-rw-rw-rw-   0        0        0     2743 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/encoding/_dt/_mac_ce.py
+-rw-rw-rw-   0        0        0     2785 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/encoding/_dt/_mac_cyrillic.py
+-rw-rw-rw-   0        0        0     2721 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/encoding/_dt/_mac_greek.py
+-rw-rw-rw-   0        0        0     2627 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/encoding/_dt/_mac_iceland.py
+-rw-rw-rw-   0        0        0     2628 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/encoding/_dt/_mac_turkish.py
+-rw-rw-rw-   0        0        0     2422 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/encoding/_dt/_win874_dec.py
+-rw-rw-rw-   0        0        0   298022 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/encoding/_dt/_win950_dec.py
+-rw-rw-rw-   0        0        0    12122 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/encoding/utils.py
+-rw-rw-rw-   0        0        0    58987 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/enums.py
+-rw-rw-rw-   0        0        0     4048 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.634226 extract_msg-0.44.0/extract_msg/msg_classes/
+-rw-rw-rw-   0        0        0     1249 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/__init__.py
+-rw-rw-rw-   0        0        0     6722 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/appointment.py
+-rw-rw-rw-   0        0        0     2930 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/calendar.py
+-rw-rw-rw-   0        0        0    19315 2023-08-03 21:39:50.000000 extract_msg-0.44.0/extract_msg/msg_classes/calendar_base.py
+-rw-rw-rw-   0        0        0    46043 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/contact.py
+-rw-rw-rw-   0        0        0     3590 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/meeting_cancellation.py
+-rw-rw-rw-   0        0        0     1630 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/meeting_exception.py
+-rw-rw-rw-   0        0        0     3737 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/meeting_forward.py
+-rw-rw-rw-   0        0        0     1900 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/meeting_related.py
+-rw-rw-rw-   0        0        0     6577 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/meeting_request.py
+-rw-rw-rw-   0        0        0     2223 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/meeting_response.py
+-rw-rw-rw-   0        0        0      163 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/message.py
+-rw-rw-rw-   0        0        0    58309 2023-08-03 21:39:50.000000 extract_msg-0.44.0/extract_msg/msg_classes/message_base.py
+-rw-rw-rw-   0        0        0      201 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/message_signed.py
+-rw-rw-rw-   0        0        0     5016 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/message_signed_base.py
+-rw-rw-rw-   0        0        0    37988 2023-08-03 21:39:50.000000 extract_msg-0.44.0/extract_msg/msg_classes/msg.py
+-rw-rw-rw-   0        0        0     2610 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/post.py
+-rw-rw-rw-   0        0        0     1675 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/sticky_note.py
+-rw-rw-rw-   0        0        0    12686 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/task.py
+-rw-rw-rw-   0        0        0     4017 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/msg_classes/task_request.py
+-rw-rw-rw-   0        0        0    41660 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/ole_writer.py
+-rw-rw-rw-   0        0        0     8558 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/open_msg.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.650292 extract_msg-0.44.0/extract_msg/properties/
+-rw-rw-rw-   0        0        0      549 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/properties/__init__.py
+-rw-rw-rw-   0        0        0    15147 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/properties/named.py
+-rw-rw-rw-   0        0        0     6806 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/properties/prop.py
+-rw-rw-rw-   0        0        0     7627 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/properties/properties_store.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.44.0/extract_msg/py.typed
+-rw-rw-rw-   0        0        0    13687 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/recipient.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.695167 extract_msg-0.44.0/extract_msg/structures/
+-rw-rw-rw-   0        0        0      336 2023-05-09 19:54:43.000000 extract_msg-0.44.0/extract_msg/structures/__init__.py
+-rw-rw-rw-   0        0        0    11737 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/structures/_helpers.py
+-rw-rw-rw-   0        0        0     6682 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/structures/business_card.py
+-rw-rw-rw-   0        0        0    19050 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/structures/entry_id.py
+-rw-rw-rw-   0        0        0     6179 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/structures/misc_id.py
+-rw-rw-rw-   0        0        0     7352 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/structures/recurrence_pattern.py
+-rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.44.0/extract_msg/structures/report_tag.py
+-rw-rw-rw-   0        0        0     1397 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/structures/system_time.py
+-rw-rw-rw-   0        0        0     1616 2023-05-09 19:54:43.000000 extract_msg-0.44.0/extract_msg/structures/time_zone_definition.py
+-rw-rw-rw-   0        0        0     2443 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/structures/time_zone_struct.py
+-rw-rw-rw-   0        0        0     3254 2023-07-29 23:17:08.000000 extract_msg-0.44.0/extract_msg/structures/tz_rule.py
+-rw-rw-rw-   0        0        0    48515 2023-08-03 21:39:50.000000 extract_msg-0.44.0/extract_msg/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:39:54.434362 extract_msg-0.44.0/extract_msg.egg-info/
+-rw-rw-rw-   0        0        0    12474 2023-08-03 21:39:54.000000 extract_msg-0.44.0/extract_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3136 2023-08-03 21:39:54.000000 extract_msg-0.44.0/extract_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 21:39:54.000000 extract_msg-0.44.0/extract_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-08-03 21:39:54.000000 extract_msg-0.44.0/extract_msg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      270 2023-08-03 21:39:54.000000 extract_msg-0.44.0/extract_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-03 21:39:54.000000 extract_msg-0.44.0/extract_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      193 2023-07-29 23:17:08.000000 extract_msg-0.44.0/requirements.txt
+-rw-rw-rw-   0        0        0      218 2023-08-03 21:39:54.698135 extract_msg-0.44.0/setup.cfg
+-rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.44.0/setup.py
```

### Comparing `extract_msg-0.43.0/CHANGELOG.md` & `extract_msg-0.44.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+**v0.44.0**
+* Fixed a bug that caused `MessageBase.headerInit` to always return `False` after the 0.42.0 update.
+* Changed `MessageBase.headerInit` to a property.
+* Fixed `extract_msg.utils.__all__`.
+* Minor regoanization within `extract_msg/utils.py`.
+* Minor changes to docstrings.
+* Minor README updates.
+* Fix issue with folded header fields decoding incorrectly when given to `extract_msg.utils.decodeRfc2047`.
+
 **v0.43.0**
 * [[TeamMsgExtractor #56](https://github.com/TeamMsgExtractor/msg-extractor/issues/56)] [[TeamMsgExtractor #248](https://github.com/TeamMsgExtractor/msg-extractor/issues/248)] Added new function `MessageBase.asEmailMessage` which will convert the `MessageBase` instance, if possible, to an `email.message.EmailMessage` object. If an embedded MSG file on a `MessageBase` object is of a class that does not have this function, it will simply be attached to the instance as bytes.
 * Changed imports in `message_base.py` to help with type checkers.
 * Changed from using `email.parser.EmailParser` to `email.parser.HeaderParser` in `MessageBase.header`.
 * Changed some of the internal code for `MessageBase.header`. This should improve usage of it, and should not have any noticeable negative changes. You man notice some of the values parse slightly differently, but this effect should be mostly suppressed.
 
 **v0.42.2**
```

### Comparing `extract_msg-0.43.0/LICENSE.txt` & `extract_msg-0.44.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/PKG-INFO` & `extract_msg-0.44.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: extract_msg
-Version: 0.43.0
+Version: 0.44.0
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: mime
 Provides-Extra: image
 License-File: LICENSE.txt
 
-|License: GPL v3| |PyPI3| |PyPI2|
+|License: GPL v3| |PyPI3| |PyPI2| |Read the Docs|
 
 extract-msg
 =============
 
 Extracts emails and attachments saved in Microsoft Outlook's .msg files
 
 The python package extract_msg automates the extraction of key email
 data (from, to, cc, date, subject, body) and the email's attachments.
 
 Documentation can be found in the code, on the `wiki`_, and on the
-`read the docs`_ page.
+`Read the Docs`_ page.
 
 NOTICE
 ======
 0.29.* is the branch that supports both Python 2 and Python 3. It is now only
 receiving bug fixes and will not be receiving feature updates.
 
 0.39.* is the last versions that supported Python 3.6 and 3.7. Support for those
@@ -254,28 +254,33 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.43.0-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.43.0/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.44.0-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.44.0/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
+
+.. |Read the Docs| image:: https://readthedocs.org/projects/msg-extractor/badge/?version=latest
+    :target: https://msg-extractor.readthedocs.io/en/stable/?badge=latest
+    :alt: Documentation Status
+
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
 .. _Dean Malmgren: https://github.com/deanmalmgren
 .. _Joel Kaufman: https://github.com/joelkaufman
 .. _Liam: https://github.com/LiamPM5
 .. _Seamus Tuohy: https://github.com/seamustuohy
 .. _Discord: https://discord.com/invite/B77McRmzdc
 .. _Buy Me a Coffee: https://www.buymeacoffee.com/DestructionE
 .. _Ko-fi: https://ko-fi.com/destructione
 .. _Patreon: https://www.patreon.com/DestructionE
 .. _msg-explorer: https://pypi.org/project/msg-explorer/
 .. _wiki: https://github.com/TeamMsgExtractor/msg-extractor/wiki
-.. _read the docs: https://msg-extractor.rtfd.io/
+.. _Read the Docs: https://msg-extractor.rtfd.io/
 .. _Changelog: https://github.com/TeamMsgExtractor/msg-extractor/blob/master/CHANGELOG.md
```

### Comparing `extract_msg-0.43.0/README.rst` & `extract_msg-0.44.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-|License: GPL v3| |PyPI3| |PyPI2|
+|License: GPL v3| |PyPI3| |PyPI2| |Read the Docs|
 
 extract-msg
 =============
 
 Extracts emails and attachments saved in Microsoft Outlook's .msg files
 
 The python package extract_msg automates the extraction of key email
 data (from, to, cc, date, subject, body) and the email's attachments.
 
 Documentation can be found in the code, on the `wiki`_, and on the
-`read the docs`_ page.
+`Read the Docs`_ page.
 
 NOTICE
 ======
 0.29.* is the branch that supports both Python 2 and Python 3. It is now only
 receiving bug fixes and will not be receiving feature updates.
 
 0.39.* is the last versions that supported Python 3.6 and 3.7. Support for those
@@ -238,28 +238,33 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.43.0-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.43.0/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.44.0-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.44.0/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
+
+.. |Read the Docs| image:: https://readthedocs.org/projects/msg-extractor/badge/?version=latest
+    :target: https://msg-extractor.readthedocs.io/en/stable/?badge=latest
+    :alt: Documentation Status
+
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
 .. _Dean Malmgren: https://github.com/deanmalmgren
 .. _Joel Kaufman: https://github.com/joelkaufman
 .. _Liam: https://github.com/LiamPM5
 .. _Seamus Tuohy: https://github.com/seamustuohy
 .. _Discord: https://discord.com/invite/B77McRmzdc
 .. _Buy Me a Coffee: https://www.buymeacoffee.com/DestructionE
 .. _Ko-fi: https://ko-fi.com/destructione
 .. _Patreon: https://www.patreon.com/DestructionE
 .. _msg-explorer: https://pypi.org/project/msg-explorer/
 .. _wiki: https://github.com/TeamMsgExtractor/msg-extractor/wiki
-.. _read the docs: https://msg-extractor.rtfd.io/
+.. _Read the Docs: https://msg-extractor.rtfd.io/
 .. _Changelog: https://github.com/TeamMsgExtractor/msg-extractor/blob/master/CHANGELOG.md
```

### Comparing `extract_msg-0.43.0/extract_msg/__init__.py` & `extract_msg-0.44.0/extract_msg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = 'Destiny Peterson & Matthew Walker'
-__date__ = '2023-08-02'
-__version__ = '0.43.0'
+__date__ = '2023-08-03'
+__version__ = '0.44.0'
 
 __all__ = [
     # Modules:
     'attachments',
     'enums',
     'exceptions',
     'msg_classes',
```

### Comparing `extract_msg-0.43.0/extract_msg/__main__.py` & `extract_msg-0.44.0/extract_msg/__main__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/_rtf/create_doc.py` & `extract_msg-0.44.0/extract_msg/_rtf/create_doc.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/_rtf/inject_rtf.py` & `extract_msg-0.44.0/extract_msg/_rtf/inject_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/_rtf/token.py` & `extract_msg-0.44.0/extract_msg/_rtf/token.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/_rtf/tokenize_rtf.py` & `extract_msg-0.44.0/extract_msg/_rtf/tokenize_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/__init__.py` & `extract_msg-0.44.0/extract_msg/attachments/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/attachment.py` & `extract_msg-0.44.0/extract_msg/attachments/attachment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/attachment_base.py` & `extract_msg-0.44.0/extract_msg/attachments/attachment_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/broken_att.py` & `extract_msg-0.44.0/extract_msg/attachments/broken_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/custom_att.py` & `extract_msg-0.44.0/extract_msg/attachments/custom_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/custom_att_handler/__init__.py` & `extract_msg-0.44.0/extract_msg/attachments/custom_att_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/custom_att_handler/custom_handler.py` & `extract_msg-0.44.0/extract_msg/attachments/custom_att_handler/custom_handler.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/custom_att_handler/outlook_image_dib.py` & `extract_msg-0.44.0/extract_msg/attachments/custom_att_handler/outlook_image_dib.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/emb_msg_att.py` & `extract_msg-0.44.0/extract_msg/attachments/emb_msg_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/signed_att.py` & `extract_msg-0.44.0/extract_msg/attachments/signed_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/unsupported_att.py` & `extract_msg-0.44.0/extract_msg/attachments/unsupported_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/attachments/web_att.py` & `extract_msg-0.44.0/extract_msg/attachments/web_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/constants/__init__.py` & `extract_msg-0.44.0/extract_msg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/constants/ps.py` & `extract_msg-0.44.0/extract_msg/constants/ps.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/constants/re.py` & `extract_msg-0.44.0/extract_msg/constants/re.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/constants/st.py` & `extract_msg-0.44.0/extract_msg/constants/st.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/data/logging-config/logging-nt.json` & `extract_msg-0.44.0/extract_msg/data/logging-config/logging-nt.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/data/logging-config/logging-posix.json` & `extract_msg-0.44.0/extract_msg/data/logging-config/logging-posix.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/encoding/__init__.py` & `extract_msg-0.44.0/extract_msg/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/encoding/_dt/_mac_ce.py` & `extract_msg-0.44.0/extract_msg/encoding/_dt/_mac_ce.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/encoding/_dt/_mac_cyrillic.py` & `extract_msg-0.44.0/extract_msg/encoding/_dt/_mac_cyrillic.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/encoding/_dt/_mac_greek.py` & `extract_msg-0.44.0/extract_msg/encoding/_dt/_mac_greek.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/encoding/_dt/_mac_iceland.py` & `extract_msg-0.44.0/extract_msg/encoding/_dt/_mac_iceland.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/encoding/_dt/_mac_turkish.py` & `extract_msg-0.44.0/extract_msg/encoding/_dt/_mac_turkish.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/encoding/_dt/_win874_dec.py` & `extract_msg-0.44.0/extract_msg/encoding/_dt/_win874_dec.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/encoding/_dt/_win950_dec.py` & `extract_msg-0.44.0/extract_msg/encoding/_dt/_win950_dec.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/encoding/utils.py` & `extract_msg-0.44.0/extract_msg/encoding/utils.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/enums.py` & `extract_msg-0.44.0/extract_msg/enums.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/exceptions.py` & `extract_msg-0.44.0/extract_msg/exceptions.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/__init__.py` & `extract_msg-0.44.0/extract_msg/msg_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/appointment.py` & `extract_msg-0.44.0/extract_msg/msg_classes/appointment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/calendar.py` & `extract_msg-0.44.0/extract_msg/msg_classes/calendar.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/calendar_base.py` & `extract_msg-0.44.0/extract_msg/msg_classes/calendar_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,24 +31,24 @@
     def _genRecipient(self, recipientType, recipientInt : MeetingRecipientType) -> Optional[str]:
         """
         Returns the specified recipient field.
         """
         recipientInt = MeetingRecipientType(recipientInt)
         value = None
         # Check header first.
-        if self.headerInit():
+        if self.headerInit:
             value = self.header[recipientType]
             if value:
                 value = value.replace(',', self.recipientSeparator)
 
         # If the header had a blank field or didn't have the field, generate
         # it manually.
         if not value:
             # Check if the header has initialized.
-            if self.headerInit():
+            if self.headerInit:
                 logger.info(f'Header found, but "{recipientType}" is not included. Will be generated from other streams.')
 
             # Get a list of the recipients of the specified type.
             foundRecipients = tuple(recipient.formatted for recipient in self.recipients if recipient.type == recipientInt)
 
             # If we found recipients, join them with the recipient separator
             # and a space.
```

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/contact.py` & `extract_msg-0.44.0/extract_msg/msg_classes/contact.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/meeting_cancellation.py` & `extract_msg-0.44.0/extract_msg/msg_classes/meeting_cancellation.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/meeting_exception.py` & `extract_msg-0.44.0/extract_msg/msg_classes/meeting_exception.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/meeting_forward.py` & `extract_msg-0.44.0/extract_msg/msg_classes/meeting_forward.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/meeting_related.py` & `extract_msg-0.44.0/extract_msg/msg_classes/meeting_related.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/meeting_request.py` & `extract_msg-0.44.0/extract_msg/msg_classes/meeting_request.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/meeting_response.py` & `extract_msg-0.44.0/extract_msg/msg_classes/meeting_response.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/message_base.py` & `extract_msg-0.44.0/extract_msg/msg_classes/message_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                 errorBehavior |= ErrorBehavior.RTFDE
                 kwargs['errorBehavior'] = errorBehavior
 
         super().__init__(path, **kwargs)
         # The rest needs to be in a try-except block to ensure the file closes
         # if an error occurs.
         try:
+            self.__headerInit = False
             self.__recipientSeparator = kwargs.get('recipientSeparator', ';')
             self.__deencap = kwargs.get('deencapsulationFunc')
             # Initialize properties in the order that is least likely to cause bugs.
             # TODO have each function check for initialization of needed data so
             # these lines will be unnecessary.
             self.props
             self.header
@@ -121,25 +122,25 @@
     def _genRecipient(self, recipientType, recipientInt : RecipientType) -> Optional[str]:
         """
         Returns the specified recipient field.
         """
         recipientInt = RecipientType(recipientInt)
         value = None
         # Check header first.
-        if self.headerInit():
+        if self.headerInit:
             value = self.header[recipientType]
             if value:
                 value = decodeRfc2047(value)
                 value = value.replace(',', self.__recipientSeparator)
 
         # If the header had a blank field or didn't have the field, generate
         # it manually.
         if not value:
             # Check if the header has initialized.
-            if self.headerInit():
+            if self.headerInit:
                 logger.info(f'Header found, but "{recipientType}" is not included. Will be generated from other streams.')
 
             # Get a list of the recipients of the specified type.
             foundRecipients = tuple(recipient.formatted for recipient in self.recipients if recipient.type == recipientInt)
 
             # If we found recipients, join them with the recipient separator
             # and a space.
@@ -468,24 +469,14 @@
 
         :param kwargs: Used to allow kwargs expansion in the save function.
             Arguments absorbed by this are simply ignored.
         """
         # Inject the header into the data.
         return self.injectRtfHeader()
 
-    def headerInit(self) -> bool:
-        """
-        Checks whether the header has been initialized.
-        """
-        try:
-            self._header
-            return True
-        except AttributeError:
-            return False
-
     def injectHtmlHeader(self, prepared : bool = False) -> bytes:
         """
         Returns the HTML body from the MSG file (will check that it has one) with
         the HTML header injected into it.
 
         :param prepared: Determines whether to be using the standard HTML (False) or
             the prepared HTML (True) body (Default: False).
@@ -1076,14 +1067,15 @@
             header.add_header('To', self.to)
             header.add_header('Cc', self.cc)
             header.add_header('Bcc', self.bcc)
             header.add_header('Message-Id', self.messageId)
             # TODO find authentication results outside of header
             header.add_header('Authentication-Results', None)
 
+        self.__headerInit = True
         return header
 
     @property
     def headerDict(self) -> dict:
         """
         Returns a dictionary of the entries in the header
         """
@@ -1135,14 +1127,21 @@
                 'Subject': self.subject,
             },
             '-importance-': {
                 'Importance': self.importanceString,
             },
         }
 
+    @property
+    def headerInit(self) -> bool:
+        """
+        Checks whether the header has been initialized.
+        """
+        return self.__headerInit
+
     @functools.cached_property
     def headerText(self) -> Optional[str]:
         """
         The raw text of the header stream, if it exists.
         """
         return self._getStringStream('__substg1.0_007D')
 
@@ -1236,20 +1235,20 @@
             return True
         else:
             return not bool(self.props['0E070003'].value & 8)
 
     @functools.cached_property
     def messageId(self) -> Optional[str]:
         headerResult = None
-        if self.headerInit():
+        if self.headerInit:
             headerResult = self.header['message-id']
         if headerResult is not None:
             return headerResult
 
-        if self.headerInit():
+        if self.headerInit:
             logger.info('Header found, but "Message-Id" is not included. Will be generated from other streams.')
         return self._getStringStream('__substg1.0_1035')
 
     @functools.cached_property
     def parsedDate(self):
         return email.utils.parsedate(self.date)
 
@@ -1319,15 +1318,15 @@
 
     @functools.cached_property
     def sender(self) -> Optional[str]:
         """
         Returns the message sender, if it exists.
         """
         # Check header first
-        if self.headerInit():
+        if self.headerInit:
             headerResult = self.header['from']
             if headerResult is not None:
                 return decodeRfc2047(headerResult)
             logger.info('Header found, but "sender" is not included. Will be generated from other streams.')
         # Extract from other fields
         text = self._getStringStream('__substg1.0_0C1A')
         email = self._getStringStream('__substg1.0_5D01')
```

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/message_signed_base.py` & `extract_msg-0.44.0/extract_msg/msg_classes/message_signed_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/msg.py` & `extract_msg-0.44.0/extract_msg/msg_classes/msg.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
 
     def __init__(self, path, **kwargs):
         """
         :param path: path to the msg file in the system or is the raw msg file.
         :param prefix: Used for extracting embedded msg files inside the main
             one. Do not set manually unless you know what you are doing.
-        :param parentMsg: Used for synchronizing named properties instances. Do
+        :param parentMsg: Used for synchronizing instances of shared objects. Do
             not set this unless you know what you are doing.
         :param initAttachment: Optional, the method used when creating an
             attachment for an MSG file. MUST be a function that takes 2
             arguments (the MSGFile instance and the directory in the MSG file
             where the attachment is) and returns an instance of AttachmentBase.
         :param delayAttachments: Optional, delays the initialization of
             attachments until the user attempts to retrieve them. Allows MSG
```

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/post.py` & `extract_msg-0.44.0/extract_msg/msg_classes/post.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/sticky_note.py` & `extract_msg-0.44.0/extract_msg/msg_classes/sticky_note.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/task.py` & `extract_msg-0.44.0/extract_msg/msg_classes/task.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/msg_classes/task_request.py` & `extract_msg-0.44.0/extract_msg/msg_classes/task_request.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/ole_writer.py` & `extract_msg-0.44.0/extract_msg/ole_writer.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/open_msg.py` & `extract_msg-0.44.0/extract_msg/open_msg.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/properties/__init__.py` & `extract_msg-0.44.0/extract_msg/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/properties/named.py` & `extract_msg-0.44.0/extract_msg/properties/named.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/properties/prop.py` & `extract_msg-0.44.0/extract_msg/properties/prop.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/properties/properties_store.py` & `extract_msg-0.44.0/extract_msg/properties/properties_store.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/recipient.py` & `extract_msg-0.44.0/extract_msg/recipient.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/structures/_helpers.py` & `extract_msg-0.44.0/extract_msg/structures/_helpers.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/structures/business_card.py` & `extract_msg-0.44.0/extract_msg/structures/business_card.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/structures/entry_id.py` & `extract_msg-0.44.0/extract_msg/structures/entry_id.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/structures/misc_id.py` & `extract_msg-0.44.0/extract_msg/structures/misc_id.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/structures/recurrence_pattern.py` & `extract_msg-0.44.0/extract_msg/structures/recurrence_pattern.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/structures/report_tag.py` & `extract_msg-0.44.0/extract_msg/structures/report_tag.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/structures/system_time.py` & `extract_msg-0.44.0/extract_msg/structures/system_time.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/structures/time_zone_definition.py` & `extract_msg-0.44.0/extract_msg/structures/time_zone_definition.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/structures/time_zone_struct.py` & `extract_msg-0.44.0/extract_msg/structures/time_zone_struct.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/structures/tz_rule.py` & `extract_msg-0.44.0/extract_msg/structures/tz_rule.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/extract_msg/utils.py` & `extract_msg-0.44.0/extract_msg/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     'addNumToZipDir',
     'bitwiseAdjust',
     'bitwiseAdjustedAnd',
     'bytesToGuid',
     'ceilDiv',
     'cloneOleFile',
     'createZipOpen',
+    'decodeRfc2047',
     'dictGetCasedKey',
     'divide',
     'filetimeToDatetime',
     'filetimeToUtc',
     'findWk',
     'fromTimeStamp',
     'getCommandArgs',
@@ -197,14 +198,17 @@
     return _open
 
 
 def decodeRfc2047(encoded : str) -> str:
     """
     Decodes text encoded using the method specified in RFC 2047.
     """
+    # Fix an issue with folded header fields.
+    encoded = encoded.replace('\r\n', '')
+
     # This returns a list of tuples containing the bytes and the encoding they
     # are using, so we decode each one and join them together.
     #
     # decode_header header will return a string instead of bytes for the first
     # object if the input is not encoded, something that is frustrating.
     return ''.join(
         x[0].decode(x[1] or 'ascii') if isinstance(x[0], bytes) else x[0]
@@ -273,14 +277,21 @@
     except TZError:
         # For TZError we just raise it again. It is a fatal error.
         raise
     except Exception as e:
         raise ValueError(f'Timestamp value of {filetimeToUtc(rawTime)} caused an exception. This was probably caused by the time stamp being too far in the future.')
 
 
+def filetimeToUtc(inp : int) -> float:
+    """
+    Converts a FILETIME into a unix timestamp.
+    """
+    return (inp - 116444736000000000) / 10000000.0
+
+
 def findWk(path = None):
     """
     Attempt to find the path of the wkhtmltopdf executable. If :param path: is
     provided, verifies that it is executable and returns the path if it is.
 
     :raises ExecutableNotFound: A valid executable could not be found.
     """
@@ -577,35 +588,28 @@
         return bytesInputVar.decode(encoding)
     elif bytesInputVar is None:
         return ''
     else:
         raise ConversionError('Cannot convert to str type.')
 
 
-def isEncapsulatedRtf(inp : bytes) -> bool:
-    """
-    Currently the detection is made to be *extremly* basic, but this will work
-    for now. In the future this will be fixed so that literal text in the body
-    of a message won't cause false detection.
-    """
-    return b'\\fromhtml' in inp
-
-
 def isEmptyString(inp : str) -> bool:
     """
     Returns true if the input is None or is an Empty string.
     """
     return (inp == '' or inp is None)
 
 
-def filetimeToUtc(inp : int) -> float:
+def isEncapsulatedRtf(inp : bytes) -> bool:
     """
-    Converts a FILETIME into a unix timestamp.
+    Currently the detection is made to be *extremly* basic, but this will work
+    for now. In the future this will be fixed so that literal text in the body
+    of a message won't cause false detection.
     """
-    return (inp - 116444736000000000) / 10000000.0
+    return b'\\fromhtml' in inp
 
 
 def makeWeakRef(obj : Optional[_T]) -> Optional[weakref.ReferenceType[_T]]:
     """
     Attempts to return a weak reference to the object, returning None if not
     possible.
     """
```

### Comparing `extract_msg-0.43.0/extract_msg.egg-info/PKG-INFO` & `extract_msg-0.44.0/extract_msg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: extract-msg
-Version: 0.43.0
+Version: 0.44.0
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: mime
 Provides-Extra: image
 License-File: LICENSE.txt
 
-|License: GPL v3| |PyPI3| |PyPI2|
+|License: GPL v3| |PyPI3| |PyPI2| |Read the Docs|
 
 extract-msg
 =============
 
 Extracts emails and attachments saved in Microsoft Outlook's .msg files
 
 The python package extract_msg automates the extraction of key email
 data (from, to, cc, date, subject, body) and the email's attachments.
 
 Documentation can be found in the code, on the `wiki`_, and on the
-`read the docs`_ page.
+`Read the Docs`_ page.
 
 NOTICE
 ======
 0.29.* is the branch that supports both Python 2 and Python 3. It is now only
 receiving bug fixes and will not be receiving feature updates.
 
 0.39.* is the last versions that supported Python 3.6 and 3.7. Support for those
@@ -254,28 +254,33 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.43.0-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.43.0/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.44.0-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.44.0/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
+
+.. |Read the Docs| image:: https://readthedocs.org/projects/msg-extractor/badge/?version=latest
+    :target: https://msg-extractor.readthedocs.io/en/stable/?badge=latest
+    :alt: Documentation Status
+
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
 .. _Dean Malmgren: https://github.com/deanmalmgren
 .. _Joel Kaufman: https://github.com/joelkaufman
 .. _Liam: https://github.com/LiamPM5
 .. _Seamus Tuohy: https://github.com/seamustuohy
 .. _Discord: https://discord.com/invite/B77McRmzdc
 .. _Buy Me a Coffee: https://www.buymeacoffee.com/DestructionE
 .. _Ko-fi: https://ko-fi.com/destructione
 .. _Patreon: https://www.patreon.com/DestructionE
 .. _msg-explorer: https://pypi.org/project/msg-explorer/
 .. _wiki: https://github.com/TeamMsgExtractor/msg-extractor/wiki
-.. _read the docs: https://msg-extractor.rtfd.io/
+.. _Read the Docs: https://msg-extractor.rtfd.io/
 .. _Changelog: https://github.com/TeamMsgExtractor/msg-extractor/blob/master/CHANGELOG.md
```

### Comparing `extract_msg-0.43.0/extract_msg.egg-info/SOURCES.txt` & `extract_msg-0.44.0/extract_msg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `extract_msg-0.43.0/setup.py` & `extract_msg-0.44.0/setup.py`

 * *Files identical despite different names*

