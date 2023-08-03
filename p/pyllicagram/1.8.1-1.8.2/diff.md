# Comparing `tmp/pyllicagram-1.8.1.tar.gz` & `tmp/pyllicagram-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyllicagram-1.8.1.tar", last modified: Thu Apr 27 10:54:44 2023, max compression
+gzip compressed data, was "pyllicagram-1.8.2.tar", last modified: Thu Aug  3 10:53:57 2023, max compression
```

## Comparing `pyllicagram-1.8.1.tar` & `pyllicagram-1.8.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-27 10:54:44.047212 pyllicagram-1.8.1/
--rw-r--r--   0 benoit2c   (501) staff       (20)      276 2023-04-27 10:54:44.044973 pyllicagram-1.8.1/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)     5361 2023-04-19 08:35:16.000000 pyllicagram-1.8.1/README.md
--rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-04-27 10:54:44.048403 pyllicagram-1.8.1/setup.cfg
--rw-r--r--   0 benoit2c   (501) staff       (20)      413 2023-04-27 10:54:29.000000 pyllicagram-1.8.1/setup.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-27 10:54:44.022748 pyllicagram-1.8.1/src/
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-27 10:54:44.028258 pyllicagram-1.8.1/src/pyllicagram/
--rw-r--r--   0 benoit2c   (501) staff       (20)     3853 2023-04-27 10:53:28.000000 pyllicagram-1.8.1/src/pyllicagram/__init__.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-27 10:54:44.043840 pyllicagram-1.8.1/src/pyllicagram.egg-info/
--rw-r--r--   0 benoit2c   (501) staff       (20)      276 2023-04-27 10:54:43.000000 pyllicagram-1.8.1/src/pyllicagram.egg-info/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)      240 2023-04-27 10:54:43.000000 pyllicagram-1.8.1/src/pyllicagram.egg-info/SOURCES.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-04-27 10:54:43.000000 pyllicagram-1.8.1/src/pyllicagram.egg-info/dependency_links.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-04-27 10:54:43.000000 pyllicagram-1.8.1/src/pyllicagram.egg-info/requires.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-04-27 10:54:43.000000 pyllicagram-1.8.1/src/pyllicagram.egg-info/top_level.txt
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-03 10:53:57.873826 pyllicagram-1.8.2/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      265 2023-08-03 10:53:57.873722 pyllicagram-1.8.2/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)     5361 2023-06-08 10:33:06.000000 pyllicagram-1.8.2/README.md
+-rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-08-03 10:53:57.873861 pyllicagram-1.8.2/setup.cfg
+-rw-r--r--   0 benoit2c   (501) staff       (20)      413 2023-08-03 10:52:51.000000 pyllicagram-1.8.2/setup.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-03 10:53:57.872349 pyllicagram-1.8.2/src/
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-03 10:53:57.872871 pyllicagram-1.8.2/src/pyllicagram/
+-rw-r--r--   0 benoit2c   (501) staff       (20)     6083 2023-08-03 10:49:16.000000 pyllicagram-1.8.2/src/pyllicagram/__init__.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-03 10:53:57.873581 pyllicagram-1.8.2/src/pyllicagram.egg-info/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      265 2023-08-03 10:53:57.000000 pyllicagram-1.8.2/src/pyllicagram.egg-info/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)      240 2023-08-03 10:53:57.000000 pyllicagram-1.8.2/src/pyllicagram.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-08-03 10:53:57.000000 pyllicagram-1.8.2/src/pyllicagram.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-08-03 10:53:57.000000 pyllicagram-1.8.2/src/pyllicagram.egg-info/requires.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-08-03 10:53:57.000000 pyllicagram-1.8.2/src/pyllicagram.egg-info/top_level.txt
```

### Comparing `pyllicagram-1.8.1/README.md` & `pyllicagram-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pyllicagram-1.8.1/src/pyllicagram/__init__.py` & `pyllicagram-1.8.2/src/pyllicagram/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # ------------------------
 # API CALL
 def pyllicagram(recherche,corpus="presse",debut=1789,fin=1950,resolution="default",somme=False):
         if not isinstance(recherche, str) and not isinstance(recherche, list):
             raise ValueError("La recherche doit être une chaîne de caractères ou une liste")
         if not isinstance(recherche, list): recherche = [recherche]
-        assert corpus in ["lemonde","livres","presse"], 'Vous devez choisir le corpus parmi "lemonde","livres" et "presse"'
+        assert corpus in ["lemonde","livres","presse","huma","paris"], 'Vous devez choisir le corpus parmi "lemonde","livres" et "presse"'
         assert resolution in ["default","annee","mois"], 'Vous devez choisir la résolution parmi "default", "annee" ou "mois"'
         result = []
         for gram in tqdm(recherche):
                 gram = urllib.parse.quote_plus(gram.lower()).replace("-"," ").replace("+"," ")
                 gram = gram.replace(" ","%20")
                 df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/query?corpus={corpus}&mot={gram}&from={debut}&to={fin}&resolution={resolution:}")
                 #if resolution=="mois" and corpus != "livres":
@@ -46,27 +46,71 @@
                 #        result = df
                 result.append(df)
         result = pd.concat(result)
         if somme:
                 result = result.groupby(["annee",*(("mois",) if "mois" in result.columns else()),*(("jour",) if 'jour' in result.columns else())]).agg({'n':'sum','total':'mean'}).reset_index()
                 result["gram"] = "+".join(recherche)
         result["ratio"] = result.n.values/result.total.values
+        if 'jour' in result.columns:
+            jour = result.jour.astype("str")
+        else:
+            jour = "01"
+        if 'mois' in result.columns:
+            mois = result.mois.astype("str")
+        else:
+            mois = "01"
+
+        result["date"] = result.annee.astype("str") + "-" + mois + "-" + jour
+        result.date = pd.to_datetime(result.date)
         return result
 
 
-def joker(gram,corpus="presse",debut=1789,fin=1950,after=True,n_joker=20):
+def joker(gram,corpus="presse",debut=1789,fin=1950,after=True,n_joker=20,length=None):
     if not isinstance(gram, str) and not isinstance(gram, list):
             raise ValueError("La recherche doit être une chaîne de caractères ou une liste")
     assert corpus in ["lemonde","livres","presse"], 'Vous devez choisir le corpus parmi "lemonde","livres" et "presse"'
     gram = urllib.parse.quote_plus(gram.lower()).replace("-"," ").replace(" ","%20")
-    df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/joker?corpus={corpus}&mot={gram}&from={debut}&to={fin}&after={after}&n_joker={n_joker}")
+    url=f"https://shiny.ens-paris-saclay.fr/guni/joker?corpus={corpus}&mot={gram}&from={debut}&to={fin}&after={after}"
+    if length is not None: url=url+f"length={length}"
+    df = pd.read_csv(url)
     return df 
 
 
-def contain(mot1,mot2,corpus="presse",debut=1789,fin=1950):
+def contain(mot1,mot2,corpus="presse",debut=1789,fin=1950,count=True):
     if not isinstance(mot1,str) or not isinstance(mot2,str):
-        raise ValueError("La recherche doit être une chaîne de caractères ou une liste")
+        raise ValueError("La recherche doit être une chaîne de caractères")
     assert corpus in ["lemonde","livres","presse"], 'Vous devez choisir le corpus parmi "lemonde","livres" et "presse"'
     mot1 = urllib.parse.quote_plus(mot1.lower()).replace("-"," ").replace(" ","%20")
     mot2 = urllib.parse.quote_plus(mot2.lower()).replace("-"," ").replace(" ","%20")
-    df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/contain?corpus={corpus}&mot1={mot1}&mot2={mot2}&from={debut}&to={fin}")
+    df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/contain?corpus={corpus}&mot1={mot1}&mot2={mot2}&from={debut}&to={fin}&count={count}")
+    return df
+
+def cooccur_doc(mot1,mot2,debut=1945,fin=2022,resolution="mois"):
+    if not isinstance(mot1,str) or not isinstance(mot2,str):
+        raise ValueError("La recherche doit être une chaîne de caractères")
+    assert resolution in ["annee","mois"], 'Vous devez choisir la résolution parmi "annee" et "mois"'
+    mot1 = urllib.parse.quote_plus(mot1.lower()).replace("-"," ").replace(" ","%20")
+    mot2 = urllib.parse.quote_plus(mot2.lower()).replace("-"," ").replace(" ","%20")
+    df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/cooccur?mot1={mot1}&mot2={mot2}&from={debut}&to={fin}&resolution={resolution}")
+    return df
+
+def associated_article(mot,debut=1945,fin=2022,n_joker=100,stopwords=0):
+    #if not isinstance(mot):
+    #    raise ValueError("La recherche doit être une chaîne de caractères")
+    mot = urllib.parse.quote_plus(mot.lower()).replace("-"," ").replace(" ","%20")
+    url=f"https://shiny.ens-paris-saclay.fr/guni/associated_article?mot={mot}&from={debut}&to={fin}&n_joker={n_joker}&stopwords={stopwords}"
+    df = pd.read_csv(url)
+    return df
+
+
+
+
+def associated(gram,corpus="presse",debut=1789,fin=1950,n_joker=20,length=None,stopwords=0):
+    if not isinstance(gram, str) and not isinstance(gram, list):
+            raise ValueError("La recherche doit être une chaîne de caractères ou une liste")
+    assert corpus in ["lemonde","livres","presse"], 'Vous devez choisir le corpus parmi "lemonde","livres" et "presse"'
+    gram = urllib.parse.quote_plus(gram.lower()).replace("-"," ").replace(" ","%20")
+    url=f"https://shiny.ens-paris-saclay.fr/guni/associated?corpus={corpus}&mot={gram}&from={debut}&to={fin}&stopwords={stopwords}"
+    if length is not None: url=url+f"&length={length}"
+    df = pd.read_csv(url)
     return df
+
```

