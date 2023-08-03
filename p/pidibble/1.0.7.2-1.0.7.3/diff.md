# Comparing `tmp/pidibble-1.0.7.2.tar.gz` & `tmp/pidibble-1.0.7.3.tar.gz`

## Comparing `pidibble-1.0.7.2.tar` & `pidibble-1.0.7.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/.readthedocs.yaml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/MANIFEST.in
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/docs/make.bat
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/docs/source/api.rst
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/docs/source/conf.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/docs/source/index.rst
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/docs/source/notes.md
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/docs/source/usage.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/pidibble/__init__.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/pidibble/baseparsers.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/pidibble/baserecord.py
--rw-r--r--   0        0        0     7518 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/pidibble/pdbparse.py
--rw-r--r--   0        0        0    15375 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/pidibble/pdbrecord.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/pidibble/resources/__init__.py
--rw-r--r--   0        0        0    24391 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/pidibble/resources/pdb_format.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/tests/__init__.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/tests/conftest.py
--rw-r--r--   0        0        0    28325 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/tests/unit/test_rcsb.py
--rw-r--r--   0        0        0  2098386 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/tests/unit/test_rcsb/4tvp.pdb
--rw-r--r--   0        0        0   862642 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/tests/unit/test_rcsb/4zmj.pdb
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/tests/unit/test_rcsb/test.pdb
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/tests/unit/test_rcsb/test_pdb_format.yaml
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/LICENSE
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/README.md
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 pidibble-1.0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/.readthedocs.yaml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/MANIFEST.in
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/docs/make.bat
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/docs/source/api.rst
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/docs/source/conf.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/docs/source/index.rst
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/docs/source/notes.md
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/docs/source/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/pidibble/__init__.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/pidibble/baseparsers.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/pidibble/baserecord.py
+-rw-r--r--   0        0        0     7518 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/pidibble/pdbparse.py
+-rw-r--r--   0        0        0    17535 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/pidibble/pdbrecord.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/pidibble/resources/__init__.py
+-rw-r--r--   0        0        0    24797 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/pidibble/resources/pdb_format.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/tests/__init__.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/tests/conftest.py
+-rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/tests/unit/test_rcsb.py
+-rw-r--r--   0        0        0  2098386 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/tests/unit/test_rcsb/4tvp.pdb
+-rw-r--r--   0        0        0   862642 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/tests/unit/test_rcsb/4zmj.pdb
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/tests/unit/test_rcsb/test.pdb
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/tests/unit/test_rcsb/test_pdb_format.yaml
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/LICENSE
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/README.md
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 pidibble-1.0.7.3/PKG-INFO
```

### Comparing `pidibble-1.0.7.2/.readthedocs.yaml` & `pidibble-1.0.7.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/docs/Makefile` & `pidibble-1.0.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/docs/make.bat` & `pidibble-1.0.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/docs/source/conf.py` & `pidibble-1.0.7.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/docs/source/index.rst` & `pidibble-1.0.7.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/docs/source/notes.md` & `pidibble-1.0.7.3/docs/source/notes.md`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/docs/source/usage.rst` & `pidibble-1.0.7.3/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/pidibble/baseparsers.py` & `pidibble-1.0.7.3/pidibble/baseparsers.py`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/pidibble/baserecord.py` & `pidibble-1.0.7.3/pidibble/baserecord.py`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/pidibble/pdbparse.py` & `pidibble-1.0.7.3/pidibble/pdbparse.py`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/pidibble/pdbrecord.py` & `pidibble-1.0.7.3/pidibble/pdbrecord.py`

 * *Files 8% similar despite different names*

```diff
@@ -182,89 +182,115 @@
                 embedfmt=format_dict.get(espec['record_format'],{})
                 assert embedfmt!={},f'Record {self.key} contains an embedded_records specification with an invalid record format [{espec["record_format"]}]'
             else:
                 assert type(espec['record_format'])==dict,'Record {self.key} has an embed spec {ename} for which no format is specified'
                 embedfmt=espec['record_format']
             skiplines=espec.get('skiplines',0)
             tokenize=espec.get('tokenize',{})
-            header=embedfmt.get('header',{})
+            headers=espec.get('headers',{})
+            token_hold={}
+            header_hold=[]
             if tokenize:
-                self.tokens={}
                 tokenparser=BaseRecordParser({'token':tokenize['from']},typemap).parse
-            # if header:
-            #     headerparser=
+                if headers:
+                    headertokenparse=BaseRecordParser({k:v['format'] for k,v in headers['formats'].items()},typemap).parse
+                    headernum=0
             key=base_key
             embedkey=base_key
             idx=-1
             lskip=0
             triggered=False
             capturing=False
             for record in self.__dict__[embedfrom]:
                 # check for signal
-
                 sigrec=sigparse(record)
                 if not triggered and sigrec.signal==espec['value']:
                     # this is a signal-line
                     triggered=True
-                    if not skiplines and not tokenize:
+                    if not skiplines and not tokenize and not headers:
                         capturing=True
                     embedkey=f'{base_key}.{ename}'
                     if hasattr(sigrec,'record_index'):
                         idx=sigrec.record_index
-                        embedkey=f'{base_key}.{ename}.{idx}' # this separates biomolecules
-                    # print(f'initiating capture for key {key} using {embedkey}')
-                elif triggered and not capturing:
+                        embedkey=f'{base_key}.{ename}{idx}'
+                    savkey=embedkey
+                    continue
+                if triggered and not capturing:
+                    # we can skip lines or we can gather tokens
                     if skiplines:
                         # print(f'Skipping {record}')
                         lskip+=1
                         if lskip==skiplines:
                             capturing=True
-                    elif tokenize:
-                        tokenrec=tokenparser(record)
-                        tokenstr=tokenrec.token
-                        # print(f'Checking non-data line for tokenization "{tokenstr}"')
+                        continue
+                    if tokenize:
+                        tokenstr=tokenparser(record).token
                         if tokenize['d'] in tokenstr:
                             k,v=tokenstr.split(tokenize['d'])
-                            self.tokens[k]=v
-                        else:
-                            capturing=True
+                            header_hold=header_check(record,headers,headertokenparse,header_hold)
+                            # print('header_hold',header_hold)
+                            if not header_hold:
+                                token_hold=gather_token(k,v,token_hold)
+                            continue
+                        # if we are tokenizing after the trigger, then 
+                        # the first occurrence of a line that is not token-containing
+                        # turns on capturing
+                        capturing=True
                 elif capturing:
+                    # if we are capturing, the first occurrence of a blank line
+                    # terminates the search for embedded records
                     if(terparser(record).blank==''):
                         # print(f'Terminate embed capture for {embedkey} from record  {record}')
-                        break # blank line ends the subrecord
+                        break
                     # print(f'Parsing "{record}"')
-                    # we may hit a token line in the middle of the table
+                    # capturing can capture embedded records or tokens
                     if tokenize:
-                        tokenrec=tokenparser(record)
-                        tokenstr=tokenrec.token
-                        # print(f'Checking non-data line for tokenization "{tokenstr}"')
-                        if tokenize['d'] in tokenstr:
+                        tokenstr=tokenparser(record).token
+                        if tokenize['d'] in tokenstr: # for sure this is a token
+                            if not header_hold:
+                                embedkey=savkey
                             k,v=tokenstr.split(tokenize['d'])
-                            # print(f'while capturing encountered token line: {k} {v}')
-                            if k in self.tokens:
-                                if type(self.tokens[k])!=list:
-                                    self.tokens[k]=[self.tokens[k]]
-                                self.tokens[k].append(v)
-                            else:
-                                self.tokens[k]=v
+                            header_hold=header_check(record,headers,headertokenparse,header_hold)
+                            if not header_hold:
+                                token_hold=gather_token(k,v,token_hold)
+                            continue
                             # we are done with this record
                             # print(f'We are done with {record}')
-                            continue
+                    # if there is either a token_hold or a header_hold, and
+                    # we have made it this far (so we know we are parsing a true subrecord
+                    # line), we hand the holds off to the new record, and reset them
+                    if header_hold:
+                        headernum+=1
+                        savkey=embedkey
+                        embedkey=f'{embedkey}.{headers["divlabel"]}{headernum}'
+                        # print(f'header hold updates key to {embedkey}')
+                    # print(f'record to {embedkey}')
                     new_record=PDBRecord.newrecord(embedkey,record,embedfmt,typemap)
                     key=new_record.key
                     record_format=new_record.format
+                    if header_hold:
+                        new_record.header=header_hold
+                        header_hold=[]
+                    if token_hold:
+                        new_record.tokens=token_hold
+                        token_hold={}
                     # print(f'new record has key {key}')
                     if not key in new_records:
                 # print(f'new record for {key}')
                         new_records[key]=new_record
                     else:
                 # this must be a continuation record
                 # print(f'continuing record for {key}')
                         root_record=new_records[key]
                         root_record.continue_record(new_record,record_format)
+                        if hasattr(new_record,'tokens'):
+                            if hasattr(root_record,'tokens'):
+                                root_record.tokens.update(new_record.tokens)
+                            else:
+                                root_record.tokens=new_record.tokens
                 # else:
                     # print(f'Ingoring {record}')
                         
         # print(f'embed rec new keys',new_records)
         return new_records
 
     def parse_tables(self,typemap):
@@ -299,7 +325,27 @@
                     if sigparser(l).signal=='':
                         # print(f'Terminate table {tname}')
                         scanbegin=i+1
                         break
                     parsedrow=rowparser(l)
                     if not all([x=='' for x in parsedrow.__dict__.values()]):
                         self.tables[tname].append(parsedrow)
+
+def header_check(record,headers,parse,hold=[]):
+    r=parse(record)
+    if r.mainline==headers['formats']['mainline']['signalvalue']:
+        hold=[x.strip() for x in r.value.strip().split(',')]
+        if '' in hold:
+            hold.remove('')
+    elif r.andline==headers['formats']['andline']['signalvalue']:
+        hold.extend([x.strip() for x in r.value.strip().split(',')])
+    return hold
+
+def gather_token(k,v,hold={}):
+    if k in hold:
+        if not type(hold[k])==list:
+            hold[k]=[hold[k],v]
+        else:
+            hold[k].append(v)
+    else:
+        hold[k]=v
+    return hold
```

### Comparing `pidibble-1.0.7.2/pidibble/resources/pdb_format.yaml` & `pidibble-1.0.7.3/pidibble/resources/pdb_format.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -776,14 +776,25 @@
               from: freetext
               signal: [String,[12,22]]
               value: BIOMOLECULE
               record_index: [Integer,[24,26]]
               tokenize:  # lines between the signal line and the embedded record data header are tokenized if a delimiter is found
                 d: ':'
                 from: [String,[12,80]]
+              headers:
+                divlabel: TRANSFORM
+                formats:
+                  mainline:
+                    format: [String,[12,40]]
+                    signalvalue: APPLY THE FOLLOWING TO CHAINS
+                  andline:
+                    format: [String,[31,40]]
+                    signalvalue: AND CHAINS
+                  value:
+                    format: [String,[43,80]]
               record_format:
                 fields:
                   rowName: [SList,[14,19]]
                   replNum: [Integer,[21,23]]
                   m1: [Float,[24,33]]
                   m2: [Float,[34,43]]
                   m3: [Float,[44,53]]
```

### Comparing `pidibble-1.0.7.2/tests/conftest.py` & `pidibble-1.0.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/tests/unit/test_rcsb.py` & `pidibble-1.0.7.3/tests/unit/test_rcsb.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,19 +432,20 @@
                                             [0.866025,0.500000,0.000000],
                                             [ 0.00000,  0.000000,1.000000]
                                         ])))
         self.assertTrue(np.array_equal(Tlist[-1],np.array([0.0,0.0,51.53])))
     
     def test_remark_350(self):
         self.assertTrue('REMARK.350' in self.P.parsed)
-        self.assertTrue(hasattr(self.P.parsed['REMARK.350'],'tokens'))
+        # self.assertTrue(hasattr(self.P.parsed['REMARK.350'],'tokens'))
         rec=self.P.parsed['REMARK.350']
-        self.assertEqual(rec.tokens['APPLY THE FOLLOWING TO CHAINS'],' G, B, A, C, D')
-        self.assertTrue('REMARK.350.BIOMOLECULE.1' in self.P.parsed)
-        rec=self.P.parsed['REMARK.350.BIOMOLECULE.1']
+        # self.assertEqual(rec.tokens['APPLY THE FOLLOWING TO CHAINS'],' G, B, A, C, D')
+        # self.assertTrue('REMARK.350.BIOMOLECULE1' in self.P.parsed)
+        self.assertTrue('REMARK.350.BIOMOLECULE1.TRANSFORM1' in self.P.parsed)
+        rec=self.P.parsed['REMARK.350.BIOMOLECULE1.TRANSFORM1']
         Mlist,Tlist=get_symm_ops(rec)
         self.assertEqual(len(Mlist),3)
         self.assertTrue(np.array_equal(Mlist[0],np.identity(3)))
         self.assertTrue(np.array_equal(Mlist[1],
                                        np.array(
                                         [
                                             [-0.500000,-0.866025,0.000000],
@@ -587,31 +588,35 @@
     
     def test_title(self):
         p=self.P.parsed
         self.assertEqual(p['TITLE'].title,'CRYSTAL STRUCTURE OF THE HIV-1 BG505 SOSIP.664 ENV TRIMER ECTODOMAIN, COMPRISING ATOMIC-LEVEL DEFINITION OF PRE-FUSION GP120 AND GP41, IN COMPLEX WITH HUMAN ANTIBODIES PGT122 AND 35O22')
 
     def test_remark_350(self):
         self.assertTrue('REMARK.350' in self.P.parsed)
-        self.assertTrue(hasattr(self.P.parsed['REMARK.350'],'tokens'))
         rec=self.P.parsed['REMARK.350']
-        # self.assertEqual(rec.tokens['APPLY THE FOLLOWING TO CHAINS'],[' G, B, L, H, D, E, A, C, F, I,', ' G, B, L, H, D, E, A, C, F, I,'])
-        self.assertTrue('REMARK.350.BIOMOLECULE.1' in self.P.parsed)
-        rec=self.P.parsed['REMARK.350.BIOMOLECULE.1']
-        print(rec)
+        self.assertTrue('REMARK.350.BIOMOLECULE1.TRANSFORM1' in self.P.parsed)
+        rec=self.P.parsed['REMARK.350.BIOMOLECULE1.TRANSFORM1']
+        self.assertEqual(rec.header,['G', 'B', 'L', 'H', 'D', 'E', 'A', 'C', 'F', 'I', 'J', 'K', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T'])
         Mlist,Tlist=get_symm_ops(rec)
-        self.assertEqual(len(Mlist),3)
+        self.assertEqual(len(Mlist),1)
+        self.assertTrue(np.array_equal(Tlist[0],np.array([0.0,0.0,0.0])))
         self.assertTrue(np.array_equal(Mlist[0],np.identity(3)))
-        self.assertTrue(np.array_equal(Mlist[1],
+        self.assertTrue('REMARK.350.BIOMOLECULE1.TRANSFORM2' in self.P.parsed)
+        rec=self.P.parsed['REMARK.350.BIOMOLECULE1.TRANSFORM2']
+        self.assertEqual(rec.header,['G', 'B', 'L', 'H', 'D', 'E', 'A', 'C', 'F', 'I', 'J', 'K', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T'])
+        Mlist,Tlist=get_symm_ops(rec)
+        self.assertEqual(len(Mlist),1)
+        self.assertTrue(np.array_equal(Mlist[0],
                                        np.array(
                                         [
                                             [-0.500000,-0.866025,0.000000],
                                             [ 0.866025,-0.500000,0.000000],
                                             [ 0.00000,  0.000000,1.000000]
                                         ])))
-        self.assertTrue(np.array_equal(Tlist[1],np.array([-515.56,0.0,0.0])))
+        self.assertTrue(np.array_equal(Tlist[0],np.array([-515.56,0.0,0.0])))
 
     def test_remark_375(self):
         self.assertTrue('REMARK.375' in self.P.parsed)
         rec=self.P.parsed['REMARK.375']
         self.assertTrue(hasattr(rec,'tables'))
         tables=rec.tables
         self.assertTrue('SPECIAL_POSITIONS' in tables)
```

### Comparing `pidibble-1.0.7.2/tests/unit/test_rcsb/4tvp.pdb` & `pidibble-1.0.7.3/tests/unit/test_rcsb/4tvp.pdb`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/tests/unit/test_rcsb/4zmj.pdb` & `pidibble-1.0.7.3/tests/unit/test_rcsb/4zmj.pdb`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/tests/unit/test_rcsb/test.pdb` & `pidibble-1.0.7.3/tests/unit/test_rcsb/test.pdb`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/tests/unit/test_rcsb/test_pdb_format.yaml` & `pidibble-1.0.7.3/tests/unit/test_rcsb/test_pdb_format.yaml`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/.gitignore` & `pidibble-1.0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/LICENSE` & `pidibble-1.0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pidibble-1.0.7.2/README.md` & `pidibble-1.0.7.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,16 @@
  [ 0.        0.        1.      ]]
 [[-0.5       0.866025  0.      ]
  [-0.866025 -0.5       0.      ]
  [ 0.        0.        1.      ]]
 ```
 ## Release History
 
+* 1.0.7.3
+    * improved parsing of BIOMT transforms
 * 1.0.7.2
     * added documentation stub at readthedocs
 * 1.0.7.1
     * support for split BIOMT tables and REMARKS 280, 375, 650, and 700
 * 1.0.7
     * pretty-print enabled
 * 1.0
```

### Comparing `pidibble-1.0.7.2/pyproject.toml` & `pidibble-1.0.7.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "pidibble"
-version = "1.0.7.2"
+version = "1.0.7.3"
 authors = [
   { name="Cameron F Abrams", email="cfa22@drexel.edu" },
 ]
 description = "A complete Protein Data Bank (PDB) file parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pidibble-1.0.7.2/PKG-INFO` & `pidibble-1.0.7.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidibble
-Version: 1.0.7.2
+Version: 1.0.7.3
 Summary: A complete Protein Data Bank (PDB) file parser
 Project-URL: Source, https://github.com/cameronabrams/pidibble
 Project-URL: Documentation, https://pidibble.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/cameronabrams/pidibble/issues
 Author-email: Cameron F Abrams <cfa22@drexel.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -82,14 +82,16 @@
  [ 0.        0.        1.      ]]
 [[-0.5       0.866025  0.      ]
  [-0.866025 -0.5       0.      ]
  [ 0.        0.        1.      ]]
 ```
 ## Release History
 
+* 1.0.7.3
+    * improved parsing of BIOMT transforms
 * 1.0.7.2
     * added documentation stub at readthedocs
 * 1.0.7.1
     * support for split BIOMT tables and REMARKS 280, 375, 650, and 700
 * 1.0.7
     * pretty-print enabled
 * 1.0
```

