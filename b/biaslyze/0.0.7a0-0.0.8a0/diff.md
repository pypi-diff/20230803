# Comparing `tmp/biaslyze-0.0.7a0.tar.gz` & `tmp/biaslyze-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biaslyze-0.0.7a0.tar", max compression
+gzip compressed data, was "biaslyze-0.0.8a0.tar", max compression
```

## Comparing `biaslyze-0.0.7a0.tar` & `biaslyze-0.0.8a0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1495 2023-04-21 09:03:51.243806 biaslyze-0.0.7a0/LICENSE
--rw-r--r--   0        0        0     3887 2023-07-14 16:24:22.552701 biaslyze-0.0.7a0/README.md
--rw-r--r--   0        0        0        0 2023-03-09 11:50:10.881651 biaslyze-0.0.7a0/biaslyze/__init__.py
--rw-r--r--   0        0        0    12586 2023-07-14 15:08:56.944651 biaslyze-0.0.7a0/biaslyze/_plotly_dashboard.py
--rw-r--r--   0        0        0     6931 2023-06-01 14:53:12.469622 biaslyze-0.0.7a0/biaslyze/_plotting.py
--rw-r--r--   0        0        0      281 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/augmentors.py
--rw-r--r--   0        0        0      220 2023-06-01 14:53:12.469622 biaslyze-0.0.7a0/biaslyze/bias_detectors/__init__.py
--rw-r--r--   0        0        0    14155 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/bias_detectors/counterfactual_biasdetector.py
--rw-r--r--   0        0        0     5547 2023-06-01 14:53:12.469622 biaslyze-0.0.7a0/biaslyze/bias_detectors/lime_biasdetector.py
--rw-r--r--   0        0        0     6546 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/concept_class.py
--rw-r--r--   0        0        0     1831 2023-06-01 14:53:12.469622 biaslyze-0.0.7a0/biaslyze/concept_detectors.py
--rw-r--r--   0        0        0    62578 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/concepts.py
--rw-r--r--   0        0        0    13637 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/results/counterfactual_detection_results.py
--rw-r--r--   0        0        0     4990 2023-06-01 14:53:12.469622 biaslyze-0.0.7a0/biaslyze/results/lime_detection_results.py
--rw-r--r--   0        0        0     2992 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/text_representation.py
--rw-r--r--   0        0        0     1756 2023-07-14 16:24:22.552701 biaslyze-0.0.7a0/pyproject.toml
--rw-r--r--   0        0        0     5589 1970-01-01 00:00:00.000000 biaslyze-0.0.7a0/setup.py
--rw-r--r--   0        0        0     5918 1970-01-01 00:00:00.000000 biaslyze-0.0.7a0/PKG-INFO
+-rw-r--r--   0        0        0     1495 2023-04-21 09:03:51.243806 biaslyze-0.0.8a0/LICENSE
+-rw-r--r--   0        0        0     3888 2023-08-02 13:09:25.190136 biaslyze-0.0.8a0/README.md
+-rw-r--r--   0        0        0        0 2023-03-09 11:50:10.881651 biaslyze-0.0.8a0/biaslyze/__init__.py
+-rw-r--r--   0        0        0    12586 2023-07-28 08:13:53.815096 biaslyze-0.0.8a0/biaslyze/_plotly_dashboard.py
+-rw-r--r--   0        0        0     6951 2023-08-03 09:37:02.307492 biaslyze-0.0.8a0/biaslyze/_plotting.py
+-rw-r--r--   0        0        0      281 2023-07-28 08:13:53.815096 biaslyze-0.0.8a0/biaslyze/augmentors.py
+-rw-r--r--   0        0        0      222 2023-08-03 09:34:35.495130 biaslyze-0.0.8a0/biaslyze/bias_detectors/__init__.py
+-rw-r--r--   0        0        0    15271 2023-08-03 09:35:42.667193 biaslyze-0.0.8a0/biaslyze/bias_detectors/counterfactual_biasdetector.py
+-rw-r--r--   0        0        0     5562 2023-08-03 09:35:42.667193 biaslyze-0.0.8a0/biaslyze/bias_detectors/lime_biasdetector.py
+-rw-r--r--   0        0        0     7693 2023-08-03 09:35:42.667193 biaslyze-0.0.8a0/biaslyze/concept_class.py
+-rw-r--r--   0        0        0     2518 2023-08-03 09:35:42.667193 biaslyze-0.0.8a0/biaslyze/concept_detectors.py
+-rw-r--r--   0        0        0    66476 2023-08-03 09:35:42.667193 biaslyze-0.0.8a0/biaslyze/concepts.py
+-rw-r--r--   0        0        0    14383 2023-08-03 09:37:02.307492 biaslyze-0.0.8a0/biaslyze/results/counterfactual_detection_results.py
+-rw-r--r--   0        0        0     4990 2023-06-01 14:53:12.469622 biaslyze-0.0.8a0/biaslyze/results/lime_detection_results.py
+-rw-r--r--   0        0        0     2992 2023-07-28 08:13:53.819096 biaslyze-0.0.8a0/biaslyze/text_representation.py
+-rw-r--r--   0        0        0      317 2023-08-03 09:35:42.667193 biaslyze-0.0.8a0/biaslyze/utils.py
+-rw-r--r--   0        0        0     1273 2023-08-03 09:59:18.477060 biaslyze-0.0.8a0/pyproject.toml
+-rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 biaslyze-0.0.8a0/setup.py
+-rw-r--r--   0        0        0     5084 1970-01-01 00:00:00.000000 biaslyze-0.0.8a0/PKG-INFO
```

### Comparing `biaslyze-0.0.7a0/LICENSE` & `biaslyze-0.0.8a0/LICENSE`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.7a0/README.md` & `biaslyze-0.0.8a0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 <div align="center">
-  <img src="resources/biaslyze-logo-no-bg.png" alt="Biaslyze" height="220px">
+  <img src="resources/biaslyze_logo_farbe_rgb.svg" alt="Biaslyze" width="40%">
   <h1>The NLP Bias Identification Toolkit</h1>
 </div>
 
 <div align="center">
     <a href="https://github.com/biaslyze-dev/biaslyze/blob/main/LICENSE">
         <img alt="licence" src="https://img.shields.io/github/license/biaslyze-dev/biaslyze">
     </a>
@@ -51,24 +51,24 @@
     texts=texts,
     predict_func=clf.predict_proba
 )
 
 # see a summary of the detection
 detection_res.report()
 
-# visualize the counterfactual scores
-detection_res.visualize_counterfactual_scores(concept="religion", top_n=10)
+# launch the dashboard visualize the counterfactual scores
+detection_res.dashboard(num_keywords=10)
 ```
 
 You will get results as Boxplots, among others, indicating the impact of keywords and concepts on the prediction of your model.
 Example output:
-![](resources/hatespeech_dl_scores_religion.png)
+![](resources/biaslyze-demo-box-plot.gif)
 
 
-See more detailed examples in the [tutorial](tutorials/tutorial-toxic-comments/).
+See more detailed examples in the [tutorial](https://biaslyze.org/tutorials/tutorial-toxic-comments/).
 
 
 ## Development setup
 
 - First you need to install poetry to manage your python environment: https://python-poetry.org/docs/#installation
 - Run `make install` to install the dependencies and get the spacy basemodels.
 - Now you can use `biaslyze` in your jupyter notebooks.
@@ -92,14 +92,14 @@
 ## Style guide
 
 We are using isort and black: `make style`
 For linting we are running ruff: `make lint`
 
 ## Contributing
 
-Follow the google style guide for python: https://google.github.io/styleguide/pyguide.html
+Follow the Google style guide for Python: https://google.github.io/styleguide/pyguide.html
 
 This project uses black, isort and ruff to enforce style. Apply it by running `make style` and `make lint`.
 
 ## Acknowledgements
 
 * Funded from March 2023 until August 2023 by ![logos of the "Bundesministerium für Bildung und Forschung", Prodotype Fund and OKFN-Deutschland](resources/pf_funding_logos.svg)
```

#### html2text {}

```diff
@@ -18,29 +18,29 @@
 download the required spacy models: ```bash python -m spacy download
 en_core_web_sm ``` ## Quickstart ```python from biaslyze.bias_detectors import
 CounterfactualBiasDetector bias_detector = CounterfactualBiasDetector() #
 detect bias in the model based on the given texts # here, clf is a scikit-learn
 text classification pipeline trained for a binary classification task
 detection_res = bias_detector.process( texts=texts,
 predict_func=clf.predict_proba ) # see a summary of the detection
-detection_res.report() # visualize the counterfactual scores
-detection_res.visualize_counterfactual_scores(concept="religion", top_n=10) ```
-You will get results as Boxplots, among others, indicating the impact of
-keywords and concepts on the prediction of your model. Example output: ![]
-(resources/hatespeech_dl_scores_religion.png) See more detailed examples in the
-[tutorial](tutorials/tutorial-toxic-comments/). ## Development setup - First
-you need to install poetry to manage your python environment: https://python-
-poetry.org/docs/#installation - Run `make install` to install the dependencies
-and get the spacy basemodels. - Now you can use `biaslyze` in your jupyter
-notebooks. ### Adding concepts and keywords You can add concepts and new
-keywords for existing concepts by editing [concepts.py](https://github.com/
-biaslyze-dev/biaslyze/blob/main/biaslyze/concepts.py). ## Preview/build the
-documentation with mkdocs To preview the documentation run `make doc-preview`.
-This will launch a preview of the documentation on `http://127.0.0.1:8000/`. To
-build the documentation html run `make doc`. ## Run the automated tests `make
-test` ## Style guide We are using isort and black: `make style` For linting we
-are running ruff: `make lint` ## Contributing Follow the google style guide for
-python: https://google.github.io/styleguide/pyguide.html This project uses
-black, isort and ruff to enforce style. Apply it by running `make style` and
-`make lint`. ## Acknowledgements * Funded from March 2023 until August 2023 by
-![logos of the "Bundesministerium fÃ¼r Bildung und Forschung", Prodotype Fund
-and OKFN-Deutschland](resources/pf_funding_logos.svg)
+detection_res.report() # launch the dashboard visualize the counterfactual
+scores detection_res.dashboard(num_keywords=10) ``` You will get results as
+Boxplots, among others, indicating the impact of keywords and concepts on the
+prediction of your model. Example output: ![](resources/biaslyze-demo-box-
+plot.gif) See more detailed examples in the [tutorial](https://biaslyze.org/
+tutorials/tutorial-toxic-comments/). ## Development setup - First you need to
+install poetry to manage your python environment: https://python-poetry.org/
+docs/#installation - Run `make install` to install the dependencies and get the
+spacy basemodels. - Now you can use `biaslyze` in your jupyter notebooks. ###
+Adding concepts and keywords You can add concepts and new keywords for existing
+concepts by editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/
+blob/main/biaslyze/concepts.py). ## Preview/build the documentation with mkdocs
+To preview the documentation run `make doc-preview`. This will launch a preview
+of the documentation on `http://127.0.0.1:8000/`. To build the documentation
+html run `make doc`. ## Run the automated tests `make test` ## Style guide We
+are using isort and black: `make style` For linting we are running ruff: `make
+lint` ## Contributing Follow the Google style guide for Python: https://
+google.github.io/styleguide/pyguide.html This project uses black, isort and
+ruff to enforce style. Apply it by running `make style` and `make lint`. ##
+Acknowledgements * Funded from March 2023 until August 2023 by ![logos of the
+"Bundesministerium fÃ¼r Bildung und Forschung", Prodotype Fund and OKFN-
+Deutschland](resources/pf_funding_logos.svg)
```

### Comparing `biaslyze-0.0.7a0/biaslyze/_plotly_dashboard.py` & `biaslyze-0.0.8a0/biaslyze/_plotly_dashboard.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.7a0/biaslyze/_plotting.py` & `biaslyze-0.0.8a0/biaslyze/_plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 """This module contains functions for plotting results and metrics."""
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 import yaml
-from bokeh.layouts import column
-from bokeh.models import ColumnDataSource, DataTable, TableColumn
-from bokeh.palettes import Spectral
-from bokeh.plotting import figure
-from bokeh.themes import Theme
 
 
 def _plot_box_plot(dataf: pd.DataFrame, top_n: Optional[int] = None):
     """Plot a box plot of scores.
 
     Args:
         dataf: A dataframe with scores for each sample.
@@ -61,14 +56,19 @@
         keywords: The keywords of the samples.
         keyword_positions: The positions of the keywords in the samples.
         num_tokens: The number of tokens in the samples.
         top_words: The top words of the samples.
         use_position: If True, use the normalized position for plotting.
         score_version: The name of the score version.
     """
+    from bokeh.layouts import column
+    from bokeh.models import ColumnDataSource, DataTable, TableColumn
+    from bokeh.palettes import Spectral
+    from bokeh.plotting import figure
+    from bokeh.themes import Theme
 
     # dataframe used for plotting
     plot_dataf = pd.DataFrame(
         {
             "text": texts,
             "bias_concepts": concepts,
             "score": scores,
```

### Comparing `biaslyze-0.0.7a0/biaslyze/bias_detectors/counterfactual_biasdetector.py` & `biaslyze-0.0.8a0/biaslyze/bias_detectors/counterfactual_biasdetector.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from biaslyze.concept_class import Concept, load_concepts
 from biaslyze.concept_detectors import KeywordConceptDetector
 from biaslyze.results.counterfactual_detection_results import (
     CounterfactualConceptResult,
     CounterfactualDetectionResult,
     CounterfactualSample,
 )
-from biaslyze.augmentors import CounterfactualTextAugmentor
 from biaslyze.text_representation import TextRepresentation, process_texts_with_spacy
 
 
 class CounterfactualBiasDetector:
     """Detect hints of bias by calculating counterfactual token scores for protected concepts.
 
     The counterfactual score is defined as the difference between the predicted
@@ -42,42 +41,61 @@
             texts=texts,
             predict_func=clf.predict_proba
         )
 
         # see a summary of the detection
         detection_res.report()
 
-        # visualize the counterfactual scores
-        detection_res.visualize_counterfactual_scores(concept="religion")
-
-        # visualize the counterfactual sample scores
-        detection_res.visualize_counterfactual_score_by_sample_histogram(concepts=["religion", "gender"])
+        # visualize the counterfactual scores as a dash dashboard
+        detection_res.dashboard()
         ```
 
     Attributes:
+        lang: The language of the texts. Decides which concepts and keywords to use.
         use_tokenizer: If keywords should only be searched in tokenized text. Can be useful for short keywords like 'she'.
-        concept_detector: an instance of KeywordConceptDetector
-        text_augmentor: an instance of CounterfactualTextAugmentor
     """
 
     def __init__(
         self,
+        lang: str = "en",
         use_tokenizer: bool = False,
-        concept_detector: KeywordConceptDetector = KeywordConceptDetector(),
-        text_augmentor: CounterfactualTextAugmentor = CounterfactualTextAugmentor(), 
     ):
+        self.lang = lang
         self.use_tokenizer = use_tokenizer
-        self.concept_detector = concept_detector
-        self.text_augmentor = text_augmentor
-
-        # overwrite use_tokenizer
-        self.concept_detector.use_tokenizer = self.use_tokenizer
+        self.concept_detector = KeywordConceptDetector(lang=lang, use_tokenizer=use_tokenizer)
 
         # load the concepts
-        self.concepts = load_concepts()
+        self.concepts = load_concepts(lang=lang)
+    
+    def register_concept(self, concept: Concept):
+        """Register a new, custom concept to the detector.
+
+        Example usage:
+        ```python
+        names_concept = Concept.from_dict_keyword_list(
+            name="names",
+            lang="de",
+            keywords=[{"keyword": "Hans", "function": ["name"]}],
+        )
+        bias_detector = CounterfactualBiasDetector(lang="de")
+        bias_detector.register_concept(names_concept)
+        ```
+        
+        Args:
+            concept: The concept to register.
+
+        Raises:
+            ValueError: If concept is not a Concept object.
+            ValueError: If a concept with this name is already registered.
+        """
+        if not isinstance(concept, Concept):
+            raise ValueError("concept must be a Concept object.")
+        if concept.name in [c.name for c in self.concepts]:
+            raise ValueError(f"Concept '{concept.name}' already registered.")
+        self.concepts.append(concept)
 
     def process(
         self,
         texts: List[str],
         predict_func: Callable[[List[str]], List[float]],
         labels: Optional[List[str]] = None,
         concepts_to_consider: Optional[List[str]] = [],
@@ -95,14 +113,18 @@
             max_counterfactual_samples_per_text: Optional. The maximum number of counterfactual samples to return per text. Defaults to None, which returns all possible counterfactual samples.
 
         Returns:
             A [CounterfactualDetectionResult](/biaslyze/results/counterfactual_detection_results/) object.
 
         Raises:
             ValueError: If texts or predict_func is not given.
+            ValueError: If concepts_to_consider is not a list.
+            ValueError: If max_counterfactual_samples is given but not a positive integer.
+            ValueError: If max_counterfactual_samples_per_text is given but not a positive integer.
+            ValueError: If concepts_to_consider contains a concept that is not registered.
         """
         if texts is None:
             raise ValueError("texts must be given.")
         if predict_func is None:
             raise ValueError("predict_func must be given.")
         if not isinstance(concepts_to_consider, list):
             raise ValueError("concepts_to_consider must be a list.")
@@ -116,17 +138,21 @@
         if max_counterfactual_samples_per_text:
             if (not isinstance(max_counterfactual_samples_per_text, int)) or (
                 max_counterfactual_samples_per_text < 1
             ):
                 raise ValueError(
                     "max_counterfactual_samples_per_text must be a positive integer."
                 )
+        if concepts_to_consider:
+            for c in concepts_to_consider:
+                if c not in [c.name for c in self.concepts]:
+                    raise ValueError(f"Concept '{c}' not found in language '{self.lang}'.")
 
         # find bias relevant texts
-        detected_texts = self.concept_detector.detect(texts)
+        detected_texts = self.concept_detector.detect(texts, concepts_to_consider=concepts_to_consider)
 
         # limit the number of counterfactual samples per text if max_counterfactual_samples is given
         if max_counterfactual_samples:
             max_counterfactual_samples_per_text = max_counterfactual_samples // len(
                 detected_texts
             ) + 1
 
@@ -140,15 +166,15 @@
             counterfactual_samples = _extract_counterfactual_concept_samples(
                 texts=detected_texts,
                 concept=concept,
                 labels=labels,
                 n_texts=max_counterfactual_samples_per_text,
             )
             if not counterfactual_samples:
-                logger.warning(f"No samples containing {concept.name} found. Skipping.")
+                logger.warning(f"No samples containing '{concept.name}' found. Skipping.")
                 continue
 
             # calculate counterfactual scores for each keyword
             for keyword in tqdm(concept.keywords):
                 # get the counterfactual scores
                 try:
                     counterfactual_scores = _calculate_counterfactual_scores(
```

### Comparing `biaslyze-0.0.7a0/biaslyze/bias_detectors/lime_biasdetector.py` & `biaslyze-0.0.8a0/biaslyze/bias_detectors/lime_biasdetector.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 from eli5.lime import TextExplainer
 from loguru import logger
 from tqdm import tqdm
 
 from biaslyze.concept_detectors import KeywordConceptDetector
-from biaslyze.concepts import CONCEPTS
+from biaslyze.concepts import CONCEPTS_EN as CONCEPTS
 from biaslyze.results.lime_detection_results import (
     LimeDetectionResult,
     LimeSampleResult,
 )
 
 
 class LimeBiasDetector:
```

### Comparing `biaslyze-0.0.7a0/biaslyze/concepts.py` & `biaslyze-0.0.8a0/biaslyze/concepts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,69 @@
 """Dict of concepts with related keywords.
 
 Function abbreviations can be found here: https://v2.spacy.io/api/annotation#pos-tagging 
 """
-CONCEPTS = {
+CONCEPTS_DE = {
+    "gender": [
+        {"keyword": "sie", "function": ["subject"], "category": "PRON"},
+        {"keyword": "er", "function": ["subject"], "category": "PRON"},
+        {"keyword": "ihr", "function": ["object"], "category": "PRON"},
+        {"keyword": "ihn", "function": ["object"], "category": "PRON"},
+        {"keyword": "ihre", "function": ["object"], "category": "PRON"},
+        {"keyword": "ihm", "function": ["object"], "category": "PRON"},
+        {"keyword": "seine", "function": ["object"], "category": "PRON"},
+        {"keyword": "seinen", "function": ["object"], "category": "PRON"},
+        {"keyword": "seiner", "function": ["object"], "category": "PRON"},
+        {"keyword": "seines", "function": ["object"], "category": "PRON"},
+        {"keyword": "ihres", "function": ["object"], "category": "PRON"},
+        {"keyword": "ihren", "function": ["object"], "category": "PRON"},
+        {"keyword": "ihrem", "function": ["object"], "category": "PRON"},
+        {"keyword": "ihnen", "function": ["object"], "category": "PRON"},
+    ],
+    "religion": [
+        {"keyword": "christ", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "christin", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "christen", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "christentum", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "christlich", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "christliche", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "christlichen", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "christlicher", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "christliches", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "christinnen", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "christi", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "christus", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "jude", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "jüdin", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "jüdisch", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "jüdische", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "jüdischen", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "jüdischer", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "jüdisches", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "jüdisches", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "judentum", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "muslim", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "muslima", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "muslimisch", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "muslimische", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "muslimischen", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "muslimischer", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "muslimisches", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "muslime", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "islam", "function": ["NOUN"], "category": "religion"},
+        {"keyword": "islamisch", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "islamische", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "islamischen", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "islamischer", "function": ["ADJ"], "category": "religion"},
+        {"keyword": "islamisches", "function": ["ADJ"], "category": "religion"},
+    ],        
+}
+
+
+CONCEPTS_EN = {
     "nationality": [
         {"keyword": "california", "function": ["NOUN"], "category": "region"},
         {"keyword": "afghanistan", "function": ["NOUN"], "category": "country"},
         {"keyword": "albania", "function": ["NOUN"], "category": "country"},
         {"keyword": "algeria", "function": ["NOUN"], "category": "country"},
         {"keyword": "samoa", "function": ["NOUN"], "category": "country"},
         {"keyword": "andorra", "function": ["NOUN"], "category": "country"},
```

### Comparing `biaslyze-0.0.7a0/biaslyze/results/counterfactual_detection_results.py` & `biaslyze-0.0.8a0/biaslyze/results/counterfactual_detection_results.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This module contains classes to store and process the results of counterfactual bias detection runs."""
 import warnings
+import dill
 from collections import defaultdict
 from typing import List, Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
@@ -68,14 +69,39 @@
     Attributes:
         concept_results: A list of CounterfactualConceptResult objects.
     """
 
     def __init__(self, concept_results: List[CounterfactualConceptResult]):
         self.concept_results = concept_results
 
+    def save(self, path: str):
+        """Save the detection result to a file.
+
+        Load again by
+
+        ```python
+        from biaslyze.utils import load_results
+
+        results = load_results(path)
+        ```
+        
+        Args:
+            path (str): The path to save the result to.
+
+        Raises:
+            ValueError: If the path is not valid.
+        """
+        try:
+            with open(path, "wb") as f:
+                dill.dump(self, f)
+        except ValueError:
+            warnings.warn(
+                "Could not save result. Please make sure that the path is valid."
+            )
+
     def _get_result_by_concept(self, concept: str) -> pd.DataFrame:
         """Get the result for a given concept.
 
         Args:
             concept: The concept for which to get the result.
 
         Returns:
@@ -245,125 +271,125 @@
             scores=all_scores,
             keywords=[sample.keyword for sample in all_samples],
             score_version="CounterfactualSampleScore",
         )
 
         return dashboard
 
-    def visualize_counterfactual_score_by_sample(self, concept: str):
-        """Visualize the counterfactual scores for each sample for a given concept."""
-        import yaml
-        from bokeh.layouts import column
-        from bokeh.models import ColumnDataSource, HoverTool, Slider
-        from bokeh.palettes import Category10_10
-        from bokeh.plotting import figure
-        from bokeh.themes import Theme
-        from sentence_transformers import SentenceTransformer
-        from umap import UMAP
-
-        dataf = self._get_result_by_concept(concept=concept)
-        samples = self._get_counterfactual_samples_by_concept(concept=concept)
-
-        # get the original samples
-        original_samples = [
-            sample for sample in samples if (sample.keyword == sample.orig_keyword)
-        ]
-
-        # get text representations in 2d
-        docs = [sample.text for sample in original_samples]
-        sentence_model = SentenceTransformer("all-MiniLM-L6-v2")
-        embeddings = sentence_model.encode(docs, show_progress_bar=True)
-
-        # Train BERTopic
-        reduced_embeddings = UMAP(
-            n_neighbors=10, n_components=2, min_dist=0.0, metric="cosine"
-        ).fit_transform(embeddings)
-
-        # build the visualization
-        def bkapp(doc):
-            hover_tool = HoverTool(
-                tooltips=[
-                    ("Text", "@text"),
-                    ("Keywords", "@keywords"),
-                    ("Counterfactual score", "@counterfactual_sample_score"),
-                ]
-            )
-            p = figure(
-                width=1200,
-                height=800,
-                tools=["pan", "wheel_zoom", "box_zoom", "reset", hover_tool],
-            )
-
-            bias_intensity = np.array(dataf.mean(axis=1))
-
-            # configure
-            df = pd.DataFrame(
-                dict(
-                    text=[sample.text for sample in original_samples],
-                    keywords=[sample.keyword for sample in original_samples],
-                    x=reduced_embeddings[:, 0],
-                    y=reduced_embeddings[:, 1],
-                    color=[
-                        Category10_10[idx] for idx in (bias_intensity <= 0).astype(int)
-                    ],
-                    bias_intensity=500 * np.abs(bias_intensity),
-                    counterfactual_sample_score=np.round(bias_intensity, 4),
-                )
-            )
-            source = ColumnDataSource(data=df)
-
-            # add a circle renderer with a size, color, and alpha
-            p.scatter(
-                "x",
-                "y",
-                source=source,
-                color="color",
-                size="bias_intensity",
-                alpha=0.3,
-            )
-
-            # p.legend.location = "top_left"
-            # p.legend.click_policy="hide"
-
-            # slider
-            threshold = Slider(
-                title="threshold",
-                value=0.0,
-                start=0.0,
-                end=df.bias_intensity.max(),
-                step=0.01,
-                width=750,
-            )
-
-            def update_data(attrname, old, new):
-                # Get the current slider values
-                t = threshold.value
-                new_df = df.copy()
-                new_df["bias_intensity"] = new_df.bias_intensity.apply(
-                    lambda x: x if x >= t else 0.0
-                )
-                source.data = new_df
-
-            threshold.on_change("value", update_data)
-
-            doc.add_root(column(threshold, p, width=800))
-
-            # show the results
-            doc.theme = Theme(
-                json=yaml.load(
-                    """
-                attrs:
-                    figure:
-                        background_fill_color: "#DDDDDD"
-                        outline_line_color: white
-                        toolbar_location: above
-                        height: 800
-                        width: 1200
-                    Grid:
-                        grid_line_dash: [6, 4]
-                        grid_line_color: white
-            """,
-                    Loader=yaml.FullLoader,
-                )
-            )
-
-        return bkapp
+#    def visualize_counterfactual_score_by_sample(self, concept: str):
+#        """Visualize the counterfactual scores for each sample for a given concept."""
+#        import yaml
+#        from bokeh.layouts import column
+#        from bokeh.models import ColumnDataSource, HoverTool, Slider
+#        from bokeh.palettes import Category10_10
+#        from bokeh.plotting import figure
+#        from bokeh.themes import Theme
+#        from sentence_transformers import SentenceTransformer
+#        from umap import UMAP
+#
+#        dataf = self._get_result_by_concept(concept=concept)
+#        samples = self._get_counterfactual_samples_by_concept(concept=concept)
+#
+#        # get the original samples
+#        original_samples = [
+#            sample for sample in samples if (sample.keyword == sample.orig_keyword)
+#        ]
+#
+#        # get text representations in 2d
+#        docs = [sample.text for sample in original_samples]
+#        sentence_model = SentenceTransformer("all-MiniLM-L6-v2")
+#        embeddings = sentence_model.encode(docs, show_progress_bar=True)
+#
+#        # Train BERTopic
+#        reduced_embeddings = UMAP(
+#            n_neighbors=10, n_components=2, min_dist=0.0, metric="cosine"
+#        ).fit_transform(embeddings)
+#
+#        # build the visualization
+#        def bkapp(doc):
+#            hover_tool = HoverTool(
+#                tooltips=[
+#                    ("Text", "@text"),
+#                    ("Keywords", "@keywords"),
+#                    ("Counterfactual score", "@counterfactual_sample_score"),
+#                ]
+#            )
+#            p = figure(
+#                width=1200,
+#                height=800,
+#                tools=["pan", "wheel_zoom", "box_zoom", "reset", hover_tool],
+#            )
+#
+#            bias_intensity = np.array(dataf.mean(axis=1))
+#
+#            # configure
+#            df = pd.DataFrame(
+#                dict(
+#                    text=[sample.text for sample in original_samples],
+#                    keywords=[sample.keyword for sample in original_samples],
+#                    x=reduced_embeddings[:, 0],
+#                    y=reduced_embeddings[:, 1],
+#                    color=[
+#                        Category10_10[idx] for idx in (bias_intensity <= 0).astype(int)
+#                    ],
+#                    bias_intensity=500 * np.abs(bias_intensity),
+#                    counterfactual_sample_score=np.round(bias_intensity, 4),
+#                )
+#            )
+#            source = ColumnDataSource(data=df)
+#
+#            # add a circle renderer with a size, color, and alpha
+#            p.scatter(
+#                "x",
+#                "y",
+#                source=source,
+#                color="color",
+#                size="bias_intensity",
+#                alpha=0.3,
+#            )
+#
+#            # p.legend.location = "top_left"
+#            # p.legend.click_policy="hide"
+#
+#            # slider
+#            threshold = Slider(
+#                title="threshold",
+#                value=0.0,
+#                start=0.0,
+#                end=df.bias_intensity.max(),
+#                step=0.01,
+#                width=750,
+#            )
+#
+#            def update_data(attrname, old, new):
+#                # Get the current slider values
+#                t = threshold.value
+#                new_df = df.copy()
+#                new_df["bias_intensity"] = new_df.bias_intensity.apply(
+#                    lambda x: x if x >= t else 0.0
+#                )
+#                source.data = new_df
+#
+#            threshold.on_change("value", update_data)
+#
+#            doc.add_root(column(threshold, p, width=800))
+#
+#            # show the results
+#            doc.theme = Theme(
+#                json=yaml.load(
+#                    """
+#                attrs:
+#                    figure:
+#                        background_fill_color: "#DDDDDD"
+#                        outline_line_color: white
+#                        toolbar_location: above
+#                        height: 800
+#                        width: 1200
+#                    Grid:
+#                        grid_line_dash: [6, 4]
+#                        grid_line_color: white
+#            """,
+#                    Loader=yaml.FullLoader,
+#                )
+#            )
+#
+#        return bkapp
```

### Comparing `biaslyze-0.0.7a0/biaslyze/results/lime_detection_results.py` & `biaslyze-0.0.8a0/biaslyze/results/lime_detection_results.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.7a0/biaslyze/text_representation.py` & `biaslyze-0.0.8a0/biaslyze/text_representation.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.7a0/pyproject.toml` & `biaslyze-0.0.8a0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biaslyze"
-version = "0.0.7-alpha"
+version = "0.0.8-alpha"
 description = "The NLP Bias Identification Toolkit"
 authors = [
     "Tobias Sterbak & Stina Lohmüller <hello@biaslyze.org>",
 ]
 maintainers = [
     "Tobias Sterbak <hello@tobiassterbak.com>",
     "Stina Lohmüller <slohmueller@posteo.de>",
@@ -25,34 +25,18 @@
 numpy = "1.23.2"
 pandas = "^1.5.3"
 scipy = "1.8.0"
 jupyterlab = "^3.5.2"
 scikit-learn = "^1.2.0"
 loguru = "^0.6.0"
 matplotlib = "^3.7.1"
-bokeh = "^3.1.0"
-eli5 = "^0.13.0"
 spacy = "^3.5.0"
-transformers = "^4.26.1"
-bertopic = "0.13.0"
-umap-learn = "^0.5.3"
-nvidia-cublas-cu11 = "^11.11.3.6"
-nvidia-cudnn-cu11 = "^8.9.1.23"
-nvidia-cuda-cupti-cu11 = "^11.8.87"
-nvidia-cuda-nvrtc-cu11 = "^11.8.89"
-nvidia-cuda-runtime-cu11 = "^11.8.89"
-nvidia-cufft-cu11 = "^10.9.0.58"
-nvidia-curand-cu11 = "^10.3.0.86"
-nvidia-cusolver-cu11 = "^11.4.1.48"
-nvidia-cusparse-cu11 = "^11.7.5.86"
-nvidia-nccl-cu11 = "^2.16.5"
-nvidia-nvtx-cu11 = "^11.8.86"
-triton = "^2.0.0.post1"
 dash = "^2.11.1"
 plotly = "^5.15.0"
+dill = "^0.3.7"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs-material = "^9.1.1"
 material-plausible-plugin = "^0.2.0"
 mkgendocs = "^0.9.2"
 Pillow = "^10.0.0"
 CairoSVG = "^2.7.0"
```

### Comparing `biaslyze-0.0.7a0/setup.py` & `biaslyze-0.0.8a0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,47 +4,31 @@
 packages = \
 ['biaslyze', 'biaslyze.bias_detectors', 'biaslyze.results']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bertopic==0.13.0',
- 'bokeh>=3.1.0,<4.0.0',
- 'dash>=2.11.1,<3.0.0',
- 'eli5>=0.13.0,<0.14.0',
+['dash>=2.11.1,<3.0.0',
+ 'dill>=0.3.7,<0.4.0',
  'jupyterlab>=3.5.2,<4.0.0',
  'loguru>=0.6.0,<0.7.0',
  'matplotlib>=3.7.1,<4.0.0',
  'numpy==1.23.2',
- 'nvidia-cublas-cu11>=11.11.3.6,<12.0.0.0',
- 'nvidia-cuda-cupti-cu11>=11.8.87,<12.0.0',
- 'nvidia-cuda-nvrtc-cu11>=11.8.89,<12.0.0',
- 'nvidia-cuda-runtime-cu11>=11.8.89,<12.0.0',
- 'nvidia-cudnn-cu11>=8.9.1.23,<9.0.0.0',
- 'nvidia-cufft-cu11>=10.9.0.58,<11.0.0.0',
- 'nvidia-curand-cu11>=10.3.0.86,<11.0.0.0',
- 'nvidia-cusolver-cu11>=11.4.1.48,<12.0.0.0',
- 'nvidia-cusparse-cu11>=11.7.5.86,<12.0.0.0',
- 'nvidia-nccl-cu11>=2.16.5,<3.0.0',
- 'nvidia-nvtx-cu11>=11.8.86,<12.0.0',
  'pandas>=1.5.3,<2.0.0',
  'plotly>=5.15.0,<6.0.0',
  'scikit-learn>=1.2.0,<2.0.0',
  'scipy==1.8.0',
- 'spacy>=3.5.0,<4.0.0',
- 'transformers>=4.26.1,<5.0.0',
- 'triton>=2.0.0.post1,<3.0.0',
- 'umap-learn>=0.5.3,<0.6.0']
+ 'spacy>=3.5.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'biaslyze',
-    'version': '0.0.7a0',
+    'version': '0.0.8a0',
     'description': 'The NLP Bias Identification Toolkit',
-    'long_description': '\n<div align="center">\n  <img src="resources/biaslyze-logo-no-bg.png" alt="Biaslyze" height="220px">\n  <h1>The NLP Bias Identification Toolkit</h1>\n</div>\n\n<div align="center">\n    <a href="https://github.com/biaslyze-dev/biaslyze/blob/main/LICENSE">\n        <img alt="licence" src="https://img.shields.io/github/license/biaslyze-dev/biaslyze">\n    </a>\n    <a href="https://pypi.org/project/biaslyze/">\n        <img alt="pypi" src="https://img.shields.io/pypi/v/biaslyze">\n    </a>\n    <a href="https://pypi.org/project/biaslyze/">\n        <img alt="pypi" src="https://img.shields.io/pypi/pyversions/biaslyze">\n    </a>\n</div>\n\n\nBias is often subtle and difficult to detect in NLP models, as the protected attributes are less obvious and can take many forms in language (e.g. proxies, double meanings, ambiguities etc.). Therefore, technical bias testing is a key step in avoiding algorithmically mediated discrimination. However, it is currently conducted too rarely due to the effort involved, missing resources or lack of awareness for the problem.\n\nBiaslyze helps to get started with the analysis of bias within NLP models and offers a concrete entry point for further impact assessments and mitigation measures. Especially for developers, researchers and teams with limited resources, our toolbox offers a low-effort approach to bias testing in NLP use cases.\n\n## Supported Models\n\nAll text classification models with probability output are supported. This includes models from scikit-learn, tensorflow, pytorch, huggingface transformers and others. \nSee the tutorials section for examples.\n\n## Installation\n\nInstallation can be done using pypi:\n```bash\npip install biaslyze\n```\n\nThen you need to download the required spacy models:\n```bash\npython -m spacy download en_core_web_sm\n```\n\n## Quickstart\n\n```python\nfrom biaslyze.bias_detectors import CounterfactualBiasDetector\n\nbias_detector = CounterfactualBiasDetector()\n\n# detect bias in the model based on the given texts\n# here, clf is a scikit-learn text classification pipeline trained for a binary classification task\ndetection_res = bias_detector.process(\n    texts=texts,\n    predict_func=clf.predict_proba\n)\n\n# see a summary of the detection\ndetection_res.report()\n\n# visualize the counterfactual scores\ndetection_res.visualize_counterfactual_scores(concept="religion", top_n=10)\n```\n\nYou will get results as Boxplots, among others, indicating the impact of keywords and concepts on the prediction of your model.\nExample output:\n![](resources/hatespeech_dl_scores_religion.png)\n\n\nSee more detailed examples in the [tutorial](tutorials/tutorial-toxic-comments/).\n\n\n## Development setup\n\n- First you need to install poetry to manage your python environment: https://python-poetry.org/docs/#installation\n- Run `make install` to install the dependencies and get the spacy basemodels.\n- Now you can use `biaslyze` in your jupyter notebooks.\n\n\n### Adding concepts and keywords\n\nYou can add concepts and new keywords for existing concepts by editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/blob/main/biaslyze/concepts.py).\n\n## Preview/build the documentation with mkdocs\n\nTo preview the documentation run `make doc-preview`. This will launch a preview of the documentation on `http://127.0.0.1:8000/`.\nTo build the documentation html run `make doc`.\n\n\n## Run the automated tests\n\n`make test`\n\n\n## Style guide\n\nWe are using isort and black: `make style`\nFor linting we are running ruff: `make lint`\n\n## Contributing\n\nFollow the google style guide for python: https://google.github.io/styleguide/pyguide.html\n\nThis project uses black, isort and ruff to enforce style. Apply it by running `make style` and `make lint`.\n\n## Acknowledgements\n\n* Funded from March 2023 until August 2023 by ![logos of the "Bundesministerium für Bildung und Forschung", Prodotype Fund and OKFN-Deutschland](resources/pf_funding_logos.svg)\n',
+    'long_description': '\n<div align="center">\n  <img src="resources/biaslyze_logo_farbe_rgb.svg" alt="Biaslyze" width="40%">\n  <h1>The NLP Bias Identification Toolkit</h1>\n</div>\n\n<div align="center">\n    <a href="https://github.com/biaslyze-dev/biaslyze/blob/main/LICENSE">\n        <img alt="licence" src="https://img.shields.io/github/license/biaslyze-dev/biaslyze">\n    </a>\n    <a href="https://pypi.org/project/biaslyze/">\n        <img alt="pypi" src="https://img.shields.io/pypi/v/biaslyze">\n    </a>\n    <a href="https://pypi.org/project/biaslyze/">\n        <img alt="pypi" src="https://img.shields.io/pypi/pyversions/biaslyze">\n    </a>\n</div>\n\n\nBias is often subtle and difficult to detect in NLP models, as the protected attributes are less obvious and can take many forms in language (e.g. proxies, double meanings, ambiguities etc.). Therefore, technical bias testing is a key step in avoiding algorithmically mediated discrimination. However, it is currently conducted too rarely due to the effort involved, missing resources or lack of awareness for the problem.\n\nBiaslyze helps to get started with the analysis of bias within NLP models and offers a concrete entry point for further impact assessments and mitigation measures. Especially for developers, researchers and teams with limited resources, our toolbox offers a low-effort approach to bias testing in NLP use cases.\n\n## Supported Models\n\nAll text classification models with probability output are supported. This includes models from scikit-learn, tensorflow, pytorch, huggingface transformers and others. \nSee the tutorials section for examples.\n\n## Installation\n\nInstallation can be done using pypi:\n```bash\npip install biaslyze\n```\n\nThen you need to download the required spacy models:\n```bash\npython -m spacy download en_core_web_sm\n```\n\n## Quickstart\n\n```python\nfrom biaslyze.bias_detectors import CounterfactualBiasDetector\n\nbias_detector = CounterfactualBiasDetector()\n\n# detect bias in the model based on the given texts\n# here, clf is a scikit-learn text classification pipeline trained for a binary classification task\ndetection_res = bias_detector.process(\n    texts=texts,\n    predict_func=clf.predict_proba\n)\n\n# see a summary of the detection\ndetection_res.report()\n\n# launch the dashboard visualize the counterfactual scores\ndetection_res.dashboard(num_keywords=10)\n```\n\nYou will get results as Boxplots, among others, indicating the impact of keywords and concepts on the prediction of your model.\nExample output:\n![](resources/biaslyze-demo-box-plot.gif)\n\n\nSee more detailed examples in the [tutorial](https://biaslyze.org/tutorials/tutorial-toxic-comments/).\n\n\n## Development setup\n\n- First you need to install poetry to manage your python environment: https://python-poetry.org/docs/#installation\n- Run `make install` to install the dependencies and get the spacy basemodels.\n- Now you can use `biaslyze` in your jupyter notebooks.\n\n\n### Adding concepts and keywords\n\nYou can add concepts and new keywords for existing concepts by editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/blob/main/biaslyze/concepts.py).\n\n## Preview/build the documentation with mkdocs\n\nTo preview the documentation run `make doc-preview`. This will launch a preview of the documentation on `http://127.0.0.1:8000/`.\nTo build the documentation html run `make doc`.\n\n\n## Run the automated tests\n\n`make test`\n\n\n## Style guide\n\nWe are using isort and black: `make style`\nFor linting we are running ruff: `make lint`\n\n## Contributing\n\nFollow the Google style guide for Python: https://google.github.io/styleguide/pyguide.html\n\nThis project uses black, isort and ruff to enforce style. Apply it by running `make style` and `make lint`.\n\n## Acknowledgements\n\n* Funded from March 2023 until August 2023 by ![logos of the "Bundesministerium für Bildung und Forschung", Prodotype Fund and OKFN-Deutschland](resources/pf_funding_logos.svg)\n',
     'author': 'Tobias Sterbak & Stina Lohmüller',
     'author_email': 'hello@biaslyze.org',
     'maintainer': 'Tobias Sterbak',
     'maintainer_email': 'hello@tobiassterbak.com',
     'url': 'https://biaslyze.org',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,24 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['biaslyze',
 'biaslyze.bias_detectors', 'biaslyze.results'] package_data = \ {'': ['*']}
-install_requires = \ ['bertopic==0.13.0', 'bokeh>=3.1.0,<4.0.0',
-'dash>=2.11.1,<3.0.0', 'eli5>=0.13.0,<0.14.0', 'jupyterlab>=3.5.2,<4.0.0',
-'loguru>=0.6.0,<0.7.0', 'matplotlib>=3.7.1,<4.0.0', 'numpy==1.23.2', 'nvidia-
-cublas-cu11>=11.11.3.6,<12.0.0.0', 'nvidia-cuda-cupti-cu11>=11.8.87,<12.0.0',
-'nvidia-cuda-nvrtc-cu11>=11.8.89,<12.0.0', 'nvidia-cuda-runtime-
-cu11>=11.8.89,<12.0.0', 'nvidia-cudnn-cu11>=8.9.1.23,<9.0.0.0', 'nvidia-cufft-
-cu11>=10.9.0.58,<11.0.0.0', 'nvidia-curand-cu11>=10.3.0.86,<11.0.0.0', 'nvidia-
-cusolver-cu11>=11.4.1.48,<12.0.0.0', 'nvidia-cusparse-
-cu11>=11.7.5.86,<12.0.0.0', 'nvidia-nccl-cu11>=2.16.5,<3.0.0', 'nvidia-nvtx-
-cu11>=11.8.86,<12.0.0', 'pandas>=1.5.3,<2.0.0', 'plotly>=5.15.0,<6.0.0',
-'scikit-learn>=1.2.0,<2.0.0', 'scipy==1.8.0', 'spacy>=3.5.0,<4.0.0',
-'transformers>=4.26.1,<5.0.0', 'triton>=2.0.0.post1,<3.0.0', 'umap-
-learn>=0.5.3,<0.6.0'] setup_kwargs = { 'name': 'biaslyze', 'version':
-'0.0.7a0', 'description': 'The NLP Bias Identification Toolkit',
-'long_description': '\n
+install_requires = \ ['dash>=2.11.1,<3.0.0', 'dill>=0.3.7,<0.4.0',
+'jupyterlab>=3.5.2,<4.0.0', 'loguru>=0.6.0,<0.7.0', 'matplotlib>=3.7.1,<4.0.0',
+'numpy==1.23.2', 'pandas>=1.5.3,<2.0.0', 'plotly>=5.15.0,<6.0.0', 'scikit-
+learn>=1.2.0,<2.0.0', 'scipy==1.8.0', 'spacy>=3.5.0,<4.0.0'] setup_kwargs =
+{ 'name': 'biaslyze', 'version': '0.0.8a0', 'description': 'The NLP Bias
+Identification Toolkit', 'long_description': '\n
                                 \n [Biaslyze]\n
                ****** The NLP Bias Identification Toolkit ******
                                       \n
 \n\n
                 \n \n_[licence]\n\n \n_[pypi]\n\n \n_[pypi]\n\n
 \n\n\nBias is often subtle and difficult to detect in NLP models, as the
 protected attributes are less obvious and can take many forms in language (e.g.
@@ -38,35 +29,35 @@
 \n```bash\npython -m spacy download en_core_web_sm\n```\n\n##
 Quickstart\n\n```python\nfrom biaslyze.bias_detectors import
 CounterfactualBiasDetector\n\nbias_detector = CounterfactualBiasDetector()\n\n#
 detect bias in the model based on the given texts\n# here, clf is a scikit-
 learn text classification pipeline trained for a binary classification
 task\ndetection_res = bias_detector.process(\n texts=texts,\n
 predict_func=clf.predict_proba\n)\n\n# see a summary of the
-detection\ndetection_res.report()\n\n# visualize the counterfactual
-scores\ndetection_res.visualize_counterfactual_scores(concept="religion",
-top_n=10)\n```\n\nYou will get results as Boxplots, among others, indicating
-the impact of keywords and concepts on the prediction of your model.\nExample
-output:\n![](resources/hatespeech_dl_scores_religion.png)\n\n\nSee more
-detailed examples in the [tutorial](tutorials/tutorial-toxic-comments/
-).\n\n\n## Development setup\n\n- First you need to install poetry to manage
-your python environment: https://python-poetry.org/docs/#installation\n- Run
-`make install` to install the dependencies and get the spacy basemodels.\n- Now
-you can use `biaslyze` in your jupyter notebooks.\n\n\n### Adding concepts and
-keywords\n\nYou can add concepts and new keywords for existing concepts by
-editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/blob/main/
-biaslyze/concepts.py).\n\n## Preview/build the documentation with mkdocs\n\nTo
-preview the documentation run `make doc-preview`. This will launch a preview of
-the documentation on `http://127.0.0.1:8000/`.\nTo build the documentation html
-run `make doc`.\n\n\n## Run the automated tests\n\n`make test`\n\n\n## Style
-guide\n\nWe are using isort and black: `make style`\nFor linting we are running
-ruff: `make lint`\n\n## Contributing\n\nFollow the google style guide for
-python: https://google.github.io/styleguide/pyguide.html\n\nThis project uses
-black, isort and ruff to enforce style. Apply it by running `make style` and
-`make lint`.\n\n## Acknowledgements\n\n* Funded from March 2023 until August
-2023 by ![logos of the "Bundesministerium fÃ¼r Bildung und Forschung",
-Prodotype Fund and OKFN-Deutschland](resources/pf_funding_logos.svg)\n',
-'author': 'Tobias Sterbak & Stina LohmÃ¼ller', 'author_email':
-'hello@biaslyze.org', 'maintainer': 'Tobias Sterbak', 'maintainer_email':
-'hello@tobiassterbak.com', 'url': 'https://biaslyze.org', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.10,<3.11', } setup(**setup_kwargs)
+detection\ndetection_res.report()\n\n# launch the dashboard visualize the
+counterfactual scores\ndetection_res.dashboard(num_keywords=10)\n```\n\nYou
+will get results as Boxplots, among others, indicating the impact of keywords
+and concepts on the prediction of your model.\nExample output:\n![](resources/
+biaslyze-demo-box-plot.gif)\n\n\nSee more detailed examples in the [tutorial]
+(https://biaslyze.org/tutorials/tutorial-toxic-comments/).\n\n\n## Development
+setup\n\n- First you need to install poetry to manage your python environment:
+https://python-poetry.org/docs/#installation\n- Run `make install` to install
+the dependencies and get the spacy basemodels.\n- Now you can use `biaslyze` in
+your jupyter notebooks.\n\n\n### Adding concepts and keywords\n\nYou can add
+concepts and new keywords for existing concepts by editing [concepts.py](https:
+//github.com/biaslyze-dev/biaslyze/blob/main/biaslyze/concepts.py).\n\n##
+Preview/build the documentation with mkdocs\n\nTo preview the documentation run
+`make doc-preview`. This will launch a preview of the documentation on `http://
+127.0.0.1:8000/`.\nTo build the documentation html run `make doc`.\n\n\n## Run
+the automated tests\n\n`make test`\n\n\n## Style guide\n\nWe are using isort
+and black: `make style`\nFor linting we are running ruff: `make lint`\n\n##
+Contributing\n\nFollow the Google style guide for Python: https://
+google.github.io/styleguide/pyguide.html\n\nThis project uses black, isort and
+ruff to enforce style. Apply it by running `make style` and `make lint`.\n\n##
+Acknowledgements\n\n* Funded from March 2023 until August 2023 by ![logos of
+the "Bundesministerium fÃ¼r Bildung und Forschung", Prodotype Fund and OKFN-
+Deutschland](resources/pf_funding_logos.svg)\n', 'author': 'Tobias Sterbak &
+Stina LohmÃ¼ller', 'author_email': 'hello@biaslyze.org', 'maintainer': 'Tobias
+Sterbak', 'maintainer_email': 'hello@tobiassterbak.com', 'url': 'https://
+biaslyze.org', 'packages': packages, 'package_data': package_data,
+'install_requires': install_requires, 'python_requires': '>=3.10,<3.11', }
+setup(**setup_kwargs)
```

### Comparing `biaslyze-0.0.7a0/PKG-INFO` & `biaslyze-0.0.8a0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,41 @@
 Metadata-Version: 2.1
 Name: biaslyze
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: The NLP Bias Identification Toolkit
 Home-page: https://biaslyze.org
 License: BSD-3-Clause
 Keywords: NLP,bias,ethics,fairness
 Author: Tobias Sterbak & Stina Lohmüller
 Author-email: hello@biaslyze.org
 Maintainer: Tobias Sterbak
 Maintainer-email: hello@tobiassterbak.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: bertopic (==0.13.0)
-Requires-Dist: bokeh (>=3.1.0,<4.0.0)
 Requires-Dist: dash (>=2.11.1,<3.0.0)
-Requires-Dist: eli5 (>=0.13.0,<0.14.0)
+Requires-Dist: dill (>=0.3.7,<0.4.0)
 Requires-Dist: jupyterlab (>=3.5.2,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (==1.23.2)
-Requires-Dist: nvidia-cublas-cu11 (>=11.11.3.6,<12.0.0.0)
-Requires-Dist: nvidia-cuda-cupti-cu11 (>=11.8.87,<12.0.0)
-Requires-Dist: nvidia-cuda-nvrtc-cu11 (>=11.8.89,<12.0.0)
-Requires-Dist: nvidia-cuda-runtime-cu11 (>=11.8.89,<12.0.0)
-Requires-Dist: nvidia-cudnn-cu11 (>=8.9.1.23,<9.0.0.0)
-Requires-Dist: nvidia-cufft-cu11 (>=10.9.0.58,<11.0.0.0)
-Requires-Dist: nvidia-curand-cu11 (>=10.3.0.86,<11.0.0.0)
-Requires-Dist: nvidia-cusolver-cu11 (>=11.4.1.48,<12.0.0.0)
-Requires-Dist: nvidia-cusparse-cu11 (>=11.7.5.86,<12.0.0.0)
-Requires-Dist: nvidia-nccl-cu11 (>=2.16.5,<3.0.0)
-Requires-Dist: nvidia-nvtx-cu11 (>=11.8.86,<12.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: plotly (>=5.15.0,<6.0.0)
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Requires-Dist: scipy (==1.8.0)
 Requires-Dist: spacy (>=3.5.0,<4.0.0)
-Requires-Dist: transformers (>=4.26.1,<5.0.0)
-Requires-Dist: triton (>=2.0.0.post1,<3.0.0)
-Requires-Dist: umap-learn (>=0.5.3,<0.6.0)
 Project-URL: Repository, https://github.com/biaslyze-dev/biaslyze/issues
 Description-Content-Type: text/markdown
 
 
 <div align="center">
-  <img src="resources/biaslyze-logo-no-bg.png" alt="Biaslyze" height="220px">
+  <img src="resources/biaslyze_logo_farbe_rgb.svg" alt="Biaslyze" width="40%">
   <h1>The NLP Bias Identification Toolkit</h1>
 </div>
 
 <div align="center">
     <a href="https://github.com/biaslyze-dev/biaslyze/blob/main/LICENSE">
         <img alt="licence" src="https://img.shields.io/github/license/biaslyze-dev/biaslyze">
     </a>
@@ -98,24 +82,24 @@
     texts=texts,
     predict_func=clf.predict_proba
 )
 
 # see a summary of the detection
 detection_res.report()
 
-# visualize the counterfactual scores
-detection_res.visualize_counterfactual_scores(concept="religion", top_n=10)
+# launch the dashboard visualize the counterfactual scores
+detection_res.dashboard(num_keywords=10)
 ```
 
 You will get results as Boxplots, among others, indicating the impact of keywords and concepts on the prediction of your model.
 Example output:
-![](resources/hatespeech_dl_scores_religion.png)
+![](resources/biaslyze-demo-box-plot.gif)
 
 
-See more detailed examples in the [tutorial](tutorials/tutorial-toxic-comments/).
+See more detailed examples in the [tutorial](https://biaslyze.org/tutorials/tutorial-toxic-comments/).
 
 
 ## Development setup
 
 - First you need to install poetry to manage your python environment: https://python-poetry.org/docs/#installation
 - Run `make install` to install the dependencies and get the spacy basemodels.
 - Now you can use `biaslyze` in your jupyter notebooks.
@@ -139,15 +123,15 @@
 ## Style guide
 
 We are using isort and black: `make style`
 For linting we are running ruff: `make lint`
 
 ## Contributing
 
-Follow the google style guide for python: https://google.github.io/styleguide/pyguide.html
+Follow the Google style guide for Python: https://google.github.io/styleguide/pyguide.html
 
 This project uses black, isort and ruff to enforce style. Apply it by running `make style` and `make lint`.
 
 ## Acknowledgements
 
 * Funded from March 2023 until August 2023 by ![logos of the "Bundesministerium für Bildung und Forschung", Prodotype Fund and OKFN-Deutschland](resources/pf_funding_logos.svg)
```

#### html2text {}

```diff
@@ -1,35 +1,23 @@
-Metadata-Version: 2.1 Name: biaslyze Version: 0.0.7a0 Summary: The NLP Bias
+Metadata-Version: 2.1 Name: biaslyze Version: 0.0.8a0 Summary: The NLP Bias
 Identification Toolkit Home-page: https://biaslyze.org License: BSD-3-Clause
 Keywords: NLP,bias,ethics,fairness Author: Tobias Sterbak & Stina LohmÃ¼ller
 Author-email: hello@biaslyze.org Maintainer: Tobias Sterbak Maintainer-email:
 hello@tobiassterbak.com Requires-Python: >=3.10,<3.11 Classifier: License ::
 OSI Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Dist: bertopic (==0.13.0)
-Requires-Dist: bokeh (>=3.1.0,<4.0.0) Requires-Dist: dash (>=2.11.1,<3.0.0)
-Requires-Dist: eli5 (>=0.13.0,<0.14.0) Requires-Dist: jupyterlab
-(>=3.5.2,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-Dist:
-matplotlib (>=3.7.1,<4.0.0) Requires-Dist: numpy (==1.23.2) Requires-Dist:
-nvidia-cublas-cu11 (>=11.11.3.6,<12.0.0.0) Requires-Dist: nvidia-cuda-cupti-
-cu11 (>=11.8.87,<12.0.0) Requires-Dist: nvidia-cuda-nvrtc-cu11
-(>=11.8.89,<12.0.0) Requires-Dist: nvidia-cuda-runtime-cu11 (>=11.8.89,<12.0.0)
-Requires-Dist: nvidia-cudnn-cu11 (>=8.9.1.23,<9.0.0.0) Requires-Dist: nvidia-
-cufft-cu11 (>=10.9.0.58,<11.0.0.0) Requires-Dist: nvidia-curand-cu11
-(>=10.3.0.86,<11.0.0.0) Requires-Dist: nvidia-cusolver-cu11
-(>=11.4.1.48,<12.0.0.0) Requires-Dist: nvidia-cusparse-cu11
-(>=11.7.5.86,<12.0.0.0) Requires-Dist: nvidia-nccl-cu11 (>=2.16.5,<3.0.0)
-Requires-Dist: nvidia-nvtx-cu11 (>=11.8.86,<12.0.0) Requires-Dist: pandas
-(>=1.5.3,<2.0.0) Requires-Dist: plotly (>=5.15.0,<6.0.0) Requires-Dist: scikit-
-learn (>=1.2.0,<2.0.0) Requires-Dist: scipy (==1.8.0) Requires-Dist: spacy
-(>=3.5.0,<4.0.0) Requires-Dist: transformers (>=4.26.1,<5.0.0) Requires-Dist:
-triton (>=2.0.0.post1,<3.0.0) Requires-Dist: umap-learn (>=0.5.3,<0.6.0)
-Project-URL: Repository, https://github.com/biaslyze-dev/biaslyze/issues
-Description-Content-Type: text/markdown
+Development :: Libraries :: Python Modules Requires-Dist: dash
+(>=2.11.1,<3.0.0) Requires-Dist: dill (>=0.3.7,<0.4.0) Requires-Dist:
+jupyterlab (>=3.5.2,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-
+Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: numpy (==1.23.2) Requires-
+Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: plotly (>=5.15.0,<6.0.0) Requires-
+Dist: scikit-learn (>=1.2.0,<2.0.0) Requires-Dist: scipy (==1.8.0) Requires-
+Dist: spacy (>=3.5.0,<4.0.0) Project-URL: Repository, https://github.com/
+biaslyze-dev/biaslyze/issues Description-Content-Type: text/markdown
                                   [Biaslyze]
                ****** The NLP Bias Identification Toolkit ******
                             [licence] [pypi] [pypi]
 Bias is often subtle and difficult to detect in NLP models, as the protected
 attributes are less obvious and can take many forms in language (e.g. proxies,
 double meanings, ambiguities etc.). Therefore, technical bias testing is a key
 step in avoiding algorithmically mediated discrimination. However, it is
@@ -46,29 +34,29 @@
 download the required spacy models: ```bash python -m spacy download
 en_core_web_sm ``` ## Quickstart ```python from biaslyze.bias_detectors import
 CounterfactualBiasDetector bias_detector = CounterfactualBiasDetector() #
 detect bias in the model based on the given texts # here, clf is a scikit-learn
 text classification pipeline trained for a binary classification task
 detection_res = bias_detector.process( texts=texts,
 predict_func=clf.predict_proba ) # see a summary of the detection
-detection_res.report() # visualize the counterfactual scores
-detection_res.visualize_counterfactual_scores(concept="religion", top_n=10) ```
-You will get results as Boxplots, among others, indicating the impact of
-keywords and concepts on the prediction of your model. Example output: ![]
-(resources/hatespeech_dl_scores_religion.png) See more detailed examples in the
-[tutorial](tutorials/tutorial-toxic-comments/). ## Development setup - First
-you need to install poetry to manage your python environment: https://python-
-poetry.org/docs/#installation - Run `make install` to install the dependencies
-and get the spacy basemodels. - Now you can use `biaslyze` in your jupyter
-notebooks. ### Adding concepts and keywords You can add concepts and new
-keywords for existing concepts by editing [concepts.py](https://github.com/
-biaslyze-dev/biaslyze/blob/main/biaslyze/concepts.py). ## Preview/build the
-documentation with mkdocs To preview the documentation run `make doc-preview`.
-This will launch a preview of the documentation on `http://127.0.0.1:8000/`. To
-build the documentation html run `make doc`. ## Run the automated tests `make
-test` ## Style guide We are using isort and black: `make style` For linting we
-are running ruff: `make lint` ## Contributing Follow the google style guide for
-python: https://google.github.io/styleguide/pyguide.html This project uses
-black, isort and ruff to enforce style. Apply it by running `make style` and
-`make lint`. ## Acknowledgements * Funded from March 2023 until August 2023 by
-![logos of the "Bundesministerium fÃ¼r Bildung und Forschung", Prodotype Fund
-and OKFN-Deutschland](resources/pf_funding_logos.svg)
+detection_res.report() # launch the dashboard visualize the counterfactual
+scores detection_res.dashboard(num_keywords=10) ``` You will get results as
+Boxplots, among others, indicating the impact of keywords and concepts on the
+prediction of your model. Example output: ![](resources/biaslyze-demo-box-
+plot.gif) See more detailed examples in the [tutorial](https://biaslyze.org/
+tutorials/tutorial-toxic-comments/). ## Development setup - First you need to
+install poetry to manage your python environment: https://python-poetry.org/
+docs/#installation - Run `make install` to install the dependencies and get the
+spacy basemodels. - Now you can use `biaslyze` in your jupyter notebooks. ###
+Adding concepts and keywords You can add concepts and new keywords for existing
+concepts by editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/
+blob/main/biaslyze/concepts.py). ## Preview/build the documentation with mkdocs
+To preview the documentation run `make doc-preview`. This will launch a preview
+of the documentation on `http://127.0.0.1:8000/`. To build the documentation
+html run `make doc`. ## Run the automated tests `make test` ## Style guide We
+are using isort and black: `make style` For linting we are running ruff: `make
+lint` ## Contributing Follow the Google style guide for Python: https://
+google.github.io/styleguide/pyguide.html This project uses black, isort and
+ruff to enforce style. Apply it by running `make style` and `make lint`. ##
+Acknowledgements * Funded from March 2023 until August 2023 by ![logos of the
+"Bundesministerium fÃ¼r Bildung und Forschung", Prodotype Fund and OKFN-
+Deutschland](resources/pf_funding_logos.svg)
```

