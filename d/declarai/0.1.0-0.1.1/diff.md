# Comparing `tmp/declarai-0.1.0.tar.gz` & `tmp/declarai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "declarai-0.1.0.tar", max compression
+gzip compressed data, was "declarai-0.1.1.tar", max compression
```

## Comparing `declarai-0.1.0.tar` & `declarai-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,76 @@
--rw-r--r--   0        0        0     1065 2023-07-24 18:50:16.069080 declarai-0.1.0/LICENSE
--rw-r--r--   0        0        0     5970 2023-07-24 18:50:16.069080 declarai-0.1.0/README.md
--rw-r--r--   0        0        0      449 2023-07-24 18:50:16.069080 declarai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/configurations/__init__.py
--rw-r--r--   0        0        0      271 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/configurations/prompt_config.py
--rw-r--r--   0        0        0      250 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/llm/__init__.py
--rw-r--r--   0        0        0      217 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/llm/base_llm.py
--rw-r--r--   0        0        0       94 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/llm/config.py
--rw-r--r--   0        0        0       34 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/llm/openai_llm/__init__.py
--rw-r--r--   0        0        0       99 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/llm/openai_llm/config.py
--rw-r--r--   0        0        0      996 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/llm/openai_llm/openai_llm.py
--rw-r--r--   0        0        0       44 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/python_parser/__init__.py
--rw-r--r--   0        0        0     1794 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/python_parser/function_parser.py
--rw-r--r--   0        0        0     2816 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/python_parser/method_docstring_parser.py
--rw-r--r--   0        0        0     2444 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/reducer.py
--rw-r--r--   0        0        0     3167 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/task.py
--rw-r--r--   0        0        0        0 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/tasks/__init__.py
--rw-r--r--   0        0        0     2498 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/tasks/base_llm_task.py
--rw-r--r--   0        0        0     2182 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/tasks/func_llm_translator.py
--rw-r--r--   0        0        0      110 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/templates/__init__.py
--rw-r--r--   0        0        0      191 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/templates/chain_of_thought.py
--rw-r--r--   0        0        0       98 2023-07-24 18:50:16.069080 declarai-0.1.0/src/declarai/templates/instruct_function.py
--rw-r--r--   0        0        0     6385 1970-01-01 00:00:00.000000 declarai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-03 16:51:13.176588 declarai-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4169 2023-08-03 16:51:13.176588 declarai-0.1.1/README.md
+-rw-r--r--   0        0        0      646 2023-08-03 16:51:13.188588 declarai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/core/__init__.py
+-rw-r--r--   0        0        0      279 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/core/core_settings.py
+-rw-r--r--   0        0        0     1567 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/declarai.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/decorators/__init__.py
+-rw-r--r--   0        0        0      983 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/decorators/base.py
+-rw-r--r--   0        0        0     1496 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/decorators/chat_decorator.py
+-rw-r--r--   0        0        0      645 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/decorators/magic.py
+-rw-r--r--   0        0        0      569 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/decorators/task_decorator.py
+-rw-r--r--   0        0        0     6647 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/__init__.py
+-rw-r--r--   0        0        0     5989 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/evaluator.py
+-rw-r--r--   0        0        0      422 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/extraction/__init__.py
+-rw-r--r--   0        0        0      486 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/extraction/multiple_value.py
+-rw-r--r--   0        0        0      682 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/extraction/multiple_value_multi_types.py
+-rw-r--r--   0        0        0      427 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/extraction/single_value.py
+-rw-r--r--   0        0        0      631 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/extraction/single_value_multi_types.py
+-rw-r--r--   0        0        0      484 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/generation/__init__.py
+-rw-r--r--   0        0        0      693 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/generation/structured_open_ended.py
+-rw-r--r--   0        0        0     1224 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/generation/structured_strict_complex.py
+-rw-r--r--   0        0        0      270 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/generation/unstructured_long_form.py
+-rw-r--r--   0        0        0      251 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/generation/unstructured_short_form.py
+-rw-r--r--   0        0        0       64 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/logical_tasks/__init__.py
+-rw-r--r--   0        0        0     2082 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/logical_tasks/sequence.py
+-rw-r--r--   0        0        0       86 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/manipulation/__init__.py
+-rw-r--r--   0        0        0      586 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/manipulation/data_manipulation_structured.py
+-rw-r--r--   0        0        0      393 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/metadata_significance/__init__.py
+-rw-r--r--   0        0        0     1550 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/metadata_significance/simple_task_significance.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/providers/__init__.py
+-rw-r--r--   0        0        0      549 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/providers/openai.py
+-rw-r--r--   0        0        0     3763 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/runner.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/middlewares/__init__.py
+-rw-r--r--   0        0        0      610 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/middlewares/base.py
+-rw-r--r--   0        0        0       46 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/middlewares/declarai/__init__.py
+-rw-r--r--   0        0        0     1177 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/middlewares/declarai/log_middleware.py
+-rw-r--r--   0        0        0       48 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/middlewares/third_party/__init__.py
+-rw-r--r--   0        0        0     2947 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/middlewares/third_party/wandb_monitor.py
+-rw-r--r--   0        0        0     1345 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/__init__.py
+-rw-r--r--   0        0        0     1845 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/llm_settings.py
+-rw-r--r--   0        0        0       98 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/types/__init__.py
+-rw-r--r--   0        0        0      721 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/types/llm.py
+-rw-r--r--   0        0        0      510 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/types/message.py
+-rw-r--r--   0        0        0      701 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/types/operator.py
+-rw-r--r--   0        0        0       46 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/__init__.py
+-rw-r--r--   0        0        0     2796 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/chat_operator.py
+-rw-r--r--   0        0        0       34 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/openai_llm/__init__.py
+-rw-r--r--   0        0        0     1840 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/openai_llm/openai_llm.py
+-rw-r--r--   0        0        0      298 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/openai_llm/settings.py
+-rw-r--r--   0        0        0     3916 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/task_operator.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/__init__.py
+-rw-r--r--   0        0        0     1709 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/output_prompt.py
+-rw-r--r--   0        0        0      215 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/templates/__init__.py
+-rw-r--r--   0        0        0      189 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/templates/chain_of_thought.py
+-rw-r--r--   0        0        0       75 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/templates/instruct_function.py
+-rw-r--r--   0        0        0      371 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/templates/output_structure.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/__init__.py
+-rw-r--r--   0        0        0     2559 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/chat_orchestrator.py
+-rw-r--r--   0        0        0      745 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/future_llm_task.py
+-rw-r--r--   0        0        0     2822 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/sequence.py
+-rw-r--r--   0        0        0     2821 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/task_orchestrator.py
+-rw-r--r--   0        0        0      124 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/types.py
+-rw-r--r--   0        0        0       38 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/annotations/__init__.py
+-rw-r--r--   0        0        0     2433 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/annotations/type_annotation_to_schema.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/docstring_parsers/__init__.py
+-rw-r--r--   0        0        0       40 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/docstring_parsers/reST/__init__.py
+-rw-r--r--   0        0        0     1922 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/docstring_parsers/reST/parser.py
+-rw-r--r--   0        0        0      445 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/docstring_parsers/types.py
+-rw-r--r--   0        0        0     1909 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/magic_parser.py
+-rw-r--r--   0        0        0     4925 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/parser.py
+-rw-r--r--   0        0        0      767 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/types.py
+-rw-r--r--   0        0        0     4817 1970-01-01 00:00:00.000000 declarai-0.1.1/PKG-INFO
```

### Comparing `declarai-0.1.0/LICENSE` & `declarai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `declarai-0.1.0/src/declarai/reducer.py` & `declarai-0.1.1/src/declarai/orchestrator/sequence.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,87 @@
 """Reducer
 
 The reducer allows chaining together a collection of tasks.
 The reducer than compiles the tasks into a single task that can be executed.
 At the moment the reducer only supports reducing tasks using the `chain of thought` strategy.
 
 Usage:
-    >>> reducer = Reducer()
+    >>> reducer = Sequence()
     >>> reducer.add("step1", func1, param1=1, param2=2)
     >>> reducer.add("step2", func2, param1="step1")
     >>> reducer.add("step3", func3, param1="step2")
     >>> reducer.execute()
     # You can also compile your tasks withouth executing them to review the generated task
     >>> reducer.compile()
 """
 
-from typing import Any
+from typing import Optional, Set, Tuple
 
-from declarai import templates
-from declarai.tasks.base_llm_task import BaseLLMTask
+from typing_extensions import Literal
 
+from declarai.operators.shared import templates
+from declarai.orchestrator.future_llm_task import FutureLLMTask
 
-class Reducer:
-    def __init__(self):
-        self.res = {}
-
-    def add(self, name, func, **kwargs):
-        template = templates.InstructFunctionTemplate.format(
-            input_instructions=func.llm_translator.parsed_func.doc_description,
-            input_placeholder=func.llm_translator.make_input_placeholder(),
-            output_instructions=func.llm_translator.make_output_prompt(
-                return_name=name
-            ),
-        )
-
-        llm_task = BaseLLMTask(template=template)
-        func.llm_task = llm_task
-        self.res[name] = (func, kwargs)
-
-    @staticmethod
-    def get_ai_func_template(function, kwargs):
-        return function.llm_task.populate_template(**kwargs)
-
-    def __compile(self):
-        step_count = len(self.res)
-        steps = ""
-        for step, step_function in enumerate(self.res.values()):
-            function, kwargs = step_function
-            for k, v in kwargs.items():
-                if isinstance(v, tuple) and callable(v[0]):
-                    kwargs[k] = "From previous step"
-            step_prompt = self.get_ai_func_template(function, kwargs)
-            steps += f"Step {step + 1}: {step_prompt}\n"
-
-        ai_func = BaseLLMTask(
-            template=templates.ChainOfThoughtsTemplate.format(
-                num_steps=step_count,
-                steps=steps,
+ReduceStrategies = Literal["ChainOfThought"]
+
+
+class Sequence:
+    def __init__(
+        self,
+        ai_future_task: FutureLLMTask,
+        reduce_strategy: Optional[ReduceStrategies] = "ChainOfThought",
+    ):
+        """
+
+        :param ai_future_task: A result to calling `.plan(...)` on a declarai task
+        :param reduce_strategy: The strategy to use for reducing the tasks
+        """
+        self.ai_future_task = ai_future_task
+        self.reduce_strategy = reduce_strategy
+
+    def _exec(self):
+        """
+        Executes the task
+        :return: The result of the task
+        """
+        if self.reduce_strategy == "ChainOfThought":
+            prompt, num_steps = chain_of_thought_reducer(self.ai_future_task)
+            reduced_prompt = templates.ChainOfThoughtsTemplate.format(
+                steps=prompt, num_steps=num_steps
             )
-        )
-        return ai_func
+            self.ai_future_task.exec_func.__self__.prompt_config.multi_results = True
+            return self.ai_future_task.exec_func(reduced_prompt)
 
-    def execute(self) -> Any:
-        compiled_ai_func = self.__compile()
-        res = compiled_ai_func.generate_structured(
-            compiled_ai_func.generation_template, multi_results=True
-        )
-        return res
+    def __call__(self):
+        return self._exec()
 
-    def compile(self):
-        return self.__compile().generation_template
 
-    def __getitem__(self, item):
-        return self.res[item]
+def chain_of_thought_reducer(
+    future_task: FutureLLMTask,
+    prompt: str = "",
+    steps: int = 0,
+    visited_tasks: Set = None,
+) -> Tuple[str, int]:
+    """
+    Recursive resolving of future_ai_tasks
+    and compiling them into a single task with the chain of thought strategy.
+    """
+    if not visited_tasks:
+        visited_tasks = set()
+
+    kwargs = future_task.task_kwargs
+
+    for param, value in kwargs.items():
+        if isinstance(value, FutureLLMTask):
+            if value not in visited_tasks:
+                visited_tasks.add(value)
+                new_prompt, new_steps = chain_of_thought_reducer(
+                    value, "", steps, visited_tasks
+                )
+                prompt += new_prompt
+                steps = new_steps
+            kwargs[param] = "From previous steps"
+
+    steps += 1
+    task_prompt = f"\nStep {steps}:\n{future_task.compiled_template.format(**kwargs)}"
+    prompt += task_prompt
+    return prompt, steps
```

