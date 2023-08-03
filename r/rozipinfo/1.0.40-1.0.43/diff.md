# Comparing `tmp/rozipinfo-1.0.40.tar.gz` & `tmp/rozipinfo-1.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rozipinfo-1.0.40.tar", last modified: Fri Jul 21 22:58:46 2023, max compression
+gzip compressed data, was "dist/rozipinfo-1.0.43.tar", last modified: Thu Aug  3 17:50:39 2023, max compression
```

## Comparing `rozipinfo-1.0.40.tar` & `rozipinfo-1.0.43.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 charles    (502) staff       (20)        0 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/
--rw-rw-r--   0 charles    (502) staff       (20)     6939 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/PKG-INFO
--rw-rw-r--   0 charles    (502) staff       (20)    54448 2023-04-02 13:38:30.000000 rozipinfo-1.0.40/rozipinfo.py
--rwxrwxr-x   0 charles    (502) staff       (20)    20344 2023-07-21 22:43:48.000000 rozipinfo-1.0.40/rozipfile.py
--rw-rw-r--   0 charles    (502) staff       (20)     5239 2023-04-02 13:37:16.000000 rozipinfo-1.0.40/README.md
--rwxrwxr-x   0 charles    (502) staff       (20)     1584 2023-07-21 22:58:45.000000 rozipinfo-1.0.40/setup.py
--rw-rw-r--   0 charles    (502) staff       (20)       38 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/setup.cfg
-drwxrwxr-x   0 charles    (502) staff       (20)        0 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/rozipinfo.egg-info/
--rw-rw-r--   0 charles    (502) staff       (20)     6939 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/rozipinfo.egg-info/PKG-INFO
--rw-rw-r--   0 charles    (502) staff       (20)      176 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/rozipinfo.egg-info/SOURCES.txt
--rw-rw-r--   0 charles    (502) staff       (20)       20 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/rozipinfo.egg-info/top_level.txt
--rw-rw-r--   0 charles    (502) staff       (20)        1 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/rozipinfo.egg-info/dependency_links.txt
+drwxrwxr-x   0 charles    (502) staff       (20)        0 2023-08-03 17:50:39.000000 rozipinfo-1.0.43/
+-rw-rw-r--   0 charles    (502) staff       (20)     6939 2023-08-03 17:50:39.000000 rozipinfo-1.0.43/PKG-INFO
+-rw-rw-r--   0 charles    (502) staff       (20)    54837 2023-08-03 17:45:25.000000 rozipinfo-1.0.43/rozipinfo.py
+-rwxrwxr-x   0 charles    (502) staff       (20)    20613 2023-08-03 17:34:51.000000 rozipinfo-1.0.43/rozipfile.py
+-rw-rw-r--   0 charles    (502) staff       (20)     5239 2022-08-17 07:46:02.000000 rozipinfo-1.0.43/README.md
+-rwxrwxr-x   0 charles    (502) staff       (20)     1584 2023-08-03 17:50:38.000000 rozipinfo-1.0.43/setup.py
+-rw-rw-r--   0 charles    (502) staff       (20)       38 2023-08-03 17:50:39.000000 rozipinfo-1.0.43/setup.cfg
+drwxrwxr-x   0 charles    (502) staff       (20)        0 2023-08-03 17:50:39.000000 rozipinfo-1.0.43/rozipinfo.egg-info/
+-rw-rw-r--   0 charles    (502) staff       (20)     6939 2023-08-03 17:50:39.000000 rozipinfo-1.0.43/rozipinfo.egg-info/PKG-INFO
+-rw-rw-r--   0 charles    (502) staff       (20)      176 2023-08-03 17:50:39.000000 rozipinfo-1.0.43/rozipinfo.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles    (502) staff       (20)       20 2023-08-03 17:50:39.000000 rozipinfo-1.0.43/rozipinfo.egg-info/top_level.txt
+-rw-rw-r--   0 charles    (502) staff       (20)        1 2023-08-03 17:50:39.000000 rozipinfo-1.0.43/rozipinfo.egg-info/dependency_links.txt
```

### Comparing `rozipinfo-1.0.40/PKG-INFO` & `rozipinfo-1.0.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rozipinfo
-Version: 1.0.40
+Version: 1.0.43
 Summary: Managing Zip archives with RISC OS filetype information present
 Home-page: https://github.com/gerph/python-zipinfo-riscos
 Author: Charles Ferguson
 Author-email: gerph@gerph.org
 License: BSD
 Description: # Python ZipInfo processing for RISC OS archives
```

### Comparing `rozipinfo-1.0.40/rozipinfo.py` & `rozipinfo-1.0.43/rozipinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,17 @@
     header_id_riscos = 0x4341
     header_id_riscos_spark = 0x30435241
 
     # Filetype to use when none is known, and when the file is marked as text
     default_filetype = 0xFFD
     default_filetype_text = 0xFFF
 
+    # Whether we force files with no RISC OS information to have a default filetype
+    force_riscos_filetype = False
+
     # Filetype to use for the directory in the API, and in the loadaddr
     directory_filetype = 0x1000
     directory_filetype_internal = 0xFFD
 
     # Encoding to use for riscos_filename
     # For use in a wider environment, consider using riscos-latin1 from the python-codecs-riscos module.
     filename_encoding_name = 'latin-1'
@@ -389,14 +392,17 @@
 
             # Some archive tools have written the filename ending in a '/' but not marked the
             # file as being a directory. This causes problems when we try to extract because we
             # create a 0 length file, which then cannot be a directory.
             if self.filename.endswith('/'):
                 self.external_attr |= self.external_attr_msdos_directory
 
+            if self.force_riscos_filetype and self._riscos_filetype is None:
+                self.riscos_filetype = self.riscos_filetype
+
         self._nfs_encoding = nfs_encoding
         self.create_system = 13  # RISC OS
 
     def __repr__(self):
         try:
             ro_load = '&{:08x}({})'.format(self.riscos_loadaddr, 'inferred' if self._riscos_loadaddr is None else 'set')
             ro_exec = '&{:08x}({})'.format(self.riscos_execaddr, 'inferred' if self._riscos_execaddr is None else 'set')
@@ -1304,11 +1310,14 @@
         zinfo.external_attr = (st.st_mode & 0xFFFF) << 16  # Unix attributes
         if isdir:
             zinfo.file_size = 0
             zinfo.external_attr |= 0x10  # MS-DOS directory flag
         else:
             zinfo.file_size = st.st_size
 
+        if cls.force_riscos_filetype and zinfo._riscos_filetype is None:
+            zinfo.riscos_filetype = zinfo.riscos_filetype
+
         # Finally set the encoding to the format requested, so that we get the encoding
         # format they want to use.
         zinfo.nfs_encoding = nfs_encoding
         return zinfo
```

### Comparing `rozipinfo-1.0.40/rozipfile.py` & `rozipinfo-1.0.43/rozipfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,21 +62,28 @@
             0xFDC: 'SoftLink',
             0xFD3: 'DebImage',
             0xFCA: 'Squash',
             0xFC9: 'SunRastr',
             0xFAF: 'HTML',
             0xFAE: 'Resource',
             0xF89: 'GZip',
+            0xF81: 'JS',
+            0xF80: 'XML',
+            0xF7F: 'XML_DTD',
+            0xF7E: 'XSL',
+            0xF75: 'JSON',
+            0xF74: 'YAML',
             0xD94: 'ArtWork',
             0xC85: 'JPEG',
             0xBBC: 'BBC ROM',
             0xB61: 'XBM',
             0xB60: 'PNG',
             0xB2F: 'WMF',
             0xAFF: 'DrawFile',
+            0xAAD: 'SVG',
             0xA91: 'Zip',
             0xA66: 'WebP',
             0xA65: 'JPEG2000',
             0x69E: 'PNM',
             0x69D: 'Targa',
             0x69C: 'BMP',
             0x697: 'PCX',
@@ -108,15 +115,18 @@
                     default_filetype = file_type
                 except ValueError:
                     raise RISCOSZipFileError("Unrecognised default filetype '{}'".format(default_filetype))
         self.default_filetype = default_filetype
 
         if self.default_filetype:
             class ZipInfoRISCOSCustom(self.cls_zipinfo):
-                pass
+
+                # Force the use of the default filetype
+                force_riscos_filetype = True
+
             ZipInfoRISCOSCustom.default_filetype = default_filetype
             self.cls_zipinfo = ZipInfoRISCOSCustom
 
         self.base_dir = os.path.abspath(base_dir)
         self._fileslist = None
         self._namesdict = None
```

### Comparing `rozipinfo-1.0.40/README.md` & `rozipinfo-1.0.43/README.md`

 * *Files identical despite different names*

### Comparing `rozipinfo-1.0.40/setup.py` & `rozipinfo-1.0.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name = 'rozipinfo',
     py_modules = ['rozipfile', 'rozipinfo'],
-    version = '1.0.40',
+    version = '1.0.43',
     license='BSD',
     description = 'Managing Zip archives with RISC OS filetype information present',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author = 'Charles Ferguson',
     author_email = 'gerph@gerph.org',
     url = 'https://github.com/gerph/python-zipinfo-riscos',
```

### Comparing `rozipinfo-1.0.40/rozipinfo.egg-info/PKG-INFO` & `rozipinfo-1.0.43/rozipinfo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rozipinfo
-Version: 1.0.40
+Version: 1.0.43
 Summary: Managing Zip archives with RISC OS filetype information present
 Home-page: https://github.com/gerph/python-zipinfo-riscos
 Author: Charles Ferguson
 Author-email: gerph@gerph.org
 License: BSD
 Description: # Python ZipInfo processing for RISC OS archives
```

