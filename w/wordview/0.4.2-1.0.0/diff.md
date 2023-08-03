# Comparing `tmp/wordview-0.4.2.tar.gz` & `tmp/wordview-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-0.4.2.tar", max compression
+gzip compressed data, was "wordview-1.0.0.tar", max compression
```

## Comparing `wordview-0.4.2.tar` & `wordview-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
--rw-r--r--   0        0        0     2107 2023-07-13 10:31:23.988287 wordview-0.4.2/CHANGES.rst
--rw-r--r--   0        0        0     1074 2023-07-13 10:31:23.988287 wordview-0.4.2/LICENSE
--rw-r--r--   0        0        0     4192 2023-07-13 10:31:23.988287 wordview-0.4.2/README.rst
--rw-r--r--   0        0        0      893 2023-07-13 10:31:24.076289 wordview-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      163 2023-07-13 10:31:24.076289 wordview-0.4.2/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-07-13 10:31:24.076289 wordview-0.4.2/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-07-13 10:31:24.076289 wordview-0.4.2/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4789 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       48 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/clustering/cluster.py
--rw-r--r--   0        0        0       85 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     2900 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/mwes/am.py
--rw-r--r--   0        0        0    11970 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     3962 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0       55 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0       75 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    12315 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/text_analysis/core.py
--rw-r--r--   0        0        0     8763 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 wordview-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     2705 2023-08-03 11:22:29.022213 wordview-1.0.0/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2023-08-03 11:22:29.022213 wordview-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4047 2023-08-03 11:22:29.022213 wordview-1.0.0/README.rst
+-rw-r--r--   0        0        0      937 2023-08-03 11:22:29.130264 wordview-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4789 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       48 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0     1340 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/io/dataframe_reader.py
+-rw-r--r--   0        0        0       85 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     2900 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/am.py
+-rw-r--r--   0        0        0     1499 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/association_measures.py
+-rw-r--r--   0        0        0     1438 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/chunker.py
+-rw-r--r--   0        0        0     9431 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     3962 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/mwe_utils.py
+-rw-r--r--   0        0        0     1967 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/patterns.py
+-rw-r--r--   0        0        0      111 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0     3718 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/preprocessing/count.py
+-rw-r--r--   0        0        0       75 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    12315 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0     8763 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 wordview-1.0.0/PKG-INFO
```

### Comparing `wordview-0.4.2/LICENSE` & `wordview-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-0.4.2/README.rst` & `wordview-1.0.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,15 @@
    :alt: PyPI - Python Version
 
 .. image:: https://img.shields.io/pypi/dm/wordview
    :alt: PyPI - Downloads
 
 Wordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.
 Wordview's Python API is open-source and available under the `MIT
-license <https://en.wikipedia.org/wiki/MIT_License>`__. We, however,
-offer a framework on top of Wordview for enterprise use under a commercial license. See this page for
-more information about this framework.
+license <https://en.wikipedia.org/wiki/MIT_License>`__.
 
 |cover|
 
 
 Usage
 ######
 
@@ -43,16 +41,16 @@
 
 Text Analysis
 *************
 Using this feature, you can have an overview of your text data in terms of various statistics, plots and distribution.
 See `text analysis documentation pages <./docs/source/textstats.rst>`__  for usage and examples.
 
 
-Label Analysis
-**************
+Analysis of Labels
+******************
 Wordview calculates several statistics for labels in labeled datasets whether they are at document or sequence level.
 See `label analysis documentation pages <./docs/source/labels.rst>`__ for usage and examples.
 
 
 Feature Extraction
 ###################
 
@@ -95,8 +93,8 @@
 
 Contributing
 ############
 
 Thank you for contributing to wordview! We and the users of this repo
 appreciate your efforts! You can visit the `contributing page <CONTRIBUTING.rst>`__ for detailed instructions about how you can contribute to Wordview.
 
-.. |cover| image:: docs/figs/cover.png
+.. |cover| image:: docs/figs/cover.png
```

### Comparing `wordview-0.4.2/pyproject.toml` & `wordview-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "wordview"
-version = "0.4.2"
+version = "1.0.0"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
+exclude = ["notebooks/", "tests/", "data/"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 langdetect = ">=1.0.9"
 pandas = "2.0.1"
```

### Comparing `wordview-0.4.2/wordview/anomaly/gaussianize.py` & `wordview-1.0.0/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.2/wordview/anomaly/normaldist.py` & `wordview-1.0.0/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.2/wordview/clustering/cluster.py` & `wordview-1.0.0/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.2/wordview/mwes/am.py` & `wordview-1.0.0/wordview/mwes/am.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.2/wordview/mwes/mwe.py` & `wordview-1.0.0/wordview/mwes/mwe.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,257 +1,30 @@
-import json
-from collections import Counter
+import string
 from typing import Dict, Optional
 
 import pandas
-import tqdm
 from nltk import RegexpParser, word_tokenize
+from tabulate import tabulate  # type: ignore
+from tqdm import tqdm
 
 from wordview import logger
-from wordview.mwes.am import calculate_am
-from wordview.mwes.mwe_utils import get_pos_tags, is_alphanumeric_latinscript_multigram
+from wordview.io.dataframe_reader import DataFrameReader
+from wordview.mwes.association_measures import PMICalculator
+from wordview.mwes.mwe_utils import get_pos_tags
+from wordview.mwes.patterns import DeMWEPatterns, EnMWEPatterns
 
 
-class MWE(object):
-    """
-    Represents a Multiword Expression.
-    """
+class MWEPatternAssociation:
+    """Extract MWE candidates from a list of tokens based on a given pattern."""
 
-    def __init__(
-        self,
-        df: pandas.DataFrame,
-        text_column: str,
-        mwe_types: list[str] = ["NC"],
-        tokenize=False,
-    ) -> None:
-        """Initialize a new MWE object with the given df, text_column and mwe_types.
-
-        Args:
-            df (pandas.DataFram): DataFrame with a text_column that contains the corpus.
-            text_column (str): Specifies the column of DataFrame where text data resides.
-            mwe_types (List): Types of MWEs to be extracted. Supports: NC for Noun-Noun and JNC for Adjective-Noun compounds. Example: ['NC', 'JNC'].
-            tokenize (bool): Tokenize the content of `df[text_column]`.
-
-        Returns:
-            None
-        """
-        self.df = df
-        self.text_column = text_column
-        if not mwe_types:
-            raise ValueError("mwe_types is empty.")
-        if not isinstance(mwe_types, list):
-            raise TypeError("mwe_types is not a list.")
-        for mt in mwe_types:
-            if mt not in ["NC", "JNC"]:
-                raise ValueError(f"{mt} type is not recognized.")
-        self.mwe_types = mwe_types
-        if tokenize:
-            logger.info(
-                '"tokenize" flag set to True. This might lead to a slow instantiation.'
-            )
-            self.df[text_column] = self.df[text_column].apply(self._tokenize)
-        else:
-            self._check_tokenized()
-
-    def _tokenize(self, x):
-        """Helper function to tokenize and join the results with a space.
-
-        Args:
-            x:
-
-        Returns:
-            None
-        """
-        return " ".join(word_tokenize(x))
-
-    def _check_tokenized(self) -> None:
-        """Helper function to check if the content of text_column is tokenized.
-
-        Args:
-            None
-
-        Returns:
-            None
-        """
-        if self.df[self.text_column].shape[0] > 200:
-            tests = self.df[self.text_column].sample(n=200).tolist()
-        else:
-            tests = self.df[self.text_column].sample(frac=0.8).tolist()
-        num_pass = 0
-        for t in tests:
-            try:
-                if " ".join(word_tokenize(t)) == t:
-                    num_pass += 1
-            except Exception as E:
-                logger.error(f"Could not tokenize and join tokens in {t}: \n {E} ")
-
-        if float(num_pass) / float(len(tests)) < 0.8:
-            logger.warning(
-                f"It seems that the content of {self.text_column} in the input data frame is not (fully) tokenized.\nThis can lead to poor results. Consider re-instantiating your MWE instance with 'tokenize' flag set to True.\nNote that this might lead to a slower instantiation."
-            )
-
-    def build_counts(self, counts_filename: Optional[str] = None) -> Optional[Dict]:
-        """Create various count files to be used by downstream methods
-        by calling wordview.mwes.mwe_utils.
-
-        Args:
-            counts_filename (str): Filename for storing counts.
-
-        Returns:
-            None when no counts_filename is provided, otherwise res which is a dictionary of counts.
-        """
-        logger.info("Creating counts...")
-        res = self.get_counts()
-        if not counts_filename:
-            return res
-        else:
-            try:
-                with open(counts_filename, "w") as file:
-                    json.dump(res, file)
-            except Exception as e:
-                logger.error(e)
-                raise e
-            return None
-
-    def extract_mwes(
-        self,
-        am: str = "pmi",
-        mwes_filename: Optional[str] = None,
-        counts_filename: Optional[str] = None,
-        counts: Optional[dict] = None,
-    ) -> dict:
-        """
-        Extract MWEs from counts_filename with respect to the association measure specified by `am`.
-
-        Args:
-            am (str): The association measure to be used. Can be any of [pmi, npmi]
-            mwes_filename (str): File for storing MWEs. Defaults to None.
-            counts_filename (str): File to read counts from.
-
-        Returns:
-            Dictionary of MWEs.
-        """
-        if counts:
-            count_data = counts
-        elif counts_filename is not None:
-            try:
-                with open(counts_filename, "r") as file:
-                    count_data = json.load(file)
-            except Exception as e:
-                logger.error(e)
-                logger.error(
-                    "Counts must be provided either via input argument `counts` or `counts_filename`. Argument `counts` is not specified and it seems like there was an error reading the counts from `counts_filename`."
-                )
-                raise e
-        else:
-            raise ValueError("Either 'counts' or 'counts_filename' must be provided.")
-
-        logger.info(f"Extracting {self.mwe_types} based on {am}")
-        mwe_am_dict = calculate_am(
-            count_data=count_data, am=am, mwe_types=self.mwe_types
-        )
-        if mwes_filename:
-            try:
-                with open(mwes_filename, "w") as file:
-                    json.dump(mwe_am_dict, file)
-            except Exception as e:
-                logger.error(e)
-                raise e
-            finally:
-                return mwe_am_dict
-        else:
-            return mwe_am_dict
-
-    def get_counts(self) -> Dict:
-        """Read a corpus in pandas.DataFrame format and generates all counts necessary for calculating AMs.
+    def __init__(self, association_measure: PMICalculator, pattern: str) -> None:
+        """Initializes a new instance of MWEExtractor class.
 
         Args:
-            None
-
-        Returns:
-            res: Dictionary of mwe_types to dictionary of individual mwe within that type and their count.
-                E.g. {'NC':{'climate change': 10, 'brain drain': 3}, 'JNC': {'black sheep': 3, 'red flag': 2}}
-        """
-        res: Dict = {}
-        for mt in self.mwe_types:
-            res[mt] = {}
-        res["WORDS"] = {}
-        for sent in tqdm.tqdm(self.df[self.text_column]):
-            tokens = sent.split(" ")
-            word_count_dict = Counter(tokens)
-            for k, v in word_count_dict.items():
-                if k in res["WORDS"]:
-                    res["WORDS"][k] += v
-                else:
-                    res["WORDS"][k] = v
-            for mt in self.mwe_types:
-                mwes_count_dic = self.extract_mwes_from_sent(tokens, mwe_type=mt)
-                for k, v in mwes_count_dic.items():
-                    if k in res[mt]:
-                        res[mt][k] += v
-                    else:
-                        res[mt][k] = v
-        return res
-
-    def extract_mwes_from_sent(self, tokens: list[str], mwe_type: str) -> Dict:
-        """Extract two-word noun compounds from tokenized input.
-
-        Args:
-            tokens: A tokenized sentence, i.e. list of tokens.
-            type: Type of MWE. Any of ['NC', 'JNC'].
-
-        Returns:
-            mwes_count_dic: Dictionary of compounds to their count.
-        """
-        if not isinstance(tokens, list):
-            raise TypeError(
-                f'Input argument "tokens" must be a list of string. Currently it is of type {type(tokens)} \
-                with a value of: {tokens}.'
-            )
-        if len(tokens) == 0:
-            return {}
-        mwes = []
-        postag_tokens: list[tuple[str, str]] = get_pos_tags(tokens)
-        w1_pos_tags = []
-        w2_pos_tags = []
-        if mwe_type == "NC":
-            w1_pos_tags = ["NN", "NNS"]
-            w2_pos_tags = ["NN", "NNS"]
-        elif mwe_type == "JNC":
-            w1_pos_tags = ["JJ"]
-            w2_pos_tags = ["NN", "NNS"]
-        for i in range(len(postag_tokens) - 1):
-            w1 = postag_tokens[i]
-            if w1[1] not in w1_pos_tags:
-                continue
-            else:
-                w2 = postag_tokens[i + 1]
-                if not is_alphanumeric_latinscript_multigram(
-                    w1[0]
-                ) or not is_alphanumeric_latinscript_multigram(w2[0]):
-                    continue
-                if w2[1] in w2_pos_tags:
-                    if i + 2 < len(postag_tokens):
-                        w3 = postag_tokens[i + 2]
-                        if w3 not in ["NN", "NNS"]:
-                            mwes.append(w1[0] + " " + w2[0])
-                    else:
-                        mwes.append(w1[0] + " " + w2[0])
-        mwes_count_dic = Counter(mwes)
-        return mwes_count_dic
-
-
-class HigherOrderMWEExtractor:
-    """Extract higher order MWEs from a list of tokens based on a given pattern."""
-
-    def __init__(self, tokens: list[str], pattern: str) -> None:
-        """Initializes a new instance of HigherOrderMWEExtractor class.
-
-        Args:
-            tokens: A list of tokens.
+            association_measure: An instance of an association measure class.
             pattern: A string pattern to match against the tokens. The pattern must be a string of the following form.
 
         Examples of user-defined patterns:
         - NP: {<DT>?<JJ>*<NN>} # Noun phrase
         - VP: {<MD>?<VB.*><NP|PP|CLAUSE>+$} # Verb phrase
         - PP: {<IN><NP>} # Prepositional phrase
 
@@ -262,64 +35,198 @@
         ADJP: {<RB|RBR|RBS>*<JJ>} # Adjective phrase
         ADVP: {<RB.*>+<VB.*><RB.*>*} # Adverb phrase
         '''
 
         In this case, patterns of a clause are executed in order.  An earlier
         pattern may introduce a chunk boundary that prevents a later pattern from executing.
         """
-        self.tokens = tokens
         self.pattern = pattern
-        self._validate_input()
+        self.association_measure = association_measure
 
-    def _validate_input(self) -> None:
-        if not isinstance(self.tokens, list):
-            raise TypeError(
-                f'Input argument "tokens" must be a list of string. Currently it is of type {type(self.tokens)} \
-                with a value of: {self.tokens}.'
-            )
-        if len(self.tokens) == 0:
-            raise ValueError(
-                'Input argument "tokens" must be a non-empty list of string.'
-            )
-        if not isinstance(self.pattern, str):
-            raise TypeError(
-                f'Input argument "pattern" must be a string. Currently it is of type {type(self.pattern)} \
-                with a value of: {self.pattern}.'
-            )
-        if len(self.pattern) == 0:
-            raise ValueError(
-                'Input argument "pattern" must be a non-zero length string.'
-            )
-
-    def extract_higher_order_mwe_candidates(self) -> dict:
+    def _extract_mwe_candidates(self, tokens: list[str]) -> dict:
         """
         Extract variable-length MWE from tokenized input, using a user-defined POS regex pattern.
 
         Args:
-            None
+            tokens (list[str]): A list of tokens from which mwe candidates are to be extracted.
 
         Returns:
             match_counter (dict[str, dict[str, int]]): A counter dictionary with count of matched strings, grouped by pattern label.
                                                     An empty list if none were found.
         """
 
-        tagged_tokens: list[tuple[str, str]] = get_pos_tags(self.tokens)
+        def validate_input() -> None:
+            if not isinstance(tokens, list):
+                raise TypeError(
+                    f'Input argument "tokens" must be a list of string. Currently it is of type {type(self.tokens)} \
+                    with a value of: {self.tokens}.'
+                )
+            if len(tokens) == 0:
+                raise ValueError(
+                    'Input argument "tokens" must be a non-empty list of string.'
+                )
+            if not isinstance(self.pattern, str):
+                raise TypeError(
+                    f'Input argument "pattern" must be a string. Currently it is of type {type(self.pattern)} \
+                    with a value of: {self.pattern}.'
+                )
+            if len(self.pattern) == 0:
+                raise ValueError(
+                    'Input argument "pattern" must be a non-zero length string.'
+                )
+
+        validate_input()
+        tagged_tokens: list[tuple[str, str]] = get_pos_tags(tokens)
         parser = RegexpParser(self.pattern)
         parsed_tokens = parser.parse(tagged_tokens)
 
         labels: list[str] = [
             rule.split(":")[0].strip() for rule in self.pattern.split("\n") if rule
         ]
 
-        matches: dict[str, list[str]] = {label: [] for label in labels}
+        matches: dict[str, set] = {label: set() for label in labels}
 
         for subtree in parsed_tokens.subtrees():
             label = subtree.label()
             if label in matches:
-                matches[label].append(
-                    " ".join(word for (word, tag) in subtree.leaves())
+                matches[label].add(" ".join(word for (word, tag) in subtree.leaves()))
+        return matches
+
+    def measure_candidate_association(self, tokens: list[str], threshold: float = 1.0):
+        mwes: dict[str, dict[str, float]] = {}
+        for mwe_type, candidate_set in self._extract_mwe_candidates(
+            tokens=tokens
+        ).items():
+            if mwe_type not in mwes:
+                mwes[mwe_type] = {}
+            for mwe_candidate in candidate_set:
+                association = self.association_measure.compute_association(
+                    mwe_candidate
                 )
+                if association > threshold:
+                    mwes[mwe_type][mwe_candidate] = association
+        return mwes
+
+
+class MWE:
+    def __init__(
+        self,
+        df: pandas.DataFrame,
+        text_column: str,
+        ngram_count_source=None,
+        ngram_count_file_path=None,
+        language: str = "EN",
+        custom_patterns: Optional[str] = None,
+        only_custom_patterns: bool = False,
+    ) -> None:
+        """Initializes a new instance of MWE class.
 
-        matches_counter: dict[str, dict[str, int]] = {
-            label: dict(Counter(match_list)) for label, match_list in matches.items()
-        }
-        return matches_counter
+        Args:
+            corpus: A pandas DataFrame containing the corpus.
+            text_column: The name of the column containing the text  (corpus).
+            ngram_count_source: A dictionary containing ngram counts.
+            ngram_count_file_path: A path to a json file containing ngram counts.
+            language: The language of the corpus. Currently only 'EN' and 'DE' are supported.
+            custom_pattern: pattern: A string pattern to match against the tokens. The pattern must be a string of the following form.
+                Examples of user-defined patterns:
+                NP: {<DT>?<JJ>*<NN>} # Noun phrase
+                You can use multiple and/or nested patterns, separated by a newline character e.g.:
+                custom_pattern = '''
+                NP: {<DT>?<JJ>*<NN>} # Noun phrase
+                VP: {<MD>?<VB.*><NP|PP|CLAUSE>+$} # Verb phrase
+                PROPN: {<NNP>+} # Proper noun
+                ADJP: {<RB|RBR|RBS>*<JJ>} # Adjective phrase
+                ADVP: {<RB.*>+<VB.*><RB.*>*} # Adverb phrase'''
+            only_custom_pattern: If True, only the custom pattern will be used to extract MWEs, otherwise, the default patterns will be used as well.
+
+            Returns:
+                None
+        """
+        self.language = language.upper()
+        self.mwes: Dict[str, Dict[str, float]] = {}
+        self.reader = DataFrameReader(df, text_column)
+        self.mwe_extractor = None
+
+        mwe_patterns: str = ""
+        if language == "EN":
+            for _, value in EnMWEPatterns().patterns.items():
+                for v in value:
+                    mwe_patterns += v + "\n"
+        elif language == "DE":
+            for _, value in DeMWEPatterns().patterns.items():
+                for v in value:
+                    mwe_patterns += v + "\n"
+        else:
+            raise ValueError(
+                "Language not supported. Use 'EN' for English or 'DE' for German."
+            )
+
+        if custom_patterns:
+            if only_custom_patterns:
+                if not isinstance(only_custom_patterns, bool):
+                    raise TypeError(
+                        f"only_custom_patterns argument must be a boolean. Currently it is of type {type(only_custom_patterns)} \
+                        with a value of: {custom_patterns}."
+                    )
+                mwe_patterns = custom_patterns
+            else:
+                mwe_patterns += "\n" + custom_patterns
+
+        # Create an MWEPatternAssociation extractor object
+        self.mwe_extractor = MWEPatternAssociation(
+            association_measure=PMICalculator(
+                ngram_count_source=ngram_count_source,
+                ngram_count_file_path=ngram_count_file_path,
+            ),
+            pattern=mwe_patterns,
+        )
+
+    def extract_mwes(
+        self,
+        sort: bool = True,
+        top_n: Optional[int] = None,
+    ) -> dict[str, dict[str, float]]:
+        for sentence in tqdm(self.reader.get_sentences()):
+            try:
+                tokens = [
+                    word
+                    for word in word_tokenize(sentence)
+                    if word not in string.punctuation
+                ]
+            except Exception as E:
+                logger.warning(
+                    f"Could not word tokenize sentence: {sentence}.\
+                            \n{E}.\
+                            \nSkipping this sentence."
+                )
+                continue
+            if tokens:
+                returned_dict = self.mwe_extractor.measure_candidate_association(  # type: ignore
+                    tokens=tokens
+                )
+                for key, inner_dict in returned_dict.items():
+                    if key not in self.mwes:
+                        self.mwes[key] = {}
+                    self.mwes[key].update(inner_dict)
+
+        if sort:
+            for key, inner_dict in self.mwes.items():
+                tmp = sorted(inner_dict.items(), key=lambda item: item[1], reverse=True)
+                if top_n:
+                    tmp = tmp[:top_n]
+                self.mwes[key] = dict(tmp)
+
+        return self.mwes
+
+    def print_mwe_table(self):
+        sub_tables = []
+        for section, values in self.mwes.items():
+            if values:
+                formatted_values = {k: "{:.2f}".format(v) for k, v in values.items()}
+                headers = [section, "Association"]
+                table_data = list(formatted_values.items())
+                table_str = tabulate(
+                    table_data, headers=headers, tablefmt="double_outline"
+                )
+                sub_tables.append(table_str)
+        final_table = "\n\n".join(sub_tables)
+        print(final_table)
```

### Comparing `wordview-0.4.2/wordview/mwes/mwe_utils.py` & `wordview-1.0.0/wordview/mwes/mwe_utils.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.2/wordview/preprocessing/cleaning.py` & `wordview-1.0.0/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.2/wordview/text_analysis/core.py` & `wordview-1.0.0/wordview/text_analysis/core.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.2/wordview/text_analysis/wrapper.py` & `wordview-1.0.0/wordview/text_analysis/wrapper.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.2/PKG-INFO` & `wordview-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 0.4.2
+Version: 1.0.0
 Summary: Wordview is a Python package for text analysis.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -34,17 +34,15 @@
    :alt: PyPI - Python Version
 
 .. image:: https://img.shields.io/pypi/dm/wordview
    :alt: PyPI - Downloads
 
 Wordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.
 Wordview's Python API is open-source and available under the `MIT
-license <https://en.wikipedia.org/wiki/MIT_License>`__. We, however,
-offer a framework on top of Wordview for enterprise use under a commercial license. See this page for
-more information about this framework.
+license <https://en.wikipedia.org/wiki/MIT_License>`__.
 
 |cover|
 
 
 Usage
 ######
 
@@ -68,16 +66,16 @@
 
 Text Analysis
 *************
 Using this feature, you can have an overview of your text data in terms of various statistics, plots and distribution.
 See `text analysis documentation pages <./docs/source/textstats.rst>`__  for usage and examples.
 
 
-Label Analysis
-**************
+Analysis of Labels
+******************
 Wordview calculates several statistics for labels in labeled datasets whether they are at document or sequence level.
 See `label analysis documentation pages <./docs/source/labels.rst>`__ for usage and examples.
 
 
 Feature Extraction
 ###################
 
@@ -121,7 +119,8 @@
 Contributing
 ############
 
 Thank you for contributing to wordview! We and the users of this repo
 appreciate your efforts! You can visit the `contributing page <CONTRIBUTING.rst>`__ for detailed instructions about how you can contribute to Wordview.
 
 .. |cover| image:: docs/figs/cover.png
+
```

