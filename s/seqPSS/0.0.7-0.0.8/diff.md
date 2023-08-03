# Comparing `tmp/seqPSS-0.0.7-py3-none-any.whl.zip` & `tmp/seqPSS-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2788 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      822 b- defN 23-Aug-03 00:13 seqPSS/__init__.py
--rw-rw-rw-  2.0 fat     1893 b- defN 23-Aug-03 00:12 seqPSS/seqPSS.py
--rw-rw-rw-  2.0 fat      324 b- defN 23-Aug-03 00:13 seqPSS-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 00:13 seqPSS-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-03 00:13 seqPSS-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      439 b- defN 23-Aug-03 00:13 seqPSS-0.0.7.dist-info/RECORD
-6 files, 3577 bytes uncompressed, 1994 bytes compressed:  44.3%
+Zip file size: 2789 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      822 b- defN 23-Aug-03 00:16 seqPSS/__init__.py
+-rw-rw-rw-  2.0 fat     1895 b- defN 23-Aug-03 00:16 seqPSS/seqPSS.py
+-rw-rw-rw-  2.0 fat      325 b- defN 23-Aug-03 00:17 seqPSS-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 00:17 seqPSS-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-03 00:17 seqPSS-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      439 b- defN 23-Aug-03 00:17 seqPSS-0.0.8.dist-info/RECORD
+6 files, 3580 bytes uncompressed, 1995 bytes compressed:  44.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: seqPSS/__init__.py
 Comment: 
 
 Filename: seqPSS/seqPSS.py
 Comment: 
 
-Filename: seqPSS-0.0.7.dist-info/METADATA
+Filename: seqPSS-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: seqPSS-0.0.7.dist-info/WHEEL
+Filename: seqPSS-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: seqPSS-0.0.7.dist-info/top_level.txt
+Filename: seqPSS-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: seqPSS-0.0.7.dist-info/RECORD
+Filename: seqPSS-0.0.8.dist-info/RECORD
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
-import random
+import random2
 
 
 # ## data
 
 # In[3]:
 
 
@@ -49,15 +49,15 @@
    
     # select data
     condition = (simul_data['p1'] == p1) & (simul_data['p2'] == p2) & (simul_data['p3'] == p3)
     filtered_df = simul_data[condition]
     
     dfs = []
     for i in range(n): # now, extracts by #n
-        uniq_num = random.choice(pd.unique(filtered_df['uniq_num']))
+        uniq_num = random2.choice(pd.unique(filtered_df['uniq_num']))
         chosen_df = filtered_df[filtered_df['uniq_num'] == uniq_num] #filter only uniq_num
     
         # now make new simulation data
         new_data = {
             'p1': [chosen_df['p1'].iloc[0]],
             'p2': [chosen_df['p2'].iloc[0]],
             'p3': [chosen_df['p3'].iloc[0]],
```

