# Comparing `tmp/odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0.tar.gz` & `tmp/odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0.tar", last modified: Tue Apr 11 10:20:05 2023, max compression
+gzip compressed data, was "odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1.tar", last modified: Thu Aug  3 18:56:42 2023, max compression
```

## Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0.tar` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.044494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/
--rw-r--r--   0 root         (0) root         (0)      425 2023-04-11 10:20:05.044494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.031493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.032493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.035493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      709 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.035493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/data/data.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.035493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/i18n/
--rw-rw-rw-   0 root         (0) root         (0)    26377 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/i18n/es.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.038493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/account_allocation.py
--rw-rw-rw-   0 root         (0) root         (0)     1214 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/contract_participation.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/participant_liquidations.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/photovoltaic_power_station.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/res_partner_interest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.038493 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/security/
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/security/ir.model.access.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.040494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/account_allocation.xml
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/contract_participation.xml
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/photovoltaic_power_station.xml
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml
--rw-rw-rw-   0 root         (0) root         (0)     2325 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/res_partner_interest.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.041494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard_view.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:05.043494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/
--rw-r--r--   0 root         (0) root         (0)      425 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1727 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 10:20:04.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 10:20:05.044494 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-04-11 10:19:44.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:56:42.724582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-08-03 18:56:42.724582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:56:42.718582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:56:42.718582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:56:42.720582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:56:42.720582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/data/data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:56:42.720582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    29630 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/i18n/es.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:56:42.722582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/models/
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/models/account_allocation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/models/contract_participation.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/models/participant_liquidations.py
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/models/photovoltaic_power_station.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/models/res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/models/res_partner_interest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:56:42.722582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/security/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:56:42.723582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/views/
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/views/account_allocation.xml
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/views/contract_participation.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1632 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/views/photovoltaic_power_station.xml
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/views/res_partner_interest.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:56:42.723582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/wizard/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/wizard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard_view.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:56:42.724582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-08-03 18:56:42.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-08-03 18:56:42.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 18:56:42.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 18:56:42.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-03 18:56:42.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-03 18:56:42.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 18:56:42.725582 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-08-03 18:56:25.000000 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/setup.py
```

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/__manifest__.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': "Photovoltaic Management Extended",
-    'version': '13.0.1.1.0',
+    'version': '13.0.1.1.1',
     'depends': ['photovoltaic_mgmt', 'photovoltaic_participant_liquidations'],
     'author': "Librecoop",
     'category': 'Sales',
     'description': """
     This module extendes the functionality of the Photovoltaic Management module
     """,
     "installable": True,
```

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/i18n/es.po` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/i18n/es.po`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,36 @@
 # This file contains the translation of the following modules:
 # 	* photovoltaic_mgmt_extended
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 13.0-20221005\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-12-15 11:43+0000\n"
-"PO-Revision-Date: 2022-12-15 11:43+0000\n"
+"POT-Creation-Date: 2023-08-01 11:13+0000\n"
+"PO-Revision-Date: 2023-08-01 13:16+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Content-Transfer-Encoding: \n"
-"Plural-Forms: \n"
+"Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 3.3.2\n"
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__access_warning
 msgid "Access warning"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
+#: model:ir.model,name:photovoltaic_mgmt_extended.model_account_allocation
+msgid "Account allocation"
+msgstr "Reparto"
+
+#. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__message_needaction
 msgid "Action Needed"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_res_partner_interest__active
 msgid "Active"
@@ -83,14 +90,24 @@
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_res_partner_interest__child_ids
 msgid "Child Tags"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
+#: model_terms:ir.ui.view,arch_db:photovoltaic_mgmt_extended.view_photovoltaic_power_station_form_inherit
+msgid "Close long term"
+msgstr "Cerrar largo plazo"
+
+#. module: photovoltaic_mgmt_extended
+#: model_terms:ir.ui.view,arch_db:photovoltaic_mgmt_extended.view_photovoltaic_power_station_form_inherit
+msgid "Close short term"
+msgstr "Cerrar corto plazo"
+
+#. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_res_partner_interest__color
 msgid "Color Index"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__comment
 msgid "Comments"
@@ -109,22 +126,18 @@
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model,name:photovoltaic_mgmt_extended.model_res_partner
 msgid "Contact"
 msgstr "Contacto"
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.actions.act_window,name:photovoltaic_mgmt_extended.action_partner_interest_form
-#: model_terms:ir.ui.view,arch_db:photovoltaic_mgmt_extended.view_partner_interest_form
-msgid "Contact Interest"
-msgstr "Interés de contacto"
-
-#. module: photovoltaic_mgmt_extended
 #: model:ir.ui.menu,name:photovoltaic_mgmt_extended.res_partner_interest_menu
+#: model_terms:ir.ui.view,arch_db:photovoltaic_mgmt_extended.view_partner_interest_form
 msgid "Contact Interests"
-msgstr "Intereses de contacto"
+msgstr "Interés de contacto"
 
 #. module: photovoltaic_mgmt_extended
 #: model_terms:ir.ui.view,arch_db:photovoltaic_mgmt_extended.view_partner_interest_list
 msgid "Contact Tags"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
@@ -156,14 +169,28 @@
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__create_date
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_res_partner_interest__create_date
 msgid "Created on"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
+#: model:ir.model.fields.selection,name:photovoltaic_mgmt_extended.selection__account_allocation__state__crece_acumulado
+#: model:ir.model.fields.selection,name:photovoltaic_mgmt_extended.selection__account_allocation_state_update_wizard__state__crece_acumulado
+#: model:ir.model.fields.selection,name:photovoltaic_mgmt_extended.selection__participant_liquidations__state__crece_acumulado
+msgid "Crece Solar - acumulado"
+msgstr ""
+
+#. module: photovoltaic_mgmt_extended
+#: model:ir.model.fields.selection,name:photovoltaic_mgmt_extended.selection__account_allocation__state__crece_reinvertido
+#: model:ir.model.fields.selection,name:photovoltaic_mgmt_extended.selection__account_allocation_state_update_wizard__state__crece_reinvertido
+#: model:ir.model.fields.selection,name:photovoltaic_mgmt_extended.selection__participant_liquidations__state__crece_reinvertido
+msgid "Crece Solar - reinvertido"
+msgstr ""
+
+#. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_contract_participation__crece_active
 msgid "Crece Solar activado"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_contract_participation__crece_activation_date
 msgid "Crece Solar fecha activación"
@@ -222,15 +249,17 @@
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_photovoltaic_power_station__tecnical_memory_link
 msgid "Enlace memoria técnica"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
+#: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation__state
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__state
+#: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_participant_liquidations__state
 msgid "Estado"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__expense_porcentual_ids
 msgid "Expenses porcentual"
 msgstr ""
@@ -444,24 +473,39 @@
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,help:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__message_unread_counter
 msgid "Number of unread messages"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
+#: model_terms:ir.ui.view,arch_db:photovoltaic_mgmt_extended.view_photovoltaic_power_station_form_inherit
+msgid "Open long term"
+msgstr "Abrir largo plazo"
+
+#. module: photovoltaic_mgmt_extended
+#: model_terms:ir.ui.view,arch_db:photovoltaic_mgmt_extended.view_photovoltaic_power_station_form_inherit
+msgid "Open short term"
+msgstr "Abrir corto plazo"
+
+#. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_res_partner_interest__parent_id
 msgid "Parent Category"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_res_partner_interest__parent_path
 msgid "Parent Path"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
+#: model:ir.model,name:photovoltaic_mgmt_extended.model_participant_liquidations
+msgid "Participant liquidations"
+msgstr ""
+
+#. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__partner_id
 msgid "Partner"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model,name:photovoltaic_mgmt_extended.model_res_partner_interest
 msgid "Partner Interest"
@@ -489,14 +533,24 @@
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model,name:photovoltaic_mgmt_extended.model_photovoltaic_power_station
 msgid "Photovoltaic Power Stations"
 msgstr "Plantas"
 
 #. module: photovoltaic_mgmt_extended
+#: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_photovoltaic_power_station__long_term_investment
+msgid "Plant available for long term investment"
+msgstr "Planta disponible para inversión a largo plazo"
+
+#. module: photovoltaic_mgmt_extended
+#: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_photovoltaic_power_station__short_term_investment
+msgid "Plant available for sort term investment"
+msgstr "Planta disponible para inversión a corto plazo"
+
+#. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__access_url
 msgid "Portal Access URL"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__quarter
 msgid "Quarter"
@@ -504,14 +558,21 @@
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__rated_power
 msgid "Rated power"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
+#: model:ir.model.fields.selection,name:photovoltaic_mgmt_extended.selection__account_allocation__state__reinversion_iva
+#: model:ir.model.fields.selection,name:photovoltaic_mgmt_extended.selection__account_allocation_state_update_wizard__state__reinversion_iva
+#: model:ir.model.fields.selection,name:photovoltaic_mgmt_extended.selection__participant_liquidations__state__reinversion_iva
+msgid "Reinversión IVA"
+msgstr ""
+
+#. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__is_portal
 msgid "Reparto en portal"
 msgstr ""
 
 #. module: photovoltaic_mgmt_extended
 #: model:ir.model.fields,field_description:photovoltaic_mgmt_extended.field_account_allocation_state_update_wizard__allocation_sent
 msgid "Reparto enviado por email"
```

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/models/contract_participation.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/models/contract_participation.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/account_allocation.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/views/account_allocation.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/contract_participation.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/views/contract_participation.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml`

 * *Files 8% similar despite different names*

#### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/views/res_partner.xml`

```diff
@@ -6,8 +6,11 @@
     <field name="inherit_id" ref="base.view_partner_form"/>
     <field name="arch" type="xml">
       <field name="participant" position="after">
         <field name="interest_ids" widget="many2many_tags" options="{'color_field': 'color'}"/>
       </field>
     </field>
   </record>
+  <record id="mail.action_partner_mass_mail" model="ir.actions.act_window">
+    <field name="binding_view_types">list,form</field>
+  </record>
 </odoo>
```

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/views/res_partner_interest.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/views/res_partner_interest.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard_view.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo/addons/photovoltaic_mgmt_extended/wizard/account_allocation_state_update_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.0/odoo13_addon_photovoltaic_mgmt_extended.egg-info/SOURCES.txt` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.1/odoo13_addon_photovoltaic_mgmt_extended.egg-info/SOURCES.txt`

 * *Files identical despite different names*

