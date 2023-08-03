# Comparing `tmp/pygrab-1.1.6.tar.gz` & `tmp/pygrab-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrab-1.1.6.tar", last modified: Wed Jul 19 19:06:58 2023, max compression
+gzip compressed data, was "pygrab-1.2.0.tar", last modified: Thu Aug  3 21:44:16 2023, max compression
```

## Comparing `pygrab-1.1.6.tar` & `pygrab-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 19:06:58.358000 pygrab-1.1.6/
--rw-rw-rw-   0        0        0     2163 2023-07-19 19:06:58.348000 pygrab-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1937 2023-07-12 02:15:21.000000 pygrab-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 19:06:58.265000 pygrab-1.1.6/pygrab/
--rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.1.6/pygrab/__init__.py
--rw-rw-rw-   0        0        0     3164 2023-07-19 19:04:52.000000 pygrab-1.1.6/pygrab/proxylist.py
--rw-rw-rw-   0        0        0    16607 2023-07-19 18:56:41.000000 pygrab-1.1.6/pygrab/pygrab.py
-drwxrwxrwx   0        0        0        0 2023-07-19 19:06:58.337000 pygrab-1.1.6/pygrab.egg-info/
--rw-rw-rw-   0        0        0     2163 2023-07-19 19:06:58.000000 pygrab-1.1.6/pygrab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-19 19:06:58.000000 pygrab-1.1.6/pygrab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 19:06:58.000000 pygrab-1.1.6/pygrab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-19 19:06:58.000000 pygrab-1.1.6/pygrab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-19 19:06:58.000000 pygrab-1.1.6/pygrab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 19:06:58.356000 pygrab-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      616 2023-07-19 19:05:05.000000 pygrab-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:44:16.154000 pygrab-1.2.0/
+-rw-rw-rw-   0        0        0     2163 2023-08-03 21:44:16.145000 pygrab-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1937 2023-07-12 02:15:21.000000 pygrab-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 21:44:16.075000 pygrab-1.2.0/pygrab/
+-rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.2.0/pygrab/__init__.py
+-rw-rw-rw-   0        0        0     3164 2023-07-19 19:04:52.000000 pygrab-1.2.0/pygrab/proxylist.py
+-rw-rw-rw-   0        0        0    20274 2023-08-03 21:42:07.000000 pygrab-1.2.0/pygrab/pygrab.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:44:16.135000 pygrab-1.2.0/pygrab.egg-info/
+-rw-rw-rw-   0        0        0     2163 2023-08-03 21:44:15.000000 pygrab-1.2.0/pygrab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-08-03 21:44:15.000000 pygrab-1.2.0/pygrab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 21:44:15.000000 pygrab-1.2.0/pygrab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-08-03 21:44:15.000000 pygrab-1.2.0/pygrab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 21:44:15.000000 pygrab-1.2.0/pygrab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 21:44:16.152000 pygrab-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      616 2023-08-03 21:41:31.000000 pygrab-1.2.0/setup.py
```

### Comparing `pygrab-1.1.6/PKG-INFO` & `pygrab-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrab
-Version: 1.1.6
+Version: 1.2.0
 Summary: A secure python library for fetching data with async support
 Author: Anish Kanthamneni
 Author-email: akneni@gmail.com
 Description-Content-Type: text/markdown
 
 # PyGrab
```

### Comparing `pygrab-1.1.6/README.md` & `pygrab-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pygrab-1.1.6/pygrab/proxylist.py` & `pygrab-1.2.0/pygrab/proxylist.py`

 * *Files identical despite different names*

### Comparing `pygrab-1.1.6/pygrab/pygrab.py` & `pygrab-1.2.0/pygrab/pygrab.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 Javascript-enabled sites, and local requests.
 
 """
 
 
 from .proxylist import ProxyList
 import requests as _requests
-# from pyppeteer import launch as _launch
+from pyppeteer import launch as _launch
 import asyncio as _asyncio
 import time as _time
+import socket as _socket
+import re as _re
 
 
 def get(url: str, use_proxy=False, retries=5, enable_js=False, *args, **kwargs): 
     """
     Gets the content at the specified URL.
 
     Parameters:
@@ -89,27 +91,28 @@
     raise Exception(f"Invalid url: {url}")
     
 def get_async(urls, use_proxy=False, retries=5, enable_js=False, thread_limit=800, time_rest=0, *args, **kwargs) -> list:
     """
     Gets multiple URLs asynchronously.
 
     This function sends HTTP requests to a list of URLs in separate threads, allowing for concurrent HTTP requests.
-    The function returns a list of responses from the grabbed URLs.
+    The function returns a list of responses from the grabbed URLs. For each request that had a connection error,
+    the list will contain the error object instead of the requests.response object in it's spot.
 
     Args:
         urls (list): A list of URLs to grab.
         use_proxy (bool, optional): If True, uses a proxy for the HTTP requests. Defaults to False.
         retries (int, optional): The number of times to retry the HTTP request in case of failure. Defaults to 5.
         thread_limit (int, optional): The maximum number of threads that will be spawned. 
         time_rest (int, optional): The time in seconds to wait between starting each thread. Defaults to 0.
         *args: Variable length argument list to pass to the get function.
         **kwargs: Arbitrary keyword arguments to pass to the get function.
 
     Returns:
-        list: A list of responses from the grabbed URLs.
+        list: A list of responses (and possibly error objects) from the grabbed URLs.
     
     Raises:
         TypeError: If any of the arguments are not of the desired data type.
     """
     if (isinstance(urls, (str, int, float, bool))):
         raise TypeError("Argument 'urls' must be an iterable object")
     elif not (isinstance(use_proxy, bool)):
@@ -139,15 +142,15 @@
         
         for thread in threads:
             thread.join()
         thread_counter += thread_limit
         
     return result
 
-def get_local(filename:str, local_read_type:str='r', encoding:str='utf-8'):
+def get_local(filename:str, local_read_type:str='r', encoding:str='utf-8') -> str:
     """
     Reads the contens of a file and returns it to the user.
 
     This function reads the contens of a file and returns it to the user.
 
     Parameters:
         filename (str): The file to read from.
@@ -318,14 +321,100 @@
 
 def delete(url, **kwargs):
     return _requests.delete(url, **kwargs)
 
 def options(url, **kwargs):
     return _requests.options(url, **kwargs)
 
+def scan_ip(ip:str, port:int=80, timeout:int=1) -> bool:
+    """
+    Scans a given IP address to check if it's online.
+
+    This function attempts to connect to a specified IP address and port, returning True if the connection is successful
+    and False otherwise.
+
+    Args:
+        ip (str): The IP address to scan, in the format '10.0.0.3'.
+        port (int, optional): The port number to connect to. Defaults to 80.
+        timeout (int, optional): The timeout in seconds for the connection attempt. Defaults to 1.
+
+    Returns:
+        bool: True if the IP address is online, False otherwise.
+
+    Raises:
+        TypeError: If the 'ip' argument is not a string.
+        ValueError: If the 'ip' argument is not in the correct format or if an invalid IP address is provided.
+    """
+    if not isinstance(ip, str):
+        raise TypeError("Argument 'ip' must be a string.")
+
+    pattern = r'^\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}$'
+    if not _re.match(pattern, ip):
+        raise ValueError("Argument 'ip' must be in the format 10.0.0.3")
+
+    try:
+        session = _socket.socket(_socket.AF_INET, _socket.SOCK_STREAM)
+        session.settimeout(timeout)
+        session.connect((ip, port))
+        session.close()
+        return True
+    except (_socket.timeout, ConnectionRefusedError):
+        return False
+    except OSError:
+        raise ValueError("Invalid ip address.")
+
+def scan_iprange(ips:str, port:int=80, timeout:int=1) -> list:
+    """
+    Scans a range of IP addresses to check which ones are online.
+
+    This function scans a specified range of IP addresses, returning a list of those that are online.
+
+    Args:
+        ips (str): The IP address range to scan, in the format '10.0.0.1-255'.
+        port (int, optional): The port number to connect to. Defaults to 80.
+        timeout (int, optional): The timeout in seconds for the connection attempt. Defaults to 1.
+
+    Returns:
+        list: A list of IP addresses that are online within the specified range.
+
+    Raises:
+        TypeError: If the 'ips' argument is not a string.
+        ValueError: If the 'ips' argument is not in the correct format or if the IP range start is greater or equal to 255.
+    """
+    import threading as _threading
+
+    if not isinstance(ips, str):
+        raise TypeError("Argument 'ips' must be a string.")
+
+    ips = ips.replace(' ', '')
+    pattern = r'^\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}-\d{1,3}$'
+    if not _re.match(pattern, ips):
+        raise ValueError("Argument 'ips' must be in the format 10.0.0.1-255")
+
+    first_three = ips.replace(ips.split('.')[-1], '')
+    start, end = ips.split('.')[-1].split('-')
+    ip_range = [first_three + str(i) for i in range (int(start), int(end)+1)]
+
+    if start >= 255:
+        raise ValueError('Ip range must start below 255.')
+
+    threads = []
+    res = {i:False for i in ip_range}
+
+    for i in ip_range:
+        threads.append(
+            _threading.Thread(target=__scan_ip_wrapper, args=[i, port, timeout, res])
+        )
+        threads[-1].start()
+    
+    for i in threads:
+        i.join()
+    
+    return [key for key, value, in res.items() if value]
+
 def set_proxies(proxies:list):
     """Lets the user use their own proxies in the library
 
     Args:
         proxies (list): A list of proxies in the format [['23.144.56.65', '8080'], ...] or ['23.144.56.65:8080', ...]
 
     Raises:
@@ -348,21 +437,29 @@
 
     Returns:
         None
     """
     ProxyList.update_proxies()
 
 def __grab_thread_wrapper(url:str, payload:list, args, kwargs, use_proxy=False, retries=5, enable_js=False):
-    res = get(url, use_proxy=use_proxy, retries=retries, enable_js=enable_js, *args, **kwargs)
-    payload.append(res)
+    try:
+        res = get(url, use_proxy=use_proxy, retries=retries, enable_js=enable_js, *args, **kwargs)
+        payload.append(res)
+    except _requests.exceptions.RequestException as err:
+        payload.append(err)
+
+def __scan_ip_wrapper(ip, port, timeout, res):
+    try:
+        res[ip] = scan_ip(ip=ip, port=port, timeout=timeout)
+    except ValueError:
+        pass
 
 def __grab_enable_js(url):
     return _asyncio.get_event_loop().run_until_complete(__grab_enable_js_async(url))
 
 async def __grab_enable_js_async(url):
-    return ""
-    # browser = await _launch()
-    # page = await browser.newPage()
-    # await page.goto(url, waitUntil='networkidle0')
-    # html = await page.content()    
-    # await browser.close()
-    # return html
+    browser = await _launch()
+    page = await browser.newPage()
+    await page.goto(url, waitUntil='networkidle0')
+    html = await page.content()    
+    await browser.close()
+    return html
```

### Comparing `pygrab-1.1.6/pygrab.egg-info/PKG-INFO` & `pygrab-1.2.0/pygrab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrab
-Version: 1.1.6
+Version: 1.2.0
 Summary: A secure python library for fetching data with async support
 Author: Anish Kanthamneni
 Author-email: akneni@gmail.com
 Description-Content-Type: text/markdown
 
 # PyGrab
```

### Comparing `pygrab-1.1.6/setup.py` & `pygrab-1.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pygrab',
-    version='1.1.6',
+    version='1.2.0',
     description='A secure python library for fetching data with async support',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Anish Kanthamneni',
     author_email='akneni@gmail.com',
     packages=['pygrab'],
     install_requires=[
```

