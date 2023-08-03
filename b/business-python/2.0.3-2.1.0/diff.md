# Comparing `tmp/business-python-2.0.3.tar.gz` & `tmp/business_python-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "business-python-2.0.3.tar", max compression
+gzip compressed data, was "business_python-2.1.0.tar", max compression
```

## Comparing `business-python-2.0.3.tar` & `business_python-2.1.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1067 2021-07-25 07:33:21.453854 business-python-2.0.3/LICENSE
--rw-r--r--   0        0        0     6633 2021-07-25 07:33:21.454281 business-python-2.0.3/README.md
--rw-r--r--   0        0        0      448 2021-08-05 08:15:59.525852 business-python-2.0.3/business/__init__.py
--rw-r--r--   0        0        0    13031 2021-08-05 08:16:04.396186 business-python-2.0.3/business/calendar.py
--rw-r--r--   0        0        0        0 2021-07-26 09:18:51.524548 business-python-2.0.3/business/py.typed
--rw-r--r--   0        0        0     1526 2021-08-05 08:15:59.527981 business-python-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     7656 2021-08-05 08:17:56.719456 business-python-2.0.3/setup.py
--rw-r--r--   0        0        0     7745 2021-08-05 08:17:56.719832 business-python-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2020-04-30 15:05:38.000000 business_python-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6865 2023-08-03 14:24:40.917275 business_python-2.1.0/README.md
+-rw-r--r--   0        0        0      349 2023-08-03 14:24:40.918598 business_python-2.1.0/business/__init__.py
+-rw-r--r--   0        0        0    13031 2023-08-03 14:24:40.920392 business_python-2.1.0/business/calendar.py
+-rw-r--r--   0        0        0        0 2023-08-02 12:38:56.585538 business_python-2.1.0/business/py.typed
+-rw-r--r--   0        0        0     1970 2023-08-03 14:24:40.923998 business_python-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8327 1970-01-01 00:00:00.000000 business_python-2.1.0/PKG-INFO
```

### Comparing `business-python-2.0.3/LICENSE` & `business_python-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `business-python-2.0.3/README.md` & `business_python-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Business (Python)
 
 [![circleci-badge](https://circleci.com/gh/gocardless/business-python.svg?style=shield)](https://app.circleci.com/pipelines/github/gocardless/business-python) [![pypi-badge](https://badge.fury.io/py/business-python.svg)](https://badge.fury.io/py/business-python)
 
-Date calculations based on business calendars. (Python 3.6+)
+Date calculations based on business calendars. (Python 3.8+)
 
 Python implementation of https://github.com/gocardless/business
 
 ## Documentation
 
 To get business, simply:
 
 ```bash
 $ pip install business-python
 ```
 
+## Version 2.1.0 breaking changes
+
+In version 2.1.0 we have dropped support for End-of-Life Python version 3.6 and 3.7. Last release supporting these versions is [v2.0.3](https://github.com/gocardless/business-python/tree/v2.0.3).
+
 ## Version 2.0.0 breaking changes
 
 In version 2.0.0 we have removed the bundled calendars. If you still need these they are available on [v1.0.1](https://github.com/gocardless/business-python/tree/74fe7e4068e0f16b68e7478f8b5ca1cc52f9a7d0/business/data).
 
 ### Migration
 
 - Download/create calendars to a directory within your project eg: `lib/calendars`
@@ -66,15 +70,15 @@
   - 2020-12-26 # Will consider 26 Dec 2020 (A Saturday), a working day
 ```
 
 The `load_cache` method allows a thread safe way to avoid reloading the same calendar multiple times, and provides a performant way to dynamically load calendars for different requests.
 
 #### Using business-python
 
-Define your calendars in a folder eg: `lib/calendars` and set this directory  on `Calendar.load_paths=`
+Define your calendars in a folder eg: `lib/calendars` and set this directory on `Calendar.load_paths=`
 
 ```python
 Calendar.load_paths = ['lib/calendars']
 calendar = Calendar.load_cache("my_calendar")
 ```
 
 ### Input data types
@@ -160,13 +164,14 @@
 The `get_business_day_of_month` method return the running total of business days for a given date in that month. This method counts the number of business days from the start of the first day of the month to the given input date.
 
 ```python
 input_date = Calendar.parse_date("Thursday, 12 June 2014")
 calendar.get_business_day_of_month(input_date)
 # => 9
 ```
+
 ## License & Contributing
 
 - This is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
 - Bug reports and pull requests are welcome on GitHub at https://github.com/gocardless/business-python.
 
 GoCardless ♥ open source. If you do too, come [join us](https://gocardless.com/about/jobs).
```

### Comparing `business-python-2.0.3/business/calendar.py` & `business_python-2.1.0/business/calendar.py`

 * *Files identical despite different names*

### Comparing `business-python-2.0.3/pyproject.toml` & `business_python-2.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,70 @@
 [tool.poetry]
 name = "business-python"
-version = "2.0.3"
+version = "2.1.0"
 description = "Date calculations based on business calendars."
 authors = ["GoCardless <engineering@gocardless.com>"]
 readme = "README.md"
 homepage = "https://github.com/gocardless/business-python"
 repository = "https://github.com/gocardless/business-python"
 packages = [
     { include = "business" },
 ]
 keywords = ["business days", "working days", "calendar", "date"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Office/Business :: Scheduling",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/gocardless/business-python/issues"
+Changelog = "https://github.com/gocardless/business-python/blob/master/CHANGELOG.md"
+Security = "https://github.com/gocardless/business-python/blob/master/SECURITY.md"
+
 [tool.poetry.dependencies]
-python = "^3.6"
-importlib_metadata = { version = ">=1.6.0,<5.0.0", python = "<3.8" }
-python-dateutil = "^2.8.1"
-pyyaml = "^5.1.2"
+python = "^3.8.1"
+python-dateutil = "^2.8.2"
+pyyaml = "^6.0.1"
 
 [tool.poetry.dev-dependencies]
-black = "^20.8b1"
-flake8 = "^3.9.2"
-flake8-docstrings = "^1.6.0"
-flake8-isort = "^4.0.0"
-isort = "^5.8.0"
-mypy = ">=0.770,<1.0.0"
-pytest = "^6.2.3"
-pytest-cov = "^2.12.1"
-toml = "^0.10.0"
-tox = "^3.24.0"
+black = "^23.7.0"
+flake8 = "^6.0.0"
+flake8-docstrings = "^1.7.0"
+flake8-isort = "^6.0.0"
+isort = "^5.12.0"
+keyring = "^24.2.0"
+mypy = "^1.4.1"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+toml = "^0.10.2"
+tox = "^4.6.4"
+types-pyyaml = "^6.0.12.11"
+types-python-dateutil = "^2.8.19.14"
+
+[tool.poetry.group.dev.dependencies]
+types-pyyaml = "^6.0.12.11"
+types-python-dateutil = "^2.8.19.14"
 
 [tool.isort]
 force_grid_wrap = 0
 include_trailing_comma = true
 line_length = 99
 multi_line_output = 3
 use_parentheses = true
 
 [tool.black]
 line-length = 99
-target-version = ['py36']
+target-version = ["py38", "py39", "py310", "py311"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 strict = true
```

### Comparing `business-python-2.0.3/setup.py` & `business_python-2.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,208 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: business-python
+Version: 2.1.0
+Summary: Date calculations based on business calendars.
+Home-page: https://github.com/gocardless/business-python
+Keywords: business days,working days,calendar,date
+Author: GoCardless
+Author-email: engineering@gocardless.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Office/Business :: Scheduling
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Project-URL: Bug Tracker, https://github.com/gocardless/business-python/issues
+Project-URL: Changelog, https://github.com/gocardless/business-python/blob/master/CHANGELOG.md
+Project-URL: Repository, https://github.com/gocardless/business-python
+Project-URL: Security, https://github.com/gocardless/business-python/blob/master/SECURITY.md
+Description-Content-Type: text/markdown
 
-packages = \
-['business']
+# Business (Python)
 
-package_data = \
-{'': ['*']}
+[![circleci-badge](https://circleci.com/gh/gocardless/business-python.svg?style=shield)](https://app.circleci.com/pipelines/github/gocardless/business-python) [![pypi-badge](https://badge.fury.io/py/business-python.svg)](https://badge.fury.io/py/business-python)
 
-install_requires = \
-['python-dateutil>=2.8.1,<3.0.0', 'pyyaml>=5.1.2,<6.0.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib_metadata>=1.6.0,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'business-python',
-    'version': '2.0.3',
-    'description': 'Date calculations based on business calendars.',
-    'long_description': '# Business (Python)\n\n[![circleci-badge](https://circleci.com/gh/gocardless/business-python.svg?style=shield)](https://app.circleci.com/pipelines/github/gocardless/business-python) [![pypi-badge](https://badge.fury.io/py/business-python.svg)](https://badge.fury.io/py/business-python)\n\nDate calculations based on business calendars. (Python 3.6+)\n\nPython implementation of https://github.com/gocardless/business\n\n## Documentation\n\nTo get business, simply:\n\n```bash\n$ pip install business-python\n```\n\n## Version 2.0.0 breaking changes\n\nIn version 2.0.0 we have removed the bundled calendars. If you still need these they are available on [v1.0.1](https://github.com/gocardless/business-python/tree/74fe7e4068e0f16b68e7478f8b5ca1cc52f9a7d0/business/data).\n\n### Migration\n\n- Download/create calendars to a directory within your project eg: `lib/calendars`\n- Change your code to include the `load_path` for your calendars\n- Continue using `.load("my_calendar")` as usual\n\n```python\n# lib/calendars contains yml files\nCalendar.load_paths = [\'lib/calendars\']\ncalendar = Calendar.load("my_calendar")\n```\n\n### Getting started\n\nGet started with business by creating an instance of the calendar class, passing in a hash that specifies which days of the week are considered working days, and which days are holidays.\n\n```python\nfrom business.calendar import Calendar\n\ncalendar = Calendar(\n  working_days=["monday", "tuesday", "wednesday", "thursday", "friday"],\n  # array items are either parseable date strings, or real datetime.date objects\n  holidays=["January 1st, 2020", "April 10th, 2020"],\n  extra_working_dates=[],\n)\n```\n\n`extra_working_dates` key makes the calendar to consider a weekend day as a working day.\n\nIf `working_days` is missing, then common default is used (mon-fri).\nIf `holidays` is missing, "no holidays" assumed.\nIf `extra_working_dates` is missing, then no changes in `working_days` will happen.\n\nElements of `holidays` and `extra_working_dates` may be either strings that `Calendar.parse_date()` can understand, or YYYY-MM-DD (which is considered as a Date by Python YAML itself).\n\n#### Calendar YAML file example\n\n```yaml\n# lib/calendars/my_calendar.yml\nworking_days:\n  - Monday\n  - Sunday\nholidays:\n  - 2017-01-08 # Same as January 8th, 2017\nextra_working_dates:\n  - 2020-12-26 # Will consider 26 Dec 2020 (A Saturday), a working day\n```\n\nThe `load_cache` method allows a thread safe way to avoid reloading the same calendar multiple times, and provides a performant way to dynamically load calendars for different requests.\n\n#### Using business-python\n\nDefine your calendars in a folder eg: `lib/calendars` and set this directory  on `Calendar.load_paths=`\n\n```python\nCalendar.load_paths = [\'lib/calendars\']\ncalendar = Calendar.load_cache("my_calendar")\n```\n\n### Input data types\n\nThe `parse_date` method is used to process the input date(s) in each method and return a `datetime.date` object.\n\n```python\nCalendar.parse_date("2019-01-01")\n# => datetime.date(2019, 1, 1)\n```\n\nSupported data types are:\n\n- `datetime.date`\n- `datetime.datetime`\n- `pandas.Timestamp` (treated as `datetime.datetime`)\n- date string parseable by [`dateutil.parser.parse`](https://dateutil.readthedocs.io/en/stable/parser.html#dateutil.parser.parse)\n\n`numpy.datetime64` is not supported, but can be converted to `datetime.date`:\n\n```python\nnumpy.datetime64(\'2014-06-01T23:00:05.453000000\').astype(\'M8[D]\').astype(\'O\')\n# =>  datetime.date(2014, 6, 1)\n```\n\n### Checking for business days\n\nTo check whether a given date is a business day (falls on one of the specified working days or extra working dates, and is not a holiday), use the `is_business_day` method on `Calendar`.\n\n```python\ncalendar.is_business_day("Monday, 8 June 2020")\n# => true\ncalendar.is_business_day("Sunday, 7 June 2020")\n# => false\n```\n\n### Business day arithmetic\n\n> For our purposes, date-based calculations are sufficient. Supporting time-based calculations as well makes the code significantly more complex. We chose to avoid this extra complexity by sticking solely to date-based mathematics.\n\nThe `add_business_days` method is used to perform business day arithmetic on dates.\n\n```python\ninput_date = Calendar.parse_date("Thursday, 12 June 2014")\ncalendar.add_business_days(input_date, 4).strftime("%A, %d %B %Y")\n# => "Wednesday, 18 June 2014"\ncalendar.add_business_days(input_date, -4).strftime("%A, %d %B %Y")\n# => "Friday, 06 June 2014"\n```\n\nThe `roll_forward` and `roll_backward` methods snap a date to a nearby business day. If provided with a business day, they will return that date. Otherwise, they will advance (forward for `roll_forward` and backward for `roll_backward`) until a business day is found.\n\n```python\ninput_date = Calendar.parse_date("Saturday, 14 June 2014")\ncalendar.roll_forward(input_date).strftime("%A, %d %B %Y")\n# => "Monday, 16 June 2014"\ncalendar.roll_backward(input_date).strftime("%A, %d %B %Y")\n# => "Friday, 13 June 2014"\n```\n\nIn contrast, the `next_business_day` and `previous_business_day` methods will always move to a next or previous date until a business day is found, regardless if the input provided is a business day.\n\n```python\ninput_date = Calendar.parse_date("Monday, 9 June 2014")\ncalendar.roll_forward(input_date).strftime("%A, %d %B %Y")\n# => "Monday, 09 June 2014"\ncalendar.next_business_day(input_date).strftime("%A, %d %B %Y")\n# => "Tuesday, 10 June 2014"\ncalendar.previous_business_day(input_date).strftime("%A, %d %B %Y")\n# => "Friday, 06 June 2014"\n```\n\nTo count the number of business days between two dates, pass the dates to `business_days_between`. This method counts from start of the first date to start of the second date. So, assuming no holidays, there would be two business days between a Monday and a Wednesday.\n\n```python\nfrom datetime import timedelta\n\ninput_date = Calendar.parse_date("Saturday, 14 June 2014")\ncalendar.business_days_between(input_date, input_date + timedelta(days=7))\n# => 5\n```\n\nThe `get_business_day_of_month` method return the running total of business days for a given date in that month. This method counts the number of business days from the start of the first day of the month to the given input date.\n\n```python\ninput_date = Calendar.parse_date("Thursday, 12 June 2014")\ncalendar.get_business_day_of_month(input_date)\n# => 9\n```\n## License & Contributing\n\n- This is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).\n- Bug reports and pull requests are welcome on GitHub at https://github.com/gocardless/business-python.\n\nGoCardless ♥ open source. If you do too, come [join us](https://gocardless.com/about/jobs).\n',
-    'author': 'GoCardless',
-    'author_email': 'engineering@gocardless.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/gocardless/business-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6,<4.0',
-}
+Date calculations based on business calendars. (Python 3.8+)
 
+Python implementation of https://github.com/gocardless/business
+
+## Documentation
+
+To get business, simply:
+
+```bash
+$ pip install business-python
+```
+
+## Version 2.1.0 breaking changes
+
+In version 2.1.0 we have dropped support for End-of-Life Python version 3.6 and 3.7. Last release supporting these versions is [v2.0.3](https://github.com/gocardless/business-python/tree/v2.0.3).
+
+## Version 2.0.0 breaking changes
+
+In version 2.0.0 we have removed the bundled calendars. If you still need these they are available on [v1.0.1](https://github.com/gocardless/business-python/tree/74fe7e4068e0f16b68e7478f8b5ca1cc52f9a7d0/business/data).
+
+### Migration
+
+- Download/create calendars to a directory within your project eg: `lib/calendars`
+- Change your code to include the `load_path` for your calendars
+- Continue using `.load("my_calendar")` as usual
+
+```python
+# lib/calendars contains yml files
+Calendar.load_paths = ['lib/calendars']
+calendar = Calendar.load("my_calendar")
+```
+
+### Getting started
+
+Get started with business by creating an instance of the calendar class, passing in a hash that specifies which days of the week are considered working days, and which days are holidays.
+
+```python
+from business.calendar import Calendar
+
+calendar = Calendar(
+  working_days=["monday", "tuesday", "wednesday", "thursday", "friday"],
+  # array items are either parseable date strings, or real datetime.date objects
+  holidays=["January 1st, 2020", "April 10th, 2020"],
+  extra_working_dates=[],
+)
+```
+
+`extra_working_dates` key makes the calendar to consider a weekend day as a working day.
+
+If `working_days` is missing, then common default is used (mon-fri).
+If `holidays` is missing, "no holidays" assumed.
+If `extra_working_dates` is missing, then no changes in `working_days` will happen.
+
+Elements of `holidays` and `extra_working_dates` may be either strings that `Calendar.parse_date()` can understand, or YYYY-MM-DD (which is considered as a Date by Python YAML itself).
+
+#### Calendar YAML file example
+
+```yaml
+# lib/calendars/my_calendar.yml
+working_days:
+  - Monday
+  - Sunday
+holidays:
+  - 2017-01-08 # Same as January 8th, 2017
+extra_working_dates:
+  - 2020-12-26 # Will consider 26 Dec 2020 (A Saturday), a working day
+```
+
+The `load_cache` method allows a thread safe way to avoid reloading the same calendar multiple times, and provides a performant way to dynamically load calendars for different requests.
+
+#### Using business-python
+
+Define your calendars in a folder eg: `lib/calendars` and set this directory on `Calendar.load_paths=`
+
+```python
+Calendar.load_paths = ['lib/calendars']
+calendar = Calendar.load_cache("my_calendar")
+```
+
+### Input data types
+
+The `parse_date` method is used to process the input date(s) in each method and return a `datetime.date` object.
+
+```python
+Calendar.parse_date("2019-01-01")
+# => datetime.date(2019, 1, 1)
+```
+
+Supported data types are:
+
+- `datetime.date`
+- `datetime.datetime`
+- `pandas.Timestamp` (treated as `datetime.datetime`)
+- date string parseable by [`dateutil.parser.parse`](https://dateutil.readthedocs.io/en/stable/parser.html#dateutil.parser.parse)
+
+`numpy.datetime64` is not supported, but can be converted to `datetime.date`:
+
+```python
+numpy.datetime64('2014-06-01T23:00:05.453000000').astype('M8[D]').astype('O')
+# =>  datetime.date(2014, 6, 1)
+```
+
+### Checking for business days
+
+To check whether a given date is a business day (falls on one of the specified working days or extra working dates, and is not a holiday), use the `is_business_day` method on `Calendar`.
+
+```python
+calendar.is_business_day("Monday, 8 June 2020")
+# => true
+calendar.is_business_day("Sunday, 7 June 2020")
+# => false
+```
+
+### Business day arithmetic
+
+> For our purposes, date-based calculations are sufficient. Supporting time-based calculations as well makes the code significantly more complex. We chose to avoid this extra complexity by sticking solely to date-based mathematics.
+
+The `add_business_days` method is used to perform business day arithmetic on dates.
+
+```python
+input_date = Calendar.parse_date("Thursday, 12 June 2014")
+calendar.add_business_days(input_date, 4).strftime("%A, %d %B %Y")
+# => "Wednesday, 18 June 2014"
+calendar.add_business_days(input_date, -4).strftime("%A, %d %B %Y")
+# => "Friday, 06 June 2014"
+```
+
+The `roll_forward` and `roll_backward` methods snap a date to a nearby business day. If provided with a business day, they will return that date. Otherwise, they will advance (forward for `roll_forward` and backward for `roll_backward`) until a business day is found.
+
+```python
+input_date = Calendar.parse_date("Saturday, 14 June 2014")
+calendar.roll_forward(input_date).strftime("%A, %d %B %Y")
+# => "Monday, 16 June 2014"
+calendar.roll_backward(input_date).strftime("%A, %d %B %Y")
+# => "Friday, 13 June 2014"
+```
+
+In contrast, the `next_business_day` and `previous_business_day` methods will always move to a next or previous date until a business day is found, regardless if the input provided is a business day.
+
+```python
+input_date = Calendar.parse_date("Monday, 9 June 2014")
+calendar.roll_forward(input_date).strftime("%A, %d %B %Y")
+# => "Monday, 09 June 2014"
+calendar.next_business_day(input_date).strftime("%A, %d %B %Y")
+# => "Tuesday, 10 June 2014"
+calendar.previous_business_day(input_date).strftime("%A, %d %B %Y")
+# => "Friday, 06 June 2014"
+```
+
+To count the number of business days between two dates, pass the dates to `business_days_between`. This method counts from start of the first date to start of the second date. So, assuming no holidays, there would be two business days between a Monday and a Wednesday.
+
+```python
+from datetime import timedelta
+
+input_date = Calendar.parse_date("Saturday, 14 June 2014")
+calendar.business_days_between(input_date, input_date + timedelta(days=7))
+# => 5
+```
+
+The `get_business_day_of_month` method return the running total of business days for a given date in that month. This method counts the number of business days from the start of the first day of the month to the given input date.
+
+```python
+input_date = Calendar.parse_date("Thursday, 12 June 2014")
+calendar.get_business_day_of_month(input_date)
+# => 9
+```
+
+## License & Contributing
+
+- This is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
+- Bug reports and pull requests are welcome on GitHub at https://github.com/gocardless/business-python.
+
+GoCardless ♥ open source. If you do too, come [join us](https://gocardless.com/about/jobs).
 
-setup(**setup_kwargs)
```

