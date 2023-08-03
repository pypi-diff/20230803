# Comparing `tmp/andak-0.0.1.tar.gz` & `tmp/andak-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andak-0.0.1.tar", last modified: Wed Aug  2 14:28:50 2023, max compression
+gzip compressed data, was "andak-0.0.2.tar", last modified: Thu Aug  3 20:01:32 2023, max compression
```

## Comparing `andak-0.0.1.tar` & `andak-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:28:50.416919 andak-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 14:28:46.000000 andak-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-02 14:28:50.416919 andak-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:28:46.000000 andak-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:28:50.416919 andak-0.0.1/andak/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-08-02 14:28:46.000000 andak-0.0.1/andak/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:28:50.416919 andak-0.0.1/andak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-02 14:28:50.000000 andak-0.0.1/andak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-02 14:28:50.000000 andak-0.0.1/andak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:28:50.000000 andak-0.0.1/andak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:28:50.000000 andak-0.0.1/andak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 14:28:50.000000 andak-0.0.1/andak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:28:50.416919 andak-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3178 2023-08-02 14:28:46.000000 andak-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:01:32.330479 andak-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 20:01:27.000000 andak-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-03 20:01:32.330479 andak-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 20:01:27.000000 andak-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:01:32.326479 andak-0.0.2/andak/
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-08-03 20:01:27.000000 andak-0.0.2/andak/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:01:32.330479 andak-0.0.2/andak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-03 20:01:32.000000 andak-0.0.2/andak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-03 20:01:32.000000 andak-0.0.2/andak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:01:32.000000 andak-0.0.2/andak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 20:01:32.000000 andak-0.0.2/andak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 20:01:32.000000 andak-0.0.2/andak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 20:01:32.330479 andak-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3209 2023-08-03 20:01:27.000000 andak-0.0.2/setup.py
```

### Comparing `andak-0.0.1/LICENSE` & `andak-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `andak-0.0.1/setup.py` & `andak-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -101,15 +101,16 @@
 	python_requires=REQUIRES_PYTHON,
 	url=URL,
 	packages=find_packages(
 		exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
 	entry_points={
 	},
 	install_requires=[
-		"ephfile","hugg", "mystring"
+		"ephfile", "hugg", "mystring", "github-clone"
+		"PyGithub",
 	],
 	include_package_data=True,
 	classifiers=[
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python :: 3.8',
 	],
```

