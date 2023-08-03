# Comparing `tmp/fathomnet-0.6.0.tar.gz` & `tmp/fathomnet-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fathomnet-0.6.0.tar", max compression
+gzip compressed data, was "fathomnet-0.7.0.tar", max compression
```

## Comparing `fathomnet-0.6.0.tar` & `fathomnet-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0     1097 2023-01-24 00:59:25.204254 fathomnet-0.6.0/LICENSE
--rw-r--r--   0        0        0     1857 2023-02-08 00:42:36.864585 fathomnet-0.6.0/README.md
--rw-r--r--   0        0        0       29 2023-01-24 00:59:25.204254 fathomnet-0.6.0/fathomnet/__init__.py
--rw-r--r--   0        0        0     2187 2023-02-08 00:34:38.042852 fathomnet-0.6.0/fathomnet/api/__init__.py
--rw-r--r--   0        0        0     3573 2023-02-08 00:34:38.042852 fathomnet-0.6.0/fathomnet/api/boundingboxes.py
--rw-r--r--   0        0        0      449 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/api/darwincore.py
--rw-r--r--   0        0        0      669 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/api/firebase.py
--rw-r--r--   0        0        0     1661 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/api/geoimages.py
--rw-r--r--   0        0        0     4733 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/api/images.py
--rw-r--r--   0        0        0     2138 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/api/imagesetuploads.py
--rw-r--r--   0        0        0     1255 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/api/regions.py
--rw-r--r--   0        0        0      297 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/api/stats.py
--rw-r--r--   0        0        0     1294 2023-02-08 00:42:39.220573 fathomnet-0.6.0/fathomnet/api/tags.py
--rw-r--r--   0        0        0     1296 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/api/taxa.py
--rw-r--r--   0        0        0     3733 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/api/users.py
--rw-r--r--   0        0        0      722 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/api/xapikey.py
--rw-r--r--   0        0        0    15965 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/models.py
--rw-r--r--   0        0        0        0 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/scripts/__init__.py
--rw-r--r--   0        0        0    20206 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/scripts/fathomnet_generate.py
--rw-r--r--   0        0        0      666 2023-01-24 00:59:25.208254 fathomnet-0.6.0/fathomnet/util.py
--rw-r--r--   0        0        0     1042 2023-02-08 00:34:38.046851 fathomnet-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2989 1970-01-01 00:00:00.000000 fathomnet-0.6.0/setup.py
--rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 fathomnet-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-01-24 00:59:25.204254 fathomnet-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1857 2023-02-22 22:39:33.339568 fathomnet-0.7.0/README.md
+-rw-r--r--   0        0        0       29 2023-01-24 00:59:25.204254 fathomnet-0.7.0/fathomnet/__init__.py
+-rw-r--r--   0        0        0     2143 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/__init__.py
+-rw-r--r--   0        0        0     4387 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/boundingboxes.py
+-rw-r--r--   0        0        0      461 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/darwincore.py
+-rw-r--r--   0        0        0      670 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/firebase.py
+-rw-r--r--   0        0        0     1683 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/geoimages.py
+-rw-r--r--   0        0        0     4710 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/images.py
+-rw-r--r--   0        0        0     2164 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/imagesetuploads.py
+-rw-r--r--   0        0        0     1279 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/regions.py
+-rw-r--r--   0        0        0      309 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/stats.py
+-rw-r--r--   0        0        0     1271 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/tags.py
+-rw-r--r--   0        0        0     1294 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/taxa.py
+-rw-r--r--   0        0        0     4763 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/users.py
+-rw-r--r--   0        0        0      726 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/api/xapikey.py
+-rw-r--r--   0        0        0    16131 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/dto.py
+-rw-r--r--   0        0        0      250 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/models/__init__.py
+-rw-r--r--   0        0        0      798 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/models/bases.py
+-rw-r--r--   0        0        0     1896 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/models/yolov5.py
+-rw-r--r--   0        0        0        0 2023-01-24 00:59:25.208254 fathomnet-0.7.0/fathomnet/scripts/__init__.py
+-rw-r--r--   0        0        0    20203 2023-08-03 19:56:33.812509 fathomnet-0.7.0/fathomnet/scripts/fathomnet_generate.py
+-rw-r--r--   0        0        0      666 2023-01-24 00:59:25.208254 fathomnet-0.7.0/fathomnet/util.py
+-rw-r--r--   0        0        0     1819 2023-08-03 19:56:33.812509 fathomnet-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3494 1970-01-01 00:00:00.000000 fathomnet-0.7.0/setup.py
+-rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 fathomnet-0.7.0/PKG-INFO
```

### Comparing `fathomnet-0.6.0/LICENSE` & `fathomnet-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fathomnet-0.6.0/README.md` & `fathomnet-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `fathomnet-0.6.0/fathomnet/api/__init__.py` & `fathomnet-0.7.0/fathomnet/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # __init__.py (fathomnet-py)
 from typing import Union
 
 import requests
 
-# from ..util import debug_format_response
-
-session = requests.Session()
+SESSION = requests.Session()
 
 
 class EndpointManager:
     ROOT = 'http://fathomnet.org:8080'
     PATH = None
 
     @classmethod
@@ -17,15 +15,15 @@
         if cls.PATH is None:
             raise NotImplementedError
         return '/'.join([cls.ROOT, cls.PATH, endpoint])
 
     @classmethod
     def request(cls, method: str, endpoint: str, parse_json: bool = True, **kwargs) -> Union[requests.Response, dict, list]:
         url = cls.url(endpoint)
-        res = session.request(method, url, **kwargs)
+        res = SESSION.request(method, url, **kwargs)
         if res.ok:  # Status code < 400
             return res.json() if parse_json else res
         elif res.status_code == 401:  # Not authorized, need to authenticate
             raise ValueError('Unauthorized: please authenticate first.')
         elif res.status_code == 403:  # Forbidden, can't access this endpoint with given authentication
             raise ValueError('Forbidden: you cannot access this resource.')
         elif res.status_code < 500:  # User error
```

### Comparing `fathomnet-0.6.0/fathomnet/api/boundingboxes.py` & `fathomnet-0.7.0/fathomnet/api/boundingboxes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,116 @@
 # boundingboxes.py (fathomnet-py)
 from typing import List, BinaryIO, Optional
 
-from .. import models
-from . import EndpointManager
+from fathomnet import dto
+from fathomnet.api import EndpointManager
 
 
 class BoundingBoxes(EndpointManager):
     PATH = 'boundingboxes'
 
 
-def create_with_dto(bounding_box: models.BoundingBoxDTO, auth_header: Optional[models.AuthHeader] = None) -> models.BoundingBoxDTO:
+def create_with_dto(bounding_box: dto.BoundingBoxDTO, auth_header: Optional[dto.AuthHeader] = None) -> dto.BoundingBoxDTO:
     """Create a bounding box."""
     res_json = BoundingBoxes.post('',
                                   json=bounding_box.to_dict(),
                                   auth=auth_header)
-    return models.BoundingBoxDTO.from_dict(res_json)
+    return dto.BoundingBoxDTO.from_dict(res_json)
 
 
-def count_all() -> models.Count:
+def count_all() -> dto.Count:
     """Get a count of all bounding boxes."""
     res_json = BoundingBoxes.get('count')
-    return models.Count.from_dict(res_json)
+    return dto.Count.from_dict(res_json)
 
 
 def find_concepts() -> List[str]:
     """Get a list of all concepts."""
     res_json = BoundingBoxes.get('list/concepts')
     return res_json
 
 
-def count_total_by_concept() -> List[models.ByConceptCount]:
+def count_total_by_concept() -> List[dto.ByConceptCount]:
     """Get a count of bounding boxes for each concept."""
     res_json = BoundingBoxes.get('list/counts')
-    return list(map(models.ByConceptCount.from_dict, res_json))
+    return list(map(dto.ByConceptCount.from_dict, res_json))
 
 
 def find_observers() -> List[str]:
     """Get a list of all observers."""
     res_json = BoundingBoxes.get('list/observers')
     return res_json
 
 
-def count_by_concept(concept: str) -> models.ByConceptCount:
+def count_by_concept(concept: str) -> dto.ByConceptCount:
     """Get a count of bounding boxes for a concept."""
     res_json = BoundingBoxes.get('query/count/{}'.format(concept))
-    return models.ByConceptCount.from_dict(res_json)
+    return dto.ByConceptCount.from_dict(res_json)
 
 
-def find_by_user_defined_key(user_defined_key: str) -> List[models.BoundingBoxDTO]:
+def find_by_user_defined_key(user_defined_key: str) -> List[dto.BoundingBoxDTO]:
     """Get a list of bounding boxes by a user-defined key."""
     res_json = BoundingBoxes.get('query/userdefinedkey/{}'.format(user_defined_key))
-    return list(map(models.BoundingBoxDTO.from_dict, res_json))
+    return list(map(dto.BoundingBoxDTO.from_dict, res_json))
 
 
 def find_all_user_defined_keys() -> List[str]:
     """Get a list of all user-defined keys."""
     res_json = BoundingBoxes.get('query/userdefinedkeys')
     return res_json
 
 
-def upload_csv(csv_fp: BinaryIO, auth_header: Optional[models.AuthHeader] = None) -> models.Message:
+def upload_csv(csv_fp: BinaryIO, auth_header: Optional[dto.AuthHeader] = None) -> dto.Message:
     """Upload a CSV of bounding boxes."""
     res_json = BoundingBoxes.post('upload/csv',
                                   files={'csv': csv_fp},
                                   auth=auth_header)
-    return models.Message.from_dict(res_json)
+    return dto.Message.from_dict(res_json)
 
 
-def find_by_uuid(uuid: str) -> models.BoundingBoxDTO:
+def find_by_uuid(uuid: str) -> dto.BoundingBoxDTO:
     """Get a bounding box by UUID."""
     res_json = BoundingBoxes.get(uuid)
-    return models.BoundingBoxDTO.from_dict(res_json)
+    return dto.BoundingBoxDTO.from_dict(res_json)
 
 
-def update(uuid: str, bounding_box: models.ABoundingBoxDTO, auth_header: Optional[models.AuthHeader] = None) -> models.BoundingBoxDTO:
+def update(uuid: str, bounding_box: dto.ABoundingBoxDTO, auth_header: Optional[dto.AuthHeader] = None) -> dto.BoundingBoxDTO:
     """Update a bounding box."""
     res_json = BoundingBoxes.put(uuid,
                                  json=bounding_box.to_dict(),
                                  auth=auth_header)
-    return models.BoundingBoxDTO.from_dict(res_json)
+    return dto.BoundingBoxDTO.from_dict(res_json)
 
 
-def delete(uuid: str, auth_header: Optional[models.AuthHeader] = None):
+def delete(uuid: str, auth_header: Optional[dto.AuthHeader] = None):
     """Delete a bounding box."""
     BoundingBoxes.delete(uuid, auth=auth_header)
 
 
-def audit_by_uuid(uuid: str) -> List[models.BoundingBoxDTO]:
+def audit_by_uuid(uuid: str) -> List[dto.BoundingBoxDTO]:
     """Get an audit of a bounding box by UUID."""
     res_json = BoundingBoxes.get('audit/uuid/{}'.format(uuid))
-    return list(map(models.BoundingBoxDTO.from_dict, res_json))
+    return list(map(dto.BoundingBoxDTO.from_dict, res_json))
 
 
-def audit_by_user_defined_key(user_defined_key: str) -> List[models.BoundingBoxDTO]:
+def audit_by_user_defined_key(user_defined_key: str) -> List[dto.BoundingBoxDTO]:
     """Get an audit of a bounding box by user-defined key."""
     res_json = BoundingBoxes.get('audit/userdefinedkey/{}'.format(user_defined_key))
-    return list(map(models.BoundingBoxDTO.from_dict, res_json))
+    return list(map(dto.BoundingBoxDTO.from_dict, res_json))
+
+
+def find_searchable_concepts() -> List[str]:
+    """Get a list of searchable concepts."""
+    res_json = BoundingBoxes.get('list/searchable')
+    return res_json
+
+
+def find_by_observer_uuid(uuid: str, pageable: Optional[dto.Pageable] = None) -> List[dto.BoundingBoxDTO]:
+    """Get a list of bounding boxes by observer UUID."""
+    res_json = BoundingBoxes.get('query/observer/{}'.format(uuid), params=pageable.to_params() if pageable else None)
+    return list(map(dto.BoundingBoxDTO.from_dict, res_json['content']))
+
+
+def find_by_verifier_uuid(uuid: str, pageable: Optional[dto.Pageable] = None) -> List[dto.BoundingBoxDTO]:
+    """Get a list of bounding boxes by verifier UUID."""
+    res_json = BoundingBoxes.get('query/verifier/{}'.format(uuid), params=pageable.to_params() if pageable else None)
+    return list(map(dto.BoundingBoxDTO.from_dict, res_json['content']))
```

### Comparing `fathomnet-0.6.0/fathomnet/api/images.py` & `fathomnet-0.7.0/fathomnet/api/images.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,128 +1,128 @@
 # images.py (fathomnet-py)
 from typing import List, Optional
 from urllib.parse import quote_plus
 
-from .. import models
-from . import EndpointManager
+from fathomnet import dto
+from fathomnet.api import EndpointManager
 
 
 class Images(EndpointManager):
     PATH = 'images'
 
 
-def find_all_alt(pageable: models.Pageable) -> List[models.AImageDTO]:
+def find_all_alt(pageable: Optional[dto.Pageable] = None) -> List[dto.AImageDTO]:
     """Get a paged list of all images. (alternative endpoint)"""
     res_json = Images.get('',
-                          params=pageable.to_params())
-    return list(map(models.AImageDTO.from_dict, res_json['content']))
+                          params=pageable.to_params() if pageable else None)
+    return list(map(dto.AImageDTO.from_dict, res_json['content']))
 
 
-def create_if_not_exists(images: List[models.Image], auth_header: Optional[models.AuthHeader] = None) -> List[models.AImageDTO]:
+def create_if_not_exists(images: List[dto.Image], auth_header: Optional[dto.AuthHeader] = None) -> List[dto.AImageDTO]:
     """Create an image if it doesn't exist."""
     res_json = Images.post('',
-                           json=list(map(models.Image.to_dict, images)),
+                           json=list(map(dto.Image.to_dict, images)),
                            auth=auth_header)
-    return list(map(models.Image.from_dict, res_json))
+    return list(map(dto.Image.from_dict, res_json))
 
 
-def count_all() -> models.Count:
+def count_all() -> dto.Count:
     """Get a count of all images."""
     res_json = Images.get('count')
-    return models.Count.from_dict(res_json)
+    return dto.Count.from_dict(res_json)
 
 
-def find_all(pageable: models.Pageable) -> List[models.AImageDTO]:
+def find_all(pageable: Optional[dto.Pageable] = None) -> List[dto.AImageDTO]:
     """Get a paged list of all images."""
     res_json = Images.get('list/all',
-                          params=pageable.to_params())
+                          params=pageable.to_params() if pageable else None)
     # Note: schema inconsistent with response, need to grab the 'content' object
-    return list(map(models.AImageDTO.from_dict, res_json['content']))
+    return list(map(dto.AImageDTO.from_dict, res_json['content']))
 
 
 def find_distinct_submitter() -> List[str]:
     """Get a list of all submitters."""
     res_json = Images.get('list/contributors')
     return res_json
 
 
 def list_imaging_types() -> List[str]:
     """Get a list of all imaging types."""
     res_json = Images.get('list/imagingtypes')
     return res_json
 
 
-def find(geo_image_constraints: models.GeoImageConstraints) -> List[models.AImageDTO]:
+def find(geo_image_constraints: dto.GeoImageConstraints) -> List[dto.AImageDTO]:
     """Get a constrained list of images."""
     res_json = Images.post('query',
                            json=geo_image_constraints.to_dict())
-    return list(map(models.AImageDTO.from_dict, res_json))
+    return list(map(dto.AImageDTO.from_dict, res_json))
 
 
-def find_by_concept(concept: str, taxa: Optional[str] = None) -> List[models.AImageDTO]:
+def find_by_concept(concept: str, taxa: Optional[str] = None) -> List[dto.AImageDTO]:
     """Get a list of images by concept (and optionally taxa provider)."""
     res_json = Images.get('query/concept/{}'.format(concept),
                           params={'taxa': taxa} if taxa else None)
-    return list(map(models.AImageDTO.from_dict, res_json))
+    return list(map(dto.AImageDTO.from_dict, res_json))
 
 
-def find_by_contributors_email(contributors_email: str) -> List[models.AImageDTO]:
+def find_by_contributors_email(contributors_email: str) -> List[dto.AImageDTO]:
     """Get a list of images by contributor."""
     res_json = Images.get('query/contributor/{}'.format(contributors_email))
-    return list(map(models.AImageDTO.from_dict, res_json))
+    return list(map(dto.AImageDTO.from_dict, res_json))
 
 
-def count_by_submitter(contributors_email: str) -> models.ByContributorCount:
+def count_by_submitter(contributors_email: str) -> dto.ByContributorCount:
     """Get a count of images by contributor."""
     res_json = Images.get('query/count/contributor/{}'.format(contributors_email))
-    return models.ByContributorCount.from_dict(res_json)
+    return dto.ByContributorCount.from_dict(res_json)
 
 
-def find_by_observer(observer: str) -> List[models.AImageDTO]:
+def find_by_observer(observer: str) -> List[dto.AImageDTO]:
     """Get a list of images by observer."""
     res_json = Images.get('query/observer/{}'.format(observer))
-    return list(map(models.AImageDTO.from_dict, res_json))
+    return list(map(dto.AImageDTO.from_dict, res_json))
 
 
-def find_by_sha256(sha256: str) -> List[models.AImageDTO]:
+def find_by_sha256(sha256: str) -> List[dto.AImageDTO]:
     """Get a list of images by SHA256 hash."""
     res_json = Images.get('query/sha256/{}'.format(sha256))
-    return list(map(models.AImageDTO.from_dict, res_json))
+    return list(map(dto.AImageDTO.from_dict, res_json))
 
 
-def find_by_tag_key(key: str, value: str) -> List[models.AImageDTO]:
+def find_by_tag_key(key: str, value: str) -> List[dto.AImageDTO]:
     """Get a list of images by a specified tag key-value pair."""
     res_json = Images.get('query/tags',
                           params={'key': key, 'value': value})
-    return list(map(models.AImageDTO.from_dict, res_json))
+    return list(map(dto.AImageDTO.from_dict, res_json))
 
 
-def find_by_url(url: str) -> models.AImageDTO:
+def find_by_url(url: str) -> dto.AImageDTO:
     """Get an image by URL."""
     res_json = Images.get('query/url/{}'.format(quote_plus(url)))
-    return models.AImageDTO.from_dict(res_json)
+    return dto.AImageDTO.from_dict(res_json)
 
 
-def find_by_uuid_in_list(uuids: List[str]) -> List[models.AImageDTO]:
+def find_by_uuid_in_list(uuids: List[str]) -> List[dto.AImageDTO]:
     """Get a list of images corresponding to a specified list of UUIDs."""
     res_json = Images.post('query/uuids',
                            json=uuids)
-    return list(map(models.AImageDTO.from_dict, res_json))
+    return list(map(dto.AImageDTO.from_dict, res_json))
 
 
-def find_by_uuid(uuid: str) -> models.AImageDTO:
+def find_by_uuid(uuid: str) -> dto.AImageDTO:
     """Get an image by UUID."""
     res_json = Images.get(uuid)
-    return models.AImageDTO.from_dict(res_json)
+    return dto.AImageDTO.from_dict(res_json)
 
 
-def update(uuid: str, image: models.AImageDTO, auth_header: Optional[models.AuthHeader] = None) -> models.AImageDTO:
+def update(uuid: str, image: dto.AImageDTO, auth_header: Optional[dto.AuthHeader] = None) -> dto.AImageDTO:
     """Update an image."""
     res_json = Images.put(uuid,
                           json=image.to_dict(),
                           auth=auth_header)
-    return models.AImageDTO.from_dict(res_json)
+    return dto.AImageDTO.from_dict(res_json)
 
 
-def delete(uuid: str, auth_header: Optional[models.AuthHeader] = None):
+def delete(uuid: str, auth_header: Optional[dto.AuthHeader] = None):
     """Delete an image."""
     Images.delete(uuid, auth=auth_header)
```

### Comparing `fathomnet-0.6.0/fathomnet/api/imagesetuploads.py` & `fathomnet-0.7.0/fathomnet/api/imagesetuploads.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 # imagesetuploads.py (fathomnet-py)
-from typing import List
+from typing import List, Optional
 
-from .. import models
-from . import EndpointManager
+from fathomnet import dto
+from fathomnet.api import EndpointManager
 
 
 class ImageSetUploads(EndpointManager):
     PATH = 'imagesetuploads'
 
 
-def count_all() -> models.Count:
+def count_all() -> dto.Count:
     """Count all image set uploads."""
     res_json = ImageSetUploads.get('count')
-    return models.Count.from_dict(res_json)
+    return dto.Count.from_dict(res_json)
 
 
-def find_collections(pageable: models.Pageable) -> List[models.BImageSetUploadDTO]:
+def find_collections(pageable: Optional[dto.Pageable] = None) -> List[dto.BImageSetUploadDTO]:
     """Get a paged list of all image set uploads."""
     res_json = ImageSetUploads.get('list/all',
-                                   params=pageable.to_params())
+                                   params=pageable.to_params() if pageable else None)
     # Note: schema inconsistent with response, need to grab the 'content' object
-    return list(map(models.BImageSetUploadDTO.from_dict, res_json['content']))
+    return list(map(dto.BImageSetUploadDTO.from_dict, res_json['content']))
 
 
 def find_contributors() -> List[str]:
     """Get a list of all contributors."""
     res_json = ImageSetUploads.get('list/contributors')
     return res_json
 
 
 def find_rejection_reasons() -> List[str]:
     """Get a list of all rejection reasons."""
     res_json = ImageSetUploads.get('list/rejectionreasons')
     return res_json
 
 
-def find_by_contributor(contributors_email: str) -> List[models.BImageSetUploadDTO]:
+def find_by_contributor(contributors_email: str) -> List[dto.BImageSetUploadDTO]:
     """Get a list of image set uploads by contributor."""
     res_json = ImageSetUploads.get('query/contributor/{}'.format(contributors_email))
-    return list(map(models.BImageSetUploadDTO.from_dict, res_json))
+    return list(map(dto.BImageSetUploadDTO.from_dict, res_json))
 
 
-def find_by_image_uuid(image_uuid: str) -> List[models.BImageSetUploadDTO]:
+def find_by_image_uuid(image_uuid: str) -> List[dto.BImageSetUploadDTO]:
     """Get an image set upload by UUID."""
     res_json = ImageSetUploads.get('query/image/{}'.format(image_uuid))
-    return list(map(models.BImageSetUploadDTO.from_dict, res_json))
+    return list(map(dto.BImageSetUploadDTO.from_dict, res_json))
 
 
-def stats(image_set_upload_uuid: str) -> models.ImageSetUploadStats:
+def stats(image_set_upload_uuid: str) -> dto.ImageSetUploadStats:
     """Get image set upload statistics for a corresponding image set upload UUID."""
     res_json = ImageSetUploads.get('stats/{}'.format(image_set_upload_uuid))
-    return models.ImageSetUploadStats.from_dict(res_json)
+    return dto.ImageSetUploadStats.from_dict(res_json)
 
 
-def find_by_uuid(uuid: str) -> models.BImageSetUploadDTO:
+def find_by_uuid(uuid: str) -> dto.BImageSetUploadDTO:
     """Get an image set upload by UUID."""
     res_json = ImageSetUploads.get(uuid)
-    return models.BImageSetUploadDTO.from_dict(res_json)
+    return dto.BImageSetUploadDTO.from_dict(res_json)
```

### Comparing `fathomnet-0.6.0/fathomnet/api/regions.py` & `fathomnet-0.7.0/fathomnet/api/regions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # regions.py (fathomnet-py)
 from typing import List, Optional
 
-from .. import models
-from . import EndpointManager
+from fathomnet import dto
+from fathomnet.api import EndpointManager
 
 
 class Regions(EndpointManager):
     PATH = 'regions'
 
 
-def find_all() -> List[models.MarineRegion]:
+def find_all() -> List[dto.MarineRegion]:
     """Get a list of all marine regions."""
     res_json = Regions.get('')
-    return list(map(models.MarineRegion.from_dict, res_json))
+    return list(map(dto.MarineRegion.from_dict, res_json))
 
 
 def count_all() -> int:
     """Get a count of all marine regions."""
     res = Regions.get('count', parse_json=False)
     return int(res.content)
 
 
-def find_all_paged(pageable: models.Pageable) -> List[models.MarineRegion]:
+def find_all_paged(pageable: Optional[dto.Pageable]) -> List[dto.MarineRegion]:
     """Get a paged list of all marine regions."""
-    res_json = Regions.get('list/all', params=pageable.to_params())
-    return list(map(models.MarineRegion.from_dict, res_json['content']))
+    res_json = Regions.get('list/all', params=pageable.to_params() if pageable else None)
+    return list(map(dto.MarineRegion.from_dict, res_json['content']))
 
 
-def sync(auth_header: Optional[models.AuthHeader] = None) -> int:
+def sync(auth_header: Optional[dto.AuthHeader] = None) -> int:
     """Synchronize."""
     res = Regions.get('sync', parse_json=False, auth=auth_header)
     return int(res.content)
 
 
-def find_at(latitude: float, longitude: float) -> List[models.MarineRegion]:
+def find_at(latitude: float, longitude: float) -> List[dto.MarineRegion]:
     """Get the marine regions at the given latitude and longitude."""
     res_json = Regions.get('at', params={'latitude': latitude, 'longitude': longitude})
-    return list(map(models.MarineRegion.from_dict, res_json))
+    return list(map(dto.MarineRegion.from_dict, res_json))
```

### Comparing `fathomnet-0.6.0/fathomnet/api/tags.py` & `fathomnet-0.7.0/fathomnet/api/tags.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # tags.py (fathomnet-py)
 from typing import List, Optional
 
-from .. import models
-from . import EndpointManager
+from fathomnet import dto
+from fathomnet.api import EndpointManager
 
 
 class Tags(EndpointManager):
     PATH = 'tags'
 
 
-def create_with_dto(tag: models.TagDTO, auth_header: Optional[models.AuthHeader] = None) -> models.TagDTO:
+def create_with_dto(tag: dto.TagDTO, auth_header: Optional[dto.AuthHeader] = None) -> dto.TagDTO:
     """Create a tag."""
     res_json = Tags.post('',
                          json=tag.to_dict(),
                          auth=auth_header)
-    return models.TagDTO.from_dict(res_json)
+    return dto.TagDTO.from_dict(res_json)
 
 
-def find_by_uuid(uuid: str) -> models.TagDTO:
+def find_by_uuid(uuid: str) -> dto.TagDTO:
     """Get a tag by UUID."""
     res_json = Tags.get(uuid)
-    return models.TagDTO.from_dict(res_json)
+    return dto.TagDTO.from_dict(res_json)
 
 
-def find_by_image_uuid_and_key(image_uuid: str, key: str) -> List[models.TagDTO]:
+def find_by_image_uuid_and_key(image_uuid: str, key: str) -> List[dto.TagDTO]:
     """Get a tag by image UUID and key."""
     res_json = Tags.get('query/bykey/{}/{}'.format(image_uuid, key))
-    return list(map(models.TagDTO.from_dict, res_json))
+    return list(map(dto.TagDTO.from_dict, res_json))
 
 
-def update(uuid: str, tag: models.TagDTO, auth_header: Optional[models.AuthHeader] = None) -> models.TagDTO:
+def update(uuid: str, tag: dto.TagDTO, auth_header: Optional[dto.AuthHeader] = None) -> dto.TagDTO:
     """Update a tag."""
     res_json = Tags.put(uuid,
                         json=tag.to_dict(),
                         auth=auth_header)
-    return models.TagDTO.from_dict(res_json)
+    return dto.TagDTO.from_dict(res_json)
 
 
-def delete(uuid: str, auth_header: Optional[models.AuthHeader] = None):
+def delete(uuid: str, auth_header: Optional[dto.AuthHeader] = None):
     """Delete a tag."""
     Tags.delete(uuid, auth=auth_header)
```

### Comparing `fathomnet-0.6.0/fathomnet/api/taxa.py` & `fathomnet-0.7.0/fathomnet/api/taxa.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # taxa.py (fathomnet-py)
 from typing import List
 
-from .. import models
-from . import EndpointManager
+from fathomnet import dto
+from fathomnet.api import EndpointManager
 
 
 class Taxa(EndpointManager):
     PATH = 'taxa'
 
 
 def index() -> str:
@@ -17,23 +17,23 @@
 
 def list_taxa_providers() -> List[str]:
     """Get a list of all taxa providers."""
     res_json = Taxa.get('list/providers')
     return res_json
 
 
-def find_children(provider_name: str, concept: str) -> List[models.Taxa]:
+def find_children(provider_name: str, concept: str) -> List[dto.Taxa]:
     """Find the taxonomic children for a concept according to a taxa provider."""
     res_json = Taxa.get('query/children/{}/{}'.format(provider_name, concept))
-    return list(map(models.Taxa.from_dict, res_json))
+    return list(map(dto.Taxa.from_dict, res_json))
 
 
-def find_parent(provider_name: str, concept: str) -> models.Taxa:
+def find_parent(provider_name: str, concept: str) -> dto.Taxa:
     """Find the taxonomic parent for a concept according to a taxa provider."""
     res_json = Taxa.get('query/parent/{}/{}'.format(provider_name, concept))
-    return models.Taxa.from_dict(res_json)
+    return dto.Taxa.from_dict(res_json)
 
 
-def find_taxa(provider_name: str, concept: str) -> List[models.Taxa]:
+def find_taxa(provider_name: str, concept: str) -> List[dto.Taxa]:
     """Get a list of all taxonomic descendants of a concept (including the concept itself) according to a taxa provider."""
     res_json = Taxa.get('query/{}/{}'.format(provider_name, concept))
-    return list(map(models.Taxa.from_dict, res_json))
+    return list(map(dto.Taxa.from_dict, res_json))
```

### Comparing `fathomnet-0.6.0/fathomnet/api/xapikey.py` & `fathomnet-0.7.0/fathomnet/api/xapikey.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # xapikey.py (fathomnet-py)
 from typing import Optional
 
-from .. import models
-from . import EndpointManager, session
+from fathomnet import dto
+from fathomnet.api import EndpointManager, SESSION
 
 
 class XApiKey(EndpointManager):
     PATH = 'xapikey'
 
 
-def auth(x_api_key_token: str) -> models.AuthHeader:
+def auth(x_api_key_token: str) -> dto.AuthHeader:
     """Exchange an X-API-key token for a JWT."""
     res_json = XApiKey.post('auth', headers={'X-API-Key': x_api_key_token})  # TODO figure out request body
-    auth_header = models.AuthHeader.from_dict(res_json)
-    session.auth = auth_header  # Update session auth
+    auth_header = dto.AuthHeader.from_dict(res_json)
+    SESSION.auth = auth_header  # Update session auth
     return auth_header
 
 
-def index(auth_header: Optional[models.AuthHeader] = None):
+def index(auth_header: Optional[dto.AuthHeader] = None):
     """Test a JWT to ensure it's valid."""
     res_json = XApiKey.get('test', auth=auth_header)
-    return models.Message.from_dict(res_json)
+    return dto.Message.from_dict(res_json)
```

### Comparing `fathomnet-0.6.0/fathomnet/models.py` & `fathomnet-0.7.0/fathomnet/dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# models.py (fathomnet-py)
+# dto.py (fathomnet-py)
 from dataclasses import dataclass
 from dataclasses_json import dataclass_json
 from enum import Enum
 from typing import List, Optional
 from requests.auth import AuthBase
 from lxml import etree
 from lxml.builder import E
@@ -324,14 +324,15 @@
     avatarUrl: Optional[str] = None
     createdTimestamp: Optional[str] = None
     lastUpdatedTimestamp: Optional[str] = None
     disabled: Optional[bool] = None
     expertiseRank: Optional[str] = None
     displayName: Optional[str] = None
     roles: Optional[List['Roles']] = None
+    orcid: Optional[str] = None
 
 
 @dataclass_json
 @dataclass
 class GeoImage:
     uuid: Optional[str] = None
     url: Optional[str] = None
@@ -539,7 +540,15 @@
 
 
 @dataclass_json
 @dataclass
 class Taxa:
     name: Optional[str] = None
     rank: Optional[str] = None
+
+
+@dataclass_json
+@dataclass
+class Badge:
+    name: Optional[str] = None
+    since: Optional[str] = None
+    data: Optional[dict] = None
```

### Comparing `fathomnet-0.6.0/fathomnet/scripts/fathomnet_generate.py` & `fathomnet-0.7.0/fathomnet/scripts/fathomnet_generate.py`

 * *Files identical despite different names*

```diff
@@ -16,15 +16,15 @@
 from coco_lib.objectdetection import (
     ObjectDetectionAnnotation,
     ObjectDetectionCategory,
     ObjectDetectionDataset,
 )
 
 from ..api import images, taxa, darwincore
-from ..models import AImageDTO, GeoImageConstraints
+from ..dto import AImageDTO, GeoImageConstraints
 
 
 @dataclass
 class Arguments:
     """Parsed command-line arguments"""
 
     output: str
```

### Comparing `fathomnet-0.6.0/fathomnet/util.py` & `fathomnet-0.7.0/fathomnet/util.py`

 * *Files identical despite different names*

### Comparing `fathomnet-0.6.0/setup.py` & `fathomnet-0.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['fathomnet', 'fathomnet.api', 'fathomnet.scripts']
+['fathomnet', 'fathomnet.api', 'fathomnet.models', 'fathomnet.scripts']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['coco-lib>=0.1.2,<0.2.0',
  'dataclasses-json>=0.5.4,<0.6.0',
  'lxml>=4.6.0,<5.0.0',
  'progressbar2>=3.37.0,<4.0.0',
  'requests>=2.20.0,<3.0.0']
 
+extras_require = \
+{'models': ['appdirs>=1.4.4,<2.0.0',
+            'torch>=2.0.1,<3.0.0',
+            'opencv-python>=4.7.0,<5.0.0',
+            'pandas>=2.0.3,<3.0.0',
+            'pillow>=10.0.0,<11.0.0',
+            'psutil>=5.9.5,<6.0.0',
+            'torchvision>=0.15.2,<0.16.0',
+            'pyyaml>=6.0.1,<7.0.0',
+            'tqdm>=4.65.0,<5.0.0',
+            'ultralytics>=8.0.146,<9.0.0',
+            'gitpython>=3.1.32,<4.0.0']}
+
 entry_points = \
 {'console_scripts': ['fathomnet-generate = '
                      'fathomnet.scripts.fathomnet_generate:main']}
 
 setup_kwargs = {
     'name': 'fathomnet',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'fathomnet-py is a client-side API to help scientists, researchers, and developers interact with FathomNet data.',
     'long_description': "# fathomnet-py\n\n**`fathomnet-py`** is a client-side API to help scientists, researchers, and developers interact with [FathomNet](https://fathomnet.org/) data.\n\n```python\n>>> from fathomnet.api import boundingboxes\n>>> boundingboxes.find_concepts()\n['2G Robotics structured light laser', '55-gallon drum', ...]\n>>> from fathomnet.api import images\n>>> images.find_by_concept('Nanomia')\n[\n    AImageDTO(\n        id=2274942, \n        uuid='cdbfca66-284f-48ac-a36f-7b2ac2b43533', \n        url='https://fathomnet.org/static/m3/framegrabs/MiniROV/images/0056/02_18_37_20.png', \n        ...\n    ),\n    ...\n]\n>>> from fathomnet.api import taxa\n>>> taxa.find_children('mbari', 'Bathochordaeus')\n[\n    Taxa(name='Bathochordaeus stygius', rank='species'), \n    Taxa(name='Bathochordaeus charon', rank='species'), \n    Taxa(name='Bathochordaeus mcnutti', rank='species')\n]\n>>> from fathomnet.api import xapikey\n>>> xapikey.auth('NuCLjlNUlgHchtgDB01Sp1fABJVcWR')  # your API key here\nAuthHeader(\n    type='Bearer', \n    token='eyJhbGciOiJI...'\n)\n```\n\nThe `fathomnet-py` API offers native Python interaction with the FathomNet REST API, abstracting away the underlying HTTP requests.\n\n[![tests](https://github.com/fathomnet/fathomnet-py/actions/workflows/tests.yml/badge.svg)](https://github.com/fathomnet/fathomnet-py/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/fathomnet-py/badge/?version=latest)](https://fathomnet-py.readthedocs.io/en/latest/?badge=latest)\n[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fathomnet/fathomnet-py/blob/main/tutorial.ipynb)\n## Installing `fathomnet-py`\n\n`fathomnet-py` is available on PyPI:\n\n```bash\n$ python -m pip install fathomnet\n```\n\n## API Reference available on [Read the Docs](https://fathomnet-py.readthedocs.io/)\n",
     'author': 'Kevin Barnard',
     'author_email': 'kbarnard@mbari.org',
     'maintainer': 'Kevin Barnard',
     'maintainer_email': 'kbarnard@mbari.org',
     'url': 'https://github.com/fathomnet/fathomnet-py',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `fathomnet-0.6.0/PKG-INFO` & `fathomnet-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 Metadata-Version: 2.1
 Name: fathomnet
-Version: 0.6.0
+Version: 0.7.0
 Summary: fathomnet-py is a client-side API to help scientists, researchers, and developers interact with FathomNet data.
 Home-page: https://github.com/fathomnet/fathomnet-py
 License: MIT
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Maintainer: Kevin Barnard
 Maintainer-email: kbarnard@mbari.org
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: models
+Requires-Dist: appdirs (>=1.4.4,<2.0.0); extra == "models"
 Requires-Dist: coco-lib (>=0.1.2,<0.2.0)
 Requires-Dist: dataclasses-json (>=0.5.4,<0.6.0)
+Requires-Dist: gitpython (>=3.1.32,<4.0.0); extra == "models"
 Requires-Dist: lxml (>=4.6.0,<5.0.0)
+Requires-Dist: opencv-python (>=4.7.0,<5.0.0); extra == "models"
+Requires-Dist: pandas (>=2.0.3,<3.0.0); extra == "models"
+Requires-Dist: pillow (>=10.0.0,<11.0.0); extra == "models"
 Requires-Dist: progressbar2 (>=3.37.0,<4.0.0)
+Requires-Dist: psutil (>=5.9.5,<6.0.0); extra == "models"
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0); extra == "models"
 Requires-Dist: requests (>=2.20.0,<3.0.0)
+Requires-Dist: torch (>=2.0.1,<3.0.0); extra == "models"
+Requires-Dist: torchvision (>=0.15.2,<0.16.0); extra == "models"
+Requires-Dist: tqdm (>=4.65.0,<5.0.0); extra == "models"
+Requires-Dist: ultralytics (>=8.0.146,<9.0.0); extra == "models"
 Project-URL: Bug Tracker, https://github.com/fathomnet/fathomnet-py/issues
 Project-URL: Documentation, https://fathomnet-py.readthedocs.io
 Project-URL: Repository, https://github.com/fathomnet/fathomnet-py
 Description-Content-Type: text/markdown
 
 # fathomnet-py
```

