# Comparing `tmp/facit-0.1.5.tar.gz` & `tmp/facit-0.2.0.tar.gz`

## Comparing `facit-0.1.5.tar` & `facit-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,24 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 facit-0.1.5/.DS_Store
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 facit-0.1.5/CITATION.cff
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 facit-0.1.5/.github/workflows/main.yml
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 facit-0.1.5/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facit-0.1.5/src/pangolin/__init__.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 facit-0.1.5/src/pangolin/_pyinstaller_hooks/__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 facit-0.1.5/src/pangolin/_pyinstaller_hooks/stdhooks/hook-OCP.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 facit-0.1.5/src/pangolin/_pyinstaller_hooks/stdhooks/hook-cadquery.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 facit-0.1.5/src/pangolin/_pyinstaller_hooks/stdhooks/hook-openmdao.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 facit-0.1.5/src/pangolin/_pyinstaller_hooks/stdhooks/hook-vtk.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 facit-0.1.5/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 facit-0.1.5/LICENSE
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 facit-0.1.5/README.md
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 facit-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 facit-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 facit-0.2.0/CITATION.cff
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 facit-0.2.0/noxfile.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/__init__.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/components.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/constants.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/io.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/modelling.py
+-rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/processing.py
+-rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/recording.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/_pyinstaller_hooks/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/_pyinstaller_hooks/conftest.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/_pyinstaller_hooks/stdhooks/hook-OCP.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/_pyinstaller_hooks/stdhooks/hook-cadquery.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/_pyinstaller_hooks/stdhooks/hook-openmdao.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 facit-0.2.0/src/facit/_pyinstaller_hooks/stdhooks/hook-vtk.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 facit-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 facit-0.2.0/tests/test_modelling.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 facit-0.2.0/tests/test_recording.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 facit-0.2.0/tests/test_smoke.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 facit-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 facit-0.2.0/LICENSE
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 facit-0.2.0/README.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 facit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 facit-0.2.0/PKG-INFO
```

### Comparing `facit-0.1.5/LICENSE` & `facit-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (C) 2022-2023 Olle Vidner
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Copyright (C) 2022-2023 Olle Vidner
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

