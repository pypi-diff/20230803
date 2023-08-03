# Comparing `tmp/seqPSS-0.0.5-py3-none-any.whl.zip` & `tmp/seqPSS-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 2788 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat      822 b- defN 23-Aug-02 23:53 seqPSS/__init__.py
--rw-rw-rw-  2.0 fat     1894 b- defN 23-Aug-02 23:59 seqPSS/seqPSS.py
--rw-rw-rw-  2.0 fat      324 b- defN 23-Aug-03 00:00 seqPSS-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 00:00 seqPSS-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-03 00:00 seqPSS-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      439 b- defN 23-Aug-03 00:00 seqPSS-0.0.5.dist-info/RECORD
-6 files, 3578 bytes uncompressed, 1994 bytes compressed:  44.3%
+-rw-rw-rw-  2.0 fat     1877 b- defN 23-Aug-03 00:04 seqPSS/seqPSS.py
+-rw-rw-rw-  2.0 fat      325 b- defN 23-Aug-03 00:05 seqPSS-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 00:05 seqPSS-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-03 00:05 seqPSS-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      439 b- defN 23-Aug-03 00:05 seqPSS-0.0.6.dist-info/RECORD
+6 files, 3562 bytes uncompressed, 1994 bytes compressed:  44.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: seqPSS/__init__.py
 Comment: 
 
 Filename: seqPSS/seqPSS.py
 Comment: 
 
-Filename: seqPSS-0.0.5.dist-info/METADATA
+Filename: seqPSS-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: seqPSS-0.0.5.dist-info/WHEEL
+Filename: seqPSS-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: seqPSS-0.0.5.dist-info/top_level.txt
+Filename: seqPSS-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: seqPSS-0.0.5.dist-info/RECORD
+Filename: seqPSS-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## seqPSS/seqPSS.py

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-# In[6]:
+# In[14]:
 
 
 import numpy as np
 import pandas as pd
-from random import *
+import random2
 
 
 # ## data
 
-# In[3]:
+# In[15]:
 
 
 path = '../sampleData/'
 simul_data = pd.read_csv(path + 'concatenated_df.csv')
 
 
 # ## simulation code
 
-# In[11]:
+# In[16]:
 
 
 def simple_Simulation(p1: 'int', p2: 'int', p3: 'int', n = 10):
     '''
     to make simple simulation
     
     Parameters
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
@@ -85,13 +85,7 @@
 
 
 # In[ ]:
 
 
 
 
-
-# In[ ]:
-
-
-
-
```

