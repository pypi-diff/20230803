# Comparing `tmp/UzSyllable-0.0.6.tar.gz` & `tmp/UzSyllable-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UzSyllable-0.0.6.tar", last modified: Sun Apr 30 02:11:02 2023, max compression
+gzip compressed data, was "UzSyllable-0.0.7.tar", last modified: Thu Aug  3 06:19:01 2023, max compression
```

## Comparing `UzSyllable-0.0.6.tar` & `UzSyllable-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 02:11:02.044363 UzSyllable-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-04-12 11:44:40.000000 UzSyllable-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3404 2023-04-30 02:11:02.044363 UzSyllable-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2023-04-30 02:06:10.000000 UzSyllable-0.0.6/README.md
--rw-rw-rw-   0        0        0       86 2023-04-12 11:44:40.000000 UzSyllable-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 02:11:02.044363 UzSyllable-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1110 2023-04-30 02:07:12.000000 UzSyllable-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 02:11:01.983869 UzSyllable-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 02:11:02.037676 UzSyllable-0.0.6/src/UzSyllable/
--rw-rw-rw-   0        0        0     4683 2023-04-28 05:09:12.000000 UzSyllable-0.0.6/src/UzSyllable/UzSyllable.py
--rw-rw-rw-   0        0        0      104 2023-04-28 05:00:03.000000 UzSyllable-0.0.6/src/UzSyllable/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 02:11:02.044363 UzSyllable-0.0.6/src/UzSyllable.egg-info/
--rw-rw-rw-   0        0        0     3404 2023-04-30 02:11:01.000000 UzSyllable-0.0.6/src/UzSyllable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-30 02:11:01.000000 UzSyllable-0.0.6/src/UzSyllable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 02:11:01.000000 UzSyllable-0.0.6/src/UzSyllable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-30 02:11:01.000000 UzSyllable-0.0.6/src/UzSyllable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 06:19:01.507027 UzSyllable-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-08-03 06:03:16.000000 UzSyllable-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4193 2023-08-03 06:19:01.506238 UzSyllable-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3565 2023-08-03 06:03:16.000000 UzSyllable-0.0.7/README.md
+-rw-rw-rw-   0        0        0       86 2023-08-03 06:03:16.000000 UzSyllable-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 06:19:01.507027 UzSyllable-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-08-03 06:16:32.000000 UzSyllable-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 06:19:01.480686 UzSyllable-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 06:19:01.487591 UzSyllable-0.0.7/src/UzSyllable/
+-rw-rw-rw-   0        0        0     4840 2023-08-03 06:14:05.000000 UzSyllable-0.0.7/src/UzSyllable/UzSyllable.py
+-rw-rw-rw-   0        0        0      105 2023-08-03 06:03:16.000000 UzSyllable-0.0.7/src/UzSyllable/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 06:19:01.500472 UzSyllable-0.0.7/src/UzSyllable.egg-info/
+-rw-rw-rw-   0        0        0     4193 2023-08-03 06:19:01.000000 UzSyllable-0.0.7/src/UzSyllable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-08-03 06:19:01.000000 UzSyllable-0.0.7/src/UzSyllable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 06:19:01.000000 UzSyllable-0.0.7/src/UzSyllable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 06:19:01.000000 UzSyllable-0.0.7/src/UzSyllable.egg-info/top_level.txt
```

### Comparing `UzSyllable-0.0.6/LICENSE` & `UzSyllable-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `UzSyllable-0.0.6/PKG-INFO` & `UzSyllable-0.0.7/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: UzSyllable
-Version: 0.0.6
-Summary: UzSyllable | The Syllable Separator, Line breaks and Counter for Uzbek Language
-Home-page: https://github.com/UlugbekSalaev/UzSyllable
-Author: Ulugbek Salaev
-Author-email: ulugbek0302@gmail.com
-Project-URL: Bug Tracker, https://github.com/UlugbekSalaev/UzSyllable/issues
-Keywords: syllable,line-break,uzbek-language
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # UzSyllable
 
 https://pypi.org/project/UzSyllable <br>
 https://github.com/UlugbekSalaev/UzSyllable
 
 UzSyllable tool is focused to make division of syllables and end of line breaks of Uzbek language. The tool includes Syllabification, End-of-Line, Count of Syllables methods.
 It is created as a python library and uploaded to [PyPI](https://pypi.org/). It is simply easy to use in your python project or other programming language projects via the API. 
@@ -26,59 +10,98 @@
 The UzSyllable project is a text processing tool that includes three main methods: syllabification, end-of-line, and count of syllables. Syllabification involves dividing words in Uzbek text into their constituent syllables, which can be useful for pronunciation, spelling, and linguistic analysis. End-of-line justification involves determining the appropriate places to break lines in Uzbek text, which can improve the readability and aesthetics of written materials. Count of syllables involves counting the number of syllables in a given word or sentence, which can be useful for metrics such as rhyme and meter in poetry or for determining the complexity of a text. The UzSyllable project uses machine learning algorithms and linguistic rules to perform these methods accurately and efficiently on Uzbek text.
 ## Quick links
 
 - [Github](https://github.com/UlugbekSalaev/UzSyllable)
 - [PyPI](https://pypi.org/project/UzSyllable/)
 - [Web-UI](https://nlp.urdu.uz/?menu=uzsyllable)
 
-## Demo
-
-You can use [web interface](http://nlp.urdu.uz/?menu=uzsyllable).
 
 ## Features
 
 - Syllabification
-- End-of-Line
+- Hyphenation
 - Count of Syllables
 
 ## Usage
 
-Two options to run UzSyllable:
+Three options to use UzSyllable:
 
 - pip
-- Web interface
+- Web tool
+- API
 
-### pip installation
+## pip installation
 
 To install UzSyllable, simply run:
 
 ```code
 pip install UzSyllable
 ```
 
 After installation, use in python like following:
-```yml
-import UzSyllable
-# call syllables method
-print(UzSyllable.syllables('maktabimda'))
+
+### Syllabification
+```code
+from UzSyllable import syllables
+print(syllables('maktabimda'))
 # Output : ['mak-ta-bim-da']
-print(UzSyllable.syllables('мактабимда'))
+
+print(syllables('мактабимда'))
 # Output : ['мак-та-бим-да']
-# call end-of-line method
-print(UzSyllable.line_break('maktabimda'))
+```
+
+### Hyphenation
+```code
+from UzSyllable import hyphenation
+# call hyphenation method
+print(hyphenation('maktabimda'))
 # Output : ['mak-tabimda', 'makta-bimda', 'maktabim-da']
+```
+
+### Count of Syllables
+```code
+from UzSyllable import count
 # call count of syllables method
-print(UzSyllable.count('maktabimda'))
+print(count('maktabimda'))
 # Output : 4
 ```
 
 
-## Documentation
+## Web interface
+
+You can use [web interface](https://nlp.urdu.uz/?menu=uzsyllable).
+
+<img width="1437" alt="image" src="https://github.com/UlugbekSalaev/UzSyllable/assets/71002671/ee3bc563-35d8-4d15-bcd0-6cbad8a6107a">
+
+
+## API
+
+### Syllabification
+
+- #### URL: https://api.urdu.uz/syllables
+- #### Method: POST
+- #### Parametres: word
+- #### Example Request: https://api.urdu.uz/syllables?word=maktab
+
+
+### Hyphenation
+
+- #### URL: https://api.urdu.uz/line-break-syllables
+- #### Method: POST
+- #### Parametres: word
+- #### Example Request: https://api.urdu.uz/line-break-syllables?word=maktabgacha
+
+
+### Count of Syllables
+
+- #### URL: https://api.urdu.uz/count-syllables
+- #### Method: POST
+- #### Parametres: word
+- #### Example Request: https://api.urdu.uz/count-syllables?word=maktabgacha
 
-See [here](https://github.com/UlugbekSalaev/UzSyllable).
 
 ## Citation
 
 ```tex
 @misc{UzSyllable,
   title={UzSyllable}: Syllabification Tool for Uzbek},
   url={https://github.com/UlugbekSalaev/UzSyllable},
```

### Comparing `UzSyllable-0.0.6/setup.py` & `UzSyllable-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="UzSyllable",
-    version="0.0.6",
+    version="0.0.7",
     author="Ulugbek Salaev",
     author_email="ulugbek0302@gmail.com",
     description="UzSyllable | The Syllable Separator, Line breaks and Counter for Uzbek Language",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UlugbekSalaev/UzSyllable",
     project_urls={
         "Bug Tracker": "https://github.com/UlugbekSalaev/UzSyllable/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    keywords=['syllable', 'line-break', 'uzbek-language'],
+    keywords=['syllable', 'hyphenation', 'uzbek-language'],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     install_requires=[],
     python_requires=">=3.6",
     include_package_data=True,
     #package_data={"": ["*.csv"]},
     #package_data={"": ["cyr_exwords.csv", "lat_exwords.csv"],},
```

### Comparing `UzSyllable-0.0.6/src/UzSyllable/UzSyllable.py` & `UzSyllable-0.0.7/src/UzSyllable/UzSyllable.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,46 +86,48 @@
                 str += w
                 if not w.__contains__('-'):
                     str += '-'
         sylls.append(str[0:len(str)-1])
     return sylls
 def processing(text):
     text = str(text)
+    text = text.replace("`", "'")
     text = text.replace("O'", "O‘").replace("o'", "o‘").replace("G'", "G‘").replace("g'", "g‘").replace("'", "’")
-    tokens = text.split()
-    return tokens
-def line_break(text):
+    return text.split()
+def hyphenation(text):
     word = text
     syllable = ' '.join(syllables(text))
     begin = end = ''
     if word.__contains__('-'):
         for i in range(0, len(word)):
             if word[i] == '-':
                 begin = word[i - 1]
                 end = word[i + 1]
     lines = list()
     if not syllable.__contains__('-'):
         lines.append(syllable)
     tokens = syllable.split('-')
     count = len(tokens) - 1
     for j in range(1, len(tokens)):
-        w = ''
-        for i in range(0, j):
-            w += tokens[i]
-        if len(tokens[j - 1]) != 1 and not tokens[j - 1].__contains__(chr(8217)):
-            w += '-'
-        for i in range(j, len(tokens)):
-            w += tokens[i]
-        if begin != end != '':
-            for i in range(0, len(w) - 1):
-                if w[i] == begin and w[i + 1] == end:
-                    w = w[0:i + 1] + '-' + w[i + 1:len(w)]
-                    break
-        if w != word or count == 1 or word.__contains__('-') and w not in lines:
-            lines.append(w)
+        if len(tokens[j]) != 1:
+            w = ''
+            for i in range(0, j):
+                w += tokens[i]
+            if len(tokens[j - 1]) != 1 and not tokens[j - 1].__contains__(chr(8217)):
+                w += '-'
+            for i in range(j, len(tokens)):
+                if len(tokens[i]):
+                    w += tokens[i]
+            if begin != end != '' and len(end):
+                for i in range(0, len(w) - 1):
+                    if w[i] == begin and w[i + 1] == end:
+                        w = w[0:i + 1] + '-' + w[i + 1:len(w)]
+                        break
+            if w != word or count == 1 or word.__contains__('-') and w not in lines:
+                lines.append(w)
     return lines
 def count(text):
     tokens = syllables(text)
     count = 0
     for token in tokens:
         syll = token.split('-')
         count += len(syll)
```

### Comparing `UzSyllable-0.0.6/src/UzSyllable.egg-info/PKG-INFO` & `UzSyllable-0.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: UzSyllable
-Version: 0.0.6
+Version: 0.0.7
 Summary: UzSyllable | The Syllable Separator, Line breaks and Counter for Uzbek Language
 Home-page: https://github.com/UlugbekSalaev/UzSyllable
 Author: Ulugbek Salaev
 Author-email: ulugbek0302@gmail.com
 Project-URL: Bug Tracker, https://github.com/UlugbekSalaev/UzSyllable/issues
-Keywords: syllable,line-break,uzbek-language
+Keywords: syllable,hyphenation,uzbek-language
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -26,59 +26,98 @@
 The UzSyllable project is a text processing tool that includes three main methods: syllabification, end-of-line, and count of syllables. Syllabification involves dividing words in Uzbek text into their constituent syllables, which can be useful for pronunciation, spelling, and linguistic analysis. End-of-line justification involves determining the appropriate places to break lines in Uzbek text, which can improve the readability and aesthetics of written materials. Count of syllables involves counting the number of syllables in a given word or sentence, which can be useful for metrics such as rhyme and meter in poetry or for determining the complexity of a text. The UzSyllable project uses machine learning algorithms and linguistic rules to perform these methods accurately and efficiently on Uzbek text.
 ## Quick links
 
 - [Github](https://github.com/UlugbekSalaev/UzSyllable)
 - [PyPI](https://pypi.org/project/UzSyllable/)
 - [Web-UI](https://nlp.urdu.uz/?menu=uzsyllable)
 
-## Demo
-
-You can use [web interface](http://nlp.urdu.uz/?menu=uzsyllable).
 
 ## Features
 
 - Syllabification
-- End-of-Line
+- Hyphenation
 - Count of Syllables
 
 ## Usage
 
-Two options to run UzSyllable:
+Three options to use UzSyllable:
 
 - pip
-- Web interface
+- Web tool
+- API
 
-### pip installation
+## pip installation
 
 To install UzSyllable, simply run:
 
 ```code
 pip install UzSyllable
 ```
 
 After installation, use in python like following:
-```yml
-import UzSyllable
-# call syllables method
-print(UzSyllable.syllables('maktabimda'))
+
+### Syllabification
+```code
+from UzSyllable import syllables
+print(syllables('maktabimda'))
 # Output : ['mak-ta-bim-da']
-print(UzSyllable.syllables('мактабимда'))
+
+print(syllables('мактабимда'))
 # Output : ['мак-та-бим-да']
-# call end-of-line method
-print(UzSyllable.line_break('maktabimda'))
+```
+
+### Hyphenation
+```code
+from UzSyllable import hyphenation
+# call hyphenation method
+print(hyphenation('maktabimda'))
 # Output : ['mak-tabimda', 'makta-bimda', 'maktabim-da']
+```
+
+### Count of Syllables
+```code
+from UzSyllable import count
 # call count of syllables method
-print(UzSyllable.count('maktabimda'))
+print(count('maktabimda'))
 # Output : 4
 ```
 
 
-## Documentation
+## Web interface
+
+You can use [web interface](https://nlp.urdu.uz/?menu=uzsyllable).
+
+<img width="1437" alt="image" src="https://github.com/UlugbekSalaev/UzSyllable/assets/71002671/ee3bc563-35d8-4d15-bcd0-6cbad8a6107a">
+
+
+## API
+
+### Syllabification
+
+- #### URL: https://api.urdu.uz/syllables
+- #### Method: POST
+- #### Parametres: word
+- #### Example Request: https://api.urdu.uz/syllables?word=maktab
+
+
+### Hyphenation
+
+- #### URL: https://api.urdu.uz/line-break-syllables
+- #### Method: POST
+- #### Parametres: word
+- #### Example Request: https://api.urdu.uz/line-break-syllables?word=maktabgacha
+
+
+### Count of Syllables
+
+- #### URL: https://api.urdu.uz/count-syllables
+- #### Method: POST
+- #### Parametres: word
+- #### Example Request: https://api.urdu.uz/count-syllables?word=maktabgacha
 
-See [here](https://github.com/UlugbekSalaev/UzSyllable).
 
 ## Citation
 
 ```tex
 @misc{UzSyllable,
   title={UzSyllable}: Syllabification Tool for Uzbek},
   url={https://github.com/UlugbekSalaev/UzSyllable},
```

