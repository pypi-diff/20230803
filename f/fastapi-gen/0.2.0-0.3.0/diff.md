# Comparing `tmp/fastapi_gen-0.2.0.tar.gz` & `tmp/fastapi_gen-0.3.0.tar.gz`

## Comparing `fastapi_gen-0.2.0.tar` & `fastapi_gen-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,33 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/cli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/cli/__init__.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/cli/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/__init__.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/hello_world/.gitignore
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/hello_world/Makefile
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/hello_world/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/hello_world/__init__.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/hello_world/main.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/hello_world/requirements.txt
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/hello_world/test_main.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/nlp/.env_dev
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/nlp/.gitignore
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/nlp/Makefile
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/nlp/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/nlp/__init__.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/nlp/main.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/nlp/requirements.txt
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/src/templates/nlp/test_main.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/LICENSE
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/README.md
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 fastapi_gen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/cli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/cli/__init__.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/cli/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/__init__.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/.gitignore
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/__init__.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/main.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/requirements.txt
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/test_main.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/.env_dev
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/.gitignore
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/__init__.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/main.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/requirements.txt
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/test_main.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/.env_dev
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/.gitignore
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/__init__.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/main.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/requirements.txt
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/test_main.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/README.md
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/PKG-INFO
```

### Comparing `fastapi_gen-0.2.0/src/cli/__main__.py` & `fastapi_gen-0.3.0/src/cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import re
 import subprocess
 import sys
 from importlib import resources
 
 import click
-
 from cli.__about__ import __version__
 
 _pattern = r"^[a-zA-Z0-9_]+$"
 
 
 def is_valid_name(name) -> bool:
     return re.match(_pattern, name) is not None
@@ -21,16 +20,19 @@
 
     modified_content = content.replace(old_string, new_string)
 
     with open(file_path, "w") as file:
         file.write(modified_content)
 
 
+_choices = ["hello_world", "nlp", "langchain"]
+
+
 @click.command()
-@click.option("-t", "--template", default="hello_world", type=click.Choice(["hello_world", "nlp"]), help="template")
+@click.option("-t", "--template", default="hello_world", type=click.Choice(_choices), help="template")
 @click.argument("name")
 @click.version_option(version=__version__, prog_name="create-fast-api")
 def fastapi_create(name: str, template: str):
     """This script creates new FastAPI project with NAME using TEMPLATE."""
     if not is_valid_name(name):
         click.echo(f"Error. Invalid name {name}. Name contain only: {_pattern}")
         sys.exit(1)
```

### Comparing `fastapi_gen-0.2.0/src/templates/hello_world/.gitignore` & `fastapi_gen-0.3.0/src/templates/hello_world/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.2.0/src/templates/hello_world/README.md` & `fastapi_gen-0.3.0/src/templates/hello_world/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.2.0/src/templates/hello_world/main.py` & `fastapi_gen-0.3.0/src/templates/hello_world/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.2.0/src/templates/hello_world/test_main.py` & `fastapi_gen-0.3.0/src/templates/hello_world/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.2.0/src/templates/nlp/.gitignore` & `fastapi_gen-0.3.0/src/templates/langchain/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.2.0/src/templates/nlp/README.md` & `fastapi_gen-0.3.0/src/templates/langchain/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.2.0/src/templates/nlp/main.py` & `fastapi_gen-0.3.0/src/templates/nlp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-import os
-
 from fastapi import FastAPI, HTTPException
 from pydantic_settings import BaseSettings, SettingsConfigDict
 from transformers import pipeline
 
 
 class Settings(BaseSettings):
     model_config = SettingsConfigDict(
         # `.env.prod` takes priority over `.env_dev`
-        env_file=(".env_dev", ".env.prod")
+        env_file=(".env_dev", ".env.prod"),
     )
     summarize_model: str
     ner_model: str
     text_generation_model: str
     text_generation_temperature: float
     text_generation_do_sample: bool
 
@@ -35,16 +33,14 @@
     result[0]["original_text"] = text
 
     return {"summary_text": result[0]["summary_text"], "original_text": text}
 
 
 @app.get("/ner")
 def ner(text: str | None = None):
-    os.environ["TOKENIZERS_PARALLELISM"] = "false"
-
     if text is None:
         raise HTTPException(status_code=400, detail="Text must be specified.")
 
     text = text.strip()
 
     nlp = pipeline("ner", model=settings.ner_model, aggregation_strategy="simple")
     result = nlp(text)
@@ -62,14 +58,15 @@
 def text_generation(text: str | None = None):
     if text is None:
         raise HTTPException(status_code=400, detail="Text must be specified.")
 
     text = text.strip()
 
     text_generator = pipeline(
-        model="gpt2",
+        task="text-generation",
+        model=settings.text_generation_model,
         do_sample=settings.text_generation_do_sample,
         model_kwargs={"temperature": settings.text_generation_temperature},
     )
     result = text_generator(text)
 
     return {"generated_text": result[0]["generated_text"], "original_text": text}
```

### Comparing `fastapi_gen-0.2.0/src/templates/nlp/test_main.py` & `fastapi_gen-0.3.0/src/templates/nlp/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
 Charting a world map requires global knowledge of the earth, its oceans, and its continents. From prehistory through the Middle ages, creating an accurate world map would have been impossible because less than half of Earth's coastlines and only a small fraction of its continental interiors were known to any culture. With exploration that began during the European Renaissance, knowledge of the Earth's surface accumulated rapidly, such that most of the world's coastlines had been mapped, at least roughly, by the mid-1700s and the continental interiors by the twentieth century.
 """
     response = client.get(f"/summarize?text={urllib.parse.quote(text)}")
 
     assert response.is_success
     assert (
-        # ruff: disable=E501
         response.json()["summary_text"]
         == "maps rendered in two dimensions by necessity distort the display of the three-dimensional surface of the earth . this is true of any map, but these distortions reach extremes in a world map . from prehistory through the Middle ages, creating an accurate world map would have been impossible ."
     )
 
 
 def test_ner_400():
     response = client.get("/ner")
```

### Comparing `fastapi_gen-0.2.0/.gitignore` & `fastapi_gen-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.2.0/LICENSE` & `fastapi_gen-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.2.0/README.md` & `fastapi_gen-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,207 @@
 00000000: 2320 4661 7374 4170 6920 4765 6e0a 0a43  # FastApi Gen..C
 00000010: 7265 6174 6520 4661 7374 4150 4920 6170  reate FastAPI ap
 00000020: 7073 2077 6974 6820 6e6f 2062 7569 6c64  ps with no build
 00000030: 2063 6f6e 6669 6775 7261 7469 6f6e 2e0a   configuration..
-00000040: 0a46 6173 7441 7069 2047 656e 2077 6f72  .FastApi Gen wor
-00000050: 6b73 206f 6e20 6d61 634f 5320 616e 6420  ks on macOS and 
-00000060: 4c69 6e75 782e 3c62 723e 0a49 6620 736f  Linux.<br>.If so
-00000070: 6d65 7468 696e 6720 646f 6573 6ee2 8099  mething doesn...
-00000080: 7420 776f 726b 2c20 706c 6561 7365 205b  t work, please [
-00000090: 6669 6c65 2061 6e20 6973 7375 655d 2868  file an issue](h
-000000a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000000b0: 6d2f 6d69 7270 6f2f 6661 7374 6170 692d  m/mirpo/fastapi-
-000000c0: 6765 6e2f 6973 7375 6573 2f6e 6577 292e  gen/issues/new).
-000000d0: 0a0a 4176 6169 6c61 626c 6520 7465 6d70  ..Available temp
-000000e0: 6c61 7465 733a 0a0a 312e 2044 6566 6175  lates:..1. Defau
-000000f0: 6c74 202d 2062 6173 6963 2074 656d 706c  lt - basic templ
-00000100: 6174 6520 7769 7468 2047 4554 2f50 4f53  ate with GET/POS
-00000110: 5420 6578 616d 706c 6573 2e0a 322e 204e  T examples..2. N
-00000120: 6c70 202d 206e 6174 7572 616c 206c 616e  lp - natural lan
-00000130: 6775 6167 6520 7072 6f63 6573 7369 6e67  guage processing
-00000140: 2074 656d 706c 6174 6520 7769 7468 2065   template with e
-00000150: 7861 6d70 6c65 7320 686f 7720 746f 2075  xamples how to u
-00000160: 7365 2048 7567 6769 6e66 6163 6520 7375  se Hugginface su
-00000170: 6d6d 6172 697a 6174 696f 6e2c 206e 616d  mmarization, nam
-00000180: 6564 2d65 6e74 6974 7920 7265 636f 676e  ed-entity recogn
-00000190: 6974 696f 6e20 616e 6420 7465 7874 2067  ition and text g
-000001a0: 656e 6572 6174 696f 6e20 7573 696e 6720  eneration using 
-000001b0: 4c4c 4d2e 0a0a 4d6f 7265 2074 6f20 636f  LLM...More to co
-000001c0: 6d65 210a 0a23 2320 5175 6963 6b20 4f76  me!..## Quick Ov
-000001d0: 6572 7669 6577 0a0a 6060 6063 6f6e 736f  erview..```conso
-000001e0: 6c65 0a70 6970 3320 696e 7374 616c 6c20  le.pip3 install 
-000001f0: 6661 7374 6170 692d 6765 6e0a 6661 7374  fastapi-gen.fast
-00000200: 6170 692d 6765 6e20 6d79 5f61 7070 0a63  api-gen my_app.c
-00000210: 6420 6d79 5f61 7070 0a6d 616b 6520 7374  d my_app.make st
-00000220: 6172 742d 6465 760a 6060 600a 0a6f 7220  art-dev.```..or 
-00000230: 0a0a 6060 6063 6f6e 736f 6c65 0a70 6970  ..```console.pip
-00000240: 7820 7275 6e20 6661 7374 6170 692d 6765  x run fastapi-ge
-00000250: 6e20 6d79 5f61 7070 0a63 6420 6d79 5f61  n my_app.cd my_a
-00000260: 7070 0a6d 616b 6520 7374 6172 742d 6465  pp.make start-de
-00000270: 760a 6060 600a 0a49 6620 796f 7527 7665  v.```..If you've
-00000280: 2070 7265 7669 6f75 736c 7920 696e 7374   previously inst
-00000290: 616c 6c65 6420 6066 6173 7461 7069 2d67  alled `fastapi-g
-000002a0: 656e 6020 676c 6f62 616c 6c79 2076 6961  en` globally via
-000002b0: 2060 7069 7033 2069 6e73 7461 6c6c 2066   `pip3 install f
-000002c0: 6173 7461 7069 2d67 656e 602c 2077 6520  astapi-gen`, we 
-000002d0: 7265 636f 6d6d 656e 6420 796f 7520 7265  recommend you re
-000002e0: 696e 7374 616c 6c20 7468 6520 7061 636b  install the pack
-000002f0: 6167 6520 7573 696e 6720 6070 6970 3320  age using `pip3 
-00000300: 696e 7374 616c 6c20 2d2d 7570 6772 6164  install --upgrad
-00000310: 6520 2d2d 666f 7263 652d 7265 696e 7374  e --force-reinst
-00000320: 616c 6c20 6661 7374 6170 692d 6765 6e60  all fastapi-gen`
-00000330: 206f 7220 6070 6970 7820 7570 6772 6164   or `pipx upgrad
-00000340: 6520 6661 7374 6170 692d 6765 6e60 2074  e fastapi-gen` t
-00000350: 6f20 656e 7375 7265 2074 6861 7420 796f  o ensure that yo
-00000360: 7520 7573 6520 7468 6520 6c61 7465 7374  u use the latest
-00000370: 2076 6572 7369 6f6e 2e0a 0a54 6865 6e20   version...Then 
-00000380: 6f70 656e 2068 7474 703a 2f2f 6c6f 6361  open http://loca
-00000390: 6c68 6f73 743a 3830 3030 2f64 6f63 7320  lhost:8000/docs 
-000003a0: 746f 2073 6565 2079 6f75 7220 6170 7020  to see your app 
-000003b0: 4f70 656e 4150 4920 646f 6375 6d65 6e74  OpenAPI document
-000003c0: 6174 696f 6e2e 0a0a 2323 2320 4765 7420  ation...### Get 
-000003d0: 5374 6172 7465 6420 496d 6d65 6469 6174  Started Immediat
-000003e0: 656c 790a 0a59 6f75 202a 2a64 6f6e e280  ely..You **don..
-000003f0: 9974 2a2a 206e 6565 6420 746f 2069 6e73  .t** need to ins
-00000400: 7461 6c6c 206f 7220 636f 6e66 6967 7572  tall or configur
-00000410: 6520 6465 7065 6e63 656e 6465 6963 6573  e depencendeices
-00000420: 206c 696b 6520 4661 7374 4170 6920 6f72   like FastApi or
-00000430: 2050 7974 6573 742e 3c62 723e 0a54 6865   Pytest.<br>.The
-00000440: 7920 6172 6520 7072 6563 6f6e 6669 6775  y are preconfigu
-00000450: 7265 6420 616e 6420 6869 6464 656e 2073  red and hidden s
-00000460: 6f20 7468 6174 2079 6f75 2063 616e 2066  o that you can f
-00000470: 6f63 7573 206f 6e20 7468 6520 636f 6465  ocus on the code
-00000480: 2e0a 0a43 7265 6174 6520 6120 7072 6f6a  ...Create a proj
-00000490: 6563 742c 2061 6e64 2079 6f75 e280 9972  ect, and you...r
-000004a0: 6520 676f 6f64 2074 6f20 676f 2e0a 0a23  e good to go...#
-000004b0: 2320 4372 6561 7469 6e67 2061 6e20 4170  # Creating an Ap
-000004c0: 700a 0a2a 2a59 6f75 e280 996c 6c20 6e65  p..**You...ll ne
-000004d0: 6564 2074 6f20 6861 7665 2050 7974 686f  ed to have Pytho
-000004e0: 6e20 332e 372b 206f 7220 6c61 7465 7220  n 3.7+ or later 
-000004f0: 7665 7273 696f 6e20 6f6e 2079 6f75 7220  version on your 
-00000500: 6c6f 6361 6c20 6465 7665 6c6f 706d 656e  local developmen
-00000510: 7420 6d61 6368 696e 652a 2a2e 2057 6520  t machine**. We 
-00000520: 7265 636f 6d6d 656e 6420 7573 696e 6720  recommend using 
-00000530: 7468 6520 6c61 7465 7374 204c 5453 2076  the latest LTS v
-00000540: 6572 7369 6f6e 2e20 596f 7520 6361 6e20  ersion. You can 
-00000550: 7573 6520 5b70 7965 6e76 5d28 6874 7470  use [pyenv](http
-00000560: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00000570: 7965 6e76 2f70 7965 6e76 2920 286d 6163  yenv/pyenv) (mac
-00000580: 4f53 2f4c 696e 7578 2920 746f 2073 7769  OS/Linux) to swi
-00000590: 7463 6820 5079 7468 6f6e 2076 6572 7369  tch Python versi
-000005a0: 6f6e 7320 6265 7477 6565 6e20 6469 6666  ons between diff
-000005b0: 6572 656e 7420 7072 6f6a 6563 7473 2e0a  erent projects..
-000005c0: 0a23 2323 2062 6173 6963 2074 656d 706c  .### basic templ
-000005d0: 6174 650a 0a60 6060 636f 6e73 6f6c 650a  ate..```console.
-000005e0: 7069 7033 2069 6e73 7461 6c6c 2066 6173  pip3 install fas
-000005f0: 7461 7069 2d67 656e 0a66 6173 7461 7069  tapi-gen.fastapi
-00000600: 2d67 656e 206d 795f 6170 700a 6060 600a  -gen my_app.```.
-00000610: 0a6f 720a 0a60 6060 636f 6e73 6f6c 650a  .or..```console.
-00000620: 7069 7033 2069 6e73 7461 6c6c 2066 6173  pip3 install fas
-00000630: 7461 7069 2d67 656e 0a66 6173 7461 7069  tapi-gen.fastapi
-00000640: 2d67 656e 206d 795f 6170 7020 2d2d 7465  -gen my_app --te
-00000650: 6d70 6c61 7465 2068 656c 6c6f 5f77 6f72  mplate hello_wor
-00000660: 6c64 0a60 6060 0a0a 2323 2320 4e4c 5020  ld.```..### NLP 
-00000670: 7465 6d70 6c61 7465 0a0a 6060 6063 6f6e  template..```con
-00000680: 736f 6c65 0a70 6970 2069 6e73 7461 6c6c  sole.pip install
-00000690: 2066 6173 7461 7069 2d67 656e 0a66 6173   fastapi-gen.fas
-000006a0: 7461 7069 2d67 656e 206d 795f 6170 7020  tapi-gen my_app 
-000006b0: 2d2d 7465 6d70 6c61 7465 206e 6c70 0a60  --template nlp.`
-000006c0: 6060 0a0a 496e 7369 6465 2074 6865 206e  ``..Inside the n
-000006d0: 6577 6c79 2063 7265 6174 6564 2070 726f  ewly created pro
-000006e0: 6a65 6374 2c20 796f 7520 6361 6e20 7275  ject, you can ru
-000006f0: 6e20 736f 6d65 2062 7569 6c74 2d69 6e20  n some built-in 
-00000700: 636f 6d6d 616e 6473 3a0a 0a23 2323 2060  commands:..### `
-00000710: 6d61 6b65 2073 7461 7274 600a 0a52 756e  make start`..Run
-00000720: 7320 7468 6520 6170 7020 696e 2064 6576  s the app in dev
-00000730: 656c 6f70 6d65 6e74 206d 6f64 652e 3c62  elopment mode.<b
-00000740: 723e 0a4f 7065 6e20 5b68 7474 703a 2f2f  r>.Open [http://
-00000750: 6c6f 6361 6c68 6f73 743a 3830 3030 2f64  localhost:8000/d
-00000760: 6f63 735d 2868 7474 703a 2f2f 6c6f 6361  ocs](http://loca
-00000770: 6c68 6f73 743a 3830 3030 2f64 6f63 7329  lhost:8000/docs)
-00000780: 2074 6f20 7669 6577 204f 7065 6e41 5049   to view OpenAPI
-00000790: 2064 6f63 756d 656e 7461 7469 6f6e 2069   documentation i
-000007a0: 6e20 7468 6520 6272 6f77 7365 722e 0a0a  n the browser...
-000007b0: 5468 6520 7061 6765 2077 696c 6c20 6175  The page will au
-000007c0: 746f 6d61 7469 6361 6c6c 7920 7265 6c6f  tomatically relo
-000007d0: 6164 2069 6620 796f 7520 6d61 6b65 2063  ad if you make c
-000007e0: 6861 6e67 6573 2074 6f20 7468 6520 636f  hanges to the co
-000007f0: 6465 2e0a 0a23 2323 2060 6d61 6b65 2074  de...### `make t
-00000800: 6573 7460 0a0a 5275 6e73 2074 6573 7473  est`..Runs tests
-00000810: 2e3c 6272 3e0a 4279 2064 6566 6175 6c74  .<br>.By default
-00000820: 2c20 7275 6e73 2074 6573 7473 2072 656c  , runs tests rel
-00000830: 6174 6564 2074 6f20 6669 6c65 7320 6368  ated to files ch
-00000840: 616e 6765 6420 7369 6e63 6520 7468 6520  anged since the 
-00000850: 6c61 7374 2063 6f6d 6d69 742e 0a0a 2323  last commit...##
-00000860: 204c 6963 656e 7365 0a0a 6066 6173 7461   License..`fasta
-00000870: 7069 2d67 656e 6020 6973 2064 6973 7472  pi-gen` is distr
-00000880: 6962 7574 6564 2075 6e64 6572 2074 6865  ibuted under the
-00000890: 2074 6572 6d73 206f 6620 7468 6520 5b4d   terms of the [M
-000008a0: 4954 5d28 6874 7470 733a 2f2f 6769 7468  IT](https://gith
-000008b0: 7562 2e63 6f6d 2f6d 6972 706f 2f66 6173  ub.com/mirpo/fas
-000008c0: 7461 7069 2d67 656e 2f62 6c6f 622f 6d61  tapi-gen/blob/ma
-000008d0: 7374 6572 2f4c 4943 454e 5345 2920 6c69  ster/LICENSE) li
-000008e0: 6365 6e73 652e 0a                        cense..
+00000040: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000050: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6972  //github.com/mir
+00000060: 706f 2f66 6173 7461 7069 2d67 656e 2f61  po/fastapi-gen/a
+00000070: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000080: 2f74 6573 742e 796d 6c3f 7175 6572 793d  /test.yml?query=
+00000090: 776f 726b 666c 6f77 2533 4174 6573 742b  workflow%3Atest+
+000000a0: 6576 656e 7425 3341 7075 7368 2b62 7261  event%3Apush+bra
+000000b0: 6e63 6825 3341 6d61 7374 6572 2220 7461  nch%3Amaster" ta
+000000c0: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
+000000d0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+000000e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000000f0: 6d69 7270 6f2f 6661 7374 6170 692d 6765  mirpo/fastapi-ge
+00000100: 6e2f 6163 7469 6f6e 732f 776f 726b 666c  n/actions/workfl
+00000110: 6f77 732f 7465 7374 2e79 6d6c 2f62 6164  ows/test.yml/bad
+00000120: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
+00000130: 7374 6572 2220 616c 743d 2254 6573 7422  ster" alt="Test"
+00000140: 3e0a 3c2f 613e 0a3c 6120 6872 6566 3d22  >.</a>.<a href="
+00000150: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000160: 2f70 726f 6a65 6374 2f66 6173 7461 7069  /project/fastapi
+00000170: 2d67 656e 2220 7461 7267 6574 3d22 5f62  -gen" target="_b
+00000180: 6c61 6e6b 223e 0a20 2020 203c 696d 6720  lank">.    <img 
+00000190: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000001a0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+000001b0: 2f76 2f66 6173 7461 7069 2d67 656e 3f63  /v/fastapi-gen?c
+000001c0: 6f6c 6f72 3d25 3233 3334 4430 3538 266c  olor=%2334D058&l
+000001d0: 6162 656c 3d70 7970 6925 3230 7061 636b  abel=pypi%20pack
+000001e0: 6167 6522 2061 6c74 3d22 5061 636b 6167  age" alt="Packag
+000001f0: 6520 7665 7273 696f 6e22 3e0a 3c2f 613e  e version">.</a>
+00000200: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000210: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000220: 6374 2f66 6173 7461 7069 2d67 656e 2220  ct/fastapi-gen" 
+00000230: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00000240: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000250: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000260: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
+00000270: 7369 6f6e 732f 6661 7374 6170 692d 6765  sions/fastapi-ge
+00000280: 6e2e 7376 673f 636f 6c6f 723d 2532 3333  n.svg?color=%233
+00000290: 3444 3035 3822 2061 6c74 3d22 5375 7070  4D058" alt="Supp
+000002a0: 6f72 7465 6420 5079 7468 6f6e 2076 6572  orted Python ver
+000002b0: 7369 6f6e 7322 3e0a 3c2f 613e 0a0a 2d2d  sions">.</a>..--
+000002c0: 2d0a 0a46 6173 7441 7069 2047 656e 2077  -..FastApi Gen w
+000002d0: 6f72 6b73 206f 6e20 6d61 634f 5320 616e  orks on macOS an
+000002e0: 6420 4c69 6e75 782e 3c62 723e 0a49 6620  d Linux.<br>.If 
+000002f0: 736f 6d65 7468 696e 6720 646f 6573 6ee2  something doesn.
+00000300: 8099 7420 776f 726b 2c20 706c 6561 7365  ..t work, please
+00000310: 205b 6669 6c65 2061 6e20 6973 7375 655d   [file an issue]
+00000320: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000330: 636f 6d2f 6d69 7270 6f2f 6661 7374 6170  com/mirpo/fastap
+00000340: 692d 6765 6e2f 6973 7375 6573 2f6e 6577  i-gen/issues/new
+00000350: 292e 0a0a 4176 6169 6c61 626c 6520 7465  )...Available te
+00000360: 6d70 6c61 7465 733a 0a0a 312e 2044 6566  mplates:..1. Def
+00000370: 6175 6c74 202d 2062 6173 6963 2074 656d  ault - basic tem
+00000380: 706c 6174 6520 7769 7468 2047 4554 2f50  plate with GET/P
+00000390: 4f53 5420 6578 616d 706c 6573 2e0a 322e  OST examples..2.
+000003a0: 204e 4c50 202d 206e 6174 7572 616c 206c   NLP - natural l
+000003b0: 616e 6775 6167 6520 7072 6f63 6573 7369  anguage processi
+000003c0: 6e67 2074 656d 706c 6174 6520 7769 7468  ng template with
+000003d0: 2065 7861 6d70 6c65 7320 686f 7720 746f   examples how to
+000003e0: 2075 7365 206c 6f63 616c 2048 7567 6769   use local Huggi
+000003f0: 6e66 6163 6520 6d6f 6465 6c73 2066 6f72  nface models for
+00000400: 2073 756d 6d61 7269 7a61 7469 6f6e 2c20   summarization, 
+00000410: 6e61 6d65 642d 656e 7469 7479 2072 6563  named-entity rec
+00000420: 6f67 6e69 7469 6f6e 2061 6e64 2074 6578  ognition and tex
+00000430: 7420 6765 6e65 7261 7469 6f6e 2075 7369  t generation usi
+00000440: 6e67 204c 4c4d 2e0a 332e 204c 616e 6763  ng LLM..3. Langc
+00000450: 6861 696e 202d 2074 656d 706c 6174 6520  hain - template 
+00000460: 7769 7468 2065 7861 6d70 6c65 7320 686f  with examples ho
+00000470: 7720 746f 2075 7365 204c 616e 6743 6861  w to use LangCha
+00000480: 696e 2077 6974 6820 6c6f 6361 6c20 4875  in with local Hu
+00000490: 6767 696e 6661 6365 206d 6f64 656c 7320  gginface models 
+000004a0: 284c 4c4d 7329 2066 6f72 2074 6578 7420  (LLMs) for text 
+000004b0: 6765 6e65 7261 7469 6f6e 2061 6e64 2071  generation and q
+000004c0: 7565 7374 696f 6e20 616e 7377 6572 696e  uestion answerin
+000004d0: 672e 0a0a 2a49 6d70 6f72 7461 6e74 206e  g...*Important n
+000004e0: 6f74 652a 202d 204c 616e 6763 6861 696e  ote* - Langchain
+000004f0: 2074 656d 706c 6174 6520 7265 7175 6972   template requir
+00000500: 6573 2068 6172 6477 6172 6520 746f 2072  es hardware to r
+00000510: 756e 2061 6e64 2077 696c 6c20 6175 746f  un and will auto
+00000520: 6d61 7469 6361 6c6c 7920 646f 776e 6c6f  matically downlo
+00000530: 6164 2072 6571 7569 7265 6420 6d6f 6465  ad required mode
+00000540: 6c73 2c20 6265 2070 6174 6965 6e74 2e0a  ls, be patient..
+00000550: 0a4d 6f72 6520 746f 2063 6f6d 6521 0a0a  .More to come!..
+00000560: 2323 2051 7569 636b 204f 7665 7276 6965  ## Quick Overvie
+00000570: 770a 0a60 6060 636f 6e73 6f6c 650a 7069  w..```console.pi
+00000580: 7033 2069 6e73 7461 6c6c 2066 6173 7461  p3 install fasta
+00000590: 7069 2d67 656e 0a66 6173 7461 7069 2d67  pi-gen.fastapi-g
+000005a0: 656e 206d 795f 6170 700a 6364 206d 795f  en my_app.cd my_
+000005b0: 6170 700a 6d61 6b65 2073 7461 7274 2d64  app.make start-d
+000005c0: 6576 0a60 6060 0a0a 6f72 200a 0a60 6060  ev.```..or ..```
+000005d0: 636f 6e73 6f6c 650a 7069 7078 2072 756e  console.pipx run
+000005e0: 2066 6173 7461 7069 2d67 656e 206d 795f   fastapi-gen my_
+000005f0: 6170 700a 6364 206d 795f 6170 700a 6d61  app.cd my_app.ma
+00000600: 6b65 2073 7461 7274 2d64 6576 0a60 6060  ke start-dev.```
+00000610: 0a0a 4966 2079 6f75 2776 6520 7072 6576  ..If you've prev
+00000620: 696f 7573 6c79 2069 6e73 7461 6c6c 6564  iously installed
+00000630: 2060 6661 7374 6170 692d 6765 6e60 2067   `fastapi-gen` g
+00000640: 6c6f 6261 6c6c 7920 7669 6120 6070 6970  lobally via `pip
+00000650: 3320 696e 7374 616c 6c20 6661 7374 6170  3 install fastap
+00000660: 692d 6765 6e60 2c20 7765 2072 6563 6f6d  i-gen`, we recom
+00000670: 6d65 6e64 2079 6f75 2072 6569 6e73 7461  mend you reinsta
+00000680: 6c6c 2074 6865 2070 6163 6b61 6765 2075  ll the package u
+00000690: 7369 6e67 2060 7069 7033 2069 6e73 7461  sing `pip3 insta
+000006a0: 6c6c 202d 2d75 7067 7261 6465 202d 2d66  ll --upgrade --f
+000006b0: 6f72 6365 2d72 6569 6e73 7461 6c6c 2066  orce-reinstall f
+000006c0: 6173 7461 7069 2d67 656e 6020 6f72 2060  astapi-gen` or `
+000006d0: 7069 7078 2075 7067 7261 6465 2066 6173  pipx upgrade fas
+000006e0: 7461 7069 2d67 656e 6020 746f 2065 6e73  tapi-gen` to ens
+000006f0: 7572 6520 7468 6174 2079 6f75 2075 7365  ure that you use
+00000700: 2074 6865 206c 6174 6573 7420 7665 7273   the latest vers
+00000710: 696f 6e2e 0a0a 5468 656e 206f 7065 6e20  ion...Then open 
+00000720: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+00000730: 3a38 3030 302f 646f 6373 2074 6f20 7365  :8000/docs to se
+00000740: 6520 796f 7572 2061 7070 204f 7065 6e41  e your app OpenA
+00000750: 5049 2064 6f63 756d 656e 7461 7469 6f6e  PI documentation
+00000760: 2e0a 0a23 2323 2047 6574 2053 7461 7274  ...### Get Start
+00000770: 6564 2049 6d6d 6564 6961 7465 6c79 0a0a  ed Immediately..
+00000780: 596f 7520 2a2a 646f 6ee2 8099 742a 2a20  You **don...t** 
+00000790: 6e65 6564 2074 6f20 696e 7374 616c 6c20  need to install 
+000007a0: 6f72 2063 6f6e 6669 6775 7265 2064 6570  or configure dep
+000007b0: 656e 6365 6e64 6569 6365 7320 6c69 6b65  encendeices like
+000007c0: 2046 6173 7441 7069 206f 7220 5079 7465   FastApi or Pyte
+000007d0: 7374 2e3c 6272 3e0a 5468 6579 2061 7265  st.<br>.They are
+000007e0: 2070 7265 636f 6e66 6967 7572 6564 2061   preconfigured a
+000007f0: 6e64 2068 6964 6465 6e20 736f 2074 6861  nd hidden so tha
+00000800: 7420 796f 7520 6361 6e20 666f 6375 7320  t you can focus 
+00000810: 6f6e 2074 6865 2063 6f64 652e 0a0a 4372  on the code...Cr
+00000820: 6561 7465 2061 2070 726f 6a65 6374 2c20  eate a project, 
+00000830: 616e 6420 796f 75e2 8099 7265 2067 6f6f  and you...re goo
+00000840: 6420 746f 2067 6f2e 0a0a 2323 2043 7265  d to go...## Cre
+00000850: 6174 696e 6720 616e 2041 7070 0a0a 2a2a  ating an App..**
+00000860: 596f 75e2 8099 6c6c 206e 6565 6420 746f  You...ll need to
+00000870: 2068 6176 6520 5079 7468 6f6e 2033 2e37   have Python 3.7
+00000880: 2b20 6f72 206c 6174 6572 2076 6572 7369  + or later versi
+00000890: 6f6e 206f 6e20 796f 7572 206c 6f63 616c  on on your local
+000008a0: 2064 6576 656c 6f70 6d65 6e74 206d 6163   development mac
+000008b0: 6869 6e65 2a2a 2e20 5765 2072 6563 6f6d  hine**. We recom
+000008c0: 6d65 6e64 2075 7369 6e67 2074 6865 206c  mend using the l
+000008d0: 6174 6573 7420 4c54 5320 7665 7273 696f  atest LTS versio
+000008e0: 6e2e 2059 6f75 2063 616e 2075 7365 205b  n. You can use [
+000008f0: 7079 656e 765d 2868 7474 7073 3a2f 2f67  pyenv](https://g
+00000900: 6974 6875 622e 636f 6d2f 7079 656e 762f  ithub.com/pyenv/
+00000910: 7079 656e 7629 2028 6d61 634f 532f 4c69  pyenv) (macOS/Li
+00000920: 6e75 7829 2074 6f20 7377 6974 6368 2050  nux) to switch P
+00000930: 7974 686f 6e20 7665 7273 696f 6e73 2062  ython versions b
+00000940: 6574 7765 656e 2064 6966 6665 7265 6e74  etween different
+00000950: 2070 726f 6a65 6374 732e 0a0a 2323 2320   projects...### 
+00000960: 6261 7369 6320 7465 6d70 6c61 7465 0a0a  basic template..
+00000970: 6060 6063 6f6e 736f 6c65 0a70 6970 3320  ```console.pip3 
+00000980: 696e 7374 616c 6c20 6661 7374 6170 692d  install fastapi-
+00000990: 6765 6e0a 6661 7374 6170 692d 6765 6e20  gen.fastapi-gen 
+000009a0: 6d79 5f61 7070 0a60 6060 0a0a 6f72 0a0a  my_app.```..or..
+000009b0: 6060 6063 6f6e 736f 6c65 0a70 6970 3320  ```console.pip3 
+000009c0: 696e 7374 616c 6c20 6661 7374 6170 692d  install fastapi-
+000009d0: 6765 6e0a 6661 7374 6170 692d 6765 6e20  gen.fastapi-gen 
+000009e0: 6d79 5f61 7070 202d 2d74 656d 706c 6174  my_app --templat
+000009f0: 6520 6865 6c6c 6f5f 776f 726c 640a 6060  e hello_world.``
+00000a00: 600a 0a23 2323 204e 4c50 2074 656d 706c  `..### NLP templ
+00000a10: 6174 650a 0a60 6060 636f 6e73 6f6c 650a  ate..```console.
+00000a20: 7069 7020 696e 7374 616c 6c20 6661 7374  pip install fast
+00000a30: 6170 692d 6765 6e0a 6661 7374 6170 692d  api-gen.fastapi-
+00000a40: 6765 6e20 6d79 5f61 7070 202d 2d74 656d  gen my_app --tem
+00000a50: 706c 6174 6520 6e6c 700a 6060 600a 0a23  plate nlp.```..#
+00000a60: 2323 204c 616e 6763 6861 696e 2074 656d  ## Langchain tem
+00000a70: 706c 6174 650a 0a60 6060 636f 6e73 6f6c  plate..```consol
+00000a80: 650a 7069 7020 696e 7374 616c 6c20 6661  e.pip install fa
+00000a90: 7374 6170 692d 6765 6e0a 6661 7374 6170  stapi-gen.fastap
+00000aa0: 692d 6765 6e20 6d79 5f61 7070 202d 2d74  i-gen my_app --t
+00000ab0: 656d 706c 6174 6520 4c61 6e67 6368 6169  emplate Langchai
+00000ac0: 6e0a 6060 600a 0a49 6e73 6964 6520 7468  n.```..Inside th
+00000ad0: 6520 6e65 776c 7920 6372 6561 7465 6420  e newly created 
+00000ae0: 7072 6f6a 6563 742c 2079 6f75 2063 616e  project, you can
+00000af0: 2072 756e 2073 6f6d 6520 6275 696c 742d   run some built-
+00000b00: 696e 2063 6f6d 6d61 6e64 733a 0a0a 2323  in commands:..##
+00000b10: 2320 606d 616b 6520 7374 6172 7460 0a0a  # `make start`..
+00000b20: 5275 6e73 2074 6865 2061 7070 2069 6e20  Runs the app in 
+00000b30: 6465 7665 6c6f 706d 656e 7420 6d6f 6465  development mode
+00000b40: 2e3c 6272 3e0a 4f70 656e 205b 6874 7470  .<br>.Open [http
+00000b50: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3030  ://localhost:800
+00000b60: 302f 646f 6373 5d28 6874 7470 3a2f 2f6c  0/docs](http://l
+00000b70: 6f63 616c 686f 7374 3a38 3030 302f 646f  ocalhost:8000/do
+00000b80: 6373 2920 746f 2076 6965 7720 4f70 656e  cs) to view Open
+00000b90: 4150 4920 646f 6375 6d65 6e74 6174 696f  API documentatio
+00000ba0: 6e20 696e 2074 6865 2062 726f 7773 6572  n in the browser
+00000bb0: 2e0a 0a54 6865 2070 6167 6520 7769 6c6c  ...The page will
+00000bc0: 2061 7574 6f6d 6174 6963 616c 6c79 2072   automatically r
+00000bd0: 656c 6f61 6420 6966 2079 6f75 206d 616b  eload if you mak
+00000be0: 6520 6368 616e 6765 7320 746f 2074 6865  e changes to the
+00000bf0: 2063 6f64 652e 0a0a 2323 2320 606d 616b   code...### `mak
+00000c00: 6520 7465 7374 600a 0a52 756e 7320 7465  e test`..Runs te
+00000c10: 7374 732e 3c62 723e 0a42 7920 6465 6661  sts.<br>.By defa
+00000c20: 756c 742c 2072 756e 7320 7465 7374 7320  ult, runs tests 
+00000c30: 7265 6c61 7465 6420 746f 2066 696c 6573  related to files
+00000c40: 2063 6861 6e67 6564 2073 696e 6365 2074   changed since t
+00000c50: 6865 206c 6173 7420 636f 6d6d 6974 2e0a  he last commit..
+00000c60: 0a23 2320 4c69 6365 6e73 650a 0a60 6661  .## License..`fa
+00000c70: 7374 6170 692d 6765 6e60 2069 7320 6469  stapi-gen` is di
+00000c80: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
+00000c90: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
+00000ca0: 205b 4d49 545d 2868 7474 7073 3a2f 2f67   [MIT](https://g
+00000cb0: 6974 6875 622e 636f 6d2f 6d69 7270 6f2f  ithub.com/mirpo/
+00000cc0: 6661 7374 6170 692d 6765 6e2f 626c 6f62  fastapi-gen/blob
+00000cd0: 2f6d 6173 7465 722f 4c49 4345 4e53 4529  /master/LICENSE)
+00000ce0: 206c 6963 656e 7365 2e0a                  license..
```

### Comparing `fastapi_gen-0.2.0/pyproject.toml` & `fastapi_gen-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,172 +1,125 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
-include = [
-  "src",
-]
+include = ["src"]
 
 [tool.hatch.build.targets.wheel]
 sources = ["src"]
 
 [project]
 name = "fastapi-gen"
 dynamic = ["version"]
 description = "Set up a modern REST API by running one command."
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 keywords = [
-  "fastapi", "cli", "hello world","huggingface", "langchain", "summarization", 
-  "nlp", "ner", "named-entity recognition", "text generation", "llama", "llama.cpp",
+  "fastapi",
+  "cli",
+  "hello world",
+  "huggingface",
+  "langchain",
+  "summarization",
+  "nlp",
+  "ner",
+  "named-entity recognition",
+  "text generation",
+  "llama",
+  "llama.cpp",
 ]
 authors = [
   { name = "Miroslav Pokrovskii", email = "miroslavpokrovskiy@gmail.com" },
 ]
 classifiers = [
-    "Intended Audience :: Information Technology",
-    "Intended Audience :: System Administrators",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python",
-    "Topic :: Internet",
-    "Topic :: Software Development :: Libraries :: Application Frameworks",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: Software Development :: Libraries",
-    "Topic :: Software Development",
-    "Typing :: Typed",
-    "Development Status :: 4 - Beta",
-    "Environment :: Web Environment",
-    "Framework :: AsyncIO",
-    "Framework :: FastAPI",
-    "Framework :: Pydantic",
-    "Framework :: Pydantic :: 1",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
-    "Topic :: Internet :: WWW/HTTP",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
-]
-dependencies = [
-  "click==8.1.6",
-  "colorama==0.4.6",
-  "importlib_resources==6.0.0",
+  "Intended Audience :: Information Technology",
+  "Intended Audience :: System Administrators",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python",
+  "Topic :: Internet",
+  "Topic :: Software Development :: Libraries :: Application Frameworks",
+  "Topic :: Software Development :: Libraries :: Python Modules",
+  "Topic :: Software Development :: Libraries",
+  "Topic :: Software Development",
+  "Typing :: Typed",
+  "Development Status :: 4 - Beta",
+  "Environment :: Web Environment",
+  "Framework :: AsyncIO",
+  "Framework :: FastAPI",
+  "Framework :: Pydantic",
+  "Framework :: Pydantic :: 1",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
+  "Topic :: Internet :: WWW/HTTP",
+  "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
+dependencies = ["click==8.1.6", "colorama==0.4.6", "importlib_resources==6.0.0"]
 
 [project.optional-dependencies]
-dev = [
-  "mypy==1.4.1",
-  "ruff==0.0.280",
-  "black==23.7.0",
-]
+dev = ["ruff==0.0.280"]
 
 [project.urls]
 Documentation = "https://github.com/mirpo/fastapi-gen#readme"
 Issues = "https://github.com/mirpo/fastapi-gen/issues"
 Source = "https://github.com/mirpo/fastapi-gen"
 
 [project.scripts]
 fastapi-gen = "cli.__main__:main"
 
 [tool.hatch.version]
 path = "src/cli/__about__.py"
 
 [tool.hatch.envs.default]
-dependencies = [
-  "coverage[toml]>=6.5",
-  "pytest",
-]
+dependencies = ["coverage[toml]>=6.5", "pytest"]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.10", "3.11"]
 
-[tool.hatch.envs.lint]
-detached = true
-dependencies = [
-  "mypy==1.4.1",
-  "ruff==0.0.280",
-  "black==23.7.0",
-]
-
-[tool.hatch.envs.lint.scripts]
-style = [
-  "ruff {args:.}",
-  "black --check --diff {args:.}",
-]
-fmt = [
-  "black {args:.}",
-  "ruff --fix {args:.}",
-  "style",
-]
-all = [
-  "style",
-  "typing",
-]
-
 [tool.black]
 target-version = ["py311"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py311"
 line-length = 120
-select = [
-  "A",
-  "ARG",
-  "B",
-  "C",
-  "DTZ",
-  "E",
-  "EM",
-  "F",
-  "FBT",
-  "I",
-  "ICN",
-  "ISC",
-  "N",
-  "PLC",
-  "PLE",
-  "PLR",
-  "PLW",
-  "Q",
-  "RUF",
-  "S",
-  "T",
-  "TID",
-  "UP",
-  "W",
-  "YTT",
-]
+select = ["ALL"]
 ignore = [
-  # Allow non-abstract empty methods in abstract base classes
-  "B027",
-  # Allow boolean positional values in function calls, like `dict.get(... True)`
-  "FBT003",
-  # Ignore checks for possible passwords
-  "S105", "S106", "S107", 
-  # Ignore complexity
-  "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
-  "S603", "S607", "S101", "PLR2004",
+  "ANN",     # Type hints related, let mypy handle these.
+  "B027",    # Allow non-abstract empty methods in abstract base classes
+  "D",       # Docstring errors. Should add proper documentation at some point.
+  "FBT003",  # Allow boolean positional values in function calls, like `dict.get(... True)`
+  "S105",    # Ignore checks for possible passwords
+  "S106",
+  "S107",
+  "C901",    # Ignore complexity
+  "PLR0911",
+  "PLR0912",
+  "PLR0913",
+  "PLR0915",
+  "PTH",     # User Pathlib stuff over os.*. Should migrate to Pathlib at some point.
+  "S603",
+  "S607",
+  "S101",
+  "PLR2004",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
 [tool.ruff.isort]
-known-first-party = ["cli"]
+known-first-party = ["src"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
```

### Comparing `fastapi_gen-0.2.0/PKG-INFO` & `fastapi_gen-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6661 7374  : 2.1.Name: fast
 00000020: 6170 692d 6765 6e0a 5665 7273 696f 6e3a  api-gen.Version:
-00000030: 2030 2e32 2e30 0a53 756d 6d61 7279 3a20   0.2.0.Summary: 
+00000030: 2030 2e33 2e30 0a53 756d 6d61 7279 3a20   0.3.0.Summary: 
 00000040: 5365 7420 7570 2061 206d 6f64 6572 6e20  Set up a modern 
 00000050: 5245 5354 2041 5049 2062 7920 7275 6e6e  REST API by runn
 00000060: 696e 6720 6f6e 6520 636f 6d6d 616e 642e  ing one command.
 00000070: 0a50 726f 6a65 6374 2d55 524c 3a20 446f  .Project-URL: Do
 00000080: 6375 6d65 6e74 6174 696f 6e2c 2068 7474  cumentation, htt
 00000090: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 000000a0: 6d69 7270 6f2f 6661 7374 6170 692d 6765  mirpo/fastapi-ge
@@ -70,213 +70,263 @@
 00000450: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
 00000460: 2033 0a43 6c61 7373 6966 6965 723a 2050   3.Classifier: P
 00000470: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
 00000480: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
 00000490: 2033 203a 3a20 4f6e 6c79 0a43 6c61 7373   3 :: Only.Class
 000004a0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
 000004b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000004c0: 7974 686f 6e20 3a3a 2033 2e37 0a43 6c61  ython :: 3.7.Cla
-000004d0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000004e0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000004f0: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
-00000500: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000510: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000520: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-00000530: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000540: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000550: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000560: 2e31 300a 436c 6173 7369 6669 6572 3a20  .10.Classifier: 
-00000570: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000580: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000590: 3a20 332e 3131 0a43 6c61 7373 6966 6965  : 3.11.Classifie
-000005a0: 723a 2054 6f70 6963 203a 3a20 496e 7465  r: Topic :: Inte
-000005b0: 726e 6574 0a43 6c61 7373 6966 6965 723a  rnet.Classifier:
-000005c0: 2054 6f70 6963 203a 3a20 496e 7465 726e   Topic :: Intern
-000005d0: 6574 203a 3a20 5757 572f 4854 5450 0a43  et :: WWW/HTTP.C
-000005e0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-000005f0: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
-00000600: 5757 572f 4854 5450 203a 3a20 4854 5450  WWW/HTTP :: HTTP
-00000610: 2053 6572 7665 7273 0a43 6c61 7373 6966   Servers.Classif
-00000620: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
-00000630: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
-00000640: 7269 6e67 203a 3a20 4172 7469 6669 6369  ring :: Artifici
-00000650: 616c 2049 6e74 656c 6c69 6765 6e63 650a  al Intelligence.
-00000660: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-00000670: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
-00000680: 7665 6c6f 706d 656e 740a 436c 6173 7369  velopment.Classi
-00000690: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
-000006a0: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
-000006b0: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
-000006c0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
-000006d0: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
-000006e0: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
-000006f0: 6272 6172 6965 7320 3a3a 2041 7070 6c69  braries :: Appli
-00000700: 6361 7469 6f6e 2046 7261 6d65 776f 726b  cation Framework
-00000710: 730a 436c 6173 7369 6669 6572 3a20 546f  s.Classifier: To
-00000720: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
-00000730: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
-00000740: 6962 7261 7269 6573 203a 3a20 5079 7468  ibraries :: Pyth
-00000750: 6f6e 204d 6f64 756c 6573 0a43 6c61 7373  on Modules.Class
-00000760: 6966 6965 723a 2054 7970 696e 6720 3a3a  ifier: Typing ::
-00000770: 2054 7970 6564 0a52 6571 7569 7265 732d   Typed.Requires-
-00000780: 5079 7468 6f6e 3a20 3e3d 332e 3130 0a52  Python: >=3.10.R
-00000790: 6571 7569 7265 732d 4469 7374 3a20 636c  equires-Dist: cl
-000007a0: 6963 6b3d 3d38 2e31 2e36 0a52 6571 7569  ick==8.1.6.Requi
-000007b0: 7265 732d 4469 7374 3a20 636f 6c6f 7261  res-Dist: colora
-000007c0: 6d61 3d3d 302e 342e 360a 5265 7175 6972  ma==0.4.6.Requir
-000007d0: 6573 2d44 6973 743a 2069 6d70 6f72 746c  es-Dist: importl
-000007e0: 6962 2d72 6573 6f75 7263 6573 3d3d 362e  ib-resources==6.
-000007f0: 302e 300a 5072 6f76 6964 6573 2d45 7874  0.0.Provides-Ext
-00000800: 7261 3a20 6465 760a 5265 7175 6972 6573  ra: dev.Requires
-00000810: 2d44 6973 743a 2062 6c61 636b 3d3d 3233  -Dist: black==23
-00000820: 2e37 2e30 3b20 6578 7472 6120 3d3d 2027  .7.0; extra == '
-00000830: 6465 7627 0a52 6571 7569 7265 732d 4469  dev'.Requires-Di
-00000840: 7374 3a20 6d79 7079 3d3d 312e 342e 313b  st: mypy==1.4.1;
-00000850: 2065 7874 7261 203d 3d20 2764 6576 270a   extra == 'dev'.
-00000860: 5265 7175 6972 6573 2d44 6973 743a 2072  Requires-Dist: r
-00000870: 7566 663d 3d30 2e30 2e32 3830 3b20 6578  uff==0.0.280; ex
-00000880: 7472 6120 3d3d 2027 6465 7627 0a44 6573  tra == 'dev'.Des
-00000890: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-000008a0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-000008b0: 646f 776e 0a0a 2320 4661 7374 4170 6920  down..# FastApi 
-000008c0: 4765 6e0a 0a43 7265 6174 6520 4661 7374  Gen..Create Fast
-000008d0: 4150 4920 6170 7073 2077 6974 6820 6e6f  API apps with no
-000008e0: 2062 7569 6c64 2063 6f6e 6669 6775 7261   build configura
-000008f0: 7469 6f6e 2e0a 0a46 6173 7441 7069 2047  tion...FastApi G
-00000900: 656e 2077 6f72 6b73 206f 6e20 6d61 634f  en works on macO
-00000910: 5320 616e 6420 4c69 6e75 782e 3c62 723e  S and Linux.<br>
-00000920: 0a49 6620 736f 6d65 7468 696e 6720 646f  .If something do
-00000930: 6573 6ee2 8099 7420 776f 726b 2c20 706c  esn...t work, pl
-00000940: 6561 7365 205b 6669 6c65 2061 6e20 6973  ease [file an is
-00000950: 7375 655d 2868 7474 7073 3a2f 2f67 6974  sue](https://git
-00000960: 6875 622e 636f 6d2f 6d69 7270 6f2f 6661  hub.com/mirpo/fa
-00000970: 7374 6170 692d 6765 6e2f 6973 7375 6573  stapi-gen/issues
-00000980: 2f6e 6577 292e 0a0a 4176 6169 6c61 626c  /new)...Availabl
-00000990: 6520 7465 6d70 6c61 7465 733a 0a0a 312e  e templates:..1.
-000009a0: 2044 6566 6175 6c74 202d 2062 6173 6963   Default - basic
-000009b0: 2074 656d 706c 6174 6520 7769 7468 2047   template with G
-000009c0: 4554 2f50 4f53 5420 6578 616d 706c 6573  ET/POST examples
-000009d0: 2e0a 322e 204e 6c70 202d 206e 6174 7572  ..2. Nlp - natur
-000009e0: 616c 206c 616e 6775 6167 6520 7072 6f63  al language proc
-000009f0: 6573 7369 6e67 2074 656d 706c 6174 6520  essing template 
-00000a00: 7769 7468 2065 7861 6d70 6c65 7320 686f  with examples ho
-00000a10: 7720 746f 2075 7365 2048 7567 6769 6e66  w to use Hugginf
-00000a20: 6163 6520 7375 6d6d 6172 697a 6174 696f  ace summarizatio
-00000a30: 6e2c 206e 616d 6564 2d65 6e74 6974 7920  n, named-entity 
-00000a40: 7265 636f 676e 6974 696f 6e20 616e 6420  recognition and 
-00000a50: 7465 7874 2067 656e 6572 6174 696f 6e20  text generation 
-00000a60: 7573 696e 6720 4c4c 4d2e 0a0a 4d6f 7265  using LLM...More
-00000a70: 2074 6f20 636f 6d65 210a 0a23 2320 5175   to come!..## Qu
-00000a80: 6963 6b20 4f76 6572 7669 6577 0a0a 6060  ick Overview..``
-00000a90: 6063 6f6e 736f 6c65 0a70 6970 3320 696e  `console.pip3 in
-00000aa0: 7374 616c 6c20 6661 7374 6170 692d 6765  stall fastapi-ge
-00000ab0: 6e0a 6661 7374 6170 692d 6765 6e20 6d79  n.fastapi-gen my
-00000ac0: 5f61 7070 0a63 6420 6d79 5f61 7070 0a6d  _app.cd my_app.m
-00000ad0: 616b 6520 7374 6172 742d 6465 760a 6060  ake start-dev.``
-00000ae0: 600a 0a6f 7220 0a0a 6060 6063 6f6e 736f  `..or ..```conso
-00000af0: 6c65 0a70 6970 7820 7275 6e20 6661 7374  le.pipx run fast
-00000b00: 6170 692d 6765 6e20 6d79 5f61 7070 0a63  api-gen my_app.c
-00000b10: 6420 6d79 5f61 7070 0a6d 616b 6520 7374  d my_app.make st
-00000b20: 6172 742d 6465 760a 6060 600a 0a49 6620  art-dev.```..If 
-00000b30: 796f 7527 7665 2070 7265 7669 6f75 736c  you've previousl
-00000b40: 7920 696e 7374 616c 6c65 6420 6066 6173  y installed `fas
-00000b50: 7461 7069 2d67 656e 6020 676c 6f62 616c  tapi-gen` global
-00000b60: 6c79 2076 6961 2060 7069 7033 2069 6e73  ly via `pip3 ins
-00000b70: 7461 6c6c 2066 6173 7461 7069 2d67 656e  tall fastapi-gen
-00000b80: 602c 2077 6520 7265 636f 6d6d 656e 6420  `, we recommend 
-00000b90: 796f 7520 7265 696e 7374 616c 6c20 7468  you reinstall th
-00000ba0: 6520 7061 636b 6167 6520 7573 696e 6720  e package using 
-00000bb0: 6070 6970 3320 696e 7374 616c 6c20 2d2d  `pip3 install --
-00000bc0: 7570 6772 6164 6520 2d2d 666f 7263 652d  upgrade --force-
-00000bd0: 7265 696e 7374 616c 6c20 6661 7374 6170  reinstall fastap
-00000be0: 692d 6765 6e60 206f 7220 6070 6970 7820  i-gen` or `pipx 
-00000bf0: 7570 6772 6164 6520 6661 7374 6170 692d  upgrade fastapi-
-00000c00: 6765 6e60 2074 6f20 656e 7375 7265 2074  gen` to ensure t
-00000c10: 6861 7420 796f 7520 7573 6520 7468 6520  hat you use the 
-00000c20: 6c61 7465 7374 2076 6572 7369 6f6e 2e0a  latest version..
-00000c30: 0a54 6865 6e20 6f70 656e 2068 7474 703a  .Then open http:
-00000c40: 2f2f 6c6f 6361 6c68 6f73 743a 3830 3030  //localhost:8000
-00000c50: 2f64 6f63 7320 746f 2073 6565 2079 6f75  /docs to see you
-00000c60: 7220 6170 7020 4f70 656e 4150 4920 646f  r app OpenAPI do
-00000c70: 6375 6d65 6e74 6174 696f 6e2e 0a0a 2323  cumentation...##
-00000c80: 2320 4765 7420 5374 6172 7465 6420 496d  # Get Started Im
-00000c90: 6d65 6469 6174 656c 790a 0a59 6f75 202a  mediately..You *
-00000ca0: 2a64 6f6e e280 9974 2a2a 206e 6565 6420  *don...t** need 
-00000cb0: 746f 2069 6e73 7461 6c6c 206f 7220 636f  to install or co
-00000cc0: 6e66 6967 7572 6520 6465 7065 6e63 656e  nfigure depencen
-00000cd0: 6465 6963 6573 206c 696b 6520 4661 7374  deices like Fast
-00000ce0: 4170 6920 6f72 2050 7974 6573 742e 3c62  Api or Pytest.<b
-00000cf0: 723e 0a54 6865 7920 6172 6520 7072 6563  r>.They are prec
-00000d00: 6f6e 6669 6775 7265 6420 616e 6420 6869  onfigured and hi
-00000d10: 6464 656e 2073 6f20 7468 6174 2079 6f75  dden so that you
-00000d20: 2063 616e 2066 6f63 7573 206f 6e20 7468   can focus on th
-00000d30: 6520 636f 6465 2e0a 0a43 7265 6174 6520  e code...Create 
-00000d40: 6120 7072 6f6a 6563 742c 2061 6e64 2079  a project, and y
-00000d50: 6f75 e280 9972 6520 676f 6f64 2074 6f20  ou...re good to 
-00000d60: 676f 2e0a 0a23 2320 4372 6561 7469 6e67  go...## Creating
-00000d70: 2061 6e20 4170 700a 0a2a 2a59 6f75 e280   an App..**You..
-00000d80: 996c 6c20 6e65 6564 2074 6f20 6861 7665  .ll need to have
-00000d90: 2050 7974 686f 6e20 332e 372b 206f 7220   Python 3.7+ or 
-00000da0: 6c61 7465 7220 7665 7273 696f 6e20 6f6e  later version on
-00000db0: 2079 6f75 7220 6c6f 6361 6c20 6465 7665   your local deve
-00000dc0: 6c6f 706d 656e 7420 6d61 6368 696e 652a  lopment machine*
-00000dd0: 2a2e 2057 6520 7265 636f 6d6d 656e 6420  *. We recommend 
-00000de0: 7573 696e 6720 7468 6520 6c61 7465 7374  using the latest
-00000df0: 204c 5453 2076 6572 7369 6f6e 2e20 596f   LTS version. Yo
-00000e00: 7520 6361 6e20 7573 6520 5b70 7965 6e76  u can use [pyenv
-00000e10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000e20: 2e63 6f6d 2f70 7965 6e76 2f70 7965 6e76  .com/pyenv/pyenv
-00000e30: 2920 286d 6163 4f53 2f4c 696e 7578 2920  ) (macOS/Linux) 
-00000e40: 746f 2073 7769 7463 6820 5079 7468 6f6e  to switch Python
-00000e50: 2076 6572 7369 6f6e 7320 6265 7477 6565   versions betwee
-00000e60: 6e20 6469 6666 6572 656e 7420 7072 6f6a  n different proj
-00000e70: 6563 7473 2e0a 0a23 2323 2062 6173 6963  ects...### basic
-00000e80: 2074 656d 706c 6174 650a 0a60 6060 636f   template..```co
-00000e90: 6e73 6f6c 650a 7069 7033 2069 6e73 7461  nsole.pip3 insta
-00000ea0: 6c6c 2066 6173 7461 7069 2d67 656e 0a66  ll fastapi-gen.f
-00000eb0: 6173 7461 7069 2d67 656e 206d 795f 6170  astapi-gen my_ap
-00000ec0: 700a 6060 600a 0a6f 720a 0a60 6060 636f  p.```..or..```co
-00000ed0: 6e73 6f6c 650a 7069 7033 2069 6e73 7461  nsole.pip3 insta
-00000ee0: 6c6c 2066 6173 7461 7069 2d67 656e 0a66  ll fastapi-gen.f
-00000ef0: 6173 7461 7069 2d67 656e 206d 795f 6170  astapi-gen my_ap
-00000f00: 7020 2d2d 7465 6d70 6c61 7465 2068 656c  p --template hel
-00000f10: 6c6f 5f77 6f72 6c64 0a60 6060 0a0a 2323  lo_world.```..##
-00000f20: 2320 4e4c 5020 7465 6d70 6c61 7465 0a0a  # NLP template..
-00000f30: 6060 6063 6f6e 736f 6c65 0a70 6970 2069  ```console.pip i
-00000f40: 6e73 7461 6c6c 2066 6173 7461 7069 2d67  nstall fastapi-g
-00000f50: 656e 0a66 6173 7461 7069 2d67 656e 206d  en.fastapi-gen m
-00000f60: 795f 6170 7020 2d2d 7465 6d70 6c61 7465  y_app --template
-00000f70: 206e 6c70 0a60 6060 0a0a 496e 7369 6465   nlp.```..Inside
-00000f80: 2074 6865 206e 6577 6c79 2063 7265 6174   the newly creat
-00000f90: 6564 2070 726f 6a65 6374 2c20 796f 7520  ed project, you 
-00000fa0: 6361 6e20 7275 6e20 736f 6d65 2062 7569  can run some bui
-00000fb0: 6c74 2d69 6e20 636f 6d6d 616e 6473 3a0a  lt-in commands:.
-00000fc0: 0a23 2323 2060 6d61 6b65 2073 7461 7274  .### `make start
-00000fd0: 600a 0a52 756e 7320 7468 6520 6170 7020  `..Runs the app 
-00000fe0: 696e 2064 6576 656c 6f70 6d65 6e74 206d  in development m
-00000ff0: 6f64 652e 3c62 723e 0a4f 7065 6e20 5b68  ode.<br>.Open [h
-00001000: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00001010: 3830 3030 2f64 6f63 735d 2868 7474 703a  8000/docs](http:
-00001020: 2f2f 6c6f 6361 6c68 6f73 743a 3830 3030  //localhost:8000
-00001030: 2f64 6f63 7329 2074 6f20 7669 6577 204f  /docs) to view O
-00001040: 7065 6e41 5049 2064 6f63 756d 656e 7461  penAPI documenta
-00001050: 7469 6f6e 2069 6e20 7468 6520 6272 6f77  tion in the brow
-00001060: 7365 722e 0a0a 5468 6520 7061 6765 2077  ser...The page w
-00001070: 696c 6c20 6175 746f 6d61 7469 6361 6c6c  ill automaticall
-00001080: 7920 7265 6c6f 6164 2069 6620 796f 7520  y reload if you 
-00001090: 6d61 6b65 2063 6861 6e67 6573 2074 6f20  make changes to 
-000010a0: 7468 6520 636f 6465 2e0a 0a23 2323 2060  the code...### `
-000010b0: 6d61 6b65 2074 6573 7460 0a0a 5275 6e73  make test`..Runs
-000010c0: 2074 6573 7473 2e3c 6272 3e0a 4279 2064   tests.<br>.By d
-000010d0: 6566 6175 6c74 2c20 7275 6e73 2074 6573  efault, runs tes
-000010e0: 7473 2072 656c 6174 6564 2074 6f20 6669  ts related to fi
-000010f0: 6c65 7320 6368 616e 6765 6420 7369 6e63  les changed sinc
-00001100: 6520 7468 6520 6c61 7374 2063 6f6d 6d69  e the last commi
-00001110: 742e 0a0a 2323 204c 6963 656e 7365 0a0a  t...## License..
-00001120: 6066 6173 7461 7069 2d67 656e 6020 6973  `fastapi-gen` is
-00001130: 2064 6973 7472 6962 7574 6564 2075 6e64   distributed und
-00001140: 6572 2074 6865 2074 6572 6d73 206f 6620  er the terms of 
-00001150: 7468 6520 5b4d 4954 5d28 6874 7470 733a  the [MIT](https:
-00001160: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6972  //github.com/mir
-00001170: 706f 2f66 6173 7461 7069 2d67 656e 2f62  po/fastapi-gen/b
-00001180: 6c6f 622f 6d61 7374 6572 2f4c 4943 454e  lob/master/LICEN
-00001190: 5345 2920 6c69 6365 6e73 652e 0a         SE) license..
+000004c0: 7974 686f 6e20 3a3a 2033 2e31 300a 436c  ython :: 3.10.Cl
+000004d0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000004e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000004f0: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
+00000500: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000510: 6963 203a 3a20 496e 7465 726e 6574 0a43  ic :: Internet.C
+00000520: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+00000530: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
+00000540: 5757 572f 4854 5450 0a43 6c61 7373 6966  WWW/HTTP.Classif
+00000550: 6965 723a 2054 6f70 6963 203a 3a20 496e  ier: Topic :: In
+00000560: 7465 726e 6574 203a 3a20 5757 572f 4854  ternet :: WWW/HT
+00000570: 5450 203a 3a20 4854 5450 2053 6572 7665  TP :: HTTP Serve
+00000580: 7273 0a43 6c61 7373 6966 6965 723a 2054  rs.Classifier: T
+00000590: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
+000005a0: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
+000005b0: 3a20 4172 7469 6669 6369 616c 2049 6e74  : Artificial Int
+000005c0: 656c 6c69 6765 6e63 650a 436c 6173 7369  elligence.Classi
+000005d0: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+000005e0: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+000005f0: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
+00000600: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
+00000610: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
+00000620: 204c 6962 7261 7269 6573 0a43 6c61 7373   Libraries.Class
+00000630: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+00000640: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
+00000650: 6d65 6e74 203a 3a20 4c69 6272 6172 6965  ment :: Librarie
+00000660: 7320 3a3a 2041 7070 6c69 6361 7469 6f6e  s :: Application
+00000670: 2046 7261 6d65 776f 726b 730a 436c 6173   Frameworks.Clas
+00000680: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00000690: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
+000006a0: 706d 656e 7420 3a3a 204c 6962 7261 7269  pment :: Librari
+000006b0: 6573 203a 3a20 5079 7468 6f6e 204d 6f64  es :: Python Mod
+000006c0: 756c 6573 0a43 6c61 7373 6966 6965 723a  ules.Classifier:
+000006d0: 2054 7970 696e 6720 3a3a 2054 7970 6564   Typing :: Typed
+000006e0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
+000006f0: 3a20 3e3d 332e 3130 0a52 6571 7569 7265  : >=3.10.Require
+00000700: 732d 4469 7374 3a20 636c 6963 6b3d 3d38  s-Dist: click==8
+00000710: 2e31 2e36 0a52 6571 7569 7265 732d 4469  .1.6.Requires-Di
+00000720: 7374 3a20 636f 6c6f 7261 6d61 3d3d 302e  st: colorama==0.
+00000730: 342e 360a 5265 7175 6972 6573 2d44 6973  4.6.Requires-Dis
+00000740: 743a 2069 6d70 6f72 746c 6962 2d72 6573  t: importlib-res
+00000750: 6f75 7263 6573 3d3d 362e 302e 300a 5072  ources==6.0.0.Pr
+00000760: 6f76 6964 6573 2d45 7874 7261 3a20 6465  ovides-Extra: de
+00000770: 760a 5265 7175 6972 6573 2d44 6973 743a  v.Requires-Dist:
+00000780: 2072 7566 663d 3d30 2e30 2e32 3830 3b20   ruff==0.0.280; 
+00000790: 6578 7472 6120 3d3d 2027 6465 7627 0a44  extra == 'dev'.D
+000007a0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+000007b0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+000007c0: 726b 646f 776e 0a0a 2320 4661 7374 4170  rkdown..# FastAp
+000007d0: 6920 4765 6e0a 0a43 7265 6174 6520 4661  i Gen..Create Fa
+000007e0: 7374 4150 4920 6170 7073 2077 6974 6820  stAPI apps with 
+000007f0: 6e6f 2062 7569 6c64 2063 6f6e 6669 6775  no build configu
+00000800: 7261 7469 6f6e 2e0a 0a3c 6120 6872 6566  ration...<a href
+00000810: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000820: 2e63 6f6d 2f6d 6972 706f 2f66 6173 7461  .com/mirpo/fasta
+00000830: 7069 2d67 656e 2f61 6374 696f 6e73 2f77  pi-gen/actions/w
+00000840: 6f72 6b66 6c6f 7773 2f74 6573 742e 796d  orkflows/test.ym
+00000850: 6c3f 7175 6572 793d 776f 726b 666c 6f77  l?query=workflow
+00000860: 2533 4174 6573 742b 6576 656e 7425 3341  %3Atest+event%3A
+00000870: 7075 7368 2b62 7261 6e63 6825 3341 6d61  push+branch%3Ama
+00000880: 7374 6572 2220 7461 7267 6574 3d22 5f62  ster" target="_b
+00000890: 6c61 6e6b 223e 0a20 2020 203c 696d 6720  lank">.    <img 
+000008a0: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+000008b0: 6875 622e 636f 6d2f 6d69 7270 6f2f 6661  hub.com/mirpo/fa
+000008c0: 7374 6170 692d 6765 6e2f 6163 7469 6f6e  stapi-gen/action
+000008d0: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
+000008e0: 2e79 6d6c 2f62 6164 6765 2e73 7667 3f62  .yml/badge.svg?b
+000008f0: 7261 6e63 683d 6d61 7374 6572 2220 616c  ranch=master" al
+00000900: 743d 2254 6573 7422 3e0a 3c2f 613e 0a3c  t="Test">.</a>.<
+00000910: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000920: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000930: 2f66 6173 7461 7069 2d67 656e 2220 7461  /fastapi-gen" ta
+00000940: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
+00000950: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000960: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000970: 2e69 6f2f 7079 7069 2f76 2f66 6173 7461  .io/pypi/v/fasta
+00000980: 7069 2d67 656e 3f63 6f6c 6f72 3d25 3233  pi-gen?color=%23
+00000990: 3334 4430 3538 266c 6162 656c 3d70 7970  34D058&label=pyp
+000009a0: 6925 3230 7061 636b 6167 6522 2061 6c74  i%20package" alt
+000009b0: 3d22 5061 636b 6167 6520 7665 7273 696f  ="Package versio
+000009c0: 6e22 3e0a 3c2f 613e 0a3c 6120 6872 6566  n">.</a>.<a href
+000009d0: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+000009e0: 7267 2f70 726f 6a65 6374 2f66 6173 7461  rg/project/fasta
+000009f0: 7069 2d67 656e 2220 7461 7267 6574 3d22  pi-gen" target="
+00000a00: 5f62 6c61 6e6b 223e 0a20 2020 203c 696d  _blank">.    <im
+00000a10: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000a20: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000a30: 7069 2f70 7976 6572 7369 6f6e 732f 6661  pi/pyversions/fa
+00000a40: 7374 6170 692d 6765 6e2e 7376 673f 636f  stapi-gen.svg?co
+00000a50: 6c6f 723d 2532 3333 3444 3035 3822 2061  lor=%2334D058" a
+00000a60: 6c74 3d22 5375 7070 6f72 7465 6420 5079  lt="Supported Py
+00000a70: 7468 6f6e 2076 6572 7369 6f6e 7322 3e0a  thon versions">.
+00000a80: 3c2f 613e 0a0a 2d2d 2d0a 0a46 6173 7441  </a>..---..FastA
+00000a90: 7069 2047 656e 2077 6f72 6b73 206f 6e20  pi Gen works on 
+00000aa0: 6d61 634f 5320 616e 6420 4c69 6e75 782e  macOS and Linux.
+00000ab0: 3c62 723e 0a49 6620 736f 6d65 7468 696e  <br>.If somethin
+00000ac0: 6720 646f 6573 6ee2 8099 7420 776f 726b  g doesn...t work
+00000ad0: 2c20 706c 6561 7365 205b 6669 6c65 2061  , please [file a
+00000ae0: 6e20 6973 7375 655d 2868 7474 7073 3a2f  n issue](https:/
+00000af0: 2f67 6974 6875 622e 636f 6d2f 6d69 7270  /github.com/mirp
+00000b00: 6f2f 6661 7374 6170 692d 6765 6e2f 6973  o/fastapi-gen/is
+00000b10: 7375 6573 2f6e 6577 292e 0a0a 4176 6169  sues/new)...Avai
+00000b20: 6c61 626c 6520 7465 6d70 6c61 7465 733a  lable templates:
+00000b30: 0a0a 312e 2044 6566 6175 6c74 202d 2062  ..1. Default - b
+00000b40: 6173 6963 2074 656d 706c 6174 6520 7769  asic template wi
+00000b50: 7468 2047 4554 2f50 4f53 5420 6578 616d  th GET/POST exam
+00000b60: 706c 6573 2e0a 322e 204e 4c50 202d 206e  ples..2. NLP - n
+00000b70: 6174 7572 616c 206c 616e 6775 6167 6520  atural language 
+00000b80: 7072 6f63 6573 7369 6e67 2074 656d 706c  processing templ
+00000b90: 6174 6520 7769 7468 2065 7861 6d70 6c65  ate with example
+00000ba0: 7320 686f 7720 746f 2075 7365 206c 6f63  s how to use loc
+00000bb0: 616c 2048 7567 6769 6e66 6163 6520 6d6f  al Hugginface mo
+00000bc0: 6465 6c73 2066 6f72 2073 756d 6d61 7269  dels for summari
+00000bd0: 7a61 7469 6f6e 2c20 6e61 6d65 642d 656e  zation, named-en
+00000be0: 7469 7479 2072 6563 6f67 6e69 7469 6f6e  tity recognition
+00000bf0: 2061 6e64 2074 6578 7420 6765 6e65 7261   and text genera
+00000c00: 7469 6f6e 2075 7369 6e67 204c 4c4d 2e0a  tion using LLM..
+00000c10: 332e 204c 616e 6763 6861 696e 202d 2074  3. Langchain - t
+00000c20: 656d 706c 6174 6520 7769 7468 2065 7861  emplate with exa
+00000c30: 6d70 6c65 7320 686f 7720 746f 2075 7365  mples how to use
+00000c40: 204c 616e 6743 6861 696e 2077 6974 6820   LangChain with 
+00000c50: 6c6f 6361 6c20 4875 6767 696e 6661 6365  local Hugginface
+00000c60: 206d 6f64 656c 7320 284c 4c4d 7329 2066   models (LLMs) f
+00000c70: 6f72 2074 6578 7420 6765 6e65 7261 7469  or text generati
+00000c80: 6f6e 2061 6e64 2071 7565 7374 696f 6e20  on and question 
+00000c90: 616e 7377 6572 696e 672e 0a0a 2a49 6d70  answering...*Imp
+00000ca0: 6f72 7461 6e74 206e 6f74 652a 202d 204c  ortant note* - L
+00000cb0: 616e 6763 6861 696e 2074 656d 706c 6174  angchain templat
+00000cc0: 6520 7265 7175 6972 6573 2068 6172 6477  e requires hardw
+00000cd0: 6172 6520 746f 2072 756e 2061 6e64 2077  are to run and w
+00000ce0: 696c 6c20 6175 746f 6d61 7469 6361 6c6c  ill automaticall
+00000cf0: 7920 646f 776e 6c6f 6164 2072 6571 7569  y download requi
+00000d00: 7265 6420 6d6f 6465 6c73 2c20 6265 2070  red models, be p
+00000d10: 6174 6965 6e74 2e0a 0a4d 6f72 6520 746f  atient...More to
+00000d20: 2063 6f6d 6521 0a0a 2323 2051 7569 636b   come!..## Quick
+00000d30: 204f 7665 7276 6965 770a 0a60 6060 636f   Overview..```co
+00000d40: 6e73 6f6c 650a 7069 7033 2069 6e73 7461  nsole.pip3 insta
+00000d50: 6c6c 2066 6173 7461 7069 2d67 656e 0a66  ll fastapi-gen.f
+00000d60: 6173 7461 7069 2d67 656e 206d 795f 6170  astapi-gen my_ap
+00000d70: 700a 6364 206d 795f 6170 700a 6d61 6b65  p.cd my_app.make
+00000d80: 2073 7461 7274 2d64 6576 0a60 6060 0a0a   start-dev.```..
+00000d90: 6f72 200a 0a60 6060 636f 6e73 6f6c 650a  or ..```console.
+00000da0: 7069 7078 2072 756e 2066 6173 7461 7069  pipx run fastapi
+00000db0: 2d67 656e 206d 795f 6170 700a 6364 206d  -gen my_app.cd m
+00000dc0: 795f 6170 700a 6d61 6b65 2073 7461 7274  y_app.make start
+00000dd0: 2d64 6576 0a60 6060 0a0a 4966 2079 6f75  -dev.```..If you
+00000de0: 2776 6520 7072 6576 696f 7573 6c79 2069  've previously i
+00000df0: 6e73 7461 6c6c 6564 2060 6661 7374 6170  nstalled `fastap
+00000e00: 692d 6765 6e60 2067 6c6f 6261 6c6c 7920  i-gen` globally 
+00000e10: 7669 6120 6070 6970 3320 696e 7374 616c  via `pip3 instal
+00000e20: 6c20 6661 7374 6170 692d 6765 6e60 2c20  l fastapi-gen`, 
+00000e30: 7765 2072 6563 6f6d 6d65 6e64 2079 6f75  we recommend you
+00000e40: 2072 6569 6e73 7461 6c6c 2074 6865 2070   reinstall the p
+00000e50: 6163 6b61 6765 2075 7369 6e67 2060 7069  ackage using `pi
+00000e60: 7033 2069 6e73 7461 6c6c 202d 2d75 7067  p3 install --upg
+00000e70: 7261 6465 202d 2d66 6f72 6365 2d72 6569  rade --force-rei
+00000e80: 6e73 7461 6c6c 2066 6173 7461 7069 2d67  nstall fastapi-g
+00000e90: 656e 6020 6f72 2060 7069 7078 2075 7067  en` or `pipx upg
+00000ea0: 7261 6465 2066 6173 7461 7069 2d67 656e  rade fastapi-gen
+00000eb0: 6020 746f 2065 6e73 7572 6520 7468 6174  ` to ensure that
+00000ec0: 2079 6f75 2075 7365 2074 6865 206c 6174   you use the lat
+00000ed0: 6573 7420 7665 7273 696f 6e2e 0a0a 5468  est version...Th
+00000ee0: 656e 206f 7065 6e20 6874 7470 3a2f 2f6c  en open http://l
+00000ef0: 6f63 616c 686f 7374 3a38 3030 302f 646f  ocalhost:8000/do
+00000f00: 6373 2074 6f20 7365 6520 796f 7572 2061  cs to see your a
+00000f10: 7070 204f 7065 6e41 5049 2064 6f63 756d  pp OpenAPI docum
+00000f20: 656e 7461 7469 6f6e 2e0a 0a23 2323 2047  entation...### G
+00000f30: 6574 2053 7461 7274 6564 2049 6d6d 6564  et Started Immed
+00000f40: 6961 7465 6c79 0a0a 596f 7520 2a2a 646f  iately..You **do
+00000f50: 6ee2 8099 742a 2a20 6e65 6564 2074 6f20  n...t** need to 
+00000f60: 696e 7374 616c 6c20 6f72 2063 6f6e 6669  install or confi
+00000f70: 6775 7265 2064 6570 656e 6365 6e64 6569  gure depencendei
+00000f80: 6365 7320 6c69 6b65 2046 6173 7441 7069  ces like FastApi
+00000f90: 206f 7220 5079 7465 7374 2e3c 6272 3e0a   or Pytest.<br>.
+00000fa0: 5468 6579 2061 7265 2070 7265 636f 6e66  They are preconf
+00000fb0: 6967 7572 6564 2061 6e64 2068 6964 6465  igured and hidde
+00000fc0: 6e20 736f 2074 6861 7420 796f 7520 6361  n so that you ca
+00000fd0: 6e20 666f 6375 7320 6f6e 2074 6865 2063  n focus on the c
+00000fe0: 6f64 652e 0a0a 4372 6561 7465 2061 2070  ode...Create a p
+00000ff0: 726f 6a65 6374 2c20 616e 6420 796f 75e2  roject, and you.
+00001000: 8099 7265 2067 6f6f 6420 746f 2067 6f2e  ..re good to go.
+00001010: 0a0a 2323 2043 7265 6174 696e 6720 616e  ..## Creating an
+00001020: 2041 7070 0a0a 2a2a 596f 75e2 8099 6c6c   App..**You...ll
+00001030: 206e 6565 6420 746f 2068 6176 6520 5079   need to have Py
+00001040: 7468 6f6e 2033 2e37 2b20 6f72 206c 6174  thon 3.7+ or lat
+00001050: 6572 2076 6572 7369 6f6e 206f 6e20 796f  er version on yo
+00001060: 7572 206c 6f63 616c 2064 6576 656c 6f70  ur local develop
+00001070: 6d65 6e74 206d 6163 6869 6e65 2a2a 2e20  ment machine**. 
+00001080: 5765 2072 6563 6f6d 6d65 6e64 2075 7369  We recommend usi
+00001090: 6e67 2074 6865 206c 6174 6573 7420 4c54  ng the latest LT
+000010a0: 5320 7665 7273 696f 6e2e 2059 6f75 2063  S version. You c
+000010b0: 616e 2075 7365 205b 7079 656e 765d 2868  an use [pyenv](h
+000010c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000010d0: 6d2f 7079 656e 762f 7079 656e 7629 2028  m/pyenv/pyenv) (
+000010e0: 6d61 634f 532f 4c69 6e75 7829 2074 6f20  macOS/Linux) to 
+000010f0: 7377 6974 6368 2050 7974 686f 6e20 7665  switch Python ve
+00001100: 7273 696f 6e73 2062 6574 7765 656e 2064  rsions between d
+00001110: 6966 6665 7265 6e74 2070 726f 6a65 6374  ifferent project
+00001120: 732e 0a0a 2323 2320 6261 7369 6320 7465  s...### basic te
+00001130: 6d70 6c61 7465 0a0a 6060 6063 6f6e 736f  mplate..```conso
+00001140: 6c65 0a70 6970 3320 696e 7374 616c 6c20  le.pip3 install 
+00001150: 6661 7374 6170 692d 6765 6e0a 6661 7374  fastapi-gen.fast
+00001160: 6170 692d 6765 6e20 6d79 5f61 7070 0a60  api-gen my_app.`
+00001170: 6060 0a0a 6f72 0a0a 6060 6063 6f6e 736f  ``..or..```conso
+00001180: 6c65 0a70 6970 3320 696e 7374 616c 6c20  le.pip3 install 
+00001190: 6661 7374 6170 692d 6765 6e0a 6661 7374  fastapi-gen.fast
+000011a0: 6170 692d 6765 6e20 6d79 5f61 7070 202d  api-gen my_app -
+000011b0: 2d74 656d 706c 6174 6520 6865 6c6c 6f5f  -template hello_
+000011c0: 776f 726c 640a 6060 600a 0a23 2323 204e  world.```..### N
+000011d0: 4c50 2074 656d 706c 6174 650a 0a60 6060  LP template..```
+000011e0: 636f 6e73 6f6c 650a 7069 7020 696e 7374  console.pip inst
+000011f0: 616c 6c20 6661 7374 6170 692d 6765 6e0a  all fastapi-gen.
+00001200: 6661 7374 6170 692d 6765 6e20 6d79 5f61  fastapi-gen my_a
+00001210: 7070 202d 2d74 656d 706c 6174 6520 6e6c  pp --template nl
+00001220: 700a 6060 600a 0a23 2323 204c 616e 6763  p.```..### Langc
+00001230: 6861 696e 2074 656d 706c 6174 650a 0a60  hain template..`
+00001240: 6060 636f 6e73 6f6c 650a 7069 7020 696e  ``console.pip in
+00001250: 7374 616c 6c20 6661 7374 6170 692d 6765  stall fastapi-ge
+00001260: 6e0a 6661 7374 6170 692d 6765 6e20 6d79  n.fastapi-gen my
+00001270: 5f61 7070 202d 2d74 656d 706c 6174 6520  _app --template 
+00001280: 4c61 6e67 6368 6169 6e0a 6060 600a 0a49  Langchain.```..I
+00001290: 6e73 6964 6520 7468 6520 6e65 776c 7920  nside the newly 
+000012a0: 6372 6561 7465 6420 7072 6f6a 6563 742c  created project,
+000012b0: 2079 6f75 2063 616e 2072 756e 2073 6f6d   you can run som
+000012c0: 6520 6275 696c 742d 696e 2063 6f6d 6d61  e built-in comma
+000012d0: 6e64 733a 0a0a 2323 2320 606d 616b 6520  nds:..### `make 
+000012e0: 7374 6172 7460 0a0a 5275 6e73 2074 6865  start`..Runs the
+000012f0: 2061 7070 2069 6e20 6465 7665 6c6f 706d   app in developm
+00001300: 656e 7420 6d6f 6465 2e3c 6272 3e0a 4f70  ent mode.<br>.Op
+00001310: 656e 205b 6874 7470 3a2f 2f6c 6f63 616c  en [http://local
+00001320: 686f 7374 3a38 3030 302f 646f 6373 5d28  host:8000/docs](
+00001330: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+00001340: 3a38 3030 302f 646f 6373 2920 746f 2076  :8000/docs) to v
+00001350: 6965 7720 4f70 656e 4150 4920 646f 6375  iew OpenAPI docu
+00001360: 6d65 6e74 6174 696f 6e20 696e 2074 6865  mentation in the
+00001370: 2062 726f 7773 6572 2e0a 0a54 6865 2070   browser...The p
+00001380: 6167 6520 7769 6c6c 2061 7574 6f6d 6174  age will automat
+00001390: 6963 616c 6c79 2072 656c 6f61 6420 6966  ically reload if
+000013a0: 2079 6f75 206d 616b 6520 6368 616e 6765   you make change
+000013b0: 7320 746f 2074 6865 2063 6f64 652e 0a0a  s to the code...
+000013c0: 2323 2320 606d 616b 6520 7465 7374 600a  ### `make test`.
+000013d0: 0a52 756e 7320 7465 7374 732e 3c62 723e  .Runs tests.<br>
+000013e0: 0a42 7920 6465 6661 756c 742c 2072 756e  .By default, run
+000013f0: 7320 7465 7374 7320 7265 6c61 7465 6420  s tests related 
+00001400: 746f 2066 696c 6573 2063 6861 6e67 6564  to files changed
+00001410: 2073 696e 6365 2074 6865 206c 6173 7420   since the last 
+00001420: 636f 6d6d 6974 2e0a 0a23 2320 4c69 6365  commit...## Lice
+00001430: 6e73 650a 0a60 6661 7374 6170 692d 6765  nse..`fastapi-ge
+00001440: 6e60 2069 7320 6469 7374 7269 6275 7465  n` is distribute
+00001450: 6420 756e 6465 7220 7468 6520 7465 726d  d under the term
+00001460: 7320 6f66 2074 6865 205b 4d49 545d 2868  s of the [MIT](h
+00001470: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001480: 6d2f 6d69 7270 6f2f 6661 7374 6170 692d  m/mirpo/fastapi-
+00001490: 6765 6e2f 626c 6f62 2f6d 6173 7465 722f  gen/blob/master/
+000014a0: 4c49 4345 4e53 4529 206c 6963 656e 7365  LICENSE) license
+000014b0: 2e0a                                     ..
```

