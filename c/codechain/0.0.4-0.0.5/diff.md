# Comparing `tmp/codechain-0.0.4.tar.gz` & `tmp/codechain-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codechain-0.0.4.tar", last modified: Mon Jul 31 17:31:26 2023, max compression
+gzip compressed data, was "codechain-0.0.5.tar", last modified: Thu Aug  3 12:35:48 2023, max compression
```

## Comparing `codechain-0.0.4.tar` & `codechain-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-31 17:31:26.589179 codechain-0.0.4/
--rw-r--r--   0 james      (501) staff       (20)     1587 2023-07-31 17:31:26.589038 codechain-0.0.4/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1011 2023-07-27 11:41:19.000000 codechain-0.0.4/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-31 17:31:26.587963 codechain-0.0.4/codechain/
--rw-r--r--   0 james      (501) staff       (20)       69 2023-07-27 01:45:29.000000 codechain-0.0.4/codechain/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      948 2023-07-27 16:35:20.000000 codechain-0.0.4/codechain/evaluation.py
--rw-r--r--   0 james      (501) staff       (20)     3416 2023-07-27 16:38:54.000000 codechain-0.0.4/codechain/generation.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-31 17:31:26.588834 codechain-0.0.4/codechain.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     1587 2023-07-31 17:31:26.000000 codechain-0.0.4/codechain.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      252 2023-07-31 17:31:26.000000 codechain-0.0.4/codechain.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-07-31 17:31:26.000000 codechain-0.0.4/codechain.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       10 2023-07-31 17:31:26.000000 codechain-0.0.4/codechain.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       10 2023-07-31 17:31:26.000000 codechain-0.0.4/codechain.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-07-31 17:31:26.589217 codechain-0.0.4/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1066 2023-07-31 16:04:44.000000 codechain-0.0.4/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-03 12:35:48.826333 codechain-0.0.5/
+-rw-r--r--   0 james      (501) staff       (20)     1664 2023-08-03 12:35:48.826178 codechain-0.0.5/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1088 2023-08-03 12:32:12.000000 codechain-0.0.5/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-03 12:35:48.825271 codechain-0.0.5/codechain/
+-rw-r--r--   0 james      (501) staff       (20)       69 2023-07-27 01:45:29.000000 codechain-0.0.5/codechain/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      929 2023-08-03 12:13:01.000000 codechain-0.0.5/codechain/evaluation.py
+-rw-r--r--   0 james      (501) staff       (20)     3645 2023-08-03 12:25:24.000000 codechain-0.0.5/codechain/generation.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-03 12:35:48.825990 codechain-0.0.5/codechain.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     1664 2023-08-03 12:35:48.000000 codechain-0.0.5/codechain.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      252 2023-08-03 12:35:48.000000 codechain-0.0.5/codechain.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-08-03 12:35:48.000000 codechain-0.0.5/codechain.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       10 2023-08-03 12:35:48.000000 codechain-0.0.5/codechain.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       10 2023-08-03 12:35:48.000000 codechain-0.0.5/codechain.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-08-03 12:35:48.826377 codechain-0.0.5/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1066 2023-08-03 12:33:37.000000 codechain-0.0.5/setup.py
```

### Comparing `codechain-0.0.4/PKG-INFO` & `codechain-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codechain
-Version: 0.0.4
+Version: 0.0.5
 Summary: Code generation with LLMs
 Author: James Murdza
 Author-email: <james@jamesmurdza.com>
 Project-URL: Source, https://github.com/jamesmurdza/codechain
 Keywords: python,llms,codegen,code generation
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -17,27 +17,31 @@
 
 # CodeChain
 
 CodeChain is a library for generating and evaluating code with LLMs.
 
 To install: `pip install codechain`
 
+To install from source: `pip install -e .`
+
+To run unit tests: `python tests/*.py`
+
 ## Code completion
 
 Usage is very simple:
 
 ```python
 from codechain.generation import CompleteCodeChain
 from langchain.chat_models import ChatOpenAI
 
 generator = CompleteCodeChain.from_llm(
     ChatOpenAI(model="gpt-3.5-turbo", temperature=0.2)
     )
 
-result = await generator.arun("""
+result = generator.run("""
 def fibonacci(n):
 # Generate the n-th fibonacci number.
 """)
 
 print(result)
 ```
```

### Comparing `codechain-0.0.4/README.md` & `codechain-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # CodeChain
 
 CodeChain is a library for generating and evaluating code with LLMs.
 
 To install: `pip install codechain`
 
+To install from source: `pip install -e .`
+
+To run unit tests: `python tests/*.py`
+
 ## Code completion
 
 Usage is very simple:
 
 ```python
 from codechain.generation import CompleteCodeChain
 from langchain.chat_models import ChatOpenAI
 
 generator = CompleteCodeChain.from_llm(
     ChatOpenAI(model="gpt-3.5-turbo", temperature=0.2)
     )
 
-result = await generator.arun("""
+result = generator.run("""
 def fibonacci(n):
 # Generate the n-th fibonacci number.
 """)
 
 print(result)
 ```
```

### Comparing `codechain-0.0.4/codechain/evaluation.py` & `codechain-0.0.5/codechain/evaluation.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.problems = read_problems()
 
     def evaluate_run(self, run: Run, example: Optional[Example] = None) -> EvaluationResult:
 
         from human_eval.execution import check_correctness
 
         print("Evaluating " + run.inputs["task_id"])
-        problem = HumanEvalEvaluator.self.problems[run.inputs["task_id"]]
+        problem = self.problems[run.inputs["task_id"]]
         solution = run.outputs["output"]
 
         # The HumanEval evaluator, which runs the Python code against unit tests
         result = check_correctness(problem, solution, 5)
 
         return EvaluationResult(
             key = "Correctness",
```

### Comparing `codechain-0.0.4/codechain/generation.py` & `codechain-0.0.5/codechain/generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from typing import Dict
 
 from langchain.chains import LLMChain, SimpleSequentialChain, SequentialChain, TransformChain
-from langchain.prompts import PromptTemplate
+from langchain.prompts import BasePromptTemplate, PromptTemplate
 from langchain.base_language import BaseLanguageModel
 import re
 
 class CodeChain(SimpleSequentialChain):
     """ Chain that generates code from a prompt. """
     
     @staticmethod
-    async def extract_code(inputs: dict) -> dict:
+    def extract_code(inputs: dict) -> dict:
         text = inputs["text"]
         result = re.search(r'```.*?\n(.*?)\n```', text, re.DOTALL)
         result = result.group(1) if result else text
         return {"output": result}
+    
+    @staticmethod
+    async def aextract_code(inputs: dict) -> dict:
+        return CodeChain.extract_code(inputs)
 
     @classmethod
-    def from_prompt(cls, prompt, llm: BaseLanguageModel) -> "CodeChain":
+    def from_prompt(cls, prompt: BasePromptTemplate, llm: BaseLanguageModel) -> "CodeChain":
         """ Return the code block from a Markdown chat response. """
 
         llm_chain = LLMChain(prompt=prompt, llm=llm)
         transform_chain = TransformChain(
             input_variables=["text"],
             output_variables=["output"],
             transform=CodeChain.extract_code,
-            atransform=CodeChain.extract_code
+            atransform=CodeChain.aextract_code
         )
         return cls(
             chains=[llm_chain, transform_chain]
         )
 
 class ModifyCodeChain(CodeChain):
     """ Chain that modifies code according to the given instruction. """
@@ -53,22 +57,25 @@
 
 class InputMapper(TransformChain):
   """ Chain that maps input variables to output variables. """
 
   @classmethod
   def from_mapping(cls, mapping: Dict) -> "InputMapper":
 
-      async def map_dict(input_dict: Dict) -> Dict:
+      def map_dict(input_dict: Dict) -> Dict:
         return {mapping[input]: value for input, value in input_dict.items() if input in mapping}
 
-      return TransformChain(
+      async def amap_dict(input_dict: Dict) -> Dict:
+        return map_dict(input_dict)
+
+      return cls(
           input_variables=[input for input in mapping.keys()],
           output_variables=[output for output in mapping.values() if output is not None],
           transform=map_dict,
-          atransform=map_dict
+          atransform=amap_dict
       )
 
 class HumanEvalChain(SequentialChain):
   """ Chain that generates a solution to a HumanEval problem. """
 
   @classmethod
   def from_chain(cls, chain: CodeChain) -> "HumanEvalChain":
```

### Comparing `codechain-0.0.4/codechain.egg-info/PKG-INFO` & `codechain-0.0.5/codechain.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codechain
-Version: 0.0.4
+Version: 0.0.5
 Summary: Code generation with LLMs
 Author: James Murdza
 Author-email: <james@jamesmurdza.com>
 Project-URL: Source, https://github.com/jamesmurdza/codechain
 Keywords: python,llms,codegen,code generation
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -17,27 +17,31 @@
 
 # CodeChain
 
 CodeChain is a library for generating and evaluating code with LLMs.
 
 To install: `pip install codechain`
 
+To install from source: `pip install -e .`
+
+To run unit tests: `python tests/*.py`
+
 ## Code completion
 
 Usage is very simple:
 
 ```python
 from codechain.generation import CompleteCodeChain
 from langchain.chat_models import ChatOpenAI
 
 generator = CompleteCodeChain.from_llm(
     ChatOpenAI(model="gpt-3.5-turbo", temperature=0.2)
     )
 
-result = await generator.arun("""
+result = generator.run("""
 def fibonacci(n):
 # Generate the n-th fibonacci number.
 """)
 
 print(result)
 ```
```

### Comparing `codechain-0.0.4/setup.py` & `codechain-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Code generation with LLMs'
 
 # Setting up
 setup(
     name="codechain",
     version=VERSION,
     author="James Murdza",
```

