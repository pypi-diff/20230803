# Comparing `tmp/cmsis_stream-1.6.1-py3-none-any.whl.zip` & `tmp/cmsis_stream-1.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 89435 bytes, number of entries: 72
+Zip file size: 89570 bytes, number of entries: 72
 -rw-rw-rw-  2.0 fat      298 b- defN 23-May-11 12:29 cmsis_stream/__init__.py
 -rw-rw-rw-  2.0 fat      546 b- defN 23-Jun-02 06:34 cmsis_stream/cmsis_stream.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/__init__.py
 -rw-rw-rw-  2.0 fat     7448 b- defN 23-May-11 12:29 cmsis_stream/cg/types.py
 -rw-rw-rw-  2.0 fat     1925 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/CFFT.py
 -rw-rw-rw-  2.0 fat     1990 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/Duplicate.py
 -rw-rw-rw-  2.0 fat     1930 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/ICFFT.py
@@ -26,15 +26,15 @@
 -rw-rw-rw-  2.0 fat     4018 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/message.py
 -rw-rw-rw-  2.0 fat      118 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/__init__.py
 -rw-rw-rw-  2.0 fat     1691 b- defN 23-Jun-02 05:41 cmsis_stream/cg/scheduler/args.py
 -rw-rw-rw-  2.0 fat     3762 b- defN 23-Jul-11 11:52 cmsis_stream/cg/scheduler/ccode.py
 -rw-rw-rw-  2.0 fat     7077 b- defN 23-Jul-11 06:04 cmsis_stream/cg/scheduler/config.py
 -rw-rw-rw-  2.0 fat    41853 b- defN 23-Jun-09 07:44 cmsis_stream/cg/scheduler/description.py
 -rw-rw-rw-  2.0 fat    10849 b- defN 23-Jun-09 12:50 cmsis_stream/cg/scheduler/graphviz.py
--rw-rw-rw-  2.0 fat    38334 b- defN 23-Jul-11 12:02 cmsis_stream/cg/scheduler/node.py
+-rw-rw-rw-  2.0 fat    38491 b- defN 23-Jul-25 05:58 cmsis_stream/cg/scheduler/node.py
 -rw-rw-rw-  2.0 fat     1868 b- defN 23-Jul-18 10:59 cmsis_stream/cg/scheduler/pythoncode.py
 -rw-rw-rw-  2.0 fat     7540 b- defN 23-Jul-11 06:29 cmsis_stream/cg/scheduler/standard.py
 -rw-rw-rw-  2.0 fat      188 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt
 -rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.linux
 -rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.mac
 -rw-rw-rw-  2.0 fat      369 b- defN 23-Jun-02 06:57 cmsis_stream/cg/scheduler/example/Makefile.windows
 -rw-rw-rw-  2.0 fat      566 b- defN 23-Jun-06 06:05 cmsis_stream/cg/scheduler/example/README.md
@@ -43,32 +43,32 @@
 -rw-rw-rw-  2.0 fat      598 b- defN 23-Jul-20 11:15 cmsis_stream/cg/scheduler/example/simple.cproject.yml
 -rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/example/simple_ac6.csolution.yml
 -rw-rw-rw-  2.0 fat     2178 b- defN 23-Jun-02 06:48 cmsis_stream/cg/scheduler/example/start_project_appnodes.h
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Jun-02 06:10 cmsis_stream/cg/scheduler/example/start_project_custom.h
 -rw-rw-rw-  2.0 fat     1798 b- defN 23-Jun-02 06:26 cmsis_stream/cg/scheduler/example/start_project_graph.py
 -rw-rw-rw-  2.0 fat      197 b- defN 23-Jun-02 06:05 cmsis_stream/cg/scheduler/example/start_project_main.c
 -rw-rw-rw-  2.0 fat      878 b- defN 23-Jul-20 11:15 cmsis_stream/cg/scheduler/example/vht.clayer.yml
--rw-rw-rw-  2.0 fat    17428 b- defN 23-Jul-20 12:35 cmsis_stream/cg/scheduler/templates/GenericNodes.h
--rw-rw-rw-  2.0 fat     2006 b- defN 23-Jul-20 12:35 cmsis_stream/cg/scheduler/templates/cg_status.h
+-rw-rw-rw-  2.0 fat    17486 b- defN 23-Aug-03 06:01 cmsis_stream/cg/scheduler/templates/GenericNodes.h
+-rw-rw-rw-  2.0 fat     2006 b- defN 23-Aug-03 06:01 cmsis_stream/cg/scheduler/templates/cg_status.h
 -rw-rw-rw-  2.0 fat      434 b- defN 23-Jun-12 07:09 cmsis_stream/cg/scheduler/templates/cmsis.cpp
 -rw-rw-rw-  2.0 fat      287 b- defN 23-Jun-12 06:56 cmsis_stream/cg/scheduler/templates/cmsis.py
 -rw-rw-rw-  2.0 fat      682 b- defN 23-Jun-12 06:56 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
 -rw-rw-rw-  2.0 fat     1232 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.cpp
--rw-rw-rw-  2.0 fat     1587 b- defN 23-Jul-19 09:23 cmsis_stream/cg/scheduler/templates/code.h
+-rw-rw-rw-  2.0 fat     1587 b- defN 23-Jul-25 13:03 cmsis_stream/cg/scheduler/templates/code.h
 -rw-rw-rw-  2.0 fat     2202 b- defN 23-Jul-19 09:25 cmsis_stream/cg/scheduler/templates/code.py
 -rw-rw-rw-  2.0 fat     3316 b- defN 23-Jul-11 11:52 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
--rw-rw-rw-  2.0 fat     5662 b- defN 23-Jul-19 09:25 cmsis_stream/cg/scheduler/templates/commonc.cpp
+-rw-rw-rw-  2.0 fat     5662 b- defN 23-Jul-25 13:03 cmsis_stream/cg/scheduler/templates/commonc.cpp
 -rw-rw-rw-  2.0 fat     1427 b- defN 23-Jun-12 05:39 cmsis_stream/cg/scheduler/templates/defineConfig.h
 -rw-rw-rw-  2.0 fat     7826 b- defN 23-Jun-09 12:52 cmsis_stream/cg/scheduler/templates/dot_template.dot
 -rw-rw-rw-  2.0 fat     7555 b- defN 23-Jun-09 12:52 cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot
 -rw-rw-rw-  2.0 fat       26 b- defN 23-Jul-17 05:58 cmsis_stream/cg/sds/__init__.py
 -rw-rw-rw-  2.0 fat     3923 b- defN 23-Jul-18 08:03 cmsis_stream/cg/sds/sds_nodes.py
 -rw-rw-rw-  2.0 fat      104 b- defN 23-Jul-18 08:25 cmsis_stream/cg/yaml/__init__.py
 -rw-rw-rw-  2.0 fat    14103 b- defN 23-Jul-20 09:07 cmsis_stream/cg/yaml/exportyaml.py
 -rw-rw-rw-  2.0 fat    15989 b- defN 23-Jul-20 09:08 cmsis_stream/cg/yaml/importyaml.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-20 12:35 cmsis_stream-1.6.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4848 b- defN 23-Jul-20 12:35 cmsis_stream-1.6.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 12:35 cmsis_stream-1.6.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       59 b- defN 23-Jul-20 12:35 cmsis_stream-1.6.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-20 12:35 cmsis_stream-1.6.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6920 b- defN 23-Jul-20 12:35 cmsis_stream-1.6.1.dist-info/RECORD
-72 files, 282593 bytes uncompressed, 78147 bytes compressed:  72.3%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Aug-03 06:01 cmsis_stream-1.7.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     5073 b- defN 23-Aug-03 06:01 cmsis_stream-1.7.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 06:01 cmsis_stream-1.7.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       59 b- defN 23-Aug-03 06:01 cmsis_stream-1.7.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-03 06:01 cmsis_stream-1.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6920 b- defN 23-Aug-03 06:01 cmsis_stream-1.7.0.dist-info/RECORD
+72 files, 283033 bytes uncompressed, 78282 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -192,26 +192,26 @@
 
 Filename: cmsis_stream/cg/yaml/exportyaml.py
 Comment: 
 
 Filename: cmsis_stream/cg/yaml/importyaml.py
 Comment: 
 
-Filename: cmsis_stream-1.6.1.dist-info/LICENSE.txt
+Filename: cmsis_stream-1.7.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cmsis_stream-1.6.1.dist-info/METADATA
+Filename: cmsis_stream-1.7.0.dist-info/METADATA
 Comment: 
 
-Filename: cmsis_stream-1.6.1.dist-info/WHEEL
+Filename: cmsis_stream-1.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: cmsis_stream-1.6.1.dist-info/entry_points.txt
+Filename: cmsis_stream-1.7.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cmsis_stream-1.6.1.dist-info/top_level.txt
+Filename: cmsis_stream-1.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cmsis_stream-1.6.1.dist-info/RECORD
+Filename: cmsis_stream-1.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmsis_stream/cg/scheduler/node.py

```diff
@@ -209,14 +209,19 @@
      def __init__(self,name):
         super().__init__(name)
 
      @property
      def arg(self):
         if isinstance(self._name,str):
              return("\"%s\"" % self._name) 
+        elif isinstance(self._name,bool):
+             if self._name:
+                return("true")
+             else:
+                return("false")
         else:
              return(str(self._name))
 
 class VarLiteral(SchedArg):
      def __init__(self,name):
         super().__init__(name)
```

## cmsis_stream/cg/scheduler/templates/GenericNodes.h

```diff
@@ -65,14 +65,15 @@
 #endif
 
 template<typename T>
 class FIFOBase{
 public:
     virtual T* getWriteBuffer(int nb)=0;
     virtual T* getReadBuffer(int nb)=0;
+    virtual ~FIFOBase() {};
     /*
 
     Below functions are only useful in asynchronous mode.
     Synchronous implementation can provide an empty
     implementation.
 
     */
@@ -311,14 +312,15 @@
 // GENERIC NODES 
 
 class NodeBase
 {
 public:
     virtual int run()=0;
     virtual int prepareForRunning()=0;
+    virtual ~NodeBase() {};
     void setID(int id){mNodeID = id;};
     int nodeID() const {return(mNodeID);};
 protected:
     int mNodeID = UNIDENTIFIED_NODE;
 };
 
 template<typename IN, int inputSize,typename OUT, int outputSize>
```

## cmsis_stream/cg/scheduler/templates/code.h

```diff
@@ -37,15 +37,15 @@
 {% for node in identifiedNodes %}
 #define {{node[0]}} {{node[1]}}
 {% endfor %}
 
 {% if config.CAPI -%}
 extern void *get_{{config.schedName}}_node(int32_t nodeID);
 {% else %}
-extern NodeBase *get_node_{{config.schedName}}(int32_t nodeID);
+extern NodeBase *get_{{config.schedName}}_node(int32_t nodeID);
 {% endif %}
 {% endif %}
 
 {% if config.heapAllocation %}
 extern int init_{{config.schedName}}({{optionalargs(True)}});
 extern void free_{{config.schedName}}({{optionalargs(True)}});
 {% endif %}
```

## cmsis_stream/cg/scheduler/templates/commonc.cpp

```diff
@@ -92,15 +92,15 @@
 CG_BEFORE_BUFFER
 static nodes_t nodes={0};
 
 {% if config.nodeIdentification %}
 {% if config.CAPI -%}
 void *get_{{config.schedName}}_node(int32_t nodeID)
 {% else %}
-NodeBase *get_node_{{config.schedName}}(int32_t nodeID)
+NodeBase *get_{{config.schedName}}_node(int32_t nodeID)
 {% endif %}
 {
     if (nodeID >= {{config.prefix | upper}}NB_IDENTIFIED_NODES)
     {
         return(NULL);
     }
     if (nodeID < 0)
```

## Comparing `cmsis_stream-1.6.1.dist-info/LICENSE.txt` & `cmsis_stream-1.7.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cmsis_stream-1.6.1.dist-info/METADATA` & `cmsis_stream-1.7.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsis-stream
-Version: 1.6.1
+Version: 1.7.0
 Summary: CMSIS-Stream graph description
 Home-page: https://github.com/ARM-software/CMSIS-Stream
 Author: Copyright (C) 2010-2023 ARM Limited or its affiliates. All rights reserved.
 Author-email: christophe.favergeon@arm.com
 License: License :: OSI Approved :: Apache Software License
 Project-URL: Bug Reports, https://github.com/ARM-software/CMSIS-Stream/issues
 Project-URL: Source, https://github.com/ARM-software/CMSIS-Stream
@@ -42,14 +42,20 @@
 
 * Define new compute nodes
 * Connect them into a dataflow graph to process streams
 * Generate at build time a static C scheduler to run the graph on your target (no need of an RTOS)
 
 # Change history
 
+## Version 1.7.0:
+
+* Improvements to GenericNodes.h when building with gcc
+* `addLiteral` can now also use `bool` values from Python
+* Naming of the function to get a node was not consistent between the C and CPP APIs
+
 ## Version 1.6.1:
 
 * Correction to 1.6.0 : Missing YAML module 
 
 ## Version 1.6.0:
 
 * SDS sensor and recorder nodes to interact with the [Arm SDS Framework](https://github.com/ARM-software/SDS-Framework/tree/main) to record stream of samples and replay them in Arm Virtual Hardware
```

## Comparing `cmsis_stream-1.6.1.dist-info/RECORD` & `cmsis_stream-1.7.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 cmsis_stream/cg/nodes/host/message.py,sha256=e2hto5-Ly08sUCKN8F94qH3O3lAxcGGIGBLkf6cLJCY,4018
 cmsis_stream/cg/scheduler/__init__.py,sha256=-GMWFk8b3LpReDjD7yHF_SLrFDu5PRZuxN1RbjkY6nk,118
 cmsis_stream/cg/scheduler/args.py,sha256=mepFm7CJa2wnB-21a-h1FrufP5KtI78l_B3HNb87ayk,1691
 cmsis_stream/cg/scheduler/ccode.py,sha256=NBv9eqec1TdyhRcn2-ZwBb7sVeIc4SwmS5rOStt0HoY,3762
 cmsis_stream/cg/scheduler/config.py,sha256=SOSgp7rDFccmVEjikyodwUczN9hfdeJAKFQnTmu6E_w,7077
 cmsis_stream/cg/scheduler/description.py,sha256=FPLRFTxk3mGduq2_hLPxNiL5MNzpFDzl-Nk1ivyyBVk,41853
 cmsis_stream/cg/scheduler/graphviz.py,sha256=TwiDslHOJlek2otwA_5sspTWaf_trLV4QMthpv6fzM4,10849
-cmsis_stream/cg/scheduler/node.py,sha256=b_tO27sp1gphHM710mwRrHsOW8aezwxzJHDY_cSsR3s,38334
+cmsis_stream/cg/scheduler/node.py,sha256=fi5-bhXRjLiP4EsvkFOA-sDT9MrSVTS5Pj5WwFb9Wps,38491
 cmsis_stream/cg/scheduler/pythoncode.py,sha256=A5iuUMvzgDJCe7uNyeuhtZA0wZfc4PeSeDXDymeCaKc,1868
 cmsis_stream/cg/scheduler/standard.py,sha256=LFenG7Da-TBzzp_Pl2BKAzJj3li9WFLNOJF4xwnkoY4,7540
 cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt,sha256=Yn4YtMgyACdeesvFcPkP1xZ9Q8rIEarIAIrJeQNn3sw,188
 cmsis_stream/cg/scheduler/example/Makefile.linux,sha256=4x9Z6tbRIswUvBQuTuD9t0Co-DCwEGevAnaMc3CC5NU,192
 cmsis_stream/cg/scheduler/example/Makefile.mac,sha256=-2ldN02pnOEKwS1QqxY9-97qnUse6MEDZO9Ru1CkplQ,267
 cmsis_stream/cg/scheduler/example/Makefile.windows,sha256=p6ic8tdH0H0Fm6A8-877JIvIqgnhaScSjUKNSgB7Wb8,369
 cmsis_stream/cg/scheduler/example/README.md,sha256=_o0nMzYUELDms9o9Gh__4fuOTYqUAwabijVBSHkqsiA,566
@@ -42,31 +42,31 @@
 cmsis_stream/cg/scheduler/example/simple.cproject.yml,sha256=fFDUn3xWbqpvstxwcIXLAP7UFc7QrSK7-a383ZsJyZM,598
 cmsis_stream/cg/scheduler/example/simple_ac6.csolution.yml,sha256=0VoVxmTd-uY5ChO-uLZeNKZ7nd9GRB1aruqgSavSnFc,1416
 cmsis_stream/cg/scheduler/example/start_project_appnodes.h,sha256=LDAWX_fxyxi9y1WScVRdx0mWBQX67y06DYPTWGks1As,2178
 cmsis_stream/cg/scheduler/example/start_project_custom.h,sha256=_Hk_xhNBISqUU61sXkhmQfeG9YjmoyVPD5TD7a_P0lc,73
 cmsis_stream/cg/scheduler/example/start_project_graph.py,sha256=gTSFIiNYAVGFSSQ-aSs6_BL6bMbk0oEIjk8d32fr9AM,1798
 cmsis_stream/cg/scheduler/example/start_project_main.c,sha256=CFz0ZKrUafNi9bF3fIVcBBGhrwFNoxmxxODSaDCO4sQ,197
 cmsis_stream/cg/scheduler/example/vht.clayer.yml,sha256=BOZ44mIcb3P2r43vAyff5QkI8r75I5HIzwLOBqcyu2g,878
-cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=sgw6-HeFS0l6G5IVLBhbCmpHHWPWL3HjbrYEKj0oxuI,17428
+cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=JV0OBPN3W-yLnq8VMsh9bDeStWbHjCT_IKWimKUUF2Q,17486
 cmsis_stream/cg/scheduler/templates/cg_status.h,sha256=1ZBdMG2s9FMyTzdvFtxpPIK624-jnfRd_Q2Qxe_MwTM,2006
 cmsis_stream/cg/scheduler/templates/cmsis.cpp,sha256=Fw5MHQqCZt2srXAuJjvXSHS1m-78DGdT4sGHDEQgG28,434
 cmsis_stream/cg/scheduler/templates/cmsis.py,sha256=iC5sSkuZ01iGT0dBfqNPUbMKE86y10-0Gj8fLOfbgi8,287
 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp,sha256=JMn_nIJiPYSnu7qVKHS8jKEtAjktGpWSyzxg-r2olgw,682
 cmsis_stream/cg/scheduler/templates/code.cpp,sha256=uiJEAmZyGoMq_AqYqZ3aXRyX9L7cRKdkUFazGLc1eP0,1232
-cmsis_stream/cg/scheduler/templates/code.h,sha256=aYlk0BrpUYIRaMkhP7Whujfvijza_Z-H1dYrzcmsYFk,1587
+cmsis_stream/cg/scheduler/templates/code.h,sha256=HrtY5jfNiiAAduF5WsOjHVr8HC9JLvt_MoO-y0tLJdU,1587
 cmsis_stream/cg/scheduler/templates/code.py,sha256=K77zYiYQdqMGynPVABcWNmxqdGFx9cMfV1yOvuc4u8M,2202
 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp,sha256=QoQiLGGb_AUbeTE2LyaOneAkkfccxl4Ah-K-AbVoh-M,3316
-cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=AwlzR5yhV4geF5FjDYmXHWLmiqMI7aWZ2sLBbH3_Gzo,5662
+cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=HyjkpVOV_1bA16HtIrCryTn2EwwOrG9C_6RwyWs6V3Y,5662
 cmsis_stream/cg/scheduler/templates/defineConfig.h,sha256=KoW0i45XF2-Ghcs-snyqlyysT0SfcKVJcStrBotO1gE,1427
 cmsis_stream/cg/scheduler/templates/dot_template.dot,sha256=_4a8oe0kvSDx-Hl1P0aIZMFAOYMpknhGkeOUI8Nqy6g,7826
 cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot,sha256=wLfhZpZS0VHm43dpaQYZBSd8ftd0KdUS_hSo2cSHwLU,7555
 cmsis_stream/cg/sds/__init__.py,sha256=TCh0rypl6S4qKWie66n0ZGYaUGznTLIWOFl_1-2XvLE,26
 cmsis_stream/cg/sds/sds_nodes.py,sha256=NiOBo0gIGYdb9Am0RyFvivrQbDJKpnvMHl4iOZ7zDbc,3923
 cmsis_stream/cg/yaml/__init__.py,sha256=nv4KwU4bqDQoREFYliOSnL98MkQxwMh40Kmy8aGfReY,104
 cmsis_stream/cg/yaml/exportyaml.py,sha256=i0r4uZ2Cevwz7B_Ma55Va0RajBXlpAEkpQqZhuJo1qI,14103
 cmsis_stream/cg/yaml/importyaml.py,sha256=xNl6FiXuxMmIxIq8PMJw9HbF8wnLWCRwmGAUmBaXMe4,15989
-cmsis_stream-1.6.1.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
-cmsis_stream-1.6.1.dist-info/METADATA,sha256=2J9IdlsF82UZ4MB5YzBV360JdXYS6uOzEfKNSvz1L0A,4848
-cmsis_stream-1.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cmsis_stream-1.6.1.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
-cmsis_stream-1.6.1.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
-cmsis_stream-1.6.1.dist-info/RECORD,,
+cmsis_stream-1.7.0.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
+cmsis_stream-1.7.0.dist-info/METADATA,sha256=o5YeaoyHTix94-KA8p2pOFvwjeueodKDwuHGvIvnDQo,5073
+cmsis_stream-1.7.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+cmsis_stream-1.7.0.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
+cmsis_stream-1.7.0.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
+cmsis_stream-1.7.0.dist-info/RECORD,,
```

