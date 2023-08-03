# Comparing `tmp/cotea-1.3.12.tar.gz` & `tmp/cotea-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cotea-1.3.12.tar", last modified: Thu Aug  3 16:26:09 2023, max compression
+gzip compressed data, was "cotea-1.3.9.tar", last modified: Tue Nov 29 11:02:09 2022, max compression
```

## Comparing `cotea-1.3.12.tar` & `cotea-1.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-08-03 16:26:09.227894 cotea-1.3.12/
--rw-rw-r--   0 david     (1000) david     (1000)    11357 2023-08-03 13:43:07.000000 cotea-1.3.12/LICENSE.md
--rw-rw-r--   0 david     (1000) david     (1000)     2881 2023-08-03 16:26:09.227894 cotea-1.3.12/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     2347 2023-08-03 13:43:07.000000 cotea-1.3.12/README.md
--rw-rw-r--   0 david     (1000) david     (1000)       85 2023-08-03 13:43:07.000000 cotea-1.3.12/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)      656 2023-08-03 16:26:09.227894 cotea-1.3.12/setup.cfg
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-08-03 16:26:09.227894 cotea-1.3.12/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-08-03 16:26:09.227894 cotea-1.3.12/src/cotea/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1551 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/ansible_execution_sync.py
--rw-rw-r--   0 david     (1000) david     (1000)     1754 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/ansible_execution_tree.py
--rw-rw-r--   0 david     (1000) david     (1000)     1425 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/arguments_maker.py
--rw-rw-r--   0 david     (1000) david     (1000)     4894 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/debug_utils.py
--rw-rw-r--   0 david     (1000) david     (1000)     1505 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/progress_bar.py
--rw-rw-r--   0 david     (1000) david     (1000)    15605 2023-08-03 14:03:12.000000 cotea-1.3.12/src/cotea/runner.py
--rw-rw-r--   0 david     (1000) david     (1000)     2353 2023-08-03 14:06:24.000000 cotea-1.3.12/src/cotea/task_result.py
--rw-rw-r--   0 david     (1000) david     (1000)      636 2023-08-03 13:56:23.000000 cotea-1.3.12/src/cotea/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-08-03 16:26:09.227894 cotea-1.3.12/src/cotea/wrappers/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/wrappers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      208 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/wrappers/ansi_breakpoint.py
--rw-rw-r--   0 david     (1000) david     (1000)     7010 2023-08-03 16:15:52.000000 cotea-1.3.12/src/cotea/wrappers/get_next_task_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)     2923 2023-08-03 14:12:58.000000 cotea-1.3.12/src/cotea/wrappers/iterator_add_task_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)      818 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/wrappers/pbcli_run_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)      643 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/wrappers/play_prereqs_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)     3654 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/wrappers/playbook_executor_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)     1894 2023-08-03 14:11:56.000000 cotea-1.3.12/src/cotea/wrappers/strategy_run_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)     1611 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/wrappers/update_active_conn_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)      368 2023-08-03 13:43:07.000000 cotea-1.3.12/src/cotea/wrappers/wrapper_base.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-08-03 16:26:09.227894 cotea-1.3.12/src/cotea.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     2881 2023-08-03 16:26:09.000000 cotea-1.3.12/src/cotea.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      834 2023-08-03 16:26:09.000000 cotea-1.3.12/src/cotea.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-08-03 16:26:09.000000 cotea-1.3.12/src/cotea.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        6 2023-08-03 16:26:09.000000 cotea-1.3.12/src/cotea.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-11-29 11:02:09.022590 cotea-1.3.9/
+-rw-rw-r--   0 david     (1000) david     (1000)    11357 2022-06-27 18:13:28.000000 cotea-1.3.9/LICENSE.md
+-rw-rw-r--   0 david     (1000) david     (1000)     2880 2022-11-29 11:02:09.022590 cotea-1.3.9/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     2347 2022-06-27 18:13:28.000000 cotea-1.3.9/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)       85 2022-06-27 18:13:28.000000 cotea-1.3.9/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)      655 2022-11-29 11:02:09.022590 cotea-1.3.9/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-11-29 11:02:09.022590 cotea-1.3.9/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-11-29 11:02:09.022590 cotea-1.3.9/src/cotea/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1551 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/ansible_execution_sync.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1754 2022-08-11 17:04:27.000000 cotea-1.3.9/src/cotea/ansible_execution_tree.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1425 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/arguments_maker.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4568 2022-09-19 14:32:15.000000 cotea-1.3.9/src/cotea/debug_utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1505 2022-08-11 17:05:12.000000 cotea-1.3.9/src/cotea/progress_bar.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15940 2022-11-28 13:59:45.000000 cotea-1.3.9/src/cotea/runner.py
+-rw-rw-r--   0 david     (1000) david     (1000)      991 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/task_result.py
+-rw-rw-r--   0 david     (1000) david     (1000)      327 2022-08-11 17:05:50.000000 cotea-1.3.9/src/cotea/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-11-29 11:02:09.022590 cotea-1.3.9/src/cotea/wrappers/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      208 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/ansi_breakpoint.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6488 2022-11-28 13:59:01.000000 cotea-1.3.9/src/cotea/wrappers/get_next_task_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2921 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/iterator_add_task_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)      818 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/pbcli_run_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)      643 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/play_prereqs_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3654 2022-08-11 17:03:18.000000 cotea-1.3.9/src/cotea/wrappers/playbook_executor_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1584 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/strategy_run_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1611 2022-07-06 13:30:14.000000 cotea-1.3.9/src/cotea/wrappers/update_active_conn_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)      368 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/wrapper_base.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-11-29 11:02:09.022590 cotea-1.3.9/src/cotea.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     2880 2022-11-29 11:02:09.000000 cotea-1.3.9/src/cotea.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      834 2022-11-29 11:02:09.000000 cotea-1.3.9/src/cotea.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2022-11-29 11:02:09.000000 cotea-1.3.9/src/cotea.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        6 2022-11-29 11:02:09.000000 cotea-1.3.9/src/cotea.egg-info/top_level.txt
```

### Comparing `cotea-1.3.12/LICENSE.md` & `cotea-1.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cotea-1.3.12/PKG-INFO` & `cotea-1.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cotea
-Version: 1.3.12
+Version: 1.3.9
 Summary: Tool that provides Python API to run Ansible programmatically.
 Home-page: https://github.com/ispras/cotea
 Author: David Badalyan
 Author-email: dbadalyan@ispras.ru
 Project-URL: Bug Tracker, https://github.com/ispras/cotea/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cotea-1.3.12/README.md` & `cotea-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `cotea-1.3.12/setup.cfg` & `cotea-1.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cotea
-version = 1.3.12
+version = 1.3.9
 author = David Badalyan
 author_email = dbadalyan@ispras.ru
 description = Tool that provides Python API to run Ansible programmatically.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ispras/cotea
 project_urls =
```

### Comparing `cotea-1.3.12/src/cotea/ansible_execution_sync.py` & `cotea-1.3.9/src/cotea/ansible_execution_sync.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.12/src/cotea/ansible_execution_tree.py` & `cotea-1.3.9/src/cotea/ansible_execution_tree.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.12/src/cotea/arguments_maker.py` & `cotea-1.3.9/src/cotea/arguments_maker.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.12/src/cotea/debug_utils.py` & `cotea-1.3.9/src/cotea/debug_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     help_msg += "'p' - print Progress bar\n"
     help_msg += "'h'/'help' - print this msg\n"
     help_msg += "\nAction commands:\n"
     help_msg += "'re' - RErun of the failed task\n"
     help_msg += "'v' - add new Variable as extra var\n"
     help_msg += "'c' - Continue ansible execution (go to the next task)\n"
     help_msg += "'nt' - add New Task\n"
-    help_msg += "'w' - Watch ansible variable value\n"
     #help_msg += "'f' - Finish ansible execution\n"
 
     print(help_msg)
 
 
 def pretty_print_task(task: Task):
     pretty_print = "Name: {}\nAction: {}\nArgs: {}\nbecome: {}\n".format(task.name,
@@ -102,22 +101,13 @@
 
             if not add_ok:
                 print("\nThe adding process was failed with the error:\n", err_msg)
             else:
                 print("\nNew task was added! It will run on every host of current inventory.")
                 print("Press 'c' after this, not 're'. This will run new task and the failed one after it.\n")
                 r.progress_bar.add_to_total_task_count(1)
-        
-        elif command == "w":
-            print("Enter var name: ", end="")
-            
-            var_name = input()
-            value = r.get_variable(var_name)
-            msg = "{} var value:\n{}".format(var_name, value)
-            
-            print(msg)
 
         elif command == "help" or command == "h":
             print_help_msg()
 
         else:
             print("Enter commands correctly! 'help' or just 'h' will help you\n")
```

### Comparing `cotea-1.3.12/src/cotea/progress_bar.py` & `cotea-1.3.9/src/cotea/progress_bar.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.12/src/cotea/runner.py` & `cotea-1.3.9/src/cotea/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import threading
 
-import cotea.utils as cotea_utils
+from cotea.utils import remove_modules_from_imported
 
 # during the imports ansible global objects are created
 # that affects to the further work
-cotea_utils.remove_modules_from_imported(module_name_like="ansible", not_to_delete="ansible_runner")
-cotea_utils.remove_modules_from_imported(module_name_like="logging")
+remove_modules_from_imported(module_name_like="ansible", not_to_delete="ansible_runner")
+remove_modules_from_imported(module_name_like="logging")
 
 from ansible.cli import CLI
 from ansible.plugins.strategy.linear import StrategyModule
 from ansible.plugins.strategy import StrategyBase
 from ansible.cli.playbook import PlaybookCLI
 from ansible.parsing.yaml.objects import AnsibleUnicode
 from ansible.executor.playbook_executor import PlaybookExecutor
@@ -29,14 +29,15 @@
 from cotea.wrappers.iterator_add_task_wrapper import iterator_add_task_wrapper
 from cotea.progress_bar import ansible_progress_bar
 from cotea.ansible_execution_tree import AnsibleExecTree
 
 import logging
 
 
+
 class runner:
     def __init__(self, pb_path, arg_maker, debug_mod=None, show_progress_bar=False):
         logging_lvl = logging.INFO
         if debug_mod:
             logging_lvl= logging.DEBUG
         
         self.show_progress_bar = show_progress_bar
@@ -93,37 +94,35 @@
                                                               self.breakpoint_labeles["after_task"])
         StrategyBase.update_active_connections = self.update_conn_wrapper
 
         self.play_prereqs_wrp = play_prereqs_wrapper(CLI._play_prereqs,
                                                       self.sync_obj, wrp_lgr)
         CLI._play_prereqs = self.play_prereqs_wrp
 
-        if self.show_progress_bar:
-            self.playbook_executor_wrp = play_executor_wrapper(PlaybookExecutor.__init__,
-                                                            self.sync_obj, wrp_lgr,
-                                                            self.execution_tree,
-                                                            self.progress_bar)
-            PlaybookExecutor.__init__ = self.playbook_executor_wrp
+        self.playbook_executor_wrp = play_executor_wrapper(PlaybookExecutor.__init__,
+                                                           self.sync_obj, wrp_lgr,
+                                                           self.execution_tree,
+                                                           self.progress_bar)
+        PlaybookExecutor.__init__ = self.playbook_executor_wrp
 
         self.iterator_add_task_wrp = iterator_add_task_wrapper(PlayIterator.add_tasks,
                                                                   self.sync_obj, wrp_lgr,
                                                                   self.execution_tree,
                                                                   self.progress_bar)
         PlayIterator.add_tasks = self.iterator_add_task_wrp
     
 
     def _set_wrappers_back(self):
         PlaybookCLI.run = self.pbcli_run_wrp.func
         StrategyModule.run = self.play_wrp.func
         StrategyModule._get_next_task_lockstep = self.task_wrp.func
         StrategyBase.update_active_connections = self.update_conn_wrapper.func
         CLI._play_prereqs = self.play_prereqs_wrp.func
+        PlaybookExecutor.__init__ = self.playbook_executor_wrp.func
         PlayIterator.add_tasks = self.iterator_add_task_wrp.func
-        if self.show_progress_bar:
-            PlaybookExecutor.__init__ = self.playbook_executor_wrp.func
     
 
     def _start_ansible(self):
         args = self.arg_maker.args
         args.insert(0, "/usr/local/bin/ansible-playbook")
         args.insert(1, self.pb_path)
 
@@ -178,127 +177,111 @@
         self.logger.debug("run_next_task: %s", current_bp_label)
 
         if current_bp_label != self.breakpoint_labeles["after_task"]:
             self.logger.debug("run_next_task() has come not in to the 'after_task'")
         
         for task_result_ansible_obj in self.update_conn_wrapper.current_results:
             res.append(TaskResult(task_result_ansible_obj))
-
-        self.task_wrp.set_next_to_prev()
-
+        
         return res
     
 
     def rerun_last_task(self):
         self.task_wrp.rerun_last_task = True
     
 
     # returns True and empty string if success
     #         False and error msg otherwise
-    def add_new_task(self, new_task_str, is_dict=False):
-        prev_task = self.get_prev_task()
-        curr_block = None
-
-        has_attrs, error_msg = cotea_utils.obj_has_attrs(prev_task, ["_parent"])
-        if not has_attrs:
-            return False, error_msg
-        
-        curr_block = prev_task._parent
-        block_attrs = ["_loader", "_play", "_role", "_variable_manager", "_use_handlers"]
-        has_attrs, error_msg = cotea_utils.obj_has_attrs(curr_block, block_attrs)
-        if not has_attrs:
-            return False, error_msg
-
-        loader = curr_block._loader
+    def add_new_task(self, new_task_str):
+        loader = self.playbook_executor_wrp.loader
 
         ds = None
-        if not is_dict:
-            try:
-                ds = loader.load(new_task_str)
-            except Exception as e:
-                error_msg = "Exception during loader.load call, is_dict is {} "
-                error_msg += "(from str to python ds): {}"
-                return False, error_msg.format(is_dict, str(e))
+        try:
+            ds = loader.load(new_task_str)
+        except Exception as e:
+            return False, "Exception during loader.load call\
+                (from str to python ds): {}".format(str(e))
+        
+        if hasattr(ds, "__len__"):
+            if len(ds) != 1:
+                return False, "You must add 1 new task. Instead you add: {}".format(str(ds))
         else:
-            try:
-                new_task_str_dict = json.loads(new_task_str)
-            except Exception as e:
-                error_msg = "Exception during json.loads call, is_dict is {} "
-                error_msg += "(from str-aka-dict to python ds): {}"
-                return False, error_msg.format(is_dict, str(e))
-            ds = [new_task_str_dict]
-        
-        #print("DS:\n", ds)
-        
-        has_attrs, _ = cotea_utils.obj_has_attrs(ds, ["__len__"])
-        if not has_attrs:
-            error_msg = "Python repr of the input string should have "
-            error_msg += "__len__ attr. Maybe something wrong with input: {}\n"
-            error_msg += "Python repr without __len__ attr: {}"
-            return False, error_msg.format(new_task_str, str(ds))
-            
-        if len(ds) != 1:
-            error_msg = "You must add 1 new task. Instead you add: {}"
-            return False, error_msg.format(str(ds))
-
-        curr_play = curr_block._play
-        #curr_role = curr_block._role
-        variable_manager = curr_block._variable_manager
-        use_handlers=curr_block._use_handlers
+            return False, "Python repr of the input string should have\
+                        __len__ attr. Maybe something wrong with input: {}\n\
+                        Python repr without __len__ attr: {}".format(new_task_str, str(ds))
 
-        try:
-            new_ansible_task = load_list_of_tasks(
-                ds=ds,
-                play=curr_play,
-                block=curr_block,
-                #role=curr_role,
-                variable_manager=variable_manager,
-                loader=loader,
-                use_handlers=use_handlers,
-            )
+        current_play = self.play_wrp.iterator._play
+        variable_manager = self.playbook_executor_wrp.variable_manager
 
+        try:
+            new_ansible_task = load_list_of_tasks(ds=ds, play=current_play, \
+                variable_manager=variable_manager, loader=loader)
         except Exception as e:
-            error_msg = "Exception during load_list_of_tasks call "
-            error_msg += "(creats Ansible.Task objects): {}"
-            return False, error_msg.format(str(e))
+            return False, "Exception during load_list_of_tasks call\
+                (creats Ansible.Task objects): {}".format(str(e))
         
-        has_attrs, _ = cotea_utils.obj_has_attrs(new_ansible_task, ["__len__"])
-        if not has_attrs:
-            error_msg = "Python repr of the input string should have "
-            error_msg += "__len__ attr. Maybe something wrong with input: {}\n"
-            error_msg += "Python repr without __len__ attr: {}"
-            return False, error_msg.format(new_task_str, str(ds))
-
-        new_tasks_count = len(new_ansible_task)
-        if new_tasks_count != 1:
-            error_msg = "The input '{}' has been interpreted into {} tasks "
-            error_msg += "instead of 1. Interpretation result: {}"
-            return False, error_msg.format(new_task_str, new_tasks_count, str(ds))
+        if hasattr(new_ansible_task, "__len__"):
+            new_tasks_count = len(new_ansible_task)
+            if new_tasks_count != 1:
+                return False, "The input '{}' has been interpreted into {} tasks\
+                               instead of 1. Interpretation \
+                                result: {}".format(new_task_str, new_tasks_count, str(ds))
+        else:
+            return False, "Python repr of the input string should have\
+                        __len__ attr. Maybe something wrong with input: {}\n\
+                        Python repr without __len__ attr: {}".format(new_task_str, str(ds))
+        
+        # new_task doesn't have parent and parent_type attrs
+        # we will take them from previous task
+        new_task = new_ansible_task[0]
+        ser_new_task = new_task.serialize()
         
-        #self.task_wrp.new_task_to_add = True
-        self.task_wrp.new_task = new_ansible_task[0]
+        prev_task = self.get_prev_task()
+        ser_prev_task = prev_task.serialize()
+
+        if "parent" not in ser_prev_task:
+            return False, "Previous task doesn't have 'parent' attr but should.\n\
+                Previous task serialize view: {}".format(str(ser_prev_task))
+
+        if hasattr(ser_prev_task["parent"], "copy"):
+            ser_new_task["parent"] = ser_prev_task["parent"].copy()
+        else:
+            return False, "Previous task 'parent' attr doesn't have 'copy' attr but should\
+                 because it should be dict. 'parent' attr: {}".format(str(ser_prev_task))
+
+        if "parent_type" not in ser_prev_task:
+            return False, "Previous task doesn't have 'parent_type' attr but should.\n\
+                Previous task serialize view: {}".format(str(ser_prev_task))
         
-        adding_res, error_msg = self.task_wrp.add_tasks(new_ansible_task)
+        ser_new_task["parent_type"] = ser_prev_task["parent_type"]
 
-        return adding_res, error_msg
+        final_new_task = Task()
+        final_new_task.deserialize(ser_new_task)
 
-    
-    def get_new_added_task(self):
-        return self.task_wrp.new_task
+        # needs to be processed properly
+        try:
+            final_new_task._parent._play = prev_task._parent._play.copy()
+        except:
+            final_new_task._parent._play = current_play.copy() 
+        
+        self.task_wrp.new_task_to_add = True
+        self.task_wrp.new_task = final_new_task
+
+        return True, ""
 
     
     def ignore_errors_of_next_task(self):
         self.task_wrp.next_task_ignore_errors = True
 
     def get_already_ignore_failed(self):
-        return self.task_wrp.should_ignored_errors_uuids
+        return self.task_wrp.already_ignore_failed
 
 
     def get_already_ignore_unrch(self):
-        return self.task_wrp.should_ignored_unrch_uuids
+        return self.task_wrp.already_ignore_unrch
 
 
     def finish_ansible(self):
         while self.sync_obj.curr_breakpoint_label != self.breakpoint_labeles["after_playbook"]:
             self.sync_obj.continue_ansible_with_stop()
         
         self.sync_obj.continue_ansible()
@@ -416,11 +399,32 @@
     
 
     def add_var_as_extra_var(self, new_var_name, value):
         variable_manager = self.play_wrp.variable_manager
 
         ansible_way_var = AnsibleUnicode(new_var_name)
         variable_manager._extra_vars[ansible_way_var] = value
+   
+    
+    def _getIP(self):
+        var_name = "openstack_servers"
+        host_name = "localhost"
+        ip1_field_name = "interface_ip"
+        ip2_field_name = "private_v4"
 
+        res = ""
+        ostack_var = self.get_variable(var_name)
+
+        try:
+            if ip1_field_name in ostack_var[host_name][0]:
+                res = str(ostack_var[host_name][0][ip1_field_name])
+            elif ip2_field_name in ostack_var[host_name][0]:
+                res = str(ostack_var[host_name][0][ip2_field_name])
+        except Exception as e:
+            self.logger.info("During runner._getIP() call error was occured. We skipped it.")
+            self.logger.info("Error is:\n%s", e)
+
+        self.logger.debug("get_ip res = %s", res)
+        self.logger.debug(type(res))
+
+        return res
 
-    def get_stats(self):
-        return self.play_wrp.custom_stats
```

### Comparing `cotea-1.3.12/src/cotea/wrappers/iterator_add_task_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/iterator_add_task_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,9 +78,9 @@
             
             elif isinstance(task_or_block, Block):
                 _get_all_block_tasks_rec(new_tasks, task_or_block)
             
             else:
                 print("in 'block' list object is not Task/Block type:", type(task_or_block), task_or_block)
 
-    #else:
-    #    print("block has no 'block' attr:", block)
+    else:
+        print("block has no 'block' attr:", block)
```

### Comparing `cotea-1.3.12/src/cotea/wrappers/pbcli_run_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/pbcli_run_wrapper.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.12/src/cotea/wrappers/play_prereqs_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/play_prereqs_wrapper.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.12/src/cotea/wrappers/playbook_executor_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/playbook_executor_wrapper.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.12/src/cotea/wrappers/strategy_run_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/strategy_run_wrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,46 +12,37 @@
         self.current_play_name = None
         self.iterator = None
         self.play_context = None
         self.variable_manager = None
         self.hosts = None
         self.hosts_all = None
         self.was_error = False
-        self.strategy_obj = None
-        self.stats = None
 
 
     def __call__(self, real_obj, iterator, play_context):
         self.logger.debug("play run")
 
         self.was_error = False
         self.iterator = iterator
         self.play_context = play_context
         self.variable_manager = real_obj._variable_manager
         self.hosts = real_obj._hosts_cache
         self.hosts_all = real_obj._hosts_cache_all
-        self.custom_stats = None
-        
-        if hasattr(real_obj._tqm, "_stats"):
-            if hasattr(real_obj._tqm._stats, "custom"):
-                self.custom_stats = real_obj._tqm._stats.custom
-
-        self.strategy_obj = real_obj
         try:
             self.current_play_name = iterator._play.get_name()
         except:
             pass
         
         self.before_play_bp.stop()
 
         result = self.func(real_obj, iterator, play_context)
 
-        # self.iterator = None
-        # self.play_context = None
-        # self.current_play_name = None
+        self.iterator = None
+        self.play_context = None
+        self.current_play_name = None
         
         self.logger.debug("play end")
         
         self.after_play_bp.stop()
         if result != real_obj._tqm.RUN_OK:
             self.was_error = True
```

### Comparing `cotea-1.3.12/src/cotea/wrappers/update_active_conn_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/update_active_conn_wrapper.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.12/src/cotea.egg-info/PKG-INFO` & `cotea-1.3.9/src/cotea.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cotea
-Version: 1.3.12
+Version: 1.3.9
 Summary: Tool that provides Python API to run Ansible programmatically.
 Home-page: https://github.com/ispras/cotea
 Author: David Badalyan
 Author-email: dbadalyan@ispras.ru
 Project-URL: Bug Tracker, https://github.com/ispras/cotea/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cotea-1.3.12/src/cotea.egg-info/SOURCES.txt` & `cotea-1.3.9/src/cotea.egg-info/SOURCES.txt`

 * *Files identical despite different names*

