# Comparing `tmp/tortoise-api-0.2.5.tar.gz` & `tmp/tortoise-api-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise-api-0.2.5.tar", last modified: Tue Aug  1 10:47:31 2023, max compression
+gzip compressed data, was "tortoise-api-0.2.6.tar", last modified: Thu Aug  3 18:01:24 2023, max compression
```

## Comparing `tortoise-api-0.2.5.tar` & `tortoise-api-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-01 10:47:31.836737 tortoise-api-0.2.5/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.5/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-08-01 10:47:31.836489 tortoise-api-0.2.5/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.5/README.md
--rw-r--r--   0 sol        (501) staff       (20)      686 2023-08-01 10:47:00.000000 tortoise-api-0.2.5/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-08-01 10:47:31.836801 tortoise-api-0.2.5/setup.cfg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-01 10:47:31.832932 tortoise-api-0.2.5/tortoise_api/
--rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.5/tortoise_api/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     3540 2023-07-31 13:36:53.000000 tortoise-api-0.2.5/tortoise_api/api.py
--rw-r--r--   0 sol        (501) staff       (20)     3069 2023-07-31 11:44:47.000000 tortoise-api-0.2.5/tortoise_api/util.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-01 10:47:31.836185 tortoise-api-0.2.5/tortoise_api.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-08-01 10:47:31.000000 tortoise-api-0.2.5/tortoise_api.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      277 2023-08-01 10:47:31.000000 tortoise-api-0.2.5/tortoise_api.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-08-01 10:47:31.000000 tortoise-api-0.2.5/tortoise_api.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       66 2023-08-01 10:47:31.000000 tortoise-api-0.2.5/tortoise_api.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-08-01 10:47:31.000000 tortoise-api-0.2.5/tortoise_api.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 18:01:24.387108 tortoise-api-0.2.6/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.6/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-08-03 18:01:24.386894 tortoise-api-0.2.6/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.6/README.md
+-rw-r--r--   0 sol        (501) staff       (20)      686 2023-08-03 17:58:57.000000 tortoise-api-0.2.6/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-08-03 18:01:24.387161 tortoise-api-0.2.6/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 18:01:24.384736 tortoise-api-0.2.6/tortoise_api/
+-rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.6/tortoise_api/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     3373 2023-08-03 06:25:29.000000 tortoise-api-0.2.6/tortoise_api/api.py
+-rw-r--r--   0 sol        (501) staff       (20)     2691 2023-08-03 06:26:18.000000 tortoise-api-0.2.6/tortoise_api/util.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 18:01:24.386512 tortoise-api-0.2.6/tortoise_api.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-08-03 18:01:24.000000 tortoise-api-0.2.6/tortoise_api.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      277 2023-08-03 18:01:24.000000 tortoise-api-0.2.6/tortoise_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-08-03 18:01:24.000000 tortoise-api-0.2.6/tortoise_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       66 2023-08-03 18:01:24.000000 tortoise-api-0.2.6/tortoise_api.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-08-03 18:01:24.000000 tortoise-api-0.2.6/tortoise_api.egg-info/top_level.txt
```

### Comparing `tortoise-api-0.2.5/LICENSE` & `tortoise-api-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.5/PKG-INFO` & `tortoise-api-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.5
+Version: 0.2.6
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `tortoise-api-0.2.5/README.md` & `tortoise-api-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.5/pyproject.toml` & `tortoise-api-0.2.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 description = "Simplest fastest minimal REST API CRUD generator for Tortoise ORM models"
 readme = "README.md"
 license = {text = "MIT"}
 dependencies = [
     "asyncpg",
     "python-dotenv",
     "starlette",
-    "tortoise-api-model>=0.1.0",
+    "tortoise-api-model>=0.2.2",
     "uvicorn"
 ]
-version = "0.2.5"
+version = "0.2.6"
 
 [project.urls]
 Homepage = "https://github.com/mixartemev/tortoise-api"
 Repository = "https://github.com/mixartemev/tortoise-api"
 
 [tool.setuptools]
 packages = ["tortoise_api"]
```

### Comparing `tortoise-api-0.2.5/tortoise_api/api.py` & `tortoise-api-0.2.6/tortoise_api/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 from dotenv import load_dotenv
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response, RedirectResponse
 from starlette.routing import Route
 from starlette.templating import Jinja2Templates
 from tortoise.contrib.starlette import register_tortoise
-from tortoise.fields import ManyToManyRelation
 from tortoise_api_model import Model
 
-from tortoise_api.util import jsonify, update, delete, parse_qs
+from tortoise_api.util import jsonify, delete, parse_qs
 
 
 class Api:
     app: Starlette
     models: {str: Model}
 
     def __init__(
@@ -33,15 +32,15 @@
             Route('/favicon.ico', lambda req: Response(), methods=['GET']),  # avoid chrome auto favicon load
             Route('/{model}', self.all_create, methods=['GET', 'POST']),
             Route('/', self.api_menu, methods=['GET']),
         ]
         self.debug = debug
 
     def start(self, models_module):
-        self.models = {key: model for key in dir(models_module) if isinstance(model := getattr(models_module, key), type(Model)) and model.mro()[1]==Model}
+        self.models: {str: type[Model]} = {key: model for key in dir(models_module) if isinstance(model := getattr(models_module, key), type(Model)) and model.mro()[1]==Model}
         if self.debug:
             logging.basicConfig(level=logging.DEBUG)
         self.app = Starlette(debug=self.debug, routes=self.routes)
         load_dotenv()
         register_tortoise(self.app, db_url=env("DB_URL"), modules={"models": [models_module]}, generate_schemas=self.debug)
         return self.app
 
@@ -49,31 +48,28 @@
     async def api_menu(self, _: Request):
         return JSONResponse(list(self.models))
 
     async def all_create(self, request: Request):
         model: type[Model] = self._get_model(request)
         if request.method == 'POST':
             data = parse_qs(await request.body())
-            m2ms = {k: data.pop(k) for k in model._meta.m2m_fields if k in data}
-            obj: Model = await model.create(**data)
-            for k, ids in m2ms.items():
-                m2m_rel: ManyToManyRelation = getattr(obj, k)
-                items = [await m2m_rel.remote_model[i] for i in ids]
-                await m2m_rel.add(*items)
+            obj: Model = await model.upsert(data)
             return RedirectResponse('/'+model.__name__, 303) # create # {True: 201, False: 202}[res[1]]
         objects: [Model] = await model.all().prefetch_related(*model._meta.fetch_fields)
         data = [jsonify(obj) for obj in objects]
         return JSONResponse({'data': data}) # show all
 
     async def one_update(self, request: Request):
         model: type[Model] = self._get_model(request)
         oid = request.path_params['oid']
         if request.method == 'POST':
-            res = await update(model, await request.json(), oid)
-            return JSONResponse(jsonify(res[0]), status_code=202) # update
+            data = parse_qs(await request.body())
+            res = await model.upsert({model._meta.pk_attr: oid, **data})
+            # return JSONResponse(jsonify(res[0]), status_code=202) # update
+            return RedirectResponse('/'+model.__name__, 303) # create # {True: 201, False: 202}[res[1]]
         elif request.method == 'DELETE':
             res = await delete(model, oid)
             return JSONResponse(jsonify(res[0]), status_code=202) # update
         obj = await model.get(id=oid).prefetch_related(*model._meta.fetch_fields)
         return JSONResponse(jsonify(obj)) # show one
```

### Comparing `tortoise-api-0.2.5/tortoise_api/util.py` & `tortoise-api-0.2.6/tortoise_api/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from tortoise.fields.relational import RelationalField, ReverseRelation
 from tortoise_api_model import Model
 
 
 def jsonify(obj: Model) -> dict:
     def check(field: Field, key: str):
         def rel_pack(mod: Model) -> dict:
-            return {'id': mod.id, 'type': mod.__class__.__name__, 'repr': mod.repr()}
+            return {mod._meta.pk_attr: mod.pk, 'type': mod.__class__.__name__, 'repr': mod.repr()}
 
         prop = getattr(obj, key)
         if isinstance(prop, date):
             return prop.__str__().split('+')[0].split('.')[0] # '+' separates tz part, '.' separates millisecond part
         if isinstance(prop, Polygon):
             return prop.points
         if isinstance(prop, Range):
@@ -59,22 +59,12 @@
         #     else:
         #         data[k].append((v,))
 
         else: # if v is IntEnum - it requires explicit convert to int
             data[k] = int(v) if v.isnumeric() else v
     return data
 
-# async def upsert(model: type[Model], dct: dict):
-#     meta: MetaInfo = model._meta
-#     if pk := meta.pk_attr in dct.keys():
-#         unq = {pk: dct.pop(pk)}
-#     else:
-#         unq = {key: dct.pop(key) for key, ft in meta.fields_map.items() if ft.unique and key in dct.keys()}
-#     # unq = meta.unique_together
-#     res = await model.update_or_create(dct, **unq)
-#     return res
-
 async def update(model: type[Model], dct: dict, oid):
     return await model.update_or_create(dct, **{model._meta.pk_attr: oid})
 
 async def delete(model: type[Model], oid):
     return await (await model[oid]).delete()
```

### Comparing `tortoise-api-0.2.5/tortoise_api.egg-info/PKG-INFO` & `tortoise-api-0.2.6/tortoise_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.5
+Version: 0.2.6
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

