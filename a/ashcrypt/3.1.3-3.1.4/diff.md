# Comparing `tmp/ashcrypt-3.1.3.tar.gz` & `tmp/ashcrypt-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ashcrypt-3.1.3.tar", last modified: Wed Aug  2 22:46:57 2023, max compression
+gzip compressed data, was "dist/ashcrypt-3.1.4.tar", last modified: Thu Aug  3 07:55:51 2023, max compression
```

## Comparing `ashcrypt-3.1.3.tar` & `ashcrypt-3.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39564 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/exceptions/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt/utils/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/gui/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/gui/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/gui/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39564 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/exceptions/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt/utils/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/gui/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/gui/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/gui/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 07:55:50.000000 ashcrypt-3.1.4/ashcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-03 07:55:50.000000 ashcrypt-3.1.4/ashcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:55:50.000000 ashcrypt-3.1.4/ashcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 07:55:50.000000 ashcrypt-3.1.4/ashcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 07:55:50.000000 ashcrypt-3.1.4/ashcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/setup.py
```

### Comparing `ashcrypt-3.1.3/PKG-INFO` & `ashcrypt-3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.3
+Version: 3.1.4
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.3/README.md` & `ashcrypt-3.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,17 @@
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
 mainkey = Enc.genkey()
 ```
 2) Before encrypting or decrypting anything, first set the arguments you want to pass, you can have an encrypted message or a  decrypted message , and a mainkey to use.
-<br>This will output a string type key (hex) you can change that to render bytes:
+<br>This will output a string type key (hex), you can choose to render your preferred key length:
 ```python
-mainkey = Enc.genkey(raw_bytes=True)
+mainkey = Enc.genkey(desired_bytes=64) # 512-bit long key
 ```
 ```python
 mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
 ```
 The message can be of type string or bytes.
 <br>Normal string message :  
 ```python 
@@ -211,15 +211,15 @@
 ```
 ```python
 my_instance.decrypt()
 ```
 
 That's it, if you follow the steps above then everything should work just fine.
 ## `textcrypt` ## 
-Follow the same steps above the naming is just differs, and keep in mind both accept either strings or bytes 
+Follow the same steps above, and keep in mind both accept either string type objects or bytes 
 ```python
 my_instance = Crypt('Hello Wold !',key)
 ```
 ```python
 my_instance.encrypt()[1]
 ```
 ```python
@@ -236,58 +236,58 @@
 **Note** that in `database.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
 Run:
 ```python
 pip install dataclasses
 ```
 
 ### Usage ## 
-In this module I'm providing built-in functions to make it easier to perform usual queries on Sqlite tables , by default it creates a table `Classified` with two default columns :
+In this module I'm providing built-in functions to make it easier to perform usual queries over Sqlite tables , by default it creates a table `Classified` with two default columns :
 
 **content** : This can be a single character or a whole movie in binary, that depends on your specific needs.
 
 **key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key.
 1) Create a connection to the database :
 ```python
 conn = Database('test.db')
 ```
-This would automatically set the default table name to `Classifed` if no arguments are passed to the other class functions then they would all be working on the default table name , if you want to set your default table name instead of `Classified` you can pass your table name as the second argument : 
+This would automatically set the default table name to `Classifed`, if no arguments are passed then all class methods would be using the default table name , if you want to set your own default table name instead of `Classified` you can pass your table name as the second argument : 
 ```python
 conn = Database('test.db','mytable')
 ```
 2) create/add the table to the database :
 ```python
 conn.addtable()
 ```
-Added the default table that's been set to the database,  if you want to pass an argument to the function that would create another table of your choice
+Add the default table that's been set to the database,  if you want to pass an argument to the function that would create another table of your choice
 
 3) Set a reference to the key not the key itself : 
 ```python
  key = '#5482A'
 ```
 4) Use the connection to perform various tasks <br>
 The content can be anything post encryption bytes or string format
 ```python
 content='Some Encrypted Content'
 conn.insert(content=content,key='#1E89JO', optional_table_name=None)
 ```
-If the optional table name is `None` then it will insert into the default table , else it would insert into the table you specify
+If the optional table name is `None` then it will insert data into the default table , else it would insert data into the table you specify
 
 
 5) You can check the tables you have , it returns a generator object, yields the result of each element so you must run a for loop over it
 ```python
 for e in conn.show_tables():
         print(e)
 ```
 You can check the current size of the database using the size property method 
 ```python
 print(conn.size) # Size of the Database in MB 
 ```
 
 6) Check the module itself so you can run through all the available methods.
-<br>The methods available perform the usual operations like insertion, deletion , updating the database and more..
+<br>The available methods can perform usual operations like insertion, deletion , updating the database and more..
 
 
 7) to run more complex queries I've dedicated a query function that takes in `*queries` and returns the result fetched 
 ```python
 query = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
 print(conn.query(query))
 ```
@@ -303,42 +303,42 @@
 ```python
 [{'query 0': ('FAILURE', 'no such table: DoesntExist')}]
 ```
 That's it so simple !
 
 
 ## GUI ##
-The GUI as mentioned above is a fully functional application , you can use it to encrypt files , text , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
+The GUI as mentioned above is a fully functional application , you can use it to enc/dec files , text , keep track of files by storing them on demand in the main database , also on demand it can keep track of the keys used for cryptographic operations.
 ### Usage ###
 1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. Then insert it in the `MAINKEY` entry
 2) Now you're able to encrypt files or text (text is limited to 200 characters max)
 ####  Text : 
 - You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
 - Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
 <br>If the text cannot be decrypted it will display itself , so you might as well use this to display the key you're using as a qr code 
 
 #### Files
-- Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
+- Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` button to encrypt the given file , if the encryption turns out to be successful , you'll see a success message along with a `added .crypt extention to the file` message. If the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
 - The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extension you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
 #### Database
 - Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by :
 1) Specifying the actual path where you want your database to be 
 2) Give it a name, it must be a valid file name that ends with `.db` .<br>
 If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically connect.
-3) Did I mention the keys' database ? well if you give a database file name it will also create the keys database with the same name as the database you chose plus `Keys` added to the name. This database holds the actual keys and the reference to these keys.
+3) Did I mention the keys' database ? well if you give a database a file name it will also create the keys database with the same name as the database you chose plus `Keys` added to the name. This database holds the actual keys and the reference to these keys.
 <br>The only piece of data that these two separate databases have in common is the key reference values.  
 
    
 **Info**: 
 <br>Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
-`Name` that holds the filename in both databases , although for the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
-<br>`Content` in the main db, that holds the entire content of the given file whereas for the keys db that holds the actual 256 bit encryption key.
-<br>`Key` in  both db's that holds the `KeyRef` or key reference value
+`Name` that holds the filename in both databases , although for the keys database if you haven't specified any file to operate on while selecting different keys, then all these inserted keys will be tagged `STANDALONE` 
+<br>`Content` for the main db, this holds the entire content of the given file whereas for the keys db that holds the actual 256 bit encryption key.
+<br>`Key` for  both db's, this holds the `KeyRef` A.K.A key reference value
 #### Usage 
-The buttons are self-explanatory so do what you see fit. the result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
+The buttons are self-explanatory so do what you see fit. The result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
 <br>Just click buttons and check the result in the output console, it will guide you through the process.
 
 <br>To run the GUI anywhere
 ```shell
 python -m ashcrypt.gui
 ```
```

### Comparing `ashcrypt-3.1.3/ashcrypt/clicrypt.py` & `ashcrypt-3.1.4/ashcrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.3/ashcrypt/crypt.py` & `ashcrypt-3.1.4/ashcrypt/crypt.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,24 +40,22 @@
         return bcrypt.kdf(
             password=mainkey.encode('UTF-8'),
             salt=salt_pepper,
             desired_key_bytes=32,
             rounds=iterations)
 
     @staticmethod
-    def genkey(raw_bytes: Optional[bool] = False,
-               desired_bytes: Optional[int] = 32) -> Union[str, bytes]:
+    def genkey(desired_bytes: Optional[int] = 32) -> Union[str, bytes]:
         """Generates a random 256-bit ( by default )
-        key as either raw bytes or a hex string. Set raw_bytes to True to get
-        the key in bytes. Set the number of desired_bytes to a greater or equal to 32
+        key as a hex string. Set the number of desired_bytes to a greater or equal to 32
         to override the default value"""
         if desired_bytes < 32:
             raise ValueError("desired_bytes must be greater or equal to 32")
         key = os.urandom(desired_bytes)
-        return key if raw_bytes else key.hex()
+        return key.hex()
 
     def _mode(self):
         """Returns AES Cipher Block Chaining (CBC) mode with the chosen initialization vector"""
         return modes.CBC(self._iv)
 
     def _cipher(self):
         """Creates AES cipher object using the encryption key and CBC mode"""
```

### Comparing `ashcrypt-3.1.3/ashcrypt/database.py` & `ashcrypt-3.1.4/ashcrypt/database.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.3/ashcrypt/filecrypt.py` & `ashcrypt-3.1.4/ashcrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.3/ashcrypt/gui.py` & `ashcrypt-3.1.4/ashcrypt/gui.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.3/ashcrypt/textcrypt.py` & `ashcrypt-3.1.4/ashcrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.3/ashcrypt/unittests/unittest_crypt.py` & `ashcrypt-3.1.4/ashcrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.3/ashcrypt/utils/exceptions/main.py` & `ashcrypt-3.1.4/ashcrypt/utils/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.3/ashcrypt/utils/gui/file.py` & `ashcrypt-3.1.4/ashcrypt/utils/gui/file.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.3/ashcrypt/utils/gui/text.py` & `ashcrypt-3.1.4/ashcrypt/utils/gui/text.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.3/ashcrypt.egg-info/PKG-INFO` & `ashcrypt-3.1.4/ashcrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.3
+Version: 3.1.4
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.3/ashcrypt.egg-info/SOURCES.txt` & `ashcrypt-3.1.4/ashcrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.3/setup.py` & `ashcrypt-3.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('ashcrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='ashcrypt',
-    version='3.1.3',
+    version='3.1.4',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

