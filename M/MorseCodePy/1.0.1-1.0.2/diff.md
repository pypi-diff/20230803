# Comparing `tmp/MorseCodePy-1.0.1.tar.gz` & `tmp/MorseCodePy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MorseCodePy-1.0.1.tar", last modified: Wed Aug  2 19:51:12 2023, max compression
+gzip compressed data, was "MorseCodePy-1.0.2.tar", last modified: Thu Aug  3 16:39:28 2023, max compression
```

## Comparing `MorseCodePy-1.0.1.tar` & `MorseCodePy-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-08-02 19:51:12.876990 MorseCodePy-1.0.1/
-drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-08-02 19:51:12.876225 MorseCodePy-1.0.1/MorseCodePy/
--rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     2218 2023-08-02 19:31:31.000000 MorseCodePy-1.0.1/MorseCodePy/MorseCodePy.py
--rwxrwxrwx   0 artemkarpenko   (501) staff       (20)       28 2023-08-01 11:44:30.000000 MorseCodePy-1.0.1/MorseCodePy/__init__.py
-drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-08-02 19:51:12.876683 MorseCodePy-1.0.1/MorseCodePy.egg-info/
--rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     1397 2023-08-02 19:51:12.000000 MorseCodePy-1.0.1/MorseCodePy.egg-info/PKG-INFO
--rwxrwxrwx   0 artemkarpenko   (501) staff       (20)      221 2023-08-02 19:51:12.000000 MorseCodePy-1.0.1/MorseCodePy.egg-info/SOURCES.txt
--rwxrwxrwx   0 artemkarpenko   (501) staff       (20)        1 2023-08-02 19:51:12.000000 MorseCodePy-1.0.1/MorseCodePy.egg-info/dependency_links.txt
--rwxrwxrwx   0 artemkarpenko   (501) staff       (20)       12 2023-08-02 19:51:12.000000 MorseCodePy-1.0.1/MorseCodePy.egg-info/top_level.txt
--rw-r--r--   0 artemkarpenko   (501) staff       (20)     1397 2023-08-02 19:51:12.876873 MorseCodePy-1.0.1/PKG-INFO
--rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     1138 2023-08-02 19:50:24.000000 MorseCodePy-1.0.1/README.md
--rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     1069 2023-08-01 10:56:08.000000 MorseCodePy-1.0.1/license.txt
--rw-r--r--   0 artemkarpenko   (501) staff       (20)       38 2023-08-02 19:51:12.877031 MorseCodePy-1.0.1/setup.cfg
--rwxrwxrwx   0 artemkarpenko   (501) staff       (20)      581 2023-08-02 19:49:56.000000 MorseCodePy-1.0.1/setup.py
+drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-08-03 16:39:28.492844 MorseCodePy-1.0.2/
+drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-08-03 16:39:28.491948 MorseCodePy-1.0.2/MorseCodePy/
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     2644 2023-08-03 10:59:24.000000 MorseCodePy-1.0.2/MorseCodePy/MorseCodePy.py
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)        0 2023-08-02 20:01:10.000000 MorseCodePy-1.0.2/MorseCodePy/__init__.py
+drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-08-03 16:39:28.492481 MorseCodePy-1.0.2/MorseCodePy.egg-info/
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     1586 2023-08-03 16:39:28.000000 MorseCodePy-1.0.2/MorseCodePy.egg-info/PKG-INFO
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)      221 2023-08-03 16:39:28.000000 MorseCodePy-1.0.2/MorseCodePy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)        1 2023-08-03 16:39:28.000000 MorseCodePy-1.0.2/MorseCodePy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)       12 2023-08-03 16:39:28.000000 MorseCodePy-1.0.2/MorseCodePy.egg-info/top_level.txt
+-rw-r--r--   0 artemkarpenko   (501) staff       (20)     1586 2023-08-03 16:39:28.492692 MorseCodePy-1.0.2/PKG-INFO
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     1327 2023-08-03 16:38:00.000000 MorseCodePy-1.0.2/README.md
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     1092 2023-08-02 20:03:50.000000 MorseCodePy-1.0.2/license.txt
+-rw-r--r--   0 artemkarpenko   (501) staff       (20)       38 2023-08-03 16:39:28.492897 MorseCodePy-1.0.2/setup.cfg
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)      584 2023-08-03 16:39:17.000000 MorseCodePy-1.0.2/setup.py
```

### Comparing `MorseCodePy-1.0.1/MorseCodePy.egg-info/PKG-INFO` & `MorseCodePy-1.0.2/MorseCodePy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 Metadata-Version: 2.1
 Name: MorseCodePy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easily translate text into Morse code
 Home-page: https://github.com/CrazyFlyKite/MorseCode
 Author: CrazyFlyKite
 Author-email: karpenkoartem2846@gmail.com
 Description-Content-Type: text/markdown
 
 
-# MorseCodePy 1.0
+# MorseCodePy 1.0.2
 ## Introduction
 MorseCodePy is a module that simplifies the process of translating normal text into **Morse code**. This versatile module supports various languages, including **English**, **Russian**, **Spanish**, **numbers**, **symbols** and **other**.
+
 ## Installation
 
 Installing project using pip:
 
 `pip install MorseCodePy` or `pip3 install MorseCodePy`
     
 ## How to use
-`encode()` returns string with translated into Morse code. "string" is your string, that you want to translate. Also, you can customize `dit` and `dash`.
+`encode(string, dit, dash)` returns string with translated into Morse code. `string` is your text, that you want to translate. Also, you can customise `dit` and `dash`.
 
 `codes` is a dictionary with letters, numbers & symbols and their Morse code translations. **Warning**: translations use 1's and 0's.
 
+`chart(dit, dash)` writes entire dictionary of letters and their Morse codes.
+
 Examples:
 
 ```
-import MorseCodePy as mc
+import MorseCodePy as mcp
 
 string = "SOS"
-t_string = mc.encode(string)
+encode_string = mcp.encode(string)
 
-print(t_string)
+print(encoded_string)
 # Output: ··· --- ···
 ```
 
 ```
-import MorseCodePy as mc
+import MorseCodePy as mcp
 
 string = "Bye!"
-print(mc.encode(string, dit='0', dash='1'))
+print(mcp.encode(string, dit='0', dash='1'))
 # Output: 1000 1011 0 101011
 ```
 
 ```
 from MorseCodePy import codes
 
 print(codes['a'])
 # Output: 01
 ```
+
+```
+import MorseCodePy as mcp
+
+mcp.chart()
+# Output: a: 01 b: 1110 ...
+```
+
 ## Contact
 **GitHub**: https://github.com/CrazyFlyKite
 
 **Email**: karpenkoartem2846@gmail.com
 
 **Discord**: CrazyFlyKite
```

### Comparing `MorseCodePy-1.0.1/PKG-INFO` & `MorseCodePy-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 Metadata-Version: 2.1
 Name: MorseCodePy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easily translate text into Morse code
 Home-page: https://github.com/CrazyFlyKite/MorseCode
 Author: CrazyFlyKite
 Author-email: karpenkoartem2846@gmail.com
 Description-Content-Type: text/markdown
 
 
-# MorseCodePy 1.0
+# MorseCodePy 1.0.2
 ## Introduction
 MorseCodePy is a module that simplifies the process of translating normal text into **Morse code**. This versatile module supports various languages, including **English**, **Russian**, **Spanish**, **numbers**, **symbols** and **other**.
+
 ## Installation
 
 Installing project using pip:
 
 `pip install MorseCodePy` or `pip3 install MorseCodePy`
     
 ## How to use
-`encode()` returns string with translated into Morse code. "string" is your string, that you want to translate. Also, you can customize `dit` and `dash`.
+`encode(string, dit, dash)` returns string with translated into Morse code. `string` is your text, that you want to translate. Also, you can customise `dit` and `dash`.
 
 `codes` is a dictionary with letters, numbers & symbols and their Morse code translations. **Warning**: translations use 1's and 0's.
 
+`chart(dit, dash)` writes entire dictionary of letters and their Morse codes.
+
 Examples:
 
 ```
-import MorseCodePy as mc
+import MorseCodePy as mcp
 
 string = "SOS"
-t_string = mc.encode(string)
+encode_string = mcp.encode(string)
 
-print(t_string)
+print(encoded_string)
 # Output: ··· --- ···
 ```
 
 ```
-import MorseCodePy as mc
+import MorseCodePy as mcp
 
 string = "Bye!"
-print(mc.encode(string, dit='0', dash='1'))
+print(mcp.encode(string, dit='0', dash='1'))
 # Output: 1000 1011 0 101011
 ```
 
 ```
 from MorseCodePy import codes
 
 print(codes['a'])
 # Output: 01
 ```
+
+```
+import MorseCodePy as mcp
+
+mcp.chart()
+# Output: a: 01 b: 1110 ...
+```
+
 ## Contact
 **GitHub**: https://github.com/CrazyFlyKite
 
 **Email**: karpenkoartem2846@gmail.com
 
 **Discord**: CrazyFlyKite
```

### Comparing `MorseCodePy-1.0.1/README.md` & `MorseCodePy-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 
-# MorseCodePy 1.0
+# MorseCodePy 1.0.2
 ## Introduction
 MorseCodePy is a module that simplifies the process of translating normal text into **Morse code**. This versatile module supports various languages, including **English**, **Russian**, **Spanish**, **numbers**, **symbols** and **other**.
+
 ## Installation
 
 Installing project using pip:
 
 `pip install MorseCodePy` or `pip3 install MorseCodePy`
     
 ## How to use
-`encode()` returns string with translated into Morse code. "string" is your string, that you want to translate. Also, you can customize `dit` and `dash`.
+`encode(string, dit, dash)` returns string with translated into Morse code. `string` is your text, that you want to translate. Also, you can customise `dit` and `dash`.
 
 `codes` is a dictionary with letters, numbers & symbols and their Morse code translations. **Warning**: translations use 1's and 0's.
 
+`chart(dit, dash)` writes entire dictionary of letters and their Morse codes.
+
 Examples:
 
 ```
-import MorseCodePy as mc
+import MorseCodePy as mcp
 
 string = "SOS"
-t_string = mc.encode(string)
+encode_string = mcp.encode(string)
 
-print(t_string)
+print(encoded_string)
 # Output: ··· --- ···
 ```
 
 ```
-import MorseCodePy as mc
+import MorseCodePy as mcp
 
 string = "Bye!"
-print(mc.encode(string, dit='0', dash='1'))
+print(mcp.encode(string, dit='0', dash='1'))
 # Output: 1000 1011 0 101011
 ```
 
 ```
 from MorseCodePy import codes
 
 print(codes['a'])
 # Output: 01
 ```
+
+```
+import MorseCodePy as mcp
+
+mcp.chart()
+# Output: a: 01 b: 1110 ...
+```
+
 ## Contact
 **GitHub**: https://github.com/CrazyFlyKite
 
 **Email**: karpenkoartem2846@gmail.com
 
 **Discord**: CrazyFlyKite
```

### Comparing `MorseCodePy-1.0.1/license.txt` & `MorseCodePy-1.0.2/license.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,21 @@
-Copyright 2023 Artem Karpenko
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2023 Artem Karpenko
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `MorseCodePy-1.0.1/setup.py` & `MorseCodePy-1.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import setuptools
+from setuptools import setup
 from pypandoc import convert_file
 
+
 try:
     long_description = convert_file('README.md', 'rst')
-except(IOError, ImportError):
+except (IOError, ImportError):
     long_description = open('README.md').read()
 
-setuptools.setup(
+setup(
     name='MorseCodePy',
     packages=['MorseCodePy'],
-    version='1.0.1',
+    version='1.0.2',
     author='CrazyFlyKite',
     author_email='karpenkoartem2846@gmail.com',
     url='https://github.com/CrazyFlyKite/MorseCode',
     description='Easily translate text into Morse code',
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

