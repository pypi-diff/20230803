# Comparing `tmp/omero-cli-transfer-0.6.0.tar.gz` & `tmp/omero-cli-transfer-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-cli-transfer-0.6.0.tar", last modified: Mon Jul 17 14:41:51 2023, max compression
+gzip compressed data, was "omero-cli-transfer-0.7.0.tar", last modified: Thu Aug  3 18:28:21 2023, max compression
```

## Comparing `omero-cli-transfer-0.6.0.tar` & `omero-cli-transfer-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20068 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/src/generate_omero_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    41549 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/src/generate_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/src/omero/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/src/omero/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/src/omero/plugins/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-17 14:41:51.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-17 14:41:51.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:41:51.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-17 14:41:51.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 14:41:51.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:28:21.928643 omero-cli-transfer-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-08-03 18:28:19.000000 omero-cli-transfer-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-08-03 18:28:21.928643 omero-cli-transfer-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-08-03 18:28:19.000000 omero-cli-transfer-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 18:28:21.928643 omero-cli-transfer-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-08-03 18:28:19.000000 omero-cli-transfer-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:28:21.928643 omero-cli-transfer-0.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    23543 2023-08-03 18:28:19.000000 omero-cli-transfer-0.7.0/src/generate_omero_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42430 2023-08-03 18:28:19.000000 omero-cli-transfer-0.7.0/src/generate_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:28:21.928643 omero-cli-transfer-0.7.0/src/omero/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:28:21.928643 omero-cli-transfer-0.7.0/src/omero/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-03 18:28:19.000000 omero-cli-transfer-0.7.0/src/omero/plugins/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:28:21.928643 omero-cli-transfer-0.7.0/src/omero_cli_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-08-03 18:28:21.000000 omero-cli-transfer-0.7.0/src/omero_cli_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-03 18:28:21.000000 omero-cli-transfer-0.7.0/src/omero_cli_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:28:21.000000 omero-cli-transfer-0.7.0/src/omero_cli_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-03 18:28:21.000000 omero-cli-transfer-0.7.0/src/omero_cli_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 18:28:21.000000 omero-cli-transfer-0.7.0/src/omero_cli_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24781 2023-08-03 18:28:19.000000 omero-cli-transfer-0.7.0/src/omero_cli_transfer.py
```

### Comparing `omero-cli-transfer-0.6.0/LICENSE` & `omero-cli-transfer-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omero-cli-transfer-0.6.0/PKG-INFO` & `omero-cli-transfer-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-cli-transfer
-Version: 0.6.0
+Version: 0.7.0
 Summary: A set of utilities for exporting a transfer packet from an OMERO server and importing it in a different server. Developed by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/omero-cli-transfer
 Maintainer: Erick Ratamero
 Maintainer-email: erick.ratamero@jax.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -83,14 +83,18 @@
 
 `--ln_s` forces imports to use the transfer=ln_s option, in-place importing files. Same restrictions of regular in-place imports apply.
 
 `--output` allows for specifying an optional output folder where the packet will be unzipped.
 
 `--folder` allows the user to point to a previously-unpacked folder rather than a single file.
 
+`--merge` will use existing Projects, Datasets and Screens if the current user
+already owns entities with the same name as ones defined in `transfer.xml`,
+effectively merging the "new" unpacked entities with existing ones.
+
 Examples:
 ```
 omero transfer unpack transfer_pack.zip
 omero transfer unpack --output /home/user/optional_folder --ln_s
 omero transfer unpack --folder /home/user/unpacked_folder/
 ```
```

### Comparing `omero-cli-transfer-0.6.0/README.md` & `omero-cli-transfer-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,18 @@
 
 `--ln_s` forces imports to use the transfer=ln_s option, in-place importing files. Same restrictions of regular in-place imports apply.
 
 `--output` allows for specifying an optional output folder where the packet will be unzipped.
 
 `--folder` allows the user to point to a previously-unpacked folder rather than a single file.
 
+`--merge` will use existing Projects, Datasets and Screens if the current user
+already owns entities with the same name as ones defined in `transfer.xml`,
+effectively merging the "new" unpacked entities with existing ones.
+
 Examples:
 ```
 omero transfer unpack transfer_pack.zip
 omero transfer unpack --output /home/user/optional_folder --ln_s
 omero transfer unpack --folder /home/user/unpacked_folder/
 ```
```

### Comparing `omero-cli-transfer-0.6.0/setup.py` & `omero-cli-transfer-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,27 +80,27 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     packages=['', 'omero.plugins'],
     package_dir={"": "src"},
     name="omero-cli-transfer",
-    version='0.6.0',
+    version='0.7.0',
     maintainer="Erick Ratamero",
     maintainer_email="erick.ratamero@jax.org",
     description=("A set of utilities for exporting a transfer"
                  " packet from an OMERO server and importing "
                  "it in a different server. Developed by the "
                  "Research IT team at The Jackson Laboratory."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheJacksonLaboratory/omero-cli-transfer",
     install_requires=[
         'ezomero==2.0.0',
-        'ome-types==0.3.4'
+        'ome-types==0.4.0'
     ],
     extras_require={
         "rocrate": ["rocrate==0.7.0"],
     },
     python_requires='>=3.8',
     cmdclass={'test': PyTest},
     tests_require=['pytest', 'restview', 'mox3'],
```

### Comparing `omero-cli-transfer-0.6.0/src/generate_omero_objects.py` & `omero-cli-transfer-0.7.0/src/generate_omero_objects.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,30 +21,95 @@
 from omero.rtypes import rstring, RStringI, rint
 from ezomero import rois
 from pathlib import Path
 import os
 import copy
 
 
+def create_or_set_projects(pjs: List[Project], conn: BlitzGateway,
+                           merge: bool) -> dict:
+    pj_map = {}
+    if not merge:
+        pj_map = create_projects(pjs, conn)
+    else:
+        for pj in pjs:
+            pj_id = find_project(pj, conn)
+            if not pj_id:
+                pj_id = ezomero.post_project(conn, pj.name, pj.description)
+            pj_map[pj.id] = pj_id
+    return pj_map
+
+
 def create_projects(pjs: List[Project], conn: BlitzGateway) -> dict:
     pj_map = {}
     for pj in pjs:
         pj_id = ezomero.post_project(conn, pj.name, pj.description)
         pj_map[pj.id] = pj_id
     return pj_map
 
 
+def find_project(pj: Project, conn: BlitzGateway) -> int:
+    id = 0
+    my_exp_id = conn.getUser().getId()
+    for p in conn.getObjects("Project", opts={'owner': my_exp_id}):
+        if p.getName() == pj.name:
+            id = p.getId()
+    return id
+
+
+def create_or_set_screens(scrs: List[Screen], conn: BlitzGateway, merge: bool
+                          ) -> dict:
+    scr_map = {}
+    if not merge:
+        scr_map = create_screens(scrs, conn)
+    else:
+        for scr in scrs:
+            scr_id = find_screen(scr, conn)
+            if not scr_id:
+                scr_id = ezomero.post_screen(conn, scr.name, scr.description)
+            scr_map[scr.id] = scr_id
+    return scr_map
+
+
 def create_screens(scrs: List[Screen], conn: BlitzGateway) -> dict:
     scr_map = {}
     for scr in scrs:
         scr_id = ezomero.post_screen(conn, scr.name, scr.description)
         scr_map[scr.id] = scr_id
     return scr_map
 
 
+def find_screen(sc: Screen, conn: BlitzGateway) -> int:
+    id = 0
+    my_exp_id = conn.getUser().getId()
+    for s in conn.getObjects("Screen", opts={'owner': my_exp_id}):
+        if s.getName() == sc.name:
+            id = s.getId()
+    return id
+
+
+def create_or_set_datasets(dss: List[Dataset], pjs: List[Project],
+                           conn: BlitzGateway, merge: bool) -> dict:
+    ds_map = {}
+    if not merge:
+        ds_map = create_datasets(dss, conn)
+    else:
+        for ds in dss:
+            ds_id = find_dataset(ds, pjs, conn)
+            if not ds_id:
+                dataset = DatasetWrapper(conn, DatasetI())
+                dataset.setName(ds.name)
+                if ds.description is not None:
+                    dataset.setDescription(ds.description)
+                dataset.save()
+                ds_id = dataset.getId()
+            ds_map[ds.id] = ds_id
+    return ds_map
+
+
 def create_datasets(dss: List[Dataset], conn: BlitzGateway) -> dict:
     """
     Currently doing it the non-ezomero way because ezomero always
     puts "orphan" Datasets in the user's default group
     """
     ds_map = {}
     for ds in dss:
@@ -54,14 +119,39 @@
             dataset.setDescription(ds.description)
         dataset.save()
         ds_id = dataset.getId()
         ds_map[ds.id] = ds_id
     return ds_map
 
 
+def find_dataset(ds: Dataset, pjs: List[Project], conn: BlitzGateway) -> int:
+    id = 0
+    my_exp_id = conn.getUser().getId()
+    orphan = True
+    for pj in pjs:
+        for dsref in pj.dataset_refs:
+            if dsref.id == ds.id:
+                orphan = False
+    if not orphan:
+        for pj in pjs:
+            for p in conn.getObjects("Project", opts={'owner': my_exp_id}):
+                if p.getName() == pj.name:
+                    for dsref in pj.dataset_refs:
+                        if dsref.id == ds.id:
+                            for ds_rem in p.listChildren():
+                                if ds.name == ds_rem.getName():
+                                    id = ds_rem.getId()
+    else:
+        for d in conn.getObjects("Dataset", opts={'owner': my_exp_id,
+                                                  'orphaned': True}):
+            if d.getName() == ds.name:
+                id = d.getId()
+    return id
+
+
 def create_annotations(ans: List[Annotation], conn: BlitzGateway, hash: str,
                        folder: str, metadata: List[str]) -> dict:
     ann_map = {}
     for an in ans:
         if isinstance(an, TagAnnotation):
             tag_ann = TagAnnotationWrapper(conn)
             tag_ann.setValue(an.value)
@@ -69,15 +159,15 @@
             tag_ann.save()
             ann_map[an.id] = tag_ann.getId()
         elif isinstance(an, MapAnnotation):
             map_ann = MapAnnotationWrapper(conn)
             namespace = an.namespace
             map_ann.setNs(namespace)
             key_value_data = []
-            for v in an.value.m:
+            for v in an.value.ms:
                 if int(an.id.split(":")[-1]) < 0:
                     if not metadata:
                         key_value_data.append(['empty_metadata', "True"])
                         break
                     if v.k == "md5" and "md5" in metadata:
                         key_value_data.append(['zip_file_md5', hash])
                     if v.k == "origin_image_id" and "img_id" in metadata:
@@ -127,15 +217,15 @@
     return ann_map
 
 
 def create_original_file(ann: FileAnnotation, ans: List[Annotation],
                          conn: BlitzGateway, folder: str
                          ) -> OriginalFileWrapper:
     curr_folder = str(Path('.').resolve())
-    for an in ann.annotation_ref:
+    for an in ann.annotation_refs:
         clean_id = int(an.id.split(":")[-1])
         if clean_id < 0:
             cmnt_id = an.id
     for an_loop in ans:
         if an_loop.id == cmnt_id and isinstance(an_loop, CommentAnnotation):
             fpath = str(an_loop.value)
     dest_path = str(os.path.join(curr_folder, folder,  '.', fpath))
@@ -145,15 +235,15 @@
 
 def create_plate_map(ome: OME, img_map: dict, conn: BlitzGateway
                      ) -> Tuple[dict, OME]:
     newome = copy.deepcopy(ome)
     plate_map = {}
     map_ref_ids = []
     for plate in ome.plates:
-        ann_ids = [i.id for i in plate.annotation_ref]
+        ann_ids = [i.id for i in plate.annotation_refs]
         file_path = ""
         for ann in ome.structured_annotations:
             if (ann.id in ann_ids and
                     type(ann) == CommentAnnotation and
                     int(ann.id.split(":")[-1]) < 0):
                 newome.structured_annotations.remove(ann)
                 map_ref_ids.append(ann.id)
@@ -197,17 +287,17 @@
             # plate was imported as plate
             plate_id = plate_ids[0]
         else:
             # plate was imported as images
             plate_id = create_plate_from_images(plate, img_map, conn)
         plate_map[plate.id] = plate_id
     for p in newome.plates:
-        for ref in p.annotation_ref:
+        for ref in p.annotation_refs:
             if ref.id in map_ref_ids:
-                p.annotation_ref.remove(ref)
+                p.annotation_refs.remove(ref)
     return plate_map, newome
 
 
 def create_plate_from_images(plate: Plate, img_map: dict, conn: BlitzGateway
                              ) -> int:
     plateobj = PlateI()
     plateobj.name = RStringI(plate.name)
@@ -338,51 +428,61 @@
     # a = a / 256.0
     return (r, g, b, a)
 
 
 def create_rois(rois: List[ROI], imgs: List[Image], img_map: dict,
                 conn: BlitzGateway):
     for img in imgs:
-        for roiref in img.roi_ref:
+        for roiref in img.roi_refs:
             roi = next(filter(lambda x: x.id == roiref.id, rois))
             shapes = create_shapes(roi)
             img_id_dest = img_map[img.id]
             ezomero.post_roi(conn, img_id_dest, shapes, name=roi.name,
                              description=roi.description)
     return
 
 
 def link_datasets(ome: OME, proj_map: dict, ds_map: dict, conn: BlitzGateway):
     for proj in ome.projects:
         proj_id = proj_map[proj.id]
+        proj_obj = conn.getObject("Project", proj_id)
+        existing_ds = []
+        for dataset in proj_obj.listChildren():
+            existing_ds.append(dataset.getId())
         ds_ids = []
-        for ds in proj.dataset_ref:
+        for ds in proj.dataset_refs:
             ds_id = ds_map[ds.id]
-            ds_ids.append(ds_id)
+            if ds_id not in existing_ds:
+                ds_ids.append(ds_id)
         ezomero.link_datasets_to_project(conn, ds_ids, proj_id)
     return
 
 
 def link_plates(ome: OME, screen_map: dict, plate_map: dict,
                 conn: BlitzGateway):
     for screen in ome.screens:
         screen_id = screen_map[screen.id]
+        scr_obj = conn.getObject("Screen", screen_id)
+        existing_pl = []
+        for pl in scr_obj.listChildren():
+            existing_pl.append(pl.getId())
         pl_ids = []
-        for pl in screen.plate_ref:
+        for pl in screen.plate_refs:
             pl_id = plate_map[pl.id]
-            pl_ids.append(pl_id)
+            if pl_id not in existing_pl:
+                pl_ids.append(pl_id)
         ezomero.link_plates_to_screen(conn, pl_ids, screen_id)
     return
 
 
 def link_images(ome: OME, ds_map: dict, img_map: dict, conn: BlitzGateway):
     for ds in ome.datasets:
         ds_id = ds_map[ds.id]
         img_ids = []
-        for img in ds.image_ref:
+        for img in ds.image_refs:
             try:
                 img_id = img_map[img.id]
                 img_ids.append(img_id)
             except KeyError:
                 continue
         ezomero.link_images_to_dataset(conn, img_ids, ds_id)
     return
@@ -391,55 +491,55 @@
 def link_annotations(ome: OME, proj_map: dict, ds_map: dict, img_map: dict,
                      ann_map: dict, scr_map: dict, pl_map: dict,
                      conn: BlitzGateway):
     for proj in ome.projects:
         proj_id = proj_map[proj.id]
         proj_obj = conn.getObject("Project", proj_id)
         anns = ome.structured_annotations
-        for annref in proj.annotation_ref:
+        for annref in proj.annotation_refs:
             ann = next(filter(lambda x: x.id == annref.id, anns))
             link_one_annotation(proj_obj, ann, ann_map, conn)
     for ds in ome.datasets:
         ds_id = ds_map[ds.id]
         ds_obj = conn.getObject("Dataset", ds_id)
         anns = ome.structured_annotations
-        for annref in ds.annotation_ref:
+        for annref in ds.annotation_refs:
             ann = next(filter(lambda x: x.id == annref.id, anns))
             link_one_annotation(ds_obj, ann, ann_map, conn)
     for img in ome.images:
         try:
             img_id = img_map[img.id]
             img_obj = conn.getObject("Image", img_id)
             anns = ome.structured_annotations
-            for annref in img.annotation_ref:
+            for annref in img.annotation_refs:
                 ann = next(filter(lambda x: x.id == annref.id, anns))
                 link_one_annotation(img_obj, ann, ann_map, conn)
         except KeyError:
             continue
     for scr in ome.screens:
         scr_id = scr_map[scr.id]
         scr_obj = conn.getObject("Screen", scr_id)
         anns = ome.structured_annotations
-        for annref in scr.annotation_ref:
+        for annref in scr.annotation_refs:
             ann = next(filter(lambda x: x.id == annref.id, anns))
             link_one_annotation(scr_obj, ann, ann_map, conn)
     for pl in ome.plates:
         pl_id = pl_map[pl.id]
         pl_obj = conn.getObject("Plate", pl_id)
         anns = ome.structured_annotations
-        for annref in pl.annotation_ref:
+        for annref in pl.annotation_refs:
             ann = next(filter(lambda x: x.id == annref.id, anns))
             link_one_annotation(pl_obj, ann, ann_map, conn)
         anns = ome.structured_annotations
         for well in pl.wells:
-            if len(well.annotation_ref) > 0:
+            if len(well.annotation_refs) > 0:
                 row, col = well.row, well.column
                 well_id = ezomero.get_well_id(conn, pl_id, row, col)
                 well_obj = conn.getObject("Well", well_id)
-                for annref in well.annotation_ref:
+                for annref in well.annotation_refs:
                     ann = next(filter(lambda x: x.id == annref.id, anns))
                     link_one_annotation(well_obj, ann, ann_map, conn)
     return
 
 
 def link_one_annotation(obj: IObject, ann: Annotation, ann_map: dict,
                         conn: BlitzGateway):
@@ -481,21 +581,21 @@
             pl_obj.save()
         except KeyError:
             print(f"Plate corresponding to {pl.id} not found. Skipping.")
     return
 
 
 def populate_omero(ome: OME, img_map: dict, conn: BlitzGateway, hash: str,
-                   folder: str, metadata: List[str]):
+                   folder: str, metadata: List[str], merge: bool):
     plate_map, ome = create_plate_map(ome, img_map, conn)
     rename_images(ome.images, img_map, conn)
     rename_plates(ome.plates, plate_map, conn)
-    proj_map = create_projects(ome.projects, conn)
-    ds_map = create_datasets(ome.datasets, conn)
-    screen_map = create_screens(ome.screens, conn)
+    proj_map = create_or_set_projects(ome.projects, conn, merge)
+    ds_map = create_or_set_datasets(ome.datasets, ome.projects, conn, merge)
+    screen_map = create_or_set_screens(ome.screens, conn, merge)
     ann_map = create_annotations(ome.structured_annotations, conn,
                                  hash, folder, metadata)
     create_rois(ome.rois, ome.images, img_map, conn)
     link_plates(ome, screen_map, plate_map, conn)
     link_datasets(ome, proj_map, ds_map, conn)
     link_images(ome, ds_map, img_map, conn)
     link_annotations(ome, proj_map, ds_map, img_map, ann_map,
```

### Comparing `omero-cli-transfer-0.6.0/src/generate_xml.py` & `omero-cli-transfer-0.7.0/src/generate_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,15 +455,15 @@
     for _key, _value in md_dict.items():
         if _value:
             mmap.append(M(k=_key, value=str(_value)))
         else:
             mmap.append(M(k=_key, value=''))
     kv, ref = create_kv_and_ref(id=id,
                                 namespace=ns,
-                                value=Map(m=mmap))
+                                value=Map(ms=mmap))
     return kv, ref
 
 
 def create_objects(folder, filelist):
     img_files = []
     cli = CLI()
     cli.loadplugins()
@@ -523,15 +523,15 @@
     lines = text.split("\n")
     targets = [line for line in lines if not line.startswith("#")
                and len(line) > 0]
     return targets
 
 
 def parse_showinf(text, counter_imgs, counter_plates, target):
-    ome = from_xml(text, parser='xmlschema')
+    ome = from_xml(text)
     images = []
     plates = []
     annotations = []
     img_id = counter_imgs
     pl_id = counter_plates
     img_ref = {}
     for image in ome.images:
@@ -548,15 +548,18 @@
         uid = (-1) * uuid4().int
         an = CommentAnnotation(id=uid,
                                namespace=img_id_str,
                                value=target
                                )
         annotations.append(an)
         anref = AnnotationRef(id=an.id)
-        img.annotation_ref.append(anref)
+        img.annotation_refs.append(anref)
+        an, anref = create_prepare_metadata()
+        annotations.append(an)
+        img.annotation_refs.append(anref)
         images.append(img)
     for plate in ome.plates:
         pl_id_str = f"Plate:{str(pl_id)}"
         pl = Plate(id=pl_id_str, name=plate.name, wells=plate.wells)
         for w in pl.wells:
             for ws in w.well_samples:
                 ws.image_ref.id = img_ref[ws.image_ref.id]
@@ -564,19 +567,41 @@
         uid = (-1) * uuid4().int
         an = CommentAnnotation(id=uid,
                                namespace=pl_id_str,
                                value=target
                                )
         annotations.append(an)
         anref = AnnotationRef(id=an.id)
-        pl.annotation_ref.append(anref)
+        pl.annotation_refs.append(anref)
         plates.append(pl)
     return images, plates, annotations
 
 
+def create_prepare_metadata():
+    software = "omero-cli-transfer"
+    version = pkg_resources.get_distribution(software).version
+    date_time = datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
+    ns = 'openmicroscopy.org/cli/transfer/prepare'
+    id = (-1) * uuid4().int
+    md_dict: Dict[str, Any] = {}
+    md_dict['software'] = software
+    md_dict['version'] = version
+    md_dict['packing_timestamp'] = date_time
+    mmap = []
+    for _key, _value in md_dict.items():
+        if _value:
+            mmap.append(M(k=_key, value=str(_value)))
+        else:
+            mmap.append(M(k=_key, value=''))
+    kv, ref = create_kv_and_ref(id=id,
+                                namespace=ns,
+                                value=Map(ms=mmap))
+    return kv, ref
+
+
 def create_empty_pixels(image, id):
     pix_id = f"Pixels:{str(id)}"
     pixels = Pixels(
         id=pix_id,
         dimension_order=image.pixels.dimension_order,
         size_c=image.pixels.size_c,
         size_t=image.pixels.size_t,
@@ -626,19 +651,19 @@
         add_annotation(img, ann, ome, conn)
     kv, ref = create_provenance_metadata(conn, id, hostname, metadata, False)
     if kv:
         kv_id = f"Annotation:{str(kv.id)}"
         if kv_id not in [i.id for i in ome.structured_annotations]:
             ome.structured_annotations.append(kv)
         if ref:
-            img.annotation_ref.append(ref)
+            img.annotation_refs.append(ref)
     filepath_anns, refs = create_filepath_annotations(img_id, conn)
     for i in range(len(filepath_anns)):
         ome.structured_annotations.append(filepath_anns[i])
-        img.annotation_ref.append(refs[i])
+        img.annotation_refs.append(refs[i])
     roi_service = conn.getRoiService()
     rois = roi_service.findByImage(id, None).rois
     for roi in rois:
         roi_obj = conn.getObject('Roi', roi.getId().getValue())
         roi_ref = populate_roi(roi, roi_obj, ome, conn)
         if not roi_ref:
             continue
@@ -664,15 +689,15 @@
     ds, ds_ref = create_dataset_and_ref(id=id, name=name,
                                         description=desc)
     for ann in obj.listAnnotations():
         add_annotation(ds, ann, ome, conn)
     for img in obj.listChildren():
         img_obj = conn.getObject('Image', img.getId())
         img_ref = populate_image(img_obj, ome, conn, hostname, metadata)
-        ds.image_ref.append(img_ref)
+        ds.image_refs.append(img_ref)
     ds_id = f"Dataset:{str(ds.id)}"
     if ds_id not in [i.id for i in ome.datasets]:
         ome.datasets.append(ds)
     return ds_ref
 
 
 def populate_project(obj: ProjectI, ome: OME, conn: BlitzGateway,
@@ -682,30 +707,30 @@
     desc = obj.getDescription()
     proj, _ = create_proj_and_ref(id=id, name=name, description=desc)
     for ann in obj.listAnnotations():
         add_annotation(proj, ann, ome, conn)
     for ds in obj.listChildren():
         ds_obj = conn.getObject('Dataset', ds.getId())
         ds_ref = populate_dataset(ds_obj, ome, conn, hostname, metadata)
-        proj.dataset_ref.append(ds_ref)
+        proj.dataset_refs.append(ds_ref)
     ome.projects.append(proj)
 
 
 def populate_screen(obj: ScreenI, ome: OME, conn: BlitzGateway,
                     hostname: str, metadata: List[str]):
     id = obj.getId()
     name = obj.getName()
     desc = obj.getDescription()
     scr = create_screen(id=id, name=name, description=desc)
     for ann in obj.listAnnotations():
         add_annotation(scr, ann, ome, conn)
     for pl in obj.listChildren():
         pl_obj = conn.getObject('Plate', pl.getId())
         pl_ref = populate_plate(pl_obj, ome, conn, hostname, metadata)
-        scr.plate_ref.append(pl_ref)
+        scr.plate_refs.append(pl_ref)
     ome.screens.append(scr)
 
 
 def populate_plate(obj: PlateI, ome: OME, conn: BlitzGateway,
                    hostname: str, metadata: List[str]) -> PlateRef:
     id = obj.getId()
     name = obj.getName()
@@ -716,31 +741,31 @@
         add_annotation(pl, ann, ome, conn)
     kv, ref = create_provenance_metadata(conn, id, hostname, metadata, True)
     if kv:
         kv_id = f"Annotation:{str(kv.id)}"
         if kv_id not in [i.id for i in ome.structured_annotations]:
             ome.structured_annotations.append(kv)
         if ref:
-            pl.annotation_ref.append(ref)
+            pl.annotation_refs.append(ref)
     for well in obj.listChildren():
         well_obj = conn.getObject('Well', well.getId())
         well_ref = populate_well(well_obj, ome, conn, hostname, metadata)
         pl.wells.append(well_ref)
-    last_image_anns = ome.images[-1].annotation_ref
+    last_image_anns = ome.images[-1].annotation_refs
     last_image_anns_ids = [i.id for i in last_image_anns]
     for ann in ome.structured_annotations:
         if (ann.id in last_image_anns_ids and
-                type(ann) == CommentAnnotation and
+                isinstance(ann, CommentAnnotation) and
                 int(ann.id.split(":")[-1]) < 0):
             plate_path = ann.value
     filepath_anns, refs = create_filepath_annotations(pl.id, conn,
                                                       plate_path=plate_path)
     for i in range(len(filepath_anns)):
         ome.structured_annotations.append(filepath_anns[i])
-        pl.annotation_ref.append(refs[i])
+        pl.annotation_refs.append(refs[i])
     pl_id = f"Plate:{str(pl.id)}"
     if pl_id not in [i.id for i in ome.plates]:
         ome.plates.append(pl)
     return pl_ref
 
 
 def populate_well(obj: WellI, ome: OME, conn: BlitzGateway,
@@ -780,15 +805,15 @@
             if _value:
                 mmap.append(M(k=_key, value=str(_value)))
             else:
                 mmap.append(M(k=_key, value=''))
         kv, ref = create_kv_and_ref(id=ann.getId(),
                                     namespace=ann.getNs(),
                                     value=Map(
-                                    m=mmap))
+                                    ms=mmap))
         if kv.id not in [i.id for i in ome.structured_annotations]:
             ome.structured_annotations.append(kv)
         obj.annotation_ref.append(ref)
 
     elif ann.OMERO_TYPE == CommentAnnotationI:
         comm, ref = create_comm_and_ref(id=ann.getId(),
                                         value=ann.getTextValue())
@@ -930,18 +955,18 @@
     for ann in ome.structured_annotations:
         if isinstance(ann, CommentAnnotation) and ("comment" not in columns):
             clean_id = int(ann.id.split(":")[-1])
             if clean_id > 0:
                 columns.append("comment")
     anns = ome.structured_annotations
     for i in ome.images:
-        for ann_ref in i.annotation_ref:
+        for ann_ref in i.annotation_refs:
             ann = next(filter(lambda x: x.id == ann_ref.id, anns))
             if isinstance(ann, MapAnnotation):
-                for v in ann.value.m:
+                for v in ann.value.ms:
                     if v.k not in columns:
                         columns.append(v.k)
     return columns
 
 
 def list_files(ome: OME, ids: dict, top_level: str) -> List[str]:
     files = []
@@ -965,15 +990,15 @@
                                      "/" + image_name)
     return files
 
 
 def find_dataset(id: str, ome: OME) -> Union[str, None]:
     for d in ome.datasets:
         def lfunc(x): return x.id == id
-        if any(filter(lfunc, d.image_ref)):
+        if any(filter(lfunc, d.image_refs)):
             return d.name
     return None
 
 
 def generate_lines_and_move(img: Image, ome: OME, ids: dict, folder: str,
                             top_level: str, lines: List[List[str]],
                             columns: List[str]) -> dict:
@@ -1025,15 +1050,15 @@
 
     # return files, lines
     return paths
 
 
 def get_annotation_vals(cols: List[str], img: Image, ome: OME) -> List[str]:
     anns = []
-    for annref in img.annotation_ref:
+    for annref in img.annotation_refs:
         a = next(filter(lambda x: x.id == annref.id,
                  ome.structured_annotations))
         anns.append(a)
     vals = []
     commented = False
     for col in cols:
         if col == "filename" or col == "data_type" \
```

### Comparing `omero-cli-transfer-0.6.0/src/omero/plugins/transfer.py` & `omero-cli-transfer-0.7.0/src/omero/plugins/transfer.py`

 * *Files identical despite different names*

### Comparing `omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/PKG-INFO` & `omero-cli-transfer-0.7.0/src/omero_cli_transfer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-cli-transfer
-Version: 0.6.0
+Version: 0.7.0
 Summary: A set of utilities for exporting a transfer packet from an OMERO server and importing it in a different server. Developed by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/omero-cli-transfer
 Maintainer: Erick Ratamero
 Maintainer-email: erick.ratamero@jax.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -83,14 +83,18 @@
 
 `--ln_s` forces imports to use the transfer=ln_s option, in-place importing files. Same restrictions of regular in-place imports apply.
 
 `--output` allows for specifying an optional output folder where the packet will be unzipped.
 
 `--folder` allows the user to point to a previously-unpacked folder rather than a single file.
 
+`--merge` will use existing Projects, Datasets and Screens if the current user
+already owns entities with the same name as ones defined in `transfer.xml`,
+effectively merging the "new" unpacked entities with existing ones.
+
 Examples:
 ```
 omero transfer unpack transfer_pack.zip
 omero transfer unpack --output /home/user/optional_folder --ln_s
 omero transfer unpack --folder /home/user/unpacked_folder/
 ```
```

### Comparing `omero-cli-transfer-0.6.0/src/omero_cli_transfer.py` & `omero-cli-transfer-0.7.0/src/omero_cli_transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,18 @@
 
 --output allows for specifying an optional output folder where the packet
 will be unzipped.
 
 --folder allows the user to point to a previously-unpacked folder rather than
 a single file.
 
+--merge will use existing Projects, Datasets and Screens if the current user
+already owns entities with the same name as ones defined in `transfer.xml`,
+effectively merging the "new" unpacked entities with existing ones.
+
 --metadata allows you to specify which transfer metadata will be used from
 `transfer.xml` as MapAnnotation values to the images. Fields that do not
 exist on `transfer.xml` will be ignored. Default is `all` (equivalent to
 `img_id timestamp software version hostname md5 orig_user orig_group`), other
 options are `none`, `img_id`, `timestamp`, `software`, `version`, `md5`,
 `hostname`, `db_id`, `orig_user`, `orig_group`.
 
@@ -195,14 +199,17 @@
 
         file_help = ("Path to where the zip file is saved")
         unpack.add_argument("filepath", type=str, help=file_help)
         unpack.add_argument(
                 "--ln_s_import", help="Use in-place import",
                 action="store_true")
         unpack.add_argument(
+                "--merge", help="Use existing entities if possible",
+                action="store_true")
+        unpack.add_argument(
                 "--folder", help="Pass path to a folder rather than a pack",
                 action="store_true")
         unpack.add_argument(
             "--output", type=str, help="Output directory where zip "
                                        "file will be extracted"
         )
         unpack.add_argument(
@@ -380,31 +387,31 @@
         self._process_metadata(args.metadata)
         if not args.folder:
             print(f"Unzipping {args.filepath}...")
             hash, ome, folder = self._load_from_pack(args.filepath,
                                                      args.output)
         else:
             folder = Path(args.filepath)
-            ome = from_xml(folder / "transfer.xml", parser='xmlschema')
+            ome = from_xml(folder / "transfer.xml")
             hash = "imported from folder"
         print("Generating Image mapping and import filelist...")
         ome, src_img_map, filelist = self._create_image_map(ome)
         print("Importing data as orphans...")
         if args.ln_s_import:
             ln_s = True
         else:
             ln_s = False
         dest_img_map = self._import_files(folder, filelist,
                                           ln_s, args.skip, self.gateway)
         self._delete_all_rois(dest_img_map, self.gateway)
         print("Matching source and destination images...")
-        img_map = self._make_image_map(src_img_map, dest_img_map)
+        img_map = self._make_image_map(src_img_map, dest_img_map, self.gateway)
         print("Creating and linking OMERO objects...")
         populate_omero(ome, img_map, self.gateway,
-                       hash, folder, self.metadata)
+                       hash, folder, self.metadata, args.merge)
         return
 
     def _load_from_pack(self, filepath: str, output: Optional[str] = None
                         ) -> Tuple[str, OME, Path]:
         if (not filepath) or (not isinstance(filepath, str)):
             raise TypeError("filepath must be a string")
         if output and not isinstance(output, str):
@@ -429,15 +436,15 @@
                     zipobj.extractall(str(folder))
             elif Path(filepath).suffix == '.tar':
                 shutil.unpack_archive(filepath, str(folder), 'tar')
             else:
                 raise ValueError("File is not a zip or tar file")
         else:
             raise FileNotFoundError("filepath is not a zip file")
-        ome = from_xml(folder / "transfer.xml", parser='xmlschema')
+        ome = from_xml(folder / "transfer.xml")
         return hash, ome, folder
 
     def _create_image_map(self, ome: OME
                           ) -> Tuple[OME, DefaultDict, List[str]]:
         if not (type(ome) is OME):
             raise TypeError("XML is not valid OME format")
         img_map = DefaultDict(list)
@@ -454,17 +461,17 @@
                         ann.namespace.split(":")[-1]))
                     if ann.value.endswith('mock_folder'):
                         filelist.append(ann.value.rstrip("mock_folder"))
                     else:
                         filelist.append(ann.value)
                     newome.structured_annotations.remove(ann)
         for i in newome.images:
-            for ref in i.annotation_ref:
+            for ref in i.annotation_refs:
                 if ref.id in map_ref_ids:
-                    i.annotation_ref.remove(ref)
+                    i.annotation_refs.remove(ref)
         filelist = list(set(filelist))
         img_map = DefaultDict(list, {x: sorted(img_map[x])
                               for x in img_map.keys()})
         return newome, img_map, filelist
 
     def _import_files(self, folder: Path, filelist: List[str], ln_s: bool,
                       skip: str, gateway: BlitzGateway) -> dict:
@@ -528,15 +535,16 @@
                     if ann_content.getNs() == \
                             'openmicroscopy.org/cli/transfer':
                         is_annotated = True
                 if not is_annotated:
                     image_ids.append(img_id)
         return image_ids
 
-    def _make_image_map(self, source_map: dict, dest_map: dict) -> dict:
+    def _make_image_map(self, source_map: dict, dest_map: dict,
+                        conn: Optional[BlitzGateway] = None) -> dict:
         # using both source and destination file-to-image-id maps,
         # map image IDs between source and destination
         src_dict = DefaultDict(list)
         imgmap = {}
         for k, v in source_map.items():
             if k.endswith("mock_folder"):
                 newkey = k.rstrip("mock_folder")
@@ -551,18 +559,32 @@
                                       for x in src_dict.keys()})
         dest_dict = DefaultDict(list, {x: sorted(dest_dict[x])
                                        for x in dest_dict.keys()})
         for src_k in src_dict.keys():
             src_v = src_dict[src_k]
             if src_k in dest_dict.keys():
                 dest_v = dest_dict[src_k]
-                if len(src_v) == len(dest_v):
+                clean_dest = []
+                if not conn:
+                    clean_dest = dest_v
+                else:
+                    for i in dest_v:
+                        img_obj = conn.getObject("Image", i)
+                        anns = 0
+                        for j in img_obj.listAnnotations():
+                            ns = j.getNs()
+                            if ns.startswith(
+                                    "openmicroscopy.org/cli/transfer"):
+                                anns += 1
+                        if not anns:
+                            clean_dest.append(i)
+                if len(src_v) == len(clean_dest):
                     for count in range(len(src_v)):
                         map_key = f"Image:{src_v[count]}"
-                        imgmap[map_key] = dest_v[count]
+                        imgmap[map_key] = clean_dest[count]
         return imgmap
 
     def __prepare(self, args):
         populate_xml_folder(args.folder, args.filelist, self.gateway,
                             self.session)
         return
```

