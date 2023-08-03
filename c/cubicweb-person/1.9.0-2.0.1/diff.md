# Comparing `tmp/cubicweb-person-1.9.0.tar.gz` & `tmp/cubicweb-person-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-person-1.9.0.tar", last modified: Wed Oct 29 15:20:48 2014, max compression
+gzip compressed data, was "cubicweb-person-2.0.1.tar", last modified: Thu Aug  3 15:37:45 2023, max compression
```

## Comparing `cubicweb-person-1.9.0.tar` & `cubicweb-person-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,38 @@
-drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/
--rw-r--r--   0 narval     (109) narval     (113)     7094 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/setup.py
-drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/test/
--rw-r--r--   0 narval     (109) narval     (113)      311 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/test/test_person.py
-drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/migration/
--rw-r--r--   0 narval     (109) narval     (113)       66 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/migration/postcreate.py
--rw-r--r--   0 narval     (109) narval     (113)      195 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/migration/1.5.0_Any.py
-drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/data/
--rw-r--r--   0 narval     (109) narval     (113)      388 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/data/icon_person.gif
--rw-r--r--   0 narval     (109) narval     (113)       22 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/__init__.py
--rw-rw-r--   0 narval     (109) narval     (113)     2647 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/PKG-INFO
--rw-r--r--   0 narval     (109) narval     (113)     1886 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/schema.py
--rw-r--r--   0 narval     (109) narval     (113)     1525 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/__pkginfo__.py
--rw-r--r--   0 narval     (109) narval     (113)      923 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/entities.py
--rw-r--r--   0 narval     (109) narval     (113)     1925 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/README
--rw-r--r--   0 narval     (109) narval     (113)      258 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/hooks.py
-drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/i18n/
--rw-r--r--   0 narval     (109) narval     (113)     3989 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/i18n/en.po
--rw-r--r--   0 narval     (109) narval     (113)     4265 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/i18n/fr.po
--rw-r--r--   0 narval     (109) narval     (113)     4776 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/views.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-03 15:37:45.615324 cubicweb-person-2.0.1/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      452 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/MANIFEST.in
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2449 2023-08-03 15:37:45.615324 cubicweb-person-2.0.1/PKG-INFO
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2046 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/README.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-03 15:37:45.611324 cubicweb-person-2.0.1/cubicweb_person/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       22 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/cubicweb_person/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      698 2023-08-03 15:37:13.000000 cubicweb-person-2.0.1/cubicweb_person/__pkginfo__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-03 15:37:45.615324 cubicweb-person-2.0.1/cubicweb_person/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      388 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/cubicweb_person/data/icon_person.gif
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-03 15:37:45.615324 cubicweb-person-2.0.1/cubicweb_person/doc/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    46672 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/cubicweb_person/doc/schema.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      924 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/cubicweb_person/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      259 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/cubicweb_person/hooks.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-03 15:37:45.615324 cubicweb-person-2.0.1/cubicweb_person/i18n/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3989 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/cubicweb_person/i18n/en.po
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4265 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/cubicweb_person/i18n/fr.po
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-03 15:37:45.615324 cubicweb-person-2.0.1/cubicweb_person/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      105 2023-08-02 12:57:16.000000 cubicweb-person-2.0.1/cubicweb_person/migration/1.12.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      195 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/cubicweb_person/migration/1.5.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       66 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/cubicweb_person/migration/postcreate.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1876 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/cubicweb_person/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4705 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/cubicweb_person/views.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-03 15:37:45.615324 cubicweb-person-2.0.1/cubicweb_person.egg-info/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2449 2023-08-03 15:37:45.000000 cubicweb-person-2.0.1/cubicweb_person.egg-info/PKG-INFO
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      787 2023-08-03 15:37:45.000000 cubicweb-person-2.0.1/cubicweb_person.egg-info/SOURCES.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2023-08-03 15:37:45.000000 cubicweb-person-2.0.1/cubicweb_person.egg-info/dependency_links.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       42 2023-08-03 15:37:45.000000 cubicweb-person-2.0.1/cubicweb_person.egg-info/entry_points.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2023-08-02 12:53:35.000000 cubicweb-person-2.0.1/cubicweb_person.egg-info/not-zip-safe
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       50 2023-08-03 15:37:45.000000 cubicweb-person-2.0.1/cubicweb_person.egg-info/requires.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       16 2023-08-03 15:37:45.000000 cubicweb-person-2.0.1/cubicweb_person.egg-info/top_level.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       38 2023-08-03 15:37:45.615324 cubicweb-person-2.0.1/setup.cfg
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2621 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/setup.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-03 15:37:45.615324 cubicweb-person-2.0.1/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-03 15:37:45.615324 cubicweb-person-2.0.1/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/test/data/bootstrap_cubes
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      284 2023-08-02 13:16:02.000000 cubicweb-person-2.0.1/test/test_person.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      620 2023-08-02 12:53:19.000000 cubicweb-person-2.0.1/test/unittest_person.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      895 2023-08-02 13:16:02.000000 cubicweb-person-2.0.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-person-1.9.0/PKG-INFO` & `cubicweb-person-2.0.1/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,62 @@
-Metadata-Version: 1.0
-Name: cubicweb-person
-Version: 1.9.0
-Summary: person component for the CubicWeb framework
-Home-page: http://www.cubicweb.org/project/cubicweb-person
-Author: Logilab
-Author-email: contact@logilab.fr
-License: LGPL
-Description: Summary
-        -------
-        
-        `person` provides person informations :
-        
-        - firstname
-        - surname / lastname
-        - civility
-        - arbitrary text description
-        - a relation to an email address (NB, the `EmailAddress` entity is
-          automatically provided by cubicweb).
-        
-        If the `addressbook` cube is used, persons will also have *phone* and
-        *postal_address* relations to store more contact information.
-        
-        There is a special relation called 'primary_email'. A person can be linked to
-        multiple email addresses (using the 'use_email' relation). The primary email
-        must be unique. At the creation of the first email, this relation is
-        automatically added (though you can change it later, of course).
-        
-        Recommends
-        ----------
-        
-        - `addressbook` cube
-        
-        
-        Usage
-        -----
-        
-        In addition of basic entity views, this cube provides :
-        
-        - *VCardPersonView*, displays a person in the VCard file format
-           (.. _VCard on wikipedia: http://en.wikipedia.org/wiki/VCard) .
-        
-           This view creates a file called `vcard.vcf` which can be open in
-           your addressbook application (Kmail, Thunderbird and so on). In
-           order to generate this file, you have to access to a specific view
-           using an url address with `?vid=vcard` suffix.
-        
-           How to personalize the person primary view in order to add a link
-           for the vcard ?
-        
-           .. sourcecode:: python
-        
-             class PersonalizedPersonPrimaryView(PersonPrimaryView):
-        
-                 def render_entity_attributes(self, entity):
-                     super(PersonalizedPersonPrimaryView, self).render_entity_attributes(entity)
-                     self.w(u'<div><a href="%s">export contact as vcard</a></div>'  % entity.absolute_url(vid='vcard'))
-        
-            This view will not be selected by default. You have to registered
-            this view or add a selector. For more information, please refer to
-            XXX in the doc.
-        
-        - a *civility facet*, this facet (XXX: ref to facet doc) will be shown
-          if a view displays a result set of at least two Person entities with
-          different civilities.
-        
-Platform: UNKNOWN
+Summary
+-------
+
+`person` provides person informations :
+
+- firstname
+- surname / lastname
+- civility
+- arbitrary text description
+- a relation to an email address (NB, the `EmailAddress` entity is
+  automatically provided by cubicweb).
+
+If the `addressbook` cube is used, persons will also have *phone* and
+*postal_address* relations to store more contact information.
+
+There is a special relation called 'primary_email'. A person can be linked to
+multiple email addresses (using the 'use_email' relation). The primary email
+must be unique. At the creation of the first email, this relation is
+automatically added (though you can change it later, of course).
+
+Recommends
+----------
+
+- `addressbook` cube
+
+
+Usage
+-----
+
+In addition of basic entity views, this cube provides :
+
+- *VCardPersonView*, displays a person in the VCard file format
+   (.. _VCard on wikipedia: http://en.wikipedia.org/wiki/VCard) .
+
+   This view creates a file called `vcard.vcf` which can be open in
+   your addressbook application (Kmail, Thunderbird and so on). In
+   order to generate this file, you have to access to a specific view
+   using an url address with `?vid=vcard` suffix.
+
+   How to personalize the person primary view in order to add a link
+   for the vcard ?
+
+   .. sourcecode:: python
+
+     class PersonalizedPersonPrimaryView(PersonPrimaryView):
+
+         def render_entity_attributes(self, entity):
+             super(PersonalizedPersonPrimaryView, self).render_entity_attributes(entity)
+             self.w(u'<div><a href="%s">export contact as vcard</a></div>'  % entity.absolute_url(vid='vcard'))
+
+    This view will not be selected by default. You have to registered
+    this view or add a selector. For more information, please refer to
+    XXX in the doc.
+
+- a *civility facet*, this facet (XXX: ref to facet doc) will be shown
+  if a view displays a result set of at least two Person entities with
+  different civilities.
+
+Contributing
+------------
+
+Information on how to contribute can be found here https://www.logilab.org/Card/contributing
```

### Comparing `cubicweb-person-1.9.0/schema.py` & `cubicweb-person-2.0.1/cubicweb_person/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from yams.buildobjs import (EntityType, SubjectRelation, String, RichString,
                             RelationDefinition)
 from yams.reader import context
 from cubicweb.schema import RRQLExpression, RQLConstraint
 
+from cubicweb import _
 
-_ = unicode
 
 class Person(EntityType):
     """a physical person"""
-    surname   = String(required=True, fulltextindexed=True, indexed=True, maxsize=64)
+    surname = String(required=True, fulltextindexed=True, indexed=True, maxsize=64)
     firstname = String(fulltextindexed=True, maxsize=64)
-    civility  = String(required=True, internationalizable=True,
-                       vocabulary=(_('Mr'), _('Ms'), _('Mrs')),
-                       default='Mr')
+    civility = String(required=True, internationalizable=True,
+                      vocabulary=(_('Mr'), _('Mrs')),
+                      default='Mr')
 
-    description        = RichString(fulltextindexed=True)
+    description = RichString(fulltextindexed=True)
 
-    if 'PhoneNumber' in context.defined: # from addressbook package
+    if 'PhoneNumber' in context.defined:  # from addressbook package
         phone = SubjectRelation('PhoneNumber', composite='subject')
     if 'PostalAddress' in context.defined:
         postal_address = SubjectRelation('PostalAddress', composite='subject')
     if 'IMAddress' in context.defined:
         im_address = SubjectRelation('IMAddress', composite='subject')
 
 
-
 class use_email(RelationDefinition):
     """person's email account"""
     __permissions__ = {
         'read':   ('managers', 'users', 'guests',),
         'add':    ('managers', RRQLExpression('U has_update_permission S'),),
         'delete': ('managers', RRQLExpression('U has_update_permission S'),),
         }
@@ -44,9 +43,8 @@
         'read':   ('managers', 'users', 'guests',),
         'add':    ('managers', RRQLExpression('U has_update_permission S'),),
         'delete': ('managers', RRQLExpression('U has_update_permission S'),),
         }
     subject = "Person"
     object = "EmailAddress"
     cardinality = '??'
-    constraints= [RQLConstraint('S use_email O')]
-
+    constraints = [RQLConstraint('S use_email O')]
```

### Comparing `cubicweb-person-1.9.0/entities.py` & `cubicweb-person-2.0.1/cubicweb_person/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 :copyright: 2003-2011 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
 from cubicweb.entities import AnyEntity, fetch_config
 
+
 class Person(AnyEntity):
     """customized class for Person entities"""
     __regid__ = 'Person'
     fetch_attrs, cw_fetch_order = fetch_config(['surname', 'firstname'])
     rest_attr = 'surname'
     skip_copy_for = ('primary_email',)
```

### Comparing `cubicweb-person-1.9.0/README` & `cubicweb-person-2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: cubicweb-person
+Version: 2.0.1
+Summary: person component for the CubicWeb framework
+Home-page: https://www.cubicweb.org/project/cubicweb-person
+Author: Logilab
+Author-email: contact@logilab.fr
+License: LGPL
+Classifier: Environment :: Web Environment
+Classifier: Framework :: CubicWeb
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: JavaScript
+
 Summary
 -------
 
 `person` provides person informations :
 
 - firstname
 - surname / lastname
@@ -51,7 +64,12 @@
     This view will not be selected by default. You have to registered
     this view or add a selector. For more information, please refer to
     XXX in the doc.
 
 - a *civility facet*, this facet (XXX: ref to facet doc) will be shown
   if a view displays a result set of at least two Person entities with
   different civilities.
+
+Contributing
+------------
+
+Information on how to contribute can be found here https://www.logilab.org/Card/contributing
```

### Comparing `cubicweb-person-1.9.0/i18n/en.po` & `cubicweb-person-2.0.1/cubicweb_person/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-person-1.9.0/i18n/fr.po` & `cubicweb-person-2.0.1/cubicweb_person/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-person-1.9.0/views.py` & `cubicweb-person-2.0.1/cubicweb_person/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,61 +4,46 @@
 :copyright: 2003-2010 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
 from logilab.mtconverter import xml_escape
 
-from cubicweb.schema import display_name
+from cubicweb import _
 from cubicweb.predicates import is_instance, score_entity
-from cubicweb.web import action
-from cubicweb.web.views import baseviews, primary, uicfg, vcard
-from cubicweb.web.facet import AttributeFacet
+from cubicweb_web import action
+from cubicweb_web.views import baseviews, primary, uicfg, vcard
+from cubicweb_web.facet import AttributeFacet
 
-_pvs =uicfg.primaryview_section
-_pvdc = uicfg.primaryview_display_ctrl
+_pvs = uicfg.primaryview_section
 
 for attr in ('civility', 'firstname', 'surname'):
     _pvs.tag_attribute(('Person', attr), 'hidden')
-for rtype in ('use_email', 'primary_email',
-              'phone', 'im_address', 'postal_address'):
-    _pvs.tag_subject_of(('Person', rtype, '*'), 'hidden')
-_pvdc.tag_attribute(('Person', 'description'), {'showlabel': False,
-                                                'order': 0})
-
-_afs = uicfg.autoform_section
-_afs.tag_subject_of(('Person', 'phone', '*'), 'main', 'inlined')
-_afs.tag_subject_of(('Person', 'postal_address', '*'), 'main', 'inlined')
-_afs.tag_subject_of(('Person', 'im_address', '*'), 'main', 'inlined')
+
+_pvs.tag_subject_of(('Person', 'use_email', '*'), 'attributes')
+_pvs.tag_subject_of(('Person', 'primary_email', '*'), 'hidden')
+
+_pvdc = uicfg.primaryview_display_ctrl
+_pvdc.tag_attribute(('Person', 'description'),
+                    {'showlabel': False, 'order': 0})
+_pvdc.tag_attribute(('Person', 'use_email'),
+                    {'order': 2, 'vid': 'csv', 'label': 'use_email'})
+
+
+class HRSView(baseviews.CSVView):
+    __regid__ = 'person.hrs'
+    separator = u'<hr/>'
 
 
 class PersonPrimaryView(primary.PrimaryView):
     __select__ = is_instance('Person')
-    attr_table_relations = [('phone', ', '.join),
-                            ('use_email', ', '.join),
-                            ('im_address', ', '.join),
-                            ('postal_address', '<hr/>\n'.join),
-                            ]
 
     def render_entity_title(self, entity):
         self.w(u'<h1>%s</h1>' % xml_escape(entity.name(civility=True)))
 
-    def render_entity_attributes(self, entity):
-        super(PersonPrimaryView, self).render_entity_attributes(entity)
-        hascontent = False
-        for rel, join in self.attr_table_relations:
-            related = getattr(entity, rel, None)
-            if related:
-                if not hascontent:
-                    self.w(u"<table>")
-                    hascontent = True
-                self.field(rel, join(e.view('incontext') for e in related), table=True)
-        if hascontent:
-            self.w(u"</table>")
-
 
 class PersonTextView(baseviews.TextView):
     __select__ = is_instance('Person')
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
         self.w(entity.name())
@@ -97,34 +82,51 @@
         w = self.w
         who = u'%s %s' % (entity.surname or '',
                           entity.firstname or '')
         w(u'FN:%s\n' % who)
         w(u'N:%s;;;;\n' % who)
         w(u'TITLE:%s\n' % who)
         # XXX
-        #if entity.address:
+        # if entity.address:
         #    w(u'ADR;TYPE=WORK,POSTAL,PARCEL:;;%s\n' % ';'.join(entity.address.splitlines()))
         for phone in getattr(entity, 'phone', ()):
             ptype = vcard.VCARD_PHONE_TYPES.get(phone.type, phone.type.upper())
             w(u'TEL;TYPE=%s;VOICE:%s\n' % (ptype, phone.number))
         for email in getattr(entity, 'use_email', ()):
             w(u'EMAIL;TYPE=INTERNET:%s\n' % email.address)
 
 
-## actions ####################################################################
+# actions ####################################################################
 
 class AddPersonFromEmailAction(action.LinkToEntityAction):
     __regid__ = 'addperson-fromemail'
     __select__ = (is_instance('EmailAddress')
                   & score_entity(lambda x: not x.reverse_use_email))
 
     title = _('add Person use_email EmailAddress object')
     target_etype = 'Person'
     rtype = 'use_email'
     target = 'subject'
 
-## facets #####################################################################
+
+# facets #####################################################################
 
 class CivilityFacet(AttributeFacet):
     __regid__ = 'civility-facet'
     __select__ = is_instance('Person')
     rtype = 'civility'
+
+
+def registration_callback(vreg):
+    vreg.register_all(globals().values(), __name__)
+    if 'addressbook' in vreg.config.cubes():
+        for rtype in ('phone', 'im_address', 'postal_address'):
+            _pvs.tag_subject_of(('Person', rtype, '*'), 'attributes')
+        _pvdc.tag_attribute(('Person', 'phone'), {'order': 1, 'vid': 'csv'})
+        _pvdc.tag_attribute(('Person', 'im_address'), {'order': 3, 'vid': 'csv'})
+        _pvdc.tag_attribute(('Person', 'postal_address'),
+                            {'order': 4, 'vid': 'person.hrs'})
+
+        _afs = uicfg.autoform_section
+        _afs.tag_subject_of(('Person', 'phone', '*'), 'main', 'inlined')
+        _afs.tag_subject_of(('Person', 'postal_address', '*'), 'main', 'inlined')
+        _afs.tag_subject_of(('Person', 'im_address', '*'), 'main', 'inlined')
```

