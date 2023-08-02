# Comparing `tmp/panda_utils-1.5b1.tar.gz` & `tmp/panda_utils-1.5b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.5b1.tar", last modified: Tue Aug  1 22:44:25 2023, max compression
+gzip compressed data, was "panda_utils-1.5b2.tar", last modified: Wed Aug  2 22:44:18 2023, max compression
```

## Comparing `panda_utils-1.5b1.tar` & `panda_utils-1.5b2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.769596 panda_utils-1.5b1/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.5b1/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-08-01 22:44:25.769596 panda_utils-1.5b1/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.5b1/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.5b1/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.766262 panda_utils-1.5b1/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.5b1/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.5b1/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.769596 panda_utils-1.5b1/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.5b1/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5006 2023-07-31 00:27:55.000000 panda_utils-1.5b1/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      247 2023-07-28 09:44:44.000000 panda_utils-1.5b1/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      747 2023-07-30 10:56:09.000000 panda_utils-1.5b1/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    16004 2023-08-01 22:32:42.000000 panda_utils-1.5b1/panda_utils/assetpipeline/models.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.5b1/panda_utils/assetpipeline/textures.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.769596 panda_utils-1.5b1/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.5b1/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      615 2023-07-28 09:44:44.000000 panda_utils-1.5b1/panda_utils/blender/export_glb.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2025 2023-08-01 22:08:01.000000 panda_utils-1.5b1/panda_utils/blender/export_with_yabee.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      527 2023-07-28 09:44:44.000000 panda_utils-1.5b1/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.5b1/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.769596 panda_utils-1.5b1/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.5b1/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5632 2023-08-01 22:33:37.000000 panda_utils-1.5b1/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      762 2023-07-25 21:42:36.000000 panda_utils-1.5b1/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.769596 panda_utils-1.5b1/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.5b1/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.5b1/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.5b1/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.5b1/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.5b1/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.5b1/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.5b1/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.766262 panda_utils-1.5b1/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-08-01 22:44:25.000000 panda_utils-1.5b1/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      991 2023-08-01 22:44:25.000000 panda_utils-1.5b1/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-08-01 22:44:25.000000 panda_utils-1.5b1/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-08-01 22:44:25.000000 panda_utils-1.5b1/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-08-01 22:44:25.000000 panda_utils-1.5b1/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-08-01 22:44:06.000000 panda_utils-1.5b1/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.5b1/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-08-01 22:44:25.769596 panda_utils-1.5b1/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.822243 panda_utils-1.5b2/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.5b2/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-08-02 22:44:18.822243 panda_utils-1.5b2/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.5b2/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.5b2/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.815577 panda_utils-1.5b2/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.5b2/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.5b2/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.818910 panda_utils-1.5b2/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.5b2/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5006 2023-07-31 00:27:55.000000 panda_utils-1.5b2/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      247 2023-07-28 09:44:44.000000 panda_utils-1.5b2/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      747 2023-07-30 10:56:09.000000 panda_utils-1.5b2/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    15739 2023-08-02 21:27:11.000000 panda_utils-1.5b2/panda_utils/assetpipeline/models.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.5b2/panda_utils/assetpipeline/textures.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.818910 panda_utils-1.5b2/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.5b2/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      615 2023-07-28 09:44:44.000000 panda_utils-1.5b2/panda_utils/blender/export_glb.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2025 2023-08-01 22:08:01.000000 panda_utils-1.5b2/panda_utils/blender/export_with_yabee.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      527 2023-07-28 09:44:44.000000 panda_utils-1.5b2/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.5b2/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.818910 panda_utils-1.5b2/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.5b2/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     6010 2023-08-02 21:34:30.000000 panda_utils-1.5b2/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      762 2023-07-25 21:42:36.000000 panda_utils-1.5b2/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.822243 panda_utils-1.5b2/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.5b2/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.5b2/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.5b2/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.5b2/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.5b2/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.5b2/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.5b2/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.818910 panda_utils-1.5b2/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-08-02 22:44:18.000000 panda_utils-1.5b2/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      991 2023-08-02 22:44:18.000000 panda_utils-1.5b2/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-08-02 22:44:18.000000 panda_utils-1.5b2/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-08-02 22:44:18.000000 panda_utils-1.5b2/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-08-02 22:44:18.000000 panda_utils-1.5b2/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-08-02 22:44:08.000000 panda_utils-1.5b2/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.5b2/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-08-02 22:44:18.822243 panda_utils-1.5b2/setup.cfg
```

### Comparing `panda_utils-1.5b1/LICENSE` & `panda_utils-1.5b2/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/PKG-INFO` & `panda_utils-1.5b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda_utils
-Version: 1.5b1
+Version: 1.5b2
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.5b1/README.md` & `panda_utils-1.5b2/README.md`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/__main__.py` & `panda_utils-1.5b2/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.5b2/panda_utils/assetpipeline/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/assetpipeline/misc.py` & `panda_utils-1.5b2/panda_utils/assetpipeline/misc.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/assetpipeline/models.py` & `panda_utils-1.5b2/panda_utils/assetpipeline/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,21 +147,17 @@
     for file in ctx.files:
         if file.endswith(".blend"):
             logger.info("%s: Exporting through YABEE: %s", ctx.name, file)
             full_path = pathlib.Path(ctx.cwd, file)
             egg_name = file[:-6] + ".egg"
             run_blender(ctx.cwd, full_path, "blender/export_with_yabee.py", egg_name, *args_converted)
 
-            # NOTE: yabee does not care about the spaces in the file
-            # which means the file is hard to postprocess, so we have to do this thing below
-            # I think it only happens if any animations are exported - Wizz
-
-            if kwargs:
-                egg2bam(ctx.putil_ctx, egg_name)
-                bam2egg(ctx.putil_ctx, egg_name[:-4] + ".bam")
+            target_name = ctx.model_name + ".egg"
+            if egg_name != target_name:
+                shutil.move(egg_name, target_name)
 
 
 def action_optimize(ctx, map_textures="true"):
     map_textures = map_textures.lower() not in ("", "0", "false")
 
     textures = set()
     ctx.cache_eggs()
@@ -338,27 +334,27 @@
 def action_optchar(ctx, flags, expose):
     ctx.uncache_eggs()
     if isinstance(flags, str):
         flags = flags.split(",")
     if isinstance(expose, str):
         expose = expose.split(",")
 
-    for file in ctx.files:
-        if file.endswith(".egg"):
-            command = ["egg-optchar", file, "-inplace", "-keepall"]
-
-            for flag in flags:
-                command.append("-flag")
-                command.append(flag)
-
-            for joint in expose:
-                command.append("-expose")
-                command.append(joint)
+    file = ctx.model_name + ".egg"
+    if file in ctx.files:
+        command = ["egg-optchar", file, "-inplace", "-keepall"]
+
+        for flag in flags:
+            command.append("-flag")
+            command.append(flag)
+
+        for joint in expose:
+            command.append("-expose")
+            command.append(joint)
 
-            util.run_panda(ctx.putil_ctx, *command)
+        util.run_panda(ctx.putil_ctx, *command)
 
 
 def action_group_rename(ctx, **kwargs):
     ctx.cache_eggs()
     for tree in ctx.eggs.values():
         removals = set()
         for group in tree.findall("Group"):
```

### Comparing `panda_utils-1.5b1/panda_utils/assetpipeline/textures.py` & `panda_utils-1.5b2/panda_utils/assetpipeline/textures.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/blender/export_glb.py` & `panda_utils-1.5b2/panda_utils/blender/export_glb.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/blender/export_with_yabee.py` & `panda_utils-1.5b2/panda_utils/blender/export_with_yabee.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/blender/import_model.py` & `panda_utils-1.5b2/panda_utils/blender/import_model.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/eggtree/eggparse.py` & `panda_utils-1.5b2/panda_utils/eggtree/eggparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 
 
 class EggTree:
     def __init__(self, *children):
         self.children = list(children)
 
     def __iadd__(self, other):
-        self.children.append(other)
+        if isinstance(other, list):
+            self.children.extend(other)
+        else:
+            self.children.append(other)
         return self
 
     def __iter__(self):
         return iter(self.children)
 
     def __repr__(self):
         return "\n".join(str(child) for child in self.children)
@@ -141,41 +144,48 @@
 
 def sanitize_string(val):
     if val and val[0] in "\"'":
         return val[1:-1]
     return val
 
 
-single_line_leaf_regex = re.compile(r"<([A-Za-z0-9_$]+)> ([-a-z0-9A-Z_.]+ )?\{ ?(.+) ?}")
+single_line_leaf_regex = re.compile(r"<([A-Za-z0-9_$*]+)> ([-a-z0-9A-Z_.]+ )?\{ ?(.+) ?}")
 preline_regex = re.compile(r"<([A-Za-z0-9_$]+)> ([-a-z0-9A-Z_.<>\" ]+ )?\{([^\n]*)")
 
 
 def subtree_tokenize(lines: List[str]):
     last_line = lines[-1].strip()
     if len(lines) == 1:
+        if last_line.count("}") > 1 and not last_line.startswith("<VertexRef>"):
+            parts = [x + "}" for x in last_line.split("}")[:-1]]
+            nodes = []
+            for part in parts:
+                nodes += subtree_tokenize([part])
+            return nodes
+
         match = single_line_leaf_regex.match(last_line)
         if not match:
             raise ValueError(f"subtree_tokenize: Invalid single-line subtree: {lines[0]}")
 
         final = match.group(3)
         if "}" not in final or match.group(1) == "VertexRef":
-            return EggLeaf(match.group(1), match.group(2), final)
-        return EggBranch(match.group(1), match.group(2), EggTree(subtree_tokenize([final])))
+            return [EggLeaf(match.group(1), match.group(2), final)]
+        return [EggBranch(match.group(1), match.group(2), EggTree(*subtree_tokenize([final])))]
 
     lines = lines[:-1] + list(last_line)
     if lines[-1] != "}":
         raise ValueError(f"subtree_tokenize: Invalid tree finish: {lines[-1]}")
     preamble = preline_regex.match(lines[0])
     if not preamble:
         raise ValueError(f"subtree_tokenize: Invalid preamble: {lines[0]}")
     append = preamble.group(3)
     if append:
         lines.insert(1, append)
     tree = egg_tokenize([line.strip() for line in lines[1:-1]])
-    return EggBranch(preamble.group(1), preamble.group(2), tree)
+    return [EggBranch(preamble.group(1), preamble.group(2), tree)]
 
 
 def egg_tokenize(lines: List[str]) -> EggTree:
     tree = EggTree()
 
     current_indent = 0
     subtree = []
```

### Comparing `panda_utils-1.5b1/panda_utils/eggtree/operations.py` & `panda_utils-1.5b2/panda_utils/eggtree/operations.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/tools/animconvert.py` & `panda_utils-1.5b2/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/tools/convert.py` & `panda_utils-1.5b2/panda_utils/tools/convert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/tools/downscale.py` & `panda_utils-1.5b2/panda_utils/tools/downscale.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/tools/palettize.py` & `panda_utils-1.5b2/panda_utils/tools/palettize.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/tools/toontown.py` & `panda_utils-1.5b2/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils/util.py` & `panda_utils-1.5b2/panda_utils/util.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/panda_utils.egg-info/PKG-INFO` & `panda_utils-1.5b2/panda_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-utils
-Version: 1.5b1
+Version: 1.5b2
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.5b1/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.5b2/panda_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b1/pyproject.toml` & `panda_utils-1.5b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.5b1"
+version = "1.5b2"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

