# Comparing `tmp/semsimian-0.1.18rc2-cp39-none-win_amd64.whl.zip` & `tmp/semsimian-0.1.19rc1-cp311-cp311-macosx_10_7_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 356903 bytes, number of entries: 6
--rw-r--r--  4.6 unx     3164 b- defN 23-Jul-24 21:24 semsimian-0.1.18rc2.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jul-24 21:24 semsimian-0.1.18rc2.dist-info/WHEEL
--rw-r--r--  4.6 unx     1567 b- defN 23-Jul-24 21:24 semsimian-0.1.18rc2.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      119 b- defN 23-Jul-24 21:24 semsimian/__init__.py
--rwxr-xr-x  4.6 unx   826880 b- defN 23-Jul-24 21:24 semsimian/semsimian.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      506 b- defN 23-Jul-24 21:24 semsimian-0.1.18rc2.dist-info/RECORD
-6 files, 832332 bytes uncompressed, 355987 bytes compressed:  57.2%
+Zip file size: 1501736 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     3096 b- defN 23-Aug-03 17:03 semsimian-0.1.19rc1.dist-info/METADATA
+-rw-r--r--  4.6 unx      107 b- defN 23-Aug-03 17:03 semsimian-0.1.19rc1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1539 b- defN 23-Aug-03 17:03 semsimian-0.1.19rc1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      119 b- defN 23-Aug-03 17:03 semsimian/__init__.py
+-rwxr-xr-x  4.6 unx  3361336 b- defN 23-Aug-03 17:03 semsimian/semsimian.cpython-311-darwin.so
+-rw-r--r--  4.6 unx      511 b- defN 23-Aug-03 17:03 semsimian-0.1.19rc1.dist-info/RECORD
+6 files, 3366708 bytes uncompressed, 1500814 bytes compressed:  55.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: semsimian-0.1.18rc2.dist-info/METADATA
+Filename: semsimian-0.1.19rc1.dist-info/METADATA
 Comment: 
 
-Filename: semsimian-0.1.18rc2.dist-info/WHEEL
+Filename: semsimian-0.1.19rc1.dist-info/WHEEL
 Comment: 
 
-Filename: semsimian-0.1.18rc2.dist-info/license_files/LICENSE
+Filename: semsimian-0.1.19rc1.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: semsimian/__init__.py
 Comment: 
 
-Filename: semsimian/semsimian.cp39-win_amd64.pyd
+Filename: semsimian/semsimian.cpython-311-darwin.so
 Comment: 
 
-Filename: semsimian-0.1.18rc2.dist-info/RECORD
+Filename: semsimian-0.1.19rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `semsimian-0.1.18rc2.dist-info/METADATA` & `semsimian-0.1.19rc1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 Metadata-Version: 2.1
 Name: semsimian
-Version: 0.1.18rc2
+Version: 0.1.19rc1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-# semsimian
-
-## Installation
-
-- Set up your virtual environment of choice.
-- cd `semsimian` (home directory of this project)
-- `pip install maturin`
-- `maturin develop`
-- `python`
-```
-Python 3.9.16 (main, Jan 11 2023, 10:02:19) 
-[Clang 14.0.6 ] :: Anaconda, Inc. on darwin
-Type "help", "copyright", "credits" or "license" for more information.
->>> from semsimian import Semsimian
->>> s = Semsimian([('banana', 'is_a', 'fruit'), ('cherry', 'is_a', 'fruit')])
->>> s.jaccard_similarity('banana', 'cherry')
-```
-This should yield a value of 1.0.
-
-
-## Releases
-
-As of version 0.1.14, the semsimian source is released on GitHub, with a corresponding set of Python wheels released to Pypi.
-
-To trigger a new set of builds, first update the version number in `Cargo.toml`, then [create a new release](https://github.com/monarch-initiative/semsimian/releases/new).
-
-Wheels are prepared for the following environments and architectures:
-
-| OS      | Architectures                                                                            | Python Versions           |
-|---------|------------------------------------------------------------------------------------------|---------------------------|
-| Linux   | x86_64, x86_64-unknown-linux-musl, aarch64-unknown-linux-gnu, aarch64-unknown-linux-musl | 3.7, 3.8, 3.9, 3.10, 3.11 |
-| MacOS   | x86_64, universal2                                                                       | 3.7, 3.8, 3.9, 3.10, 3.11 |
-| Windows | x86_64                                                                                   | 3.7, 3.8, 3.9, 3.10, 3.11 |
-
-## Troubleshooting
-
-### Building for Mac ARM M1 architectures
-
-If a `import semsimian` results in a `ImportError` warning about incompatible architecture, try the following:
-- Install `conda`. [This guide may be helpful.](https://towardsdatascience.com/how-to-manage-conda-environments-on-an-apple-silicon-m1-mac-1e29cb3bad12)
-- Set up a virtual environment with `conda` so that your Python build is aligned with your processor architecture (in this case, ARM).
-Try something like:
-```
-$ conda create -n myenv python=3.9
-...setup happens...
-$ conda activate myenv
-```
-and then proceed as above.
-
-
-### Code Coverage via Docker
-
-Build a docker image:
-
-```
-docker build -t my-rust-app .
-```
-
-Run your tests inside a Docker container and generate coverage:
-```
-docker run -v "$(pwd)":/usr/src/app -t my-rust-app bash -c "CARGO_INCREMENTAL=0 RUSTFLAGS='-Zprofile -Ccodegen-units=1 -Cinline-threshold=0 -Coverflow-checks=off -Zpanic_abort_tests -Cpanic=abort' cargo test && grcov . -s . --binary-path ./target/debug/ -t html --branch --ignore-not-existing -o ./target/debug/coverage/"
-```
-
-Get Coverage report from:
-```
-open ./target/debug/coverage/index.html
-
-```
+# semsimian
+
+## Installation
+
+- Set up your virtual environment of choice.
+- cd `semsimian` (home directory of this project)
+- `pip install maturin`
+- `maturin develop`
+- `python`
+```
+Python 3.9.16 (main, Jan 11 2023, 10:02:19) 
+[Clang 14.0.6 ] :: Anaconda, Inc. on darwin
+Type "help", "copyright", "credits" or "license" for more information.
+>>> from semsimian import Semsimian
+>>> s = Semsimian([('banana', 'is_a', 'fruit'), ('cherry', 'is_a', 'fruit')])
+>>> s.jaccard_similarity('banana', 'cherry')
+```
+This should yield a value of 1.0.
+
+
+## Releases
+
+As of version 0.1.14, the semsimian source is released on GitHub, with a corresponding set of Python wheels released to Pypi.
+
+To trigger a new set of builds, first update the version number in `Cargo.toml`, then [create a new release](https://github.com/monarch-initiative/semsimian/releases/new).
+
+Wheels are prepared for the following environments and architectures:
+
+| OS      | Architectures                                                                            | Python Versions           |
+|---------|------------------------------------------------------------------------------------------|---------------------------|
+| Linux   | x86_64, x86_64-unknown-linux-musl, aarch64-unknown-linux-gnu, aarch64-unknown-linux-musl | 3.7, 3.8, 3.9, 3.10, 3.11 |
+| MacOS   | x86_64, universal2                                                                       | 3.7, 3.8, 3.9, 3.10, 3.11 |
+| Windows | x86_64                                                                                   | 3.7, 3.8, 3.9, 3.10, 3.11 |
+
+## Troubleshooting
+
+### Building for Mac ARM M1 architectures
+
+If a `import semsimian` results in a `ImportError` warning about incompatible architecture, try the following:
+- Install `conda`. [This guide may be helpful.](https://towardsdatascience.com/how-to-manage-conda-environments-on-an-apple-silicon-m1-mac-1e29cb3bad12)
+- Set up a virtual environment with `conda` so that your Python build is aligned with your processor architecture (in this case, ARM).
+Try something like:
+```
+$ conda create -n myenv python=3.9
+...setup happens...
+$ conda activate myenv
+```
+and then proceed as above.
+
+
+### Code Coverage via Docker
+
+Build a docker image:
+
+```
+docker build -t my-rust-app .
+```
+
+Run your tests inside a Docker container and generate coverage:
+```
+docker run -v "$(pwd)":/usr/src/app -t my-rust-app bash -c "CARGO_INCREMENTAL=0 RUSTFLAGS='-Zprofile -Ccodegen-units=1 -Cinline-threshold=0 -Coverflow-checks=off -Zpanic_abort_tests -Cpanic=abort' cargo test && grcov . -s . --binary-path ./target/debug/ -t html --branch --ignore-not-existing -o ./target/debug/coverage/"
+```
+
+Get Coverage report from:
+```
+open ./target/debug/coverage/index.html
+
+```
```

## Comparing `semsimian-0.1.18rc2.dist-info/license_files/LICENSE` & `semsimian-0.1.19rc1.dist-info/license_files/LICENSE`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-
-Copyright (c) 2023, Harry Caufield, Harshad Hegde, Carlo Kroll, Chris Mungall, Justin Reese
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of semsimian nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+Copyright (c) 2023, Harry Caufield, Harshad Hegde, Carlo Kroll, Chris Mungall, Justin Reese
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of semsimian nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

