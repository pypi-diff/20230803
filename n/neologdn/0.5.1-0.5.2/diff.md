# Comparing `tmp/neologdn-0.5.1.tar.gz` & `tmp/neologdn-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\neologdn-0.5.1.tar", last modified: Sun May  2 11:42:50 2021, max compression
+gzip compressed data, was "neologdn-0.5.2.tar", last modified: Thu Aug  3 12:53:54 2023, max compression
```

## Comparing `neologdn-0.5.1.tar` & `neologdn-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2021-05-02 11:42:50.000000 neologdn-0.5.1/
--rw-rw-rw-   0        0        0     1170 2021-05-02 11:40:34.000000 neologdn-0.5.1/CHANGES.rst
--rw-rw-rw-   0        0        0    11547 2019-01-19 16:04:36.000000 neologdn-0.5.1/LICENSE
--rw-rw-rw-   0        0        0       54 2019-01-19 16:04:36.000000 neologdn-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0   350216 2021-05-02 11:40:34.000000 neologdn-0.5.1/neologdn.cpp
-drwxrwxrwx   0        0        0        0 2021-05-02 11:42:50.000000 neologdn-0.5.1/neologdn.egg-info/
--rw-rw-rw-   0        0        0        1 2021-05-02 11:42:50.000000 neologdn-0.5.1/neologdn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     6705 2021-05-02 11:42:50.000000 neologdn-0.5.1/neologdn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2021-05-02 11:42:50.000000 neologdn-0.5.1/neologdn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2021-05-02 11:42:50.000000 neologdn-0.5.1/neologdn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6705 2021-05-02 11:42:50.000000 neologdn-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     3173 2021-05-02 11:40:34.000000 neologdn-0.5.1/README.rst
--rw-rw-rw-   0        0        0       42 2021-05-02 11:42:50.000000 neologdn-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1685 2021-05-02 02:06:17.000000 neologdn-0.5.1/setup.py
+drwxr-xr-x   0 yukino     (501) staff       (20)        0 2023-08-03 12:53:54.979622 neologdn-0.5.2/
+-rw-r--r--   0 yukino     (501) staff       (20)     1271 2023-08-03 11:54:12.000000 neologdn-0.5.2/CHANGES.rst
+-rw-r--r--   0 yukino     (501) staff       (20)    11345 2023-08-03 11:43:11.000000 neologdn-0.5.2/LICENSE
+-rw-r--r--   0 yukino     (501) staff       (20)       51 2023-08-03 11:43:11.000000 neologdn-0.5.2/MANIFEST.in
+-rw-r--r--   0 yukino     (501) staff       (20)     5580 2023-08-03 12:53:54.979514 neologdn-0.5.2/PKG-INFO
+-rw-r--r--   0 yukino     (501) staff       (20)     3298 2023-08-03 12:47:56.000000 neologdn-0.5.2/README.rst
+-rw-r--r--   0 yukino     (501) staff       (20)   564567 2023-08-03 11:47:41.000000 neologdn-0.5.2/neologdn.cpp
+drwxr-xr-x   0 yukino     (501) staff       (20)        0 2023-08-03 12:53:54.979362 neologdn-0.5.2/neologdn.egg-info/
+-rw-r--r--   0 yukino     (501) staff       (20)     5580 2023-08-03 12:53:54.000000 neologdn-0.5.2/neologdn.egg-info/PKG-INFO
+-rw-r--r--   0 yukino     (501) staff       (20)      192 2023-08-03 12:53:54.000000 neologdn-0.5.2/neologdn.egg-info/SOURCES.txt
+-rw-r--r--   0 yukino     (501) staff       (20)        1 2023-08-03 12:53:54.000000 neologdn-0.5.2/neologdn.egg-info/dependency_links.txt
+-rw-r--r--   0 yukino     (501) staff       (20)        9 2023-08-03 12:53:54.000000 neologdn-0.5.2/neologdn.egg-info/top_level.txt
+-rw-r--r--   0 yukino     (501) staff       (20)       38 2023-08-03 12:53:54.979652 neologdn-0.5.2/setup.cfg
+-rw-r--r--   0 yukino     (501) staff       (20)     1847 2023-08-03 12:52:38.000000 neologdn-0.5.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `neologdn-0.5.1/CHANGES.rst` & `neologdn-0.5.2/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 ========
 
+0.5.2 (2023-08-03)
+----------------------------
+
+- Support Python 3.10 and 3.11 (Many thanks @polm)
+
 0.5.1 (2021-05-02)
 ----------------------------
 
 - Improve performance of shorten_repeat function (Many thanks @yskn67)
 - Add tilde option to normalize function
 
 0.4 (2018-12-06)
```

### Comparing `neologdn-0.5.1/LICENSE` & `neologdn-0.5.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "{}"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2015 Yukino Ikegami
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "{}"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2015 Yukino Ikegami
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
```

### Comparing `neologdn-0.5.1/README.rst` & `neologdn-0.5.2/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 neologdn
 ===========
 
-|travis| |pyversion| |version| |license|
+|downloads| |pyversion| |version| |license|
 
 neologdn is a Japanese text normalizer for `mecab-neologd <https://github.com/neologd/mecab-ipadic-neologd>`_.
 
 The normalization is based on the neologd's rules:
 https://github.com/neologd/mecab-ipadic-neologd/wiki/Regexp.ja
 
 
@@ -64,23 +64,23 @@
 .. code:: python
 
     # Sample code from
     # https://github.com/neologd/mecab-ipadic-neologd/wiki/Regexp.ja#python-written-by-hideaki-t--overlast
     import normalize_neologd
 
     %timeit normalize(normalize_neologd.normalize_neologd)
-    # => 1 loop, best of 3: 18.3 s per loop
+    # => 9.55 s ± 29.4 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
 
     import neologdn
     %timeit normalize(neologdn.normalize)
-    # => 1 loop, best of 3: 9.05 s per loop
+    # => 6.66 s ± 35.8 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
 
-neologdn is about x2 faster than sample code.
+neologdn is about x1.43 faster than sample code.
 
 details are described as the below notebook:
 https://github.com/ikegami-yukino/neologdn/blob/master/benchmark/benchmark.ipynb
 
 
 License
 -------
@@ -89,18 +89,16 @@
 
 
 Contribution
 ------------
 
 Contributions are welcome! See: https://github.com/ikegami-yukino/neologdn/blob/master/.github/CONTRIBUTING.md
 
-
-.. |travis| image:: https://travis-ci.org/ikegami-yukino/neologdn.svg?branch=master
-    :target: https://travis-ci.org/ikegami-yukino/neologdn
-    :alt: travis-ci.org
+.. |downloads| image:: https://static.pepy.tech/personalized-badge/neologdn?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
+ :target: https://pepy.tech/project/neologdn
 
 .. |version| image:: https://img.shields.io/pypi/v/neologdn.svg
     :target: http://pypi.python.org/pypi/neologdn/
     :alt: latest version
 
 .. |pyversion| image:: https://img.shields.io/pypi/pyversions/neologdn.svg
```

### Comparing `neologdn-0.5.1/setup.py` & `neologdn-0.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # -*- coding: utf-8 -*-
 from codecs import open
 import re
 from setuptools import setup, Extension
 import platform
 
 with open('neologdn.cpp', 'r', encoding='utf8') as f:
-    version = re.compile(
-        r".*__version__ = '(.*?)'", re.S).match(f.read()).group(1)
+    version = re.compile(r".*__version__ = '(.*?)'",
+                         re.S).match(f.read()).group(1)
 
 extra_compile_args = ["-std=c++11"]
 if platform.system() == "Darwin":
     extra_compile_args.append("-mmacosx-version-min=10.7")
     extra_compile_args.append("-stdlib=libc++")
 
-setup(
-    name='neologdn',
-    version=version,
-    author='Yukino Ikegami',
-    author_email='yknikgm@gmail.com',
-    url='http://github.com/ikegami-yukino/neologdn',
-    ext_modules=[Extension('neologdn', ['neologdn.cpp'],
-                           language='c++', extra_compile_args=extra_compile_args)],
-    license='Apache Software License',
-    keywords=['japanese', 'MeCab'],
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Natural Language :: Japanese',
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Cython',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Topic :: Text Processing :: Linguistic'
-    ],
-    description='Japanese text normalizer for mecab-neologd',
-    long_description='%s\n\n%s' % (open('README.rst', 'r', encoding='utf8').read(),
-                                   open('CHANGES.rst', 'r', encoding='utf8').read()
-                                   ),
-)
+setup(name='neologdn',
+      version=version,
+      author='Yukino Ikegami',
+      author_email='yknikgm@gmail.com',
+      url='http://github.com/ikegami-yukino/neologdn',
+      ext_modules=[
+          Extension('neologdn', ['neologdn.cpp'],
+                    language='c++',
+                    extra_compile_args=extra_compile_args)
+      ],
+      license='Apache Software License',
+      keywords=['japanese', 'MeCab'],
+      classifiers=[
+          'Development Status :: 3 - Alpha', 'Intended Audience :: Developers',
+          'Natural Language :: Japanese',
+          'License :: OSI Approved :: Apache Software License',
+          'Programming Language :: Cython', 'Programming Language :: Python',
+          'Programming Language :: Python :: 3',
+          'Programming Language :: Python :: 3.6',
+          'Programming Language :: Python :: 3.7',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
+          'Topic :: Text Processing :: Linguistic'
+      ],
+      description='Japanese text normalizer for mecab-neologd',
+      long_description='%s\n\n%s' %
+      (open('README.rst', 'r', encoding='utf8').read(),
+       open('CHANGES.rst', 'r', encoding='utf8').read()),
+      long_description_content_type='text/x-rst')
```

