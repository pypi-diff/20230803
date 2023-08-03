# Comparing `tmp/lexikanon-0.4.0.tar.gz` & `tmp/lexikanon-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikanon-0.4.0.tar", max compression
+gzip compressed data, was "lexikanon-0.4.1.tar", max compression
```

## Comparing `lexikanon-0.4.0.tar` & `lexikanon-0.4.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1071 2023-07-30 10:49:34.064915 lexikanon-0.4.0/LICENSE
--rw-r--r--   0        0        0     2129 2023-07-30 10:49:34.064915 lexikanon-0.4.0/README.md
--rw-r--r--   0        0        0     3218 2023-07-30 10:50:07.065485 lexikanon-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      184 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/__cli__.py
--rw-r--r--   0        0        0      473 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/__init__.py
--rw-r--r--   0        0        0       22 2023-07-30 10:50:07.021484 lexikanon-0.4.0/src/lexikanon/_version.py
--rw-r--r--   0        0        0        0 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/__init__.py
--rw-r--r--   0        0        0      177 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/about/lexikanon.yaml
--rw-r--r--   0        0        0      213 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/normalizer/__init__.yaml
--rw-r--r--   0        0        0       79 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/normalizer/formal_en.yaml
--rw-r--r--   0        0        0      114 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/normalizer/formal_en_parantheses.yaml
--rw-r--r--   0        0        0       68 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/normalizer/formal_ko.yaml
--rw-r--r--   0        0        0      363 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/normalizer/ftfy/__init__.yaml
--rw-r--r--   0        0        0       94 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/normalizer/informal_ko.yaml
--rw-r--r--   0        0        0      102 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/normalizer/spaces/__init__.yaml
--rw-r--r--   0        0        0      151 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/normalizer/special_characters/__init__.yaml
--rw-r--r--   0        0        0       53 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/pipe/extract_nouns.yaml
--rw-r--r--   0        0        0      128 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/pipe/extract_tokens.yaml
--rw-r--r--   0        0        0      130 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/pipe/tokenize_dataset.yaml
--rw-r--r--   0        0        0      376 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/run/extract_tokens.yaml
--rw-r--r--   0        0        0      260 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/run/tokenize_dataset.yaml
--rw-r--r--   0        0        0      204 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/stopwords/__init__.yaml
--rw-r--r--   0        0        0      541 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/tokenizer/__init__.yaml
--rw-r--r--   0        0        0      262 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/tokenizer/mecab.yaml
--rw-r--r--   0        0        0      171 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/tokenizer/nltk.yaml
--rw-r--r--   0        0        0      109 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/tokenizer/simple.yaml
--rw-r--r--   0        0        0      142 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/tokenizer/tagger/mecab.yaml
--rw-r--r--   0        0        0      178 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/conf/tokenizer/tagger/nltk.yaml
--rw-r--r--   0        0        0       61 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/normalizers/__init__.py
--rw-r--r--   0        0        0    10539 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/normalizers/normalizer.py
--rw-r--r--   0        0        0        0 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/pipe/__init__.py
--rw-r--r--   0        0        0     3430 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/pipe/tokenize.py
--rw-r--r--   0        0        0      195 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/project.toml
--rw-r--r--   0        0        0        0 2023-07-30 10:49:34.068915 lexikanon-0.4.0/src/lexikanon/py.typed
--rw-r--r--   0        0        0  2355775 2023-07-30 10:49:34.080915 lexikanon-0.4.0/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic
--rw-r--r--   0        0        0       58 2023-07-30 10:49:34.080915 lexikanon-0.4.0/src/lexikanon/stopwords/__init__.py
--rw-r--r--   0        0        0     5152 2023-07-30 10:49:34.080915 lexikanon-0.4.0/src/lexikanon/stopwords/stopwords.py
--rw-r--r--   0        0        0      181 2023-07-30 10:49:34.080915 lexikanon-0.4.0/src/lexikanon/tokenizers/__init__.py
--rw-r--r--   0        0        0     9300 2023-07-30 10:49:34.084915 lexikanon-0.4.0/src/lexikanon/tokenizers/base.py
--rw-r--r--   0        0        0      817 2023-07-30 10:49:34.084915 lexikanon-0.4.0/src/lexikanon/tokenizers/mecab.py
--rw-r--r--   0        0        0     3158 2023-07-30 10:49:34.084915 lexikanon-0.4.0/src/lexikanon/tokenizers/nltk.py
--rw-r--r--   0        0        0    14339 2023-07-30 10:49:34.084915 lexikanon-0.4.0/src/lexikanon/utils/__init__.py
--rw-r--r--   0        0        0     8294 2023-07-30 10:49:34.084915 lexikanon-0.4.0/src/lexikanon/utils/hangle.py
--rw-r--r--   0        0        0      255 2023-07-30 10:49:34.084915 lexikanon-0.4.0/src/lexikanon/utils/hanja/__init__.py
--rw-r--r--   0        0        0     2123 2023-07-30 10:49:34.084915 lexikanon-0.4.0/src/lexikanon/utils/hanja/hangul.py
--rw-r--r--   0        0        0     2813 2023-07-30 10:49:34.084915 lexikanon-0.4.0/src/lexikanon/utils/hanja/impl.py
--rw-r--r--   0        0        0      427 2023-07-30 10:49:34.084915 lexikanon-0.4.0/src/lexikanon/utils/hanja/table.py
--rw-r--r--   0        0        0   522443 2023-07-30 10:49:34.084915 lexikanon-0.4.0/src/lexikanon/utils/hanja/table.yml
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 lexikanon-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-03 02:36:07.821254 lexikanon-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2129 2023-08-03 02:36:07.821254 lexikanon-0.4.1/README.md
+-rw-r--r--   0        0        0     3218 2023-08-03 02:36:45.805957 lexikanon-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      184 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/__cli__.py
+-rw-r--r--   0        0        0      473 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-03 02:36:45.753956 lexikanon-0.4.1/src/lexikanon/_version.py
+-rw-r--r--   0        0        0        0 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/__init__.py
+-rw-r--r--   0        0        0      177 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/about/lexikanon.yaml
+-rw-r--r--   0        0        0      214 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/formal_en.yaml
+-rw-r--r--   0        0        0      114 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/formal_en_parantheses.yaml
+-rw-r--r--   0        0        0       68 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/formal_ko.yaml
+-rw-r--r--   0        0        0      363 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/ftfy/__init__.yaml
+-rw-r--r--   0        0        0       94 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/informal_ko.yaml
+-rw-r--r--   0        0        0      102 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/spaces/__init__.yaml
+-rw-r--r--   0        0        0      151 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/special_characters/__init__.yaml
+-rw-r--r--   0        0        0       53 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/pipe/extract_nouns.yaml
+-rw-r--r--   0        0        0      128 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/pipe/extract_tokens.yaml
+-rw-r--r--   0        0        0      130 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/pipe/tokenize_dataset.yaml
+-rw-r--r--   0        0        0      376 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/run/extract_tokens.yaml
+-rw-r--r--   0        0        0      260 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/run/tokenize_dataset.yaml
+-rw-r--r--   0        0        0      205 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/stopwords/__init__.yaml
+-rw-r--r--   0        0        0      542 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/__init__.yaml
+-rw-r--r--   0        0        0      262 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/mecab.yaml
+-rw-r--r--   0        0        0      171 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/nltk.yaml
+-rw-r--r--   0        0        0      109 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/simple.yaml
+-rw-r--r--   0        0        0      143 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/tagger/mecab.yaml
+-rw-r--r--   0        0        0      179 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/tagger/nltk.yaml
+-rw-r--r--   0        0        0       61 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/normalizers/__init__.py
+-rw-r--r--   0        0        0    10513 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/normalizers/normalizer.py
+-rw-r--r--   0        0        0        0 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/pipe/__init__.py
+-rw-r--r--   0        0        0     3430 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/pipe/tokenize.py
+-rw-r--r--   0        0        0      195 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/project.toml
+-rw-r--r--   0        0        0        0 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/py.typed
+-rw-r--r--   0        0        0  2355775 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic
+-rw-r--r--   0        0        0       58 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/stopwords/__init__.py
+-rw-r--r--   0        0        0     5153 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/stopwords/stopwords.py
+-rw-r--r--   0        0        0      181 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/tokenizers/__init__.py
+-rw-r--r--   0        0        0     9301 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/tokenizers/base.py
+-rw-r--r--   0        0        0      818 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/tokenizers/mecab.py
+-rw-r--r--   0        0        0     3159 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/tokenizers/nltk.py
+-rw-r--r--   0        0        0    14339 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/__init__.py
+-rw-r--r--   0        0        0     8294 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/hangle.py
+-rw-r--r--   0        0        0      255 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/hanja/__init__.py
+-rw-r--r--   0        0        0     2123 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/hanja/hangul.py
+-rw-r--r--   0        0        0     2813 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/hanja/impl.py
+-rw-r--r--   0        0        0      427 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/hanja/table.py
+-rw-r--r--   0        0        0   522443 2023-08-03 02:36:07.845254 lexikanon-0.4.1/src/lexikanon/utils/hanja/table.yml
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 lexikanon-0.4.1/PKG-INFO
```

### Comparing `lexikanon-0.4.0/LICENSE` & `lexikanon-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.0/README.md` & `lexikanon-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.0/pyproject.toml` & `lexikanon-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "lexikanon"
-version = "0.4.0"
+version = "0.4.1"
 description = "A Python Library for Tokenizers"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://lexikanon.entelecheia.ai"
 repository = "https://github.com/entelecheia/lexikanon"
 readme = "README.md"
 packages = [{ include = "lexikanon", from = "src" }]
 
 [tool.poetry.scripts]
 lexikanon = 'lexikanon.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^1.12.5"
+hyfi = "^1.17.2"
 ftfy = "^6.1.1"
 nltk = "^3.8.1"
 ekonlpy = "^2.0.2"
 # hyfi = { path = "../hyfi", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `lexikanon-0.4.0/src/lexikanon/conf/tokenizer/__init__.yaml` & `lexikanon-0.4.1/src/lexikanon/conf/tokenizer/__init__.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 defaults:
   - /normalizer: __init__
   - /stopwords: __init__
 
-_config_group_: tokenizer
+_config_group_: /tokenizer
 _config_name_: __init__
 _target_: corprep.tokenizer.SimpleTokenizer
 lowercase: false
 strip_pos: false
 postag_delim: /
 postag_length:
 include_whitespace_token: true
```

### Comparing `lexikanon-0.4.0/src/lexikanon/normalizers/normalizer.py` & `lexikanon-0.4.1/src/lexikanon/normalizers/normalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 from typing import Optional
 
 from ftfy import TextFixerConfig, fix_text
-from hyfi.composer import BaseModel
-from hyfi.composer.base import BaseConfig
+from hyfi.composer import BaseConfig, BaseModel
 
 from lexikanon import HyFI
 from lexikanon.utils import (
     ACCENTS,
     APOSTROPHES,
     CONTROLS,
     DOUBLE_QUOTES,
@@ -41,15 +40,15 @@
     fix_line_breaks: true
     fix_surrogates: true
     remove_control_chars: true
     normalization: NFKC
     max_decode_length: 1000000
     """
 
-    _config_group_: str = "normalizers/fyfy"
+    _config_group_: str = "/normalizers/fyfy"
     _config_name_: str = "__init__"
 
     unescape_html: bool = True
     remove_terminal_escapes: bool = True
     fix_encoding: bool = True
     restore_byte_a0: bool = True
     replace_lossy_sequences: bool = True
@@ -70,15 +69,15 @@
     strip: true
     fix_whitespaces: true
     collapse_whitespaces: true
     replace_tabs: true
     num_spaces_for_tab: 4
     """
 
-    _config_group_: str = "normalizers/spaces"
+    _config_group_: str = "/normalizers/spaces"
     _config_name_: str = "__init__"
 
     strip: bool = True
     fix_whitespaces: bool = True
     collapse_whitespaces: bool = True
     replace_tabs: bool = True
     num_spaces_for_tab: int = 4
@@ -91,15 +90,15 @@
     fix_slashes: true
     fix_tildes: true
     fix_emoticons: false
     single_quotes_only: false
     regular_parentheses_only: false
     """
 
-    _config_group_: str = "normalizers/special_characters"
+    _config_group_: str = "/normalizers/special_characters"
     _config_name_: str = "__init__"
 
     fix_hyphens: bool = True
     fix_ellipsis: bool = True
     fix_slashes: bool = True
     fix_tildes: bool = True
     fix_emoticons: bool = False
@@ -113,15 +112,15 @@
     By default, the normal form NFKC is used for unicode normalization.
     This applies a compatibility decomposition,
     under which equivalent characters are unified, followed by a canonical composition.
     See Python docs for information
     on normal forms: http://docs.python.org/2/library/unicodedata.html#unicodedata.normalize
     """
 
-    _config_group_: str = "normalizer"
+    _config_group_: str = "/normalizer"
     _config_name_: str = "__init__"
 
     ftfy: FyfyConfig = FyfyConfig()
     spaces: SpacesConfig = SpacesConfig()
     special_characters: SpecialCharactersConfig = SpecialCharactersConfig()
     hanja2hangle: bool = True
     num_repeats: int = 2
```

### Comparing `lexikanon-0.4.0/src/lexikanon/pipe/tokenize.py` & `lexikanon-0.4.1/src/lexikanon/pipe/tokenize.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.0/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic` & `lexikanon-0.4.1/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.0/src/lexikanon/stopwords/stopwords.py` & `lexikanon-0.4.1/src/lexikanon/stopwords/stopwords.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     stopwords_fn:
     stopwords_list:
     stopwords_path:
     nltk_stopwords_lang:
     verbose: False
     """
 
-    _config_group_: str = "stopwords"
+    _config_group_: str = "/stopwords"
     _config_name_: str = "__init__"
 
     name: str = "stopwords"
     lowercase: bool = False
     stopwords_fn: Optional[Union[str, Callable[[str], bool]]] = None
     stopwords_list: Optional[List[str]] = None
     stopwords_path: Optional[str] = None
```

### Comparing `lexikanon-0.4.0/src/lexikanon/tokenizers/base.py` & `lexikanon-0.4.1/src/lexikanon/tokenizers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from lexikanon.normalizers import Normalizer
 from lexikanon.stopwords import Stopwords
 
 logger = HyFI.getLogger(__name__)
 
 
 class Tokenizer(BaseModel):
-    _config_group_: str = "tokenizers"
+    _config_group_: str = "/tokenizers"
     _config_name_: str = "__init__"
 
     stopwords: Stopwords = Stopwords()
     normalizer: Normalizer = Normalizer()
 
     lowercase: bool = False
     strip_pos: bool = False
```

### Comparing `lexikanon-0.4.0/src/lexikanon/tokenizers/mecab.py` & `lexikanon-0.4.1/src/lexikanon/tokenizers/mecab.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class MecabTagger(BaseModel):
     """
     userdic_path:
     backend: ekonlpy
     verbose: false
     """
 
-    _config_group_: str = "tokenizers/tagger"
+    _config_group_: str = "/tokenizers/tagger"
     _config_name_: str = "mecab"
 
     userdic_path: Optional[str] = None
     backend: str = "ekonlpy"
     verbose: bool = False
 
     def _parse(self, text: str) -> List[Tuple[str, str]]:
```

### Comparing `lexikanon-0.4.0/src/lexikanon/tokenizers/nltk.py` & `lexikanon-0.4.1/src/lexikanon/tokenizers/nltk.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     stem: true
     lemmatizer:
         _target_: nltk.stem.WordNetLemmatizer
     stemmer:
         _target_: nltk.stem.PorterStemmer
     """
 
-    _config_group_: str = "tokenizers/tagger"
+    _config_group_: str = "/tokenizers/tagger"
     _config_name_: str = "nltk"
 
     lemmatize: bool = False
     stem: bool = True
     lemmatizer: Optional[dict] = None
     stemmer: Optional[dict] = None
     verbose: bool = False
```

### Comparing `lexikanon-0.4.0/src/lexikanon/utils/__init__.py` & `lexikanon-0.4.1/src/lexikanon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.0/src/lexikanon/utils/hangle.py` & `lexikanon-0.4.1/src/lexikanon/utils/hangle.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.0/src/lexikanon/utils/hanja/hangul.py` & `lexikanon-0.4.1/src/lexikanon/utils/hanja/hangul.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.0/src/lexikanon/utils/hanja/impl.py` & `lexikanon-0.4.1/src/lexikanon/utils/hanja/impl.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.0/src/lexikanon/utils/hanja/table.yml` & `lexikanon-0.4.1/src/lexikanon/utils/hanja/table.yml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.0/PKG-INFO` & `lexikanon-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lexikanon
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python Library for Tokenizers
 Home-page: https://lexikanon.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: ekonlpy (>=2.0.2,<3.0.0)
 Requires-Dist: ftfy (>=6.1.1,<7.0.0)
-Requires-Dist: hyfi (>=1.12.5,<2.0.0)
+Requires-Dist: hyfi (>=1.17.2,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Project-URL: Repository, https://github.com/entelecheia/lexikanon
 Description-Content-Type: text/markdown
 
 # Lexikanon
 
 [![pypi-image]][pypi-url]
```

