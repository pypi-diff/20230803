# Comparing `tmp/monday-item-parser-0.2.8.tar.gz` & `tmp/monday-item-parser-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monday-item-parser-0.2.8.tar", max compression
+gzip compressed data, was "monday-item-parser-0.2.9.tar", max compression
```

## Comparing `monday-item-parser-0.2.8.tar` & `monday-item-parser-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/LICENSE
--rw-r--r--   0        0        0     9250 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/README.md
--rw-r--r--   0        0        0      260 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/__init__.py
--rw-r--r--   0        0        0       49 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/exceptions.py
--rw-r--r--   0        0        0      841 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/__init__.py
--rw-r--r--   0        0        0      399 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/checkbox.py
--rw-r--r--   0        0        0      965 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/country.py
--rw-r--r--   0        0        0     1723 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/date.py
--rw-r--r--   0        0        0      460 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/email.py
--rw-r--r--   0        0        0     1657 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/field.py
--rw-r--r--   0        0        0      829 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/helpers.py
--rw-r--r--   0        0        0      749 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/link.py
--rw-r--r--   0        0        0      452 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/mirror.py
--rw-r--r--   0        0        0      507 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/number.py
--rw-r--r--   0        0        0     1507 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/people.py
--rw-r--r--   0        0        0     1660 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/phone.py
--rw-r--r--   0        0        0     1278 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/status.py
--rw-r--r--   0        0        0      380 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/tags.py
--rw-r--r--   0        0        0      773 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/text.py
--rw-r--r--   0        0        0     1291 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/fields/timeline.py
--rw-r--r--   0        0        0      510 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/helpers.py
--rw-r--r--   0        0        0    16710 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/monday_item_parser/item.py
--rw-r--r--   0        0        0      558 2022-04-22 10:19:30.054123 monday-item-parser-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    10367 2022-04-22 10:21:06.939532 monday-item-parser-0.2.8/setup.py
--rw-r--r--   0        0        0     9987 2022-04-22 10:21:06.940312 monday-item-parser-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-04-22 14:51:05.875975 monday-item-parser-0.2.9/LICENSE
+-rw-r--r--   0        0        0     9304 2022-04-22 14:51:05.875975 monday-item-parser-0.2.9/README.md
+-rw-r--r--   0        0        0      260 2022-04-22 14:51:05.875975 monday-item-parser-0.2.9/monday_item_parser/__init__.py
+-rw-r--r--   0        0        0       49 2022-04-22 14:51:05.875975 monday-item-parser-0.2.9/monday_item_parser/exceptions.py
+-rw-r--r--   0        0        0      841 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/__init__.py
+-rw-r--r--   0        0        0      399 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/checkbox.py
+-rw-r--r--   0        0        0      965 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/country.py
+-rw-r--r--   0        0        0     1723 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/date.py
+-rw-r--r--   0        0        0      460 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/email.py
+-rw-r--r--   0        0        0     1657 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/field.py
+-rw-r--r--   0        0        0      829 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/helpers.py
+-rw-r--r--   0        0        0      749 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/link.py
+-rw-r--r--   0        0        0      452 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/mirror.py
+-rw-r--r--   0        0        0      507 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/number.py
+-rw-r--r--   0        0        0     1507 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/people.py
+-rw-r--r--   0        0        0     1660 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/phone.py
+-rw-r--r--   0        0        0     1278 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/status.py
+-rw-r--r--   0        0        0      380 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/tags.py
+-rw-r--r--   0        0        0      783 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/text.py
+-rw-r--r--   0        0        0     1291 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/fields/timeline.py
+-rw-r--r--   0        0        0      510 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/helpers.py
+-rw-r--r--   0        0        0    16710 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/monday_item_parser/item.py
+-rw-r--r--   0        0        0      558 2022-04-22 14:51:05.879975 monday-item-parser-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    10422 2022-04-22 14:52:46.582059 monday-item-parser-0.2.9/setup.py
+-rw-r--r--   0        0        0    10041 2022-04-22 14:52:46.582890 monday-item-parser-0.2.9/PKG-INFO
```

### Comparing `monday-item-parser-0.2.8/LICENSE` & `monday-item-parser-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/README.md` & `monday-item-parser-0.2.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ## Requirements
 
 * Python >= 3.7
 * [Monday library](https://github.com/ProdPerfect/monday) for the Mondayhttp client
 
 ## Changelog
 
+* 0.2.9 (2022-04-22) - Fixed a bug in Long Text field
 * 0.2.8 (2022-04-22) - Added support for Long Text field
 * 0.2.7 (2022-03-30) - Bumped version because of workflow problems (again :()
 * 0.2.5 (2022-03-30) - Added mirror field to readme.
 * 0.2.4 (2022-03-30) - Added support for mirror (lookup) fields.
 * 0.2.3 (2021-01-16) - Same as 0.2.2, but got some problems with PyPI and Github Workflows again. :(
 * 0.2.2 (2021-01-16) - Added support for [search items by column value](https://api.developer.monday.com/docs/items-by-column-values-queries)
 * 0.2.1 (2021-01-16) - Added hooks for field values.
```

### Comparing `monday-item-parser-0.2.8/monday_item_parser/fields/__init__.py` & `monday-item-parser-0.2.9/monday_item_parser/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/monday_item_parser/fields/country.py` & `monday-item-parser-0.2.9/monday_item_parser/fields/country.py`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/monday_item_parser/fields/date.py` & `monday-item-parser-0.2.9/monday_item_parser/fields/date.py`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/monday_item_parser/fields/field.py` & `monday-item-parser-0.2.9/monday_item_parser/fields/field.py`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/monday_item_parser/fields/helpers.py` & `monday-item-parser-0.2.9/monday_item_parser/fields/helpers.py`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/monday_item_parser/fields/link.py` & `monday-item-parser-0.2.9/monday_item_parser/fields/link.py`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/monday_item_parser/fields/people.py` & `monday-item-parser-0.2.9/monday_item_parser/fields/people.py`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/monday_item_parser/fields/phone.py` & `monday-item-parser-0.2.9/monday_item_parser/fields/phone.py`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/monday_item_parser/fields/status.py` & `monday-item-parser-0.2.9/monday_item_parser/fields/status.py`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/monday_item_parser/fields/text.py` & `monday-item-parser-0.2.9/monday_item_parser/fields/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 class LongTextField(Field):
     __monday_field_type__ = "long-text"
 
     def __init__(self, default: str = None):
         self.value = default
 
     def to_monday_dict(self):
-        return self.value
+        return {"text": self.value}
 
     def from_monday_dict(self, data: str):
         self.value = data if data else None
 
     def search_representation(self) -> str:
         return str(self.value)
```

### Comparing `monday-item-parser-0.2.8/monday_item_parser/fields/timeline.py` & `monday-item-parser-0.2.9/monday_item_parser/fields/timeline.py`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/monday_item_parser/item.py` & `monday-item-parser-0.2.9/monday_item_parser/item.py`

 * *Files identical despite different names*

### Comparing `monday-item-parser-0.2.8/pyproject.toml` & `monday-item-parser-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monday-item-parser"
-version = "0.2.8"
+version = "0.2.9"
 description = "monday-item-parser is a library used to define Monday items structure in a specific board, and lets the user fetch, create, update and delete items from this board."
 readme = "README.md"
 authors = ["Aviv Atedgi <aviv.atedgi2000@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 monday = "^1.2.7"
```

### Comparing `monday-item-parser-0.2.8/setup.py` & `monday-item-parser-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['bidict>=0.21.4,<0.22.0', 'monday>=1.2.7,<2.0.0', 'requests>=2.27.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'monday-item-parser',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'monday-item-parser is a library used to define Monday items structure in a specific board, and lets the user fetch, create, update and delete items from this board.',
-    'long_description': '# [Monday Item Parser](https://github.com/avivatedgi/monday-item-parser)\n\n[![Tests & Deploy to PyPI](https://github.com/avivatedgi/monday-item-parser/actions/workflows/deploy_pypi.yml/badge.svg)](https://github.com/avivatedgi/monday-item-parser/actions/workflows/deploy_pypi.yml) [![PyPI version](https://badge.fury.io/py/monday-item-parser.svg)](https://badge.fury.io/py/monday-item-parser)\n\n## Introduction\n\n[Monday Item Parser](https://github.com/avivatedgi/monday-item-parser) is a library used to define [Monday](www.monday.com) items structure in a specific board, and lets the user fetch, create, update and delete items from this board.\n\n## Installation\n\n```bash\npip install monday-item-parser\n```\n\n## Requirements\n\n* Python >= 3.7\n* [Monday library](https://github.com/ProdPerfect/monday) for the Mondayhttp client\n\n## Changelog\n\n* 0.2.8 (2022-04-22) - Added support for Long Text field\n* 0.2.7 (2022-03-30) - Bumped version because of workflow problems (again :()\n* 0.2.5 (2022-03-30) - Added mirror field to readme.\n* 0.2.4 (2022-03-30) - Added support for mirror (lookup) fields.\n* 0.2.3 (2021-01-16) - Same as 0.2.2, but got some problems with PyPI and Github Workflows again. :(\n* 0.2.2 (2021-01-16) - Added support for [search items by column value](https://api.developer.monday.com/docs/items-by-column-values-queries)\n* 0.2.1 (2021-01-16) - Added hooks for field values.\n* 0.2.0 (2021-01-14) - Updated the item\'s field value set method to be explicit (without calling `.value`)\n* 0.1.2 (2021-01-13) - Fixed a small bug in the `Item::__init__` function\n* 0.1.1 (2021-01-13) - Still first release, but got some problems with PyPI and Github Workflows\n* 0.1.0 (2021-01-13) - First release\n\n## How to use\n\n### Items\n\nItems are the full board item structure, built from fields.\n\n```python\nfrom monday import MondayClient\nfrom monday_item_parser import Item, CheckboxField\n\n\nboard_id = 1234\nmonday_client = MondayClient("MONDAY_API_KEY_HERE")\n\n\nclass MyItem(Item, board_id=board_id, monday_client=monday_client):\n    checkbox_example = CheckboxField()\n\n    # Can be declared either as a type or as an instance, so this is good as well:\n    checkbox_example = CheckboxField\n```\n\n**NOTE:** The variables in your item class must be named EXACTLY the same as in your monday board but in lower-case and replace spaces into underscore. For example a column in Monday with the name `My Nice Column` will must be defined in your item class `my_nice_column`.\n\n#### Fetch items from board\n\n```pycon\n>>> for item in ExampleItem.fetch_items_from_board():\n>>>     print(item)\n```\n\n![Items Preview](docs/images/items-print.png)\n\n#### Fetch items by column value\n\nYou can fetch all of the items from board by a specific column value filter.\n\n```python\n# Let\'s filter all of the items with a Status column named "status_example" that holds the label "Done"\nfor item in ExampleItem.fetch_items_by_column_value(status_example="Done"):\n    print(item)\n```\n\nMore info about supported and unsupported fields you can search by [here](https://api.developer.monday.com/docs/items-by-column-values-queries).\n\n| Field Type | Field Value to Search By |\n| ---------- | ------------------------ |\n| Text | `str` The text to search |\n| Status | `str` The label to search |\n| Numbers | Either `int` or `float`. The value to search |\n| Date | `datetime.datetime` The date (year, month and day) to search by |\n| Phone | `Phone` (internal library class) The phone number to search by |\n| Country | `str` The country code to search by |\n| Email | `str` The email to search by |\n| Timeline | `Timeline` (internal library class) The start and end date to search by |\n| Link | `Link` (internal library class) The display text (not the actual url link) to search by |\n| Mirror | `str` The text to search |\n| Long Text | `str` The text to search |\n\n#### Create Item\n\n**NOTE:** You can only create an item that isn\'t fetched from the board / already created using this exact function. If you want to create a new item that was fetched from the board you should use the `duplicate_item` function\n\n```pycon\n>>> item = MyItem(checkbox_example=True)\n>>> item.name = "My First Example"\n>>> item.create_item()\n```\n\n#### Duplicate Item\n\n**NOTE:** You can only duplicate an item that was fetched from the board / created by the `create_item` function.\n\n```pycon\n>>> new_item = item.duplicate_item()\n```\n\n#### Update Item\n\n**NOTE:** You can only update an item that was fetched from the board / created by the `create_item` function.\n\n```pycon\n>>> new_item.name = \'Updated Item\'\n>>> new_item.checkbox_example = False\n>>> new_item.update_item()\n```\n\n#### Delete Item\n\n**NOTE:** You can only delete an item that was fetched from the board / created by the `create_item` function.\n\n```pycon\n>>> new_item.delete_item()\n```\n\n#### Get Group Ids in Board\n\n```pycon\n>>> for group_id in ItemExample.fetch_group_ids():\n>>>     print(group_id)\n"topics"\n"group_title"\n```\n\n#### Hook Field Values\n\nA hook can be registered for whenever the value on a specific field is changed.\n\n```python\nfrom monday_item_parser import *\n\nclass ItemWithFieldHook(Item, monday_client=client, board_id=testing_board_id):\n    status_example = StatusField\n    checkbox_example = CheckboxField\n\n    @field_updated_hook(status_example)\n    def status_example_hook(self):\n        if self.status_example.value is not None:\n            # In the hook you must update the value with the\n            # `.value` attribute if you don\'t want to trigger the hook again\n            self.status_example.value += 1\n        else:\n            self.status_example.value = 0\n\nitem = ItemWithFieldHook()\n# Trigger the hook by setting the value WITHOUT the `.value` attribute\nitem.status_example = 5\nassert item.status_example.value == 6\n```\n\n### Fields\n\nField is actually an Monday board\'s item column. The currently supported types are:\n\n| Monday Column Type | Library Class Name |\n| ------------------ | ------------------ |\n| Checkbox | `CheckboxField` |\n| Country | `CountryField` |\n| Date | `DateField` |\n| Email | `EmailField` |\n| Link | `LinkField` |\n| Number | `NumberField` |\n| People | `PeopleField` |\n| Phone | `PhoneField` |\n| Status | `StatusField` |\n| Tags | `TagsField` |\n| Text | `TextField` |\n| Timeline | `TimelineField` |\n| Mirror | `MirrorField` |\n| Long Text | `LongTextField` |\n\n#### Full Example\n\n```python\nclass ItemExample(Item, monday_client=client, board_id=testing_board_id):\n    status_example = StatusField\n    date_example = DateField\n    checkbox_example = CheckboxField\n    country_example = CountryField\n    email_example = EmailField\n    link_example = LinkField\n    numbers_example = NumberField\n    people_example = PeopleField\n    phone_example = PhoneField\n    tags_example = TagsField\n    text_example = TextField\n    timeline_example = TimelineField\n\tmirror_example = MirrorField\n    long_text_example = LongTextField\n\nitem = ItemExample()\n\n# Setting the values of an item\nitem.item_name = "Aviv Atedgi"\nitem.status_example = "Working on it"\nitem.date_example = datetime.now()\nitem.checkbox_example = True\nitem.country_example = "IL"\nitem.email_example = "aviv.atedgi2000@gmail.com"\nitem.link_example.value.url = "https://www.github.com/avivatedgi"\nitem.link_example.value.text = "My Github Profile"\nitem.link_example = LinkField(url="https://www.google.com", text="Google It")\nitem.numbers_example = 192.4\nitem.people_example = [Person(25200525)]\nitem.phone_example.value.country_code = "IL"\nitem.phone_example.value.phone = "0501234567"\nitem.phone_example = PhoneField(phone="12123123123", country_code="US")\nitem.tags_example = [12808387]\nitem.text_example = "My Cool Text Example"\nitem.timeline_example.value.start = datetime.strptime("2000-05-01", "%Y-%m-%d")\nitem.timeline_example.value.end = datetime.now()\nitem.timeline_example = TimelineField(\n    start=datetime.strptime("2005-04-12", "%Y-%m-%d"),\n    end=datetime.now(),\n)\nitem.long_text_example = "Hello\\nWorld"\n\n# Getting the values of an item\nprint("Status Example =", item.status_example.value)\nprint("Date Example =", item.date_example.value)\nprint("Checkbox Example =", item.checkbox_example.value)\nprint("Country Example =", item.country_example.value)\nprint("Email Example =", item.email_example.value)\nprint("Link Example URL =", item.link_example.value.url)\nprint("Link Example Text =", item.link_example.value.text)\nprint("Numbers Example =", item.numbers_example.value)\nprint("People Example =", item.people_example.value)\nprint("Phone Example Country Code =", item.phone_example.value.country_code)\nprint("Phone Example Phone Number =", item.phone_example.value.phone)\nprint("Tags Example =", item.tags_example.value)\nprint("Text Example =", item.text_example.value)\nprint("Timeline Example Start Date =", item.timeline_example.value.start)\nprint("Timeline Example End Date =", item.timeline_example.value.end)\nprint("Mirror Example = ", item.mirror_example.value)\nprint("Long Text Example = ", item.long_text_example.value)\n```\n\n## Special Thanks\n\n* [Hydration](https://github.com/shustinm/hydration) ([Michael Shustin](https://github.com/shustinm/)) For the idea of the items metaclass\n* [Monday](https://github.com/ProdPerfect/monday) ([ProdPerfect](https://github.com/ProdPerfect)) For the Monday client use in the library\n',
+    'long_description': '# [Monday Item Parser](https://github.com/avivatedgi/monday-item-parser)\n\n[![Tests & Deploy to PyPI](https://github.com/avivatedgi/monday-item-parser/actions/workflows/deploy_pypi.yml/badge.svg)](https://github.com/avivatedgi/monday-item-parser/actions/workflows/deploy_pypi.yml) [![PyPI version](https://badge.fury.io/py/monday-item-parser.svg)](https://badge.fury.io/py/monday-item-parser)\n\n## Introduction\n\n[Monday Item Parser](https://github.com/avivatedgi/monday-item-parser) is a library used to define [Monday](www.monday.com) items structure in a specific board, and lets the user fetch, create, update and delete items from this board.\n\n## Installation\n\n```bash\npip install monday-item-parser\n```\n\n## Requirements\n\n* Python >= 3.7\n* [Monday library](https://github.com/ProdPerfect/monday) for the Mondayhttp client\n\n## Changelog\n\n* 0.2.9 (2022-04-22) - Fixed a bug in Long Text field\n* 0.2.8 (2022-04-22) - Added support for Long Text field\n* 0.2.7 (2022-03-30) - Bumped version because of workflow problems (again :()\n* 0.2.5 (2022-03-30) - Added mirror field to readme.\n* 0.2.4 (2022-03-30) - Added support for mirror (lookup) fields.\n* 0.2.3 (2021-01-16) - Same as 0.2.2, but got some problems with PyPI and Github Workflows again. :(\n* 0.2.2 (2021-01-16) - Added support for [search items by column value](https://api.developer.monday.com/docs/items-by-column-values-queries)\n* 0.2.1 (2021-01-16) - Added hooks for field values.\n* 0.2.0 (2021-01-14) - Updated the item\'s field value set method to be explicit (without calling `.value`)\n* 0.1.2 (2021-01-13) - Fixed a small bug in the `Item::__init__` function\n* 0.1.1 (2021-01-13) - Still first release, but got some problems with PyPI and Github Workflows\n* 0.1.0 (2021-01-13) - First release\n\n## How to use\n\n### Items\n\nItems are the full board item structure, built from fields.\n\n```python\nfrom monday import MondayClient\nfrom monday_item_parser import Item, CheckboxField\n\n\nboard_id = 1234\nmonday_client = MondayClient("MONDAY_API_KEY_HERE")\n\n\nclass MyItem(Item, board_id=board_id, monday_client=monday_client):\n    checkbox_example = CheckboxField()\n\n    # Can be declared either as a type or as an instance, so this is good as well:\n    checkbox_example = CheckboxField\n```\n\n**NOTE:** The variables in your item class must be named EXACTLY the same as in your monday board but in lower-case and replace spaces into underscore. For example a column in Monday with the name `My Nice Column` will must be defined in your item class `my_nice_column`.\n\n#### Fetch items from board\n\n```pycon\n>>> for item in ExampleItem.fetch_items_from_board():\n>>>     print(item)\n```\n\n![Items Preview](docs/images/items-print.png)\n\n#### Fetch items by column value\n\nYou can fetch all of the items from board by a specific column value filter.\n\n```python\n# Let\'s filter all of the items with a Status column named "status_example" that holds the label "Done"\nfor item in ExampleItem.fetch_items_by_column_value(status_example="Done"):\n    print(item)\n```\n\nMore info about supported and unsupported fields you can search by [here](https://api.developer.monday.com/docs/items-by-column-values-queries).\n\n| Field Type | Field Value to Search By |\n| ---------- | ------------------------ |\n| Text | `str` The text to search |\n| Status | `str` The label to search |\n| Numbers | Either `int` or `float`. The value to search |\n| Date | `datetime.datetime` The date (year, month and day) to search by |\n| Phone | `Phone` (internal library class) The phone number to search by |\n| Country | `str` The country code to search by |\n| Email | `str` The email to search by |\n| Timeline | `Timeline` (internal library class) The start and end date to search by |\n| Link | `Link` (internal library class) The display text (not the actual url link) to search by |\n| Mirror | `str` The text to search |\n| Long Text | `str` The text to search |\n\n#### Create Item\n\n**NOTE:** You can only create an item that isn\'t fetched from the board / already created using this exact function. If you want to create a new item that was fetched from the board you should use the `duplicate_item` function\n\n```pycon\n>>> item = MyItem(checkbox_example=True)\n>>> item.name = "My First Example"\n>>> item.create_item()\n```\n\n#### Duplicate Item\n\n**NOTE:** You can only duplicate an item that was fetched from the board / created by the `create_item` function.\n\n```pycon\n>>> new_item = item.duplicate_item()\n```\n\n#### Update Item\n\n**NOTE:** You can only update an item that was fetched from the board / created by the `create_item` function.\n\n```pycon\n>>> new_item.name = \'Updated Item\'\n>>> new_item.checkbox_example = False\n>>> new_item.update_item()\n```\n\n#### Delete Item\n\n**NOTE:** You can only delete an item that was fetched from the board / created by the `create_item` function.\n\n```pycon\n>>> new_item.delete_item()\n```\n\n#### Get Group Ids in Board\n\n```pycon\n>>> for group_id in ItemExample.fetch_group_ids():\n>>>     print(group_id)\n"topics"\n"group_title"\n```\n\n#### Hook Field Values\n\nA hook can be registered for whenever the value on a specific field is changed.\n\n```python\nfrom monday_item_parser import *\n\nclass ItemWithFieldHook(Item, monday_client=client, board_id=testing_board_id):\n    status_example = StatusField\n    checkbox_example = CheckboxField\n\n    @field_updated_hook(status_example)\n    def status_example_hook(self):\n        if self.status_example.value is not None:\n            # In the hook you must update the value with the\n            # `.value` attribute if you don\'t want to trigger the hook again\n            self.status_example.value += 1\n        else:\n            self.status_example.value = 0\n\nitem = ItemWithFieldHook()\n# Trigger the hook by setting the value WITHOUT the `.value` attribute\nitem.status_example = 5\nassert item.status_example.value == 6\n```\n\n### Fields\n\nField is actually an Monday board\'s item column. The currently supported types are:\n\n| Monday Column Type | Library Class Name |\n| ------------------ | ------------------ |\n| Checkbox | `CheckboxField` |\n| Country | `CountryField` |\n| Date | `DateField` |\n| Email | `EmailField` |\n| Link | `LinkField` |\n| Number | `NumberField` |\n| People | `PeopleField` |\n| Phone | `PhoneField` |\n| Status | `StatusField` |\n| Tags | `TagsField` |\n| Text | `TextField` |\n| Timeline | `TimelineField` |\n| Mirror | `MirrorField` |\n| Long Text | `LongTextField` |\n\n#### Full Example\n\n```python\nclass ItemExample(Item, monday_client=client, board_id=testing_board_id):\n    status_example = StatusField\n    date_example = DateField\n    checkbox_example = CheckboxField\n    country_example = CountryField\n    email_example = EmailField\n    link_example = LinkField\n    numbers_example = NumberField\n    people_example = PeopleField\n    phone_example = PhoneField\n    tags_example = TagsField\n    text_example = TextField\n    timeline_example = TimelineField\n\tmirror_example = MirrorField\n    long_text_example = LongTextField\n\nitem = ItemExample()\n\n# Setting the values of an item\nitem.item_name = "Aviv Atedgi"\nitem.status_example = "Working on it"\nitem.date_example = datetime.now()\nitem.checkbox_example = True\nitem.country_example = "IL"\nitem.email_example = "aviv.atedgi2000@gmail.com"\nitem.link_example.value.url = "https://www.github.com/avivatedgi"\nitem.link_example.value.text = "My Github Profile"\nitem.link_example = LinkField(url="https://www.google.com", text="Google It")\nitem.numbers_example = 192.4\nitem.people_example = [Person(25200525)]\nitem.phone_example.value.country_code = "IL"\nitem.phone_example.value.phone = "0501234567"\nitem.phone_example = PhoneField(phone="12123123123", country_code="US")\nitem.tags_example = [12808387]\nitem.text_example = "My Cool Text Example"\nitem.timeline_example.value.start = datetime.strptime("2000-05-01", "%Y-%m-%d")\nitem.timeline_example.value.end = datetime.now()\nitem.timeline_example = TimelineField(\n    start=datetime.strptime("2005-04-12", "%Y-%m-%d"),\n    end=datetime.now(),\n)\nitem.long_text_example = "Hello\\nWorld"\n\n# Getting the values of an item\nprint("Status Example =", item.status_example.value)\nprint("Date Example =", item.date_example.value)\nprint("Checkbox Example =", item.checkbox_example.value)\nprint("Country Example =", item.country_example.value)\nprint("Email Example =", item.email_example.value)\nprint("Link Example URL =", item.link_example.value.url)\nprint("Link Example Text =", item.link_example.value.text)\nprint("Numbers Example =", item.numbers_example.value)\nprint("People Example =", item.people_example.value)\nprint("Phone Example Country Code =", item.phone_example.value.country_code)\nprint("Phone Example Phone Number =", item.phone_example.value.phone)\nprint("Tags Example =", item.tags_example.value)\nprint("Text Example =", item.text_example.value)\nprint("Timeline Example Start Date =", item.timeline_example.value.start)\nprint("Timeline Example End Date =", item.timeline_example.value.end)\nprint("Mirror Example = ", item.mirror_example.value)\nprint("Long Text Example = ", item.long_text_example.value)\n```\n\n## Special Thanks\n\n* [Hydration](https://github.com/shustinm/hydration) ([Michael Shustin](https://github.com/shustinm/)) For the idea of the items metaclass\n* [Monday](https://github.com/ProdPerfect/monday) ([ProdPerfect](https://github.com/ProdPerfect)) For the Monday client use in the library\n',
     'author': 'Aviv Atedgi',
     'author_email': 'aviv.atedgi2000@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `monday-item-parser-0.2.8/PKG-INFO` & `monday-item-parser-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monday-item-parser
-Version: 0.2.8
+Version: 0.2.9
 Summary: monday-item-parser is a library used to define Monday items structure in a specific board, and lets the user fetch, create, update and delete items from this board.
 Author: Aviv Atedgi
 Author-email: aviv.atedgi2000@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
@@ -32,14 +32,15 @@
 ## Requirements
 
 * Python >= 3.7
 * [Monday library](https://github.com/ProdPerfect/monday) for the Mondayhttp client
 
 ## Changelog
 
+* 0.2.9 (2022-04-22) - Fixed a bug in Long Text field
 * 0.2.8 (2022-04-22) - Added support for Long Text field
 * 0.2.7 (2022-03-30) - Bumped version because of workflow problems (again :()
 * 0.2.5 (2022-03-30) - Added mirror field to readme.
 * 0.2.4 (2022-03-30) - Added support for mirror (lookup) fields.
 * 0.2.3 (2021-01-16) - Same as 0.2.2, but got some problems with PyPI and Github Workflows again. :(
 * 0.2.2 (2021-01-16) - Added support for [search items by column value](https://api.developer.monday.com/docs/items-by-column-values-queries)
 * 0.2.1 (2021-01-16) - Added hooks for field values.
```

