# Comparing `tmp/vitya-0.16.0.tar.gz` & `tmp/vitya-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vitya-0.16.0.tar", last modified: Tue May 30 13:40:54 2023, max compression
+gzip compressed data, was "dist/vitya-0.17.0.tar", last modified: Thu Aug  3 15:15:07 2023, max compression
```

## Comparing `vitya-0.16.0.tar` & `vitya-0.17.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-30 13:40:48.000000 vitya-0.16.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-30 13:40:54.000000 vitya-0.16.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-30 13:40:48.000000 vitya-0.16.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 13:40:48.000000 vitya-0.16.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:40:54.000000 vitya-0.16.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-30 13:40:48.000000 vitya-0.16.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-05-30 13:40:48.000000 vitya-0.16.0/tests/test_vitya.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/errors_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya/payment_order/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    28540 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya/payment_order/payments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/payments/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/payments/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/payments/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/payments/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/pydantic_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:15:07.000000 vitya-0.17.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 15:15:03.000000 vitya-0.17.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-08-03 15:15:07.000000 vitya-0.17.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-08-03 15:15:03.000000 vitya-0.17.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 15:15:03.000000 vitya-0.17.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:15:07.000000 vitya-0.17.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-03 15:15:03.000000 vitya-0.17.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:15:07.000000 vitya-0.17.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-03 15:15:03.000000 vitya-0.17.0/tests/test_error_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-08-03 15:15:03.000000 vitya-0.17.0/tests/test_vitya.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:15:07.000000 vitya-0.17.0/vitya/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/error_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/errors_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:15:07.000000 vitya-0.17.0/vitya/payment_order/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/payment_order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/payment_order/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30896 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/payment_order/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/payment_order/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:15:07.000000 vitya-0.17.0/vitya/payment_order/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/payment_order/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/payment_order/payments/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/payment_order/payments/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/payment_order/payments/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/payment_order/payments/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/payment_order/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/pydantic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/typing_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-08-03 15:15:03.000000 vitya-0.17.0/vitya/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:15:07.000000 vitya-0.17.0/vitya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-08-03 15:15:07.000000 vitya-0.17.0/vitya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-03 15:15:07.000000 vitya-0.17.0/vitya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:15:07.000000 vitya-0.17.0/vitya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 15:15:07.000000 vitya-0.17.0/vitya.egg-info/top_level.txt
```

### Comparing `vitya-0.16.0/LICENSE` & `vitya-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vitya-0.16.0/setup.py` & `vitya-0.17.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='vitya',
-    version='0.16.0',
+    version='0.17.0',
     author='hicebank.ru',
     author_email='inyutin@hicebank.ru',
     description='Validators for different russian banking values',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/hicebank/vitya',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     package_data={
         "vitya": ["py.typed"],
     },
 )
```

### Comparing `vitya-0.16.0/tests/test_vitya.py` & `vitya-0.17.0/tests/test_vitya.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,14 @@
     with pytest.raises(PydanticValidationError):
         INNIPModel(inn=inn)
 
 
 @pytest.mark.parametrize(
     'inn', [
         None,  # can't be None
-        '',
         3664069397,  # can't be nothing than str
         302502032671,
         '770708389',  # should be size of 10 or 12 chars
         '77100234440',
         '3664069398',  # wrong checksums
         '302502032672',
         '302502032681'
```

### Comparing `vitya-0.16.0/vitya/errors.py` & `vitya-0.17.0/vitya/errors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 from pydantic.errors import PydanticTypeError, PydanticValueError
 
-from vitya.errors_base import VityaDescribedError
+from vitya.errors_base import (
+    ExactFieldLenError,
+    IncorrectData,
+    IncorrectLen,
+    VityaDescribedError,
+)
 
 
 class OKTMOValidationError(VityaDescribedError, PydanticValueError):
     target = 'oktmo'
     target_ru = 'ОКТМО'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class OKTMOValidationTypeError(OKTMOValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должен быть строкой'
 
 
-class OKTMOValidationValueLenError(OKTMOValidationError):
+class OKTMOValidationValueLenError(OKTMOValidationError, IncorrectLen):
     description = 'must be match 8 or 11 digits'
     description_ru = 'должен состоять из 8 или 11 цифр'
 
 
-class OKTMOValidationValueError(OKTMOValidationError):
+class OKTMOValidationValueError(OKTMOValidationError, IncorrectData):
     description = 'must be match as ([0-9]{11}|[0-9]{8})'
     description_ru = 'должен матчиться с ([0-9]{11}|[0-9]{8})'
 
 
 class INNValidationError(VityaDescribedError, PydanticValueError):
     target = 'inn'
     target_ru = 'ИНН'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
-class INNValidationControlSumError(INNValidationError):
+class INNValidationControlSumError(INNValidationError, IncorrectData):
     description = 'invalid control sum'
     description_ru = 'неверная контрольная сумма'
 
 
-class INNValidationDigitsOnlyError(INNValidationError):
+class INNValidationDigitsOnlyError(INNValidationError, IncorrectData):
     description = 'must contains only digits'
     description_ru = 'может содержать только цифры'
 
 
-class INNValidationLenError(INNValidationError):
+class INNValidationLenError(INNValidationError, IncorrectLen):
     description = 'len must be 5, 10 or 12'
     description_ru = 'длина должна быть 5, 10 или 12 символов'
 
 
 class INNValidationTypeError(INNValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должен быть строкой'
 
 
-class INNValidationStartsWithZerosError(INNValidationError):
+class INNValidationStartsWithZerosError(INNValidationError, IncorrectData):
     description = 'cannot starts with "00"'
     description_ru = 'не может начинаться с "00"'
 
 
 class KPPValidationError(VityaDescribedError, PydanticValueError):
     target = 'kpp'
     target_ru = 'КПП'
@@ -65,25 +70,26 @@
 
 
 class KPPValidationTypeError(KPPValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должно быть строкой'
 
 
-class KPPValidationValueLenError(KPPValidationError):
+class KPPValidationValueLenError(KPPValidationError, ExactFieldLenError):
     description = 'kpp must be 9 chars'
     description_ru = 'должен содержать 9 символов'
+    required_len = 9
 
 
 class KPPValidationValueDigitsOnlyError(KPPValidationError):
     description = 'only digits allowed'
     description_ru = 'должен состоять только из цифр'
 
 
-class KPPValidationValueError(KPPValidationError):
+class KPPValidationValueError(KPPValidationError, IncorrectData):
     description = 'must matches as [0-9]{4}[0-9A-Z]{2}[0-9]{3}'
     description_ru = 'должен матчиться с [0-9]{4}[0-9A-Z]{2}[0-9]{3}'
 
 
 class KPPValidationValueCannotZerosStarts(KPPValidationError):
     description = 'cannot starts with "00"'
     description_ru = 'не может начинаться с "00"'
@@ -97,15 +103,16 @@
 
 
 class BICValidationTypeError(BICValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должен быть строкой'
 
 
-class BICValidationLenError(BICValidationError):
+class BICValidationLenError(BICValidationError, ExactFieldLenError):
     description = 'must be 9 chars'
     description_ru = 'должен содержать 9 символов'
+    required_len = 9
 
 
 class BICValidationValueDigitsOnlyError(BICValidationError):
     description = 'only digits allowed'
     description_ru = 'должен состоять только из чисел'
```

### Comparing `vitya-0.16.0/vitya/payment_order/enums.py` & `vitya-0.17.0/vitya/payment_order/enums.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 from typing import List
 
 
 class AccountKind(str, Enum):
     IP = 'ip'                           # счет ИП
     FL = 'fl'                           # счет ФЛ
     LE = 'le'                           # счет ЮР
+    CHAMELEON = 'chameleon'             # счет Хамелеона
 
 
 class PaymentType(str, Enum):
     FNS = 'fns'                         # бюджетный платеж в ФНС
     CUSTOMS = 'customs'                 # бюджетный платеж в таможню
     BUDGET_OTHER = 'budget_other'       # бюджетный платеж иное
     IP = 'ip'                           # платеж на ИП
     FL = 'fl'                           # платеж на ФЛ
     LE = 'le'                           # платеж на ЮР
+    CHAMELEON = 'chameleon'             # платеж на Хамелеона
 
     @classmethod
     def budget_types(cls) -> List['PaymentType']:
         return [PaymentType.FNS, PaymentType.CUSTOMS, PaymentType.BUDGET_OTHER]
 
     @property
     def is_budget(self) -> bool:
@@ -32,8 +34,9 @@
 _PAYMENT_TYPE_TO_RU = {
     PaymentType.FNS: 'ФНС',
     PaymentType.CUSTOMS: 'Таможня',
     PaymentType.BUDGET_OTHER: 'Иные',
     PaymentType.IP: 'ИП',
     PaymentType.FL: 'ФЛ',
     PaymentType.LE: 'ЮЛ',
+    PaymentType.CHAMELEON: 'Хамелеон',
 }
```

### Comparing `vitya-0.16.0/vitya/payment_order/errors.py` & `vitya-0.17.0/vitya/payment_order/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,374 +4,407 @@
 
 from vitya.errors import (
     INNValidationError,
     INNValidationLenError,
     KPPValidationError,
     OKTMOValidationError,
 )
-from vitya.errors_base import VityaDescribedError
+from vitya.errors_base import (
+    ExactFieldLenError,
+    IncorrectData,
+    IncorrectLen,
+    NeedRequiredField,
+    VityaDescribedError,
+)
 from vitya.payment_order.enums import PaymentType
 from vitya.payment_order.payments.constants import (
-    CHARS_FOR_PURPOSE,
     CUSTOMS_REASONS,
     DOCUMENT_NUMBERS,
     PAYER_STATUSES,
 )
 
 
 class PaymentTypeValueError(VityaDescribedError, PydanticValueError):
     target = 'payment type'
-    target_ru = 'тип платежа'
+    target_ru = 'Тип платежа'
     description = 'неизвестный тип платежа '
     description_ru = 'неизвестный тип платежа '
 
     def __init__(self, payment_type: PaymentType, *args: Any, **kwargs: Any) -> None:  # pragma: no cover
         super().__init__(*args, **kwargs)
         self.description += payment_type.name
         self.description_ru += payment_type.name_ru
 
 
 class AmountValidationError(VityaDescribedError, PydanticValueError):
     target = 'amount'
-    target_ru = 'сумма'
+    target_ru = 'Сумма'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
-class AmountValidationLengthError(AmountValidationError):
+class AmountValidationLengthError(AmountValidationError, IncorrectLen):
     description = 'str representation cannot contains more 18 chars'
     description_ru = 'строковое представление не может содержать более 18 символов'
 
 
-class AmountValidationLessOrEqualZeroError(AmountValidationError):
+class AmountValidationLessOrEqualZeroError(AmountValidationError, IncorrectData):
     description = 'cannot be less than or equal to 0.0'
     description_ru = 'не может быть меньше или равно 0.0'
 
 
-class AmountNotANumber(AmountValidationError):
+class AmountNotANumber(AmountValidationError, IncorrectData):
     description = 'require to be a number'
     description_ru = 'должно быть числом'
 
 
 class CustomerValidationError(VityaDescribedError, PydanticValueError):
     target = 'customer'
-    target_ru = 'плательщик или получатель'
+    target_ru = 'Плательщик или Получатель'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class CustomerValidationSizeError(CustomerValidationError):
     description = 'name must sized from 1 to 160 chars'
     description_ru = 'длина имени должно быть между 1 и 160 символами'
 
 
 class PayerValidationError(CustomerValidationError):
     target = 'payer'
-    target_ru = 'плательщик'
+    target_ru = 'Плательщик'
 
 
-class PayerValidationSizeError(PayerValidationError, CustomerValidationSizeError):
+class PayerValidationSizeError(PayerValidationError, CustomerValidationSizeError, IncorrectLen):
     pass
 
 
-class PayeeValidationError(CustomerValidationError):
-    target = 'payee'
-    target_ru = 'получатель'
+class ReceiverValidationError(CustomerValidationError):
+    target = 'receiver'
+    target_ru = 'Получатель'
 
 
-class PayeeValidationSizeError(PayeeValidationError, CustomerValidationSizeError):
+class ReceiverValidationSizeError(ReceiverValidationError, CustomerValidationSizeError, IncorrectLen):
     pass
 
 
-class PayeeValidationNameError(PayeeValidationError):
+class ReceiverValidationNameError(ReceiverValidationError):
     description = 'contains account number'
     description_ru = 'содержит номер счета'
 
 
-class NumberValidationLenError(VityaDescribedError, PydanticValueError):
+class NumberValidationLenError(PydanticValueError, IncorrectLen):
     target = 'number'
-    target_ru = 'номер'
+    target_ru = 'Номер'
     description = 'cannot be longer than 6 chars'
     description_ru = 'не может быть длиннее 6 символов'
 
 
 class PaymentOrderValidationError(VityaDescribedError, PydanticValueError):
     target = 'payment order'
-    target_ru = 'очередность платежа'
+    target_ru = 'Очередность платежа'
     description = 'value must be in {1, 2, 3, 4, 5}'
     description_ru = 'значение должно быть одним из {1, 2, 3, 4, 5}'
 
 
+class PaymentOrderLenError(PaymentOrderValidationError, ExactFieldLenError):
+    required_len = 1
+
+
 class OperationKindValidationError(VityaDescribedError, PydanticValueError):
     target = 'operation kind'
-    target_ru = 'вид операции'
+    target_ru = 'Вид операции'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class OperationKindValidationTypeError(OperationKindValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должен быть строкой'
 
 
 class OperationKindValidationBudgetValueError(OperationKindValidationError):
     description = 'ior budget must be one of {"01", "02", "06"}'
     description_ru = 'для бюджетных операций значение должно быть одним из {"01", "02", "06"}'
 
 
-class OperationKindValidationValueError(OperationKindValidationBudgetValueError):
+class OperationKindValidationValueError(OperationKindValidationBudgetValueError, ExactFieldLenError):
     description = 'value must be str with len 2'
     description_ru = 'значение должно быть длиной 2 символов'
+    required_len = 2
 
 
 class PurposeCodeValidationError(VityaDescribedError, PydanticValueError):
     target = 'purpose code'
-    target_ru = 'код назначения'
+    target_ru = 'Код назначения'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class PurposeCodeValidationTypeError(PurposeCodeValidationError, PydanticTypeError):
     description = 'must be int'
     description_ru = 'должен быть числом'
 
 
 class PurposeCodeValidationNullError(PurposeCodeValidationError):
     description = 'for non fl payment value must be null'
-    description_ru = 'должен отсутствовать для не ФЛ платежей'
+    description_ru = 'должен отсутствовать для не ФЛ платежей и не хамелеона'
 
 
 class PurposeCodeValidationFlError(PurposeCodeValidationError):
-    description = 'for fl payment value must be in {1, 2, 3, 4, 5}'
-    description_ru = 'для ФЛ платежей должен быть одним из {1, 2, 3, 4, 5}'
+    description = 'for fl payment value must be in {1, 2, 3, 4, 5} or must be empty'
+    description_ru = 'для платежей ФЛ должен быть одним из {1, 2, 3, 4, 5} или быть пустым'
+
+
+class PurposeCodeValidationChameleonError(PurposeCodeValidationError):
+    description = 'for chameleon payment value must be in {1, 2, 3, 4, 5} or must be empty'
+    description_ru = 'для платежей хамелеону должен быть одним из {1, 2, 3, 4, 5} или быть пустым'
 
 
 class UINValidationError(VityaDescribedError, PydanticValueError):
     target = 'uin'
     target_ru = 'УИН'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class UINValidationTypeError(UINValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должен быть строкой'
 
 
-class UINValidationLenError(UINValidationError):
+class UINValidationLenError(UINValidationError, IncorrectLen):
     description = 'len must be 4, 20 or 25 len'
     description_ru = 'длина должна быть 4, 20 или 25 символов'
 
 
-class UINValidationDigitsOnlyError(UINValidationError):
+class UINValidationDigitsOnlyError(UINValidationError, IncorrectData):
     description = 'must contains only digits'
     description_ru = 'должен содержать только числа'
 
 
-class UINValidationControlSumError(UINValidationError):
+class UINValidationControlSumError(UINValidationError, IncorrectData):
     description = 'control sum error'
     description_ru = 'некорректная контрольная сумма'
 
 
-class UINValidationValueZeroError(UINValidationError):
+class UINValidationValueZeroError(UINValidationError, NeedRequiredField):
     description = 'value cannot be zero'
     description_ru = 'значение не может быть нулем'
 
 
 class UINValidationBOLenError(UINValidationLenError):
     description = 'len uin for bo payment must be 4, 20 or 25 len'
     description_ru = 'длина для платежей с типом иные должна быть 4, 30 или 25'
 
 
 class UINValidationFNSValueError(UINValidationError):
     description = 'FNS base error'
     description_ru = 'базовая ФНС ошибка'
 
 
-class UINValidationFNSValueZeroError(UINValidationFNSValueError):
+class UINValidationFNSValueZeroError(UINValidationFNSValueError, NeedRequiredField):
     description = (
         'for FNS with payer status = "13" and empty inn uin must be non zero'
     )
     description_ru = (
         'для платежей в ФНС со статусом плательщика "13" и пустым ИНН, УИН должен быть не нулевым'
     )
 
 
-class UINValidationFNSNotValueZeroError(UINValidationFNSValueError):
+class UINValidationFNSNotValueZeroError(UINValidationFNSValueError, IncorrectData):
     description = 'for FNS with payer status = "02" uin must be zero'
     description_ru = 'для платежей в ФНС со статусом плательщика "02" и пустым ИНН, УИН должен быть нулевым'
 
 
-class UINValidationBONotEmpty(UINValidationFNSValueError):
-    description = 'for budget other and payee number starting with 03212 uin must be filled'
+class UINValidationBONotEmpty(UINValidationFNSValueError, NeedRequiredField):
+    description = 'for budget other and receiver number starting with 03212 uin must be filled'
     description_ru = (
         'для платежей в бюджет иные с номером счёта получателя, который начинается с "03212", УИН должен быть заполен'
     )
 
 
 class UINValidationFNSLenError(UINValidationLenError):
     description = 'invalid uin: len uin for FNS payment must be 20 or 25 len'
     description_ru = 'длина УИН для платежей в ФНС должна быть 20 или 15 символов'
 
 
-class UINValidationOnlyZeroError(UINValidationError):
+class UINValidationOnlyZeroError(UINValidationError, IncorrectData):
     description = 'cannot contains only 0 chars'
     description_ru = 'не может состоять только из нулей'
 
 
 class PurposeValidationError(VityaDescribedError, PydanticValueError):
     target = 'purpose'
-    target_ru = 'назначение'
+    target_ru = 'Назначение'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class PurposeValidationTypeError(PurposeValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должно быть строкой'
 
 
-class PurposeValidationMaxLenError(PurposeValidationError):
+class PurposeValidationMaxLenError(PurposeValidationError, IncorrectLen):
     description = 'len can be from 1 to 210 chars'
     description_ru = 'длина должна быть от 1 до 210 символов'
 
 
-class PurposeValidationCharactersError(PurposeValidationError):
-    description = f'can only consist of {CHARS_FOR_PURPOSE}'
-    description_ru = f'может состоять только из символов {CHARS_FOR_PURPOSE}'
-
-
-class PurposeValidationIPNDSError(PurposeValidationError):
+class PurposeValidationIPNDSError(PurposeValidationError, IncorrectData):
     description = 'for IP payment purpose must contains "НДС"'
     description_ru = 'для платежей ИП назначение должно содержать "НДС"'
 
 
 class PayerINNValidationError(INNValidationError):
     target = 'payer inn'
     target_ru = 'ИНН плательщика'
 
 
-class PayerINNValidationCustomsLen10Error(INNValidationLenError, PayerINNValidationError):
+class PayerINNValidationCustomsLen10Error(INNValidationLenError, PayerINNValidationError, ExactFieldLenError):
     description = 'for customs payment and payer status "06", inn must be 10'
-    description_ru = 'для платежей в таможню и со статусом плательщика "06" ИНН должно быть "10"'
+    description_ru = 'для платежей в таможню и со статусом плательщика "06" ИНН должно быть быть длиной 10 символов'
+    required_len = 10
 
 
-class PayerINNValidationCustomsLen12Error(INNValidationLenError, PayerINNValidationError):
+class PayerINNValidationCustomsLen12Error(INNValidationLenError, PayerINNValidationError, ExactFieldLenError):
     description = 'for customs payment and payer status 16 or 17, inn must be 12'
-    description_ru = 'для платежей таможню со статусом плательщика "16" или "17", значение ИНН должно быть "12"'
+    description_ru = (
+        'для платежей таможню со статусом плательщика "16" или "17",'
+        ' значение ИНН должно быть длиной 12 символов'
+    )
+    required_len = 12
 
 
-class PayerINNValidationEmptyNotAllowedError(PayerINNValidationError):
+class PayerINNValidationEmptyNotAllowedError(PayerINNValidationError, NeedRequiredField):
     description = 'inn cannot be empty'
     description_ru = 'не может быть пустым'
 
 
-class PayerINNValidationStartWithZerosError(PayerINNValidationError):
+class PayerINNValidationStartWithZerosError(PayerINNValidationError, IncorrectData):
     description = 'cannot start with "00"'
     description_ru = 'не может начинаться с "00"'
 
 
-class PayerINNValidationFiveOnlyZerosError(PayerINNValidationError):
-    description = 'inn with len 5 cannot be contains only zeros'
-    description_ru = 'ИНН с длиной 5 символов не может содержать только нули'
-
-
-class PayeeINNValidationError(INNValidationError):
-    target = 'payee inn'
+class ReceiverINNValidationError(INNValidationError):
+    target = 'receiver inn'
     target_ru = 'ИНН получателя'
 
 
-class PayeeINNValidationNonEmptyError(PayeeINNValidationError):
+class ReceiverINNValidationNonEmptyError(ReceiverINNValidationError):
     description = 'cannot be empty'
     description_ru = 'не может быть пустым'
 
 
-class PayeeINNValidationFLenError(INNValidationLenError, PayeeINNValidationError):
-    description = 'for fl payee inn must be 12'
+class ReceiverINNValidationFLenError(INNValidationLenError, ReceiverINNValidationError):
+    description = 'for fl receiver inn must be 12'
     description_ru = 'для платежей ИП ИНН получателя должно быть длиной 12 символов'
 
 
-class PayeeINNValidationFLLenError(INNValidationLenError, PayeeINNValidationError):
-    description = 'for fl payee inn must be empty or 12 chars'
+class ReceiverINNValidationFLLenError(INNValidationLenError, ReceiverINNValidationError):
+    description = 'for fl receiver inn must be empty or 12 chars'
     description_ru = 'для платежей ИП ИНН получателя должно быть пустым или содержать 12 символов'
 
 
-class PayeeINNValidationIPLenError(PayeeINNValidationError):
-    description = 'for ip payee inn must be 12'
+class ReceiverINNValidationChameleonLenError(INNValidationLenError, ReceiverINNValidationError):
+    description = 'for chameleon receiver inn must be empty or 12 or 10 chars'
+    description_ru = 'для платежей Хамелеону ИНН получателя должно быть пустым или содержать 12 или 10 символов'
+
+
+class ReceiverINNValidationIPLenError(ReceiverINNValidationError):
+    description = 'for ip receiver inn must be 12'
     description_ru = 'для платежей ИП ИНН получателя должно быть 12 символов'
 
 
-class PayeeINNValidationLELenError(PayeeINNValidationError):
+class ReceiverINNValidationLELenError(ReceiverINNValidationError):
     description = 'for fns, customs, bo and le inn must be 10'
     description_ru = 'для платежей в бюджет и платежей ЮЛ, ИНН должно быть 10 символов'
 
 
-class PayerAccountValidationError(VityaDescribedError, PydanticValueError):
-    target = 'payer account'
-    target_ru = 'счет плательщика'
-    description = 'base error'
-    description_ru = 'базовая ошибка'
-
-
-class PayeeAccountValidationError(VityaDescribedError, PydanticValueError):
-    target = 'payee account'
-    target_ru = 'счет получателя'
+class ReceiverAccountValidationError(VityaDescribedError, PydanticValueError):
+    target = 'receiver account'
+    target_ru = 'Счет получателя'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
-class PayeeAccountValidationNonEmptyError(PayeeAccountValidationError):
+class ReceiverAccountValidationNonEmptyError(ReceiverAccountValidationError):
     description = 'cannot be empty'
     description_ru = 'не может быть пустым'
 
 
-class PayeeAccountValidationLenError(PayeeAccountValidationError):
+class ReceiverAccountValidationLenError(ReceiverAccountValidationError):
     description = 'must be 20 digits'
     description_ru = 'должен состоять из 20 цифр'
 
 
-class PayeeAccountValidationFNSValueError(PayeeAccountValidationError):
+class ReceiverAccountValidationFNSValueError(ReceiverAccountValidationError):
     description = 'for FNS payment account must be "03100643000000018500"'
     description_ru = 'для платежей в ФНС счет должен быть "03100643000000018500"'
 
 
 class AccountNumberValidationError(VityaDescribedError, PydanticValueError):
     target = 'account number'
-    target_ru = 'номер счета'
+    target_ru = 'Номер счета'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class AccountNumberValidationTypeError(AccountNumberValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должен быть строкой'
 
 
-class AccountNumberValidationSizeError(AccountNumberValidationError):
+class AccountNumberValidationSizeError(AccountNumberValidationError, ExactFieldLenError):
     description = 'must consist of 20 chars'
     description_ru = 'должен состоять из 20 символов'
+    required_len = 20
 
 
 class AccountNumberValidationDigitsOnlyError(AccountNumberValidationError):
     description = 'must be only digits'
     description_ru = 'должен состоять только из цифр'
 
 
 class AccountValidationBICValueError(AccountNumberValidationError):
     description = 'account is not valid for bic'
     description_ru = 'не ключуется с БИКом'
 
 
-class PayeeAccountValidationBICValueError(AccountValidationBICValueError, PayeeAccountValidationError):
+class ReceiverAccountNumberValidationTypeError(
+    ReceiverAccountValidationError,
+    AccountNumberValidationTypeError,
+):
+    pass
+
+
+class ReceiverAccountNumberValidationSizeError(
+    ReceiverAccountValidationError,
+    AccountNumberValidationSizeError,
+):
+    pass
+
+
+class ReceiverAccountNumberValidationDigitsOnlyError(
+    ReceiverAccountValidationError,
+    AccountNumberValidationDigitsOnlyError,
+):
+    pass
+
+
+class ReceiverAccountValidationBICValueError(
+    ReceiverAccountValidationError,
+    AccountValidationBICValueError,
+):
     pass
 
 
 class PayerStatusValidationError(VityaDescribedError, PydanticValueError):
     target = 'payer status'
-    target_ru = 'статус плательщика'
+    target_ru = 'Статус плательщика'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class PayerStatusValidationTypeError(PayerStatusValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должен быть строкой'
@@ -383,15 +416,15 @@
 
 
 class PayerStatusValidationNullNotAllowedError(PayerStatusValidationError):
     description = 'for budget payments empty value is not allowed'
     description_ru = 'для платежей в бюджет значение не должно быть пустым'
 
 
-class PayerStatusValidationCustoms05NotAllowedError(PayerStatusValidationError):
+class PayerStatusValidationCustoms05NotAllowedError(PayerStatusValidationError, IncorrectData):
     description = 'for customs payment and for_third_face = true value "06" not allowed'
     description_ru = 'для платежей в таможню и для платежей за третьих лиц значение статуса не может быть "06"'
 
 
 class KPPValidationOnlyEmptyError(KPPValidationError):
     description = 'only empty is allowed'
     description_ru = 'должно быть пустым'
@@ -410,113 +443,114 @@
 
 
 class PayerKPPValidationOnlyEmptyError(PayerKPPValidationError, KPPValidationOnlyEmptyError):
     description = 'for ip, fl or le value must be empty'
     description_ru = 'для платежей ИП, ФЛ, И ЮЛ значение должно быть пустым'
 
 
-class PayerKPPValidationINN10EmptyNotAllowed(PayerKPPValidationError, KPPValidationEmptyNotAllowed):
+class PayerKPPValidationINN10EmptyNotAllowed(PayerKPPValidationError, KPPValidationEmptyNotAllowed, NeedRequiredField):
     description = 'for budget payment with inn length 10 kpp empty value is not allowed'
     description_ru = 'для платежей в бюджет с длиной ИНН равной 10 значение КПП должно быть заполнено'
 
 
-class PayerKPPValidationINN12OnlyEmptyError(PayerKPPValidationOnlyEmptyError):
+class PayerKPPValidationINN12OnlyEmptyError(PayerKPPValidationOnlyEmptyError, IncorrectData):
     description = 'for budget with inn length 12 kpp only empty allowed'
     description_ru = 'для платежей в бюджет с длиной ИНН равной 12 значение КПП должно быть пустым'
 
 
-class PayeeKPPValidationError(KPPValidationError):
-    target = 'payee kpp'
+class ReceiverKPPValidationError(KPPValidationError):
+    target = 'receiver kpp'
     target_ru = 'КПП получателя'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
-class PayeeKPPValidationOnlyEmptyError(PayeeKPPValidationError, KPPValidationOnlyEmptyError):
+class ReceiverKPPValidationOnlyEmptyError(ReceiverKPPValidationError, KPPValidationOnlyEmptyError):
     description = 'for ip or fl only empty allowed'
     description_ru = 'для платежей ИП и ФЛ значение должно быть пустым'
 
 
-class PayeeKPPValidationEmptyNotAllowed(PayeeKPPValidationError, KPPValidationEmptyNotAllowed):
-    description = 'for fns, customs, budget other or le empty value is not allowed'
-    description_ru = 'для платежей в бюджет или платежей ЮЛ пустое значение недопустимо'
+class ReceiverKPPValidationEmptyNotAllowed(ReceiverKPPValidationError, KPPValidationEmptyNotAllowed):
+    description = 'for fns, customs, budget other empty value is not allowed'
+    description_ru = 'для платежей в бюджет пустое значение недопустимо'
 
 
-class PayeeKPPValidationStartsWithZeros(PayeeKPPValidationError):
-    description = 'for fns, customs, budget other or le kpp cannot starts with "00"'
-    description_ru = 'для платежей в бюджет или платежей ЮЛ значение не может начинаться с "00"'
+class ReceiverKPPValidationStartsWithZeros(ReceiverKPPValidationError):
+    description = 'for fns, customs, budget other kpp cannot starts with "00"'
+    description_ru = 'для платежей в бюджет значение не может начинаться с "00"'
 
 
 class CBCValidationError(VityaDescribedError, PydanticValueError):
     target = 'CBC'
     target_ru = 'КБК'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class CBCValidationTypeError(CBCValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должен быть строкой'
 
 
-class CBCValidationEmptyNotAllowed(CBCValidationError):
+class CBCValidationEmptyNotAllowed(CBCValidationError, NeedRequiredField):
     description = 'for fns or customs empty value is not allowed'
     description_ru = 'для платежей в ФНС или таможню значение не должно быть пустым'
 
 
-class CBCValidationValueLenError(CBCValidationError):
+class CBCValidationValueLenError(CBCValidationError, ExactFieldLenError):
     description = 'must be 20 digits'
     description_ru = 'должен состоять из 20 цифр'
+    required_len = 20
 
 
-class CBCValidationValueDigitsOnlyError(CBCValidationError):
+class CBCValidationValueDigitsOnlyError(CBCValidationError, IncorrectData):
     description = 'only digits are allowed'
     description_ru = 'должен состоять только из цифр'
 
 
-class CBCValidationValueCannotZerosOnly(CBCValidationError):
+class CBCValidationValueCannotZerosOnly(CBCValidationError, IncorrectData):
     description = 'cannot contain only zeros'
     description_ru = 'не может состоять только из нулей'
 
 
 class OKTMOValidationEmptyNotAllowed(OKTMOValidationError):
     target = 'oktmo'
     target_ru = 'ОКТМО'
     description = 'empty value is not allowed'
     description_ru = 'значение не должно быть пустым'
 
 
-class OKTMOValidationFNSEmptyNotAllowed(OKTMOValidationEmptyNotAllowed):
+class OKTMOValidationFNSEmptyNotAllowed(OKTMOValidationEmptyNotAllowed, NeedRequiredField):
     description = 'invalid oktmo: for fns with payer status = "02" empty value is not allowed'
     description_ru = 'для платежей в фнс со статусом плательщика "02" значение не может быть пустым'
 
 
 class OKTMOValidationZerosNotAllowed(OKTMOValidationError):
     description = 'cannot be all zeros'
     description_ru = 'не может состоять полностью из нулей'
 
 
 class ReasonValidationError(VityaDescribedError, PydanticValueError):
     target = 'reason'
-    target_ru = 'основание платежа'
+    target_ru = 'Основание платежа'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class ReasonValidationTypeError(ReasonValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должно быть строкой'
 
 
-class ReasonValidationValueLenError(ReasonValidationError):
+class ReasonValidationValueLenError(ReasonValidationError, IncorrectLen):
     description = 'must be 2 chars'
     description_ru = 'должно состоять из 2 символов'
 
 
-class ReasonValidationValueErrorCustoms(ReasonValidationError):
+class ReasonValidationValueErrorCustoms(ReasonValidationError, IncorrectData):
     description = f'for customs payment value must be in {CUSTOMS_REASONS}'
     description_ru = f'для платежей в таможню значение должно быть одним из {CUSTOMS_REASONS}'
 
 
 class TaxPeriodValidationError(VityaDescribedError, PydanticValueError):
     target = 'tax period'
     target_ru = 'Периодичность платежа / Код таможенного органа'
@@ -535,51 +569,53 @@
 
 
 class TaxPeriodValidationValueLenError(TaxPeriodValidationError):
     description = 'invalid len'
     description_ru = 'некорректная длина'
 
 
-class TaxPeriodValidationBOValueLenError(TaxPeriodValidationValueLenError):
+class TaxPeriodValidationBOValueLenError(TaxPeriodValidationValueLenError, IncorrectLen):
     description = 'for bo must be 10'
     description_ru = 'для иных платежей в бюджет длина должны быть равна 10'
 
 
-class TaxPeriodValidationCustomsEmptyNotAllowed(TaxPeriodValidationEmptyNotAllowed):
+class TaxPeriodValidationCustomsEmptyNotAllowed(TaxPeriodValidationEmptyNotAllowed, NeedRequiredField):
     pass
 
 
-class TaxPeriodValidationCustomsValueLenError(TaxPeriodValidationValueLenError):
+class TaxPeriodValidationCustomsValueLenError(TaxPeriodValidationValueLenError, ExactFieldLenError):
     description = 'for customs len must be 8'
     description_ru = 'для платежей в таможню длина должна быть 8 символов'
+    required_len = 8
 
 
 class TaxPeriodValidationFNS02EmptyNotAllowed(TaxPeriodValidationError):
     description = 'for fns with payer status = "02" empty is not allowed'
     description_ru = 'для платежей в ФНС со статусом плательщика "02" пустое значение недопустимо'
 
 
-class TaxPeriodValidationFNS01OnlyEmpty(TaxPeriodValidationError):
+class TaxPeriodValidationFNS01OnlyEmpty(TaxPeriodValidationError, IncorrectData):
     description = 'for fns with payer status = "01" or "13" only empty allowed'
     description_ru = 'для платежей в ФНС со статусом плательщика "01" или "13" значение должно быть пустым'
 
 
-class TaxPeriodValidationFNSEmptyNotAllowed(TaxPeriodValidationEmptyNotAllowed):
+class TaxPeriodValidationFNSEmptyNotAllowed(TaxPeriodValidationEmptyNotAllowed, NeedRequiredField):
     description = 'for fns empty is not allowed'
     description_ru = 'для платежей в ФНС пустое значение недопустимо'
 
 
-class TaxPeriodValidationFNSValueLenError(TaxPeriodValidationValueLenError):
+class TaxPeriodValidationFNSValueLenError(TaxPeriodValidationValueLenError, ExactFieldLenError):
     description = 'for fns len must be 10 chars'
     description_ru = 'для платежей в ФНС длина значения должна быть 10 символов'
+    required_len = 10
 
 
 class DocumentNumberValidationError(VityaDescribedError, PydanticValueError):
     target = 'document number'
-    target_ru = 'номер документа'
+    target_ru = 'Номер документа'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class DocumentNumberValidationTypeError(DocumentNumberValidationError, PydanticTypeError):
     description = 'must be a str'
     description_ru = 'должен быть строкой'
@@ -603,17 +639,26 @@
 class DocumentNumberValidationBOEmptyNotAllowed(DocumentNumberValidationEmptyNotAllowed):
     description = 'for bo with payer status = "24", empty payer inn and empty uin empty is not allowed'
     description_ru = (
         'для иных платежей в бюджет со статусом плательщика "24", пустое значение ИНН плательщика и УИН недопустимо'
     )
 
 
-class DocumentNumberValidationBOOnlyEmptyError(DocumentNumberValidationOnlyEmptyError):
+class DocumentNumberValidationBOPayerStatus33OnlyEmptyError(DocumentNumberValidationOnlyEmptyError, IncorrectData):
     description = (
-        'for bo with payee account starts with "03212",'
+        'for bo with payer status = "33" , must be empty'
+    )
+    description_ru = (
+        'для иных платежей в бюджет со статусом плательщика = «33» поле документ должно быть обязательно пустым'
+    )
+
+
+class DocumentNumberValidationBOOnlyEmptyError(DocumentNumberValidationOnlyEmptyError, IncorrectData):
+    description = (
+        'for bo with receiver account starts with "03212",'
         ' payer status = "31", uin is not empty - empty value is not allowed'
     )
     description_ru = (
         'для иных платежей в бюджет счет получателя должен начинаться с "03212",'
         ' статус плательщика должен быть "31, а УИН быть заполнен'
     )
 
@@ -622,58 +667,66 @@
     description = f'for bo first two chars should be in {DOCUMENT_NUMBERS}, and third is equal to ";"'
     description_ru = (
         f'для иных платежей в бюджет первые два символы должны быть в {DOCUMENT_NUMBERS},'
         f' а третий символ должен быть равен ";"'
     )
 
 
-class DocumentNumberValidationBOValueLenError(DocumentNumberValidationError):
+class DocumentNumberValidationBOValueLenError(DocumentNumberValidationError, IncorrectLen):
     description = 'for bo value len max 15'
     description_ru = 'для иных платежей в бюджет максимальная длина должна быть равна 15'
 
 
 class DocumentNumberValidationCustoms00ValueError(DocumentNumberValidationError):
     description = 'for customs with reason = "00" value must starts with "00"'
     description_ru = 'для платежей в таможню основание платежа должно быть равно "00", а номер должен начинаться с "00"'
 
 
-class DocumentNumberValidationCustomsValueLen7Error(DocumentNumberValidationError):
+class DocumentNumberValidationCustomsValueLen7Error(DocumentNumberValidationError, IncorrectLen):
     description = 'for customs with reason in {"ПК", "УВ", "ТГ", "ТБ", "ТД", "ПВ"} value len max 7'
     description_ru = (
         'для платежей в таможню с основанием платежа в {"ПК", "УВ", "ТГ", "ТБ", "ТД", "ПВ"}'
         ' длина значения должна быть не более 7 символов'
     )
 
 
-class DocumentNumberValidationCustomsValueLen15Error(DocumentNumberValidationError):
+class DocumentNumberValidationCustomsValueLen15Error(DocumentNumberValidationError, IncorrectLen):
     description = 'for customs with reason in {"ИЛ", "ИН", "ПБ", "КЭ"} value len from 1 to 15 chars'
     description_ru = (
         'для платежей в таможню с основанием платежа в {"ИЛ", "ИН", "ПБ", "КЭ"}'
         ' длина значения должна быть от 1 до 15 символов'
     )
 
 
 class DocumentDateValidationError(VityaDescribedError, PydanticValueError):
     target = 'document date'
-    target_ru = 'дата документа'
+    target_ru = 'Дата документа'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class DocumentDateValidationTypeError(DocumentDateValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должна быть строкой'
 
 
 class DocumentDateValidationFNSOnlyEmptyError(DocumentDateValidationError):
     description = 'for fns only empty allowed'
     description_ru = 'для платежей в ФНС значение должно быть пустым'
 
 
-class DocumentDateValidationCustomsLenError(DocumentDateValidationError):
+class DocumentDateValidationCustomsLenError(DocumentDateValidationError, ExactFieldLenError):
     description = 'for customs value must be equal 10 chars'
     description_ru = 'для платежей в таможню длина значения должна быть 10 символов'
+    required_len = 10
 
 
-class DocumentDateValidationBOLenError(DocumentDateValidationError):
+class DocumentDateValidationBOLenError(DocumentDateValidationError, IncorrectLen):
     description = 'for bo value max 10 chars'
     description_ru = 'для иных платежей в бюджет значение не должно быть длиннее 10 символов'
+
+
+class BudgetPaymentForThirdPersonError(VityaDescribedError, PydanticValueError):
+    target = None
+    target_ru = None
+    description = 'budget payment can not for third person'
+    description_ru = 'платеж в бюджет не может быть за третье лицо'
```

### Comparing `vitya-0.16.0/vitya/payment_order/fields.py` & `vitya-0.17.0/vitya/payment_order/fields.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,25 +6,26 @@
     validate_amount,
     validate_cbc,
     validate_customer,
     validate_document_date,
     validate_document_number,
     validate_number,
     validate_operation_kind,
-    validate_payee,
     validate_payer,
     validate_payer_status,
     validate_payment_order,
     validate_purpose,
     validate_purpose_code,
     validate_reason,
+    validate_receiver,
+    validate_receiver_account_number,
     validate_tax_period,
     validate_uin,
 )
-from vitya.pydantic_fields import FieldMixin
+from vitya.pydantic_fields import BIC, INN, KPP, BoolWrapper, FieldMixin
 
 CallableGenerator = Generator[Callable[..., Any], None, None]
 
 
 class Number(FieldMixin, str):
     """Номер платёжного поручения (3)"""
 
@@ -53,20 +54,20 @@
     """Плательщик (8)"""
 
     @classmethod
     def _validate(cls, value: str) -> str:
         return validate_payer(value)
 
 
-class Payee(Customer):
+class Receiver(Customer):
     """Наименование получателя (16)"""
 
     @classmethod
     def _validate(cls, value: str) -> str:
-        return validate_payee(value)
+        return validate_receiver(value)
 
 
 class PaymentOrder(FieldMixin, int):
     """Очерёдность платежа (21)"""
 
     @classmethod
     def _validate(cls, value: str) -> int:
@@ -77,14 +78,26 @@
     """Счёт"""
 
     @classmethod
     def _validate(cls, value: str) -> str:
         return validate_account_number(value)
 
 
+class ReceiverAccountNumber(AccountNumber):
+    """Счет получателя (17)"""
+
+    @classmethod
+    def _validate(cls, value: str) -> str:
+        return validate_receiver_account_number(value)
+
+
+class PayerAccountNumber(AccountNumber):
+    """Номер счёта плательщика (9)"""
+
+
 class OperationKind(FieldMixin, str):
     """Вид операции (18)"""
 
     @classmethod
     def _validate(cls, value: str) -> str:
         return validate_operation_kind(value)
 
@@ -109,14 +122,34 @@
     """Назначение платежа (24)"""
 
     @classmethod
     def _validate(cls, value: str) -> str:
         return validate_purpose(value)
 
 
+class PayerINN(INN):
+    """ИНН плательщика (60)"""
+
+
+class ReceiverINN(INN):
+    """ИНН получателя (61)"""
+
+
+class ReceiverBIC(BIC):
+    """БИК банка получателя (14)"""
+
+
+class ReceiverKPP(KPP):
+    """КПП плательщика (103)"""
+
+
+class PayerKPP(KPP):
+    """КПП получателя (102)"""
+
+
 class PayerStatus(FieldMixin, str):
     """Статус плательщика (101)"""
 
     @classmethod
     def _validate(cls, value: str) -> str:
         return validate_payer_status(value)
 
@@ -155,7 +188,11 @@
 
 class DocumentDate(FieldMixin, str):
     """Дата документа (109)"""
 
     @classmethod
     def _validate(cls, value: str) -> Optional[str]:
         return validate_document_date(value)
+
+
+class ForThirdPerson(BoolWrapper):
+    pass
```

### Comparing `vitya-0.16.0/vitya/payment_order/payments/checks.py` & `vitya-0.17.0/vitya/payment_order/payments/checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 import re
 from typing import Optional
 
 from vitya.payment_order.enums import AccountKind, PaymentType
 from vitya.payment_order.errors import (
     AccountValidationBICValueError,
+    BudgetPaymentForThirdPersonError,
     CBCValidationEmptyNotAllowed,
     DocumentDateValidationBOLenError,
     DocumentDateValidationCustomsLenError,
     DocumentDateValidationFNSOnlyEmptyError,
     DocumentNumberValidationBOEmptyNotAllowed,
     DocumentNumberValidationBOOnlyEmptyError,
+    DocumentNumberValidationBOPayerStatus33OnlyEmptyError,
     DocumentNumberValidationBOValueError,
     DocumentNumberValidationBOValueLenError,
     DocumentNumberValidationCustoms00ValueError,
     DocumentNumberValidationCustomsValueLen7Error,
     DocumentNumberValidationCustomsValueLen15Error,
     DocumentNumberValidationFNSOnlyEmptyError,
     OKTMOValidationEmptyNotAllowed,
     OKTMOValidationFNSEmptyNotAllowed,
     OKTMOValidationZerosNotAllowed,
     OperationKindValidationBudgetValueError,
-    PayeeAccountValidationBICValueError,
-    PayeeAccountValidationFNSValueError,
-    PayeeINNValidationFLLenError,
-    PayeeINNValidationIPLenError,
-    PayeeINNValidationLELenError,
-    PayeeINNValidationNonEmptyError,
-    PayeeKPPValidationEmptyNotAllowed,
-    PayeeKPPValidationOnlyEmptyError,
-    PayeeKPPValidationStartsWithZeros,
     PayerINNValidationCustomsLen10Error,
     PayerINNValidationCustomsLen12Error,
     PayerINNValidationEmptyNotAllowedError,
     PayerINNValidationStartWithZerosError,
     PayerKPPValidationINN10EmptyNotAllowed,
     PayerKPPValidationINN12OnlyEmptyError,
     PayerStatusValidationCustoms05NotAllowedError,
     PayerStatusValidationNullNotAllowedError,
     PaymentTypeValueError,
+    PurposeCodeValidationChameleonError,
     PurposeCodeValidationFlError,
     PurposeCodeValidationNullError,
     PurposeValidationIPNDSError,
     ReasonValidationValueErrorCustoms,
+    ReceiverAccountValidationBICValueError,
+    ReceiverAccountValidationFNSValueError,
+    ReceiverINNValidationChameleonLenError,
+    ReceiverINNValidationFLLenError,
+    ReceiverINNValidationIPLenError,
+    ReceiverINNValidationLELenError,
+    ReceiverINNValidationNonEmptyError,
+    ReceiverKPPValidationEmptyNotAllowed,
+    ReceiverKPPValidationOnlyEmptyError,
+    ReceiverKPPValidationStartsWithZeros,
     TaxPeriodValidationBOValueLenError,
     TaxPeriodValidationCustomsEmptyNotAllowed,
     TaxPeriodValidationCustomsValueLenError,
     TaxPeriodValidationFNS01OnlyEmpty,
     TaxPeriodValidationFNS02EmptyNotAllowed,
     TaxPeriodValidationFNSEmptyNotAllowed,
     TaxPeriodValidationFNSValueLenError,
@@ -56,95 +60,104 @@
 )
 from vitya.payment_order.fields import (
     CBC,
     UIN,
     AccountNumber,
     DocumentDate,
     DocumentNumber,
+    ForThirdPerson,
     OperationKind,
+    PayerAccountNumber,
+    PayerINN,
+    PayerKPP,
     PayerStatus,
     Purpose,
     PurposeCode,
     Reason,
+    ReceiverAccountNumber,
+    ReceiverBIC,
+    ReceiverINN,
+    ReceiverKPP,
     TaxPeriod,
 )
 from vitya.payment_order.payments.constants import (
     CUSTOMS_REASONS,
     DOCUMENT_NUMBERS,
-    FNS_PAYEE_ACCOUNT_NUMBER,
+    FNS_RECEIVER_ACCOUNT_NUMBER,
 )
 from vitya.payment_order.payments.tools import get_account_kind
-from vitya.pydantic_fields import BIC, INN, KPP, OKTMO
+from vitya.pydantic_fields import BIC, OKTMO
 
 
 def check_account_by_bic(
     account_number: AccountNumber,
     bic: BIC,
 ) -> None:
     _sum = 0
     for c, v in zip(bic[-3:] + account_number, [7, 1, 3] * 8):
         _sum += int(c) * v
     if _sum % 10 != 0:
         raise AccountValidationBICValueError
 
 
-def check_payee_account(
-    value: AccountNumber,
+def check_receiver_account(
+    value: ReceiverAccountNumber,
     payment_type: PaymentType,
-    payee_bic: BIC,
+    receiver_bic: ReceiverBIC,
 ) -> str:
     if payment_type == PaymentType.FNS:
-        if value != FNS_PAYEE_ACCOUNT_NUMBER:
-            raise PayeeAccountValidationFNSValueError
+        if value != FNS_RECEIVER_ACCOUNT_NUMBER:
+            raise ReceiverAccountValidationFNSValueError
     elif not payment_type.is_budget:
         try:
-            check_account_by_bic(account_number=value, bic=payee_bic)
+            check_account_by_bic(account_number=value, bic=receiver_bic)
         except AccountValidationBICValueError as e:
-            raise PayeeAccountValidationBICValueError from e
+            raise ReceiverAccountValidationBICValueError from e
     return value
 
 
 def check_operation_kind(
     value: OperationKind,
     payment_type: PaymentType
 ) -> OperationKind:
-    if payment_type.is_budget:
-        if value not in {'01', '02', '06'}:
-            raise OperationKindValidationBudgetValueError
+    if payment_type.is_budget and value not in {'01', '02', '06'}:
+        raise OperationKindValidationBudgetValueError
     return value
 
 
 def check_purpose_code(
     value: Optional[PurposeCode],
     payment_type: PaymentType,
 ) -> Optional[PurposeCode]:
-    if payment_type != PaymentType.FL:
+    if payment_type not in (PaymentType.FL, PaymentType.CHAMELEON):
         if value is not None:
             raise PurposeCodeValidationNullError
         return None
     if value is not None and value not in {1, 2, 3, 4, 5}:
-        raise PurposeCodeValidationFlError
+        if payment_type == PaymentType.FL:
+            raise PurposeCodeValidationFlError
+        raise PurposeCodeValidationChameleonError
     return value
 
 
 def check_uin(
     value: Optional[UIN],
-    payee_account: AccountNumber,
+    receiver_account: ReceiverAccountNumber,
     payment_type: PaymentType,
     payer_status: Optional[PayerStatus],
-    payer_inn: Optional[str],
+    payer_inn: Optional[PayerINN],
 ) -> Optional[UIN]:
     if not payment_type.is_budget:
         return None
 
     if payer_status == '31' and value is None:
         raise UINValidationValueZeroError
 
     if payment_type == PaymentType.BUDGET_OTHER:
-        if payee_account.startswith('03212') and value is None:
+        if receiver_account.startswith('03212') and value is None:
             raise UINValidationBONotEmpty
         return value
 
     if payment_type == PaymentType.FNS:
         if payer_status == '13' and payer_inn is None and value is None:
             raise UINValidationFNSValueZeroError
         if payer_status == '02':
@@ -152,15 +165,15 @@
                 raise UINValidationFNSNotValueZeroError
             return value
     return value
 
 
 def check_purpose(
     value: Optional[Purpose],
-    payer_account: AccountNumber,
+    payer_account: PayerAccountNumber,
     payment_type: PaymentType,
 ) -> Optional[Purpose]:
     if (
         not payment_type.is_budget
         and get_account_kind(payer_account) == AccountKind.IP
         and (
             value is None
@@ -168,108 +181,121 @@
         )
     ):
         raise PurposeValidationIPNDSError
     return value
 
 
 def check_payer_inn(
-    value: Optional[INN],
+    value: Optional[PayerINN],
     payment_type: PaymentType,
     payer_status: Optional[PayerStatus],
-    for_third_face: bool,
-) -> Optional[INN]:
+    for_third_person: ForThirdPerson,
+) -> Optional[PayerINN]:
     if not payment_type.is_budget:
         return value
 
     if value is None:
         if payment_type == PaymentType.BUDGET_OTHER:
             return None
         elif payment_type == PaymentType.FNS and payer_status == '13':
             return None
         elif payment_type == PaymentType.CUSTOMS and payer_status == '30':
             return None
         raise PayerINNValidationEmptyNotAllowedError
 
     if payment_type == PaymentType.CUSTOMS:
-        if payer_status == '06' and for_third_face and len(value) != 10:
+        if payer_status == '06' and for_third_person and len(value) != 10:
             raise PayerINNValidationCustomsLen10Error
 
         if payer_status in {'16', '17'} and len(value) != 12:
             raise PayerINNValidationCustomsLen12Error
 
     if value.startswith('00'):
         raise PayerINNValidationStartWithZerosError
 
     return value
 
 
-def check_payee_inn(
-    value: Optional[INN],
+def check_receiver_inn(
+    value: Optional[ReceiverINN],
     payment_type: PaymentType,
-) -> Optional[INN]:
+) -> Optional[ReceiverINN]:
     if payment_type == PaymentType.IP:
         if value is None or len(value) != 12:
-            raise PayeeINNValidationIPLenError
+            raise ReceiverINNValidationIPLenError
         return value
     elif payment_type == PaymentType.FL:
         if value is not None and len(value) != 12:
-            raise PayeeINNValidationFLLenError
+            raise ReceiverINNValidationFLLenError
+        return value
+    elif payment_type == PaymentType.CHAMELEON:
+        if value is not None and len(value) not in (10, 12):
+            raise ReceiverINNValidationChameleonLenError
         return value
     if value is None:
-        raise PayeeINNValidationNonEmptyError
+        raise ReceiverINNValidationNonEmptyError
     elif len(value) != 10:
-        raise PayeeINNValidationLELenError
+        raise ReceiverINNValidationLELenError
     return value
 
 
+def check_payment_type_and_for_third_person(
+    payment_type: PaymentType,
+    for_third_person: ForThirdPerson,
+) -> None:
+    if for_third_person and not payment_type.is_budget:
+        raise BudgetPaymentForThirdPersonError
+
+
 def check_payer_status(
     value: Optional[PayerStatus],
     payment_type: PaymentType,
-    for_third_face: bool,
+    for_third_person: ForThirdPerson,
 ) -> Optional[PayerStatus]:
     if not payment_type.is_budget:
         return None
 
     if value is None:
         raise PayerStatusValidationNullNotAllowedError
 
-    if payment_type == PaymentType.CUSTOMS and for_third_face and value == '06':
+    if payment_type == PaymentType.CUSTOMS and for_third_person and value == '06':
         raise PayerStatusValidationCustoms05NotAllowedError
 
     return value
 
 
 def check_payer_kpp(
-    value: Optional[KPP],
+    value: Optional[PayerKPP],
     payment_type: PaymentType,
-    payer_inn: Optional[str],
-) -> Optional[KPP]:
+    payer_inn: Optional[PayerINN],
+) -> Optional[PayerKPP]:
     if not payment_type.is_budget:
         return None
 
     if payer_inn is not None and len(payer_inn) == 10 and value is None:
         raise PayerKPPValidationINN10EmptyNotAllowed
     elif payer_inn is not None and len(payer_inn) == 12 and value is not None:
         raise PayerKPPValidationINN12OnlyEmptyError
     return value
 
 
-def check_payee_kpp(
-    value: Optional[KPP],
+def check_receiver_kpp(
+    value: Optional[ReceiverKPP],
     payment_type: PaymentType,
-) -> Optional[KPP]:
+) -> Optional[ReceiverKPP]:
     if payment_type in {PaymentType.FL, PaymentType.IP}:
         if value is not None:
-            raise PayeeKPPValidationOnlyEmptyError
+            raise ReceiverKPPValidationOnlyEmptyError
         return None
-
+    if payment_type in {PaymentType.LE, PaymentType.CHAMELEON}:
+        return value
     if value is None:
-        raise PayeeKPPValidationEmptyNotAllowed
+        raise ReceiverKPPValidationEmptyNotAllowed
     if value.startswith('00'):
-        raise PayeeKPPValidationStartsWithZeros
+        raise ReceiverKPPValidationStartsWithZeros
     return value
 
 
 def check_cbc(
     value: Optional[CBC],
     payment_type: PaymentType,
 ) -> Optional[CBC]:
@@ -360,27 +386,31 @@
 
 
 def check_document_number(
     value: Optional[DocumentNumber],
     payment_type: PaymentType,
     reason: Optional[Reason],
     payer_status: Optional[PayerStatus],
-    payee_account: AccountNumber,
+    receiver_account: ReceiverAccountNumber,
     uin: Optional[UIN],
-    payer_inn: Optional[INN],
+    payer_inn: Optional[PayerINN],
 ) -> Optional[DocumentNumber]:
     if not payment_type.is_budget:
         return None
 
     if payment_type == PaymentType.FNS:
         if value is not None:
             raise DocumentNumberValidationFNSOnlyEmptyError
         return None
     elif payment_type == PaymentType.BUDGET_OTHER:
-        if payee_account.startswith('03212') and payer_status == '31' and uin is not None:
+        if payer_status == '33':
+            if value is not None:
+                raise DocumentNumberValidationBOPayerStatus33OnlyEmptyError
+            return None
+        if receiver_account.startswith('03212') and payer_status == '31' and uin is not None:
             if value is not None:
                 raise DocumentNumberValidationBOOnlyEmptyError
             return None
 
         if payer_status == '24' and payer_inn is None and uin is None and value is None:
             raise DocumentNumberValidationBOEmptyNotAllowed
         if value is not None:
```

### Comparing `vitya-0.16.0/vitya/payment_order/payments/constants.py` & `vitya-0.17.0/vitya/payment_order/payments/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FNS_PAYEE_ACCOUNT_NUMBER = '03100643000000018500'
+FNS_RECEIVER_ACCOUNT_NUMBER = '03100643000000018500'
 
 REPLACE_CHARS_FOR_SPACE = {
     '\t', '\n', '\x0b', '\x0c', '\r', ' ', '\x85', '\xa0', '\u1680', '\u2000', '\u2001',
     '\u2002', '\u2003', '\u2004', '\u2005', '\u2006', '\u2007', '\u2008', '\u2009', '\u200a',
     '\u2028', '\u2029', '\u202f', '\u205f', '\u3000'
 }
```

### Comparing `vitya-0.16.0/vitya/payment_order/validators.py` & `vitya-0.17.0/vitya/payment_order/validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from decimal import Decimal, InvalidOperation
-from typing import Optional
+from typing import Optional, Union
 
 from vitya.payment_order.errors import (
     AccountNumberValidationDigitsOnlyError,
     AccountNumberValidationSizeError,
     AccountNumberValidationTypeError,
     AmountNotANumber,
     AmountValidationLengthError,
@@ -15,26 +15,29 @@
     CBCValidationValueLenError,
     CustomerValidationSizeError,
     DocumentDateValidationTypeError,
     DocumentNumberValidationTypeError,
     NumberValidationLenError,
     OperationKindValidationTypeError,
     OperationKindValidationValueError,
-    PayeeValidationNameError,
-    PayeeValidationSizeError,
     PayerStatusValidationTypeError,
     PayerStatusValidationValueError,
     PayerValidationSizeError,
+    PaymentOrderLenError,
     PaymentOrderValidationError,
     PurposeCodeValidationTypeError,
-    PurposeValidationCharactersError,
     PurposeValidationMaxLenError,
     PurposeValidationTypeError,
     ReasonValidationTypeError,
     ReasonValidationValueLenError,
+    ReceiverAccountNumberValidationDigitsOnlyError,
+    ReceiverAccountNumberValidationSizeError,
+    ReceiverAccountNumberValidationTypeError,
+    ReceiverValidationNameError,
+    ReceiverValidationSizeError,
     TaxPeriodValidationTypeError,
     UINValidationControlSumError,
     UINValidationDigitsOnlyError,
     UINValidationLenError,
     UINValidationOnlyZeroError,
     UINValidationTypeError,
 )
@@ -79,28 +82,30 @@
     try:
         validate_customer(value)
     except CustomerValidationSizeError as e:
         raise PayerValidationSizeError from e
     return value
 
 
-def validate_payee(value: str) -> str:
+def validate_receiver(value: str) -> str:
     try:
         validate_customer(value)
     except CustomerValidationSizeError as e:
-        raise PayeeValidationSizeError from e
+        raise ReceiverValidationSizeError from e
     if bool(re.match('(.*)(4)[0-9]{19}', value)):
-        raise PayeeValidationNameError
+        raise ReceiverValidationNameError
     return value
 
 
-def validate_payment_order(value: Optional[str]) -> int:
+def validate_payment_order(value: Optional[Union[int, str]]) -> int:
     if value is None or value == '':
         return 5
 
+    if isinstance(value, str) and len(value) != 1:
+        raise PaymentOrderLenError
     try:
         value_int = int(value)
     except ValueError:
         raise PaymentOrderValidationError
     if value_int not in {1, 2, 3, 4, 5}:
         raise PaymentOrderValidationError
     return value_int
@@ -112,14 +117,25 @@
     if len(value) != 20:
         raise AccountNumberValidationSizeError
     if not only_digits(value):
         raise AccountNumberValidationDigitsOnlyError
     return value
 
 
+def validate_receiver_account_number(value: str) -> str:
+    try:
+        return validate_account_number(value)
+    except AccountNumberValidationTypeError:
+        raise ReceiverAccountNumberValidationTypeError
+    except AccountNumberValidationSizeError:
+        raise ReceiverAccountNumberValidationSizeError
+    except AccountNumberValidationDigitsOnlyError:
+        raise ReceiverAccountNumberValidationDigitsOnlyError
+
+
 def validate_operation_kind(value: str) -> str:
     if not isinstance(value, str):
         raise OperationKindValidationTypeError
     if len(value) != 2:
         raise OperationKindValidationValueError
     return value
 
@@ -183,28 +199,27 @@
     try:
         value = int(value)
     except Exception:
         raise PurposeCodeValidationTypeError
     return value
 
 
+_PURPOSE_TRANS_TABLE = str.maketrans({char: ' ' for char in REPLACE_CHARS_FOR_SPACE})
+
+
 def validate_purpose(value: str) -> str:
     if not isinstance(value, str):
         raise PurposeValidationTypeError
 
     if value == '':
         return '0'
 
+    value = ''.join(c for c in value.translate(_PURPOSE_TRANS_TABLE) if c in CHARS_FOR_PURPOSE)
     if len(value) > 210:
         raise PurposeValidationMaxLenError
-
-    replaced_space_value = ''.join(map(lambda x: x if x not in REPLACE_CHARS_FOR_SPACE else ' ', value))
-    for c in replaced_space_value:
-        if c not in CHARS_FOR_PURPOSE:
-            raise PurposeValidationCharactersError
     return value
 
 
 def validate_payer_status(value: str) -> str:
     if not isinstance(value, str):
         raise PayerStatusValidationTypeError
     elif value not in PAYER_STATUSES:
```

### Comparing `vitya-0.16.0/vitya/pydantic_fields.py` & `vitya-0.17.0/vitya/pydantic_fields.py`

 * *Files 24% similar despite different names*

```diff
@@ -65,27 +65,27 @@
                     return None
                 raise MissingError
         yield validator
 
 
 class INN(FieldMixin, str):
     @classmethod
-    def _validate(cls, value: str) -> str:
+    def _validate(cls, value: str) -> Optional[str]:
         return validate_inn(value)
 
 
 class INNIP(FieldMixin, str):
     @classmethod
-    def _validate(cls, value: str) -> str:
+    def _validate(cls, value: str) -> Optional[str]:
         return validate_inn_ip(value)
 
 
 class INNLE(FieldMixin, str):
     @classmethod
-    def _validate(cls, value: str) -> str:
+    def _validate(cls, value: str) -> Optional[str]:
         return validate_inn_le(value)
 
 
 class KPP(FieldMixin, str):
     @classmethod
     def _validate(cls, value: str) -> Optional[str]:
         return validate_kpp(value)
@@ -115,7 +115,40 @@
         return _validate_wrapper(validate_snils, "snils", value)
 
 
 class OKTMO(FieldMixin, str):
     @classmethod
     def _validate(cls, value: str) -> Optional[str]:
         return validate_oktmo(value)
+
+
+# Pydantic strip NewType from ModelField.type_
+
+class BoolWrapper:
+    __slots__ = ('_value', )
+
+    def __init__(self, value: bool):
+        self._value = value
+
+    def __bool__(self) -> bool:
+        return self._value
+
+    def __hash__(self) -> int:
+        return hash(self._value)
+
+    def __eq__(self, other: Any) -> Any:
+        if isinstance(other, type(self)):
+            return self._value == other._value
+        if isinstance(other, bool):
+            return self._value == other
+        return NotImplemented
+
+    @classmethod
+    def __get_validators__(cls) -> CallableGenerator:
+        def validator(value: Any) -> Any:
+            if isinstance(value, bool):
+                return cls(value)
+            if isinstance(value, cls):
+                return value
+            raise TypeError
+
+        yield validator
```

### Comparing `vitya-0.16.0/vitya/validators.py` & `vitya-0.17.0/vitya/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,23 +28,26 @@
 
 def _count_inn_checksum(inn: str, coefficients: List[int]) -> int:
     assert len(inn) == len(coefficients)
     n = sum([int(digit) * coef for digit, coef in zip(inn, coefficients)])
     return n % 11 % 10
 
 
-def validate_inn(inn: str, is_ip: Optional[bool] = None) -> str:
+def validate_inn(inn: str, is_ip: Optional[bool] = None) -> Optional[str]:
     """
     Source:
     https://www.consultant.ru/document/cons_doc_LAW_134082/947eeb5630c9f58cbc6103f0910440cef8eaccac/
     https://ru.wikipedia.org/wiki/%D0%98%D0%B4%D0%B5%D0%BD%D1%82%D0%B8%D1%84%D0%B8%D0%BA%D0%B0%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D1%8B%D0%B9_%D0%BD%D0%BE%D0%BC%D0%B5%D1%80_%D0%BD%D0%B0%D0%BB%D0%BE%D0%B3%D0%BE%D0%BF%D0%BB%D0%B0%D1%82%D0%B5%D0%BB%D1%8C%D1%89%D0%B8%D0%BA%D0%B0
     """
     if not isinstance(inn, str):
         raise INNValidationTypeError
 
+    if inn in {'', '0'}:
+        return None
+
     if not re.fullmatch(r'[0-9]+', inn):
         raise INNValidationDigitsOnlyError
 
     if inn.startswith('00'):
         raise INNValidationStartsWithZerosError
 
     coefs10 = [2, 4, 10, 3, 5, 9, 4, 6, 8]
@@ -67,19 +70,19 @@
         return inn
     elif len(inn) == 5:
         return inn
 
     raise INNValidationLenError
 
 
-def validate_inn_ip(inn: str) -> str:
+def validate_inn_ip(inn: str) -> Optional[str]:
     return validate_inn(inn, is_ip=True)
 
 
-def validate_inn_le(inn: str) -> str:
+def validate_inn_le(inn: str) -> Optional[str]:
     return validate_inn(inn, is_ip=False)
 
 
 def validate_kpp(kpp: str) -> Optional[str]:
     """
     Source: https://kontur.ru/bk/spravka/491-chtotakoe_kpp
     """
```

### Comparing `vitya-0.16.0/vitya.egg-info/SOURCES.txt` & `vitya-0.17.0/vitya.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+tests/test_error_description.py
 tests/test_vitya.py
 vitya/__init__.py
+vitya/error_description.py
 vitya/errors.py
 vitya/errors_base.py
 vitya/py.typed
 vitya/pydantic_fields.py
+vitya/typing_helpers.py
 vitya/validators.py
 vitya.egg-info/PKG-INFO
 vitya.egg-info/SOURCES.txt
 vitya.egg-info/dependency_links.txt
 vitya.egg-info/top_level.txt
 vitya/payment_order/__init__.py
 vitya/payment_order/enums.py
```

