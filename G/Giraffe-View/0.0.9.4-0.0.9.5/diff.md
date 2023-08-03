# Comparing `tmp/Giraffe_View-0.0.9.4.tar.gz` & `tmp/Giraffe_View-0.0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Giraffe_View-0.0.9.4.tar", last modified: Sat Jul 22 12:04:04 2023, max compression
+gzip compressed data, was "Giraffe_View-0.0.9.5.tar", last modified: Sat Jul 22 13:24:27 2023, max compression
```

## Comparing `Giraffe_View-0.0.9.4.tar` & `Giraffe_View-0.0.9.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-22 12:04:04.872175 Giraffe_View-0.0.9.4/
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-22 12:04:04.868175 Giraffe_View-0.0.9.4/Giraffe_View/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-22 06:47:12.000000 Giraffe_View-0.0.9.4/Giraffe_View/__init__.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2838 2023-07-22 11:58:17.000000 Giraffe_View-0.0.9.4/Giraffe_View/estimated_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4755 2023-07-22 11:58:35.000000 Giraffe_View-0.0.9.4/Giraffe_View/function.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3287 2023-07-22 11:58:52.000000 Giraffe_View-0.0.9.4/Giraffe_View/gc_bias.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5819 2023-07-22 12:00:28.000000 Giraffe_View-0.0.9.4/Giraffe_View/giraffe
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4752 2023-07-22 12:01:18.000000 Giraffe_View-0.0.9.4/Giraffe_View/homopolymer.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2953 2023-07-22 07:03:46.000000 Giraffe_View-0.0.9.4/Giraffe_View/observed_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     8167 2023-07-22 10:55:54.000000 Giraffe_View-0.0.9.4/Giraffe_View/plot.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2157 2023-07-22 09:24:19.000000 Giraffe_View-0.0.9.4/Giraffe_View/regional_modification.py
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-22 12:04:04.872175 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5285 2023-07-22 12:04:04.000000 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/PKG-INFO
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-22 12:04:04.000000 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/SOURCES.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-22 12:04:04.000000 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/dependency_links.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       88 2023-07-22 12:04:04.000000 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/requires.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-22 12:04:04.000000 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/top_level.txt
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-22 06:47:12.000000 Giraffe_View-0.0.9.4/LICENSE
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5285 2023-07-22 12:04:04.872175 Giraffe_View-0.0.9.4/PKG-INFO
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4875 2023-07-22 11:56:21.000000 Giraffe_View-0.0.9.4/README.md
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-22 12:04:04.872175 Giraffe_View-0.0.9.4/setup.cfg
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      965 2023-07-22 12:03:15.000000 Giraffe_View-0.0.9.4/setup.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-22 13:24:27.377711 Giraffe_View-0.0.9.5/
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-22 13:24:27.377711 Giraffe_View-0.0.9.5/Giraffe_View/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-22 12:14:39.000000 Giraffe_View-0.0.9.5/Giraffe_View/__init__.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2838 2023-07-22 12:14:39.000000 Giraffe_View-0.0.9.5/Giraffe_View/estimated_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4755 2023-07-22 12:14:39.000000 Giraffe_View-0.0.9.5/Giraffe_View/function.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3287 2023-07-22 12:25:12.000000 Giraffe_View-0.0.9.5/Giraffe_View/gc_bias.py
+-rwxrwxrwx   0 xudongliu  (1000) xudongliu  (1000)     5848 2023-07-22 12:57:48.000000 Giraffe_View-0.0.9.5/Giraffe_View/giraffe
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4752 2023-07-22 12:14:39.000000 Giraffe_View-0.0.9.5/Giraffe_View/homopolymer.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2953 2023-07-22 12:14:39.000000 Giraffe_View-0.0.9.5/Giraffe_View/observed_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     8149 2023-07-22 13:12:44.000000 Giraffe_View-0.0.9.5/Giraffe_View/plot.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2157 2023-07-22 12:14:39.000000 Giraffe_View-0.0.9.5/Giraffe_View/regional_modification.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-22 13:24:27.377711 Giraffe_View-0.0.9.5/Giraffe_View.egg-info/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5261 2023-07-22 13:24:27.000000 Giraffe_View-0.0.9.5/Giraffe_View.egg-info/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-22 13:24:27.000000 Giraffe_View-0.0.9.5/Giraffe_View.egg-info/SOURCES.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-22 13:24:27.000000 Giraffe_View-0.0.9.5/Giraffe_View.egg-info/dependency_links.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       88 2023-07-22 13:24:27.000000 Giraffe_View-0.0.9.5/Giraffe_View.egg-info/requires.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-22 13:24:27.000000 Giraffe_View-0.0.9.5/Giraffe_View.egg-info/top_level.txt
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-22 12:14:39.000000 Giraffe_View-0.0.9.5/LICENSE
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5261 2023-07-22 13:24:27.377711 Giraffe_View-0.0.9.5/PKG-INFO
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4850 2023-07-22 12:59:52.000000 Giraffe_View-0.0.9.5/README.md
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-22 13:24:27.377711 Giraffe_View-0.0.9.5/setup.cfg
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      965 2023-07-22 12:14:52.000000 Giraffe_View-0.0.9.5/setup.py
```

### Comparing `Giraffe_View-0.0.9.4/Giraffe_View/estimated_read_accuracy.py` & `Giraffe_View-0.0.9.5/Giraffe_View/estimated_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.4/Giraffe_View/function.py` & `Giraffe_View-0.0.9.5/Giraffe_View/function.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.4/Giraffe_View/gc_bias.py` & `Giraffe_View-0.0.9.5/Giraffe_View/gc_bias.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 		ff.write(str(i) + "\t" + str(ave_dp) + "\t" + str(len(tmp)) + "\n")
 	ff.close()
 
 	#get the 95% data for downstream normalization
 	df = pd.read_csv("results/GC_bias/GC_bias_raw.txt", delim_whitespace=True)
 	max_number = df["number"].max()
 	total_number = df["number"].sum()
-	porportion = 0.95
+	porportion = 0.90
 	tmp = df[df["number"] == max_number].copy()
 	
 	if len(tmp) == 1:
 		for i in tmp["GC_content"]:
 			start = i
 			end = i
```

### Comparing `Giraffe_View-0.0.9.4/Giraffe_View/giraffe` & `Giraffe_View-0.0.9.5/Giraffe_View/giraffe`

 * *Files 11% similar despite different names*

```diff
@@ -15,27 +15,32 @@
 
 def observed(args):
     print_with_color("Start data processing!")
     Data_process(args.input, args.ref, args.cpu)
     
     print_with_color("Start observed accuracy analysis!")
     observed_accuracy("results/observed_quality/tmp.sort.bam")
-    
+
+    if args.plot:
+    	print_with_color("Start plotting results of observe read accuracy!")
+    	plot_observe_acc()
+    else:
+    	pass
+
     print_with_color("Start homopolymer identification!")
     homopolymer_from_bam("results/observed_quality/tmp.sort.bam")
     homopolymer_summary_1("results/observed_quality/homo.txt")
     homopolymer_summary_2()
-    
+
     if args.plot:
-        print_with_color("Start plotting!")
-        plot_observe()
-        print_with_color("Observe read quality analysis finished!")
+    	print_with_color("Start plotting results of homopolymer identification!")
+    	plot_observe_homo()
     else:
-        print_with_color("Observe read quality analysis finished!")
-    
+    	pass
+
     mes = "The results are available at " + str(working_path) + "/results/observed_quality!"
     print_with_color(str(mes))
 
 def estimated(args):
     mkdir_d("estimated_quality")
 
     print_with_color("Start estimated read accuracy analysis!")
@@ -78,17 +83,14 @@
         print_with_color("Analysis finished!")
     else:
         print_with_color("Analysis finished!")
 
     mes = "The results are available at " + str(working_path) + "/results/regional_modification!"
     print_with_color(str(mes))
 
-
-
-
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(prog="giraffe", description="A tool to help you assess quality of ONT data.")
 
     # Define subparsers
     subparsers = parser.add_subparsers(dest='function', help="")
     observed_parser = subparsers.add_parser('observe', help='Observed quality in accuracy, mismatch, and homopolymer identification')
     observed_parser.add_argument("--input", type=str, metavar="<fastq>", required=True, help="input reads")
@@ -97,21 +99,21 @@
     observed_parser.add_argument("--plot", required=False, help="Results visualization", action='store_true')
 
     estimated_parser = subparsers.add_parser('estimate', help='Estimated read accuracy')
     estimated_parser.add_argument("--input", type=str, metavar="<fastq>", required=True, help="input reads")
     estimated_parser.add_argument("--cpu", type=int, metavar="<number>", required=False, help="number of cpu (default:10)", default=10)
     estimated_parser.add_argument("--plot", required=False, help="Results visualization", action='store_true')
 
-    GC_bias_parser = subparsers.add_parser('gc_bias', help='Relationship between GC content and depth')
+    GC_bias_parser = subparsers.add_parser('gcbias', help='Relationship between GC content and depth')
     GC_bias_parser.add_argument("--ref", type=str, metavar="<reference>", required=True, help="input reference file")
     GC_bias_parser.add_argument("--input", type=str, metavar="<sam/bam>", required=True, help="input bam/sam file")
     GC_bias_parser.add_argument("--binsize", type=int, metavar="", required=False, help="input bin size (default:1000)", default=1000)
     GC_bias_parser.add_argument("--plot", required=False, help="Results visualization", action='store_true')
 
-    methylation_parser = subparsers.add_parser('modi_bin', help='Average modification proportion of bins')
+    methylation_parser = subparsers.add_parser('modibin', help='Average modification proportion of bins')
     methylation_parser.add_argument("--input", type=str, metavar="<bed>", required=True, help="input modificated bed file, please use the .bed as the file suffix")
     methylation_parser.add_argument("--ref", type=str, metavar="<reference>", required=True, help="input position file with CSV format, please use the .csv as the file suffix")
     methylation_parser.add_argument("--cpu", type=int, metavar="<number>", required=False, help="number of cpu (default:10)", default=10)
     methylation_parser.add_argument("--plot", required=False, help="Results visualization", action='store_true')
 
     # Add function to print help if no arguments are provided
     if len(sys.argv) == 1:
@@ -120,15 +122,15 @@
 
     args = parser.parse_args()
 
     # Call the appropriate function based on the subparser used
     if args.function == "observe":
         observed(args)
 
-    elif args.function == "modi_bin":
+    elif args.function == "modibin":
         methylation(args)
 
-    elif args.function == "gc_bias":
+    elif args.function == "gcbias":
         GC_bias(args)
 
     elif args.function == "estimate":
         estimated(args)
```

### Comparing `Giraffe_View-0.0.9.4/Giraffe_View/homopolymer.py` & `Giraffe_View-0.0.9.5/Giraffe_View/homopolymer.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.4/Giraffe_View/observed_read_accuracy.py` & `Giraffe_View-0.0.9.5/Giraffe_View/observed_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.4/Giraffe_View/plot.py` & `Giraffe_View-0.0.9.5/Giraffe_View/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from plotnine import * 
 import pandas as pd
 import numpy as np
 import warnings
 
 warnings.filterwarnings('ignore')
 
-def plot_observe():
+def plot_observe_acc():
 	df=pd.read_csv("./results/observed_quality/final_observed_accuracy.txt", sep="\t")
 	df=pd.DataFrame(df)
 
 	df["Acc"] = df["Acc"] * 100
 	min_1 = df["Acc"].min()
 	if min_1 >= 75:
 		acc_scale = [75,100]
@@ -29,57 +29,53 @@
 			geom_density(adjust=10, size=1.5, color="#96D1E8") +
 	    	scale_x_continuous(name="Observed read accuracy", 
 	    		limits=acc_scale, breaks=acc_breaks) +
 	    	scale_y_continuous(name="Probability Density Function (PDF)") +
 	    	theme_bw() + 
 	   		# geom_vline(aes(xintercept=90), color="grey", linetype="dotted") +
 	    	# geom_vline(aes(xintercept=99), color="grey", linetype="dotted") +
-	    	theme(axis_text=element_text(size=15, color="black"),
+	    	theme(axis_text=element_text(size=12, color="black"),
 	          axis_title=element_text(size=15, color="black"))
 	    )
 
+	Acc.save(filename = "Observed_read_accuracy.pdf", 
+		width=8, height=6, dpi=300, path="results/observed_quality/")
+
 	df["p_ins"] = 100 * df["Ins"]/(df["Ins"] + df["Del"] + df["Sub"] + df["Mat"])
 	df["p_del"] = 100 * df["Del"]/(df["Ins"] + df["Del"] + df["Sub"] + df["Mat"])
 	df["p_sub"] = 100 * df["Sub"]/(df["Ins"] + df["Del"] + df["Sub"] + df["Mat"])
 	df1 = df[["p_ins", "p_del", "p_sub"]].melt()
 
 	max_1 = df["p_ins"].max()
 	max_2 = df["p_del"].max()
 	max_3 = df["p_sub"].max()
 	max_4 = max(max_1, max_2, max_3)
 
-	if max_4 <= 5:
-		mis_scale = [0,5]
-		mis_breaks = [i for i in range(0, 6, 1)]
-	elif max_4 <= 10:
-		mis_scale = [0,10]
-		mis_breaks = [i for i in range(0, 11, 2)]
-	elif max_4 <= 25:
-		mis_scale = [0,25]
-		mis_breaks = [i for i in range(0, 26, 5)]
+	if max_4 <= 20:
+		mis_breaks = [i for i in range(0, 101, 1)]
 	elif max_4 <= 50:
-		mis_scale = [0,50]
-		mis_breaks = [i for i in range(0, 51, 10)]	
+		mis_breaks = [i for i in range(0, 101, 2)]
 	else:
-		mis_scale = [0,100]
-		mis_breaks = [i for i in range(0, 101, 10)]		
+		mis_breaks = [i for i in range(0, 101, 5)]		
 
 	Mis = (
 		ggplot(df1, aes(x="variable", y="value")) + 
-			geom_boxplot(width=0.25, outlier_size=1, 
-				fill="#96D1E8", outlier_color="black", alpha=0.3) +
+			geom_boxplot(width=0.25, outlier_shape='', fill="#96D1E8", alpha=0.3) +
 			theme_bw() +
-	    	scale_y_continuous(name="Mismatch proportion (%)", 
-	    		limits=mis_scale, breaks=mis_breaks) +
+	    	scale_y_continuous(name="Mismatch proportion (%)",breaks=mis_breaks) +
 	    	scale_x_discrete(name="Mismatch type", 
 	    		labels=["Deletion", "Insertion", "Substitution"]) +
-	    	theme(axis_text=element_text(size=15, color="black"),
+	    	theme(axis_text=element_text(size=12, color="black"),
 	        	  axis_title=element_text(size=15, color="black"))
 		)
 
+	Mis.save(filename = "Observed_mismatch_proportion.pdf", 
+		width=8, height=6, dpi=300, path="results/observed_quality/")
+
+def plot_observe_homo():
 	df2=pd.read_csv("./results/observed_quality/final_homo_summary.txt", sep="\t")
 	df2["value"] = df2["value"] * 100
 	df2["group"] = "group"
 
 	min_2 = df2["value"].min()
 	if min_2 >= 75:
 		homo_scale = [75,100]
@@ -98,22 +94,18 @@
 		ggplot(df2, aes(x="base",y="value", group="group"))  + 
 			geom_line(size=1, color="#96D1E8", alpha=.7, linetype="dashed") + 
 			geom_point(size=3, fill="#96D1E8", color="grey") + 
 		    
 		    scale_y_continuous(name="Accuracy of homopolymer identification (%)", 
 		    	limits=homo_scale, breaks =homo_breaks) +
 		    xlab("Base") + theme_bw() + 
-		    theme(axis_text=element_text(size=15, color="black"),
+		    theme(axis_text=element_text(size=12, color="black"),
 		          axis_title=element_text(size=15, color="black"))
 		)
 
-	Acc.save(filename = "Observed_read_accuracy.pdf", 
-		width=8, height=6, dpi=300, path="results/observed_quality/")
-	Mis.save(filename = "Observed_mismatch_proportion.pdf", 
-		width=8, height=6, dpi=300, path="results/observed_quality/")
 	Homo.save(filename = "Observed_homopolymer_identification.pdf", 
 		width=8, height=6, dpi=300, path="results/observed_quality/")
 
 def plot_estimate():
 	df=pd.read_csv("results/estimated_quality/final_estimated_accuracy.txt", sep="\t")
 	df=pd.DataFrame(df)
 	df["acc"] = df["acc"] * 100
@@ -137,15 +129,15 @@
 			geom_density(adjust=10, size=1.5, color="#96D1E8") +
             scale_x_continuous(name="Estimated read accuracy (%)",
             	limits=acc_scale, breaks=acc_breaks) + 
       #      	geom_vline(aes(xintercept=90), color="grey", linetype="dotted") +
 	    	# geom_vline(aes(xintercept=99), color="grey", linetype="dotted") +
             scale_y_continuous(name="Probability Density Function (PDF)") + 
             theme_bw() +
-            theme(axis_text=element_text(size=15, color="black"),
+            theme(axis_text=element_text(size=12, color="black"),
                   axis_title=element_text(size=15, color="black"))
 		)
 
 	Acc.save(filename = "estimated_read_accuracy.pdf", 
 		width=8, height=6, dpi=300, path="results/estimated_quality")
 
 def plot_GC_bias():
@@ -158,32 +150,41 @@
 	distribution_len = (
 		ggplot(df, aes(x="GC_content", y="number")) + 
 			geom_line(size=2, color="#96D1E8", alpha=.3) + 
 			geom_point(size=2, fill="#96D1E8", color="grey") +
             scale_x_continuous(name = "GC content (%)", 
             	limits=accurac_scale, breaks =accurac_break) +
             scale_y_continuous(name="Number of bins") + theme_bw() +
-            theme(axis_text=element_text(size=15, color="black"),
+            theme(axis_text=element_text(size=12, color="black"),
                   axis_title=element_text(size=15, color="black"))
 		)
 
 	df1=pd.read_csv("results/GC_bias/final_GC_bias_nor.txt", sep="\t")
 	df1=pd.DataFrame(df1)
 
+	dif = df1["GC_content"].max() - df1["GC_content"].min()
+	if dif <= 15:
+		gc_breaks = [i for i in range(0, 101, 1)]
+	elif dif <= 30:
+		gc_breaks = [i for i in range(0, 101, 2)]
+	elif dif <= 50:
+		gc_breaks = [i for i in range(0, 101, 5)]
+	else:
+		gc_breaks = [i for i in range(0, 101, 10)]
+
 	GC_bias = (
 		ggplot(df1, aes(x="GC_content", y="nor_dp")) + 
 			geom_hline(aes(yintercept=1), color="grey", linetype="dotted") + 
 			geom_line(size=2, color="#96D1E8", alpha=.3) + 
 			geom_point(size=2, fill="#96D1E8", color="grey") +
 			scale_y_continuous(name="Normalized depth", 
 				limits=[0, 2], breaks=np.arange(0, 2.1, 0.2)) +
 			theme_bw() + 
-			scale_x_continuous(name="GC content (%)", 
-				breaks=[i for i in range(0, 101, 1)]) +
-            theme(axis_text=element_text(size=15, color="black"),
+			scale_x_continuous(name="GC content (%)", breaks=gc_breaks) +
+            theme(axis_text=element_text(size=12, color="black"),
                   axis_title=element_text(size=15, color="black"))
 		)
 
 	distribution_len.save(filename = "bin_distribution.pdf", 
 		width=8, height=6, dpi=300, path="results/GC_bias/")
 	GC_bias.save(filename = "GC_bias.pdf", 
 		width=8, height=6, dpi=300, path="results/GC_bias/")
@@ -204,30 +205,28 @@
 	elif diff <= 40:
 		Breaks = [i for i in range(0, 101, 5)]
 	else:
 		Breaks = [i for i in range(0, 101, 10)]
 
 	Bin_box = (
 		ggplot(df, aes(x="group", y="Value")) + 
-			geom_boxplot(width=0.15, fill="#96D1E8", 
-				alpha=0.2, outlier_size=0.5, outlier_color="black") +
-			theme_bw() +
+			geom_boxplot(width=0.15, fill="#96D1E8", alpha=0.2, outlier_shape="") +
 			scale_y_continuous(name="Modification proportion (%)",
-				breaks=Breaks) + xlab("") + 
-			theme(axis_text=element_text(size=15, color="black"),
+				breaks=Breaks) + xlab("") + theme_bw() +
+			theme(axis_text=element_text(size=12, color="black"),
                   axis_title=element_text(size=15, color="black"))
 		)
 
 	Bin_violin = (
 		ggplot(df, aes(x="group", y="Value")) + 
 			geom_violin(width=0.15, fill="#96D1E8", alpha=0.3) + 
 			theme_bw() +
 			scale_y_continuous(name="Modification proportion (%)",
 				breaks=Breaks) + xlab("") + 
-			theme(axis_text=element_text(size=15, color="black"),
+			theme(axis_text=element_text(size=12, color="black"),
                   axis_title=element_text(size=15, color="black"))
 		)
 
 	Bin_box.save(filename = "motif_bin_box.pdf", 
 		width=8, height=6, dpi=300, path="results/regional_modification/")
 
 	Bin_violin.save(filename = "motif_bin_violin.pdf",
```

### Comparing `Giraffe_View-0.0.9.4/Giraffe_View/regional_modification.py` & `Giraffe_View-0.0.9.5/Giraffe_View/regional_modification.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.4/Giraffe_View.egg-info/PKG-INFO` & `Giraffe_View-0.0.9.5/Giraffe_View.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe-View
-Version: 0.0.9.4
+Version: 0.0.9.5
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,16 +14,16 @@
 
 # Giraffe_View 
 
 **Giraffe_View** is designed to help assess and visualize the accuracy of a sequencing dataset, specifically for Oxford Nanopore Technologies (ONT) long-read sequencing including DNA and RNA data. There are four main functions to validate the read quality.
 
 - `observe`  calculates the observed read accuracy, mismatches porportion, and homopolymer identification.
 - `estimate`  calculates the estimated read accuracy, which is equal to Quality Score.
-- `gc_bias`  compares the relationship between GC content and read coverage.
-- `modi_bin` perform statistics on the distribution of modification based on the bed file.
+- `gcbias`  compares the relationship between GC content and read coverage.
+- `modibin` perform statistics on the distribution of modification based on the bed file.
 
 
 
 ## Install
 
 To use this software, you need to install additional dependencies including samtools, minimap2, seqkit, and bedtools for read processing. The following commands can help you to install the package  and dependencies.
 
@@ -35,25 +35,24 @@
 
 
 ## General Usage
 
 Giraffe View is run simply with fllowing commands:
 
 ```
-giraffe -h
-usage: giraffe [-h] {observe,estimate,gc_bias,modi_bin} ...
+usage: giraffe [-h] {observe,estimate,gcbias,modibin} ...
 
 A tool to help you assess quality of ONT data.
 
 positional arguments:
-  {observe,estimate,gc_bias,modi_bin}
+  {observe,estimate,gcbias,modibin}
     observe             Observed quality in accuracy, mismatch, and homopolymer identification
     estimate            Estimated read accuracy
-    gc_bias             Relationship between GC content and depth
-    modi_bin            Average modification proportion of bins
+    gcbias              Relationship between GC content and depth
+    modibin             Average modification proportion of bins
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
 
 
@@ -90,19 +89,19 @@
   --input <fastq>  input reads
   --cpu <number>   number of cpu (default:10)
   --plot           Results visualization
 ```
 
 
 
-#### gc_bias
+#### gcbias
 
 ```
-giraffe gc_bias -h
-usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize] [--plot]
+giraffe gcbias -h
+usage: giraffe gcbias [-h] --ref <reference> --input <sam/bam> [--binsize] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --ref <reference>  input reference file
   --input <sam/bam>  input bam/sam file
   --binsize          input bin size (default:1000)
   --plot             Results visualization
@@ -110,19 +109,19 @@
 
 - `reference` - the reference file in fasta format.
 - `sam` / `bam` - the result of mapping in sam/bam file. If you have used the observe function to process your data, the resulting `tmp.sort.bam` file can be used as the input.
 - `binsize` - the length of bin. A bin is the smallest unit to count the read coverage and GC content.
 
 
 
-#### modi_bin
+#### modibin
 
 ```
-giraffe modi_bin -h
-usage: giraffe modi_bin [-h] --input <bed> --ref <reference> [--cpu <number>] [--plot]
+giraffe modibin -h
+usage: giraffe modibin [-h] --input <bed> --ref <reference> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <bed>      input modificated bed file, please use the .bed as the file suffix
   --ref <reference>  input position file with CSV format, please use the .csv as the file suffix
   --cpu <number>     number of cpu (default:10)
   --plot             Results visualization
@@ -148,22 +147,22 @@
 
 ## Workflow
 
 ```mermaid
 graph TD
 	A(raw signal) -.-> |Basecall| B(FASTA)
 	A(raw signal) -.-> |Basecall| C(modificated BED)
-	C(modificated BED) --> |modi_bin| D(modification distribution)
+	C(modificated BED) --> |modibin| D(modification distribution)
 	B(FASTA) --> |estimate|e(estimated accuracy)
 	B(FASTA) --> |observe| f(clean reads)
 	f(clean reads) --> |observe| g(aligned BAM)
 	
 	g(aligned BAM) --> |observe|h(homopolymer identification)
  	g(aligned BAM) --> |observe|i(observed accuracy)
-	g(aligned BAM) --> |gc_bias|j(GC bias) 
+	g(aligned BAM) --> |gcbias|j(GC bias) 
 ```
 
 
 
 ## Developing
 
-- run the homopolymer identification with multi-processed
+- run the homopolymer identification with multi processes.
```

### Comparing `Giraffe_View-0.0.9.4/LICENSE` & `Giraffe_View-0.0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.4/PKG-INFO` & `Giraffe_View-0.0.9.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe_View
-Version: 0.0.9.4
+Version: 0.0.9.5
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,16 +14,16 @@
 
 # Giraffe_View 
 
 **Giraffe_View** is designed to help assess and visualize the accuracy of a sequencing dataset, specifically for Oxford Nanopore Technologies (ONT) long-read sequencing including DNA and RNA data. There are four main functions to validate the read quality.
 
 - `observe`  calculates the observed read accuracy, mismatches porportion, and homopolymer identification.
 - `estimate`  calculates the estimated read accuracy, which is equal to Quality Score.
-- `gc_bias`  compares the relationship between GC content and read coverage.
-- `modi_bin` perform statistics on the distribution of modification based on the bed file.
+- `gcbias`  compares the relationship between GC content and read coverage.
+- `modibin` perform statistics on the distribution of modification based on the bed file.
 
 
 
 ## Install
 
 To use this software, you need to install additional dependencies including samtools, minimap2, seqkit, and bedtools for read processing. The following commands can help you to install the package  and dependencies.
 
@@ -35,25 +35,24 @@
 
 
 ## General Usage
 
 Giraffe View is run simply with fllowing commands:
 
 ```
-giraffe -h
-usage: giraffe [-h] {observe,estimate,gc_bias,modi_bin} ...
+usage: giraffe [-h] {observe,estimate,gcbias,modibin} ...
 
 A tool to help you assess quality of ONT data.
 
 positional arguments:
-  {observe,estimate,gc_bias,modi_bin}
+  {observe,estimate,gcbias,modibin}
     observe             Observed quality in accuracy, mismatch, and homopolymer identification
     estimate            Estimated read accuracy
-    gc_bias             Relationship between GC content and depth
-    modi_bin            Average modification proportion of bins
+    gcbias              Relationship between GC content and depth
+    modibin             Average modification proportion of bins
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
 
 
@@ -90,19 +89,19 @@
   --input <fastq>  input reads
   --cpu <number>   number of cpu (default:10)
   --plot           Results visualization
 ```
 
 
 
-#### gc_bias
+#### gcbias
 
 ```
-giraffe gc_bias -h
-usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize] [--plot]
+giraffe gcbias -h
+usage: giraffe gcbias [-h] --ref <reference> --input <sam/bam> [--binsize] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --ref <reference>  input reference file
   --input <sam/bam>  input bam/sam file
   --binsize          input bin size (default:1000)
   --plot             Results visualization
@@ -110,19 +109,19 @@
 
 - `reference` - the reference file in fasta format.
 - `sam` / `bam` - the result of mapping in sam/bam file. If you have used the observe function to process your data, the resulting `tmp.sort.bam` file can be used as the input.
 - `binsize` - the length of bin. A bin is the smallest unit to count the read coverage and GC content.
 
 
 
-#### modi_bin
+#### modibin
 
 ```
-giraffe modi_bin -h
-usage: giraffe modi_bin [-h] --input <bed> --ref <reference> [--cpu <number>] [--plot]
+giraffe modibin -h
+usage: giraffe modibin [-h] --input <bed> --ref <reference> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <bed>      input modificated bed file, please use the .bed as the file suffix
   --ref <reference>  input position file with CSV format, please use the .csv as the file suffix
   --cpu <number>     number of cpu (default:10)
   --plot             Results visualization
@@ -148,22 +147,22 @@
 
 ## Workflow
 
 ```mermaid
 graph TD
 	A(raw signal) -.-> |Basecall| B(FASTA)
 	A(raw signal) -.-> |Basecall| C(modificated BED)
-	C(modificated BED) --> |modi_bin| D(modification distribution)
+	C(modificated BED) --> |modibin| D(modification distribution)
 	B(FASTA) --> |estimate|e(estimated accuracy)
 	B(FASTA) --> |observe| f(clean reads)
 	f(clean reads) --> |observe| g(aligned BAM)
 	
 	g(aligned BAM) --> |observe|h(homopolymer identification)
  	g(aligned BAM) --> |observe|i(observed accuracy)
-	g(aligned BAM) --> |gc_bias|j(GC bias) 
+	g(aligned BAM) --> |gcbias|j(GC bias) 
 ```
 
 
 
 ## Developing
 
-- run the homopolymer identification with multi-processed
+- run the homopolymer identification with multi processes.
```

### Comparing `Giraffe_View-0.0.9.4/README.md` & `Giraffe_View-0.0.9.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Giraffe_View 
 
 **Giraffe_View** is designed to help assess and visualize the accuracy of a sequencing dataset, specifically for Oxford Nanopore Technologies (ONT) long-read sequencing including DNA and RNA data. There are four main functions to validate the read quality.
 
 - `observe`  calculates the observed read accuracy, mismatches porportion, and homopolymer identification.
 - `estimate`  calculates the estimated read accuracy, which is equal to Quality Score.
-- `gc_bias`  compares the relationship between GC content and read coverage.
-- `modi_bin` perform statistics on the distribution of modification based on the bed file.
+- `gcbias`  compares the relationship between GC content and read coverage.
+- `modibin` perform statistics on the distribution of modification based on the bed file.
 
 
 
 ## Install
 
 To use this software, you need to install additional dependencies including samtools, minimap2, seqkit, and bedtools for read processing. The following commands can help you to install the package  and dependencies.
 
@@ -21,25 +21,24 @@
 
 
 ## General Usage
 
 Giraffe View is run simply with fllowing commands:
 
 ```
-giraffe -h
-usage: giraffe [-h] {observe,estimate,gc_bias,modi_bin} ...
+usage: giraffe [-h] {observe,estimate,gcbias,modibin} ...
 
 A tool to help you assess quality of ONT data.
 
 positional arguments:
-  {observe,estimate,gc_bias,modi_bin}
+  {observe,estimate,gcbias,modibin}
     observe             Observed quality in accuracy, mismatch, and homopolymer identification
     estimate            Estimated read accuracy
-    gc_bias             Relationship between GC content and depth
-    modi_bin            Average modification proportion of bins
+    gcbias              Relationship between GC content and depth
+    modibin             Average modification proportion of bins
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
 
 
@@ -76,19 +75,19 @@
   --input <fastq>  input reads
   --cpu <number>   number of cpu (default:10)
   --plot           Results visualization
 ```
 
 
 
-#### gc_bias
+#### gcbias
 
 ```
-giraffe gc_bias -h
-usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize] [--plot]
+giraffe gcbias -h
+usage: giraffe gcbias [-h] --ref <reference> --input <sam/bam> [--binsize] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --ref <reference>  input reference file
   --input <sam/bam>  input bam/sam file
   --binsize          input bin size (default:1000)
   --plot             Results visualization
@@ -96,19 +95,19 @@
 
 - `reference` - the reference file in fasta format.
 - `sam` / `bam` - the result of mapping in sam/bam file. If you have used the observe function to process your data, the resulting `tmp.sort.bam` file can be used as the input.
 - `binsize` - the length of bin. A bin is the smallest unit to count the read coverage and GC content.
 
 
 
-#### modi_bin
+#### modibin
 
 ```
-giraffe modi_bin -h
-usage: giraffe modi_bin [-h] --input <bed> --ref <reference> [--cpu <number>] [--plot]
+giraffe modibin -h
+usage: giraffe modibin [-h] --input <bed> --ref <reference> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <bed>      input modificated bed file, please use the .bed as the file suffix
   --ref <reference>  input position file with CSV format, please use the .csv as the file suffix
   --cpu <number>     number of cpu (default:10)
   --plot             Results visualization
@@ -134,22 +133,22 @@
 
 ## Workflow
 
 ```mermaid
 graph TD
 	A(raw signal) -.-> |Basecall| B(FASTA)
 	A(raw signal) -.-> |Basecall| C(modificated BED)
-	C(modificated BED) --> |modi_bin| D(modification distribution)
+	C(modificated BED) --> |modibin| D(modification distribution)
 	B(FASTA) --> |estimate|e(estimated accuracy)
 	B(FASTA) --> |observe| f(clean reads)
 	f(clean reads) --> |observe| g(aligned BAM)
 	
 	g(aligned BAM) --> |observe|h(homopolymer identification)
  	g(aligned BAM) --> |observe|i(observed accuracy)
-	g(aligned BAM) --> |gc_bias|j(GC bias) 
+	g(aligned BAM) --> |gcbias|j(GC bias) 
 ```
 
 
 
 ## Developing
 
-- run the homopolymer identification with multi-processed
+- run the homopolymer identification with multi processes.
```

### Comparing `Giraffe_View-0.0.9.4/setup.py` & `Giraffe_View-0.0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="Giraffe_View",
-  version="0.0.9.4",
+  version="0.0.9.5",
   author="Xudong Liu",
   author_email="xudongliu98@gmail.com",
   description="A small tool help assess and visualize the accuracy of a sequencing dataset, \
   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/lxd98/Giraffe_View",
```

