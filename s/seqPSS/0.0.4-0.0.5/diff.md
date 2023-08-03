# Comparing `tmp/seqPSS-0.0.4-py3-none-any.whl.zip` & `tmp/seqPSS-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2784 bytes, number of entries: 6
+Zip file size: 2788 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat      822 b- defN 23-Aug-02 23:53 seqPSS/__init__.py
--rw-rw-rw-  2.0 fat     1889 b- defN 23-Aug-02 23:55 seqPSS/seqPSS.py
--rw-rw-rw-  2.0 fat      324 b- defN 23-Aug-02 23:56 seqPSS-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-02 23:56 seqPSS-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-02 23:56 seqPSS-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      439 b- defN 23-Aug-02 23:56 seqPSS-0.0.4.dist-info/RECORD
-6 files, 3573 bytes uncompressed, 1990 bytes compressed:  44.3%
+-rw-rw-rw-  2.0 fat     1894 b- defN 23-Aug-02 23:59 seqPSS/seqPSS.py
+-rw-rw-rw-  2.0 fat      324 b- defN 23-Aug-03 00:00 seqPSS-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 00:00 seqPSS-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-03 00:00 seqPSS-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      439 b- defN 23-Aug-03 00:00 seqPSS-0.0.5.dist-info/RECORD
+6 files, 3578 bytes uncompressed, 1994 bytes compressed:  44.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: seqPSS/__init__.py
 Comment: 
 
 Filename: seqPSS/seqPSS.py
 Comment: 
 
-Filename: seqPSS-0.0.4.dist-info/METADATA
+Filename: seqPSS-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: seqPSS-0.0.4.dist-info/WHEEL
+Filename: seqPSS-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: seqPSS-0.0.4.dist-info/top_level.txt
+Filename: seqPSS-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: seqPSS-0.0.4.dist-info/RECORD
+Filename: seqPSS-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## seqPSS/seqPSS.py

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 
 # In[6]:
 
 
 import numpy as np
 import pandas as pd
-# import random
+from random import *
 
 
 # ## data
 
 # In[3]:
```

