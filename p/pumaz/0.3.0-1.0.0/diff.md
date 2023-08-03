# Comparing `tmp/pumaz-0.3.0.tar.gz` & `tmp/pumaz-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pumaz-0.3.0.tar", last modified: Wed Aug  2 14:18:03 2023, max compression
+gzip compressed data, was "pumaz-1.0.0.tar", last modified: Wed Aug  2 20:01:06 2023, max compression
```

## Comparing `pumaz-0.3.0.tar` & `pumaz-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 x          (501) staff       (20)        0 2023-08-02 14:18:03.538448 pumaz-0.3.0/
--rw-r--r--   0 x          (501) staff       (20)     7084 2023-08-02 14:18:03.538298 pumaz-0.3.0/PKG-INFO
--rw-r--r--   0 x          (501) staff       (20)     5833 2023-08-02 14:13:35.000000 pumaz-0.3.0/README.md
-drwxr-xr-x   0 x          (501) staff       (20)        0 2023-08-02 14:18:03.537282 pumaz-0.3.0/pumaz/
--rw-r--r--   0 x          (501) staff       (20)      305 2023-07-07 10:51:04.000000 pumaz-0.3.0/pumaz/__init__.py
--rw-r--r--   0 x          (501) staff       (20)     2146 2023-08-02 14:13:35.000000 pumaz-0.3.0/pumaz/constants.py
--rw-r--r--   0 x          (501) staff       (20)     3526 2023-07-19 15:20:58.000000 pumaz-0.3.0/pumaz/display.py
--rw-r--r--   0 x          (501) staff       (20)     4197 2023-07-19 15:20:58.000000 pumaz-0.3.0/pumaz/download.py
--rw-r--r--   0 x          (501) staff       (20)     4281 2023-07-19 15:21:10.000000 pumaz-0.3.0/pumaz/file_utilities.py
--rw-r--r--   0 x          (501) staff       (20)     7661 2023-07-19 15:21:11.000000 pumaz-0.3.0/pumaz/image_conversion.py
--rw-r--r--   0 x          (501) staff       (20)    16076 2023-08-02 14:13:35.000000 pumaz-0.3.0/pumaz/image_processing.py
--rw-r--r--   0 x          (501) staff       (20)     2306 2023-07-19 15:20:58.000000 pumaz-0.3.0/pumaz/input_validation.py
--rw-r--r--   0 x          (501) staff       (20)     5295 2023-08-02 14:13:35.000000 pumaz-0.3.0/pumaz/pumaz.py
--rw-r--r--   0 x          (501) staff       (20)     1688 2023-07-07 08:51:22.000000 pumaz-0.3.0/pumaz/resources.py
-drwxr-xr-x   0 x          (501) staff       (20)        0 2023-08-02 14:18:03.538042 pumaz-0.3.0/pumaz.egg-info/
--rw-r--r--   0 x          (501) staff       (20)     7084 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/PKG-INFO
--rw-r--r--   0 x          (501) staff       (20)      402 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/SOURCES.txt
--rw-r--r--   0 x          (501) staff       (20)        1 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/dependency_links.txt
--rw-r--r--   0 x          (501) staff       (20)       44 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/entry_points.txt
--rw-r--r--   0 x          (501) staff       (20)      242 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/requires.txt
--rw-r--r--   0 x          (501) staff       (20)        6 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/top_level.txt
--rw-r--r--   0 x          (501) staff       (20)       38 2023-08-02 14:18:03.538518 pumaz-0.3.0/setup.cfg
--rw-r--r--   0 x          (501) staff       (20)     1996 2023-08-02 14:13:35.000000 pumaz-0.3.0/setup.py
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-08-02 20:01:06.386745 pumaz-1.0.0/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     7086 2023-08-02 20:01:06.386745 pumaz-1.0.0/PKG-INFO
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     5835 2023-08-02 20:00:24.000000 pumaz-1.0.0/README.md
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-08-02 20:01:06.382744 pumaz-1.0.0/pumaz/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      305 2023-07-07 18:44:14.000000 pumaz-1.0.0/pumaz/__init__.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     2146 2023-08-02 18:30:29.000000 pumaz-1.0.0/pumaz/constants.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     3526 2023-07-08 08:44:00.000000 pumaz-1.0.0/pumaz/display.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     4197 2023-07-07 20:08:58.000000 pumaz-1.0.0/pumaz/download.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     4641 2023-08-02 18:30:29.000000 pumaz-1.0.0/pumaz/file_utilities.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     7661 2023-07-27 07:34:55.000000 pumaz-1.0.0/pumaz/image_conversion.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)    17779 2023-08-02 19:20:11.000000 pumaz-1.0.0/pumaz/image_processing.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     2306 2023-07-08 08:25:48.000000 pumaz-1.0.0/pumaz/input_validation.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     5470 2023-08-02 19:58:56.000000 pumaz-1.0.0/pumaz/pumaz.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     1688 2023-07-04 19:36:14.000000 pumaz-1.0.0/pumaz/resources.py
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-08-02 20:01:06.386745 pumaz-1.0.0/pumaz.egg-info/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     7086 2023-08-02 20:01:06.000000 pumaz-1.0.0/pumaz.egg-info/PKG-INFO
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      402 2023-08-02 20:01:06.000000 pumaz-1.0.0/pumaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)        1 2023-08-02 20:01:06.000000 pumaz-1.0.0/pumaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)       44 2023-08-02 20:01:06.000000 pumaz-1.0.0/pumaz.egg-info/entry_points.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      247 2023-08-02 20:01:06.000000 pumaz-1.0.0/pumaz.egg-info/requires.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)        6 2023-08-02 20:01:06.000000 pumaz-1.0.0/pumaz.egg-info/top_level.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)       38 2023-08-02 20:01:06.386745 pumaz-1.0.0/setup.cfg
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     2012 2023-08-02 19:59:49.000000 pumaz-1.0.0/setup.py
```

### Comparing `pumaz-0.3.0/PKG-INFO` & `pumaz-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pumaz
-Version: 0.3.0
+Version: 1.0.0
 Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
 Home-page: https://github.com/QIMP-Team/PUMA
 Author: Sebastian Gutschmayer, Lalith Kumar Shiyam Sundar
 Author-email: Sebastian.Gutschmayer@meduniwien.ac.at, Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
 Platform: UNKNOWN
@@ -145,16 +145,16 @@
 
 Note: All the PET and CT images related to a tracer should be placed in the same directory named after the tracer.
 
 ## To do  🚧
 
 **PUMA v.1.0: August 2023 release candidate**
 
-- [ ] Train moose to remove the CT bed and patient arms, to improve registration accuracy [@Keyn34](https://github.com/Keyn34)
-- [ ] Implement the generated model to puma as a preprocessing step before initiating the alignment [@LalithShiyam](https://github.com/LalithShiyam)
+- [x] Train moose to remove the CT bed and patient arms, to improve registration accuracy [@mprires](https://github.com/mprires)
+- [x] Implement the generated model to puma as a preprocessing step before initiating the alignment [@LalithShiyam](https://github.com/LalithShiyam)
 
 ## A Note on QIMP Python Packages: The 'Z' Factor 📚🚀
 
 All of our Python packages here at QIMP carry a special signature – a distinctive 'Z' at the end of their names. The 'Z' is more than just a letter to us; it's a symbol of our forward-thinking approach and commitment to continuous innovation.
 
 Our PUMA package, for example, is named as 'pumaz', pronounced "puma-see". So, why 'Z'?
```

### Comparing `pumaz-0.3.0/README.md` & `pumaz-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -123,16 +123,16 @@
 
 Note: All the PET and CT images related to a tracer should be placed in the same directory named after the tracer.
 
 ## To do  🚧
 
 **PUMA v.1.0: August 2023 release candidate**
 
-- [ ] Train moose to remove the CT bed and patient arms, to improve registration accuracy [@Keyn34](https://github.com/Keyn34)
-- [ ] Implement the generated model to puma as a preprocessing step before initiating the alignment [@LalithShiyam](https://github.com/LalithShiyam)
+- [x] Train moose to remove the CT bed and patient arms, to improve registration accuracy [@mprires](https://github.com/mprires)
+- [x] Implement the generated model to puma as a preprocessing step before initiating the alignment [@LalithShiyam](https://github.com/LalithShiyam)
 
 ## A Note on QIMP Python Packages: The 'Z' Factor 📚🚀
 
 All of our Python packages here at QIMP carry a special signature – a distinctive 'Z' at the end of their names. The 'Z' is more than just a letter to us; it's a symbol of our forward-thinking approach and commitment to continuous innovation.
 
 Our PUMA package, for example, is named as 'pumaz', pronounced "puma-see". So, why 'Z'?
```

### Comparing `pumaz-0.3.0/pumaz/constants.py` & `pumaz-1.0.0/pumaz/constants.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.3.0/pumaz/display.py` & `pumaz-1.0.0/pumaz/display.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.3.0/pumaz/download.py` & `pumaz-1.0.0/pumaz/download.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.3.0/pumaz/file_utilities.py` & `pumaz-1.0.0/pumaz/file_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,7 +124,19 @@
     for modality in modalities:
         files_to_copy = select_files_by_modality(tracer_dirs, modality)
         copy_files_to_destination(files_to_copy, os.path.join(pumaz_dir, modality))
 
 
 def move_file(file, destination):
     shutil.move(file, destination)
+
+
+def move_files_to_directory(src_dir, dest_dir):
+    src_files = get_files(src_dir, '*')
+    for src_file in src_files:
+        move_file(src_file, os.path.join(dest_dir, os.path.basename(src_file)))
+
+
+def remove_directory(directory_path):
+    # Remove the directory only if it is empty
+    if not os.listdir(directory_path):
+        os.rmdir(directory_path)
```

### Comparing `pumaz-0.3.0/pumaz/image_conversion.py` & `pumaz-1.0.0/pumaz/image_conversion.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.3.0/pumaz/image_processing.py` & `pumaz-1.0.0/pumaz/image_processing.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Description:
 # This module handles image processing for the pumaz.
 #
 # Usage:
 # The functions in this module can be imported and used in other modules within the pumaz to perform image conversion.
 #
 # ----------------------------------------------------------------------------------------------------------------------
-
+import contextlib
 import SimpleITK as sitk
 import numpy as np
 import glob
 from pumaz import constants
 from pumaz.constants import GREEDY_PATH
 from mpire import WorkerPool
 import multiprocessing
@@ -29,17 +29,56 @@
 from concurrent.futures import ThreadPoolExecutor
 import os
 import pathlib
 import subprocess
 import logging
 import sys
 import re
-from rich.progress import track
+from rich.progress import track, Progress
 from moosez import moose
 import nibabel as nib
+from pumaz.file_utilities import create_directory, move_file, remove_directory, move_files_to_directory, get_files
+from halo import Halo
+import time
+
+
+def process_and_moose_ct_files(ct_dir: str, mask_dir: str, moose_model: str, accelerator: str):
+    # Get all ct_files in the ct_dir
+    ct_files = get_files(ct_dir, '*.nii*')
+
+    with Progress() as progress_bar:
+        task = progress_bar.add_task("[cyan] MOOSE-ing CT files...", total=len(ct_files))
+
+        for ct_file in ct_files:
+            base_name = os.path.basename(ct_file).split('.')[0]
+
+            ct_file_dir = os.path.join(ct_dir, base_name)
+            create_directory(ct_file_dir)
+            move_file(ct_file, os.path.join(ct_file_dir, os.path.basename(ct_file)))
+
+            mask_file_dir = os.path.join(mask_dir, base_name)
+            create_directory(mask_file_dir)
+
+            progress_bar.update(task, advance=0, description=f"[cyan] Running MOOSE on {base_name}...")
+
+            with open(os.devnull, 'w') as devnull:
+                with contextlib.redirect_stdout(devnull), contextlib.redirect_stderr(devnull):
+                    moose(moose_model, ct_file_dir, mask_file_dir, accelerator)
+
+            progress_bar.update(task, advance=0, description=f"[cyan] Completed MOOSE on {base_name}, cleaning up...")
+
+            move_files_to_directory(ct_file_dir, ct_dir)
+            move_files_to_directory(mask_file_dir, mask_dir)
+
+            remove_directory(ct_file_dir)
+            remove_directory(mask_file_dir)
+
+            progress_bar.update(task, advance=1, description=f"[cyan] Finished processing {base_name}")
+
+            time.sleep(1)  # delay for 1 second
 
 
 def reslice_identity(reference_image: sitk.Image, moving_image: sitk.Image,
                      output_image_path: str = None, is_label_image: bool = False) -> sitk.Image:
     """
     Reslice an image to the same space as another image
     :param reference_image: The reference image
@@ -75,14 +114,15 @@
             sitk.ReadImage(pt_file[0]),
             sitk.ReadImage(ct_file[0]),
             resliced_ct_file,
             False
         ))
     return tasks
 
+
 def copy_and_rename_file(src, dst, subdir):
     file_utilities.copy_file(src, dst)
     new_file = os.path.join(dst, os.path.basename(subdir) + '_' + os.path.basename(src))
     os.rename(os.path.join(dst, os.path.basename(src)), new_file)
 
 
 def change_mask_labels(mask_file: str, label_map: dict, excluded_labels: list):
@@ -152,15 +192,15 @@
             os.rename(pt_file[0], new_pt_file)
 
             index += 1
             executor.submit(copy_and_rename_file, new_pt_file, pt_dir, subdir)
 
     # Run moosez to get the masks
 
-    moose(constants.MOOSE_MODEL, ct_dir, mask_dir, constants.ACCELERATOR)
+    process_and_moose_ct_files(ct_dir, mask_dir, constants.MOOSE_MODEL, constants.ACCELERATOR)
 
     # remove the prefix from the mask files
 
     for mask_file in glob.glob(os.path.join(mask_dir, constants.MOOSE_PREFIX + '*')):
         new_mask_file = re.sub(rf'{constants.MOOSE_PREFIX}', '', mask_file)
         os.rename(mask_file, new_mask_file)
         change_mask_labels(new_mask_file, constants.MOOSE_LABEL_INDEX, ["Arms"])
@@ -254,15 +294,14 @@
             cmd += f" -ri LABEL 0.2vox -rm {re.escape(segmentation)} {re.escape(resampled_seg)}"
         for transform_file in transform_files:
             cmd += f" -r {re.escape(transform_file)}"
         return cmd
 
 
 def align(puma_working_dir: str, ct_dir: str, pt_dir: str, mask_dir: str):
-
     ct_files = sorted(glob.glob(os.path.join(ct_dir, '*.nii*')))
 
     reference_image = ct_files[0]
     fixed_mask = glob.glob(os.path.join(mask_dir, os.path.basename(reference_image).split('_')[0] + '*.nii*'))[0]
     moving_images = ct_files[1:]
 
     with Progress() as progress:
@@ -318,10 +357,7 @@
         # copy the pet file corresponding to the reference ct file to the aligned_pet_dir and add an aligned prefix
         # to the copied file
         file_utilities.copy_file(
             glob.glob(os.path.join(pt_dir, os.path.basename(reference_image).split('_')[0] + '*.nii*'))[0],
             os.path.join(aligned_pet_dir, constants.ALIGNED_PREFIX +
                          os.path.basename(glob.glob(
                              os.path.join(pt_dir, os.path.basename(reference_image).split('_')[0] + '*.nii*'))[0])))
-
-
-
```

### Comparing `pumaz-0.3.0/pumaz/input_validation.py` & `pumaz-1.0.0/pumaz/input_validation.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.3.0/pumaz/pumaz.py` & `pumaz-1.0.0/pumaz/pumaz.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,9 +125,11 @@
     logging.info(' ')
     puma_dir, ct_dir, pt_dir, mask_dir = image_processing.preprocess(puma_compliant_subjects)
     image_processing.align(puma_dir, ct_dir, pt_dir, mask_dir)
     end_time = time.time()
     elapsed_time = end_time - start_time
     # show elapsed time in minutes and round it to 2 decimal places
     elapsed_time = round(elapsed_time / 60, 2)
-    print(f'{constants.ANSI_GREEN} {emoji.emojize(":hourglass_done:")} Preprocessing and registration complete. Elapsed time: {elapsed_time} minutes!')
+    print(f'{constants.ANSI_GREEN} {emoji.emojize(":hourglass_done:")} Preprocessing and registration complete.'
+          f' Elapsed time: {elapsed_time} minutes! {emoji.emojize(":partying_face:")} Aligned images are stored in'
+          f' {puma_dir}! Look for the directories with prefix "aligned"! {constants.ANSI_RESET}')
```

### Comparing `pumaz-0.3.0/pumaz/resources.py` & `pumaz-1.0.0/pumaz/resources.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.3.0/pumaz.egg-info/PKG-INFO` & `pumaz-1.0.0/pumaz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pumaz
-Version: 0.3.0
+Version: 1.0.0
 Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
 Home-page: https://github.com/QIMP-Team/PUMA
 Author: Sebastian Gutschmayer, Lalith Kumar Shiyam Sundar
 Author-email: Sebastian.Gutschmayer@meduniwien.ac.at, Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
 Platform: UNKNOWN
@@ -145,16 +145,16 @@
 
 Note: All the PET and CT images related to a tracer should be placed in the same directory named after the tracer.
 
 ## To do  🚧
 
 **PUMA v.1.0: August 2023 release candidate**
 
-- [ ] Train moose to remove the CT bed and patient arms, to improve registration accuracy [@Keyn34](https://github.com/Keyn34)
-- [ ] Implement the generated model to puma as a preprocessing step before initiating the alignment [@LalithShiyam](https://github.com/LalithShiyam)
+- [x] Train moose to remove the CT bed and patient arms, to improve registration accuracy [@mprires](https://github.com/mprires)
+- [x] Implement the generated model to puma as a preprocessing step before initiating the alignment [@LalithShiyam](https://github.com/LalithShiyam)
 
 ## A Note on QIMP Python Packages: The 'Z' Factor 📚🚀
 
 All of our Python packages here at QIMP carry a special signature – a distinctive 'Z' at the end of their names. The 'Z' is more than just a letter to us; it's a symbol of our forward-thinking approach and commitment to continuous innovation.
 
 Our PUMA package, for example, is named as 'pumaz', pronounced "puma-see". So, why 'Z'?
```

### Comparing `pumaz-0.3.0/setup.py` & `pumaz-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='pumaz',
-    version='0.3.0',
+    version='1.0.0',
     author='Sebastian Gutschmayer, Lalith Kumar Shiyam Sundar',
     author_email='Sebastian.Gutschmayer@meduniwien.ac.at, Lalith.shiyamsundar@meduniwien.ac.at',
     description='PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.',
     python_requires='>=3.9',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/QIMP-Team/PUMA',
@@ -40,15 +40,16 @@
         'natsort~=8.1.0',
         'pillow>=9.2.0',
         'colorama~=0.4.6',
         'rich',
         'pandas',
         'dicom2nifti~=2.4.8',
         'requests',
-        'moosez'
+        'moosez',
+        'halo'
     ],
     entry_points={
         'console_scripts': [
             'pumaz=pumaz.pumaz:main',
         ],
     },
 )
```

