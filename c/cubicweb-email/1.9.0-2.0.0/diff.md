# Comparing `tmp/cubicweb-email-1.9.0.tar.gz` & `tmp/cubicweb-email-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-email-1.9.0.tar", last modified: Sat Nov 17 22:38:28 2012, max compression, from Unix
+gzip compressed data, was "cubicweb-email-2.0.0.tar", last modified: Thu Aug  3 15:12:50 2023, max compression
```

## Comparing `cubicweb-email-1.9.0.tar` & `cubicweb-email-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,57 @@
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2012-11-17 22:38:28.000000 cubicweb-email-1.9.0/
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2012-11-17 22:38:28.000000 cubicweb-email-1.9.0/test/
--rw-------   0 narval     (105) narval     (109)      382 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/test/test_email.py
--rw-------   0 narval     (105) narval     (109)    10004 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/mboximport.py
--rw-------   0 narval     (105) narval     (109)      190 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/README
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2012-11-17 22:38:28.000000 cubicweb-email-1.9.0/views/
--rw-------   0 narval     (105) narval     (109)     6899 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/views/email.py
--rw-------   0 narval     (105) narval     (109)      996 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/views/__init__.py
--rw-rw-r--   0 narval     (105) narval     (109)      485 2012-11-17 22:38:28.000000 cubicweb-email-1.9.0/PKG-INFO
--rw-------   0 narval     (105) narval     (109)     2831 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/schema.py
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2012-11-17 22:38:28.000000 cubicweb-email-1.9.0/migration/
--rw-------   0 narval     (105) narval     (109)       66 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/migration/postcreate.py
--rw-------   0 narval     (105) narval     (109)       86 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/migration/1.4.1_Any.py
--rw-------   0 narval     (105) narval     (109)       74 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/migration/1.1.1_Any.py
--rw-------   0 narval     (105) narval     (109)       29 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/migration/1.2.2_Any.py
--rw-------   0 narval     (105) narval     (109)       71 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/migration/1.1.0_Any.py
--rw-------   0 narval     (105) narval     (109)     4102 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/hooks.py
--rw-------   0 narval     (105) narval     (109)     4438 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/emailcites.py
--rw-------   0 narval     (105) narval     (109)      269 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/__init__.py
--rw-------   0 narval     (105) narval     (109)     4623 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/entities.py
--rw-------   0 narval     (105) narval     (109)     1664 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/__pkginfo__.py
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2012-11-17 22:38:28.000000 cubicweb-email-1.9.0/i18n/
--rw-------   0 narval     (105) narval     (109)     4940 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/i18n/en.po
--rw-------   0 narval     (105) narval     (109)     5518 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/i18n/fr.po
--rw-------   0 narval     (105) narval     (109)     3008 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/ccplugin.py
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2012-11-17 22:38:28.000000 cubicweb-email-1.9.0/doc/
--rw-------   0 narval     (105) narval     (109)     1324 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/doc/email.txt
--rw-------   0 narval     (105) narval     (109)     3255 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/doc/email.html
--rw-------   0 narval     (105) narval     (109)     5488 2012-11-17 22:30:38.000000 cubicweb-email-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.793972 cubicweb-email-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      890 2023-08-03 15:12:50.793972 cubicweb-email-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.765971 cubicweb-email-2.0.0/bin/
+-rwxrwxrwx   0 root         (0) root         (0)       62 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/bin/cw-mboximport
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.769971 cubicweb-email-2.0.0/cubicweb_email/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      707 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4488 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/emailcites.py
+-rw-rw-rw-   0 root         (0) root         (0)     4592 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     8799 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.777972 cubicweb-email-2.0.0/cubicweb_email/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     4942 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     5518 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.781972 cubicweb-email-2.0.0/cubicweb_email/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/migration/1.1.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/migration/1.1.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/migration/1.11.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/migration/1.2.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/migration/1.4.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2928 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/testutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.785972 cubicweb-email-2.0.0/cubicweb_email/views/
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6959 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cubicweb_email/views/email.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.777972 cubicweb-email-2.0.0/cubicweb_email.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      890 2023-08-03 15:12:50.000000 cubicweb-email-2.0.0/cubicweb_email.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-08-03 15:12:50.000000 cubicweb-email-2.0.0/cubicweb_email.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 15:12:50.000000 cubicweb-email-2.0.0/cubicweb_email.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-08-03 15:12:50.000000 cubicweb-email-2.0.0/cubicweb_email.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 15:12:50.000000 cubicweb-email-2.0.0/cubicweb_email.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       97 2023-08-03 15:12:50.000000 cubicweb-email-2.0.0/cubicweb_email.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-03 15:12:50.000000 cubicweb-email-2.0.0/cubicweb_email.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.785972 cubicweb-email-2.0.0/cwemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cwemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6518 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/cwemail/mboximport.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-03 15:12:50.793972 cubicweb-email-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2617 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.789972 cubicweb-email-2.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.789972 cubicweb-email-2.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.757971 cubicweb-email-2.0.0/test/data/maildir/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:12:50.793972 cubicweb-email-2.0.0/test/data/maildir/cur/
+-rw-rw-rw-   0 root         (0) root         (0)     6056 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test/data/maildir/cur/1366704331.6558_1.orion:2,S
+-rw-rw-rw-   0 root         (0) root         (0)    16968 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test/data/maildir/cur/1366704331.6558_3.orion:2,S
+-rw-rw-rw-   0 root         (0) root         (0)    23194 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test/data/mbox
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test/data/reply.mbox
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test/test_email.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test/unittest_emailcites.py
+-rw-rw-rw-   0 root         (0) root         (0)     9516 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10868 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test/unittest_mboximport.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/test-requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2023-08-03 15:12:17.000000 cubicweb-email-2.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-email-1.9.0/views/email.py` & `cubicweb-email-2.0.0/cubicweb_email/views/email.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,171 +1,203 @@
 """Specific views for email related entities
 
 :organization: Logilab
-:copyright: 2003-2010 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+:copyright: 2003-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
-_ = unicode
+
+from cubicweb import _
 
 from logilab.mtconverter import xml_escape
 
-from cubicweb.selectors import is_instance
+from cubicweb.predicates import is_instance
 from cubicweb.uilib import soup2xhtml
-from cubicweb.view import EntityView
-from cubicweb.web import uicfg, formwidgets
-from cubicweb.web.views import baseviews, primary
-
-for rtype in ('sender', 'recipients', 'cc', 'parts'):
-    uicfg.primaryview_section.tag_subject_of(('Email', rtype, '*'), 'hidden')
-
-uicfg.autoform_field_kwargs.tag_attribute(('Email', 'subject'),
-                                          {'widget': formwidgets.TextInput})
-
-uicfg.actionbox_appearsin_addmenu.tag_subject_of(('Email', 'attachment', '*'),
-                                                 True)
-
-uicfg.actionbox_appearsin_addmenu.tag_object_of(('EmailThread', 'forked_from', 'EmailThread'),
-                                                True)
+from cubicweb_web.view import EntityView
+from cubicweb_web import formwidgets
+from cubicweb_web.views import baseviews, primary, uicfg
+
+for rtype in ("sender", "recipients", "cc", "parts"):
+    uicfg.primaryview_section.tag_subject_of(("Email", rtype, "*"), "hidden")
+
+uicfg.autoform_field_kwargs.tag_attribute(
+    ("Email", "subject"), {"widget": formwidgets.TextInput}
+)
+
+uicfg.actionbox_appearsin_addmenu.tag_subject_of(("Email", "attachment", "*"), True)
+
+uicfg.actionbox_appearsin_addmenu.tag_object_of(
+    ("EmailThread", "forked_from", "EmailThread"), True
+)
 
 
 def formated_sender(email):
     if email.sender:
-        return email.sender[0].view('oneline')
+        return email.sender[0].view("oneline")
     # sender address has been removed, look in email's headers
     message = email.umessage_headers()
     if message:
-        return xml_escape(message.get('From', ''))
-    return email._cw._('unknown sender')
+        return xml_escape(message.get("From", ""))
+    return email._cw._("unknown sender")
+
 
 class EmailPrimaryView(primary.PrimaryView):
-    __select__ = is_instance('Email')
+    __select__ = is_instance("Email")
 
     def render_entity_attributes(self, entity):
-        self.w(u'<div class="emailheader"><table>')
-        self.w(u'<tr><td>%s</td><td>%s</td></tr>' %
-               (self._cw._('From'), formated_sender(entity)))
-        self.w(u'<tr><td>%s</td><td>%s</td></tr>' %
-               (self._cw._('To'), ', '.join(ea.view('oneline') for ea in entity.recipients)))
+        self.w('<div class="emailheader"><table>')
+        self.w(
+            f"<tr><td>{self._cw._('From')}</td><td>{formated_sender(entity)}</td></tr>"
+        )
+        self.w(
+            "<tr><td>%s</td><td>%s</td></tr>"
+            % (
+                self._cw._("To"),
+                ", ".join(ea.view("oneline") for ea in entity.recipients),
+            )
+        )
         if entity.cc:
-            self.w(u'<tr><td>%s</td><td>%s</td></tr>' %
-                   (self._cw._('CC'), ', '.join(ea.view('oneline') for ea in entity.cc)))
-        self.w(u'<tr><td>%s</td><td>%s</td></tr>' %
-               (self._cw._('Date'), self._cw.format_date(entity.date, time=True)))
-        self.w(u'<tr><td>%s</td><td>%s</td></tr>' %
-               (self._cw._('Subject'), xml_escape(entity.subject)))
-        self.w(u'</table></div><div class="emailcontent">')
+            self.w(
+                "<tr><td>%s</td><td>%s</td></tr>"
+                % (self._cw._("CC"), ", ".join(ea.view("oneline") for ea in entity.cc))
+            )
+        self.w(
+            "<tr><td>%s</td><td>%s</td></tr>"
+            % (self._cw._("Date"), self._cw.format_date(entity.date, time=True))
+        )
+        self.w(
+            "<tr><td>%s</td><td>%s</td></tr>"
+            % (self._cw._("Subject"), xml_escape(entity.subject))
+        )
+        self.w('</table></div><div class="emailcontent">')
         for part in entity.parts_in_order():
             content, mime = part.content, part.content_format
-            if mime == 'text/html':
+            if mime == "text/html":
                 content = soup2xhtml(content, self._cw.encoding)
-            elif 'pgp-signature' in mime:
-                content = entity._cw_mtc_transform(content, mime, 'text/html', self._cw.encoding)
-            elif mime != 'text/xhtml':
+            elif "pgp-signature" in mime:
+                content = entity._cw_mtc_transform(
+                    content, mime, "text/html", self._cw.encoding
+                )
+            elif mime != "text/xhtml":
                 content = xml_escape(content)
-                if mime == 'text/plain':
-                    content = content.replace('\n', '<br/>').replace(' ', '&nbsp;')
+                if mime == "text/plain":
+                    content = content.replace("\n", "<br/>").replace(" ", "&nbsp;")
             # XXX some headers to skip if html ?
             self.w(content)
-            self.w(u'<br class="partseparator"/>')
-        self.w(u'</div>')
+            self.w('<br class="partseparator"/>')
+        self.w("</div>")
 
     def render_entity_title(self, entity):
-        self.w(u'<h1><span class="etype">%s</span> %s</h1>'
-               % (entity.dc_type().capitalize(), xml_escape(entity.dc_title())))
+        self.w(
+            '<h1><span class="etype">%s</span> %s</h1>'
+            % (entity.dc_type().capitalize(), xml_escape(entity.dc_title()))
+        )
 
 
 class EmailHeadersView(baseviews.EntityView):
     """display email's headers"""
-    __regid__ = 'headers'
-    __select__ = is_instance('Email')
-    title = _('headers')
+
+    __regid__ = "headers"
+    __select__ = is_instance("Email")
+    title = _("headers")
     templatable = False
-    content_type = 'text/plain'
+    content_type = "text/plain"
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
         self.w(entity.headers)
 
 
 class EmailOneLineView(baseviews.OneLineView):
     """short view usable in the context of the email sender/recipient (in which
     case the caller should specify its context eid) or outside any context
     """
-    __select__ = is_instance('Email')
-    title = _('oneline')
+
+    __select__ = is_instance("Email")
+    title = _("oneline")
 
     def cell_call(self, row, col, contexteid=None):
         entity = self.cw_rset.get_entity(row, col)
-        self.w(u'<div class="email">')
-        self.w(u'<i>%s&nbsp;%s</i> ' % (
-            self._cw._('email_date'), self._cw.format_date(entity.date, time=True)))
+        self.w('<div class="email">')
+        self.w(
+            "<i>{}&nbsp;{}</i> ".format(
+                self._cw._("email_date"), self._cw.format_date(entity.date, time=True)
+            )
+        )
         sender = entity.senderaddr
         if sender is None or contexteid != sender.eid:
-            self.w(u'<b>%s</b>&nbsp;%s '
-                   % (self._cw._('email_from'), formated_sender(entity)))
+            self.w(f"<b>{self._cw._('email_from')}</b>&nbsp;{formated_sender(entity)} ")
         if contexteid not in (r.eid for r in entity.recipients):
-            recipients = ', '.join(r.view('oneline') for r in entity.recipients)
-            self.w(u'<b>%s</b>&nbsp;%s'
-                   % (self._cw._('email_to'), recipients))
-        self.w(u'<br/>\n<a href="%s">%s</a>' % (
-            xml_escape(entity.absolute_url()), xml_escape(entity.subject)))
-        self.w(u'</div>')
+            recipients = ", ".join(r.view("oneline") for r in entity.recipients)
+            self.w(f"<b>{self._cw._('email_to')}</b>&nbsp;{recipients}")
+        self.w(
+            '<br/>\n<a href="{}">{}</a>'.format(
+                xml_escape(entity.absolute_url()), xml_escape(entity.subject)
+            )
+        )
+        self.w("</div>")
 
 
 class EmailOutOfContextView(EmailOneLineView):
     """short view outside the context of the email"""
-    __regid__ = 'outofcontext'
-    title = _('out of context')
+
+    __regid__ = "outofcontext"
+    title = _("out of context")
 
 
 class EmailInContextView(EmailOneLineView):
     """short view inside the context of the email"""
-    __regid__ = 'incontext'
+
+    __regid__ = "incontext"
+
 
 class EmailTreeItemView(EmailOutOfContextView):
-    __regid__ = 'treeitem'
+    __regid__ = "treeitem"
     title = None
 
+
 class EmailPartOutOfContextView(baseviews.OutOfContextView):
     """out of context an email part is redirecting to related email view"""
-    __select__ = is_instance('EmailPart')
+
+    __select__ = is_instance("EmailPart")
+
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
-        entity.reverse_parts[0].view('outofcontext', w=self.w)
+        entity.reverse_parts[0].view("outofcontext", w=self.w)
 
 
 class EmailThreadView(EntityView):
-    __regid__ = 'emailthread'
-    __select__ = is_instance('EmailThread')
+    __regid__ = "emailthread"
+    __select__ = is_instance("EmailThread")
 
     def entity_call(self, entity):
         # get top level emails in this thread (ie message which are not a reply
         # of a message in this thread)
         #
         # Warn: adding Y in_thread E changes the meaning of the query since it joins
         # with messages which are not a direct reply (eg if A reply_to B, B reply_to C
         # B is also retreived since it's not a reply of C
         #
         # XXX  union with
         #   DISTINCT Any X,D ORDERBY D WHERE X date D, X in_thread E, X reply_to Y,
         #   NOT Y in_thread E, E eid %(x)s'
         # to get message which are a reply of a message in another thread ?
         # we may get duplicates in this case
-        rset =  self._cw.execute('DISTINCT Any X,D ORDERBY D '
-                                 'WHERE X date D, X in_thread E, '
-                                 'NOT X reply_to Y, E eid %(x)s',
-                                 {'x': entity.eid})
+        rset = self._cw.execute(
+            "DISTINCT Any X,D ORDERBY D "
+            "WHERE X date D, X in_thread E, "
+            "NOT X reply_to Y, E eid %(x)s",
+            {"x": entity.eid},
+        )
         if rset:
-            self.w(u'<ul>')
-            self.w(u'\n'.join(email.view('tree') for email in rset.entities()))
-            self.w(u'</ul>')
+            self.w("<ul>")
+            self.w("\n".join(email.view("tree") for email in rset.entities()))
+            self.w("</ul>")
 
 
 class EmailThreadPrimaryView(primary.PrimaryView):
-    __select__ = is_instance('EmailThread')
+    __select__ = is_instance("EmailThread")
 
     def cell_call(self, row, col):
         entity = self.cw_rset.complete_entity(row, col)
-        self.w(u'<h1>%s</h1>' % xml_escape(entity.title))
-        entity.view('emailthread', w=self.w)
-
+        self.w(f"<h1>{xml_escape(entity.title)}</h1>")
+        entity.view("emailthread", w=self.w)
```

### Comparing `cubicweb-email-1.9.0/schema.py` & `cubicweb-email-2.0.0/cubicweb_email/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,120 @@
 """entity/relation schemas to store email in an cubicweb instance
 
 :organization: Logilab
-:copyright: 2006-2010 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+:copyright: 2006-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
-_ = unicode
+
+from cubicweb import _
+
 
 # pylint: disable-msg=E0611,F0401
-from yams.buildobjs import (SubjectRelation, RelationType, EntityType,
-                            String, Datetime, Int, RelationDefinition)
+from yams.buildobjs import (
+    SubjectRelation,
+    RelationType,
+    EntityType,
+    String,
+    Datetime,
+    Int,
+    RelationDefinition,
+)
 from yams.reader import context
 
 from cubicweb.schema import ERQLExpression
 
 
 class Email(EntityType):
     """electronic mail"""
-    subject   = String(fulltextindexed=True)
-    date      = Datetime(description=_('UTC time on which the mail was sent'))
-    messageid = String(required=True, indexed=True)
-    headers   = String(description=_('raw headers'))
 
-    sender     = SubjectRelation('EmailAddress', cardinality='?*')
+    subject = String(fulltextindexed=True)
+    date = Datetime(description=_("UTC time on which the mail was sent"))
+    messageid = String(required=True, indexed=True, unique=True)
+    headers = String(description=_("raw headers"))
+
+    sender = SubjectRelation("EmailAddress", cardinality="?*")
     # an email with only Bcc is acceptable, don't require any recipients
-    recipients = SubjectRelation('EmailAddress')
-    cc         = SubjectRelation('EmailAddress')
+    recipients = SubjectRelation("EmailAddress")
+    cc = SubjectRelation("EmailAddress")
 
-    parts       = SubjectRelation('EmailPart', cardinality='*1', composite='subject')
-    attachment  = SubjectRelation('File')
+    parts = SubjectRelation("EmailPart", cardinality="*1", composite="subject")
+    attachment = SubjectRelation("File")
 
-    reply_to    = SubjectRelation('Email', cardinality='?*')
-    cites       = SubjectRelation('Email')
-    in_thread   = SubjectRelation('EmailThread', cardinality='?*')
+    reply_to = SubjectRelation("Email", cardinality="?*")
+    cites = SubjectRelation("Email")
+    in_thread = SubjectRelation("EmailThread", cardinality="?*")
 
 
 class EmailPart(EntityType):
     """an email attachment"""
+
     __permissions__ = {
-        'read':   ('managers', 'users', 'guests',), # XXX if E parts X, U has_read_permission E
-        'add':    ('managers', ERQLExpression('E parts X, U has_update_permission E'),),
-        'delete': ('managers', ERQLExpression('E parts X, U has_update_permission E')),
-        'update': ('managers', 'owners',),
-        }
+        "read": (
+            "managers",
+            "users",
+            "guests",
+        ),  # XXX if E parts X, U has_read_permission E
+        "add": (
+            "managers",
+            ERQLExpression("E parts X, U has_update_permission E"),
+        ),
+        "delete": ("managers", ERQLExpression("E parts X, U has_update_permission E")),
+        "update": (
+            "managers",
+            "owners",
+        ),
+    }
 
-    content  = String(fulltextindexed=True)
-    content_format = String(required=True, meta=True, maxsize=50)
+    content = String(fulltextindexed=True)
+    content_format = String(required=True, maxsize=50)
     ordernum = Int(required=True)
-    alternative = SubjectRelation('EmailPart', symmetric=True)
+    alternative = SubjectRelation("EmailPart", symmetric=True)
 
 
 class EmailThread(EntityType):
     """discussion thread"""
+
     title = String(required=True, indexed=True, fulltextindexed=True)
-    see_also = SubjectRelation('EmailThread')
-    forked_from = SubjectRelation('EmailThread', cardinality='?*')
+    see_also = SubjectRelation("EmailThread")
+    forked_from = SubjectRelation("EmailThread", cardinality="?*")
+
 
 class parts(RelationType):
     """ """
-    fulltext_container = 'subject'
+
+    fulltext_container = "subject"
+
 
 class sender(RelationType):
     """ """
+
     inlined = True
 
+
 class in_thread(RelationType):
     """ """
+
     inlined = True
 
+
 class reply_to(RelationType):
     """ """
+
     inlined = True
 
+
 class generated_by(RelationType):
     """mark an entity as generated from an email"""
-    cardinality = '?*'
-    subject = ('TrInfo',)
-    object = 'Email'
 
-# if comment is installed
-if 'Comment' in context.defined:
-    class comment_generated_by(RelationDefinition):
-        subject = 'Comment'
-        name = 'generated_by'
-        object = 'Email'
+    cardinality = "?*"
+    subject = ("TrInfo",)
+    object = "Email"
+
 
+# if comment is installed
+if "Comment" in context.defined:
 
+    class comment_generated_by(RelationDefinition):
+        subject = "Comment"
+        name = "generated_by"
+        object = "Email"
```

### Comparing `cubicweb-email-1.9.0/emailcites.py` & `cubicweb-email-2.0.0/cubicweb_email/emailcites.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,73 @@
 """some utilities to process email information
 
 :organization: Logilab
-:copyright: 2007-2008 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+:copyright: 2007-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
 
-def parse_body(body, quote='>'):
+def parse_body(body, quote=">"):
     """return a `ParsedMessage` instance where actual content is separated from
     cited content
     """
     res = []
     level = 0
     current = []
     seenlevels = set()
     for line in body.splitlines(True):
         newlevel = 0
         while line.startswith(quote):
             newlevel += 1
             line = line[1:].lstrip()
-        if line.strip() == '--':
-            break # ignore following signature
+        if line.strip() == "--":
+            break  # ignore following signature
         if newlevel != level:
             # detect lines such as
             #   On Wed, Jan 23, 2008 at 06:48:22PM +0100, machin wrote:
             # preceding citation
-            if not newlevel in seenlevels and res and res[-1][1] and \
-                   res[-1][1][-1].rstrip().endswith(':'):
+            if (
+                newlevel not in seenlevels
+                and res
+                and res[-1][1]
+                and res[-1][1][-1].rstrip().endswith(":")
+            ):
                 current.insert(0, res[-1][1].pop())
             seenlevels.add(newlevel)
-            res.append( (level, current) )
+            res.append((level, current))
             current = []
         level = newlevel
         current.append(line)
-    res.append( (level, current) )
+    res.append((level, current))
     pmsg = ParsedMessage()
     for level, lines in res:
-        para = ''.join(lines).strip()
+        para = "".join(lines).strip()
         if not para:
             continue
-        if level > 0 :
+        if level > 0:
             pmsg.cites.append(para)
         else:
             pmsg.content.append(para)
     return pmsg
 
-class ParsedMessage(object):
+
+class ParsedMessage:
     def __init__(self):
         self.content = []
         self.cites = []
 
     @property
     def actual_content(self):
-        return '\n'.join(self.content)
+        return "\n".join(self.content)
+
     @property
     def cited_content(self):
-        return '\n'.join(self.cites)
+        return "\n".join(self.cites)
+
 
 # import sys
 # from mailbox import UnixMailbox
 # from maboa.umessage import message_from_file
 # from cubicweb.web.uilib import remove_html_tags
 
 # def ignore_cite(para):
```

### Comparing `cubicweb-email-1.9.0/entities.py` & `cubicweb-email-2.0.0/cubicweb_email/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """entity classes for entity types provided by the cubicweb email package
 
 :organization: Logilab
-:copyright: 2003-2010 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+:copyright: 2003-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
 import re
 
 from logilab.common import umessage
 
 from cubicweb.entities import AnyEntity, fetch_config, adapters
-from cubicweb.selectors import is_instance
-from cubes.email.emailcites import parse_body
+from cubicweb.predicates import is_instance
+
+from cubicweb_email.emailcites import parse_body
 
 
 class Email(AnyEntity):
     """customized class for Email entities"""
-    __regid__ = 'Email'
-    fetch_attrs, fetch_order = fetch_config(['subject'])
+
+    __regid__ = "Email"
+    fetch_attrs, cw_fetch_order = fetch_config(["subject"])
 
     def dc_title(self):
         return self.subject
 
     @property
     def senderaddr(self):
         return self.sender and self.sender[0] or None
@@ -31,77 +33,78 @@
     def in_reply_to(self):
         return self.reply_to and self.reply_to[0] or None
 
     @property
     def thread(self):
         return self.in_thread and self.in_thread[0] or None
 
-    def parts_in_order(self, prefered_mime_type='text/html'):
+    def parts_in_order(self, prefered_mime_type="text/html"):
         """sort an email parts in order, selecting among alternatives according to a
         prefered mime type
         """
         parts_by_eid = {}
         alternatives = []
         result = []
         for part in self.parts:
             parts_by_eid[part.eid] = part
             if part.alternative:
                 for altset in alternatives:
                     if part.eid in altset:
                         break
                 else:
-                    alternatives.append(set(p.eid for p in part.alternative))
+                    alternatives.append({p.eid for p in part.alternative})
                     alternatives[-1].add(part.eid)
             else:
                 result.append(part)
         if alternatives:
             for altset in alternatives:
-                selected = [parts_by_eid[peid] for peid in altset
-                            if parts_by_eid[peid].content_format == prefered_mime_type]
+                selected = [
+                    parts_by_eid[peid]
+                    for peid in altset
+                    if parts_by_eid[peid].content_format == prefered_mime_type
+                ]
                 if selected:
                     selected = selected[0]
                 else:
                     selected = parts_by_eid[altset.pop()]
                 result.append(selected)
         return sorted(result, key=lambda x: x.ordernum)
 
     def references(self):
         result = set()
         message = self.umessage_headers()
         if not message:
             return result
-        replyto = message.get('In-reply-to')
+        replyto = message.get("In-reply-to")
         if replyto:
             result.add(replyto)
-        for refs in message.get_all('References', ()):
+        for refs in message.get_all("References", ()):
             result.update(refs.split())
         return result
 
-    lines_rgx = re.compile('^Lines:\s*\d+\s*\n', re.I|re.U|re.M)
-    clength_rgx = re.compile('^Content-Length:\s*\d+\s*\n', re.I|re.U|re.M)
-    ctype_rgx = re.compile('^Content-Type:[^:]', re.I|re.U|re.M)
+    lines_rgx = re.compile(r"^Lines:\s*\d+\s*\n", re.I | re.U | re.M)
+    clength_rgx = re.compile(r"^Content-Length:\s*\d+\s*\n", re.I | re.U | re.M)
+    ctype_rgx = re.compile(r"^Content-Type:[^:]", re.I | re.U | re.M)
 
     def umessage_headers(self):
         if not self.headers:
             return None
-        headers = self.lines_rgx.sub('', self.headers)
-        headers = self.clength_rgx.sub('', headers)
-        headers = self.ctype_rgx.sub('Content-type: text/plain; charset=utf8', headers)
-        headers = headers.encode('utf8')
-        return umessage.message_from_string(headers + '\n\n')
-
+        headers = self.lines_rgx.sub("", self.headers)
+        headers = self.clength_rgx.sub("", headers)
+        headers = self.ctype_rgx.sub("Content-type: text/plain; charset=utf8", headers)
+        return umessage.message_from_string(headers + "\n\n")
 
 
 class EmailPart(AnyEntity):
     """customized class for EmailPart entities"""
-    __regid__ = 'EmailPart'
+
+    __regid__ = "EmailPart"
 
     def dc_title(self):
-        return '%s (%s %s)' % (self.email.subject,
-                               self._cw._('part'), self.ordernum)
+        return f"{self.email.subject} ({self._cw._('part')} {self.ordernum})"
 
     @property
     def email(self):
         return self.reverse_parts[0]
 
     def parent(self):
         """for breadcrumbs"""
@@ -109,36 +112,37 @@
 
     def actual_content(self):
         """return content of this part with citations and signature removed
 
         this method may raise `TransformError` exception if the part can't
         be displayed as text/plain.
         """
-        content = self.printable_value('content', format='text/plain')
+        content = self.printable_value("content", format="text/plain")
         return parse_body(content).actual_content
 
 
 class EmailThread(AnyEntity):
     """customized class for EmailThread entities"""
-    __regid__ = 'EmailThread'
-    fetch_attrs, fetch_order = fetch_config(['title'])
+
+    __regid__ = "EmailThread"
+    fetch_attrs, cw_fetch_order = fetch_config(["title"])
 
     def dc_title(self):
         return self.title
 
 
 class EmailITreeAdapter(adapters.ITreeAdapter):
-    __select__ = is_instance('Email')
-    tree_relation = 'reply_to'
+    __select__ = is_instance("Email")
+    tree_relation = "reply_to"
 
 
 class EmailPartIFTIAdapter(adapters.IFTIndexableAdapter):
     """customize EmailPart IFTI adapter so we don't index pgp signature"""
-    __select__ = adapters.IFTIndexableAdapter.__select__ & is_instance('EmailPart')
+
+    __select__ = adapters.IFTIndexableAdapter.__select__ & is_instance("EmailPart")
 
     def get_words(self):
         try:
-            if self.entity.contenttype == 'application/pgp-signature':
+            if self.entity.contenttype == "application/pgp-signature":
                 return []
         except AttributeError:
-            return super(EmailPartIFTIAdapter, self).get_words()
-
+            return super().get_words()
```

### Comparing `cubicweb-email-1.9.0/i18n/en.po` & `cubicweb-email-2.0.0/cubicweb_email/i18n/en.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # cubicweb-email i18n catalog
-# Copyright 2003-2008 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# Copyright 2003-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # Logilab <contact@logilab.fr>
 msgid ""
 msgstr ""
 "Project-Id-Version: cubicweb-email 0.1.0\n"
 "PO-Revision-Date: 2008-02-15 10:49+0100\n"
 "Last-Translator: Logilab Team <contact@logilab.fr>\n"
 "Language-Team: en <contact@logilab.fr>\n"
@@ -73,15 +73,15 @@
 msgstr "attachment"
 
 # add related box generated message
 msgid "add Email parts EmailPart subject"
 msgstr "email part"
 
 msgid "add EmailThread forked_from EmailThread object"
-msgstr "fored thread"
+msgstr "forked thread"
 
 # subject and object forms for each relation type
 # (no object form for final relation types)
 msgid "alternative"
 msgstr ""
 
 msgctxt "EmailPart"
@@ -169,15 +169,15 @@
 msgid "email_from"
 msgstr "from"
 
 msgid "email_to"
 msgstr "to"
 
 msgid "forked_from"
-msgstr "fored from"
+msgstr "forked from"
 
 msgctxt "EmailThread"
 msgid "forked_from"
 msgstr "forked from"
 
 msgid "forked_from_object"
 msgstr "forks"
```

### Comparing `cubicweb-email-1.9.0/i18n/fr.po` & `cubicweb-email-2.0.0/cubicweb_email/i18n/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # cubicweb-email i18n catalog
-# Copyright 2003-2008 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# Copyright 2003-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # Logilab <contact@logilab.fr>
 msgid ""
 msgstr ""
 "Project-Id-Version: cubicweb-email 0.1.0\n"
 "PO-Revision-Date: 2008-08-07 16:30+0200\n"
 "Last-Translator: Logilab Team <contact@logilab.fr>\n"
 "Language-Team: fr <contact@logilab.fr>\n"
```

