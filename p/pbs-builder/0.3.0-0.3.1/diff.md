# Comparing `tmp/pbs_builder-0.3.0.tar.gz` & `tmp/pbs_builder-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbs_builder-0.3.0.tar", max compression
+gzip compressed data, was "pbs_builder-0.3.1.tar", max compression
```

## Comparing `pbs_builder-0.3.0.tar` & `pbs_builder-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-07-19 02:02:11.000000 pbs_builder-0.3.0/LICENSE
--rw-r--r--   0        0        0      697 2023-07-31 08:58:00.000000 pbs_builder-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-07-19 02:03:05.000000 pbs_builder-0.3.0/pbs_builder/__init__.py
--rwxr-xr-x   0        0        0    22740 2023-07-31 09:48:03.000000 pbs_builder-0.3.0/pbs_builder/bin/pestat
--rwxr-xr-x   0        0        0      203 2023-07-31 09:44:00.000000 pbs_builder-0.3.0/pbs_builder/pestat.py
--rwxr-xr-x   0        0        0    36544 2023-07-19 02:02:11.000000 pbs_builder-0.3.0/pbs_builder/qbatch.py
--rwxr-xr-x   0        0        0      695 2023-07-19 02:02:11.000000 pbs_builder-0.3.0/pbs_builder/qcancel.py
--rw-r--r--   0        0        0      738 2023-07-31 09:45:05.000000 pbs_builder-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 pbs_builder-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-19 02:02:11.000000 pbs_builder-0.3.1/LICENSE
+-rw-r--r--   0        0        0      812 2023-08-03 07:54:16.000000 pbs_builder-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 02:03:05.000000 pbs_builder-0.3.1/pbs_builder/__init__.py
+-rwxr-xr-x   0        0        0    24040 2023-08-03 07:53:00.000000 pbs_builder-0.3.1/pbs_builder/bin/pestat
+-rwxr-xr-x   0        0        0      203 2023-07-31 09:44:00.000000 pbs_builder-0.3.1/pbs_builder/pestat.py
+-rwxr-xr-x   0        0        0    36544 2023-07-19 02:02:11.000000 pbs_builder-0.3.1/pbs_builder/qbatch.py
+-rwxr-xr-x   0        0        0      695 2023-07-19 02:02:11.000000 pbs_builder-0.3.1/pbs_builder/qcancel.py
+-rw-r--r--   0        0        0      745 2023-08-03 07:53:20.000000 pbs_builder-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1564 1970-01-01 00:00:00.000000 pbs_builder-0.3.1/PKG-INFO
```

### Comparing `pbs_builder-0.3.0/LICENSE` & `pbs_builder-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pbs_builder-0.3.0/README.md` & `pbs_builder-0.3.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # PBS-builder
 
 A simplified version of workflow management system for scalable data analysis.
 
 # Change log
 
-- Version 0.2.0: move sample_sheet from header to job section, add group_sheet support.
+- Version 0.3.1: add allocated/total gpus in `pestat` output
+- Version 0.3.0: include `pestat` in package data
+- Version 0.2.0: move `sample_sheet` from header to job section, add `group_sheet` support.
 - Version 0.1.0: first functional version.
 
 # Usage
 
 Please refer to our [wiki](https://bioinfo.biols.ac.cn/git/zhangjy/pbs-builder/wiki/_pages) for detailed instructions.
 
 # Installation
```

### Comparing `pbs_builder-0.3.0/pbs_builder/bin/pestat` & `pbs_builder-0.3.1/pbs_builder/bin/pestat`

 * *Files 3% similar despite different names*

```diff
@@ -20,26 +20,31 @@
 # The baseline netload information may be generated from cron, say, every 10 minutes
 # by this crontab entry:
 # */10 * * * * /usr/local/bin/pestat -C > /dev/null
 # Otherwise the default netload file is the user-specific file netload.$USER.
 # Subsequent pestat commands will use the baseline netload.
 
 # Author: zhangjinyang@biols.ac.cn
-# Version: 2.15
+# Version: 2.16
 # Update Notes:
+#  - Add information of allocated and total number of available gpus
+# Date 2023-08-03 15:41:00
+#
 #  - Support to specified queue, if no nodelist given, show all nodes
 #  - Support to get job list from \"jobs\"(jobs_from_status=0), NOT "status->jobs"
+# Date: 2020-08-17 20:27:04
+#
 #  - Reapire numtask[] error for Torque v4 (tasklist is not splited with space)
 #  - Reapire disorder for columns with different width, formating them
 # Date: 2020-08-17 20:27:04
 
 # Author: Ole.H.Nielsen@fysik.dtu.dk
 # URL: ftp://ftp.fysik.dtu.dk/pub/Torque/pestat
 
-VERSION="pestat version 2.15.  Date: 17 Aug 2020"
+VERSION="pestat version 2.16.  Date: 03 Aug 2023"
 
 # Locations of command and directories
 # Replace with path to pbsnodes and qstat commands if they are not included in $PATH
 PBSNODES=pbsnodes
 QSTAT=qstat
 AWK=/bin/awk
 
@@ -69,14 +74,15 @@
     -s: Listing only nodes in specific state (default: show all nodes)
     -f: Listing only nodes that are flagged by \*
     -d: Listing also nodes that are down
     -c/-n: Color/no color output
     -u username: Print only user <username> (do not use with the -g flag)
     -g groupname: Print only users in group <groupname>
     -j jobs: List only nodes with at least <jobs> running jobs 
+    -p length: Length of allocated processor bars
     -C: Use with cron: Netload file will be saved as $NETLOAD_CRON
     -h: Print this help information
     -v: Version information
 EOF
 }
 
 NODEBLACKLIST="node78:node161:node162:node163:node164:node165:node166:node167:node168:node169:node170"
@@ -138,15 +144,15 @@
 fi
 
 #
 # Process command arguments
 #
 listflagged=0
 listalljobs=0
-while getopts "aq:s:fdcnvu:g:j:Ch" options; do
+while getopts "aq:s:fdcnvu:g:j:Chp:" options; do
     case $options in
         a )     listalljobs=1
             # List all jobs on nodes
             ;;
         q )     queue=$OPTARG
             echo Listing only nodes in queue $queue
             # List only nodes in queue
@@ -172,14 +178,17 @@
             ;;
         g )     groupname=$OPTARG
             echo Select only users in group $groupname
             ;;
         j )     minjobs=$OPTARG
             echo List only nodes with at least $minjobs running jobs
             ;;
+        p )     proglen=$OPTARG
+            echo Length of processor bar
+            ;;
         C ) NETLOADFILE=$NETLOAD_CRON
             NETLOADWRITE=1
             ;;
         v ) echo $VERSION
             exit 0;;
         h|? ) usage
             exit 1;;
@@ -249,15 +258,15 @@
 
 #
 # Show the Torque node status and parse the results
 #
 
 $PBSNODES -a | $AWK -v listflagged=$listflagged -v listdownnodes=$listdownnodes \
     -v listalljobs=$listalljobs -v NODEBLACKLIST=$NODEBLACKLIST -v QUEUEBLACKLIST=$QUEUEBLACKLIST \
-    -v colors=$colors -v username=$username -v groupname=$groupname -v minjobs=$minjobs \
+    -v colors=$colors -v username=$username -v groupname=$groupname -v minjobs=$minjobs -v plen=$proglen \
     -v NODENAMEFORMAT=$NODENAMEFORMAT \
     -v QSTAT=$QSTAT -v queue=$queue -v tstate=$tstate \
     -v netloadprint=$netloadprint -v NETLOADFILE=$NETLOADFILE -v NETLOADWRITE=$NETLOADWRITE \
     -v netloadage=$netloadage -v NETLOADTHRES=$NETLOADTHRES -v NETLOADSCALE=$NETLOADSCALE '
 BEGIN {
     # Define terminal colors for the output if requested
     if (colors != 0) {
@@ -353,31 +362,36 @@
       BLACKNODE[nodelist[i]] = nodelist[i]
     }
 
     queuenum = split(QUEUEBLACKLIST, queuelist, ":")
     for (i = 1; i <= queuenum; ++i) {
       BLACKQUEUE[queuelist[i]] = queuelist[i]
     }
-
+    
+    if (plen == "") plen = 10
+    ptemplate = "                              "
+    pempty = substr(ptemplate, 1, plen)
     # Print a header line
+
     printf (NODENAMEFORMAT, YELLOW, "Node")
-    printf (" %sstate    load%     resi      pmem      mem  ncpu  proc                         queue    usrs tasks NetMbit jobids/users %s\n", YELLOW, NORMAL)
+    printf (" %sstate    load%     resi      pmem      mem  ncpu  proc %s     ngpu queue    usrs tasks NetMbit jobids/users %s\n", YELLOW, pempty, NORMAL)
 }
 #
 # Parse the output of pbsnodes
 #
 NF==1 { node=$1             # 1st line is nodename
     nodename[node] = node       # Node name
     getline             # Get the next input line
     numjobs[node] = 0               # Torque jobs on the node
     numtasks[node] = 0              # Number of tasks started by Torque on the node
     listnode=0          # Set to > 0 if this node gets flagged
     userusesnode=0          # If this node is used by the selected user 
     groupusesnode=0         # If this node is used by a user in the selected group 
     allocated = 0
+    allocated_gpu = 0
     njob = 0
     while (NF >= 3) {       # Read a number of non-blank lines
         if ($1 == "state") {
             if ($3 == "job-exclusive")          state[node] = "excl"
             else if ($3 == "job-exclusive,busy")        state[node] = "busy"
             else if ($3 == "busy")              state[node] = "busy"
             else if ($3 == "free")              state[node] = "free"
@@ -461,14 +475,32 @@
                 else if (b[1]=="loadave")   loadave[node]=b[2]
                 else if (b[1]=="netload")   netload[node]=b[2]
                 else if (b[1]=="size")      size[node]=b[2]
                 else if (b[1]=="rectime")   rectime[node]=b[2]
                 else if (b[1]=="message")   msg[node]=b[2]
             }
         }
+        else if ($1 == "gpus")  ngpu[node] = $3
+        else if ($1 == "gpu_status") {
+            # Get the occupied gpus
+            split (substr($0,19), gstatus, ",")
+            for (field in gstatus) {
+                split (gstatus[field], g, "=")
+                if (g[1]=="gpu_display") {}
+                else if (g[1]=="timestamp") {}
+                else if (g[1]=="driver_ver") {}
+                else if (substr(g[1], 1, 3) == "gpu") {
+                    gid = g[1]
+                    split (gstatus[field], g2, ";")
+                    for (gfield in g2) {
+                        if (g2[gfield] == "gpu_state=Exclusive") allocated_gpu++
+                    }
+                }
+            } 
+        }
         getline         # Get the next input line
     }
 
     if (NETLOADWRITE == 1) {
         # Save netload information to file (format: nodename network-bytes list-of-jobids)
         print nodename[node], netload[node], jobidlist[node] >> NETLOADFILE
     }
@@ -597,29 +629,33 @@
         jobcolor=NORMAL
     }
 
     # Listing of down nodes?
     if (listdownnodes == 0 && state[node] == "down") listnode=0
 
     # Progressbar
-    nprog = int(20 * allocated / np[node])
-    fill = "...................."
-    bar = "####################"
+    nprog = int(plen * allocated / np[node])
+    fill = ".............................."
+    bar = "##############################"
+
+    # GPU status
+    gstat = sprintf("%d/%d", allocated_gpu, ngpu[node])
     
     # Print a 1-line list for this node
     if (!listflagged || listnode > 0) {
         printf (NODENAMEFORMAT, NORMAL, node)
         printf (" %s%s%1s%s ", statecolor, state[node], stateflag, NORMAL)
         printf (" %s%6.2f%1s%s", loadcolor, loadave[node], loadflag, NORMAL)
         printf (" %s%8.2f%1s%s", statecolor, resi/1024, resiflag, NORMAL)
         printf (" %s%8.2f%s", statecolor, physmem[node]/1024/1024, NORMAL)
         printf (" %s%8.2f%s", statecolor, aval/1024, NORMAL)
         printf (" %s%5d%s", statecolor, np[node], NORMAL)
         printf (" %s%5d%s", statecolor, allocated, NORMAL)
-        printf (" %s[%s%s]%s ", statecolor, substr(bar, 1, nprog), substr(fill, 1, 20 - nprog), NORMAL)
+        printf (" %s[%s%s]%s ", statecolor, substr(bar, 1, nprog), substr(fill, 1, plen - nprog), NORMAL)
+        printf (" %s%5s%s", statecolor, gstat, NORMAL)
         printf (" %s%-8s%s", NORMAL, properties[node], NORMAL)
         printf (" %s%2d/%-2d%1s%s", sesscolor, nsessions[node], nusers[node], sessflag, NORMAL)
         printf (" %s%3d%1s%s", jobcolor, numtasks[node], jobflag, NORMAL)
         if (netloadprint == 1) {
             printf (" %s%5d%1s%s", netmbitcolor, netmbit, netloadflag, NORMAL)
         } else
             printf ("    -  ")
```

### Comparing `pbs_builder-0.3.0/pbs_builder/qbatch.py` & `pbs_builder-0.3.1/pbs_builder/qbatch.py`

 * *Files identical despite different names*

### Comparing `pbs_builder-0.3.0/pbs_builder/qcancel.py` & `pbs_builder-0.3.1/pbs_builder/qcancel.py`

 * *Files identical despite different names*

### Comparing `pbs_builder-0.3.0/pyproject.toml` & `pbs_builder-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "pbs-builder"
-version = "0.3.0"
+version = "0.3.1"
 description = "The workflow management system for scalable data analyses."
 authors = ["Jinyang Zhang <zhangjinyang@biols.ac.cn>"]
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.7"
 ]
-include = ["pbs_builder/bin/pestat"]
+include = [
+    "pbs_builder/bin/pestat",
+]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 tomli = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
```

### Comparing `pbs_builder-0.3.0/PKG-INFO` & `pbs_builder-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbs-builder
-Version: 0.3.0
+Version: 0.3.1
 Summary: The workflow management system for scalable data analyses.
 License: LICENSE
 Author: Jinyang Zhang
 Author-email: zhangjinyang@biols.ac.cn
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,17 @@
 
 # PBS-builder
 
 A simplified version of workflow management system for scalable data analysis.
 
 # Change log
 
-- Version 0.2.0: move sample_sheet from header to job section, add group_sheet support.
+- Version 0.3.1: add allocated/total gpus in `pestat` output
+- Version 0.3.0: include `pestat` in package data
+- Version 0.2.0: move `sample_sheet` from header to job section, add `group_sheet` support.
 - Version 0.1.0: first functional version.
 
 # Usage
 
 Please refer to our [wiki](https://bioinfo.biols.ac.cn/git/zhangjy/pbs-builder/wiki/_pages) for detailed instructions.
 
 # Installation
```

