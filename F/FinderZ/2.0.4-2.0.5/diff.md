# Comparing `tmp/finderz-2.0.4.tar.gz` & `tmp/finderz-2.0.5.tar.gz`

## Comparing `finderz-2.0.4.tar` & `finderz-2.0.5.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.4/.DS_Store
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 finderz-2.0.4/.readthedocs.yaml
--rw-r--r--   0        0        0    10265 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/code structure.rst
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/conf.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/credits.rst
--rw-r--r--   0        0        0    28707 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/function use.rst
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/index.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/installation.rst
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/updatev2.rst
--rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/img/logo-color.jpg
--rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.4/logo/logo-color.jpg
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.4/old/src/.DS_Store
--rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 finderz-2.0.4/old/src/FinderZ/FinderZLib.py
--rw-r--r--   0        0        0    48940 2020-02-02 00:00:00.000000 finderz-2.0.4/old/src/FinderZ/FinderZV2.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 finderz-2.0.4/old/src/FinderZ/__init__.py
--rw-r--r--   0        0        0    49539 2020-02-02 00:00:00.000000 finderz-2.0.4/src/FinderZ/FinderZV2.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 finderz-2.0.4/src/FinderZ/__init__.py
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/updates/.DS_Store
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/updates/V2 Changelog.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/updates/bash.sh
--rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/updates/parentFunctions.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/updates/update.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 finderz-2.0.4/LICENSE
--rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 finderz-2.0.4/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 finderz-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 finderz-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.5/.DS_Store
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 finderz-2.0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0    10265 2020-02-02 00:00:00.000000 finderz-2.0.5/docs/code structure.rst
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 finderz-2.0.5/docs/conf.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 finderz-2.0.5/docs/credits.rst
+-rw-r--r--   0        0        0    28940 2020-02-02 00:00:00.000000 finderz-2.0.5/docs/function use.rst
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 finderz-2.0.5/docs/index.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 finderz-2.0.5/docs/installation.rst
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 finderz-2.0.5/docs/updatev2.rst
+-rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.5/docs/img/logo-color.jpg
+-rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.5/logo/logo-color.jpg
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.5/old/src/.DS_Store
+-rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 finderz-2.0.5/old/src/FinderZ/FinderZLib.py
+-rw-r--r--   0        0        0    48940 2020-02-02 00:00:00.000000 finderz-2.0.5/old/src/FinderZ/FinderZV2.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 finderz-2.0.5/old/src/FinderZ/__init__.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.5/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.5/src/FinderZ/.DS_Store
+-rw-r--r--   0        0        0    51421 2020-02-02 00:00:00.000000 finderz-2.0.5/src/FinderZ/FinderZV2.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 finderz-2.0.5/src/FinderZ/__init__.py
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 finderz-2.0.5/tests/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.5/tests/updates/.DS_Store
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 finderz-2.0.5/tests/updates/V2 Changelog.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 finderz-2.0.5/tests/updates/bash.sh
+-rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 finderz-2.0.5/tests/updates/parentFunctions.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 finderz-2.0.5/tests/updates/update.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 finderz-2.0.5/LICENSE
+-rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 finderz-2.0.5/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 finderz-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6833 2020-02-02 00:00:00.000000 finderz-2.0.5/PKG-INFO
```

### Comparing `finderz-2.0.4/docs/code structure.rst` & `finderz-2.0.5/docs/code structure.rst`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/docs/conf.py` & `finderz-2.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/docs/function use.rst` & `finderz-2.0.5/docs/function use.rst`

 * *Files 2% similar despite different names*

```diff
@@ -498,15 +498,15 @@
 * Optional backup folder. This is useful if you want to make sure no data is lost by accident. It will automatically move everything deleted in this folder.
 * Optional, complete and detailed logging, which can be saved to a file to a custom path for complete analysis of each process.
 
 The **Synchronization** class is filled with features that are super useful to synchronize two directories effectively. Now, lets go over the usage of these functions.
 
 The ``synchronize`` function takes in two required parameters. That's it! These are: dir1 (str), dir2 (str)
 
-It also takes in four optional parameters: importantFilesFlag (str), syncBackUpFolderExists (boolean), loggingBool (boolean), logCreationPath (str).
+It also takes in five optional parameters: importantFilesFlag (str), syncBackUpFolderExists (boolean), loggingBool (boolean), logCreationPath (str), log_non_critical (bool).
 
 If you want to most basic usage, you can execute it like so:
 
 .. code-block:: python
 
     Synchronize.synchronize("/path/to/dir1", "/path/to/dir2")
 
@@ -537,17 +537,17 @@
 
 Now, for the logging. The logging is very easy to use. It provides very detailed information about which actions are performed, when they are performed, and even which mode (Synchronize or Backup) were used. (Backup is explained later on).
 
 If you want to use logging, all you need to do is set the loggingBool to True, and put a path to a directory where to create the log files.
 
 .. code-block:: python
 
-    Synchronize.synchronize("/path/to/dir1", "/path/to/dir2", loggingBool = True, logCreationPath = '/path/to/logcreationdir')
+    Synchronize.synchronize("/path/to/dir1", "/path/to/dir2", loggingBool = True, logCreationPath = '/path/to/logcreationdir', log_non_critical = True)
 
-A log will have log tags, which are either NC (Non critical) or C (Critical). This is used in order to easily find the more important activites (C), such as removing or adding files.
+A log will have log tags, which are either NC (Non critical) or C (Critical). This is used in order to easily find the more important activites (C), such as removing or adding files. You can disable non-critical (and only view critical) logging by setting log_non_critical to False. This can help with minimizing the size of the output log.
 
 A log will also have the time at which each process happened. It may seem like the time never changes, but this is solely due to the fact that the function executes very fast (so it will usually remain within the same second by the time the whole process ends)
 
 **Backup** Usage
 ================
 
 The **Backup** class is very similar to the **Synchronize** class, but it uses a main directory as its bias as to what to follow.
@@ -566,15 +566,15 @@
 
  It takes in two optional parameters: loggingBool (str), logCreationPath (list).
 
  In order to use it, you can do so like this:
 
 .. code-block:: python
 
-    Backup.backup("/path/to/maindir", ["/path/to/backupdir1", "/path/to/backupdir2"], loggingBool = True, logCreationPath = '/path/to/logcreationdir')
+    Backup.backup("/path/to/maindir", ["/path/to/backupdir1", "/path/to/backupdir2"], loggingBool = True, logCreationPath = '/path/to/logcreationdir', log_non_critical = True)
 
 The above code backs up everything in maindir to backupdir1 and backupdir2. Of course, you can have more than two backup dirs, but there are two just as an example. Here, logging is enabled, so that will work. 
 
 ``backgroundBackup``
 --------------------
 
 The ``backgroundBackup`` function is basically the same thing as ``backup``, but it actually goes in the background. It has an extra optional (default = 8) refreshInterval parameter, which defines the interval (in seconds) for each backup.
```

### Comparing `finderz-2.0.4/docs/index.rst` & `finderz-2.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/docs/updatev2.rst` & `finderz-2.0.5/docs/updatev2.rst`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/docs/img/logo-color.jpg` & `finderz-2.0.5/docs/img/logo-color.jpg`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/logo/logo-color.jpg` & `finderz-2.0.5/logo/logo-color.jpg`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/old/src/.DS_Store` & `finderz-2.0.5/old/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/old/src/FinderZ/FinderZLib.py` & `finderz-2.0.5/old/src/FinderZ/FinderZLib.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/old/src/FinderZ/FinderZV2.py` & `finderz-2.0.5/old/src/FinderZ/FinderZV2.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/src/FinderZ/FinderZV2.py` & `finderz-2.0.5/src/FinderZ/FinderZV2.py`

 * *Files 15% similar despite different names*

```diff
@@ -586,15 +586,15 @@
 		f.close()
 	#Remove a single file:
 	def removeFile(filePath):
 		os.remove(filePath)
 #The main logging class (Used in Synchronize and Backup classes)
 class Logging:
 	#Here, the announcement is simply something to announce/thecurrent/main activity or in this case print. dir is the parameter that takes in dir. dirAction consists of things like removing, adding, or copying, renaming, etc.
-	def Log(loggingBool, logList, announcement = '', dir1 = '', dir2 = '', dir1Action = '', dir2Action = '', logTag = 'NC'):
+	def Log(loggingBool, logList, announcement = '', dir1 = '', dir2 = '', dir1Action = '', dir2Action = '', logTag = 'NC', log_non_critical = True):
 		#'NC' = Not Critical, 'C' is Critical, for the logTag
 		#Check if the boolean loggingBool is True, to determine whether or not the User actually wants to log or not:
 		
 		if loggingBool == True:
 			newLogList = []
 			
 			#The main log list (which are really the lines that will be passed on to the writeLogsToFile function). This will be returned at the end:
@@ -626,18 +626,25 @@
 				elif (dir1 and dir2) != '':
 					log = f"\n	{currentTime}: SUBPROCESS: {dir1Action} {dir1} {dir2Action} {dir2}" 
 					print(log)
 					newLogList.append(log)
 				
 				return newLogList
 
-			
-			printAnnouncement(announcement, currentTime)
-			
-			newLogList = logDirectories(newLogList, dir1, dir2, dir1Action, dir2Action, currentTime)
+			#Apply non-critical filter:
+			if log_non_critical == False:
+				if logTag != 'NC':
+
+					printAnnouncement(announcement, currentTime)
+					
+					newLogList = logDirectories(newLogList, dir1, dir2, dir1Action, dir2Action, currentTime)
+			else:
+				printAnnouncement(announcement, currentTime)
+					
+				newLogList = logDirectories(newLogList, dir1, dir2, dir1Action, dir2Action, currentTime)
 		else:
 			return logList
 
 		#This logList will be passed by throughout the whole process, and will then be written out to a file after everything is done.
 		return newLogList
 		
 
@@ -707,16 +714,16 @@
 			fileOperands.copyDir(filePath, syncBackUpFolderPathMain)
 			
 			#Sync path:
 			if os.path.exists(isExistingInSyncBackUpFolderDirectory_Sync) == True:
 				shutil.rmtree(isExistingInSyncBackUpFolderDirectory_Sync)
 			fileOperands.copyDir(filePath, syncBackUpFolderPathSync)
 	
-	#IMPORTANT: Important directories flag is used to never delete certain directories that start with a specific character (default = _ ). The importantFilesFlag is important as it may prevent deletion of directories!
-	def synchronizeComponents(dir1, dir2, syncBackUpFolderName, syncBackUpFolderExists, importantFilesFlag, loggingBool, maindir, syncdir):
+	#IMPORTANT: Important files flag is used to never delete certain files that start with a specific character (default = _ ). The importantFilesFlag is important as it may prevent deletion of files/dirs!
+	def synchronizeComponents(dir1, dir2, syncBackUpFolderName, syncBackUpFolderExists, importantFilesFlag, loggingBool, maindir, syncdir, log_non_critical = True):
 		
 		logList = []
 		#Checks whether or not the directory or file is important by checking the first character of the string:
 		def isImportantFile(dir, importantFilesFlag):
 
 			dir = os.path.basename(os.path.normpath(dir))
 			#Get first character and check if it equals importFilesFlag:
@@ -797,40 +804,40 @@
 			matchBoolean = GatherInfo.isOneInCommon(parentdirHashes, parentdir2Hashes)
 			
 			return matchBoolean
 			#Take in both the parentfiles lists to get the files in each directory. For each of those, create a list with the computed hashes. IF any of those hashes matches any other hash from the other files listed... else...
 			#We can return a boolean. True = mathing. False = not matching. Based on this boolean, we can then execute either deleting or merging.
 			
 		#Main class that takes in dir1, dir2, separates the files and dirs, makes the comparisons, and adds/removes the files, or even renames directories.
-		def main(parentdir, parentdir2, syncBackUpFolderName, syncBackUpFolderExists, importantFilesFlag, loggingBool, maindir, syncdir):
+		def main(parentdir, parentdir2, syncBackUpFolderName, syncBackUpFolderExists, importantFilesFlag, loggingBool, maindir, syncdir, log_non_critical = log_non_critical):
 			
 			logList = []
 			#Get the source components of the parentdir and parentdir2:
 			parentdirs, parentfiles = GatherInfo.readDir(parentdir)
 			parent2dirs, parent2files = GatherInfo.readDir(parentdir2)
 			
 			
 			
 			#First, do the basic operations:
 
 			#To add files:
 			for dir in parentdirs:
 				if dir not in parent2dirs:
 
-					newLogList = Logging.Log(loggingBool, logList, announcement = f"Adding directories that exist in mainpath but not in syncpath (missing/extra).", dir1 = f"'{dir}'", dir2 = parentdir2, dir1Action = 'Found directory', dir2Action = f'in {parentdir}, but not in', logTag = "C")
+					newLogList = Logging.Log(loggingBool, logList, announcement = f"Adding directories that exist in mainpath but not in syncpath (missing/extra).", dir1 = f"'{dir}'", dir2 = parentdir2, dir1Action = 'Found directory', dir2Action = f'in {parentdir}, but not in', logTag = "C", log_non_critical = log_non_critical)
 					logList.extend(newLogList)
 					#If the directory is not in the folder to sync to, then it adds it:
 					path = os.path.join(parentdir2, dir)
 					os.mkdir(path)
 			for file in parentfiles:
 				#If the file is not in the folder to sync to, then it adds it
 				if file not in parent2files:
 					originalpath = os.path.join(parentdir, file)
 
-					newLogList = Logging.Log(loggingBool, logList, announcement = f"Adding files that exist in mainpath but not in syncpath (missing/extra).", dir1 = f"'{file}'", dir2 = parentdir2, dir1Action = 'Found file', dir2Action = f'in {parentdir}, but not in', logTag = 'C')
+					newLogList = Logging.Log(loggingBool, logList, announcement = f"Adding files that exist in mainpath but not in syncpath (missing/extra).", dir1 = f"'{file}'", dir2 = parentdir2, dir1Action = 'Found file', dir2Action = f'in {parentdir}, but not in', logTag = 'C', log_non_critical = log_non_critical)
 					logList.extend(newLogList)
 					fileOperands.copyFile(originalpath, parentdir2)
 
 			#Second, do the hard operations (Merging, replacing with newer versions, important files/dirs)
 			
 			#Pop out the syncBackUps folder name as to not remove any files or folders from there, if the syncBackUpsFolderExists, of course:
 			if syncBackUpFolderExists:
@@ -840,28 +847,28 @@
 					parent2dirs.pop(parent2dirs.index(syncBackUpFolderName))
 
 			#To deal with removing files:
 			for file in parent2files:
 				if file not in parentfiles:
 					
 					#Log it:
-					newLogList = Logging.Log(loggingBool, logList, announcement = f"Removing additional files:", dir1 = os.path.join(parentdir2, file), dir2 = f'Removing file from {parentdir}', dir1Action = 'File found at ', dir2Action = f'but not found in {parentdir}', logTag = 'C')
+					newLogList = Logging.Log(loggingBool, logList, announcement = f"Removing additional files:", dir1 = os.path.join(parentdir2, file), dir2 = f'Removing file from {parentdir}', dir1Action = 'File found at ', dir2Action = f'but not found in {parentdir}', logTag = 'C', log_non_critical = log_non_critical)
 					logList.extend(newLogList)
 					isMatching = mergeFiles(parentdir, parentdir2, parentfiles, parent2files)
 
 					directory = os.path.join(parentdir2, file)
 
 					if isMatching == True or len(parentfiles) < 1:
 						
-						newLogList = Logging.Log(loggingBool, logList, announcement = "Skipping file and directory merging as some files/dirs are matching.", logTag = 'C')
+						newLogList = Logging.Log(loggingBool, logList, announcement = "Skipping file and directory merging as some files/dirs are matching.", logTag = 'C', log_non_critical = log_non_critical)
 						logList.extend(newLogList)
 						#Check if the files are important files. If they are, do not remove them, but rather copy them to the parent dir:
 						if isImportantFile(directory, importantFilesFlag) == True:
 							#Log it:
-							newLogList = Logging.Log(loggingBool, logList, announcement = f"'{directory}' is an important file, as the first character matches the importantFilesFlag. Restoring...", logTag = 'C')
+							newLogList = Logging.Log(loggingBool, logList, announcement = f"'{directory}' is an important file, as the first character matches the importantFilesFlag. Restoring...", logTag = 'C', log_non_critical = log_non_critical)
 							logList.extend(newLogList)
 
 							fileOperands.copyFile(directory, os.path.join(parentdir))
 						else:
 							
 							#If the directory is not in the main directory but is in the sync directory, remove the directory from the sync directory:
 							checkDir = os.path.split(directory)[0]
@@ -869,36 +876,36 @@
 								pass
 							else:
 								#Check if the user wants a backup folder or not:
 								if syncBackUpFolderExists:
 									Synchronize.backUpToSyncFolder(directory, syncBackUpFolderName, maindir, syncdir)
 								
 								#Log it:
-								newLogList = Logging.Log(loggingBool, logList, announcement = f"Removing {file} from {parentdir2}, as it doesn't exist in {parentdir}", logTag = 'C')
+								newLogList = Logging.Log(loggingBool, logList, announcement = f"Removing {file} from {parentdir2}, as it doesn't exist in {parentdir}", logTag = 'C', log_non_critical = log_non_critical)
 								logList.extend(newLogList)
 								os.remove(directory)
 					elif isMatching == False:
 						#Log it:
 						
 						#Merge the directories as well:
 						for dir in parent2dirs:
 							if dir not in parentdirs:
 								#Log it:
-								newLogList = Logging.Log(loggingBool, logList, announcement = "Merging files and dirs, as no files/dirs are matching.", dir1 = dir, dir2 = f"'{parentdir}'. Merging directories...", dir1Action = "Directory '", dir2Action = f"' exists in {parentdir2}, but not in", logTag = 'C')
+								newLogList = Logging.Log(loggingBool, logList, announcement = "Merging files and dirs, as no files/dirs are matching.", dir1 = dir, dir2 = f"'{parentdir}'. Merging directories...", dir1Action = "Directory '", dir2Action = f"' exists in {parentdir2}, but not in", logTag = 'C', log_non_critical = log_non_critical)
 								logList.extend(newLogList)
 								dirDirectory = os.path.join(parentdir2, dir)
 
 								dirDirectoryParent = os.path.join(parentdir, dir)
 								
 								#Copy the files and the directories:
 								if os.path.exists(dirDirectoryParent) == False:
 									fileOperands.copyDir(dirDirectory, os.path.join(parentdir))
 						
 						#Log list:
-						newLogList = Logging.Log(loggingBool, logList, announcement = f"Merging missing file: {file} into {parentdir}", logTag = 'C')
+						newLogList = Logging.Log(loggingBool, logList, announcement = f"Merging missing file: {file} into {parentdir}", logTag = 'C', log_non_critical = log_non_critical)
 						logList.extend(newLogList)
 						fileOperands.copyFile(directory, os.path.join(parentdir))
 			#To deal with directories: (remove from folder to sync to:)
 			for dir in parent2dirs:
 				if dir not in parentdirs:
 					
 					#If the directory is not in the main directory but is in the sync directory, remove the directory from the sync directory:
@@ -906,58 +913,58 @@
 
 					isMatching = mergeDirectories(parentdir, parentdir2, parentdirs, parent2dirs)
 					
 					directory = os.path.join(parentdir2, dir)
 
 					if isMatching == True or len(parentdirs) < 1:
 						#Log it: CONTINUE HERE
-						newLogList = Logging.Log(loggingBool, logList, announcement = "Skipping file and directory merging as some files/dirs are matching.")
+						newLogList = Logging.Log(loggingBool, logList, announcement = "Skipping file and directory merging as some files/dirs are matching.", log_non_critical = log_non_critical)
 						logList.extend(newLogList)
 						
 						#Check if it is important directory:
 						if isImportantFile(directory, importantFilesFlag) == True:
 							#Log it:
-							newLogList = Logging.Log(loggingBool, logList, announcement = f"'{directory}' is an important directory, as the first character matches the importantFilesFlag. Restoring...", logTag ='C')
+							newLogList = Logging.Log(loggingBool, logList, announcement = f"'{directory}' is an important directory, as the first character matches the importantFilesFlag. Restoring...", logTag ='C', log_non_critical = log_non_critical)
 							logList.extend(newLogList)
 							
 							fileOperands.copyDir(directory, os.path.join(parentdir))
 						else:
 							#Here check if the directory name before the directory is the synBackUpFolderName. That way, the remove doesnt deal with the synBackUpsFolder:
 							checkDir = os.path.split(directory)[0]
 							if os.path.basename(os.path.normpath(checkDir)) == syncBackUpFolderName:
 								pass
 							else:
 								#Backup:
 								if syncBackUpFolderExists:
 									Synchronize.backUpToSyncFolder(directory, syncBackUpFolderName, maindir, syncdir)
 								
 								#Log it:
-								newLogList = Logging.Log(loggingBool, logList, announcement = f"Removing {directory} and all of its contents, as it is directory {parentdir2}, but not in {parentdir}", logTag= 'C')
+								newLogList = Logging.Log(loggingBool, logList, announcement = f"Removing {directory} and all of its contents, as it is directory {parentdir2}, but not in {parentdir}", logTag= 'C', log_non_critical = log_non_critical)
 								logList.extend(newLogList)
 
 								shutil.rmtree(directory)
 					else:
 						
 						for file in parent2files:
 							if file not in parentfiles:
 								fileDirectory = os.path.join(parentdir2, file)
 								parentFileDirectory = os.path.join(parentdir, file)
 
 								#Log it:
-								newLogList = Logging.Log(loggingBool, logList, announcement = "Merging files and dirs, as no files/dirs are matching.", dir1 = file, dir2 = f"'{parentdir}'. Merging Files...", dir1Action = "File '", dir2Action = f"' exists in {parentdir2}, but not in", logTag = 'C')
+								newLogList = Logging.Log(loggingBool, logList, announcement = "Merging files and dirs, as no files/dirs are matching.", dir1 = file, dir2 = f"'{parentdir}'. Merging Files...", dir1Action = "File '", dir2Action = f"' exists in {parentdir2}, but not in", logTag = 'C', log_non_critical = log_non_critical)
 								logList.extend(newLogList)
 
 								#Copy the files and the directories:
 								if os.path.exists(parentFileDirectory) == False:
 									fileOperands.copyFile(fileDirectory, os.path.join(parentdir))
 						
 						#Add a try except block in case the function above this one already took care of the directories:
 						try:
 
-							newLogList = Logging.Log(loggingBool, logList, announcement = f"Copying missing dir: {dir}, into {parentdir}", logTag = 'C')
+							newLogList = Logging.Log(loggingBool, logList, announcement = f"Copying missing dir: {dir}, into {parentdir}", logTag = 'C', log_non_critical = log_non_critical)
 							logList.extend(newLogList)
 
 							fileOperands.copyDir(directory, os.path.join(parentdir))
 						except FileExistsError:
 							pass
 
 				
@@ -971,19 +978,19 @@
 				dirsyncfiletime = os.path.getmtime(dirsyncpath)
 				#Compute hashes (hot fix 2.0.4)
 				if (GatherInfo.computeHash(maindirpath) != GatherInfo.computeHash(dirsyncpath)):
 					if (mainfiletime > dirsyncfiletime):
 						#Remove and copy the file:
 						os.remove(dirsyncpath)
 						fileOperands.copyFile(maindirpath, os.path.split(dirsyncpath)[0])
-						newLogList = Logging.Log(loggingBool, logList, announcement = f"Updating file contents:", dir1 = maindirpath, dir2 = "Updating file.", dir1Action = 'File at path', dir2Action = f'was modified before file {dirsyncpath}.', logTag = 'C')
+						newLogList = Logging.Log(loggingBool, logList, announcement = f"Updating file contents:", dir1 = maindirpath, dir2 = "Updating file.", dir1Action = 'File at path', dir2Action = f'was modified before file {dirsyncpath}.', logTag = 'C', log_non_critical = log_non_critical)
 						logList.extend(newLogList)
 					elif mainfiletime < dirsyncfiletime:
 						os.remove(maindirpath)
-						newLogList = Logging.Log(loggingBool, logList, announcement = f"Updating file contents:", dir1 = dirsyncpath, dir2 = "Updating file.", dir1Action = 'File at path', dir2Action = f'was modified before file {maindirpath}.', logTag = 'C')
+						newLogList = Logging.Log(loggingBool, logList, announcement = f"Updating file contents:", dir1 = dirsyncpath, dir2 = "Updating file.", dir1Action = 'File at path', dir2Action = f'was modified before file {maindirpath}.', logTag = 'C', log_non_critical = log_non_critical)
 						logList.extend(newLogList)
 						fileOperands.copyFile(dirsyncpath, os.path.split(maindirpath)[0])
 			return logList
 		#Execute the main function:		
 		newLogList = main(dir1, dir2, syncBackUpFolderName, syncBackUpFolderExists, importantFilesFlag, loggingBool, maindir, syncdir)
 		logList.extend(newLogList)
 		
@@ -1001,22 +1008,22 @@
 			os.mkdir(syncBackUpFolderName)
 
 		os.chdir(dir2)
 		if os.path.exists(syncBackUpFolderName) == False:
 			os.mkdir(syncBackUpFolderName)
 
 	#For synchronizing files and dirs (The main function:)
-	def synchronize(dir1, dir2, importantFilesFlag = '_', syncBackUpFolderExists = True, loggingBool = False, logCreationPath = ''):
+	def synchronize(dir1, dir2, importantFilesFlag = '_', syncBackUpFolderExists = True, loggingBool = False, logCreationPath = '', log_non_critical = True):
 		
 		#The main logList:
 		logList = []
 
 		#Log it:
 		#Check if the user actually wants to create a syncBackUpFolder (It is recommended in order to reduce the chances of accidental file loss!)
-		newLogList = Logging.Log(loggingBool, logList, announcement = f"Running in mode SYNCHRONIZATION: importantFilesFlag = '{importantFilesFlag}', syncBackUpFolderExists = {syncBackUpFolderExists}", logTag = 'C')
+		newLogList = Logging.Log(loggingBool, logList, announcement = f"Running in mode SYNCHRONIZATION: importantFilesFlag = '{importantFilesFlag}', syncBackUpFolderExists = {syncBackUpFolderExists}", logTag = 'C', log_non_critical = log_non_critical)
 		#Append to the logList
 		logList.extend(newLogList)
 		#Initialize the backup directory:
 		syncBackUpFolderName = f"{importantFilesFlag}syncBackups"
 		if syncBackUpFolderExists == True:
 			
 			#Create the backup Folder:
@@ -1076,120 +1083,121 @@
 
 
 
 		dir1time = max(dir1ti_m)
 		dir2time = max(dir2ti_m)
 
 		#Log it:
-		newLogList = Logging.Log(loggingBool, logList, announcement = f"Recursively got the time last modified for each directory: {dir1time} for {dir1} and {dir2time} for {dir2}",)
+		newLogList = Logging.Log(loggingBool, logList, announcement = f"Recursively got the time last modified for each directory: {dir1time} for {dir1} and {dir2time} for {dir2}", log_non_critical = log_non_critical)
 		#Append to the logList
 		logList.extend(newLogList)
 
 		#The greater (bigger) time indicates the folder that was edited most recently:
 		if float(dir1time) > float(dir2time):
 			#IMPORTANT: Here, place if statement, deciding which folder was edited last (In other words, decide which one should follow the other based on the time they were edited. The one that gets edited the most recent gets the priority)
 			#When doing the above, invert the dir1 with dir2 (Because you are doing pretty much the opposite!)
 			for folder, dirs, files in os.walk(dir1):
 				#Here, get everything that is after the dir1 in order to get the other directories:
 				
 				childdir = (folder.split(dir1,1)[1])
 				
 				syncpath = os.path.join(dir2, childdir)
 
-				newLogList = Logging.Log(loggingBool, logList, announcement = f"Iterating through main loop with {dir1} as the main dir, as {dir2} has an older modification time.", dir1 = folder, dir2 = syncpath, dir1Action = 'Entering child directory', dir2Action = "to compare files and dirs with ")
+				newLogList = Logging.Log(loggingBool, logList, announcement = f"Iterating through main loop with {dir1} as the main dir, as {dir2} has an older modification time.", dir1 = folder, dir2 = syncpath, dir1Action = 'Entering child directory', dir2Action = "to compare files and dirs with ", log_non_critical = log_non_critical)
 				#Append to the logList
 				logList.extend(newLogList)
 				
 				#Set the newLogList equal to the log that the function returns:
-				newLogList = Synchronize.synchronizeComponents(folder, syncpath, syncBackUpFolderName, syncBackUpFolderExists, importantFilesFlag, loggingBool, maindir, syncdir)
+				newLogList = Synchronize.synchronizeComponents(folder, syncpath, syncBackUpFolderName, syncBackUpFolderExists, importantFilesFlag, loggingBool, maindir, syncdir, log_non_critical = log_non_critical)
 				logList.extend(newLogList)
 
 		elif float(dir1time) < float(dir2time):
 			for folder, dirs, files in os.walk(dir2):
 				#Here, get everything that is after the dir1 in order to get the other directories:
 				childdir = (folder.split(dir2,1)[1])
 				syncpath = os.path.join(dir1, childdir)
 
-				newLogList = Logging.Log(loggingBool, logList, announcement = f"Iterating through main loop with {dir2} as the main dir, as {dir1} has an older modification time.", dir1 = folder, dir2 = syncpath, dir1Action = 'Entering child directory', dir2Action = "to compare files and dirs with ")
+				newLogList = Logging.Log(loggingBool, logList, announcement = f"Iterating through main loop with {dir2} as the main dir, as {dir1} has an older modification time.", dir1 = folder, dir2 = syncpath, dir1Action = 'Entering child directory', dir2Action = "to compare files and dirs with ", log_non_critical = log_non_critical)
 				#Append to the logList
 				logList.extend(newLogList)
 
 				#Set the newLogList equal to the log that the function returns:
-				newLogList = Synchronize.synchronizeComponents(folder, syncpath, syncBackUpFolderName, syncBackUpFolderExists, importantFilesFlag, loggingBool, maindir, syncdir)
+				newLogList = Synchronize.synchronizeComponents(folder, syncpath, syncBackUpFolderName, syncBackUpFolderExists, importantFilesFlag, loggingBool, maindir, syncdir, log_non_critical = log_non_critical)
 				
 		
 				logList.extend(newLogList)
 		#At the very end, check if loggingBool is True. If it is, write the lines of the list logList to the specific directory of where the Log should be created:
 		if loggingBool == True:
 			#Write logs to file:
 			Logging.writeLogsToFile(logCreationPath, logList, 'synchronize')
 			
 #Class Backup: Unlike synchronization, this backs up to a 'child' directory, meaning that the 'child' directory plays no role on the parent one.
 class Backup:
 	#Capture the newLogList from the mainIteration function:
-	def main(parentmaindir, childbackupdir, loggingBool):
+	def main(parentmaindir, childbackupdir, loggingBool, log_non_critical = True):
 		
 		
 		
 		#Define the main loglist to append to:
 		logList = []
 		
 		
 		#Get the source components of the parentdir and childsyncdir (in order to compare them later:)
+		
 		maindirs, mainfiles = GatherInfo.readDir(parentmaindir)
 		syncdirs, syncfiles = GatherInfo.readDir(childbackupdir)
 		
 		#Log it:
-		newLogList = Logging.Log(loggingBool, logList, announcement = "Reading directories and files in the listed directories:", dir1 = parentmaindir, dir2 = childbackupdir, dir2Action = ',')
+		newLogList = Logging.Log(loggingBool, logList, announcement = "Reading directories and files in the listed directories:", dir1 = parentmaindir, dir2 = childbackupdir, dir2Action = ',', log_non_critical=log_non_critical)
 		#Append to the logList
 		logList.extend(newLogList)
 		
 		#To add files:
 		for dir in maindirs:
 			if dir not in syncdirs:
 				#If the directory is not in the folder to sync to, then it adds it:
 
 				#Log it:
-				newLogList = Logging.Log(loggingBool, logList, announcement = "Adding missing directories in the backup folder(s): ", dir1 = parentmaindir, dir2 = childbackupdir, dir1Action = f"Dir '{dir}' found in", dir2Action = 'but not found in', logTag = 'C')
+				newLogList = Logging.Log(loggingBool, logList, announcement = "Adding missing directories in the backup folder(s): ", dir1 = parentmaindir, dir2 = childbackupdir, dir1Action = f"Dir '{dir}' found in", dir2Action = 'but not found in', logTag = 'C', log_non_critical=log_non_critical)
 				#Append to the logList
 				logList.extend(newLogList)
 
 				path = os.path.join(childbackupdir, dir)
 				os.mkdir(path)
 		for file in mainfiles:
 			#If the file is not in the folder to sync to, then it adds it:
 			if file not in syncfiles:
 				filepath = os.path.join(parentmaindir, file)
 
-				newLogList = Logging.Log(loggingBool, logList, announcement = "Adding missing files in the backup folder(s): ", dir1 = parentmaindir, dir2 = childbackupdir, dir1Action = f"File '{file}' found in", dir2Action = 'but not found in', logTag = 'C')
+				newLogList = Logging.Log(loggingBool, logList, announcement = "Adding missing files in the backup folder(s): ", dir1 = parentmaindir, dir2 = childbackupdir, dir1Action = f"File '{file}' found in", dir2Action = 'but not found in', logTag = 'C', log_non_critical=log_non_critical)
 				#Append to the logList
 				logList.extend(newLogList)
 
 				fileOperands.copyFile(filepath, childbackupdir)
 
 		#To remove files (remove from folder to sync to:)
 		for dir in syncdirs:
 			if dir not in maindirs:
 				
 				#Log it:
-				newLogList = Logging.Log(loggingBool, logList, announcement = "Removing extra directories in the backup folder: ", dir1 = parentmaindir, dir2 = childbackupdir, dir1Action = f"File '{file}' not found in", dir2Action = 'but found in backup folder. Removing from backup Folder:', logTag = 'C')
+				newLogList = Logging.Log(loggingBool, logList, announcement = "Removing extra directories in the backup folder: ", dir1 = parentmaindir, dir2 = childbackupdir, dir1Action = f"File '{file}' not found in", dir2Action = 'but found in backup folder. Removing from backup Folder:', logTag = 'C', log_non_critical=log_non_critical)
 				#Append to the logList
 				logList.extend(newLogList)
 				#If the directory is in the backup directory but not in the main dir, remove the dir from the backup (sync) directory:
 				directory = os.path.join(childbackupdir, dir)
 			
 				
 				shutil.rmtree(directory)
 		
 		#Remove the file from the 
 		for file in syncfiles:
 			if file not in mainfiles:
 				
 				#Log it:
-				newLogList = Logging.Log(loggingBool, logList, announcement = "Removing any extra files in the backup folder: ", dir1 = parentmaindir, dir2 = childbackupdir, dir1Action = f"File '{file}'not found in", dir2Action = 'but found in backup folder. Adding removing from backup Folder:', logTag = 'C')
+				newLogList = Logging.Log(loggingBool, logList, announcement = "Removing any extra files in the backup folder: ", dir1 = parentmaindir, dir2 = childbackupdir, dir1Action = f"File '{file}'not found in", dir2Action = 'but found in backup folder. Adding removing from backup Folder:', logTag = 'C', log_non_critical=log_non_critical)
 				logList.extend(newLogList)
 				
 				#If the backup directory has the file but the main one doesn't, remove it from the backup directory:
 				os.remove(os.path.join(childbackupdir, file))	
 
 		#Use this to update file content:
 		for file in mainfiles:
@@ -1197,86 +1205,86 @@
 				dirsyncpath = os.path.join(childbackupdir, file)
 
 				mainfiletime = os.path.getmtime(maindirpath)
 
 				dirsyncfiletime = os.path.getmtime(dirsyncpath)
 
 				#If the file needs to be updated, remove the old one and copy the new one to the backup folder:
-				if mainfiletime > dirsyncfiletime:
-					#Remove and copy the file:
-					os.remove(dirsyncpath)
-					fileOperands.copyFile(maindirpath, os.path.split(dirsyncpath)[0])
-				
-					newLogList = Logging.Log(loggingBool, logList, announcement = f"Updating content of file '{file}'", dir1 = dirsyncpath, dir2 = maindirpath, dir1Action = "Updating file content at '", dir2Action = f"' as file '{file}' in backup folder is older than")
-					logList.extend(newLogList)
+				if (GatherInfo.computeHash(maindirpath) != GatherInfo.computeHash(dirsyncpath)):
+					if mainfiletime > dirsyncfiletime:
+						#Remove and copy the file:
+						os.remove(dirsyncpath)
+						fileOperands.copyFile(maindirpath, os.path.split(dirsyncpath)[0])
+					
+						newLogList = Logging.Log(loggingBool, logList, announcement = f"Updating content of file '{file}'", dir1 = dirsyncpath, dir2 = maindirpath, dir1Action = "Updating file content at '", dir2Action = f"' as file '{file}' in backup folder is older than", logTag = 'C', log_non_critical=log_non_critical)
+						logList.extend(newLogList)
 		
 		#At the end of the main() function, return the logList
 		return logList
-	def mainIteration(maindir, backupdir, loggingBool):
+	def mainIteration(maindir, backupdir, loggingBool, log_non_critical = True):
 		
 		logList = []
 		for folder, dirs, files in os.walk(maindir):
 			
 			childdir = (folder.split(maindir,1)[1])
-
+			backupdir = Synchronize.organizePathSlashes(backupdir)
 			#Here, the very start is blank because the childdir is blank (Perhaps, just leave it as is? It does not really matter)
-
-			backUpFullPath = os.path.join(backupdir, childdir.replace("/", ''))
+			backUpFullPath = os.path.join(backupdir, childdir.replace("/", '', 1))
 			#Log it:
-			newLogList = Logging.Log(loggingBool, logList, announcement = "Entering main loop under mainIteration function", dir1 = childdir, dir2 = backUpFullPath, dir1Action = "Merged child path string '", dir2Action = "' into sync path:")
+			newLogList = Logging.Log(loggingBool, logList, announcement = "Entering main loop under mainIteration function", dir1 = childdir, dir2 = backUpFullPath, dir1Action = "Merged child path string '", dir2Action = "' into sync path:", log_non_critical=log_non_critical)
 			logList.extend(newLogList)
 			
 			#Transfer the newLogList to the main() function:
 
-			logListMain = Backup.main(folder, backUpFullPath, loggingBool)
+			logListMain = Backup.main(folder, backUpFullPath, loggingBool, log_non_critical = log_non_critical)
 
 			logList.extend(logListMain)
 		
 		#Return the logList, which is the file lines to write:
 		return logList
-	def backup(maindir, backupdirs, loggingBool = False, logCreationPath = ''):
+	def backup(maindir, backupdirs, loggingBool = False, logCreationPath = '', log_non_critical = True):
 		#Initialize the main logList:
 		logList = [] 
 		
-		newLogList = Logging.Log(loggingBool, logList, announcement = "Running in BACKUP mode:", logTag = 'C')
+		newLogList = Logging.Log(loggingBool, logList, announcement = "Running in BACKUP mode:", logTag = 'C', log_non_critical=log_non_critical)
 		
 		logList.extend(newLogList)
 		
 		
 		if isinstance(backupdirs, list) != True:
 			raise Exception("ERR: 'backupdirs' must be of type 'list'")
 		
 		#For every dir within the backup directories, backup:
 		for dir in backupdirs:
 			if len(backupdirs) > 1:
-				newLog = Logging.Log(loggingBool, logList, announcement = f"Multiple Directories were given. Now, backing up to directory: {dir}")
+				newLog = Logging.Log(loggingBool, logList, announcement = f"Multiple Directories were given. Now, backing up to directory: {dir}", log_non_critical=log_non_critical)
 				logList.extend(newLog)
-			newLogList = Backup.mainIteration(maindir, dir, loggingBool)
+			newLogList = Backup.mainIteration(maindir, dir, loggingBool, log_non_critical=log_non_critical)
 			logList.extend(newLogList)
 		#Write the logs:
 		
 		if loggingBool == True:
 			Logging.writeLogsToFile(logCreationPath, logList, 'backup')
-	def backgroundBackup(maindir, backupdirs, loggingBool = False, logCreationPath = '', refreshInterval = 8):
+	def backgroundBackup(maindir, backupdirs, loggingBool = False, logCreationPath = '', refreshInterval = 8, log_non_critical = True):
 
 		#Now, implement logging in the synchronization algorithm.
 		modeAnnounced = False
 		while True:
 			logList = []
 			if modeAnnounced == False:
-				newLogList = Logging.Log(loggingBool, logList, announcement = "Running in BACKGROUNDBACKUP mode:", logTag = 'C')
+				newLogList = Logging.Log(loggingBool, logList, announcement = "Running in BACKGROUNDBACKUP mode:", logTag = 'C', log_non_critical=log_non_critical)
 				logList.extend(newLogList)
 				modeAnnounced = True
 			
 			for dir in backupdirs:
 				
 				if len(backupdirs) > 1:
-					newLog = Logging.Log(loggingBool, logList, announcement = f"Multiple Directories were given. Now, backing up to directory: {dir}")
+					newLog = Logging.Log(loggingBool, logList, announcement = f"Multiple Directories were given. Now, backing up to directory: {dir}", log_non_critical=log_non_critical)
 					logList.extend(newLog)
-				newLogList = Backup.mainIteration(maindir, dir, loggingBool)
+				newLogList = Backup.mainIteration(maindir, dir, loggingBool, log_non_critical=log_non_critical)
 				logList.extend(newLogList)
 				#Write the logs to a file:
 			if loggingBool == True:
 				Logging.writeLogsToFile(logCreationPath, logList, 'backgroundBackup')
 			time.sleep(refreshInterval)
 			
 #Call a bash/shell script:
```

### Comparing `finderz-2.0.4/tests/.DS_Store` & `finderz-2.0.5/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/tests/updates/.DS_Store` & `finderz-2.0.5/tests/updates/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/tests/updates/V2 Changelog.txt` & `finderz-2.0.5/tests/updates/V2 Changelog.txt`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/tests/updates/parentFunctions.py` & `finderz-2.0.5/tests/updates/parentFunctions.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/tests/updates/update.py` & `finderz-2.0.5/tests/updates/update.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/LICENSE` & `finderz-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `finderz-2.0.4/README.md` & `finderz-2.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 **AND: Huge thank you to [@RichardDally](https://github.com/RichardDally) , [@mikudae](https://github.com/mikudae) , [@kyzsuukii](https://github.com/kyzsuukii) , and [@fablau](github.com/fablau) for starring FinderZ.**
 ## **Written in python, this library provides you with different file operation commands as well as info gathering commands on directories as well as files.** 
 ____________________________________________________________________________
 ## **CHANGELOG: V2.0.0**
 
 To check out the details of V2, go to the [documentation](https://finderz.readthedocs.io/en/latest/index.html). This is a big update with many new things!
 
+**Minor Fix Version 2.0.5:**
+1. Added log_non_critical parameter in the Synchronize and Backup class functions. If put to False, only critical actions will be displayed, resulting in a minimized log.
+2. Fixed file updating in Backup class by adding hash computation to the backup function when updating files. This was already in the Synchronize class.
+3. Fixed the Backup directories error (I thought this was already fixed before, but it is totally fixed now.)
 
 **Minor Fix Version 2.0.4:**
 - Fixed bug where removing more than one file at a time gave an existence error. Sorry for that!
 - Fixed bug where removing a folder that contained folder with the same name as the sync backup folder would result in an infinite loop of backup folders being created.
 - Minimized logging by making file updating hash-dependent. Now, updating files is marked as a critical (C) action in the log.
 - Removed unnecessary printing in some functions.
 - Added a file comparison function in GatherInfo
@@ -87,8 +91,8 @@
 - [Time module](https://docs.python.org/3/library/time.html)
 - [Hashlib module](https://docs.python.org/3/library/hashlib.html)
 - [re](https://docs.python.org/3/library/re.html)
 - [Subprocess module](https://docs.python.org/3/library/subprocess.html)
 
 ____________________________________________________________________________
 ## **Make sure to leave a star!**
-- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
+- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
```

### Comparing `finderz-2.0.4/pyproject.toml` & `finderz-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FinderZ"
-version = "2.0.4"
+version = "2.0.5"
 authors = [
 	{ name="PatzEdi", email="patzedigithub@gmail.com" },
 ]
 description = "A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 keywords = ["files", "filemanagement", "library", "development"]
```

### Comparing `finderz-2.0.4/PKG-INFO` & `finderz-2.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinderZ
-Version: 2.0.4
+Version: 2.0.5
 Summary: A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!
 Project-URL: Homepage, https://github.com/PatzEdi
 Project-URL: Repository, https://github.com/PatzEdi/FinderZ
 Project-URL: Bug Tracker, https://github.com/PatzEdi/FinderZ/issues
 Author-email: PatzEdi <patzedigithub@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
@@ -45,14 +45,18 @@
 **AND: Huge thank you to [@RichardDally](https://github.com/RichardDally) , [@mikudae](https://github.com/mikudae) , [@kyzsuukii](https://github.com/kyzsuukii) , and [@fablau](github.com/fablau) for starring FinderZ.**
 ## **Written in python, this library provides you with different file operation commands as well as info gathering commands on directories as well as files.** 
 ____________________________________________________________________________
 ## **CHANGELOG: V2.0.0**
 
 To check out the details of V2, go to the [documentation](https://finderz.readthedocs.io/en/latest/index.html). This is a big update with many new things!
 
+**Minor Fix Version 2.0.5:**
+1. Added log_non_critical parameter in the Synchronize and Backup class functions. If put to False, only critical actions will be displayed, resulting in a minimized log.
+2. Fixed file updating in Backup class by adding hash computation to the backup function when updating files. This was already in the Synchronize class.
+3. Fixed the Backup directories error (I thought this was already fixed before, but it is totally fixed now.)
 
 **Minor Fix Version 2.0.4:**
 - Fixed bug where removing more than one file at a time gave an existence error. Sorry for that!
 - Fixed bug where removing a folder that contained folder with the same name as the sync backup folder would result in an infinite loop of backup folders being created.
 - Minimized logging by making file updating hash-dependent. Now, updating files is marked as a critical (C) action in the log.
 - Removed unnecessary printing in some functions.
 - Added a file comparison function in GatherInfo
@@ -104,8 +108,8 @@
 - [Time module](https://docs.python.org/3/library/time.html)
 - [Hashlib module](https://docs.python.org/3/library/hashlib.html)
 - [re](https://docs.python.org/3/library/re.html)
 - [Subprocess module](https://docs.python.org/3/library/subprocess.html)
 
 ____________________________________________________________________________
 ## **Make sure to leave a star!**
-- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
+- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
```

