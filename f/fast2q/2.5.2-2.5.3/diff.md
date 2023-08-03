# Comparing `tmp/fast2q-2.5.2.tar.gz` & `tmp/fast2q-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fast2q-2.5.2.tar", last modified: Thu Apr 27 13:11:37 2023, max compression
+gzip compressed data, was "dist\fast2q-2.5.3.tar", last modified: Thu Aug  3 08:38:43 2023, max compression
```

## Comparing `fast2q-2.5.2.tar` & `fast2q-2.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 13:11:37.000000 fast2q-2.5.2/
--rw-rw-rw-   0        0        0    13645 2023-04-27 13:11:37.000000 fast2q-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      492 2021-11-17 10:01:50.000000 fast2q-2.5.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 13:11:37.000000 fast2q-2.5.2/fast2q/
--rw-rw-rw-   0        0        0        0 2021-05-14 10:49:48.000000 fast2q-2.5.2/fast2q/__init__.py
--rw-rw-rw-   0        0        0       76 2021-09-02 14:00:47.000000 fast2q-2.5.2/fast2q/__main__.py
--rw-rw-rw-   0        0        0    49523 2023-04-27 13:00:29.000000 fast2q-2.5.2/fast2q/fast2q.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:11:37.000000 fast2q-2.5.2/fast2q.egg-info/
--rw-rw-rw-   0        0        0    13645 2023-04-27 13:11:36.000000 fast2q-2.5.2/fast2q.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-27 13:11:36.000000 fast2q-2.5.2/fast2q.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 13:11:36.000000 fast2q-2.5.2/fast2q.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-04-27 13:11:36.000000 fast2q-2.5.2/fast2q.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 13:11:36.000000 fast2q-2.5.2/fast2q.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 13:11:37.000000 fast2q-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1525 2023-04-27 13:09:14.000000 fast2q-2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:38:43.000000 fast2q-2.5.3/
+-rw-rw-rw-   0        0        0    11539 2023-08-03 08:38:43.000000 fast2q-2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2021-11-17 10:01:50.000000 fast2q-2.5.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 08:38:43.000000 fast2q-2.5.3/fast2q/
+-rw-rw-rw-   0        0        0        0 2021-05-14 10:49:48.000000 fast2q-2.5.3/fast2q/__init__.py
+-rw-rw-rw-   0        0        0       76 2021-09-02 14:00:47.000000 fast2q-2.5.3/fast2q/__main__.py
+-rw-rw-rw-   0        0        0    49713 2023-08-03 08:20:59.000000 fast2q-2.5.3/fast2q/fast2q.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:38:43.000000 fast2q-2.5.3/fast2q.egg-info/
+-rw-rw-rw-   0        0        0    11539 2023-08-03 08:38:42.000000 fast2q-2.5.3/fast2q.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-08-03 08:38:42.000000 fast2q-2.5.3/fast2q.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 08:38:42.000000 fast2q-2.5.3/fast2q.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-08-03 08:38:42.000000 fast2q-2.5.3/fast2q.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 08:38:42.000000 fast2q-2.5.3/fast2q.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 08:38:43.000000 fast2q-2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1525 2023-08-03 08:38:25.000000 fast2q-2.5.3/setup.py
```

### Comparing `fast2q-2.5.2/PKG-INFO` & `fast2q-2.5.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast2q
-Version: 2.5.2
+Version: 2.5.3
 Summary: A Python3 program that counts sequence occurences in fastq files.
 Home-page: https://github.com/afombravo/2FAST2Q
 Author: Afonso M Bravo
 Author-email: <afonsombravo@hotmail.com>
 License: UNKNOWN
 Description: # Welcome to 2FAST2Q
         A Python3 based program that counts sequence occurrences in FASTQ files
@@ -146,23 +146,22 @@
         =================================
         
         2FAST2Q is coded to maximize any computer's processing power (it runs multiprocessed, so it can process various samples simultaneously). It is therefore advisable to not heavily use the computer while 2FAST2Q is running to avoid constraining the processor.
         
         When running 2FAST2Q in the compiled form, the initialization sequence might take up to a minute. 2FAST2Q will be operational when "Version X.X.X" appears on the window.
         Depending on the used computer, 2FAST2Q might take a few minutes to run. If no errors are shown, 2FAST2Q is still running. GIVE IT TIME!
         
-        \\\\\\\
         
         macOS use WARNING!
         
         When using the graphical user interface option, it's possible that the interface is buggy on some MacOS versions. In this case, it might be better to run the command line version via pip install fast2q
-         =================================
         
         A completion message should be given at the end. In any case, the program will be finish when the compiled.csv file is visible in the directory.
         
+        =================================
         
         # Output
         
         Upon completion, several files should be seen in the indicated output folder (when running in default mode only b, c, and d will be kept):
         
         a. 	“*_reads.csv” files corresponding to the read counts per feature per inputted sequencing file; 
         
@@ -205,30 +204,14 @@
         2. Download the "example.fastq.gz"
         3. Run 2FAST2Q
         
         In this example, sgRNA0850 and sgRNA867 share the same sequence; this will appear as a warning message.
         
         The expected example output file is given: "compiled.csv"
         
-        
-        
-        Common Errors:
-        
-        
-        | Error Message | Probable Cause/Fix |
-        | ------------- | ------------------ |
-        |Please enter a valid directory for the following request: (see printed requests). Please close the program and start again | You have entered an invalid file or folder location. Check that the correct folder/file was selected. When choosing a file click on the file. When selecting a folder, double click (go into the folder, no files will be visible. Its normal).|
-        |Please confirm that all the input boxes are filled. Some parameters are missing. Press any key to exit | Click OK on the pop up parameter box. The wrong parameter format was entered. Please restart the program and re-introduce ALL the required paths (you must use the browse buttons for this), and parameters (or leave at default). Please close the program and start again |
-        | Only numeric values are accepted in the following fields: ... | Introduce parameters that respect the default format (text and integers, when appropriate). |
-        | Warning!! X and Y share the same sequence. Only X will be considered valid. |X and Y correspond to feature names. The indicated entries have the same sequence, and only the first will be considered valid. |
-        | Check the path to the feature file. No file found in the following path: X | Confirm the indicated path (X) to the feature .csv file is correct |
-        | Check the path to the X files folder. No files of this type found. | Confirm the indicated path to the folder with the sequencing (X) files is correct. |
-        | Program doesn’t initialize | Confirm the downloaded program is the appropriate one for the current operating system. Contact the 2FAST2Q developer if the issue persists. |
-        | Program crashes, or behaves unexpectedly. | Restart the program and carefully indicate the appropriate required input paths. Check if the program behaves as expected with the provided sample data. Contact the 2FAST2Q developer if the issue persists. |
-        
 Keywords: CRISPRi,CRISPRi-Seq,essentiality,gene fitness
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fast2q-2.5.2/fast2q/fast2q.py` & `fast2q-2.5.3/fast2q/fast2q.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,17 @@
                     start,end=unfixed_starting_place_parser(str(reading[1],"utf-8"),\
                                                             reading[3],\
                                                             param)
                         
                     if (start is not None) & (end is not None):
                         if end < start: #if the end is not found or found before the start
                             start=None
+                            quality_failed += 1
+                    else:
+                        quality_failed += 1
 
                 if (fixed_start) or (start is not None):
                     seq = str(reading[1][start:end].upper(),"utf-8")
                     quality = str(reading[3][start:end],"utf-8") #convert from bin to str
 
                     if len(param['quality_set'].intersection(quality)) == 0:
                         
@@ -269,16 +272,16 @@
                 reads += 1
                 
                 # keeps RAM under control by avoiding overflow
                 if reads % 1000000 == 0:
                     ram_clearance=ram_lock()
                 
                 if preprocess:
-                    if reads == 200000:
-                        return reads,perfect_counter,imperfect_counter,features,failed_reads,passed_reads
+                    if reads == 100000:
+                        return reads,perfect_counter,imperfect_counter,features,failed_reads,passed_reads,0,0
         
         if (not preprocess) & (param['Progress bar']):
             pbar.close()
 
         return reads,perfect_counter,imperfect_counter,features,failed_reads,passed_reads,non_aligned_counter,quality_failed
     
     fixed_start,end,start = True,0,0
@@ -333,15 +336,15 @@
     """ Matches 2 sequences (after converting to int8 format)
     based on the allowed mismatches. Used for sequencing searching
     a start/end place in a read"""
     
     s=seq.size
     r=read.size
     fall_over_index = r-s-1
-    for i,bp in enumerate(read): #range doesnt exist in njit
+    for i,bp in enumerate(read): 
         comparison = read[i:s+i]
         finder = binary_subtract(seq,comparison,mismatch)
         if i > fall_over_index:
             return
         if finder != 0:
             return i
 
@@ -357,44 +360,44 @@
         if binary_subtract(binary_features[guide],read,mismatch):
             found+=1
             found_guide = guide
             if found>=2:
                 return
     if found==1:
         return found_guide
-    return #not needed, but here for peace of mind
 
 def mismatch_search_handler(seq,mismatch,failed_reads,binary_features,imperfect_counter,features,passed_reads,ram_clearance,non_aligned_counter):
     
     """Converts a read into numpy int 8 form. Runs the imperfect alignment 
     function for all number of inputed mismatches."""
     
     read=seq2bin(seq)                         
     for miss in mismatch:
 
         # we already know this read is going to pass
         if seq in passed_reads:
             features[passed_reads[seq]].counts += 1
             imperfect_counter += 1
-            break
+            return features,imperfect_counter,failed_reads,passed_reads,non_aligned_counter
         
         elif seq not in failed_reads:
             features,imperfect_counter,feature=\
                 imperfect_alignment(read,binary_features,\
                                     miss, imperfect_counter,\
                                     features)
-            if ram_clearance:
-                if feature is None:
+            if feature is None:
+                if ram_clearance:
                     failed_reads.add(seq)
-                    non_aligned_counter += 1
-                    break
-                else:
-                    passed_reads[seq] = feature
-        else:
-            non_aligned_counter += 1
+            else:
+                passed_reads[seq] = feature
+                imperfect_counter += 1
+                return features,imperfect_counter,failed_reads,passed_reads,non_aligned_counter
+    
+    #if function reaches here its because nothing was aligned anywhere
+    non_aligned_counter += 1
 
     return features,imperfect_counter,failed_reads,passed_reads,non_aligned_counter
 
 def imperfect_alignment(read,binary_features, mismatch, counter, features):
     
     """ for the inputed read sequence, this compares if there is a feature 
     with a sequence that is similar to it, to the indicated mismatch degree"""
@@ -448,22 +451,22 @@
         master_list.sort(key = lambda master_list: master_list[0]) #alphabetical sorting
     
     master_list.insert(0,["#Feature"] + ["Reads"])
     master_list.insert(0,[stats_condition])
     
     csvfile = os.path.join(param["directory"], name+"_reads.csv")
     csv_writer(csvfile, master_list)
-    
+
     return failed_reads,passed_reads
 
 def csv_writer(path, outfile):
     
     """ writes the indicated outfile into an .csv file in the directory"""
         
-    with open(path, "w", newline='') as output: #writes the output
+    with open(path, "w", newline='') as output: 
         writer = csv.writer(output)
         writer.writerows(outfile)
 
 def inputs_handler():
     
     """ assertains the correct parsing of the input parameters"""
     
@@ -646,15 +649,15 @@
 
     print(f"\nVersion: {version}")
 
     param = inputs_handler() if cmd is None else cmd
 
     param["version"] = version
     
-    quality_list = '!"#$%&' + "'()*+,-/0123456789:;<=>?@ABCDEFGHI" #Phred score
+    quality_list = '!"#$%&' + "'()*+,-/0123456789:;<=>?@ABCDEFGHI" #Phred score in order of probabilities
 
     param["quality_set"] = set(quality_list[:int(param['phred'])-1])
     param["quality_set_up"] = set(quality_list[:int(param['qual_up'])-1])
     param["quality_set_down"] = set(quality_list[:int(param['qual_down'])-1])
     
     current_time = datetime.datetime.now().strftime('%Y_%m_%d_%H_%M_%S')
     param["directory"] = os.path.join(param['out'], f"2FAST2Q_output_{current_time}")
@@ -685,15 +688,15 @@
     return param
 
 def input_parser():
     
     """ Handles the cmd line interface, and all the parameter inputs"""
     
     global version
-    version = "2.5.2"
+    version = "2.5.3"
     
     def current_dir_path_handling(param):
         if param[0] is None:
             parameters[param[1]]=os.getcwd()
             if param[1] == 'feature':
                 file = path_finder(os.getcwd(), ["*.csv"])
                 if parameters['Running Mode']!="EC":
@@ -1096,46 +1099,48 @@
     """ parsed the results from all the processes, merging the individual failed and
     passed reads into one master file, that will be subsquently used for the new
     samples's processing """ 
     
     for failed,passed in zip(failed_reads_compiled,passed_reads_compiled):
         failed_reads = set.union(failed_reads,failed)
         passed_reads = {**passed_reads,**passed}
-        
+
     return failed_reads,passed_reads
 
 def hash_preprocesser(files,features,param,pool,cpu):
     
     """ For the smallest files, we processe them for the first x amount of reads to
     initialize the failed reads and passed reads hash tables. This will confer some 
     speed advantages, as subsquent files normally share the same reads that dont
     align to anything, or reads with mismatches that indeed align"""
     
     print("\nPlease standby for the initialization procedure.")
     result=[]
+
     for name in files[:cpu]:
         result.append(pool.apply_async(reads_counter, args=(0,0,name,features,param,cpu,set(),{},True)))
     
     compiled = [x.get() for x in result]
-    throw1,throw2,throw3,throw4,failed_reads_compiled,passed_reads_compiled = zip(*compiled)
-    
+
+    _,_,_,_,failed_reads_compiled,passed_reads_compiled,_,_ = zip(*compiled)
+
     return hash_reads_parsing(result,failed_reads_compiled,passed_reads_compiled,set(),{})
 
 def aligner_mp_dispenser(files,features,param):
     
     """ starts and handles the parallel processing of all the samples by calling 
     multiple instances of the "aligner" function (one per sample) """
     
     if not os.path.exists(param["directory"]):
         os.makedirs(param["directory"])
     
     start,failed_reads,passed_reads = 0,set(),{}
     pool,cpu = cpu_counter(param["cpu"])
     
-    if (len(files)>cpu) & (param["miss"] != 0):
+    if param["miss"] != 0:
         failed_reads,passed_reads=hash_preprocesser(files,features,param,pool,cpu)
     
     print(f"\nProcessing {len(files)} files. Please hold.")
     for start in range(0,len(files),cpu):
         failed_reads,passed_reads = \
         multiprocess_merger(start,failed_reads,passed_reads,files,\
                             features,param,pool,cpu)
```

### Comparing `fast2q-2.5.2/fast2q.egg-info/PKG-INFO` & `fast2q-2.5.3/fast2q.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast2q
-Version: 2.5.2
+Version: 2.5.3
 Summary: A Python3 program that counts sequence occurences in fastq files.
 Home-page: https://github.com/afombravo/2FAST2Q
 Author: Afonso M Bravo
 Author-email: <afonsombravo@hotmail.com>
 License: UNKNOWN
 Description: # Welcome to 2FAST2Q
         A Python3 based program that counts sequence occurrences in FASTQ files
@@ -146,23 +146,22 @@
         =================================
         
         2FAST2Q is coded to maximize any computer's processing power (it runs multiprocessed, so it can process various samples simultaneously). It is therefore advisable to not heavily use the computer while 2FAST2Q is running to avoid constraining the processor.
         
         When running 2FAST2Q in the compiled form, the initialization sequence might take up to a minute. 2FAST2Q will be operational when "Version X.X.X" appears on the window.
         Depending on the used computer, 2FAST2Q might take a few minutes to run. If no errors are shown, 2FAST2Q is still running. GIVE IT TIME!
         
-        \\\\\\\
         
         macOS use WARNING!
         
         When using the graphical user interface option, it's possible that the interface is buggy on some MacOS versions. In this case, it might be better to run the command line version via pip install fast2q
-         =================================
         
         A completion message should be given at the end. In any case, the program will be finish when the compiled.csv file is visible in the directory.
         
+        =================================
         
         # Output
         
         Upon completion, several files should be seen in the indicated output folder (when running in default mode only b, c, and d will be kept):
         
         a. 	“*_reads.csv” files corresponding to the read counts per feature per inputted sequencing file; 
         
@@ -205,30 +204,14 @@
         2. Download the "example.fastq.gz"
         3. Run 2FAST2Q
         
         In this example, sgRNA0850 and sgRNA867 share the same sequence; this will appear as a warning message.
         
         The expected example output file is given: "compiled.csv"
         
-        
-        
-        Common Errors:
-        
-        
-        | Error Message | Probable Cause/Fix |
-        | ------------- | ------------------ |
-        |Please enter a valid directory for the following request: (see printed requests). Please close the program and start again | You have entered an invalid file or folder location. Check that the correct folder/file was selected. When choosing a file click on the file. When selecting a folder, double click (go into the folder, no files will be visible. Its normal).|
-        |Please confirm that all the input boxes are filled. Some parameters are missing. Press any key to exit | Click OK on the pop up parameter box. The wrong parameter format was entered. Please restart the program and re-introduce ALL the required paths (you must use the browse buttons for this), and parameters (or leave at default). Please close the program and start again |
-        | Only numeric values are accepted in the following fields: ... | Introduce parameters that respect the default format (text and integers, when appropriate). |
-        | Warning!! X and Y share the same sequence. Only X will be considered valid. |X and Y correspond to feature names. The indicated entries have the same sequence, and only the first will be considered valid. |
-        | Check the path to the feature file. No file found in the following path: X | Confirm the indicated path (X) to the feature .csv file is correct |
-        | Check the path to the X files folder. No files of this type found. | Confirm the indicated path to the folder with the sequencing (X) files is correct. |
-        | Program doesn’t initialize | Confirm the downloaded program is the appropriate one for the current operating system. Contact the 2FAST2Q developer if the issue persists. |
-        | Program crashes, or behaves unexpectedly. | Restart the program and carefully indicate the appropriate required input paths. Check if the program behaves as expected with the provided sample data. Contact the 2FAST2Q developer if the issue persists. |
-        
 Keywords: CRISPRi,CRISPRi-Seq,essentiality,gene fitness
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fast2q-2.5.2/setup.py` & `fast2q-2.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-VERSION = '2.5.2' 
+VERSION = '2.5.3' 
 DESCRIPTION = """A Python3 program that counts sequence occurences in fastq files."""
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="fast2q", 
         version=VERSION,
```

