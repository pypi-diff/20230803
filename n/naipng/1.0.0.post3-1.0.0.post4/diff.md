# Comparing `tmp/naipng-1.0.0.post3.tar.gz` & `tmp/naipng-1.0.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naipng-1.0.0.post3.tar", last modified: Thu Aug  3 08:25:49 2023, max compression, from Unix
+gzip compressed data, was "naipng-1.0.0.post4.tar", last modified: Thu Aug  3 08:29:25 2023, max compression, from Unix
```

## Comparing `naipng-1.0.0.post3.tar` & `naipng-1.0.0.post4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 08:25:49.472662 naipng-1.0.0.post3/
--rwxrwxrwx   0 root         (0) root         (0)      859 2023-08-03 00:07:01.000000 naipng-1.0.0.post3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     8608 2023-08-03 08:25:49.471663 naipng-1.0.0.post3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     7886 2023-08-03 08:24:32.000000 naipng-1.0.0.post3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 08:25:49.431663 naipng-1.0.0.post3/naipng/
--rwxrwxrwx   0 root         (0) root         (0)    18711 2023-08-03 07:40:08.000000 naipng-1.0.0.post3/naipng/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4030 2023-08-03 07:52:51.000000 naipng-1.0.0.post3/naipng/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 08:25:49.463663 naipng-1.0.0.post3/naipng.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     8608 2023-08-03 08:25:49.000000 naipng-1.0.0.post3/naipng.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      223 2023-08-03 08:25:49.000000 naipng-1.0.0.post3/naipng.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-08-03 08:25:49.000000 naipng-1.0.0.post3/naipng.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       48 2023-08-03 08:25:49.000000 naipng-1.0.0.post3/naipng.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-08-03 08:25:49.000000 naipng-1.0.0.post3/naipng.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     1051 2023-08-03 08:24:32.000000 naipng-1.0.0.post3/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-08-03 08:25:49.472662 naipng-1.0.0.post3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 08:29:25.015461 naipng-1.0.0.post4/
+-rwxrwxrwx   0 root         (0) root         (0)      859 2023-08-03 00:07:01.000000 naipng-1.0.0.post4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     8268 2023-08-03 08:29:25.014460 naipng-1.0.0.post4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     7546 2023-08-03 08:27:28.000000 naipng-1.0.0.post4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 08:29:24.974461 naipng-1.0.0.post4/naipng/
+-rwxrwxrwx   0 root         (0) root         (0)    18711 2023-08-03 07:40:08.000000 naipng-1.0.0.post4/naipng/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4030 2023-08-03 07:52:51.000000 naipng-1.0.0.post4/naipng/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 08:29:25.007460 naipng-1.0.0.post4/naipng.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     8268 2023-08-03 08:29:24.000000 naipng-1.0.0.post4/naipng.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      223 2023-08-03 08:29:24.000000 naipng-1.0.0.post4/naipng.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-08-03 08:29:24.000000 naipng-1.0.0.post4/naipng.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       48 2023-08-03 08:29:24.000000 naipng-1.0.0.post4/naipng.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-08-03 08:29:24.000000 naipng-1.0.0.post4/naipng.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1051 2023-08-03 08:28:51.000000 naipng-1.0.0.post4/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-08-03 08:29:25.015461 naipng-1.0.0.post4/setup.cfg
```

### Comparing `naipng-1.0.0.post3/LICENSE` & `naipng-1.0.0.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `naipng-1.0.0.post3/PKG-INFO` & `naipng-1.0.0.post4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naipng
-Version: 1.0.0.post3
+Version: 1.0.0.post4
 Summary: Library and command-line tool to read NovelAI data encoded in PNG files
 Author: Eta
 License: zlib/libpng License
 Project-URL: Homepage, https://github.com/Eta0/naipng
 Keywords: novelai,nai,png,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: zlib/libpng License
@@ -15,39 +15,36 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # naipng ✒️🖼️
-<a id="naipng"></a>
 
 `naipng` is a Python library and command-line tool to read [NovelAI](https://novelai.net)
 data encoded in PNG files (like in Lorebook cards and generated images), with no dependencies.
 
 Also check out my website [pngmeta](https://pngmeta.glitch.me) for a browser-based tool for
 [viewing](https://pngmeta.glitch.me) and [copying](https://pngmeta.glitch.me/transfer) PNG `tEXt` metadata.
 
 # Table of Contents
-<a id="table-of-contents"></a>
 
 - [What Is This?](#what-is-this)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Library](#library)
     - [Example](#naipngread-example)
     - [Error Handling](#error-handling)
   - [CLI](#cli)
     - [Help Text](#help-text)
     - [Examples](#examples)
 - [Technical Background](#technical-background)
 - [License](#license)
 
 # What Is This?
-<a id="what-is-this"></a>
 
 User-made content for the web service [NovelAI](https://novelai.net) is often shared off-platform in the form of files.
 These files take on multiple formats. Though most are simple JSON, some content can be shared embedded within PNGs,
 which is more complicated to extract.
 
 **Text Generation**: NovelAI allows exporting certain settings and objects related to text generation AI as PNG images
 in place of regular JSON files, as a way of associating art with the descriptions of characters and places being shared.
@@ -57,45 +54,41 @@
 such as `prompt`, `steps`, and so on, to make it easier to replicate and modify generated images.
 
 Both domains use PNG metadata to encode this information, thus this tool allows the extraction of that metadata.
 
 See more technical details in the [Technical Background](#technical-background) section.
 
 # Installation
-<a id="installation"></a>
 
 `naipng` is available on PyPI, so it can be installed through `pip`:
 
 ```bash
 python -m pip install naipng
 ```
 
 Since `naipng` has no dependencies, you can also import or run it by simply adding the `naipng` directory
 to your source tree.
 
 # Usage
-<a id="usage"></a>
 
 `naipng` may be used either as a [library](#library) or a [command-line tool](#cli).
 
 ## Library
-<a id="library"></a>
 
 The primary function entrypoint provided by `naipng` is `naipng.read(file: bytes | BinaryIO)`.
 This can be used to parse a PNG image for NovelAI metadata from either an open file or a `bytes` object in memory.
 
 Two more specific variations of `naipng.read()` also exist:
 
 - `naipng.read_text_gen(file: bytes | BinaryIO)` only returns text generation data
   - *E.g. Lorebooks*
 - `naipng.read_image_gen(file: bytes | BinaryIO)` only returns image generation data
   - *E.g. image prompts*
 
 ### `naipng.read()` Example
-<a id="naipngread-example"></a>
 
 ```python
 import naipng
 
 # Using a file-like object
 with open("image.png", "rb") as file:
     decoded = naipng.read(file)
@@ -118,15 +111,14 @@
 data: bytes = pathlib.Path("image.png").read_bytes()
 decoded = naipng.read(data)
 
 # ...
 ```
 
 ### Error Handling
-<a id="error-handling"></a>
 
 `naipng` defines two error types for `naipng.read()` and its variants:
 
 - `naipng.InvalidPNGError` is raised when a PNG is invalid and cannot be parsed, such as when:
   - The PNG datastream ends prematurely (before `IEND`)
   - A `tEXt` chunk is corrupted *(i.e. has an invalid CRC)*
   - The PNG signature is missing
@@ -157,20 +149,18 @@
 This outputs:
 
 ```
 Error: not a valid PNG file: ends prematurely
 ```
 
 ## CLI
-<a id="cli"></a>
 
 `naipng` may be invoked on the command line as either `python -m naipng <file>` or simply `naipng <file>`.
 
 ### Help Text
-<a id="help-text"></a>
 
 ```
 usage: naipng [-h] [-q] [-c] [-t] [-i] file [outfile]
 
 read NovelAI data encoded in a PNG file
 
 positional arguments:
@@ -182,15 +172,14 @@
   -q, --quiet    don't print errors
   -c, --compact  don't pretty-print decoded JSON
   -t, --text     only check for text generation data
   -i, --image    only check for image generation data
 ```
 
 ### Examples
-<a id="examples"></a>
 
 - Printing to stdout:
 
 ```bash
 naipng image.png
 ```
 
@@ -220,22 +209,20 @@
 ```bash
 $ curl -fs https://files.catbox.moe/3b6dux.png | naipng -c - | jq -r ".[\"entries\"][][\"text\"]"
 
 Everyone said that no man now living or ever after would be born who would be equal to him in strength, courage, and in all sorts of courtesy, as well as in boldness and generosity that he had above all men, and that his name would never perish in the German tongue, and the same was true with the Norsemen
 ```
 
 #### Trivia
-<a id="trivia"></a>
 
 The linked file is the first Lorebook card shared as an example when PNG embedding was announced.
 Its art is by Tarmillustrates.
 The quote in it is from *[Þiðreks saga](https://en.wikipedia.org/wiki/%C3%9Ei%C3%B0reks_saga)*.
 
 # Technical Background
-<a id="technical-background"></a>
 
 PNGs are made up of a sequence of data chunks.
 Beyond those used to store visual information (e.g. pixels, palettes),
 there are also several varieties of metadata chunks.
 See [the official PNG specification](http://www.libpng.org/pub/png/spec/1.2/PNG-Structure.html) for full details.
 
 NovelAI uses [`tEXt` metadata chunks](http://www.libpng.org/pub/png/spec/1.2/PNG-Chunks.html#C.Anc-text)
@@ -247,10 +234,9 @@
   - Some of these include `Title`, `Description`, `Software`, `Source`, and `Comment`.
   - `naipng` only reads the `Comment` field among these, which is JSON-encoded and contains the most information.
   - `Comment` is a standard `tEXt` keyword, so recognizing these chunks is slightly ambiguous.
     - Other software may use the `Comment` `tEXt` chunk type for other purposes, and may or may not store JSON in it.
     - `naipng` assumes that the first JSON-encoded `Comment` `tEXt` chunk found is valid image generation metadata.
 
 # License
-<a id="license"></a>
 
 `naipng` is free and open-source software provided under the [zlib license](https://opensource.org/licenses/Zlib).
```

### Comparing `naipng-1.0.0.post3/README.md` & `naipng-1.0.0.post4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # naipng ✒️🖼️
-<a id="naipng"></a>
 
 `naipng` is a Python library and command-line tool to read [NovelAI](https://novelai.net)
 data encoded in PNG files (like in Lorebook cards and generated images), with no dependencies.
 
 Also check out my website [pngmeta](https://pngmeta.glitch.me) for a browser-based tool for
 [viewing](https://pngmeta.glitch.me) and [copying](https://pngmeta.glitch.me/transfer) PNG `tEXt` metadata.
 
 # Table of Contents
-<a id="table-of-contents"></a>
 
 - [What Is This?](#what-is-this)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Library](#library)
     - [Example](#naipngread-example)
     - [Error Handling](#error-handling)
   - [CLI](#cli)
     - [Help Text](#help-text)
     - [Examples](#examples)
 - [Technical Background](#technical-background)
 - [License](#license)
 
 # What Is This?
-<a id="what-is-this"></a>
 
 User-made content for the web service [NovelAI](https://novelai.net) is often shared off-platform in the form of files.
 These files take on multiple formats. Though most are simple JSON, some content can be shared embedded within PNGs,
 which is more complicated to extract.
 
 **Text Generation**: NovelAI allows exporting certain settings and objects related to text generation AI as PNG images
 in place of regular JSON files, as a way of associating art with the descriptions of characters and places being shared.
@@ -37,45 +34,41 @@
 such as `prompt`, `steps`, and so on, to make it easier to replicate and modify generated images.
 
 Both domains use PNG metadata to encode this information, thus this tool allows the extraction of that metadata.
 
 See more technical details in the [Technical Background](#technical-background) section.
 
 # Installation
-<a id="installation"></a>
 
 `naipng` is available on PyPI, so it can be installed through `pip`:
 
 ```bash
 python -m pip install naipng
 ```
 
 Since `naipng` has no dependencies, you can also import or run it by simply adding the `naipng` directory
 to your source tree.
 
 # Usage
-<a id="usage"></a>
 
 `naipng` may be used either as a [library](#library) or a [command-line tool](#cli).
 
 ## Library
-<a id="library"></a>
 
 The primary function entrypoint provided by `naipng` is `naipng.read(file: bytes | BinaryIO)`.
 This can be used to parse a PNG image for NovelAI metadata from either an open file or a `bytes` object in memory.
 
 Two more specific variations of `naipng.read()` also exist:
 
 - `naipng.read_text_gen(file: bytes | BinaryIO)` only returns text generation data
   - *E.g. Lorebooks*
 - `naipng.read_image_gen(file: bytes | BinaryIO)` only returns image generation data
   - *E.g. image prompts*
 
 ### `naipng.read()` Example
-<a id="naipngread-example"></a>
 
 ```python
 import naipng
 
 # Using a file-like object
 with open("image.png", "rb") as file:
     decoded = naipng.read(file)
@@ -98,15 +91,14 @@
 data: bytes = pathlib.Path("image.png").read_bytes()
 decoded = naipng.read(data)
 
 # ...
 ```
 
 ### Error Handling
-<a id="error-handling"></a>
 
 `naipng` defines two error types for `naipng.read()` and its variants:
 
 - `naipng.InvalidPNGError` is raised when a PNG is invalid and cannot be parsed, such as when:
   - The PNG datastream ends prematurely (before `IEND`)
   - A `tEXt` chunk is corrupted *(i.e. has an invalid CRC)*
   - The PNG signature is missing
@@ -137,20 +129,18 @@
 This outputs:
 
 ```
 Error: not a valid PNG file: ends prematurely
 ```
 
 ## CLI
-<a id="cli"></a>
 
 `naipng` may be invoked on the command line as either `python -m naipng <file>` or simply `naipng <file>`.
 
 ### Help Text
-<a id="help-text"></a>
 
 ```
 usage: naipng [-h] [-q] [-c] [-t] [-i] file [outfile]
 
 read NovelAI data encoded in a PNG file
 
 positional arguments:
@@ -162,15 +152,14 @@
   -q, --quiet    don't print errors
   -c, --compact  don't pretty-print decoded JSON
   -t, --text     only check for text generation data
   -i, --image    only check for image generation data
 ```
 
 ### Examples
-<a id="examples"></a>
 
 - Printing to stdout:
 
 ```bash
 naipng image.png
 ```
 
@@ -200,22 +189,20 @@
 ```bash
 $ curl -fs https://files.catbox.moe/3b6dux.png | naipng -c - | jq -r ".[\"entries\"][][\"text\"]"
 
 Everyone said that no man now living or ever after would be born who would be equal to him in strength, courage, and in all sorts of courtesy, as well as in boldness and generosity that he had above all men, and that his name would never perish in the German tongue, and the same was true with the Norsemen
 ```
 
 #### Trivia
-<a id="trivia"></a>
 
 The linked file is the first Lorebook card shared as an example when PNG embedding was announced.
 Its art is by Tarmillustrates.
 The quote in it is from *[Þiðreks saga](https://en.wikipedia.org/wiki/%C3%9Ei%C3%B0reks_saga)*.
 
 # Technical Background
-<a id="technical-background"></a>
 
 PNGs are made up of a sequence of data chunks.
 Beyond those used to store visual information (e.g. pixels, palettes),
 there are also several varieties of metadata chunks.
 See [the official PNG specification](http://www.libpng.org/pub/png/spec/1.2/PNG-Structure.html) for full details.
 
 NovelAI uses [`tEXt` metadata chunks](http://www.libpng.org/pub/png/spec/1.2/PNG-Chunks.html#C.Anc-text)
@@ -227,10 +214,9 @@
   - Some of these include `Title`, `Description`, `Software`, `Source`, and `Comment`.
   - `naipng` only reads the `Comment` field among these, which is JSON-encoded and contains the most information.
   - `Comment` is a standard `tEXt` keyword, so recognizing these chunks is slightly ambiguous.
     - Other software may use the `Comment` `tEXt` chunk type for other purposes, and may or may not store JSON in it.
     - `naipng` assumes that the first JSON-encoded `Comment` `tEXt` chunk found is valid image generation metadata.
 
 # License
-<a id="license"></a>
 
 `naipng` is free and open-source software provided under the [zlib license](https://opensource.org/licenses/Zlib).
```

### Comparing `naipng-1.0.0.post3/naipng/__init__.py` & `naipng-1.0.0.post4/naipng/__init__.py`

 * *Files identical despite different names*

### Comparing `naipng-1.0.0.post3/naipng/__main__.py` & `naipng-1.0.0.post4/naipng/__main__.py`

 * *Files identical despite different names*

### Comparing `naipng-1.0.0.post3/naipng.egg-info/PKG-INFO` & `naipng-1.0.0.post4/naipng.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naipng
-Version: 1.0.0.post3
+Version: 1.0.0.post4
 Summary: Library and command-line tool to read NovelAI data encoded in PNG files
 Author: Eta
 License: zlib/libpng License
 Project-URL: Homepage, https://github.com/Eta0/naipng
 Keywords: novelai,nai,png,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: zlib/libpng License
@@ -15,39 +15,36 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # naipng ✒️🖼️
-<a id="naipng"></a>
 
 `naipng` is a Python library and command-line tool to read [NovelAI](https://novelai.net)
 data encoded in PNG files (like in Lorebook cards and generated images), with no dependencies.
 
 Also check out my website [pngmeta](https://pngmeta.glitch.me) for a browser-based tool for
 [viewing](https://pngmeta.glitch.me) and [copying](https://pngmeta.glitch.me/transfer) PNG `tEXt` metadata.
 
 # Table of Contents
-<a id="table-of-contents"></a>
 
 - [What Is This?](#what-is-this)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Library](#library)
     - [Example](#naipngread-example)
     - [Error Handling](#error-handling)
   - [CLI](#cli)
     - [Help Text](#help-text)
     - [Examples](#examples)
 - [Technical Background](#technical-background)
 - [License](#license)
 
 # What Is This?
-<a id="what-is-this"></a>
 
 User-made content for the web service [NovelAI](https://novelai.net) is often shared off-platform in the form of files.
 These files take on multiple formats. Though most are simple JSON, some content can be shared embedded within PNGs,
 which is more complicated to extract.
 
 **Text Generation**: NovelAI allows exporting certain settings and objects related to text generation AI as PNG images
 in place of regular JSON files, as a way of associating art with the descriptions of characters and places being shared.
@@ -57,45 +54,41 @@
 such as `prompt`, `steps`, and so on, to make it easier to replicate and modify generated images.
 
 Both domains use PNG metadata to encode this information, thus this tool allows the extraction of that metadata.
 
 See more technical details in the [Technical Background](#technical-background) section.
 
 # Installation
-<a id="installation"></a>
 
 `naipng` is available on PyPI, so it can be installed through `pip`:
 
 ```bash
 python -m pip install naipng
 ```
 
 Since `naipng` has no dependencies, you can also import or run it by simply adding the `naipng` directory
 to your source tree.
 
 # Usage
-<a id="usage"></a>
 
 `naipng` may be used either as a [library](#library) or a [command-line tool](#cli).
 
 ## Library
-<a id="library"></a>
 
 The primary function entrypoint provided by `naipng` is `naipng.read(file: bytes | BinaryIO)`.
 This can be used to parse a PNG image for NovelAI metadata from either an open file or a `bytes` object in memory.
 
 Two more specific variations of `naipng.read()` also exist:
 
 - `naipng.read_text_gen(file: bytes | BinaryIO)` only returns text generation data
   - *E.g. Lorebooks*
 - `naipng.read_image_gen(file: bytes | BinaryIO)` only returns image generation data
   - *E.g. image prompts*
 
 ### `naipng.read()` Example
-<a id="naipngread-example"></a>
 
 ```python
 import naipng
 
 # Using a file-like object
 with open("image.png", "rb") as file:
     decoded = naipng.read(file)
@@ -118,15 +111,14 @@
 data: bytes = pathlib.Path("image.png").read_bytes()
 decoded = naipng.read(data)
 
 # ...
 ```
 
 ### Error Handling
-<a id="error-handling"></a>
 
 `naipng` defines two error types for `naipng.read()` and its variants:
 
 - `naipng.InvalidPNGError` is raised when a PNG is invalid and cannot be parsed, such as when:
   - The PNG datastream ends prematurely (before `IEND`)
   - A `tEXt` chunk is corrupted *(i.e. has an invalid CRC)*
   - The PNG signature is missing
@@ -157,20 +149,18 @@
 This outputs:
 
 ```
 Error: not a valid PNG file: ends prematurely
 ```
 
 ## CLI
-<a id="cli"></a>
 
 `naipng` may be invoked on the command line as either `python -m naipng <file>` or simply `naipng <file>`.
 
 ### Help Text
-<a id="help-text"></a>
 
 ```
 usage: naipng [-h] [-q] [-c] [-t] [-i] file [outfile]
 
 read NovelAI data encoded in a PNG file
 
 positional arguments:
@@ -182,15 +172,14 @@
   -q, --quiet    don't print errors
   -c, --compact  don't pretty-print decoded JSON
   -t, --text     only check for text generation data
   -i, --image    only check for image generation data
 ```
 
 ### Examples
-<a id="examples"></a>
 
 - Printing to stdout:
 
 ```bash
 naipng image.png
 ```
 
@@ -220,22 +209,20 @@
 ```bash
 $ curl -fs https://files.catbox.moe/3b6dux.png | naipng -c - | jq -r ".[\"entries\"][][\"text\"]"
 
 Everyone said that no man now living or ever after would be born who would be equal to him in strength, courage, and in all sorts of courtesy, as well as in boldness and generosity that he had above all men, and that his name would never perish in the German tongue, and the same was true with the Norsemen
 ```
 
 #### Trivia
-<a id="trivia"></a>
 
 The linked file is the first Lorebook card shared as an example when PNG embedding was announced.
 Its art is by Tarmillustrates.
 The quote in it is from *[Þiðreks saga](https://en.wikipedia.org/wiki/%C3%9Ei%C3%B0reks_saga)*.
 
 # Technical Background
-<a id="technical-background"></a>
 
 PNGs are made up of a sequence of data chunks.
 Beyond those used to store visual information (e.g. pixels, palettes),
 there are also several varieties of metadata chunks.
 See [the official PNG specification](http://www.libpng.org/pub/png/spec/1.2/PNG-Structure.html) for full details.
 
 NovelAI uses [`tEXt` metadata chunks](http://www.libpng.org/pub/png/spec/1.2/PNG-Chunks.html#C.Anc-text)
@@ -247,10 +234,9 @@
   - Some of these include `Title`, `Description`, `Software`, `Source`, and `Comment`.
   - `naipng` only reads the `Comment` field among these, which is JSON-encoded and contains the most information.
   - `Comment` is a standard `tEXt` keyword, so recognizing these chunks is slightly ambiguous.
     - Other software may use the `Comment` `tEXt` chunk type for other purposes, and may or may not store JSON in it.
     - `naipng` assumes that the first JSON-encoded `Comment` `tEXt` chunk found is valid image generation metadata.
 
 # License
-<a id="license"></a>
 
 `naipng` is free and open-source software provided under the [zlib license](https://opensource.org/licenses/Zlib).
```

### Comparing `naipng-1.0.0.post3/pyproject.toml` & `naipng-1.0.0.post4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "naipng"
-version = "1.0.0.post3"
+version = "1.0.0.post4"
 license = { text = "zlib/libpng License" }
 keywords = ["novelai", "nai", "png", "cli"]
 authors = [
   { name="Eta" }
 ]
 description = "Library and command-line tool to read NovelAI data encoded in PNG files"
 readme = "README.md"
```

