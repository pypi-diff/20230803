# Comparing `tmp/pinjected-0.1.110.tar.gz` & `tmp/pinjected-0.1.111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.1.110.tar", max compression
+gzip compressed data, was "pinjected-0.1.111.tar", max compression
```

## Comparing `pinjected-0.1.110.tar` & `pinjected-0.1.111.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.1.110/LICENSE
--rw-r--r--   0        0        0      407 2023-08-01 10:55:32.734086 pinjected-0.1.110/pinjected/__init__.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.1.110/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.1.110/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     2522 2023-08-01 10:55:32.770639 pinjected-0.1.110/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      635 2023-08-01 10:55:32.714575 pinjected-0.1.110/pinjected/di/applicative.py
--rw-r--r--   0        0        0     6641 2023-08-01 10:58:43.087334 pinjected-0.1.110/pinjected/di/ast.py
--rw-r--r--   0        0        0     1145 2023-08-01 10:55:32.707779 pinjected-0.1.110/pinjected/di/bindings.py
--rw-r--r--   0        0        0     1009 2023-08-01 10:55:32.748920 pinjected-0.1.110/pinjected/di/design.py
--rw-r--r--   0        0        0     1918 2023-08-01 10:55:32.712483 pinjected-0.1.110/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.1.110/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    21758 2023-08-01 10:55:32.754770 pinjected-0.1.110/pinjected/di/graph.py
--rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinjected-0.1.110/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    32965 2023-08-01 10:58:43.085630 pinjected-0.1.110/pinjected/di/injected.py
--rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinjected-0.1.110/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0     2931 2023-08-01 10:55:32.737082 pinjected-0.1.110/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinjected-0.1.110/pinjected/di/permissioned/__init__.py
--rw-r--r--   0        0        0     7805 2023-08-01 10:55:32.728581 pinjected-0.1.110/pinjected/di/permissioned/blueprint.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.1.110/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.1.110/pinjected/di/provider.py
--rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinjected-0.1.110/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.1.110/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.1.110/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6169 2023-08-01 10:55:32.723083 pinjected-0.1.110/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.1.110/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      980 2023-08-01 10:55:32.724965 pinjected-0.1.110/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1500 2023-08-01 10:55:32.752600 pinjected-0.1.110/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2239 2023-08-01 10:55:32.766231 pinjected-0.1.110/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      690 2023-08-01 10:55:32.735563 pinjected-0.1.110/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0    18907 2023-08-01 10:55:32.742623 pinjected-0.1.110/pinjected/di/util.py
--rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinjected-0.1.110/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinjected-0.1.110/pinjected/global_configs
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.1.110/pinjected/global_configs.py
--rw-r--r--   0        0        0     2725 2023-08-01 10:55:32.769019 pinjected-0.1.110/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     1733 2023-08-01 10:55:32.719258 pinjected-0.1.110/pinjected/helper_structure.py
--rw-r--r--   0        0        0     7936 2023-08-01 10:58:43.088847 pinjected-0.1.110/pinjected/helpers.py
--rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinjected-0.1.110/pinjected/module_inspector.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.1.110/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0    23563 2023-08-01 10:58:43.077925 pinjected-0.1.110/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1580 2023-08-01 10:55:32.732359 pinjected-0.1.110/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0      928 2023-08-01 10:55:32.750717 pinjected-0.1.110/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.1.110/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      365 2023-08-01 10:58:43.080069 pinjected-0.1.110/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0    18619 2023-08-01 10:55:32.710604 pinjected-0.1.110/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.1.110/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       73 2023-08-01 10:55:32.761801 pinjected-0.1.110/pinjected/viz/graph.py
--rw-r--r--   0        0        0      694 2023-08-01 11:01:03.613382 pinjected-0.1.110/pyproject.toml
--rw-r--r--   0        0        0      918 1970-01-01 00:00:00.000000 pinjected-0.1.110/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.1.111/LICENSE
+-rw-r--r--   0        0        0      407 2023-08-01 10:55:32.734086 pinjected-0.1.111/pinjected/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.1.111/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.1.111/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     2522 2023-08-01 10:55:32.770639 pinjected-0.1.111/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      635 2023-08-01 10:55:32.714575 pinjected-0.1.111/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     6641 2023-08-01 10:58:43.087334 pinjected-0.1.111/pinjected/di/ast.py
+-rw-r--r--   0        0        0     1145 2023-08-01 10:55:32.707779 pinjected-0.1.111/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     1009 2023-08-01 10:55:32.748920 pinjected-0.1.111/pinjected/di/design.py
+-rw-r--r--   0        0        0     1918 2023-08-01 10:55:32.712483 pinjected-0.1.111/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.1.111/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    21758 2023-08-01 10:55:32.754770 pinjected-0.1.111/pinjected/di/graph.py
+-rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinjected-0.1.111/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    32965 2023-08-01 10:58:43.085630 pinjected-0.1.111/pinjected/di/injected.py
+-rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinjected-0.1.111/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0     2931 2023-08-01 10:55:32.737082 pinjected-0.1.111/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinjected-0.1.111/pinjected/di/permissioned/__init__.py
+-rw-r--r--   0        0        0     7805 2023-08-01 10:55:32.728581 pinjected-0.1.111/pinjected/di/permissioned/blueprint.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.1.111/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.1.111/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinjected-0.1.111/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.1.111/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.1.111/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6169 2023-08-01 10:55:32.723083 pinjected-0.1.111/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.1.111/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      980 2023-08-01 10:55:32.724965 pinjected-0.1.111/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1500 2023-08-01 10:55:32.752600 pinjected-0.1.111/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2239 2023-08-01 10:55:32.766231 pinjected-0.1.111/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      690 2023-08-01 10:55:32.735563 pinjected-0.1.111/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0    18907 2023-08-01 10:55:32.742623 pinjected-0.1.111/pinjected/di/util.py
+-rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinjected-0.1.111/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinjected-0.1.111/pinjected/global_configs
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.1.111/pinjected/global_configs.py
+-rw-r--r--   0        0        0     2725 2023-08-01 10:55:32.769019 pinjected-0.1.111/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     1734 2023-08-02 05:47:02.096952 pinjected-0.1.111/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     7936 2023-08-01 10:58:43.088847 pinjected-0.1.111/pinjected/helpers.py
+-rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinjected-0.1.111/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.1.111/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0    23645 2023-08-02 05:47:54.138652 pinjected-0.1.111/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1580 2023-08-01 10:55:32.732359 pinjected-0.1.111/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0      928 2023-08-01 10:55:32.750717 pinjected-0.1.111/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.1.111/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      365 2023-08-01 10:58:43.080069 pinjected-0.1.111/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0    18015 2023-08-03 01:33:08.549182 pinjected-0.1.111/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.1.111/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       73 2023-08-01 10:55:32.761801 pinjected-0.1.111/pinjected/viz/graph.py
+-rw-r--r--   0        0        0      694 2023-08-03 01:33:16.137811 pinjected-0.1.111/pyproject.toml
+-rw-r--r--   0        0        0      918 1970-01-01 00:00:00.000000 pinjected-0.1.111/PKG-INFO
```

### Comparing `pinjected-0.1.110/LICENSE` & `pinjected-0.1.111/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/app_designed.py` & `pinjected-0.1.111/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/app_injected.py` & `pinjected-0.1.111/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/applicative.py` & `pinjected-0.1.111/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/ast.py` & `pinjected-0.1.111/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/bindings.py` & `pinjected-0.1.111/pinjected/di/bindings.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/design.py` & `pinjected-0.1.111/pinjected/di/design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/designed.py` & `pinjected-0.1.111/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/dynamic_proxy.py` & `pinjected-0.1.111/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/graph.py` & `pinjected-0.1.111/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/injected.py` & `pinjected-0.1.111/pinjected/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/injected_analysis.py` & `pinjected-0.1.111/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/modular_injected.py` & `pinjected-0.1.111/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/permissioned/blueprint.py` & `pinjected-0.1.111/pinjected/di/permissioned/blueprint.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/proxiable.py` & `pinjected-0.1.111/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/session.py` & `pinjected-0.1.111/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/sessioned.py` & `pinjected-0.1.111/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/static_proxy.py` & `pinjected-0.1.111/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.1.111/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/test_graph.py` & `pinjected-0.1.111/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/test_injected.py` & `pinjected-0.1.111/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/test_proxiable.py` & `pinjected-0.1.111/pinjected/di/test_proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/di/util.py` & `pinjected-0.1.111/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/exceptions.py` & `pinjected-0.1.111/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/graph_inspection.py` & `pinjected-0.1.111/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/helper_structure.py` & `pinjected-0.1.111/pinjected/helper_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     # this needs to be checked from intellij side
 
 
 class IdeaRunConfigurations(BaseModel):
     configs: Dict[str, List[IdeaRunConfiguration]]
 
 
+
 @dataclass
 class MetaContext:
     trace: List[ModuleVarSpec]
     accumulated: Design
 
 
 @dataclass
```

### Comparing `pinjected-0.1.110/pinjected/helpers.py` & `pinjected-0.1.111/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/module_inspector.py` & `pinjected-0.1.111/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/nx_graph_util.py` & `pinjected-0.1.111/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/run_config_utils.py` & `pinjected-0.1.111/pinjected/run_config_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,18 @@
     )
     design = args.to_design()
     g = design.to_graph()
     configs: IdeaRunConfigurations = g[inspect_and_make_configurations(module_path)]
     pinjected.global_configs.pinjected_TRACK_ORIGIN = True
     logger.info(f"configs:{configs}")
     if print_to_stdout:
-        print(configs.model_dump_json())
+        try:
+            print(configs.model_dump_json())
+        except Exception as e:
+            print(configs.json())
     else:
         return configs
 
 
 SANDBOX_TEMPLATE = """
 from {design_path} import {design_name}
 from {var_path} import {var_name}
```

### Comparing `pinjected-0.1.110/pinjected/run_config_utils_v2.py` & `pinjected-0.1.111/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/test_package/__init__.py` & `pinjected-0.1.111/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.1.110/pinjected/visualize_di.py` & `pinjected-0.1.111/pinjected/visualize_di.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,64 +34,52 @@
 
 
 @safe
 def getitem(tgt, name):
     return tgt[name]
 
 
-# %%
-@dataclass
-class PinProvider:
-    src: Callable
+import colorsys
 
-    def __post_init__(self):
-        # self.arg_binding_keys:Result = safe_attr(self.src, "_pinject_arg_binding_keys")
-        self.non_injectables: Result = safe_attr(self.src, "_pinject_non_injectables")
-        # self.orig_f:Result = safe_attr(self.src, "_pinject_orig_fn")
-        # self.provider_decorations:Result = safe_attr(self.src, "_pinject_provider_decorations")
+def rgb_to_hex(rgb):
+    return '#%02x%02x%02x' % rgb
 
+def get_color(n_edges):
+    h = (1.0 - max(0,min(10,n_edges)) / 10.0) * 0.67  # 0.67 is the hue for blue in the HSV color system.
+    rgb = [int(x * 255) for x in colorsys.hsv_to_rgb(h, 1.0, 1.0)]  # convert hsv color (h,1,1) to rgb then multiply by 255
+    return rgb_to_hex(tuple(rgb))
 
 @dataclass
 class DIGraph:
     src: Design
 
     def new_name(self, base: str):
         return f"{base}_{str(uuid.uuid4())[:6]}"
 
     def __post_init__(self):
         self.src = self.src.bind_instance(session='DummyForVisualization').build()
         self.helper = DIGraphHelper(self.src)
+        # TODO combine these mappings into one. the keys must not override each other
         self.implicit_mappings = dict(self.helper.get_implicit_mapping())
-        # we want to know if the binding is InjectedProvider or not
         self.explicit_mappings: Dict[str, Injected] = {k: b.to_injected() for k, b in self.src.bindings.items()}
-
         self.explicit_mappings.update(**self.helper.total_mappings())
         self.multi_mappings = {k: b for k, b in self.src.multi_binds.items()}
 
         self.direct_injected = dict()
         self.injected_to_id = dict()
 
         @memoize
         def deps_impl(src: str):
             if "provide_" in src:
                 src = src.replace("provide_", "")
             if src in self.explicit_mappings:
                 em = self.explicit_mappings[src]
                 return self.resolve_injected(em)
-                # if isinstance(em, InjectedProvider):
-                #     return self.resolve_injected(em.src)
-                # else:
-                #     return em.to_injected().dynamic_dependencies()
             elif src in self.implicit_mappings:
                 return Injected.bind(self.implicit_mappings[src]).dynamic_dependencies()
-            elif src in self.pinject_mappings:
-                pp: PinProvider = self.pinject_mappings[src]
-                deps = [d for d in Injected.bind(pp.src).dynamic_dependencies() if
-                        d not in pp.non_injectables.value_or([])]
-                return deps
             elif src in self.multi_mappings:
                 return list(
                     set(chain(*[Injected.bind(tgt).dynamic_dependencies() for tgt in self.multi_mappings[src]])))
             elif src in self.direct_injected:
                 di = self.direct_injected[src]
                 return self.resolve_injected(di)
             else:
@@ -154,16 +142,14 @@
         item = getitem(
             self.src.bindings, key
         ).lash(
             lambda e: getitem(self.explicit_mappings, key)
         ).lash(
             lambda e: getitem(self.implicit_mappings, key)
         ).lash(
-            lambda e: getitem(self.pinject_mappings, key)
-        ).lash(
             lambda e: getitem(self.multi_mappings, key)
         ).lash(
             lambda e: getitem(self.direct_injected, key)
         )
         if isinstance(item, Failure):
             raise KeyError(f"{key} is not found in design!")
         return item.unwrap()
@@ -317,20 +303,22 @@
 
             if replace_missing and not is_successful(safe(self.__getitem__)(n)):
                 group, short, long = "missing", f"missing_{n}", f"missing_{n}"
             else:
                 group, short, long = parse(self[n])
             short = str(short).replace("<", "").replace(">", "")[:100]
             n_edges = len(list(nx_graph.neighbors(n))) + safe(self.dependencies_of)(n).map(len).value_or(0)
+
+
             return dict(
                 label=f"{n}\n{short}",
                 title=long,
-                group=group,
                 value=n_edges,
                 mass=n_edges * 0.5 + 1,
+                color=get_color(n_edges),
             )
 
         return node_to_sl
 
     def stylize_graph(self, nx_graph, replace_missing):
         node_to_sl = self.get_node_to_sl(nx_graph, replace_missing)
         for n in nx_graph.nodes:
```

### Comparing `pinjected-0.1.110/pyproject.toml` & `pinjected-0.1.111/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.1.110"
+version = "0.1.111"
 description = "immutable wrapper for pinject"
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "^0.21.0"
```

### Comparing `pinjected-0.1.110/PKG-INFO` & `pinjected-0.1.111/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.1.110
+Version: 0.1.111
 Summary: immutable wrapper for pinject
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

