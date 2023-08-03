# Comparing `tmp/python_statemachine-2.1.0.tar.gz` & `tmp/python_statemachine-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_statemachine-2.1.0.tar", max compression
+gzip compressed data, was "python_statemachine-2.1.1.tar", max compression
```

## Comparing `python_statemachine-2.1.0.tar` & `python_statemachine-2.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1074 2023-01-12 02:09:26.102515 python_statemachine-2.1.0/LICENSE
--rw-r--r--   0        0        0    10510 2023-06-12 01:16:16.754636 python_statemachine-2.1.0/README.md
--rw-r--r--   0        0        0     3966 2023-06-12 01:17:52.284641 python_statemachine-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      192 2023-06-12 01:17:52.284641 python_statemachine-2.1.0/statemachine/__init__.py
--rw-r--r--   0        0        0     5714 2023-06-12 01:16:16.754636 python_statemachine-2.1.0/statemachine/callbacks.py
--rw-r--r--   0        0        0        0 2023-01-12 02:09:26.112515 python_statemachine-2.1.0/statemachine/contrib/__init__.py
--rw-r--r--   0        0        0     6748 2023-03-05 22:27:00.883303 python_statemachine-2.1.0/statemachine/contrib/diagram.py
--rw-r--r--   0        0        0     2884 2023-06-12 01:16:16.754636 python_statemachine-2.1.0/statemachine/dispatcher.py
--rw-r--r--   0        0        0     2106 2023-03-13 01:49:09.127086 python_statemachine-2.1.0/statemachine/event.py
--rw-r--r--   0        0        0     2257 2023-03-13 01:45:45.507089 python_statemachine-2.1.0/statemachine/event_data.py
--rw-r--r--   0        0        0      731 2023-03-05 22:27:00.883303 python_statemachine-2.1.0/statemachine/events.py
--rw-r--r--   0        0        0      952 2023-03-13 01:45:45.507089 python_statemachine-2.1.0/statemachine/exceptions.py
--rw-r--r--   0        0        0     5557 2023-06-12 01:16:16.754636 python_statemachine-2.1.0/statemachine/factory.py
--rw-r--r--   0        0        0      359 2023-01-12 02:09:26.112515 python_statemachine-2.1.0/statemachine/graph.py
--rw-r--r--   0        0        0      362 2023-03-05 22:27:00.883303 python_statemachine-2.1.0/statemachine/i18n.py
--rw-r--r--   0        0        0      452 2023-06-12 01:10:29.514642 python_statemachine-2.1.0/statemachine/locale/en/LC_MESSAGES/statemachine.mo
--rw-r--r--   0        0        0     1685 2023-06-12 01:17:52.284641 python_statemachine-2.1.0/statemachine/locale/en/LC_MESSAGES/statemachine.po
--rw-r--r--   0        0        0     1914 2023-06-12 01:10:29.514642 python_statemachine-2.1.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.mo
--rw-r--r--   0        0        0     2375 2023-06-12 01:17:52.284641 python_statemachine-2.1.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po
--rw-r--r--   0        0        0     1055 2023-03-13 01:45:45.507089 python_statemachine-2.1.0/statemachine/mixins.py
--rw-r--r--   0        0        0      211 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/model.py
--rw-r--r--   0        0        0      959 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/registry.py
--rw-r--r--   0        0        0     6260 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/signature.py
--rw-r--r--   0        0        0     7057 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/state.py
--rw-r--r--   0        0        0    11608 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/statemachine.py
--rw-r--r--   0        0        0     4151 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/states.py
--rw-r--r--   0        0        0     4637 2023-03-13 01:45:45.507089 python_statemachine-2.1.0/statemachine/transition.py
--rw-r--r--   0        0        0     5949 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/transition_list.py
--rw-r--r--   0        0        0      367 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/utils.py
--rw-r--r--   0        0        0    11639 1970-01-01 00:00:00.000000 python_statemachine-2.1.0/setup.py
--rw-r--r--   0        0        0    11654 1970-01-01 00:00:00.000000 python_statemachine-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-01-12 02:09:26.102515 python_statemachine-2.1.1/LICENSE
+-rw-r--r--   0        0        0    10511 2023-08-03 11:07:28.388948 python_statemachine-2.1.1/README.md
+-rw-r--r--   0        0        0     3990 2023-08-03 11:08:01.138949 python_statemachine-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      192 2023-08-03 11:08:01.138949 python_statemachine-2.1.1/statemachine/__init__.py
+-rw-r--r--   0        0        0     5714 2023-06-12 01:16:16.754636 python_statemachine-2.1.1/statemachine/callbacks.py
+-rw-r--r--   0        0        0        0 2023-01-12 02:09:26.112515 python_statemachine-2.1.1/statemachine/contrib/__init__.py
+-rw-r--r--   0        0        0     6748 2023-03-05 22:27:00.883303 python_statemachine-2.1.1/statemachine/contrib/diagram.py
+-rw-r--r--   0        0        0     2884 2023-06-12 01:16:16.754636 python_statemachine-2.1.1/statemachine/dispatcher.py
+-rw-r--r--   0        0        0     2106 2023-03-13 01:49:09.127086 python_statemachine-2.1.1/statemachine/event.py
+-rw-r--r--   0        0        0     2257 2023-03-13 01:45:45.507089 python_statemachine-2.1.1/statemachine/event_data.py
+-rw-r--r--   0        0        0      731 2023-03-05 22:27:00.883303 python_statemachine-2.1.1/statemachine/events.py
+-rw-r--r--   0        0        0      952 2023-03-13 01:45:45.507089 python_statemachine-2.1.1/statemachine/exceptions.py
+-rw-r--r--   0        0        0     5779 2023-08-03 11:07:28.388948 python_statemachine-2.1.1/statemachine/factory.py
+-rw-r--r--   0        0        0      359 2023-01-12 02:09:26.112515 python_statemachine-2.1.1/statemachine/graph.py
+-rw-r--r--   0        0        0      362 2023-03-05 22:27:00.883303 python_statemachine-2.1.1/statemachine/i18n.py
+-rw-r--r--   0        0        0      452 2023-06-12 01:10:29.514642 python_statemachine-2.1.1/statemachine/locale/en/LC_MESSAGES/statemachine.mo
+-rw-r--r--   0        0        0     1685 2023-06-12 01:17:52.284641 python_statemachine-2.1.1/statemachine/locale/en/LC_MESSAGES/statemachine.po
+-rw-r--r--   0        0        0     1914 2023-06-12 01:10:29.514642 python_statemachine-2.1.1/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.mo
+-rw-r--r--   0        0        0     2375 2023-06-12 01:17:52.284641 python_statemachine-2.1.1/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po
+-rw-r--r--   0        0        0     1055 2023-03-13 01:45:45.507089 python_statemachine-2.1.1/statemachine/mixins.py
+-rw-r--r--   0        0        0      211 2023-06-12 01:16:16.764636 python_statemachine-2.1.1/statemachine/model.py
+-rw-r--r--   0        0        0      959 2023-06-12 01:16:16.764636 python_statemachine-2.1.1/statemachine/registry.py
+-rw-r--r--   0        0        0     6592 2023-08-03 11:07:28.388948 python_statemachine-2.1.1/statemachine/signature.py
+-rw-r--r--   0        0        0     7057 2023-06-12 01:16:16.764636 python_statemachine-2.1.1/statemachine/state.py
+-rw-r--r--   0        0        0    11608 2023-08-02 16:39:14.549882 python_statemachine-2.1.1/statemachine/statemachine.py
+-rw-r--r--   0        0        0     4151 2023-06-12 01:16:16.764636 python_statemachine-2.1.1/statemachine/states.py
+-rw-r--r--   0        0        0     4637 2023-03-13 01:45:45.507089 python_statemachine-2.1.1/statemachine/transition.py
+-rw-r--r--   0        0        0     5949 2023-06-12 01:16:16.764636 python_statemachine-2.1.1/statemachine/transition_list.py
+-rw-r--r--   0        0        0      367 2023-06-12 01:16:16.764636 python_statemachine-2.1.1/statemachine/utils.py
+-rw-r--r--   0        0        0    11640 1970-01-01 00:00:00.000000 python_statemachine-2.1.1/setup.py
+-rw-r--r--   0        0        0    11655 1970-01-01 00:00:00.000000 python_statemachine-2.1.1/PKG-INFO
```

### Comparing `python_statemachine-2.1.0/LICENSE` & `python_statemachine-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/README.md` & `python_statemachine-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
 * <a class="github-button" href="https://github.com/fgmacedo/python-statemachine" data-icon="octicon-star" aria-label="Star fgmacedo/python-statemachine on GitHub">Star this project</a>
 * <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/issues" data-icon="octicon-issue-opened" aria-label="Issue fgmacedo/python-statemachine on GitHub">Open an Issue</a>
 * <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/fork" data-icon="octicon-repo-forked" aria-label="Fork fgmacedo/python-statemachine on GitHub">Fork</a>
 
 - If you found this project helpful, please consider giving it a star on GitHub.
 
 - **Contribute code**: If you would like to contribute code to this project, please submit a pull
-request. For more information on how to contribute, please see our [contributing.md]contributing.md) file.
+request. For more information on how to contribute, please see our [contributing.md](contributing.md) file.
 
 - **Report bugs**: If you find any bugs in this project, please report them by opening an issue
   on our GitHub issue tracker.
 
 - **Suggest features**: If you have a great idea for a new feature, please let us know by opening
   an issue on our GitHub issue tracker.
```

### Comparing `python_statemachine-2.1.0/pyproject.toml` & `python_statemachine-2.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-statemachine"
-version = "2.1.0"
+version = "2.1.1"
 description = "Python Finite State Machines made easy."
 authors = ["Fernando Macedo <fgmacedo@gmail.com>"]
 maintainers = [
     "Fernando Macedo <fgmacedo@gmail.com>",
 ]
 license = "MIT license"
 readme = "README.md"
@@ -41,14 +41,15 @@
 pytest-sugar = "^0.9.6"
 pydot = "^1.4.2"
 ruff = "^0.0.257"
 pre-commit = "^2.21.0"
 mypy = "^0.991"
 black = "^22.12.0"
 pdbpp = "^0.10.3"
+pytest-mock = "^3.10.0"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "4.5.0"
 sphinx-rtd-theme = "1.1.1"
 myst-parser = "^0.18.1"
 sphinx-gallery = "^0.11.1"
 pillow = "^9.4.0"
```

### Comparing `python_statemachine-2.1.0/statemachine/callbacks.py` & `python_statemachine-2.1.1/statemachine/callbacks.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/contrib/diagram.py` & `python_statemachine-2.1.1/statemachine/contrib/diagram.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/dispatcher.py` & `python_statemachine-2.1.1/statemachine/dispatcher.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/event.py` & `python_statemachine-2.1.1/statemachine/event.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/event_data.py` & `python_statemachine-2.1.1/statemachine/event_data.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/events.py` & `python_statemachine-2.1.1/statemachine/events.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/exceptions.py` & `python_statemachine-2.1.1/statemachine/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/factory.py` & `python_statemachine-2.1.1/statemachine/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Dict
+from typing import List
 from typing import Tuple
 from uuid import uuid4
 
 from . import registry
 from .event import Event
 from .event import trigger_event_factory
 from .exceptions import InvalidDefinition
@@ -27,52 +28,29 @@
 
         cls._abstract = True
         cls._events: Dict[str, Event] = {}
 
         cls.add_inherited(bases)
         cls.add_from_attributes(attrs)
 
-        cls._set_special_states()
+        try:
+            cls.initial_state: State = next(s for s in cls.states if s.initial)
+        except StopIteration:
+            cls.initial_state = None  # Abstract SM still don't have states
+
+        cls.final_states: List[State] = [state for state in cls.states if state.final]
+
         cls._check()
 
     if TYPE_CHECKING:
         """Makes mypy happy with dynamic created attributes"""
 
         def __getattr__(self, attribute: str) -> Any:
             ...
 
-    def _set_special_states(cls):
-        if not cls.states:
-            return
-        initials = [s for s in cls.states if s.initial]
-        if len(initials) != 1:
-            raise InvalidDefinition(
-                _(
-                    "There should be one and only one initial state. "
-                    "Your currently have these: {!r}"
-                ).format([s.id for s in initials])
-            )
-        cls.initial_state = initials[0]
-        cls.final_states = [state for state in cls.states if state.final]
-
-    def _disconnected_states(cls, starting_state):
-        visitable_states = set(visit_connected_states(starting_state))
-        return set(cls.states) - visitable_states
-
-    def _check_disconnected_state(cls):
-        disconnected_states = cls._disconnected_states(cls.initial_state)
-        if disconnected_states:
-            raise InvalidDefinition(
-                _(
-                    "There are unreachable states. "
-                    "The statemachine graph should have a single component. "
-                    "Disconnected states: {}"
-                ).format([s.id for s in disconnected_states])
-            )
-
     def _check(cls):
         has_states = bool(cls.states)
         has_events = bool(cls._events)
 
         cls._abstract = not has_states and not has_events
 
         # do not validate the base abstract classes
@@ -81,27 +59,55 @@
 
         if not has_states:
             raise InvalidDefinition(_("There are no states."))
 
         if not has_events:
             raise InvalidDefinition(_("There are no events."))
 
+        cls._check_initial_state()
+        cls._check_final_states()
         cls._check_disconnected_state()
 
+    def _check_initial_state(cls):
+        initials = [s for s in cls.states if s.initial]
+        if len(initials) != 1:
+            raise InvalidDefinition(
+                _(
+                    "There should be one and only one initial state. "
+                    "Your currently have these: {!r}"
+                ).format([s.id for s in initials])
+            )
+
+    def _check_final_states(cls):
         final_state_with_invalid_transitions = [
             state for state in cls.final_states if state.transitions
         ]
 
         if final_state_with_invalid_transitions:
             raise InvalidDefinition(
                 _(
                     "Cannot declare transitions from final state. Invalid state(s): {}"
                 ).format([s.id for s in final_state_with_invalid_transitions])
             )
 
+    def _disconnected_states(cls, starting_state):
+        visitable_states = set(visit_connected_states(starting_state))
+        return set(cls.states) - visitable_states
+
+    def _check_disconnected_state(cls):
+        disconnected_states = cls._disconnected_states(cls.initial_state)
+        if disconnected_states:
+            raise InvalidDefinition(
+                _(
+                    "There are unreachable states. "
+                    "The statemachine graph should have a single component. "
+                    "Disconnected states: {}"
+                ).format([s.id for s in disconnected_states])
+            )
+
     def add_inherited(cls, bases):
         for base in bases:
             for state in getattr(base, "states", []):
                 cls.add_state(state.id, state)
 
             events = getattr(base, "_events", {})
             for event in events.values():
```

### Comparing `python_statemachine-2.1.0/statemachine/locale/en/LC_MESSAGES/statemachine.po` & `python_statemachine-2.1.1/statemachine/locale/en/LC_MESSAGES/statemachine.po`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.mo` & `python_statemachine-2.1.1/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.mo`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po` & `python_statemachine-2.1.1/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/mixins.py` & `python_statemachine-2.1.1/statemachine/mixins.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/registry.py` & `python_statemachine-2.1.1/statemachine/registry.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/signature.py` & `python_statemachine-2.1.1/statemachine/signature.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,24 @@
         )
         return sig
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         ba = self.bind_expected(*args, **kwargs)
         return self.method(*ba.args, **ba.kwargs)
 
+    @classmethod
+    def from_callable(cls, method):
+        if hasattr(method, "__signature__"):
+            sig = method.__signature__
+            return SignatureAdapter(
+                sig.parameters.values(),
+                return_annotation=sig.return_annotation,
+            )
+        return super().from_callable(method)
+
     def bind_expected(self, *args: Any, **kwargs: Any) -> BoundArguments:  # noqa: C901
         """Get a BoundArguments object, that maps the passed `args`
         and `kwargs` to the function's signature.  It avoids to raise `TypeError`
         trying to fill all the required arguments and ignoring the unknown ones.
 
         Adapted from the internal `inspect.Signature._bind`.
         """
```

### Comparing `python_statemachine-2.1.0/statemachine/state.py` & `python_statemachine-2.1.1/statemachine/state.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/statemachine.py` & `python_statemachine-2.1.1/statemachine/statemachine.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/states.py` & `python_statemachine-2.1.1/statemachine/states.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/transition.py` & `python_statemachine-2.1.1/statemachine/transition.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/statemachine/transition_list.py` & `python_statemachine-2.1.1/statemachine/transition_list.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.0/setup.py` & `python_statemachine-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 package_data = \
 {'': ['*'],
  'statemachine': ['locale/en/LC_MESSAGES/*', 'locale/pt_BR/LC_MESSAGES/*']}
 
 setup_kwargs = {
     'name': 'python-statemachine',
-    'version': '2.1.0',
+    'version': '2.1.1',
     'description': 'Python Finite State Machines made easy.',
-    'long_description': '# Python StateMachine\n\n[![pypi](https://img.shields.io/pypi/v/python-statemachine.svg)](https://pypi.python.org/pypi/python-statemachine)\n[![downloads](https://img.shields.io/pypi/dm/python-statemachine.svg)](https://pypi.python.org/pypi/python-statemachine)\n[![build status](https://github.com/fgmacedo/python-statemachine/actions/workflows/python-package.yml/badge.svg?branch=develop)](https://github.com/fgmacedo/python-statemachine/actions/workflows/python-package.yml?query=branch%3Adevelop)\n[![Coverage report](https://codecov.io/gh/fgmacedo/python-statemachine/branch/develop/graph/badge.svg)](https://codecov.io/gh/fgmacedo/python-statemachine)\n[![Documentation Status](https://readthedocs.org/projects/python-statemachine/badge/?version=latest)](https://python-statemachine.readthedocs.io/en/latest/?badge=latest)\n[![GitHub commits since last release (main)](https://img.shields.io/github/commits-since/fgmacedo/python-statemachine/main/develop)](https://github.com/fgmacedo/python-statemachine/compare/main...develop)\n\n\nPython [finite-state machines](https://en.wikipedia.org/wiki/Finite-state_machine) made easy.\n\n\n* Free software: MIT license\n* Documentation: https://python-statemachine.readthedocs.io.\n\n\nWelcome to python-statemachine, an intuitive and powerful state machine framework designed for a\ngreat developer experience.\n\n🚀 With StateMachine, you can easily create complex, dynamic systems with clean, readable code.\n\n💡 Our framework makes it easy to understand and reason about the different states, events and\ntransitions in your system, so you can focus on building great products.\n\n🔒 python-statemachine also provides robust error handling and ensures that your system stays\nin a valid state at all times.\n\n\nA few reasons why you may consider using it:\n\n* 📈 python-statemachine is designed to help you build scalable,\n  maintainable systems that can handle any complexity.\n* 💪 You can easily create and manage multiple state machines within a single application.\n* 🚫 Prevents common mistakes and ensures that your system stays in a valid state at all times.\n\n\n## Getting started\n\n\nTo install Python State Machine, run this command in your terminal:\n\n    pip install python-statemachine\n\nTo generate diagrams from your machines, you\'ll also need `pydot` and `Graphviz`. You can\ninstall this library already with `pydot` dependency using the `extras` install option. See\nour docs for more details.\n\n    pip install python-statemachine[diagrams]\n\nDefine your state machine:\n\n```py\n>>> from statemachine import StateMachine, State\n\n>>> class TrafficLightMachine(StateMachine):\n...     "A traffic light machine"\n...     green = State(initial=True)\n...     yellow = State()\n...     red = State()\n...\n...     cycle = (\n...         green.to(yellow)\n...         | yellow.to(red)\n...         | red.to(green)\n...     )\n...\n...     def before_cycle(self, event: str, source: State, target: State, message: str = ""):\n...         message = ". " + message if message else ""\n...         return f"Running {event} from {source.id} to {target.id}{message}"\n...\n...     def on_enter_red(self):\n...         print("Don\'t move.")\n...\n...     def on_exit_red(self):\n...         print("Go ahead!")\n\n```\n\nYou can now create an instance:\n\n```py\n>>> sm = TrafficLightMachine()\n\n```\n\nThis state machine can be represented graphically as follows:\n\n```py\n>>> img_path = "docs/images/readme_trafficlightmachine.png"\n>>> sm._graph().write_png(img_path)\n\n```\n\n![](https://raw.githubusercontent.com/fgmacedo/python-statemachine/develop/docs/images/readme_trafficlightmachine.png)\n\n\nWhere on the `TrafficLightMachine`, we\'ve defined `green`, `yellow`, and `red` as states, and\none event called `cycle`, which is bound to the transitions from `green` to `yellow`, `yellow` to `red`,\nand `red` to `green`. We also have defined three callbacks by name convention, `before_cycle`, `on_enter_red`, and `on_exit_red`.\n\n\nThen start sending events to your new state machine:\n\n```py\n>>> sm.send("cycle")\n\'Running cycle from green to yellow\'\n\n```\n\nThat\'s it. This is all an external object needs to know about your state machine: How to send events.\nIdeally, all states, transitions, and actions should be kept internally and not checked externally to avoid unnecessary coupling.\n\nBut if your use case needs, you can inspect state machine properties, like the current state:\n\n```py\n>>> sm.current_state.id\n\'yellow\'\n\n```\n\nOr get a complete state representation for debugging purposes:\n\n```py\n>>> sm.current_state\nState(\'Yellow\', id=\'yellow\', value=\'yellow\', initial=False, final=False)\n\n```\n\nThe `State` instance can also be checked by equality:\n\n```py\n>>> sm.current_state == TrafficLightMachine.yellow\nTrue\n\n>>> sm.current_state == sm.yellow\nTrue\n\n```\n\nOr you can check if a state is active at any time:\n\n```py\n>>> sm.green.is_active\nFalse\n\n>>> sm.yellow.is_active\nTrue\n\n>>> sm.red.is_active\nFalse\n\n```\n\nEasily iterate over all states:\n\n```py\n>>> [s.id for s in sm.states]\n[\'green\', \'red\', \'yellow\']\n\n```\n\nOr over events:\n\n```py\n>>> [t.name for t in sm.events]\n[\'cycle\']\n\n```\n\nCall an event by its name:\n\n```py\n>>> sm.cycle()\nDon\'t move.\n\'Running cycle from yellow to red\'\n\n```\nOr send an event with the event name:\n\n```py\n>>> sm.send(\'cycle\')\nGo ahead!\n\'Running cycle from red to green\'\n\n>>> sm.green.is_active\nTrue\n\n```\n\nYou can pass arbitrary positional or keyword arguments to the event, and\nthey will be propagated to all actions and callbacks using something similar to dependency injection. In other words, the library will only inject the parameters declared on the\ncallback method.\n\nNote how `before_cycle` was declared:\n\n```py\ndef before_cycle(self, event: str, source: State, target: State, message: str = ""):\n    message = ". " + message if message else ""\n    return f"Running {event} from {source.id} to {target.id}{message}"\n```\n\nThe params `event`, `source`, `target` (and others) are available built-in to be used on any action.\nThe param `message` is user-defined, in our example we made it default empty so we can call `cycle` with\nor without a `message` parameter.\n\nIf we pass a `message` parameter, it will be used on the `before_cycle` action:\n\n```py\n>>> sm.send("cycle", message="Please, now slowdown.")\n\'Running cycle from green to yellow. Please, now slowdown.\'\n\n```\n\n\nBy default, events with transitions that cannot run from the current state or unknown events\nraise a `TransitionNotAllowed` exception:\n\n```py\n>>> sm.send("go")\nTraceback (most recent call last):\nstatemachine.exceptions.TransitionNotAllowed: Can\'t go when in Yellow.\n\n```\n\nKeeping the same state as expected:\n\n```py\n>>> sm.yellow.is_active\nTrue\n\n```\n\nA human-readable name is automatically derived from the `State.id`, which is used on the messages\nand in diagrams:\n\n```py\n>>> sm.current_state.name\n\'Yellow\'\n\n```\n\n## A more useful example\n\nA simple didactic state machine for controlling an `Order`:\n\n```py\n>>> class OrderControl(StateMachine):\n...     waiting_for_payment = State(initial=True)\n...     processing = State()\n...     shipping = State()\n...     completed = State(final=True)\n...\n...     add_to_order = waiting_for_payment.to(waiting_for_payment)\n...     receive_payment = (\n...         waiting_for_payment.to(processing, cond="payments_enough")\n...         | waiting_for_payment.to(waiting_for_payment, unless="payments_enough")\n...     )\n...     process_order = processing.to(shipping, cond="payment_received")\n...     ship_order = shipping.to(completed)\n...\n...     def __init__(self):\n...         self.order_total = 0\n...         self.payments = []\n...         self.payment_received = False\n...         super(OrderControl, self).__init__()\n...\n...     def payments_enough(self, amount):\n...         return sum(self.payments) + amount >= self.order_total\n...\n...     def before_add_to_order(self, amount):\n...         self.order_total += amount\n...         return self.order_total\n...\n...     def before_receive_payment(self, amount):\n...         self.payments.append(amount)\n...         return self.payments\n...\n...     def after_receive_payment(self):\n...         self.payment_received = True\n...\n...     def on_enter_waiting_for_payment(self):\n...         self.payment_received = False\n\n```\n\nYou can use this machine as follows.\n\n```py\n>>> control = OrderControl()\n\n>>> control.add_to_order(3)\n3\n\n>>> control.add_to_order(7)\n10\n\n>>> control.receive_payment(4)\n[4]\n\n>>> control.current_state.id\n\'waiting_for_payment\'\n\n>>> control.current_state.name\n\'Waiting for payment\'\n\n>>> control.process_order()\nTraceback (most recent call last):\n...\nstatemachine.exceptions.TransitionNotAllowed: Can\'t process_order when in Waiting for payment.\n\n>>> control.receive_payment(6)\n[4, 6]\n\n>>> control.current_state.id\n\'processing\'\n\n>>> control.process_order()\n\n>>> control.ship_order()\n\n>>> control.payment_received\nTrue\n\n>>> control.order_total\n10\n\n>>> control.payments\n[4, 6]\n\n>>> control.completed.is_active\nTrue\n\n```\n\nThere\'s a lot more to cover, please take a look at our docs:\nhttps://python-statemachine.readthedocs.io.\n\n\n## Contributing to the project\n\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine" data-icon="octicon-star" aria-label="Star fgmacedo/python-statemachine on GitHub">Star this project</a>\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/issues" data-icon="octicon-issue-opened" aria-label="Issue fgmacedo/python-statemachine on GitHub">Open an Issue</a>\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/fork" data-icon="octicon-repo-forked" aria-label="Fork fgmacedo/python-statemachine on GitHub">Fork</a>\n\n- If you found this project helpful, please consider giving it a star on GitHub.\n\n- **Contribute code**: If you would like to contribute code to this project, please submit a pull\nrequest. For more information on how to contribute, please see our [contributing.md]contributing.md) file.\n\n- **Report bugs**: If you find any bugs in this project, please report them by opening an issue\n  on our GitHub issue tracker.\n\n- **Suggest features**: If you have a great idea for a new feature, please let us know by opening\n  an issue on our GitHub issue tracker.\n\n- **Documentation**: Help improve this project\'s documentation by submitting pull requests.\n\n- **Promote the project**: Help spread the word about this project by sharing it on social media,\n  writing a blog post, or giving a talk about it. Tag me on Twitter\n  [@fgmacedo](https://twitter.com/fgmacedo) so I can share it too!\n',
+    'long_description': '# Python StateMachine\n\n[![pypi](https://img.shields.io/pypi/v/python-statemachine.svg)](https://pypi.python.org/pypi/python-statemachine)\n[![downloads](https://img.shields.io/pypi/dm/python-statemachine.svg)](https://pypi.python.org/pypi/python-statemachine)\n[![build status](https://github.com/fgmacedo/python-statemachine/actions/workflows/python-package.yml/badge.svg?branch=develop)](https://github.com/fgmacedo/python-statemachine/actions/workflows/python-package.yml?query=branch%3Adevelop)\n[![Coverage report](https://codecov.io/gh/fgmacedo/python-statemachine/branch/develop/graph/badge.svg)](https://codecov.io/gh/fgmacedo/python-statemachine)\n[![Documentation Status](https://readthedocs.org/projects/python-statemachine/badge/?version=latest)](https://python-statemachine.readthedocs.io/en/latest/?badge=latest)\n[![GitHub commits since last release (main)](https://img.shields.io/github/commits-since/fgmacedo/python-statemachine/main/develop)](https://github.com/fgmacedo/python-statemachine/compare/main...develop)\n\n\nPython [finite-state machines](https://en.wikipedia.org/wiki/Finite-state_machine) made easy.\n\n\n* Free software: MIT license\n* Documentation: https://python-statemachine.readthedocs.io.\n\n\nWelcome to python-statemachine, an intuitive and powerful state machine framework designed for a\ngreat developer experience.\n\n🚀 With StateMachine, you can easily create complex, dynamic systems with clean, readable code.\n\n💡 Our framework makes it easy to understand and reason about the different states, events and\ntransitions in your system, so you can focus on building great products.\n\n🔒 python-statemachine also provides robust error handling and ensures that your system stays\nin a valid state at all times.\n\n\nA few reasons why you may consider using it:\n\n* 📈 python-statemachine is designed to help you build scalable,\n  maintainable systems that can handle any complexity.\n* 💪 You can easily create and manage multiple state machines within a single application.\n* 🚫 Prevents common mistakes and ensures that your system stays in a valid state at all times.\n\n\n## Getting started\n\n\nTo install Python State Machine, run this command in your terminal:\n\n    pip install python-statemachine\n\nTo generate diagrams from your machines, you\'ll also need `pydot` and `Graphviz`. You can\ninstall this library already with `pydot` dependency using the `extras` install option. See\nour docs for more details.\n\n    pip install python-statemachine[diagrams]\n\nDefine your state machine:\n\n```py\n>>> from statemachine import StateMachine, State\n\n>>> class TrafficLightMachine(StateMachine):\n...     "A traffic light machine"\n...     green = State(initial=True)\n...     yellow = State()\n...     red = State()\n...\n...     cycle = (\n...         green.to(yellow)\n...         | yellow.to(red)\n...         | red.to(green)\n...     )\n...\n...     def before_cycle(self, event: str, source: State, target: State, message: str = ""):\n...         message = ". " + message if message else ""\n...         return f"Running {event} from {source.id} to {target.id}{message}"\n...\n...     def on_enter_red(self):\n...         print("Don\'t move.")\n...\n...     def on_exit_red(self):\n...         print("Go ahead!")\n\n```\n\nYou can now create an instance:\n\n```py\n>>> sm = TrafficLightMachine()\n\n```\n\nThis state machine can be represented graphically as follows:\n\n```py\n>>> img_path = "docs/images/readme_trafficlightmachine.png"\n>>> sm._graph().write_png(img_path)\n\n```\n\n![](https://raw.githubusercontent.com/fgmacedo/python-statemachine/develop/docs/images/readme_trafficlightmachine.png)\n\n\nWhere on the `TrafficLightMachine`, we\'ve defined `green`, `yellow`, and `red` as states, and\none event called `cycle`, which is bound to the transitions from `green` to `yellow`, `yellow` to `red`,\nand `red` to `green`. We also have defined three callbacks by name convention, `before_cycle`, `on_enter_red`, and `on_exit_red`.\n\n\nThen start sending events to your new state machine:\n\n```py\n>>> sm.send("cycle")\n\'Running cycle from green to yellow\'\n\n```\n\nThat\'s it. This is all an external object needs to know about your state machine: How to send events.\nIdeally, all states, transitions, and actions should be kept internally and not checked externally to avoid unnecessary coupling.\n\nBut if your use case needs, you can inspect state machine properties, like the current state:\n\n```py\n>>> sm.current_state.id\n\'yellow\'\n\n```\n\nOr get a complete state representation for debugging purposes:\n\n```py\n>>> sm.current_state\nState(\'Yellow\', id=\'yellow\', value=\'yellow\', initial=False, final=False)\n\n```\n\nThe `State` instance can also be checked by equality:\n\n```py\n>>> sm.current_state == TrafficLightMachine.yellow\nTrue\n\n>>> sm.current_state == sm.yellow\nTrue\n\n```\n\nOr you can check if a state is active at any time:\n\n```py\n>>> sm.green.is_active\nFalse\n\n>>> sm.yellow.is_active\nTrue\n\n>>> sm.red.is_active\nFalse\n\n```\n\nEasily iterate over all states:\n\n```py\n>>> [s.id for s in sm.states]\n[\'green\', \'red\', \'yellow\']\n\n```\n\nOr over events:\n\n```py\n>>> [t.name for t in sm.events]\n[\'cycle\']\n\n```\n\nCall an event by its name:\n\n```py\n>>> sm.cycle()\nDon\'t move.\n\'Running cycle from yellow to red\'\n\n```\nOr send an event with the event name:\n\n```py\n>>> sm.send(\'cycle\')\nGo ahead!\n\'Running cycle from red to green\'\n\n>>> sm.green.is_active\nTrue\n\n```\n\nYou can pass arbitrary positional or keyword arguments to the event, and\nthey will be propagated to all actions and callbacks using something similar to dependency injection. In other words, the library will only inject the parameters declared on the\ncallback method.\n\nNote how `before_cycle` was declared:\n\n```py\ndef before_cycle(self, event: str, source: State, target: State, message: str = ""):\n    message = ". " + message if message else ""\n    return f"Running {event} from {source.id} to {target.id}{message}"\n```\n\nThe params `event`, `source`, `target` (and others) are available built-in to be used on any action.\nThe param `message` is user-defined, in our example we made it default empty so we can call `cycle` with\nor without a `message` parameter.\n\nIf we pass a `message` parameter, it will be used on the `before_cycle` action:\n\n```py\n>>> sm.send("cycle", message="Please, now slowdown.")\n\'Running cycle from green to yellow. Please, now slowdown.\'\n\n```\n\n\nBy default, events with transitions that cannot run from the current state or unknown events\nraise a `TransitionNotAllowed` exception:\n\n```py\n>>> sm.send("go")\nTraceback (most recent call last):\nstatemachine.exceptions.TransitionNotAllowed: Can\'t go when in Yellow.\n\n```\n\nKeeping the same state as expected:\n\n```py\n>>> sm.yellow.is_active\nTrue\n\n```\n\nA human-readable name is automatically derived from the `State.id`, which is used on the messages\nand in diagrams:\n\n```py\n>>> sm.current_state.name\n\'Yellow\'\n\n```\n\n## A more useful example\n\nA simple didactic state machine for controlling an `Order`:\n\n```py\n>>> class OrderControl(StateMachine):\n...     waiting_for_payment = State(initial=True)\n...     processing = State()\n...     shipping = State()\n...     completed = State(final=True)\n...\n...     add_to_order = waiting_for_payment.to(waiting_for_payment)\n...     receive_payment = (\n...         waiting_for_payment.to(processing, cond="payments_enough")\n...         | waiting_for_payment.to(waiting_for_payment, unless="payments_enough")\n...     )\n...     process_order = processing.to(shipping, cond="payment_received")\n...     ship_order = shipping.to(completed)\n...\n...     def __init__(self):\n...         self.order_total = 0\n...         self.payments = []\n...         self.payment_received = False\n...         super(OrderControl, self).__init__()\n...\n...     def payments_enough(self, amount):\n...         return sum(self.payments) + amount >= self.order_total\n...\n...     def before_add_to_order(self, amount):\n...         self.order_total += amount\n...         return self.order_total\n...\n...     def before_receive_payment(self, amount):\n...         self.payments.append(amount)\n...         return self.payments\n...\n...     def after_receive_payment(self):\n...         self.payment_received = True\n...\n...     def on_enter_waiting_for_payment(self):\n...         self.payment_received = False\n\n```\n\nYou can use this machine as follows.\n\n```py\n>>> control = OrderControl()\n\n>>> control.add_to_order(3)\n3\n\n>>> control.add_to_order(7)\n10\n\n>>> control.receive_payment(4)\n[4]\n\n>>> control.current_state.id\n\'waiting_for_payment\'\n\n>>> control.current_state.name\n\'Waiting for payment\'\n\n>>> control.process_order()\nTraceback (most recent call last):\n...\nstatemachine.exceptions.TransitionNotAllowed: Can\'t process_order when in Waiting for payment.\n\n>>> control.receive_payment(6)\n[4, 6]\n\n>>> control.current_state.id\n\'processing\'\n\n>>> control.process_order()\n\n>>> control.ship_order()\n\n>>> control.payment_received\nTrue\n\n>>> control.order_total\n10\n\n>>> control.payments\n[4, 6]\n\n>>> control.completed.is_active\nTrue\n\n```\n\nThere\'s a lot more to cover, please take a look at our docs:\nhttps://python-statemachine.readthedocs.io.\n\n\n## Contributing to the project\n\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine" data-icon="octicon-star" aria-label="Star fgmacedo/python-statemachine on GitHub">Star this project</a>\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/issues" data-icon="octicon-issue-opened" aria-label="Issue fgmacedo/python-statemachine on GitHub">Open an Issue</a>\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/fork" data-icon="octicon-repo-forked" aria-label="Fork fgmacedo/python-statemachine on GitHub">Fork</a>\n\n- If you found this project helpful, please consider giving it a star on GitHub.\n\n- **Contribute code**: If you would like to contribute code to this project, please submit a pull\nrequest. For more information on how to contribute, please see our [contributing.md](contributing.md) file.\n\n- **Report bugs**: If you find any bugs in this project, please report them by opening an issue\n  on our GitHub issue tracker.\n\n- **Suggest features**: If you have a great idea for a new feature, please let us know by opening\n  an issue on our GitHub issue tracker.\n\n- **Documentation**: Help improve this project\'s documentation by submitting pull requests.\n\n- **Promote the project**: Help spread the word about this project by sharing it on social media,\n  writing a blog post, or giving a talk about it. Tag me on Twitter\n  [@fgmacedo](https://twitter.com/fgmacedo) so I can share it too!\n',
     'author': 'Fernando Macedo',
     'author_email': 'fgmacedo@gmail.com',
     'maintainer': 'Fernando Macedo',
     'maintainer_email': 'fgmacedo@gmail.com',
     'url': 'https://github.com/fgmacedo/python-statemachine',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `python_statemachine-2.1.0/PKG-INFO` & `python_statemachine-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-statemachine
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python Finite State Machines made easy.
 Home-page: https://github.com/fgmacedo/python-statemachine
 License: MIT
 Author: Fernando Macedo
 Author-email: fgmacedo@gmail.com
 Maintainer: Fernando Macedo
 Maintainer-email: fgmacedo@gmail.com
@@ -371,15 +371,15 @@
 * <a class="github-button" href="https://github.com/fgmacedo/python-statemachine" data-icon="octicon-star" aria-label="Star fgmacedo/python-statemachine on GitHub">Star this project</a>
 * <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/issues" data-icon="octicon-issue-opened" aria-label="Issue fgmacedo/python-statemachine on GitHub">Open an Issue</a>
 * <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/fork" data-icon="octicon-repo-forked" aria-label="Fork fgmacedo/python-statemachine on GitHub">Fork</a>
 
 - If you found this project helpful, please consider giving it a star on GitHub.
 
 - **Contribute code**: If you would like to contribute code to this project, please submit a pull
-request. For more information on how to contribute, please see our [contributing.md]contributing.md) file.
+request. For more information on how to contribute, please see our [contributing.md](contributing.md) file.
 
 - **Report bugs**: If you find any bugs in this project, please report them by opening an issue
   on our GitHub issue tracker.
 
 - **Suggest features**: If you have a great idea for a new feature, please let us know by opening
   an issue on our GitHub issue tracker.
```

