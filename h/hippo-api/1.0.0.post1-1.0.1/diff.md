# Comparing `tmp/hippo_api-1.0.0.post1-py3-none-any.whl.zip` & `tmp/hippo_api-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 26847 bytes, number of entries: 18
--rw-r--r--  2.0 unx       78 b- defN 23-Jul-19 02:37 transwarp_embedding_hub/__init__.py
--rw-r--r--  2.0 unx      790 b- defN 23-Jul-19 02:37 transwarp_embedding_hub/base_embedding.py
--rw-r--r--  2.0 unx      275 b- defN 23-Jul-19 02:37 transwarp_embedding_hub/config.yaml
--rw-r--r--  2.0 unx      623 b- defN 23-Jul-19 02:37 transwarp_embedding_hub/embedding_hub.py
--rw-r--r--  2.0 unx     1629 b- defN 23-Jul-19 02:37 transwarp_embedding_hub/openai.py
--rw-r--r--  2.0 unx     3738 b- defN 23-Jul-19 02:37 transwarp_embedding_hub/pulse.py
--rw-r--r--  2.0 unx     4552 b- defN 23-Jul-19 02:37 transwarp_embedding_hub/text_segmentation.py
--rw-r--r--  2.0 unx       78 b- defN 23-Jun-27 08:41 transwarp_hippo_api/__init__.py
--rw-r--r--  2.0 unx     2597 b- defN 23-Jul-14 03:15 transwarp_hippo_api/conn_mgr.py
--rw-r--r--  2.0 unx    62911 b- defN 23-Jul-19 08:57 transwarp_hippo_api/hippo_client.py
--rw-r--r--  2.0 unx     1298 b- defN 23-Jun-27 08:41 transwarp_hippo_api/hippo_type.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 02:37 transwarp_hippo_langchain/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 23-Jul-19 02:37 transwarp_hippo_langchain/embedding_hub_langchain.py
--rw-r--r--  2.0 unx    20466 b- defN 23-Jul-19 02:37 transwarp_hippo_langchain/hippo_langchain.py
--rw-r--r--  2.0 unx      262 b- defN 23-Jul-20 09:22 hippo_api-1.0.0.post1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 09:22 hippo_api-1.0.0.post1.dist-info/WHEEL
--rw-r--r--  2.0 unx       70 b- defN 23-Jul-20 09:22 hippo_api-1.0.0.post1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1642 b- defN 23-Jul-20 09:22 hippo_api-1.0.0.post1.dist-info/RECORD
-18 files, 102399 bytes uncompressed, 24091 bytes compressed:  76.5%
+Zip file size: 27885 bytes, number of entries: 19
+-rw-r--r--  2.0 unx       78 b- defN 23-Jul-20 09:35 transwarp_embedding_hub/__init__.py
+-rw-r--r--  2.0 unx     2050 b- defN 23-Aug-03 09:41 transwarp_embedding_hub/azure.py
+-rw-r--r--  2.0 unx      790 b- defN 23-Jul-20 09:35 transwarp_embedding_hub/base_embedding.py
+-rw-r--r--  2.0 unx      355 b- defN 23-Aug-03 09:41 transwarp_embedding_hub/config.yaml
+-rw-r--r--  2.0 unx      697 b- defN 23-Aug-03 09:41 transwarp_embedding_hub/embedding_hub.py
+-rw-r--r--  2.0 unx     1629 b- defN 23-Jul-20 09:35 transwarp_embedding_hub/openai.py
+-rw-r--r--  2.0 unx     3738 b- defN 23-Jul-20 09:35 transwarp_embedding_hub/pulse.py
+-rw-r--r--  2.0 unx     4552 b- defN 23-Jul-20 09:35 transwarp_embedding_hub/text_segmentation.py
+-rw-r--r--  2.0 unx       78 b- defN 23-Jul-20 09:35 transwarp_hippo_api/__init__.py
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jul-20 09:35 transwarp_hippo_api/conn_mgr.py
+-rw-r--r--  2.0 unx    63573 b- defN 23-Aug-03 09:41 transwarp_hippo_api/hippo_client.py
+-rw-r--r--  2.0 unx     1298 b- defN 23-Jul-20 09:35 transwarp_hippo_api/hippo_type.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-20 09:35 transwarp_hippo_langchain/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 23-Jul-20 09:35 transwarp_hippo_langchain/embedding_hub_langchain.py
+-rw-r--r--  2.0 unx    20509 b- defN 23-Aug-03 09:41 transwarp_hippo_langchain/hippo_langchain.py
+-rw-r--r--  2.0 unx      256 b- defN 23-Aug-03 10:15 hippo_api-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 10:15 hippo_api-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       70 b- defN 23-Aug-03 10:15 hippo_api-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1707 b- defN 23-Aug-03 10:15 hippo_api-1.0.1.dist-info/RECORD
+19 files, 105367 bytes uncompressed, 25037 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: transwarp_embedding_hub/__init__.py
 Comment: 
 
+Filename: transwarp_embedding_hub/azure.py
+Comment: 
+
 Filename: transwarp_embedding_hub/base_embedding.py
 Comment: 
 
 Filename: transwarp_embedding_hub/config.yaml
 Comment: 
 
 Filename: transwarp_embedding_hub/embedding_hub.py
@@ -36,20 +39,20 @@
 
 Filename: transwarp_hippo_langchain/embedding_hub_langchain.py
 Comment: 
 
 Filename: transwarp_hippo_langchain/hippo_langchain.py
 Comment: 
 
-Filename: hippo_api-1.0.0.post1.dist-info/METADATA
+Filename: hippo_api-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: hippo_api-1.0.0.post1.dist-info/WHEEL
+Filename: hippo_api-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: hippo_api-1.0.0.post1.dist-info/top_level.txt
+Filename: hippo_api-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: hippo_api-1.0.0.post1.dist-info/RECORD
+Filename: hippo_api-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## transwarp_embedding_hub/config.yaml

```diff
@@ -1,9 +1,15 @@
 model:
   openai:
     model_name: 'openai'
     engine: 'text-embedding-ada-002'
-    apikey: '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'
+    apikey: ''
   TranswarpVectorPulse:
     model_name: 'TranswarpVectorPulse'
     url: '172.16.30.3:12350'
-    route_path: '/v2/models/{0}/infer'
+    route_path: '/v2/models/{0}/infer'
+  azure:
+    model_name: 'azure'
+    engine: 'text-embedding-ada-eus'
+    apikey: ''
+    url: ''
+    version: '2023-03-15-preview'
```

## transwarp_embedding_hub/embedding_hub.py

```diff
@@ -1,23 +1,25 @@
 from transwarp_embedding_hub.openai import *
 from transwarp_embedding_hub.pulse import *
+from transwarp_embedding_hub.azure import *
 
 
 class EmbeddingHub:
     """Factory for embedding strategy."""
 
     def __init__(self, model_name):
         self.model_name = model_name
 
     #根据参数 获取embedding策略
     def get_strategy(self):
 
         Strategy = {
             'openai': OpenAI(),
-            'TranswarpVectorPulse': TranswarpVectorPulse()
+            'TranswarpVectorPulse': TranswarpVectorPulse(),
+            'azure': Azure()
         }.get(self.model_name)
 
 
         # 如果没有匹配的类型，则返回 'no match model'
         if not Strategy:
             raise ValueError('no match model')
         else:
```

## transwarp_hippo_api/hippo_client.py

```diff
@@ -104,14 +104,15 @@
 
 ''' 定义HippoTableMeta数据类用于存储表的元数据信息 '''
 
 
 @dataclass
 class HippoTableMeta:
     tbl_name: str  # 表名
+    auto_id: bool  # 是否是主键id
     schema: list[HippoField]  # 表结构，包含多个字段
     n_replicas: int  # 副本数量
     n_shards: int  # 分片数量
     db_name: str  # 数据库名
 
 
 ''' 定义HippoTable类用于管理和操作Hippo表 '''
@@ -140,21 +141,28 @@
                 参数:
                 cols_like: 列数据列表，每个元素是一个列表，表示一列的所有数据。
                 op_type: 操作类型，可以是 "insert"、"update"、"upsert" 或 "delete"。
 
                 返回值:
                 如果操作成功，返回 True。否则，抛出 ValueError 异常。
         """
+
+        if self.tbl_meta.auto_id and op_type == "insert" and len(cols_like) != len(self.schema):
+            schema = self.schema[1:]
+        else:
+            schema = self.schema
+
         assert len(cols_like) == len(
-            self.schema), f"to insert data columns({len(cols_like)}) does not match cols in schema({len(self.schema)})"
+            schema), f"to insert data columns({len(cols_like)}) does not match cols in schema({len(schema)})"
+
         fields_data = []
 
         rows_num = -1
         for idx, col in enumerate(cols_like):
-            col_name = self.schema[idx].name
+            col_name = schema[idx].name
 
             # TODO: 可以插入数据的类型和表里的数据类型
 
             data = cols_like[idx]
             if not isinstance(data, list):
                 raise TypeError(f"to insert data column {idx} is not a list")
             col_len = len(data)
@@ -167,25 +175,32 @@
                 "field": data,
             }
             fields_data.append(this_field_data)
 
         req_data = {
             "fields_data": fields_data,
             "num_rows": rows_num,
+            "op_type": op_type
         }
-        if op_type != "insert":
-            req_data["op_type"] = op_type
 
         js = json.dumps(req_data)
         js = json.loads(js)
         resp = self.hippo_conn.put(f"/{self.tbl_name}/_bulk?database_name={self.tbl_meta.db_name}&pretty", js_data=js)
         if resp.status_code == 200:
-            return True
+            info = json.loads(resp.text)
+            failures = info.get("failures")
+            if failures is not None:
+                raise ValueError(f"{info}")
+            else:
+                return True
         else:
-            raise ValueError(resp.content)
+            error_dict = json.loads(resp.content)
+            reason = error_dict["error"]["reason"]
+            type = error_dict["error"]["type"]
+            raise ValueError(f"error type:{str(type)},reason:{str(reason)}")
 
     # 定义插入行的方法，内部调用_manipulate_rows方法
     def insert_rows(self, cols_like):
 
         """
                 插入行数据。
 
@@ -237,15 +252,15 @@
                 返回值:
                 如果删除成功，返回 True。否则，抛出 ValueError 异常。
         """
         return self._manipulate_rows(cols_like, "delete")
 
     # 批量删除数据。expr 参数用于指定要删除的行的条件。例如，"age > 18"。
     def delete_rows_by_query(self, expr: str = "",
-                            wait_for_competion=True, timeout: str = "2m"):
+                             wait_for_competion=True, timeout: str = "2m"):
 
         """
                 批量删除数据。expr 参数用于指定要删除的行的条件。例如，"age > 18"。
 
                 参数:
                 expr: 删除条件表达式。
                 wait_for_competion: 是否等待删除完成，默认为True。
@@ -260,15 +275,14 @@
             "table_name": self.tbl_name,
             "expr": expr,
             "wait_for_completion": wait_for_competion,
             "timeout": timeout
         }
         js = json.dumps(data)
         js = json.loads(js)
-        print(js)
         resp = self.hippo_conn.post(f"/_delete_by_query?pretty", js_data=js)
         r = HippoConn.handle_json_resp(resp)
         st = r["job_status"]
         if st is not None and st == HippoJobStatus.HIPPO_JOB_SUCCESS.value:
             return st
         else:
             error = r.get("errors")
@@ -357,15 +371,14 @@
         }
 
         js = json.dumps(data)
         js = json.loads(js)
 
         resp = self.hippo_conn.delete(
             f"/{self.tbl_name}/_drop_scalar_index?database_name={self.tbl_meta.db_name}&pretty", js_data=js)
-        print(resp.status_code)
         r = HippoConn.handle_json_resp(resp)
         if r["acknowledged"]:
             return True
         else:
             raise ValueError("cannot create index due to return error.")
 
     # 删除索引。通过索引名称删除对应的索引
@@ -756,19 +769,20 @@
             raise TypeError("host_port should be str or list[str")
         self.hippo_conn = HippoConn(xx, username, pwd)
 
     # 定义了一个方法，用于处理表字典，返回一个HippoTable对象或None
     def _handle_tbl_dict(self, tbl_name: str, dd: dict) -> Optional[HippoTable]:
 
         fields = [_handle_field_schema(x) for x in dd["schema"]["fields"]]
+        auto_id = dd["schema"]["auto_id"]
 
-        print(dd)
         meta = HippoTableMeta(
             tbl_name=tbl_name,
             schema=fields,
+            auto_id=auto_id,
             n_shards=dd["settings"]["number_of_shards"],
             n_replicas=dd["settings"]["number_of_shards"],
             db_name=dd["database_name"]
         )
 
         return HippoTable(self.hippo_conn, meta)
 
@@ -1193,24 +1207,26 @@
             else:
                 raise e
 
     # 指定的数据库中创建新的表
     def create_table(self,
                      name: str,
                      fields: list[HippoField],
+                     auto_id: bool = False,
                      database_name: str = "default",
                      number_of_shards: int = 1,
                      number_of_replicas: int = 1) -> Optional[HippoTable]:
 
         """
             在指定的数据库中创建新的表。
 
             参数:
             name: 表名。
             fields: 一个HippoField对象的列表，每个对象代表一个字段。
+            auto_id: 是否设定自增主键
             database_name: 数据库名，默认为"default"。
             number_of_shards: 分片数，默认为1。
             number_of_replicas: 复制数，默认为1。
 
             返回值:
             如果创建成功，返回一个HippoTable对象。否则，抛出ValueError异常。
         """
@@ -1218,27 +1234,28 @@
 
         data = {
             'settings': {
                 'number_of_shards': number_of_shards,
                 'number_of_replicas': number_of_replicas,
             },
             'schema': {
+                'auto_id': auto_id,
                 'fields': fields_for_req,
             }
         }
 
         js = json.dumps(data, cls=HippoTypesEncoder)
         js = json.loads(js)
 
-        # print("BODY:", js)
+        print("BODY:", js)
 
         resp = self.hippo_conn.put(f"/{name}?database_name={database_name}&pretty", js_data=js)
         r = HippoConn.handle_json_resp(resp)
         if resp.status_code == 200 and r.get("acknowledged") is True:
-            meta = HippoTableMeta(tbl_name=name, schema=fields, n_replicas=number_of_replicas,
+            meta = HippoTableMeta(tbl_name=name, auto_id=auto_id, schema=fields, n_replicas=number_of_replicas,
                                   n_shards=number_of_shards, db_name=database_name)
             return HippoTable(hippo_conn=self.hippo_conn, tbl_meta=meta)
         else:
             raise ValueError(resp.content)
 
     # 重命名指定数据库中的表
     def rename_table(self, old_table_name: str, new_table_name: str, database_name: str = "default"):
@@ -1326,15 +1343,14 @@
                 values = line.split()  # 将行分成值
                 for header, value in zip(headers, values):  # 对于每一对标题和值
                     table_data[header].append(value)  # 将值添加到相应的列表
             return table_data
         else:
             raise ValueError(HippoConn.handle_json_resp(resp))
 
-
     # 此方法用于创建新的用户。你可以通过参数指定用户名、密码，并设置用户是否具有超级用户权限、是否可以创建角色和数据库
     def create_user(self, user_name: str,
                     pwd: str,
                     is_super: bool = False,
                     can_create_role: bool = False,
                     can_create_db: bool = False) -> bool:
 
@@ -1379,15 +1395,15 @@
             参数:
             user_name: 需要删除的用户名。
 
             返回值:
             一个布尔值，表示操作是否成功。
         """
 
-        resp = self.hippo_conn.delete(f"/_security/user/{user_name}?pretty",js_data="")
+        resp = self.hippo_conn.delete(f"/_security/user/{user_name}?pretty", js_data="")
         r = HippoConn.handle_json_resp(resp)
         if r.get("found"):
             return True
         else:
             raise ValueError(r)
 
     # 获取指定用户的信息
@@ -1437,15 +1453,14 @@
             }
         }
         if not change_meta:
             del data["metadata"]
 
         js = json.dumps(data, cls=HippoTypesEncoder)
         js = json.loads(js)
-        print(js)
 
         resp = self.hippo_conn.put(f"/_security/user/{user_name}/_alter?pretty", js_data=js)
         r = HippoConn.handle_json_resp(resp)
         if r.get("acknowledged"):
             return True
         else:
             raise ValueError(r)
```

## transwarp_hippo_langchain/hippo_langchain.py

```diff
@@ -201,21 +201,21 @@
                         "index_type": IndexType.IVF_FLAT,
                         "nlist": 10,
                     }
 
                     # print(self.col.tbl_meta)
                     # print(self.col.schema)
 
-                    print(self.col.create_index(
-                        self._vector_field,
-                        self.index_params['index_name'],
-                        self.index_params['index_type'],
-                        self.index_params['metric_type'],
-                        nlist=self.index_params['nlist'],
-                    ))
+                    # print(self.col.create_index(
+                    #     self._vector_field,
+                    #     self.index_params['index_name'],
+                    #     self.index_params['index_type'],
+                    #     self.index_params['metric_type'],
+                    #     nlist=self.index_params['nlist'],
+                    # ))
                     logger.debug(self.col.activate_index(self.index_params['index_name']))
                     logger.info("create index successfully")
 
     # TODO hippo暂时不需要
 
     # def _create_search_params(self) -> None:
     #     """Generate search params based on the current index type"""
@@ -256,15 +256,15 @@
                 返回值:
                 一个字符串列表，包含已插入文本的唯一标识符。
 
                 注意:
                 如果集合尚未创建，此方法将创建一个新的集合。
         """
 
-        if texts == "":
+        if not texts or all(t == "" for t in texts):
             logger.debug("Nothing to insert, skipping.")
             return []
         texts = list(texts)
 
         logger.debug(f"[add_texts] texts: {texts}")
 
         try:
```

## Comparing `hippo_api-1.0.0.post1.dist-info/RECORD` & `hippo_api-1.0.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 transwarp_embedding_hub/__init__.py,sha256=5HW4WI56IwE4O7nM7iQ7Bx0YceMppe6H5vYKagA3GDI,78
+transwarp_embedding_hub/azure.py,sha256=dxfXZILNBbDbEWWENEsuUxaTE8-D0zizCjwZaIvImRM,2050
 transwarp_embedding_hub/base_embedding.py,sha256=lZ5KYQEbRKn8Mstqti27CyYPYcRaVe3APjKZVjS2fho,790
-transwarp_embedding_hub/config.yaml,sha256=daYYx5WNWz2onzUfpxNEDWIZjA9gqAYoJea3B_ua4ZU,275
-transwarp_embedding_hub/embedding_hub.py,sha256=cg3lwzNZOTfIKz1pAk9IWV6cjElWJf4QuLm2WNrCmu0,623
+transwarp_embedding_hub/config.yaml,sha256=gUZ-_X-_RM2ScrDT-zLd4buwvQYJGzzMWtGkHQMN6cY,355
+transwarp_embedding_hub/embedding_hub.py,sha256=pXeq59x82zzPzFor3rQU5_GFEbOk2krNjrlLcGCRfTo,697
 transwarp_embedding_hub/openai.py,sha256=EAZcjy-uZdlDl4uNuM7Y7Dj2-4BVjKOzDeqI3fn2JsU,1629
 transwarp_embedding_hub/pulse.py,sha256=H3cUWovlOu5suyshg_OG-cy7Q6sF-2cSwON8B0Q5XjA,3738
 transwarp_embedding_hub/text_segmentation.py,sha256=kOjMLdAa_NHqXJl5VHNe1ywmIt1hV3u3bYf5vaH8bEA,4552
 transwarp_hippo_api/__init__.py,sha256=5HW4WI56IwE4O7nM7iQ7Bx0YceMppe6H5vYKagA3GDI,78
 transwarp_hippo_api/conn_mgr.py,sha256=HtugN55_82mXuEcN5akhviEZecTVDvqIYAHXz-oG2xk,2597
-transwarp_hippo_api/hippo_client.py,sha256=8pqC7U9F4bPSl3mTvAvLvK1jXyIAhkmnhm5SZt3RHqY,62911
+transwarp_hippo_api/hippo_client.py,sha256=ZY0hytAarbgKwGVMtz1kFLhQ48jNYcHnwzVYUPpQt4E,63573
 transwarp_hippo_api/hippo_type.py,sha256=aDLaulN_zxkB5A_UZU4sm7SPF3ohhOg961F2Secqvng,1298
 transwarp_hippo_langchain/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 transwarp_hippo_langchain/embedding_hub_langchain.py,sha256=LLXcyMVpTIjNcIfxbX0vrHduZQNIkAWcszllfSFqC7s,1298
-transwarp_hippo_langchain/hippo_langchain.py,sha256=3sPnZgCXSNU9qDsiUlHBVEnWfqxzmJsYIxUY8PaJz48,20466
-hippo_api-1.0.0.post1.dist-info/METADATA,sha256=kNGGiwXsvW9uOkQBmg5-wizYWplpPArArFLBI5vD7VQ,262
-hippo_api-1.0.0.post1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hippo_api-1.0.0.post1.dist-info/top_level.txt,sha256=riej_lCjX8ZdyUgXXOIzUd-X5AeOMg7vk89DjHqpJqc,70
-hippo_api-1.0.0.post1.dist-info/RECORD,,
+transwarp_hippo_langchain/hippo_langchain.py,sha256=Ht5XKLHhpmDcqJrmK8VtGFMQEoZo15-Li9UuSi3WMo4,20509
+hippo_api-1.0.1.dist-info/METADATA,sha256=OpYoPG6Z97kQQ0Gdq-ZIbx3kD9rTpx0uyXUh4V9aKXs,256
+hippo_api-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hippo_api-1.0.1.dist-info/top_level.txt,sha256=riej_lCjX8ZdyUgXXOIzUd-X5AeOMg7vk89DjHqpJqc,70
+hippo_api-1.0.1.dist-info/RECORD,,
```

