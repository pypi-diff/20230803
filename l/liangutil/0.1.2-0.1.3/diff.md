# Comparing `tmp/liangutil-0.1.2.tar.gz` & `tmp/liangutil-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liangutil-0.1.2.tar", last modified: Wed Aug  2 08:34:20 2023, max compression
+gzip compressed data, was "liangutil-0.1.3.tar", last modified: Thu Aug  3 07:01:49 2023, max compression
```

## Comparing `liangutil-0.1.2.tar` & `liangutil-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 08:34:20.669622 liangutil-0.1.2/
--rw-rw-rw-   0        0        0     3495 2023-08-02 08:34:20.669622 liangutil-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2023-08-02 08:22:56.000000 liangutil-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 08:34:20.665558 liangutil-0.1.2/liangutil/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.1.2/liangutil/__init__.py
--rw-rw-rw-   0        0        0     3521 2023-08-02 03:19:39.000000 liangutil-0.1.2/liangutil/lianglog.py
--rw-rw-rw-   0        0        0     4495 2023-08-02 08:16:07.000000 liangutil-0.1.2/liangutil/liangutils.py
--rw-rw-rw-   0        0        0     1318 2023-08-02 03:25:24.000000 liangutil-0.1.2/liangutil/minioutils.py
--rw-rw-rw-   0        0        0     7717 2023-08-02 08:23:39.000000 liangutil-0.1.2/liangutil/mysqlutils.py
--rw-rw-rw-   0        0        0      551 2023-08-02 06:39:07.000000 liangutil-0.1.2/liangutil/redisutils.py
--rw-rw-rw-   0        0        0    13258 2023-08-02 06:56:19.000000 liangutil-0.1.2/liangutil/requestutils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:34:20.667621 liangutil-0.1.2/liangutil.egg-info/
--rw-rw-rw-   0        0        0     3495 2023-08-02 08:34:20.000000 liangutil-0.1.2/liangutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-08-02 08:34:20.000000 liangutil-0.1.2/liangutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 08:34:20.000000 liangutil-0.1.2/liangutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-02 08:34:20.000000 liangutil-0.1.2/liangutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 08:34:20.669622 liangutil-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1095 2023-08-02 06:28:33.000000 liangutil-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:01:49.066432 liangutil-0.1.3/
+-rw-rw-rw-   0        0        0     3624 2023-08-03 07:01:49.066432 liangutil-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1866 2023-08-03 06:30:50.000000 liangutil-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 07:01:49.062370 liangutil-0.1.3/liangutil/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.1.3/liangutil/__init__.py
+-rw-rw-rw-   0        0        0     3511 2023-08-03 06:26:44.000000 liangutil-0.1.3/liangutil/lianglog.py
+-rw-rw-rw-   0        0        0     4495 2023-08-03 06:33:35.000000 liangutil-0.1.3/liangutil/liangutils.py
+-rw-rw-rw-   0        0        0     1318 2023-08-02 03:25:24.000000 liangutil-0.1.3/liangutil/minioutils.py
+-rw-rw-rw-   0        0        0     6640 2023-08-03 06:59:14.000000 liangutil-0.1.3/liangutil/mysqlutils.py
+-rw-rw-rw-   0        0        0      551 2023-08-02 06:39:07.000000 liangutil-0.1.3/liangutil/redisutils.py
+-rw-rw-rw-   0        0        0    13047 2023-08-03 06:25:17.000000 liangutil-0.1.3/liangutil/requestutils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:01:49.065431 liangutil-0.1.3/liangutil.egg-info/
+-rw-rw-rw-   0        0        0     3624 2023-08-03 07:01:49.000000 liangutil-0.1.3/liangutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-08-03 07:01:49.000000 liangutil-0.1.3/liangutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:01:49.000000 liangutil-0.1.3/liangutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-03 07:01:49.000000 liangutil-0.1.3/liangutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:01:49.066432 liangutil-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-08-03 07:01:39.000000 liangutil-0.1.3/setup.py
```

### Comparing `liangutil-0.1.2/PKG-INFO` & `liangutil-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.1.2
+Version: 0.1.3
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
@@ -85,23 +85,28 @@
         
         # 更新日志
         
         ## 2023年
         
         ### 8月
         
+        **2023-08-03**
+        
+        `0.1.3`
+        
+        - 取消了某些函数的捕获异常
+        - 修复了一些Bug
+        
         **2023-08-02** 
         
         `0.1.2`
         
         - 更改了RequestUtils中的get、post方法参数列表名称，更符合使用requests库的习惯
         - MySQLUtils增加了 update_datas() 、query_datas_dict_list()
         
-        
-        
         `0.1.1`
         
         - 统一了代码注释风格
         - 新增代码文档
         - 删除了无用函数
         - 改变了某些函数名称
```

### Comparing `liangutil-0.1.2/README.md` & `liangutil-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -77,23 +77,28 @@
 
 # 更新日志
 
 ## 2023年
 
 ### 8月
 
+**2023-08-03**
+
+`0.1.3`
+
+- 取消了某些函数的捕获异常
+- 修复了一些Bug
+
 **2023-08-02** 
 
 `0.1.2`
 
 - 更改了RequestUtils中的get、post方法参数列表名称，更符合使用requests库的习惯
 - MySQLUtils增加了 update_datas() 、query_datas_dict_list()
 
-
-
 `0.1.1`
 
 - 统一了代码注释风格
 - 新增代码文档
 - 删除了无用函数
 - 改变了某些函数名称
```

### Comparing `liangutil-0.1.2/liangutil/lianglog.py` & `liangutil-0.1.3/liangutil/lianglog.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
         Args:
             level(str): 等级(WARNING, INFO , ERROR)
             content(str): 日志信息
 
         """
         formatted_log = "{} EXCEPTION: {}".format(code_location(depth=-4),content)
-        log = "{} {} {}".format(level,get_nowdatetime(),formatted_log)
+        log = f"{level} {get_nowdatetime()} {formatted_log}"
         print(log)
 
 
 
     def record_log_to_file(self,level, content):
         """将日志记录到文件
```

### Comparing `liangutil-0.1.2/liangutil/liangutils.py` & `liangutil-0.1.3/liangutil/liangutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     """打印日志
 
     Args:
         level: 日志等级
         content: 信息
 
     """
-    formatted_log = "{} EXCEPTION: {}".format(code_location(depth=-2), content)
+    formatted_log = "{} EXCEPTION: {}".format(code_location(depth=-3), content)
     printlog = "{} {} {}".format(level,get_nowdatetime(),formatted_log)
     print(printlog)
 
 
 def code_location(depth=-2):
     """得到调用该方法的文件名称和 代码行号
```

### Comparing `liangutil-0.1.2/liangutil/minioutils.py` & `liangutil-0.1.3/liangutil/minioutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.1.2/liangutil/mysqlutils.py` & `liangutil-0.1.3/liangutil/mysqlutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,185 +20,148 @@
             table_name(str):表名
 
         Returns:
             存在返回True，否则返回False
 
         """
         cursor = self.conn.cursor()
-        try:
-            sql = "show tables like '{}'".format(table_name)
-            cursor.execute(sql)
-            result = cursor.fetchone()
-            if result:
-                return True
-            else:
-                return False
-
-        except Exception as e:
-            print_log("ERROR",e)
-        finally:
+
+        sql = "show tables like '{}'".format(table_name)
+        cursor.execute(sql)
+        result = cursor.fetchone()
+        if result:
+            cursor.close()
+            return True
+        else:
             cursor.close()
+            return False
 
 
     def insert_data(self, table_name, data: dict):
         """插入一条数据
 
         Args:
             table_name(str):表名
             data(dict):要插入的数据，以字段名为键，字段值为值。
 
         Returns:
-            插入成功返回"True"，错误返回异常
+            插入成功返回"True"
 
         """
+        cursor = self.conn.cursor()
+        # 构建 SQL 插入语句
+        columns = ', '.join(data.keys())
+        values = ', '.join(['%s'] * len(data))
+        sql = f"insert into {table_name} ({columns}) values ({values})"
+        cursor.execute(sql, tuple(data.values()))
+        self.conn.commit()
+        cursor.close()
+        return "True"
 
-        try:
-            cursor = self.conn.cursor()
-            # 构建 SQL 插入语句
-            columns = ', '.join(data.keys())
-            values = ', '.join(['%s'] * len(data))
-            sql = f"insert into {table_name} ({columns}) values ({values})"
-
-            cursor.execute(sql, tuple(data.values()))
-
-            self.conn.commit()
-
-            cursor.close()
-            return "True"
-        except Exception as e:
-            return e
 
 
     def insert_datas(self, table_name, data_list: list):
         """插入一条数据
 
         Args:
             table_name(str):表名
             data(list):要插入的数据列表，以字段名为键，字段值为值。
 
         Returns:
-            插入成功返回"True"，错误返回异常
+            插入成功返回"True"
 
         """
 
-        try:
-            cursor = self.conn.cursor()
-            columns = ', '.join(data_list[0].keys())  # 假设所有字典的键相同
-            values_template = ', '.join(['%s'] * len(data_list[0]))
-
-            # 构建 SQL 批量插入语句
-            sql = f"insert into {table_name} ({columns}) values ({values_template})"
-
-            # 构建数据列表的值元组
-            values_tuples = [tuple(d.values()) for d in data_list]
-
-            cursor.executemany(sql, values_tuples)
+        cursor = self.conn.cursor()
+        columns = ', '.join(data_list[0].keys())  # 假设所有字典的键相同
+        values_template = ', '.join(['%s'] * len(data_list[0]))
+        # 构建 SQL 批量插入语句
+        sql = f"insert into {table_name} ({columns}) values ({values_template})"
+        # 构建数据列表的值元组
+        values_tuples = [tuple(d.values()) for d in data_list]
+        cursor.executemany(sql, values_tuples)
+        self.conn.commit()
+        cursor.close()
+        return "True"
 
-            self.conn.commit()
-            cursor.close()
-            return "True"
-        except Exception as e:
-            return e
 
 
     def query_data(self, table_name, columns=[], condition=None):
         """随机查询单条数据
 
         Args:
             table_name(str):表名
             columns(list): 要查询的列名列表，如果为[]，则查询所有列
             condition(str): 查询条件
 
         Returns:
             查询结果
 
         """
-
-        try:
-            cursor = self.conn.cursor()
-
-            if len(columns) == 0:
-                columns_str = "*"
-            else:
-                columns_str = ', '.join(columns)
-
-            sql = f"SELECT {columns_str} FROM {table_name}"
-            if condition:
-                sql += f" WHERE {condition} order by rand() limit 1"
-            cursor.execute(sql)
-            result = cursor.fetchone()[0]
-            cursor.close()
-            return result
-        except Exception as e:
-            print_log("ERROR", e)
-            return None
-        finally:
-            cursor.close()
+        cursor = self.conn.cursor()
+        if len(columns) == 0:
+            columns_str = "*"
+        else:
+            columns_str = ', '.join(columns)
+        sql = f"SELECT {columns_str} FROM {table_name}"
+        if condition:
+            sql += f" WHERE {condition} order by rand() limit 1"
+        cursor.execute(sql)
+        result = cursor.fetchone()
+        cursor.close()
+        return result
 
     def query_datas(self, table_name, columns=None, condition=None):
         """查询数据
 
         Args:
             table_name(str):表名
             columns(list): 要查询的列名列表，如果为[]，则查询所有列
             condition(str): 查询条件
 
         Returns:
             查询结果(元组)，每条记录为一个元组
 
         """
-        try:
-            cursor = self.conn.cursor()
-            if columns is None:
-                columns = []
-
-            columns_str = "*" if len(columns) == 0 else ', '.join(columns)
-            sql = f"SELECT {columns_str} FROM {table_name}"
-            if condition:
-                sql += f" WHERE {condition}"
-            cursor.execute(sql)
-            result = cursor.fetchall()
-            cursor.close()
-            return result
-        except Exception as e:
-            print_log("ERROR",e)
-            return None
-        finally:
-            cursor.close()
+        cursor = self.conn.cursor()
+        if columns is None:
+            columns = []
+        columns_str = "*" if len(columns) == 0 else ', '.join(columns)
+        sql = f"SELECT {columns_str} FROM {table_name}"
+        if condition:
+            sql += f" WHERE {condition}"
+        cursor.execute(sql)
+        result = cursor.fetchall()
+        cursor.close()
+        return result
 
     def query_datas_dict_list(self, table_name, columns=None, condition=None):
         """查询数据
 
         Args:
             table_name(str):表名
             columns(list): 要查询的列名列表，如果为[]，则查询所有列
             condition(str): 查询条件
 
         Returns:
-            查询结果: [{},{},{}]
+            查询结果 [{},{},{}]
 
         """
-        try:
-            cursor = self.conn.cursor()
-            if columns is None:
-                columns = []
-
-            columns_str = "*" if len(columns) == 0 else ', '.join(columns)
-            sql = f"SELECT {columns_str} FROM {table_name}"
-            if condition:
-                sql += f" WHERE {condition}"
-            cursor.execute(sql)
-            result = self.fetchall_to_dict_list(cursor)
-            cursor.close()
-            return result
-        except Exception as e:
-            print_log("ERROR",e)
-            return None
-        finally:
-            cursor.close()
+        cursor = self.conn.cursor()
+        if columns is None:
+            columns = []
+        columns_str = "*" if len(columns) == 0 else ', '.join(columns)
+        sql = f"SELECT {columns_str} FROM {table_name}"
+        if condition:
+            sql += f" WHERE {condition}"
+        cursor.execute(sql)
+        result = self.fetchall_to_dict_list(cursor)
+        cursor.close()
+        return result
+
 
     def exists_data(self, table_name, columns=None, condition=None):
         """是否存在该数据
 
         Args:
             table_name(str):表名
             columns(list): 要查询的列名列表，如果为[]，则查询所有列
@@ -207,50 +170,43 @@
         Returns:
             存在True，否则False
 
         """
         if columns is None:
             columns = []
         if condition is None:
-            print_log("WARNING", "You didn't pass in a condition parameter, so it's pointless")
+            print("WARNING", " You didn't pass in a condition parameter, so it's pointless")
         datas = self.query_data(table_name, columns, condition)
         if datas != None:
             return len(datas) > 0
-
+        return False
 
     def update_datas(self, table_name, data, condition=None):
         """更新数据
 
         Args:
             table_name(str): 表名
             data(dict): 要更新的数据，以字段名为键，字段值为值。
             condition(str): 更新条件
 
         Returns:
             更新成功返回 "True"，失败返回异常
         """
-        try:
-            cursor = self.conn.cursor()
-
-            # 构建 SQL 更新语句
-            set_columns = ', '.join([f"{column} = %s" for column in data.keys()])
-            sql = f"UPDATE {table_name} SET {set_columns}"
-
-            if condition:
-                sql += f" WHERE {condition}"
-
-            # 执行 SQL 更新
-            cursor.execute(sql, tuple(data.values()))
-
-            # 提交事务
-            self.conn.commit()
-            cursor.close()
-            return "True"
-        except Exception as e:
-            return e
+        cursor = self.conn.cursor()
+        # 构建 SQL 更新语句
+        set_columns = ', '.join([f"{column} = %s" for column in data.keys()])
+        sql = f"UPDATE {table_name} SET {set_columns}"
+        if condition:
+            sql += f" WHERE {condition}"
+        # 执行 SQL 更新
+        cursor.execute(sql, tuple(data.values()))
+        # 提交事务
+        self.conn.commit()
+        cursor.close()
+        return "True"
 
     def fetchall_to_dict_list(self, cursor):
         """将pymysql的fetchall查询结果转换为装有dict类型的列表
 
         Args:
             cursor: pymysql游标对象
```

### Comparing `liangutil-0.1.2/liangutil/redisutils.py` & `liangutil-0.1.3/liangutil/redisutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.1.2/liangutil/requestutils.py` & `liangutil-0.1.3/liangutil/requestutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -197,60 +197,53 @@
         Args:
             proxy(str): 代理
 
         Returns:
             chrome驱动
 
         """
-        try:
-            chrome_options = Options()
+        chrome_options = Options()
 
-            if proxy != None:
-                chrome_options.add_argument("--proxy-server="+proxy)
-            elif self.proxy != None:
-                chrome_options.add_argument("--proxy-server="+self.proxy)
-
-            chrome_options.add_argument("-window-size=1920,1080") # 设置浏览器窗口的大小为1920x1080像素
-            chrome_options.add_argument('--ignore-certificate-errors') # 忽略证书错误
-            chrome_options.add_argument('--disable-gpu') # 禁用 GPU 硬件加速
-            # chrome_options.add_argument('--incognito') #无痕模式 浏览器不会记录任何浏览历史或者cookie。
-
-            # 禁止使用 /dev/shm。在某些系统中，Chrome 使用 /dev/shm 临时文件系统来共享数据，
-            # 但在 Docker 或某些特定配置的系统中，这个文件系统可能会不够用，导致 Chrome 崩溃。
-            # 这个选项可以让 Chrome 使用其它方式来共享数据，避免崩溃。
-            chrome_options.add_argument('--disable-dev-shm-usage')
-            chrome_options.add_argument('--hide-scrollbars') # 隐藏滚动条
-            chrome_options.add_argument('--disable-plugins') # 禁用插件
-            # chrome_options.add_argument('blink-settings=imagesEnabled=false') #不加载图片, 提升速度
-            # 禁用沙箱。沙箱是 Chrome 用来隔离网页进程的一种安全机制，但在某些情况下，例如在 Docker 中运行 Chrome，沙箱可能会导致问题。这个选项可以禁用沙箱。
-            chrome_options.add_argument('--no-sandbox')
-
-            if self.is_chrome_headless:
-                chrome_options.add_argument('--headless')
-            if platform.system() == "Linux":
-                chrome_options.add_argument('--headless')
-                # 单进程模式。Chrome 默认会为每个标签页或插件启动一个新的进程，
-                # 但在某些情况下，例如内存有限，可能希望所有的标签页都在一个进程中运行。这个选项可以让 Chrome 在单进程模式下运行。
-                chrome_options.add_argument('--single-process')
-
-            # undetected_chromedriver 是一个第三方库
-            # 它可以规避某些网站对 selenium 的检测，使得你的自动化脚本更不容易被网站识别出来。
-            # if self.is_undetected_chromedriver:
-            #     import undetected_chromedriver as uc  # from session not created: This version of ChromeDriver only supports Chrome version 108
-            #     driver = uc.Chrome(options=chrome_options)
-            # else:
-            #     driver = webdriver.Chrome(options=chrome_options)
-            driver = webdriver.Chrome(options=chrome_options)
-            driver.set_page_load_timeout(self.timeout) # 设置页面加载超时时间
-            driver.set_script_timeout(self.timeout) # 设置脚本执行超时时间。
+        if proxy != None:
+            chrome_options.add_argument("--proxy-server="+proxy)
+        elif self.proxy != None:
+            chrome_options.add_argument("--proxy-server="+self.proxy)
+        chrome_options.add_argument("-window-size=1920,1080") # 设置浏览器窗口的大小为1920x1080像素
+        chrome_options.add_argument('--ignore-certificate-errors') # 忽略证书错误
+        chrome_options.add_argument('--disable-gpu') # 禁用 GPU 硬件加速
+        # chrome_options.add_argument('--incognito') #无痕模式 浏览器不会记录任何浏览历史或者cookie。
+        # 禁止使用 /dev/shm。在某些系统中，Chrome 使用 /dev/shm 临时文件系统来共享数据，
+        # 但在 Docker 或某些特定配置的系统中，这个文件系统可能会不够用，导致 Chrome 崩溃。
+        # 这个选项可以让 Chrome 使用其它方式来共享数据，避免崩溃。
+        chrome_options.add_argument('--disable-dev-shm-usage')
+        chrome_options.add_argument('--hide-scrollbars') # 隐藏滚动条
+        chrome_options.add_argument('--disable-plugins') # 禁用插件
+        # chrome_options.add_argument('blink-settings=imagesEnabled=false') #不加载图片, 提升速度
+        # 禁用沙箱。沙箱是 Chrome 用来隔离网页进程的一种安全机制，但在某些情况下，例如在 Docker 中运行 Chrome，沙箱可能会导致问题。这个选项可以禁用沙箱。
+        chrome_options.add_argument('--no-sandbox')
+        if self.is_chrome_headless:
+            chrome_options.add_argument('--headless')
+        if platform.system() == "Linux":
+            chrome_options.add_argument('--headless')
+            # 单进程模式。Chrome 默认会为每个标签页或插件启动一个新的进程，
+            # 但在某些情况下，例如内存有限，可能希望所有的标签页都在一个进程中运行。这个选项可以让 Chrome 在单进程模式下运行。
+            chrome_options.add_argument('--single-process')
+        # undetected_chromedriver 是一个第三方库
+        # 它可以规避某些网站对 selenium 的检测，使得你的自动化脚本更不容易被网站识别出来。
+        # if self.is_undetected_chromedriver:
+        #     import undetected_chromedriver as uc  # from session not created: This version of ChromeDriver only supports Chrome version 108
+        #     driver = uc.Chrome(options=chrome_options)
+        # else:
+        #     driver = webdriver.Chrome(options=chrome_options)
+        driver = webdriver.Chrome(options=chrome_options)
+        driver.set_page_load_timeout(self.timeout) # 设置页面加载超时时间
+        driver.set_script_timeout(self.timeout) # 设置脚本执行超时时间。
+        return driver
 
-            return driver
 
-        except Exception as e:
-            return None
 
 
     def refresh_chrome(self):
         """重启浏览器
 
         Returns:
             重启成功返回True，否则返回False
@@ -265,15 +258,15 @@
                     self.driver.quit()
                 self.driver = self.get_chrome_driver()
                 return True
             except Exception as e:
                 retry_time -= 1
                 error = str(e)
                 time.sleep(time_sleep)
-        print_log("ERROR", error)
+        print("ERROR", str(error))
         return False
 
 
 
     def get_page_source(self, url, time_sleep=0):
         """获得网页源码
 
@@ -308,16 +301,16 @@
                 self.driver.get(url)
             except Exception as e:
                 self.driver.execute("window.stop()")
                 return {"error":e,
                         "content":"",
                         "url":url}
         time.sleep(time_sleep)
-
-        if text := self.driver.page_source:
+        text = self.driver.page_source
+        if text:
             return {"error": "",
                     "content": text,
                     "url": self.driver.current_url}
         else:
             return {"error": "没有获得 page_source",
                     "content": "",
                     "url": self.driver.current_url}
```

### Comparing `liangutil-0.1.2/liangutil.egg-info/PKG-INFO` & `liangutil-0.1.3/liangutil.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.1.2
+Version: 0.1.3
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
@@ -85,23 +85,28 @@
         
         # 更新日志
         
         ## 2023年
         
         ### 8月
         
+        **2023-08-03**
+        
+        `0.1.3`
+        
+        - 取消了某些函数的捕获异常
+        - 修复了一些Bug
+        
         **2023-08-02** 
         
         `0.1.2`
         
         - 更改了RequestUtils中的get、post方法参数列表名称，更符合使用requests库的习惯
         - MySQLUtils增加了 update_datas() 、query_datas_dict_list()
         
-        
-        
         `0.1.1`
         
         - 统一了代码注释风格
         - 新增代码文档
         - 删除了无用函数
         - 改变了某些函数名称
```

### Comparing `liangutil-0.1.2/setup.py` & `liangutil-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         # 属于什么类型
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Natural Language :: Chinese (Simplified)"
     ],
 
-    version='0.1.2',
+    version='0.1.3',
     description='Encapsulate some common tool methods',
     author='LiAng',
     author_email='l2545721422@163.com',
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
```

