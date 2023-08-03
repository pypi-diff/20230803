# Comparing `tmp/extract_msg-0.42.1.tar.gz` & `tmp/extract_msg-0.42.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extract_msg-0.42.1.tar", last modified: Mon Jul 31 13:37:59 2023, max compression
+gzip compressed data, was "extract_msg-0.42.2.tar", last modified: Thu Aug  3 03:03:30 2023, max compression
```

## Comparing `extract_msg-0.42.1.tar` & `extract_msg-0.42.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.779826 extract_msg-0.42.1/
--rw-rw-rw-   0        0        0    83712 2023-07-31 13:37:55.000000 extract_msg-0.42.1/CHANGELOG.md
--rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.42.1/LICENSE.txt
--rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.42.1/MANIFEST.in
--rw-rw-rw-   0        0        0    12250 2023-07-31 13:37:59.779826 extract_msg-0.42.1/PKG-INFO
--rw-rw-rw-   0        0        0    11428 2023-07-31 13:37:55.000000 extract_msg-0.42.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.495579 extract_msg-0.42.1/extract_msg/
--rw-rw-rw-   0        0        0     1937 2023-07-31 13:37:55.000000 extract_msg-0.42.1/extract_msg/__init__.py
--rw-rw-rw-   0        0        0     3629 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.535061 extract_msg-0.42.1/extract_msg/_rtf/
--rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.42.1/extract_msg/_rtf/__init__.py
--rw-rw-rw-   0        0        0      845 2023-05-09 19:54:43.000000 extract_msg-0.42.1/extract_msg/_rtf/create_doc.py
--rw-rw-rw-   0        0        0     6250 2023-05-09 19:54:43.000000 extract_msg-0.42.1/extract_msg/_rtf/inject_rtf.py
--rw-rw-rw-   0        0        0      856 2023-05-09 19:54:43.000000 extract_msg-0.42.1/extract_msg/_rtf/token.py
--rw-rw-rw-   0        0        0     8932 2023-05-09 19:54:43.000000 extract_msg-0.42.1/extract_msg/_rtf/tokenize_rtf.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.571895 extract_msg-0.42.1/extract_msg/attachments/
--rw-rw-rw-   0        0        0     5756 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/attachments/__init__.py
--rw-rw-rw-   0        0        0     7338 2023-07-31 13:37:55.000000 extract_msg-0.42.1/extract_msg/attachments/attachment.py
--rw-rw-rw-   0        0        0    23050 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/attachments/attachment_base.py
--rw-rw-rw-   0        0        0     1188 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/attachments/broken_att.py
--rw-rw-rw-   0        0        0     6051 2023-07-31 13:37:55.000000 extract_msg-0.42.1/extract_msg/attachments/custom_att.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.577877 extract_msg-0.42.1/extract_msg/attachments/custom_att_handler/
--rw-rw-rw-   0        0        0     2591 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/attachments/custom_att_handler/__init__.py
--rw-rw-rw-   0        0        0     1766 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/attachments/custom_att_handler/custom_handler.py
--rw-rw-rw-   0        0        0     4754 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/attachments/custom_att_handler/outlook_image_dib.py
--rw-rw-rw-   0        0        0     5004 2023-07-31 13:37:55.000000 extract_msg-0.42.1/extract_msg/attachments/emb_msg_att.py
--rw-rw-rw-   0        0        0     9052 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/attachments/signed_att.py
--rw-rw-rw-   0        0        0     1162 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/attachments/unsupported_att.py
--rw-rw-rw-   0        0        0     2442 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/attachments/web_att.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.586853 extract_msg-0.42.1/extract_msg/constants/
--rw-rw-rw-   0        0        0     5670 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/constants/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/constants/ps.py
--rw-rw-rw-   0        0        0      874 2023-07-31 13:37:55.000000 extract_msg-0.42.1/extract_msg/constants/re.py
--rw-rw-rw-   0        0        0     3237 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/constants/st.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.368920 extract_msg-0.42.1/extract_msg/data/
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.590847 extract_msg-0.42.1/extract_msg/data/logging-config/
--rw-rw-rw-   0        0        0     2082 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/data/logging-config/logging-nt.json
--rw-rw-rw-   0        0        0     2058 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/data/logging-config/logging-posix.json
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.610817 extract_msg-0.42.1/extract_msg/encoding/
--rw-rw-rw-   0        0        0    12602 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/encoding/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.642706 extract_msg-0.42.1/extract_msg/encoding/_dt/
--rw-rw-rw-   0        0        0      116 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/encoding/_dt/__init__.py
--rw-rw-rw-   0        0        0     2743 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/encoding/_dt/_mac_ce.py
--rw-rw-rw-   0        0        0     2785 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/encoding/_dt/_mac_cyrillic.py
--rw-rw-rw-   0        0        0     2721 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/encoding/_dt/_mac_greek.py
--rw-rw-rw-   0        0        0     2627 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/encoding/_dt/_mac_iceland.py
--rw-rw-rw-   0        0        0     2628 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/encoding/_dt/_mac_turkish.py
--rw-rw-rw-   0        0        0     2422 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/encoding/_dt/_win874_dec.py
--rw-rw-rw-   0        0        0   298022 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/encoding/_dt/_win950_dec.py
--rw-rw-rw-   0        0        0    12122 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/encoding/utils.py
--rw-rw-rw-   0        0        0    58987 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/enums.py
--rw-rw-rw-   0        0        0     4048 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.726970 extract_msg-0.42.1/extract_msg/msg_classes/
--rw-rw-rw-   0        0        0     1249 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/__init__.py
--rw-rw-rw-   0        0        0     6722 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/appointment.py
--rw-rw-rw-   0        0        0     2930 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/calendar.py
--rw-rw-rw-   0        0        0    19319 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/calendar_base.py
--rw-rw-rw-   0        0        0    46043 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/contact.py
--rw-rw-rw-   0        0        0     3590 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/meeting_cancellation.py
--rw-rw-rw-   0        0        0     1630 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/meeting_exception.py
--rw-rw-rw-   0        0        0     3737 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/meeting_forward.py
--rw-rw-rw-   0        0        0     1900 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/meeting_related.py
--rw-rw-rw-   0        0        0     6577 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/meeting_request.py
--rw-rw-rw-   0        0        0     2223 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/meeting_response.py
--rw-rw-rw-   0        0        0      163 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/message.py
--rw-rw-rw-   0        0        0    55795 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/message_base.py
--rw-rw-rw-   0        0        0      201 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/message_signed.py
--rw-rw-rw-   0        0        0     5016 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/message_signed_base.py
--rw-rw-rw-   0        0        0    37987 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/msg.py
--rw-rw-rw-   0        0        0     2610 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/post.py
--rw-rw-rw-   0        0        0     1675 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/sticky_note.py
--rw-rw-rw-   0        0        0    12686 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/task.py
--rw-rw-rw-   0        0        0     4017 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/msg_classes/task_request.py
--rw-rw-rw-   0        0        0    41660 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/ole_writer.py
--rw-rw-rw-   0        0        0     8558 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/open_msg.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.740928 extract_msg-0.42.1/extract_msg/properties/
--rw-rw-rw-   0        0        0      549 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/properties/__init__.py
--rw-rw-rw-   0        0        0    15147 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/properties/named.py
--rw-rw-rw-   0        0        0     6806 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/properties/prop.py
--rw-rw-rw-   0        0        0     7627 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/properties/properties_store.py
--rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.42.1/extract_msg/py.typed
--rw-rw-rw-   0        0        0    13687 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/recipient.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.777833 extract_msg-0.42.1/extract_msg/structures/
--rw-rw-rw-   0        0        0      336 2023-05-09 19:54:43.000000 extract_msg-0.42.1/extract_msg/structures/__init__.py
--rw-rw-rw-   0        0        0    11737 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/structures/_helpers.py
--rw-rw-rw-   0        0        0     6682 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/structures/business_card.py
--rw-rw-rw-   0        0        0    19050 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/structures/entry_id.py
--rw-rw-rw-   0        0        0     6179 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/structures/misc_id.py
--rw-rw-rw-   0        0        0     7352 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/structures/recurrence_pattern.py
--rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.42.1/extract_msg/structures/report_tag.py
--rw-rw-rw-   0        0        0     1397 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/structures/system_time.py
--rw-rw-rw-   0        0        0     1616 2023-05-09 19:54:43.000000 extract_msg-0.42.1/extract_msg/structures/time_zone_definition.py
--rw-rw-rw-   0        0        0     2443 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/structures/time_zone_struct.py
--rw-rw-rw-   0        0        0     3254 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/structures/tz_rule.py
--rw-rw-rw-   0        0        0    48405 2023-07-29 23:17:08.000000 extract_msg-0.42.1/extract_msg/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:37:59.516524 extract_msg-0.42.1/extract_msg.egg-info/
--rw-rw-rw-   0        0        0    12250 2023-07-31 13:37:59.000000 extract_msg-0.42.1/extract_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3136 2023-07-31 13:37:59.000000 extract_msg-0.42.1/extract_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 13:37:59.000000 extract_msg-0.42.1/extract_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-31 13:37:59.000000 extract_msg-0.42.1/extract_msg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      270 2023-07-31 13:37:59.000000 extract_msg-0.42.1/extract_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-31 13:37:59.000000 extract_msg-0.42.1/extract_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      193 2023-07-29 23:17:08.000000 extract_msg-0.42.1/requirements.txt
--rw-rw-rw-   0        0        0      218 2023-07-31 13:37:59.782826 extract_msg-0.42.1/setup.cfg
--rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.42.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.572479 extract_msg-0.42.2/
+-rw-rw-rw-   0        0        0    83855 2023-08-03 03:03:26.000000 extract_msg-0.42.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.42.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.42.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    12250 2023-08-03 03:03:30.573482 extract_msg-0.42.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11428 2023-08-03 03:03:26.000000 extract_msg-0.42.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.264305 extract_msg-0.42.2/extract_msg/
+-rw-rw-rw-   0        0        0     1937 2023-08-03 03:03:26.000000 extract_msg-0.42.2/extract_msg/__init__.py
+-rw-rw-rw-   0        0        0     3629 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.306220 extract_msg-0.42.2/extract_msg/_rtf/
+-rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.42.2/extract_msg/_rtf/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-05-09 19:54:43.000000 extract_msg-0.42.2/extract_msg/_rtf/create_doc.py
+-rw-rw-rw-   0        0        0     6250 2023-05-09 19:54:43.000000 extract_msg-0.42.2/extract_msg/_rtf/inject_rtf.py
+-rw-rw-rw-   0        0        0      856 2023-05-09 19:54:43.000000 extract_msg-0.42.2/extract_msg/_rtf/token.py
+-rw-rw-rw-   0        0        0     8932 2023-05-09 19:54:43.000000 extract_msg-0.42.2/extract_msg/_rtf/tokenize_rtf.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.334117 extract_msg-0.42.2/extract_msg/attachments/
+-rw-rw-rw-   0        0        0     5756 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/attachments/__init__.py
+-rw-rw-rw-   0        0        0     7338 2023-07-31 13:37:55.000000 extract_msg-0.42.2/extract_msg/attachments/attachment.py
+-rw-rw-rw-   0        0        0    23038 2023-08-03 03:03:26.000000 extract_msg-0.42.2/extract_msg/attachments/attachment_base.py
+-rw-rw-rw-   0        0        0     1188 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/attachments/broken_att.py
+-rw-rw-rw-   0        0        0     6051 2023-07-31 13:37:55.000000 extract_msg-0.42.2/extract_msg/attachments/custom_att.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.341100 extract_msg-0.42.2/extract_msg/attachments/custom_att_handler/
+-rw-rw-rw-   0        0        0     2591 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/attachments/custom_att_handler/__init__.py
+-rw-rw-rw-   0        0        0     1766 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/attachments/custom_att_handler/custom_handler.py
+-rw-rw-rw-   0        0        0     4754 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/attachments/custom_att_handler/outlook_image_dib.py
+-rw-rw-rw-   0        0        0     5004 2023-07-31 13:37:55.000000 extract_msg-0.42.2/extract_msg/attachments/emb_msg_att.py
+-rw-rw-rw-   0        0        0     9052 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/attachments/signed_att.py
+-rw-rw-rw-   0        0        0     1162 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/attachments/unsupported_att.py
+-rw-rw-rw-   0        0        0     2442 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/attachments/web_att.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.350087 extract_msg-0.42.2/extract_msg/constants/
+-rw-rw-rw-   0        0        0     5670 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/constants/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/constants/ps.py
+-rw-rw-rw-   0        0        0      874 2023-07-31 13:37:55.000000 extract_msg-0.42.2/extract_msg/constants/re.py
+-rw-rw-rw-   0        0        0     3237 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/constants/st.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.176111 extract_msg-0.42.2/extract_msg/data/
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.356058 extract_msg-0.42.2/extract_msg/data/logging-config/
+-rw-rw-rw-   0        0        0     2082 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/data/logging-config/logging-nt.json
+-rw-rw-rw-   0        0        0     2058 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/data/logging-config/logging-posix.json
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.377029 extract_msg-0.42.2/extract_msg/encoding/
+-rw-rw-rw-   0        0        0    12602 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/encoding/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.411910 extract_msg-0.42.2/extract_msg/encoding/_dt/
+-rw-rw-rw-   0        0        0      116 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/encoding/_dt/__init__.py
+-rw-rw-rw-   0        0        0     2743 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/encoding/_dt/_mac_ce.py
+-rw-rw-rw-   0        0        0     2785 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/encoding/_dt/_mac_cyrillic.py
+-rw-rw-rw-   0        0        0     2721 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/encoding/_dt/_mac_greek.py
+-rw-rw-rw-   0        0        0     2627 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/encoding/_dt/_mac_iceland.py
+-rw-rw-rw-   0        0        0     2628 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/encoding/_dt/_mac_turkish.py
+-rw-rw-rw-   0        0        0     2422 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/encoding/_dt/_win874_dec.py
+-rw-rw-rw-   0        0        0   298022 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/encoding/_dt/_win950_dec.py
+-rw-rw-rw-   0        0        0    12122 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/encoding/utils.py
+-rw-rw-rw-   0        0        0    58987 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/enums.py
+-rw-rw-rw-   0        0        0     4048 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.508650 extract_msg-0.42.2/extract_msg/msg_classes/
+-rw-rw-rw-   0        0        0     1249 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/__init__.py
+-rw-rw-rw-   0        0        0     6722 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/appointment.py
+-rw-rw-rw-   0        0        0     2930 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/calendar.py
+-rw-rw-rw-   0        0        0    19319 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/calendar_base.py
+-rw-rw-rw-   0        0        0    46043 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/contact.py
+-rw-rw-rw-   0        0        0     3590 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/meeting_cancellation.py
+-rw-rw-rw-   0        0        0     1630 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/meeting_exception.py
+-rw-rw-rw-   0        0        0     3737 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/meeting_forward.py
+-rw-rw-rw-   0        0        0     1900 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/meeting_related.py
+-rw-rw-rw-   0        0        0     6577 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/meeting_request.py
+-rw-rw-rw-   0        0        0     2223 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/meeting_response.py
+-rw-rw-rw-   0        0        0      163 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/message.py
+-rw-rw-rw-   0        0        0    55795 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/message_base.py
+-rw-rw-rw-   0        0        0      201 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/message_signed.py
+-rw-rw-rw-   0        0        0     5016 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/message_signed_base.py
+-rw-rw-rw-   0        0        0    37987 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/msg.py
+-rw-rw-rw-   0        0        0     2610 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/post.py
+-rw-rw-rw-   0        0        0     1675 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/sticky_note.py
+-rw-rw-rw-   0        0        0    12686 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/task.py
+-rw-rw-rw-   0        0        0     4017 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/msg_classes/task_request.py
+-rw-rw-rw-   0        0        0    41660 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/ole_writer.py
+-rw-rw-rw-   0        0        0     8558 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/open_msg.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.525604 extract_msg-0.42.2/extract_msg/properties/
+-rw-rw-rw-   0        0        0      549 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/properties/__init__.py
+-rw-rw-rw-   0        0        0    15147 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/properties/named.py
+-rw-rw-rw-   0        0        0     6806 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/properties/prop.py
+-rw-rw-rw-   0        0        0     7627 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/properties/properties_store.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.42.2/extract_msg/py.typed
+-rw-rw-rw-   0        0        0    13687 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/recipient.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.571486 extract_msg-0.42.2/extract_msg/structures/
+-rw-rw-rw-   0        0        0      336 2023-05-09 19:54:43.000000 extract_msg-0.42.2/extract_msg/structures/__init__.py
+-rw-rw-rw-   0        0        0    11737 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/structures/_helpers.py
+-rw-rw-rw-   0        0        0     6682 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/structures/business_card.py
+-rw-rw-rw-   0        0        0    19050 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/structures/entry_id.py
+-rw-rw-rw-   0        0        0     6179 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/structures/misc_id.py
+-rw-rw-rw-   0        0        0     7352 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/structures/recurrence_pattern.py
+-rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.42.2/extract_msg/structures/report_tag.py
+-rw-rw-rw-   0        0        0     1397 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/structures/system_time.py
+-rw-rw-rw-   0        0        0     1616 2023-05-09 19:54:43.000000 extract_msg-0.42.2/extract_msg/structures/time_zone_definition.py
+-rw-rw-rw-   0        0        0     2443 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/structures/time_zone_struct.py
+-rw-rw-rw-   0        0        0     3254 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/structures/tz_rule.py
+-rw-rw-rw-   0        0        0    48405 2023-07-29 23:17:08.000000 extract_msg-0.42.2/extract_msg/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:03:30.287243 extract_msg-0.42.2/extract_msg.egg-info/
+-rw-rw-rw-   0        0        0    12250 2023-08-03 03:03:30.000000 extract_msg-0.42.2/extract_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3136 2023-08-03 03:03:30.000000 extract_msg-0.42.2/extract_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 03:03:30.000000 extract_msg-0.42.2/extract_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-08-03 03:03:30.000000 extract_msg-0.42.2/extract_msg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      270 2023-08-03 03:03:30.000000 extract_msg-0.42.2/extract_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-03 03:03:30.000000 extract_msg-0.42.2/extract_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      193 2023-07-29 23:17:08.000000 extract_msg-0.42.2/requirements.txt
+-rw-rw-rw-   0        0        0      218 2023-08-03 03:03:30.575471 extract_msg-0.42.2/setup.cfg
+-rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.42.2/setup.py
```

### Comparing `extract_msg-0.42.1/CHANGELOG.md` & `extract_msg-0.42.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+**v0.42.2**
+* Fix bug in `AttachmentBase.mimetype` that would cause it to throw an error when accessed. This bug was introduced in `v0.42.0`.
+
 **v0.42.1**
 * Fixed some constants being accessed with the wrong name (names were changed in reorganization).
 * Removed unused regular expression.
 
 **v0.42.0**
 * [[TeamMsgExtractor #372](https://github.com/TeamMsgExtractor/msg-extractor/issues/372)] Changed the way that the save functions return a value. This makes the return value from all save functions much more informative, allowing a user to separate if a file or folder (or if more than one) was saved from the function. It also guarantees that all classes from this module will return the relevant path(s) if data is actually saved.
 * [[TeamMsgExtractor #288](https://github.com/TeamMsgExtractor/msg-extractor/issues/288)] Added feature to allow attachment save functions to simply overwrite existing files of the same name. This can be done with the `overwriteExisting` keyword argument from code or the `--overwrite-existing` option from the command line.
```

### Comparing `extract_msg-0.42.1/LICENSE.txt` & `extract_msg-0.42.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/PKG-INFO` & `extract_msg-0.42.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract_msg
-Version: 0.42.1
+Version: 0.42.2
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
@@ -254,16 +254,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.42.1-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.42.1/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.42.2-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.42.2/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.42.1/README.rst` & `extract_msg-0.42.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -238,16 +238,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.42.1-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.42.1/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.42.2-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.42.2/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.42.1/extract_msg/__init__.py` & `extract_msg-0.42.2/extract_msg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = 'Destiny Peterson & Matthew Walker'
-__date__ = '2023-07-31'
-__version__ = '0.42.1'
+__date__ = '2023-08-02'
+__version__ = '0.42.2'
 
 __all__ = [
     # Modules:
     'attachments',
     'enums',
     'exceptions',
     'msg_classes',
```

### Comparing `extract_msg-0.42.1/extract_msg/__main__.py` & `extract_msg-0.42.2/extract_msg/__main__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/_rtf/create_doc.py` & `extract_msg-0.42.2/extract_msg/_rtf/create_doc.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/_rtf/inject_rtf.py` & `extract_msg-0.42.2/extract_msg/_rtf/inject_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/_rtf/token.py` & `extract_msg-0.42.2/extract_msg/_rtf/token.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/_rtf/tokenize_rtf.py` & `extract_msg-0.42.2/extract_msg/_rtf/tokenize_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/attachments/__init__.py` & `extract_msg-0.42.2/extract_msg/attachments/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/attachments/attachment.py` & `extract_msg-0.42.2/extract_msg/attachments/attachment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/attachments/attachment_base.py` & `extract_msg-0.42.2/extract_msg/attachments/attachment_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,15 +502,15 @@
         return self._getStringStream('__substg1.0_370D')
 
     @functools.cached_property
     def mimetype(self) -> Optional[str]:
         """
         The content-type mime header of the attachment, if specified.
         """
-        return self._getStreamAs('__substg1.0_370E', partial(tryGetMimetype, self), False)
+        return tryGetMimetype(self, self._getStringStream('__substg1.0_370E'))
 
     @property
     def msg(self) -> MSGFile:
         """
         Returns the Message instance the attachment belongs to.
 
         :raises ReferenceError: The associated MSGFile instance has been garbage
```

### Comparing `extract_msg-0.42.1/extract_msg/attachments/broken_att.py` & `extract_msg-0.42.2/extract_msg/attachments/broken_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/attachments/custom_att.py` & `extract_msg-0.42.2/extract_msg/attachments/custom_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/attachments/custom_att_handler/__init__.py` & `extract_msg-0.42.2/extract_msg/attachments/custom_att_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/attachments/custom_att_handler/custom_handler.py` & `extract_msg-0.42.2/extract_msg/attachments/custom_att_handler/custom_handler.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/attachments/custom_att_handler/outlook_image_dib.py` & `extract_msg-0.42.2/extract_msg/attachments/custom_att_handler/outlook_image_dib.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/attachments/emb_msg_att.py` & `extract_msg-0.42.2/extract_msg/attachments/emb_msg_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/attachments/signed_att.py` & `extract_msg-0.42.2/extract_msg/attachments/signed_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/attachments/unsupported_att.py` & `extract_msg-0.42.2/extract_msg/attachments/unsupported_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/attachments/web_att.py` & `extract_msg-0.42.2/extract_msg/attachments/web_att.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/constants/__init__.py` & `extract_msg-0.42.2/extract_msg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/constants/ps.py` & `extract_msg-0.42.2/extract_msg/constants/ps.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/constants/re.py` & `extract_msg-0.42.2/extract_msg/constants/re.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/constants/st.py` & `extract_msg-0.42.2/extract_msg/constants/st.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/data/logging-config/logging-nt.json` & `extract_msg-0.42.2/extract_msg/data/logging-config/logging-nt.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/data/logging-config/logging-posix.json` & `extract_msg-0.42.2/extract_msg/data/logging-config/logging-posix.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/encoding/__init__.py` & `extract_msg-0.42.2/extract_msg/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/encoding/_dt/_mac_ce.py` & `extract_msg-0.42.2/extract_msg/encoding/_dt/_mac_ce.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/encoding/_dt/_mac_cyrillic.py` & `extract_msg-0.42.2/extract_msg/encoding/_dt/_mac_cyrillic.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/encoding/_dt/_mac_greek.py` & `extract_msg-0.42.2/extract_msg/encoding/_dt/_mac_greek.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/encoding/_dt/_mac_iceland.py` & `extract_msg-0.42.2/extract_msg/encoding/_dt/_mac_iceland.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/encoding/_dt/_mac_turkish.py` & `extract_msg-0.42.2/extract_msg/encoding/_dt/_mac_turkish.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/encoding/_dt/_win874_dec.py` & `extract_msg-0.42.2/extract_msg/encoding/_dt/_win874_dec.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/encoding/_dt/_win950_dec.py` & `extract_msg-0.42.2/extract_msg/encoding/_dt/_win950_dec.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/encoding/utils.py` & `extract_msg-0.42.2/extract_msg/encoding/utils.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/enums.py` & `extract_msg-0.42.2/extract_msg/enums.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/exceptions.py` & `extract_msg-0.42.2/extract_msg/exceptions.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/__init__.py` & `extract_msg-0.42.2/extract_msg/msg_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/appointment.py` & `extract_msg-0.42.2/extract_msg/msg_classes/appointment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/calendar.py` & `extract_msg-0.42.2/extract_msg/msg_classes/calendar.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/calendar_base.py` & `extract_msg-0.42.2/extract_msg/msg_classes/calendar_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/contact.py` & `extract_msg-0.42.2/extract_msg/msg_classes/contact.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/meeting_cancellation.py` & `extract_msg-0.42.2/extract_msg/msg_classes/meeting_cancellation.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/meeting_exception.py` & `extract_msg-0.42.2/extract_msg/msg_classes/meeting_exception.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/meeting_forward.py` & `extract_msg-0.42.2/extract_msg/msg_classes/meeting_forward.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/meeting_related.py` & `extract_msg-0.42.2/extract_msg/msg_classes/meeting_related.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/meeting_request.py` & `extract_msg-0.42.2/extract_msg/msg_classes/meeting_request.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/meeting_response.py` & `extract_msg-0.42.2/extract_msg/msg_classes/meeting_response.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/message_base.py` & `extract_msg-0.42.2/extract_msg/msg_classes/message_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/message_signed_base.py` & `extract_msg-0.42.2/extract_msg/msg_classes/message_signed_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/msg.py` & `extract_msg-0.42.2/extract_msg/msg_classes/msg.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/post.py` & `extract_msg-0.42.2/extract_msg/msg_classes/post.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/sticky_note.py` & `extract_msg-0.42.2/extract_msg/msg_classes/sticky_note.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/task.py` & `extract_msg-0.42.2/extract_msg/msg_classes/task.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/msg_classes/task_request.py` & `extract_msg-0.42.2/extract_msg/msg_classes/task_request.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/ole_writer.py` & `extract_msg-0.42.2/extract_msg/ole_writer.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/open_msg.py` & `extract_msg-0.42.2/extract_msg/open_msg.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/properties/__init__.py` & `extract_msg-0.42.2/extract_msg/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/properties/named.py` & `extract_msg-0.42.2/extract_msg/properties/named.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/properties/prop.py` & `extract_msg-0.42.2/extract_msg/properties/prop.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/properties/properties_store.py` & `extract_msg-0.42.2/extract_msg/properties/properties_store.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/recipient.py` & `extract_msg-0.42.2/extract_msg/recipient.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/structures/_helpers.py` & `extract_msg-0.42.2/extract_msg/structures/_helpers.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/structures/business_card.py` & `extract_msg-0.42.2/extract_msg/structures/business_card.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/structures/entry_id.py` & `extract_msg-0.42.2/extract_msg/structures/entry_id.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/structures/misc_id.py` & `extract_msg-0.42.2/extract_msg/structures/misc_id.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/structures/recurrence_pattern.py` & `extract_msg-0.42.2/extract_msg/structures/recurrence_pattern.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/structures/report_tag.py` & `extract_msg-0.42.2/extract_msg/structures/report_tag.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/structures/system_time.py` & `extract_msg-0.42.2/extract_msg/structures/system_time.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/structures/time_zone_definition.py` & `extract_msg-0.42.2/extract_msg/structures/time_zone_definition.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/structures/time_zone_struct.py` & `extract_msg-0.42.2/extract_msg/structures/time_zone_struct.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/structures/tz_rule.py` & `extract_msg-0.42.2/extract_msg/structures/tz_rule.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg/utils.py` & `extract_msg-0.42.2/extract_msg/utils.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/extract_msg.egg-info/PKG-INFO` & `extract_msg-0.42.2/extract_msg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract-msg
-Version: 0.42.1
+Version: 0.42.2
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
@@ -254,16 +254,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.42.1-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.42.1/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.42.2-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.42.2/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.42.1/extract_msg.egg-info/SOURCES.txt` & `extract_msg-0.42.2/extract_msg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `extract_msg-0.42.1/setup.py` & `extract_msg-0.42.2/setup.py`

 * *Files identical despite different names*

