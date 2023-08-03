# Comparing `tmp/codedog-0.5.3.tar.gz` & `tmp/codedog-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedog-0.5.3.tar", max compression
+gzip compressed data, was "codedog-0.5.4.tar", max compression
```

## Comparing `codedog-0.5.3.tar` & `codedog-0.5.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      328 2023-07-30 08:13:27.833259 codedog-0.5.3/codedog/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:13:27.834259 codedog-0.5.3/codedog/actors/__init__.py
--rw-r--r--   0        0        0       22 2023-07-30 08:13:27.834259 codedog-0.5.3/codedog/actors/base.py
--rw-r--r--   0        0        0        0 2023-07-30 08:13:27.834259 codedog-0.5.3/codedog/actors/reporters/__init__.py
--rw-r--r--   0        0        0      198 2023-07-30 08:13:27.834259 codedog-0.5.3/codedog/actors/reporters/base.py
--rw-r--r--   0        0        0     1078 2023-07-30 08:13:27.835260 codedog-0.5.3/codedog/actors/reporters/code_review.py
--rw-r--r--   0        0        0     2842 2023-08-02 14:31:22.564488 codedog-0.5.3/codedog/actors/reporters/pr_summary.py
--rw-r--r--   0        0        0     2207 2023-07-30 08:13:27.835260 codedog-0.5.3/codedog/actors/reporters/pull_request.py
--rw-r--r--   0        0        0      167 2023-07-30 08:13:27.835260 codedog-0.5.3/codedog/chains/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:13:27.854264 codedog-0.5.3/codedog/chains/code_review/__init__.py
--rw-r--r--   0        0        0     4143 2023-08-02 14:30:41.484288 codedog-0.5.3/codedog/chains/code_review/base.py
--rw-r--r--   0        0        0      231 2023-07-30 08:13:27.854264 codedog-0.5.3/codedog/chains/code_review/prompts.py
--rw-r--r--   0        0        0        0 2023-07-25 13:00:53.472920 codedog-0.5.3/codedog/chains/pr_summary/__init__.py
--rw-r--r--   0        0        0     6358 2023-08-02 14:30:41.484288 codedog-0.5.3/codedog/chains/pr_summary/base.py
--rw-r--r--   0        0        0      579 2023-07-25 13:00:53.474921 codedog-0.5.3/codedog/chains/pr_summary/prompts.py
--rw-r--r--   0        0        0      714 2023-07-30 08:13:27.979292 codedog-0.5.3/codedog/localization.py
--rw-r--r--   0        0        0      738 2023-07-30 08:13:28.073313 codedog-0.5.3/codedog/models/__init__.py
--rw-r--r--   0        0        0      408 2023-07-25 13:00:53.493925 codedog-0.5.3/codedog/models/blob.py
--rw-r--r--   0        0        0     2018 2023-07-30 08:13:28.073313 codedog-0.5.3/codedog/models/change_file.py
--rw-r--r--   0        0        0      192 2023-07-25 13:00:53.493925 codedog-0.5.3/codedog/models/change_summary.py
--rw-r--r--   0        0        0      150 2023-07-30 08:13:28.106320 codedog-0.5.3/codedog/models/code_review.py
--rw-r--r--   0        0        0      800 2023-07-25 13:00:53.494925 codedog-0.5.3/codedog/models/commit.py
--rw-r--r--   0        0        0     1148 2023-07-25 13:00:53.494925 codedog-0.5.3/codedog/models/diff.py
--rw-r--r--   0        0        0      824 2023-07-25 13:00:53.494925 codedog-0.5.3/codedog/models/issue.py
--rw-r--r--   0        0        0      692 2023-07-30 08:13:28.106320 codedog-0.5.3/codedog/models/pr_summary.py
--rw-r--r--   0        0        0     1703 2023-07-30 08:13:28.107321 codedog-0.5.3/codedog/models/pull_request.py
--rw-r--r--   0        0        0      998 2023-07-25 13:00:53.495925 codedog-0.5.3/codedog/models/repository.py
--rw-r--r--   0        0        0      111 2023-07-30 08:13:28.123920 codedog-0.5.3/codedog/processors/__init__.py
--rw-r--r--   0        0        0     3835 2023-07-30 08:13:28.123920 codedog-0.5.3/codedog/processors/pull_request_processor.py
--rw-r--r--   0        0        0      178 2023-07-25 13:00:53.496925 codedog-0.5.3/codedog/retrievers/__init__.py
--rw-r--r--   0        0        0     1375 2023-07-25 13:00:53.496925 codedog-0.5.3/codedog/retrievers/base.py
--rw-r--r--   0        0        0     8661 2023-08-02 14:30:41.485287 codedog-0.5.3/codedog/retrievers/github_retriever.py
--rw-r--r--   0        0        0      126 2023-07-30 08:13:28.124920 codedog-0.5.3/codedog/retrievers/gitlab_retriever.py
--rw-r--r--   0        0        0        0 2023-07-15 01:59:22.106348 codedog-0.5.3/codedog/templates/__init__.py
--rw-r--r--   0        0        0     2910 2023-07-22 00:54:46.880133 codedog-0.5.3/codedog/templates/grimoire_cn.py
--rw-r--r--   0        0        0     4542 2023-07-30 08:13:28.167198 codedog-0.5.3/codedog/templates/grimoire_en.py
--rw-r--r--   0        0        0     1018 2023-07-22 00:54:46.914141 codedog-0.5.3/codedog/templates/template_cn.py
--rw-r--r--   0        0        0     3387 2023-07-30 08:13:28.228587 codedog-0.5.3/codedog/templates/template_en.py
--rw-r--r--   0        0        0        0 2023-08-02 13:57:13.330242 codedog-0.5.3/codedog/utils/__init__.py
--rw-r--r--   0        0        0      486 2023-07-25 13:00:53.522488 codedog-0.5.3/codedog/utils/diff_utils.py
--rw-r--r--   0        0        0      935 2023-07-30 08:13:28.243590 codedog-0.5.3/codedog/utils/langchain_utils.py
--rw-r--r--   0        0        0      118 2023-07-30 08:13:28.244591 codedog-0.5.3/codedog/version.py
--rw-r--r--   0        0        0     1067 2023-07-30 08:13:27.833259 codedog-0.5.3/LICENSE
--rw-r--r--   0        0        0     1857 2023-08-02 14:37:21.412244 codedog-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1874 2023-07-30 11:18:08.325034 codedog-0.5.3/README.md
--rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 codedog-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      328 2023-07-30 08:13:27.833259 codedog-0.5.4/codedog/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:13:27.834259 codedog-0.5.4/codedog/actors/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-30 08:13:27.834259 codedog-0.5.4/codedog/actors/base.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:13:27.834259 codedog-0.5.4/codedog/actors/reporters/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-30 08:13:27.834259 codedog-0.5.4/codedog/actors/reporters/base.py
+-rw-r--r--   0        0        0     1078 2023-07-30 08:13:27.835260 codedog-0.5.4/codedog/actors/reporters/code_review.py
+-rw-r--r--   0        0        0     2842 2023-08-02 14:31:22.564488 codedog-0.5.4/codedog/actors/reporters/pr_summary.py
+-rw-r--r--   0        0        0     2207 2023-07-30 08:13:27.835260 codedog-0.5.4/codedog/actors/reporters/pull_request.py
+-rw-r--r--   0        0        0      167 2023-07-30 08:13:27.835260 codedog-0.5.4/codedog/chains/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:13:27.854264 codedog-0.5.4/codedog/chains/code_review/__init__.py
+-rw-r--r--   0        0        0     4143 2023-08-02 14:30:41.484288 codedog-0.5.4/codedog/chains/code_review/base.py
+-rw-r--r--   0        0        0      231 2023-07-30 08:13:27.854264 codedog-0.5.4/codedog/chains/code_review/prompts.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:00:53.472920 codedog-0.5.4/codedog/chains/pr_summary/__init__.py
+-rw-r--r--   0        0        0     6360 2023-08-03 03:19:51.511130 codedog-0.5.4/codedog/chains/pr_summary/base.py
+-rw-r--r--   0        0        0      579 2023-07-25 13:00:53.474921 codedog-0.5.4/codedog/chains/pr_summary/prompts.py
+-rw-r--r--   0        0        0      714 2023-07-30 08:13:27.979292 codedog-0.5.4/codedog/localization.py
+-rw-r--r--   0        0        0      738 2023-07-30 08:13:28.073313 codedog-0.5.4/codedog/models/__init__.py
+-rw-r--r--   0        0        0      408 2023-07-25 13:00:53.493925 codedog-0.5.4/codedog/models/blob.py
+-rw-r--r--   0        0        0     2018 2023-07-30 08:13:28.073313 codedog-0.5.4/codedog/models/change_file.py
+-rw-r--r--   0        0        0      192 2023-07-25 13:00:53.493925 codedog-0.5.4/codedog/models/change_summary.py
+-rw-r--r--   0        0        0      150 2023-07-30 08:13:28.106320 codedog-0.5.4/codedog/models/code_review.py
+-rw-r--r--   0        0        0      800 2023-07-25 13:00:53.494925 codedog-0.5.4/codedog/models/commit.py
+-rw-r--r--   0        0        0     1148 2023-07-25 13:00:53.494925 codedog-0.5.4/codedog/models/diff.py
+-rw-r--r--   0        0        0      824 2023-07-25 13:00:53.494925 codedog-0.5.4/codedog/models/issue.py
+-rw-r--r--   0        0        0      692 2023-07-30 08:13:28.106320 codedog-0.5.4/codedog/models/pr_summary.py
+-rw-r--r--   0        0        0     1703 2023-07-30 08:13:28.107321 codedog-0.5.4/codedog/models/pull_request.py
+-rw-r--r--   0        0        0      998 2023-07-25 13:00:53.495925 codedog-0.5.4/codedog/models/repository.py
+-rw-r--r--   0        0        0      111 2023-07-30 08:13:28.123920 codedog-0.5.4/codedog/processors/__init__.py
+-rw-r--r--   0        0        0     3835 2023-07-30 08:13:28.123920 codedog-0.5.4/codedog/processors/pull_request_processor.py
+-rw-r--r--   0        0        0      178 2023-07-25 13:00:53.496925 codedog-0.5.4/codedog/retrievers/__init__.py
+-rw-r--r--   0        0        0     1375 2023-07-25 13:00:53.496925 codedog-0.5.4/codedog/retrievers/base.py
+-rw-r--r--   0        0        0     8661 2023-08-02 14:30:41.485287 codedog-0.5.4/codedog/retrievers/github_retriever.py
+-rw-r--r--   0        0        0      126 2023-07-30 08:13:28.124920 codedog-0.5.4/codedog/retrievers/gitlab_retriever.py
+-rw-r--r--   0        0        0        0 2023-07-15 01:59:22.106348 codedog-0.5.4/codedog/templates/__init__.py
+-rw-r--r--   0        0        0     2910 2023-07-22 00:54:46.880133 codedog-0.5.4/codedog/templates/grimoire_cn.py
+-rw-r--r--   0        0        0     4542 2023-07-30 08:13:28.167198 codedog-0.5.4/codedog/templates/grimoire_en.py
+-rw-r--r--   0        0        0     1018 2023-07-22 00:54:46.914141 codedog-0.5.4/codedog/templates/template_cn.py
+-rw-r--r--   0        0        0     3387 2023-07-30 08:13:28.228587 codedog-0.5.4/codedog/templates/template_en.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:57:13.330242 codedog-0.5.4/codedog/utils/__init__.py
+-rw-r--r--   0        0        0      486 2023-07-25 13:00:53.522488 codedog-0.5.4/codedog/utils/diff_utils.py
+-rw-r--r--   0        0        0      935 2023-07-30 08:13:28.243590 codedog-0.5.4/codedog/utils/langchain_utils.py
+-rw-r--r--   0        0        0      118 2023-07-30 08:13:28.244591 codedog-0.5.4/codedog/version.py
+-rw-r--r--   0        0        0     1067 2023-07-30 08:13:27.833259 codedog-0.5.4/LICENSE
+-rw-r--r--   0        0        0     1857 2023-08-03 03:21:16.015273 codedog-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1874 2023-07-30 11:18:08.325034 codedog-0.5.4/README.md
+-rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 codedog-0.5.4/PKG-INFO
```

### Comparing `codedog-0.5.3/codedog/actors/reporters/code_review.py` & `codedog-0.5.4/codedog/actors/reporters/code_review.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/actors/reporters/pr_summary.py` & `codedog-0.5.4/codedog/actors/reporters/pr_summary.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/actors/reporters/pull_request.py` & `codedog-0.5.4/codedog/actors/reporters/pull_request.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/chains/code_review/base.py` & `codedog-0.5.4/codedog/chains/code_review/base.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/chains/pr_summary/base.py` & `codedog-0.5.4/codedog/chains/pr_summary/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         code_summary_inputs = self._process_code_summary_inputs(pr)
         code_summary_outputs = (
             await self.code_summary_chain.aapply(code_summary_inputs, callbacks=_run_manager.get_child())
             if code_summary_inputs
             else []
         )
 
-        code_summaries = self.processor.build_code_summaries(code_summary_inputs, code_summary_outputs)
+        code_summaries = self.processor.build_change_summaries(code_summary_inputs, code_summary_outputs)
 
         pr_summary_input = self._process_pr_summary_input(pr, code_summaries)
         pr_summary_output: PRSummary = await self.pr_summary_chain(pr_summary_input, callbacks=_run_manager.get_child())
 
         return self._process_result(pr_summary_output, code_summaries)
 
     def _process_code_summary_inputs(self, pr: PullRequest) -> List[Dict[str, str]]:
```

### Comparing `codedog-0.5.3/codedog/chains/pr_summary/prompts.py` & `codedog-0.5.4/codedog/chains/pr_summary/prompts.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/localization.py` & `codedog-0.5.4/codedog/localization.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/models/__init__.py` & `codedog-0.5.4/codedog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/models/change_file.py` & `codedog-0.5.4/codedog/models/change_file.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/models/commit.py` & `codedog-0.5.4/codedog/models/commit.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/models/diff.py` & `codedog-0.5.4/codedog/models/diff.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/models/issue.py` & `codedog-0.5.4/codedog/models/issue.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/models/pr_summary.py` & `codedog-0.5.4/codedog/models/pr_summary.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/models/pull_request.py` & `codedog-0.5.4/codedog/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/models/repository.py` & `codedog-0.5.4/codedog/models/repository.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/processors/pull_request_processor.py` & `codedog-0.5.4/codedog/processors/pull_request_processor.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/retrievers/base.py` & `codedog-0.5.4/codedog/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/retrievers/github_retriever.py` & `codedog-0.5.4/codedog/retrievers/github_retriever.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/templates/grimoire_cn.py` & `codedog-0.5.4/codedog/templates/grimoire_cn.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/templates/grimoire_en.py` & `codedog-0.5.4/codedog/templates/grimoire_en.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/templates/template_cn.py` & `codedog-0.5.4/codedog/templates/template_cn.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/templates/template_en.py` & `codedog-0.5.4/codedog/templates/template_en.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/codedog/utils/langchain_utils.py` & `codedog-0.5.4/codedog/utils/langchain_utils.py`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/LICENSE` & `codedog-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/pyproject.toml` & `codedog-0.5.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codedog"
-version = "0.5.3"
+version = "0.5.4"
 license = "MIT"
 readme = "README.md"
 authors = ["Arcadia <arcadia822@gmail.com>", "Linpp "]
 description = "Codedog reviews your pull request using llm."
 repository = "https://www.github.com/codedog-ai/codedog"
 homepage = "https://www.codedog.ai"
 keywords = ["code review", "langchain", "llm"]
```

### Comparing `codedog-0.5.3/README.md` & `codedog-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `codedog-0.5.3/PKG-INFO` & `codedog-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedog
-Version: 0.5.3
+Version: 0.5.4
 Summary: Codedog reviews your pull request using llm.
 Home-page: https://www.codedog.ai
 License: MIT
 Keywords: code review,langchain,llm
 Author: Arcadia
 Author-email: arcadia822@gmail.com
 Requires-Python: >=3.10,<3.11
```

