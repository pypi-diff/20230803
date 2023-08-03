# Comparing `tmp/topic_wizard-0.3.1.tar.gz` & `tmp/topic_wizard-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topic_wizard-0.3.1.tar", max compression
+gzip compressed data, was "topic_wizard-0.4.0.tar", max compression
```

## Comparing `topic_wizard-0.3.1.tar` & `topic_wizard-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.3.1/LICENSE
--rw-r--r--   0        0        0     4534 2023-07-06 08:38:13.531980 topic_wizard-0.3.1/README.md
--rw-r--r--   0        0        0      640 2023-07-06 08:26:14.602969 topic_wizard-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      404 2023-06-30 14:25:27.164990 topic_wizard-0.3.1/topicwizard/__init__.py
--rw-r--r--   0        0        0     9512 2023-07-06 08:25:44.631006 topic_wizard-0.3.1/topicwizard/app.py
--rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.3.1/topicwizard/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.1/topicwizard/blueprints/__init__.py
--rw-r--r--   0        0        0     7443 2023-07-06 08:25:44.631006 topic_wizard-0.3.1/topicwizard/blueprints/app.py
--rw-r--r--   0        0        0     4322 2023-05-17 11:05:13.211055 topic_wizard-0.3.1/topicwizard/blueprints/documents.py
--rw-r--r--   0        0        0     2490 2023-07-06 08:25:44.631006 topic_wizard-0.3.1/topicwizard/blueprints/groups.py
--rw-r--r--   0        0        0     2516 2023-07-06 08:25:44.631006 topic_wizard-0.3.1/topicwizard/blueprints/template.py
--rw-r--r--   0        0        0     4979 2023-06-30 14:12:57.739575 topic_wizard-0.3.1/topicwizard/blueprints/topics.py
--rw-r--r--   0        0        0     3015 2023-05-17 11:05:57.615132 topic_wizard-0.3.1/topicwizard/blueprints/words.py
--rw-r--r--   0        0        0     3937 2023-07-05 08:00:17.664404 topic_wizard-0.3.1/topicwizard/compatibility/bertopic.py
--rw-r--r--   0        0        0     6425 2023-05-17 11:33:07.273886 topic_wizard-0.3.1/topicwizard/compatibility/gensim.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.1/topicwizard/components/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.3.1/topicwizard/components/documents/__init__.py
--rw-r--r--   0        0        0     1993 2023-04-24 14:00:03.181792 topic_wizard-0.3.1/topicwizard/components/documents/document_map.py
--rw-r--r--   0        0        0     1399 2023-04-24 14:04:24.294134 topic_wizard-0.3.1/topicwizard/components/documents/document_pie.py
--rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.3.1/topicwizard/components/documents/document_selector.py
--rw-r--r--   0        0        0     1708 2023-07-05 07:54:27.399506 topic_wizard-0.3.1/topicwizard/components/documents/document_timeline.py
--rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/documents/document_wordcloud.py
--rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/documents/window_slider.py
--rw-r--r--   0        0        0      938 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/components/groups/group_barplot.py
--rw-r--r--   0        0        0     2087 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/components/groups/group_map.py
--rw-r--r--   0        0        0      848 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/components/groups/group_wordcloud.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/__init__.py
--rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/intertopic_map.py
--rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/relevance_slider.py
--rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/topic_barplot.py
--rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/topic_namer.py
--rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/topic_switcher.py
--rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/topics/wordcloud.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/words/__init__.py
--rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.3.1/topicwizard/components/words/association_slider.py
--rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.3.1/topicwizard/components/words/word_barplot.py
--rw-r--r--   0        0        0     2514 2023-04-24 14:33:48.501717 topic_wizard-0.3.1/topicwizard/components/words/word_map.py
--rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.3.1/topicwizard/components/words/word_selector.py
--rw-r--r--   0        0        0      675 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/figures/__init__.py
--rw-r--r--   0        0        0     7715 2023-07-05 07:49:54.902696 topic_wizard-0.3.1/topicwizard/figures/documents.py
--rw-r--r--   0        0        0    10961 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/figures/groups.py
--rw-r--r--   0        0        0     9502 2023-07-05 11:21:34.951475 topic_wizard-0.3.1/topicwizard/figures/topics.py
--rw-r--r--   0        0        0     6392 2023-06-30 15:39:09.394441 topic_wizard-0.3.1/topicwizard/figures/words.py
--rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.3.1/topicwizard/plots/__init__.py
--rw-r--r--   0        0        0     5183 2023-05-17 10:58:27.942406 topic_wizard-0.3.1/topicwizard/plots/documents.py
--rw-r--r--   0        0        0     4228 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/plots/groups.py
--rw-r--r--   0        0        0     4244 2023-06-26 12:14:28.818856 topic_wizard-0.3.1/topicwizard/plots/topics.py
--rw-r--r--   0        0        0      274 2023-07-05 07:56:39.267858 topic_wizard-0.3.1/topicwizard/plots/utils.py
--rw-r--r--   0        0        0     3503 2023-04-24 14:33:17.069633 topic_wizard-0.3.1/topicwizard/plots/words.py
--rw-r--r--   0        0        0        0 2023-06-26 12:10:25.930511 topic_wizard-0.3.1/topicwizard/prepare/__init__.py
--rw-r--r--   0        0        0     2820 2023-07-05 07:49:23.926595 topic_wizard-0.3.1/topicwizard/prepare/documents.py
--rw-r--r--   0        0        0     4837 2023-07-06 08:25:44.635006 topic_wizard-0.3.1/topicwizard/prepare/groups.py
--rw-r--r--   0        0        0     4949 2023-07-05 11:16:13.759839 topic_wizard-0.3.1/topicwizard/prepare/topics.py
--rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.3.1/topicwizard/prepare/utils.py
--rw-r--r--   0        0        0     4923 2023-04-24 14:35:51.642035 topic_wizard-0.3.1/topicwizard/prepare/words.py
--rw-r--r--   0        0        0     5946 1970-01-01 00:00:00.000000 topic_wizard-0.3.1/setup.py
--rw-r--r--   0        0        0     5557 1970-01-01 00:00:00.000000 topic_wizard-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5024 2023-08-02 14:08:58.473602 topic_wizard-0.4.0/README.md
+-rw-r--r--   0        0        0      640 2023-08-02 14:01:28.476432 topic_wizard-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-06-30 14:25:27.164990 topic_wizard-0.4.0/topicwizard/__init__.py
+-rw-r--r--   0        0        0     9636 2023-08-02 13:59:38.376106 topic_wizard-0.4.0/topicwizard/app.py
+-rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.4.0/topicwizard/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.4.0/topicwizard/blueprints/__init__.py
+-rw-r--r--   0        0        0     7443 2023-07-06 08:25:44.631006 topic_wizard-0.4.0/topicwizard/blueprints/app.py
+-rw-r--r--   0        0        0     4322 2023-05-17 11:05:13.211055 topic_wizard-0.4.0/topicwizard/blueprints/documents.py
+-rw-r--r--   0        0        0     2490 2023-07-06 08:25:44.631006 topic_wizard-0.4.0/topicwizard/blueprints/groups.py
+-rw-r--r--   0        0        0     2516 2023-07-06 08:25:44.631006 topic_wizard-0.4.0/topicwizard/blueprints/template.py
+-rw-r--r--   0        0        0     4979 2023-06-30 14:12:57.739575 topic_wizard-0.4.0/topicwizard/blueprints/topics.py
+-rw-r--r--   0        0        0     3015 2023-05-17 11:05:57.615132 topic_wizard-0.4.0/topicwizard/blueprints/words.py
+-rw-r--r--   0        0        0     3933 2023-08-02 11:28:27.742582 topic_wizard-0.4.0/topicwizard/compatibility/bertopic.py
+-rw-r--r--   0        0        0     6474 2023-08-02 11:29:54.314757 topic_wizard-0.4.0/topicwizard/compatibility/gensim.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.4.0/topicwizard/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.4.0/topicwizard/components/documents/__init__.py
+-rw-r--r--   0        0        0     1993 2023-04-24 14:00:03.181792 topic_wizard-0.4.0/topicwizard/components/documents/document_map.py
+-rw-r--r--   0        0        0     1399 2023-04-24 14:04:24.294134 topic_wizard-0.4.0/topicwizard/components/documents/document_pie.py
+-rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.4.0/topicwizard/components/documents/document_selector.py
+-rw-r--r--   0        0        0     1708 2023-07-05 07:54:27.399506 topic_wizard-0.4.0/topicwizard/components/documents/document_timeline.py
+-rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.4.0/topicwizard/components/documents/document_wordcloud.py
+-rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.4.0/topicwizard/components/documents/window_slider.py
+-rw-r--r--   0        0        0      938 2023-07-06 08:25:44.635006 topic_wizard-0.4.0/topicwizard/components/groups/group_barplot.py
+-rw-r--r--   0        0        0     2087 2023-07-06 08:25:44.635006 topic_wizard-0.4.0/topicwizard/components/groups/group_map.py
+-rw-r--r--   0        0        0      848 2023-07-06 08:25:44.635006 topic_wizard-0.4.0/topicwizard/components/groups/group_wordcloud.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.4.0/topicwizard/components/topics/__init__.py
+-rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.4.0/topicwizard/components/topics/intertopic_map.py
+-rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.4.0/topicwizard/components/topics/relevance_slider.py
+-rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.4.0/topicwizard/components/topics/topic_barplot.py
+-rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.4.0/topicwizard/components/topics/topic_namer.py
+-rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.4.0/topicwizard/components/topics/topic_switcher.py
+-rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.4.0/topicwizard/components/topics/wordcloud.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.4.0/topicwizard/components/words/__init__.py
+-rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.4.0/topicwizard/components/words/association_slider.py
+-rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.4.0/topicwizard/components/words/word_barplot.py
+-rw-r--r--   0        0        0     2514 2023-04-24 14:33:48.501717 topic_wizard-0.4.0/topicwizard/components/words/word_map.py
+-rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.4.0/topicwizard/components/words/word_selector.py
+-rw-r--r--   0        0        0      675 2023-07-06 08:25:44.635006 topic_wizard-0.4.0/topicwizard/figures/__init__.py
+-rw-r--r--   0        0        0     7715 2023-07-05 07:49:54.902696 topic_wizard-0.4.0/topicwizard/figures/documents.py
+-rw-r--r--   0        0        0    10961 2023-07-06 08:25:44.635006 topic_wizard-0.4.0/topicwizard/figures/groups.py
+-rw-r--r--   0        0        0     9502 2023-07-05 11:21:34.951475 topic_wizard-0.4.0/topicwizard/figures/topics.py
+-rw-r--r--   0        0        0     6392 2023-06-30 15:39:09.394441 topic_wizard-0.4.0/topicwizard/figures/words.py
+-rw-r--r--   0        0        0     8937 2023-08-02 12:45:00.841811 topic_wizard-0.4.0/topicwizard/pipeline.py
+-rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.4.0/topicwizard/plots/__init__.py
+-rw-r--r--   0        0        0     5183 2023-05-17 10:58:27.942406 topic_wizard-0.4.0/topicwizard/plots/documents.py
+-rw-r--r--   0        0        0     4228 2023-07-06 08:25:44.635006 topic_wizard-0.4.0/topicwizard/plots/groups.py
+-rw-r--r--   0        0        0     4244 2023-06-26 12:14:28.818856 topic_wizard-0.4.0/topicwizard/plots/topics.py
+-rw-r--r--   0        0        0      274 2023-07-05 07:56:39.267858 topic_wizard-0.4.0/topicwizard/plots/utils.py
+-rw-r--r--   0        0        0     3503 2023-04-24 14:33:17.069633 topic_wizard-0.4.0/topicwizard/plots/words.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:10:25.930511 topic_wizard-0.4.0/topicwizard/prepare/__init__.py
+-rw-r--r--   0        0        0     2820 2023-07-05 07:49:23.926595 topic_wizard-0.4.0/topicwizard/prepare/documents.py
+-rw-r--r--   0        0        0     4837 2023-07-06 08:25:44.635006 topic_wizard-0.4.0/topicwizard/prepare/groups.py
+-rw-r--r--   0        0        0     4949 2023-07-05 11:16:13.759839 topic_wizard-0.4.0/topicwizard/prepare/topics.py
+-rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.4.0/topicwizard/prepare/utils.py
+-rw-r--r--   0        0        0     4923 2023-04-24 14:35:51.642035 topic_wizard-0.4.0/topicwizard/prepare/words.py
+-rw-r--r--   0        0        0     6452 1970-01-01 00:00:00.000000 topic_wizard-0.4.0/setup.py
+-rw-r--r--   0        0        0     6047 1970-01-01 00:00:00.000000 topic_wizard-0.4.0/PKG-INFO
```

### Comparing `topic_wizard-0.3.1/LICENSE` & `topic_wizard-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/README.md` & `topic_wizard-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 <br>
 
 
 
 https://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4
 
+## New in version 0.4.0 🌟 🌟
+
+- Introduced topic pipelines that make it easier and safer to use topic models in downstream tasks and interpretation.
+
 ## New in version 0.3.1 🌟 🌟
 
 - You can now investigate relations of pre-existing labels to your topics and words :mag:
 
 ## New in version 0.3.0 🌟 
 
  - Exclude pages, that are not needed :bird:
@@ -79,14 +83,26 @@
     NMF(n_components=30),
 )
 
 # Then fit it on the given texts
 pipeline.fit(corpus)
 ```
 
+From version 0.4.0 you can also use TopicPipelines, which are almost functionally identical but come with a set of built-in conveniences and
+safeties.
+
+```python
+from topicwizard.pipeline import make_topic_pipeline
+
+pipeline = make_topic_pipeline(
+    CountVectorizer(stop_words="english", min_df=10),
+    NMF(n_components=30),
+)
+```
+
 ### Step 2a:
 
 Visualize with the topicwizard webapp :bulb:
 
 ```python
 import topicwizard
```

### Comparing `topic_wizard-0.3.1/pyproject.toml` & `topic_wizard-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "topic-wizard"
-version = "0.3.1"
+version = "0.4.0"
 description = "Pretty and opinionated topic model visualization in Python."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "topicwizard"}]
 
 [tool.poetry.dependencies]
```

### Comparing `topic_wizard-0.3.1/topicwizard/app.py` & `topic_wizard-0.4.0/topicwizard/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,16 @@
     Thread or None
         Returns a Thread if running in a Jupyter notebook (so you can close the server)
         returns None otherwise.
     """
     vectorizer, topic_model = split_pipeline(vectorizer, topic_model, pipeline)
     exclude_pages = set() if exclude_pages is None else set(exclude_pages)
     print("Preprocessing")
+    if topic_names is None and hasattr(pipeline, "topic_names"):
+        topic_names = pipeline.topic_names  # type: ignore
     app = get_dash_app(
         vectorizer=vectorizer,
         topic_model=topic_model,
         corpus=corpus,
         document_names=document_names,
         topic_names=topic_names,
         exclude_pages=exclude_pages,
```

### Comparing `topic_wizard-0.3.1/topicwizard/assets/favicon.ico` & `topic_wizard-0.4.0/topicwizard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/blueprints/app.py` & `topic_wizard-0.4.0/topicwizard/blueprints/app.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/blueprints/documents.py` & `topic_wizard-0.4.0/topicwizard/blueprints/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/blueprints/groups.py` & `topic_wizard-0.4.0/topicwizard/blueprints/groups.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/blueprints/template.py` & `topic_wizard-0.4.0/topicwizard/blueprints/template.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/blueprints/topics.py` & `topic_wizard-0.4.0/topicwizard/blueprints/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/blueprints/words.py` & `topic_wizard-0.4.0/topicwizard/blueprints/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/compatibility/bertopic.py` & `topic_wizard-0.4.0/topicwizard/compatibility/bertopic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Iterable, List, Optional, Tuple
 
 import numpy as np
 import scipy.sparse as spr
 from sklearn.base import BaseEstimator
 from sklearn.feature_extraction.text import CountVectorizer
-from sklearn.pipeline import Pipeline, make_pipeline
+
+from topicwizard.pipeline import TopicPipeline, make_topic_pipeline
 
 
 class SparseWithText(spr.csr_array):
     """Compressed Sparse Row sparse array with a text attribute,
     this way the textual content of the sparse array can be
     passed down in a pipeline."""
 
@@ -88,33 +89,33 @@
         return np.array(dist)
 
     def fit_transform(self, X, y=None):
         self.fit(X)
         return self.transform(X)
 
 
-def bertopic_pipeline(model) -> Tuple[Pipeline, List[str]]:
+def bertopic_pipeline(model) -> TopicPipeline:
     """Creates sklearn compatible wrapper for a BERTopic topic pipeline.
 
     Parameters
     ----------
     model: BERTopic
         Any BERTopic model.
 
     Returns
     -------
-    pipeline: Pipeline
-        Sklearn pipeline wrapping the BERTopic topic model.
-    topic_names: list of str
-        Names of topics assigned in the BERTopic model.
+    pipeline: TopicPipeline
+        Sklearn compatible topic pipeline wrapping the BERTopic topic model.
     """
     vectorizer = _BERTopicVectorizer(topic_model=model)
     topic_model = _BERTopicModel(topic_model=model)
     n_components, _ = topic_model.components_.shape
     topic_names = []
     if model.custom_labels_ is not None:
         topic_labels = model.custom_labels_
     else:
         topic_labels = model.topic_labels_
     for i_topic in range(n_components):
         topic_names.append(topic_labels[i_topic])
-    return make_pipeline(vectorizer, topic_model), topic_names
+    pipeline = make_topic_pipeline(vectorizer, topic_model)
+    pipeline.topic_names = topic_names
+    return pipeline
```

### Comparing `topic_wizard-0.3.1/topicwizard/compatibility/gensim.py` & `topic_wizard-0.4.0/topicwizard/compatibility/gensim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import warnings
 from typing import Iterable
 
 import numpy as np
 import scipy.sparse as spr
 from sklearn.base import BaseEstimator
-from sklearn.pipeline import Pipeline, make_pipeline
 from tqdm import tqdm
 
+from topicwizard.pipeline import TopicPipeline, make_topic_pipeline
+
 
 class DictionaryVectorizer(BaseEstimator):
     """Wrapper for Gensim's dictionary object as an sklearn compatible vectorizer object.
 
     Parameters
     ----------
     dictionary: gensim.corpora.dictionary.Dictionary
@@ -165,26 +166,26 @@
 
     def fit_transform(self, X, y=None):
         """Does the same as transform(), kept for compatiblity reasons."""
         self.fit(X)
         return self.transform(X)
 
 
-def gensim_pipeline(dictionary, model) -> Pipeline:
+def gensim_pipeline(dictionary, model) -> TopicPipeline:
     """Creates sklearn compatible wrapper for a Gensim topic pipeline.
 
     Parameters
     ----------
     dictionary: gensim.corpora.dictionary.Dictionary
         Gensim's dictionary object. Please only pass already fitted
         dictionary objects.
     model: LdaModel | LdaMulticore | Nmf | LsiModel
         Gensim topic model. The model should already be fitted.
 
     Returns
     -------
-    Pipeline
-        Sklearn pipeline wrapping the Gensim topic model.
+    TopicPipeline
+        Sklearn compatible topic pipeline wrapping the Gensim topic model.
     """
     vectorizer = DictionaryVectorizer(dictionary)
     topic_model = TopicModelWrapper(model=model, index_to_key=vectorizer.index_to_key)
-    return make_pipeline(vectorizer, topic_model)
+    return make_topic_pipeline(vectorizer, topic_model)
```

### Comparing `topic_wizard-0.3.1/topicwizard/components/documents/document_map.py` & `topic_wizard-0.4.0/topicwizard/components/documents/document_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/documents/document_pie.py` & `topic_wizard-0.4.0/topicwizard/components/documents/document_pie.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/documents/document_selector.py` & `topic_wizard-0.4.0/topicwizard/components/documents/document_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/documents/document_timeline.py` & `topic_wizard-0.4.0/topicwizard/components/documents/document_timeline.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/documents/document_wordcloud.py` & `topic_wizard-0.4.0/topicwizard/components/documents/document_wordcloud.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/documents/window_slider.py` & `topic_wizard-0.4.0/topicwizard/components/documents/window_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/groups/group_barplot.py` & `topic_wizard-0.4.0/topicwizard/components/groups/group_barplot.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/groups/group_map.py` & `topic_wizard-0.4.0/topicwizard/components/groups/group_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/groups/group_wordcloud.py` & `topic_wizard-0.4.0/topicwizard/components/groups/group_wordcloud.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/topics/intertopic_map.py` & `topic_wizard-0.4.0/topicwizard/components/topics/intertopic_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/topics/relevance_slider.py` & `topic_wizard-0.4.0/topicwizard/components/topics/relevance_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/topics/topic_namer.py` & `topic_wizard-0.4.0/topicwizard/components/topics/topic_namer.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/topics/topic_switcher.py` & `topic_wizard-0.4.0/topicwizard/components/topics/topic_switcher.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/words/association_slider.py` & `topic_wizard-0.4.0/topicwizard/components/words/association_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/words/word_barplot.py` & `topic_wizard-0.4.0/topicwizard/components/words/word_barplot.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/words/word_map.py` & `topic_wizard-0.4.0/topicwizard/components/words/word_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/components/words/word_selector.py` & `topic_wizard-0.4.0/topicwizard/components/words/word_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/figures/__init__.py` & `topic_wizard-0.4.0/topicwizard/figures/__init__.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/figures/documents.py` & `topic_wizard-0.4.0/topicwizard/figures/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/figures/groups.py` & `topic_wizard-0.4.0/topicwizard/figures/groups.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/figures/topics.py` & `topic_wizard-0.4.0/topicwizard/figures/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/figures/words.py` & `topic_wizard-0.4.0/topicwizard/figures/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/plots/documents.py` & `topic_wizard-0.4.0/topicwizard/plots/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/plots/groups.py` & `topic_wizard-0.4.0/topicwizard/plots/groups.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/plots/topics.py` & `topic_wizard-0.4.0/topicwizard/plots/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/plots/words.py` & `topic_wizard-0.4.0/topicwizard/plots/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/prepare/documents.py` & `topic_wizard-0.4.0/topicwizard/prepare/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/prepare/groups.py` & `topic_wizard-0.4.0/topicwizard/prepare/groups.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/prepare/topics.py` & `topic_wizard-0.4.0/topicwizard/prepare/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/prepare/utils.py` & `topic_wizard-0.4.0/topicwizard/prepare/utils.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/topicwizard/prepare/words.py` & `topic_wizard-0.4.0/topicwizard/prepare/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.3.1/setup.py` & `topic_wizard-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,17 +28,17 @@
  'scikit-learn>=1.2.0,<1.3.0',
  'scipy>=1.8.0',
  'umap-learn>=0.5.3',
  'wordcloud>=1.8.2.2,<1.9.0.0']
 
 setup_kwargs = {
     'name': 'topic-wizard',
-    'version': '0.3.1',
+    'version': '0.4.0',
     'description': 'Pretty and opinionated topic model visualization in Python.',
-    'long_description': '<img align="left" width="82" height="82" src="assets/logo.svg">\n\n# topicwizard\n\n<br>\n\nPretty and opinionated topic model visualization in Python.\n\n[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/x-tabdeveloping/topic-wizard/blob/main/examples/basic_usage.ipynb)\n[![PyPI version](https://badge.fury.io/py/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![pip downloads](https://img.shields.io/pypi/dm/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![python version](https://img.shields.io/badge/Python-%3E=3.8-blue)](https://github.com/centre-for-humanities-computing/tweetopic)\n[![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)\n<br>\n\n\n\nhttps://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4\n\n## New in version 0.3.1 🌟 🌟\n\n- You can now investigate relations of pre-existing labels to your topics and words :mag:\n\n## New in version 0.3.0 🌟 \n\n - Exclude pages, that are not needed :bird:\n - Self-contained interactive figures :gift:\n - Topic name inference is now default behavior and is done implicitly.\n\n\n## Features\n\n-   Investigate complex relations between topics, words, documents and groups/genres/labels\n-   Sklearn, Gensim and BERTopic compatible :nut_and_bolt:\n-   Highly interactive web app\n-   Interactive and composable Plotly figures\n-   Automatically infer topic names, oooor...\n-   Name topics manually\n-   Easy deployment :earth_africa:\n\n## Installation\n\nInstall from PyPI:\n\n```bash\npip install topic-wizard\n```\n\n## Usage ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))\n\n### Step 0:\n\nHave a corpus ready for analysis, in this example I am going to use 20 newgroups from scikit-learn.\n\n```python\nfrom sklearn.datasets import fetch_20newsgroups\n\nnewsgroups = fetch_20newsgroups(subset="all")\ncorpus = newsgroups.data\n\n# Sklearn gives the labels back as integers, we have to map them back to\n# the actual textual label.\ngroup_labels = [newsgroups.target_names[label] for label in newsgroups.target]\n```\n\n### Step 1:\n\nTrain a scikit-learn compatible topic model.\n(If you want to use non-scikit-learn topic models, check [compatibility](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html))\n\n```python\nfrom sklearn.decomposition import NMF\nfrom sklearn.feature_extraction.text import CountVectorizer\nfrom sklearn.pipeline import make_pipeline\n\n# Create topic pipeline\npipeline = make_pipeline(\n    CountVectorizer(stop_words="english", min_df=10),\n    NMF(n_components=30),\n)\n\n# Then fit it on the given texts\npipeline.fit(corpus)\n```\n\n### Step 2a:\n\nVisualize with the topicwizard webapp :bulb:\n\n```python\nimport topicwizard\n\ntopicwizard.visualize(corpus, pipeline=pipeline)\n```\n\nFrom version 0.3.0 you can also disable pages you do not wish to display thereby sparing a lot of time for yourself:\n\n```python\n# A large corpus takes a looong time to compute 2D projections for so\n# so you can speed up preprocessing by disabling it alltogether.\ntopicwizard.visualize(corpus, pipeline=pipeline, exclude_pages=["documents"])\n```\n\n\n![topics screenshot](assets/screenshot_topics.png)\n![words screenshot](assets/screenshot_words.png)\n![words screenshot](assets/screenshot_words_zoomed.png)\n![documents screenshot](assets/screenshot_documents.png)\n\nFrom version 0.3.1 you can investigate groups/labels by passing them along to the webapp.\n\n```python\ntopicwizard.visualize(corpus, pipeline=pipeline, group_labels=group_labels)\n```\n\n![groups screenshot](docs/_static/screenshot_groups.png)\n\nOoooor...\n\n### Step 2b:\n\nProduce high quality self-contained HTML plots and create your own dashboards/reports :strawberry:\n\n### Map of words\n\n```python\nfrom topicwizard.figures import word_map\n\nword_map(corpus, pipeline=pipeline)\n```\n\n![word map screenshot](assets/word_map.png)\n\n### Timelines of topic distributions\n\n```python\nfrom topicwizard.figures import document_topic_timeline\n\ndocument_topic_timeline(\n    "Joe Biden takes over presidential office from Donald Trump.",\n    pipeline=pipeline,\n)\n```\n![document timeline](assets/document_topic_timeline.png)\n\n### Wordclouds of your topics :cloud:\n\n```python\nfrom topicwizard.figures import topic_wordclouds\n\ntopic_wordclouds(corpus, pipeline=pipeline)\n```\n\n![wordclouds](assets/topic_wordclouds.png)\n\n#### And much more... ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))\n',
+    'long_description': '<img align="left" width="82" height="82" src="assets/logo.svg">\n\n# topicwizard\n\n<br>\n\nPretty and opinionated topic model visualization in Python.\n\n[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/x-tabdeveloping/topic-wizard/blob/main/examples/basic_usage.ipynb)\n[![PyPI version](https://badge.fury.io/py/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![pip downloads](https://img.shields.io/pypi/dm/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![python version](https://img.shields.io/badge/Python-%3E=3.8-blue)](https://github.com/centre-for-humanities-computing/tweetopic)\n[![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)\n<br>\n\n\n\nhttps://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4\n\n## New in version 0.4.0 🌟 🌟\n\n- Introduced topic pipelines that make it easier and safer to use topic models in downstream tasks and interpretation.\n\n## New in version 0.3.1 🌟 🌟\n\n- You can now investigate relations of pre-existing labels to your topics and words :mag:\n\n## New in version 0.3.0 🌟 \n\n - Exclude pages, that are not needed :bird:\n - Self-contained interactive figures :gift:\n - Topic name inference is now default behavior and is done implicitly.\n\n\n## Features\n\n-   Investigate complex relations between topics, words, documents and groups/genres/labels\n-   Sklearn, Gensim and BERTopic compatible :nut_and_bolt:\n-   Highly interactive web app\n-   Interactive and composable Plotly figures\n-   Automatically infer topic names, oooor...\n-   Name topics manually\n-   Easy deployment :earth_africa:\n\n## Installation\n\nInstall from PyPI:\n\n```bash\npip install topic-wizard\n```\n\n## Usage ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))\n\n### Step 0:\n\nHave a corpus ready for analysis, in this example I am going to use 20 newgroups from scikit-learn.\n\n```python\nfrom sklearn.datasets import fetch_20newsgroups\n\nnewsgroups = fetch_20newsgroups(subset="all")\ncorpus = newsgroups.data\n\n# Sklearn gives the labels back as integers, we have to map them back to\n# the actual textual label.\ngroup_labels = [newsgroups.target_names[label] for label in newsgroups.target]\n```\n\n### Step 1:\n\nTrain a scikit-learn compatible topic model.\n(If you want to use non-scikit-learn topic models, check [compatibility](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html))\n\n```python\nfrom sklearn.decomposition import NMF\nfrom sklearn.feature_extraction.text import CountVectorizer\nfrom sklearn.pipeline import make_pipeline\n\n# Create topic pipeline\npipeline = make_pipeline(\n    CountVectorizer(stop_words="english", min_df=10),\n    NMF(n_components=30),\n)\n\n# Then fit it on the given texts\npipeline.fit(corpus)\n```\n\nFrom version 0.4.0 you can also use TopicPipelines, which are almost functionally identical but come with a set of built-in conveniences and\nsafeties.\n\n```python\nfrom topicwizard.pipeline import make_topic_pipeline\n\npipeline = make_topic_pipeline(\n    CountVectorizer(stop_words="english", min_df=10),\n    NMF(n_components=30),\n)\n```\n\n### Step 2a:\n\nVisualize with the topicwizard webapp :bulb:\n\n```python\nimport topicwizard\n\ntopicwizard.visualize(corpus, pipeline=pipeline)\n```\n\nFrom version 0.3.0 you can also disable pages you do not wish to display thereby sparing a lot of time for yourself:\n\n```python\n# A large corpus takes a looong time to compute 2D projections for so\n# so you can speed up preprocessing by disabling it alltogether.\ntopicwizard.visualize(corpus, pipeline=pipeline, exclude_pages=["documents"])\n```\n\n\n![topics screenshot](assets/screenshot_topics.png)\n![words screenshot](assets/screenshot_words.png)\n![words screenshot](assets/screenshot_words_zoomed.png)\n![documents screenshot](assets/screenshot_documents.png)\n\nFrom version 0.3.1 you can investigate groups/labels by passing them along to the webapp.\n\n```python\ntopicwizard.visualize(corpus, pipeline=pipeline, group_labels=group_labels)\n```\n\n![groups screenshot](docs/_static/screenshot_groups.png)\n\nOoooor...\n\n### Step 2b:\n\nProduce high quality self-contained HTML plots and create your own dashboards/reports :strawberry:\n\n### Map of words\n\n```python\nfrom topicwizard.figures import word_map\n\nword_map(corpus, pipeline=pipeline)\n```\n\n![word map screenshot](assets/word_map.png)\n\n### Timelines of topic distributions\n\n```python\nfrom topicwizard.figures import document_topic_timeline\n\ndocument_topic_timeline(\n    "Joe Biden takes over presidential office from Donald Trump.",\n    pipeline=pipeline,\n)\n```\n![document timeline](assets/document_topic_timeline.png)\n\n### Wordclouds of your topics :cloud:\n\n```python\nfrom topicwizard.figures import topic_wordclouds\n\ntopic_wordclouds(corpus, pipeline=pipeline)\n```\n\n![wordclouds](assets/topic_wordclouds.png)\n\n#### And much more... ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))\n',
     'author': 'Márton Kardos',
     'author_email': 'power.up1163@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `topic_wizard-0.3.1/PKG-INFO` & `topic_wizard-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topic-wizard
-Version: 0.3.1
+Version: 0.4.0
 Summary: Pretty and opinionated topic model visualization in Python.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,14 +40,18 @@
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 <br>
 
 
 
 https://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4
 
+## New in version 0.4.0 🌟 🌟
+
+- Introduced topic pipelines that make it easier and safer to use topic models in downstream tasks and interpretation.
+
 ## New in version 0.3.1 🌟 🌟
 
 - You can now investigate relations of pre-existing labels to your topics and words :mag:
 
 ## New in version 0.3.0 🌟 
 
  - Exclude pages, that are not needed :bird:
@@ -106,14 +110,26 @@
     NMF(n_components=30),
 )
 
 # Then fit it on the given texts
 pipeline.fit(corpus)
 ```
 
+From version 0.4.0 you can also use TopicPipelines, which are almost functionally identical but come with a set of built-in conveniences and
+safeties.
+
+```python
+from topicwizard.pipeline import make_topic_pipeline
+
+pipeline = make_topic_pipeline(
+    CountVectorizer(stop_words="english", min_df=10),
+    NMF(n_components=30),
+)
+```
+
 ### Step 2a:
 
 Visualize with the topicwizard webapp :bulb:
 
 ```python
 import topicwizard
```

