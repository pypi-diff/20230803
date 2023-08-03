# Comparing `tmp/litellm-0.1.223.tar.gz` & `tmp/litellm-0.1.224.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.223.tar", last modified: Thu Aug  3 15:09:34 2023, max compression
+gzip compressed data, was "litellm-0.1.224.tar", last modified: Thu Aug  3 15:18:39 2023, max compression
```

## Comparing `litellm-0.1.223.tar` & `litellm-0.1.224.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:09:34.431698 litellm-0.1.223/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.223/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:09:34.431554 litellm-0.1.223/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2285 2023-08-03 14:15:52.000000 litellm-0.1.223/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:09:34.430451 litellm-0.1.223/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      969 2023-08-03 02:58:58.000000 litellm-0.1.223/litellm/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11192 2023-08-03 02:58:28.000000 litellm-0.1.223/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.223/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    15044 2023-08-03 13:49:40.000000 litellm-0.1.223/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:09:34.431271 litellm-0.1.223/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:09:34.000000 litellm-0.1.223/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-03 15:09:34.000000 litellm-0.1.223/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 15:09:34.000000 litellm-0.1.223/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 15:09:34.000000 litellm-0.1.223/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 15:09:34.000000 litellm-0.1.223/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.223/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 15:09:34.431753 litellm-0.1.223/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-03 15:09:15.000000 litellm-0.1.223/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:18:39.128319 litellm-0.1.224/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.224/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:18:39.128188 litellm-0.1.224/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2285 2023-08-03 14:15:52.000000 litellm-0.1.224/README.md
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:18:39.127202 litellm-0.1.224/litellm/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      969 2023-08-03 02:58:58.000000 litellm-0.1.224/litellm/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    11192 2023-08-03 02:58:28.000000 litellm-0.1.224/litellm/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.224/litellm/timeout.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    15073 2023-08-03 15:17:43.000000 litellm-0.1.224/litellm/utils.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:18:39.127990 litellm-0.1.224/litellm.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:18:39.000000 litellm-0.1.224/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-03 15:18:39.000000 litellm-0.1.224/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 15:18:39.000000 litellm-0.1.224/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 15:18:39.000000 litellm-0.1.224/litellm.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 15:18:39.000000 litellm-0.1.224/litellm.egg-info/top_level.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.224/pyproject.toml
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 15:18:39.128365 litellm-0.1.224/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-03 15:18:26.000000 litellm-0.1.224/setup.py
```

### Comparing `litellm-0.1.223/LICENSE` & `litellm-0.1.224/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.223/README.md` & `litellm-0.1.224/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.223/litellm/__init__.py` & `litellm-0.1.224/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.223/litellm/main.py` & `litellm-0.1.224/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.223/litellm/timeout.py` & `litellm-0.1.224/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.223/litellm/utils.py` & `litellm-0.1.224/litellm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
           for detail in additional_details: 
             slack_msg += f"{detail}: {additional_details[detail]}\n"
           slack_app.client.chat_postMessage(channel=alerts_channel, text=slack_msg)
         elif callback == "helicone":
           print_verbose("reaches helicone for logging!")
           model = args[0] if len(args) > 0 else kwargs["model"]
           messages = args[1] if len(args) > 1 else kwargs["messages"]
-          heliconeLogger.log_success(model=model, messages=messages, response_obj=result, start_time=start_time, end_time=end_time)
+          heliconeLogger.log_success(model=model, messages=messages, response_obj=result, start_time=start_time, end_time=end_time, print_verbose=print_verbose)
       except:
         pass
 
     if success_handler and callable(success_handler):
       success_handler(args, kwargs)
     pass
   except:
```

