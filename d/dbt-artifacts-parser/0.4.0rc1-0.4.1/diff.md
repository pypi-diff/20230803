# Comparing `tmp/dbt_artifacts_parser-0.4.0rc1.tar.gz` & `tmp/dbt_artifacts_parser-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_artifacts_parser-0.4.0rc1.tar", last modified: Wed Jul  5 08:29:18 2023, max compression
+gzip compressed data, was "dbt_artifacts_parser-0.4.1.tar", last modified: Thu Aug  3 00:05:18 2023, max compression
```

## Comparing `dbt_artifacts_parser-0.4.0rc1.tar` & `dbt_artifacts_parser-0.4.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11357 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/LICENSE
--rw-r--r--   0        0        0     9177 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/README.md
--rw-r--r--   0        0        0      863 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/__init__.py
--rw-r--r--   0        0        0    12057 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parser.py
--rw-r--r--   0        0        0      796 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/__init__.py
--rw-r--r--   0        0        0      977 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/base.py
--rw-r--r--   0        0        0      796 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/catalog/__init__.py
--rw-r--r--   0        0        0     1887 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
--rw-r--r--   0        0        0      796 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/__init__.py
--rw-r--r--   0        0        0    39709 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
--rw-r--r--   0        0        0    45021 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v10.py
--rw-r--r--   0        0        0    40546 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
--rw-r--r--   0        0        0    41294 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
--rw-r--r--   0        0        0    46633 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
--rw-r--r--   0        0        0    47752 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
--rw-r--r--   0        0        0    48520 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
--rw-r--r--   0        0        0    52862 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
--rw-r--r--   0        0        0    35032 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
--rw-r--r--   0        0        0    39343 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v9.py
--rw-r--r--   0        0        0      796 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/run_results/__init__.py
--rw-r--r--   0        0        0     1719 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
--rw-r--r--   0        0        0     1755 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
--rw-r--r--   0        0        0     3346 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
--rw-r--r--   0        0        0     3458 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
--rw-r--r--   0        0        0      796 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/sources/__init__.py
--rw-r--r--   0        0        0     2044 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/sources/sources_v1.py
--rw-r--r--   0        0        0     2327 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/sources/sources_v2.py
--rw-r--r--   0        0        0     2441 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/sources/sources_v3.py
--rw-r--r--   0        0        0     2348 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/utils.py
--rw-r--r--   0        0        0     4455 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/version_map.py
--rw-r--r--   0        0        0     5968 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/catalog/catalog_v1.json
--rw-r--r--   0        0        0   129577 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v1.json
--rw-r--r--   0        0        0   146696 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v10.json
--rw-r--r--   0        0        0   135379 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v2.json
--rw-r--r--   0        0        0   138302 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v3.json
--rw-r--r--   0        0        0   157235 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v4.json
--rw-r--r--   0        0        0   159203 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v5.json
--rw-r--r--   0        0        0   163791 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v6.json
--rw-r--r--   0        0        0   174833 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v7.json
--rw-r--r--   0        0        0   115570 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v8.json
--rw-r--r--   0        0        0   129190 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v9.json
--rw-r--r--   0        0        0     4622 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/run-results/run-results_v1.json
--rw-r--r--   0        0        0     4777 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/run-results/run-results_v2.json
--rw-r--r--   0        0        0     9817 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/run-results/run-results_v3.json
--rw-r--r--   0        0        0    10272 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/run-results/run-results_v4.json
--rw-r--r--   0        0        0     5568 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/sources/sources_v1.json
--rw-r--r--   0        0        0     6790 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/sources/sources_v2.json
--rw-r--r--   0        0        0     7249 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/sources/sources_v3.json
--rw-r--r--   0        0        0     1017 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/utils.py
--rw-r--r--   0        0        0     1773 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0      830 2023-07-05 08:29:18.000000 dbt_artifacts_parser-0.4.0rc1/setup.py
--rw-r--r--   0        0        0    10963 1970-01-01 00:00:00.000000 dbt_artifacts_parser-0.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/LICENSE
+-rw-r--r--   0        0        0     9438 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/README.md
+-rw-r--r--   0        0        0      859 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/__init__.py
+-rw-r--r--   0        0        0    12025 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parser.py
+-rw-r--r--   0        0        0      796 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/__init__.py
+-rw-r--r--   0        0        0      977 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/base.py
+-rw-r--r--   0        0        0      796 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/catalog/__init__.py
+-rw-r--r--   0        0        0     1887 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
+-rw-r--r--   0        0        0      796 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/__init__.py
+-rw-r--r--   0        0        0    39709 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
+-rw-r--r--   0        0        0    45021 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v10.py
+-rw-r--r--   0        0        0    40546 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
+-rw-r--r--   0        0        0    41294 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
+-rw-r--r--   0        0        0    46633 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
+-rw-r--r--   0        0        0    47752 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
+-rw-r--r--   0        0        0    48520 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
+-rw-r--r--   0        0        0    52862 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
+-rw-r--r--   0        0        0    35032 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
+-rw-r--r--   0        0        0    39343 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v9.py
+-rw-r--r--   0        0        0      796 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/run_results/__init__.py
+-rw-r--r--   0        0        0     1719 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
+-rw-r--r--   0        0        0     1755 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
+-rw-r--r--   0        0        0     3346 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
+-rw-r--r--   0        0        0     3458 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
+-rw-r--r--   0        0        0      796 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/sources/__init__.py
+-rw-r--r--   0        0        0     2044 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/sources/sources_v1.py
+-rw-r--r--   0        0        0     2327 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/sources/sources_v2.py
+-rw-r--r--   0        0        0     2441 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/sources/sources_v3.py
+-rw-r--r--   0        0        0     2348 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/utils.py
+-rw-r--r--   0        0        0     4455 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/version_map.py
+-rw-r--r--   0        0        0     5968 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/catalog/catalog_v1.json
+-rw-r--r--   0        0        0   129577 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v1.json
+-rw-r--r--   0        0        0   146696 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v10.json
+-rw-r--r--   0        0        0   135379 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v2.json
+-rw-r--r--   0        0        0   138302 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v3.json
+-rw-r--r--   0        0        0   157235 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v4.json
+-rw-r--r--   0        0        0   159203 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v5.json
+-rw-r--r--   0        0        0   163791 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v6.json
+-rw-r--r--   0        0        0   174833 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v7.json
+-rw-r--r--   0        0        0   115570 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v8.json
+-rw-r--r--   0        0        0   129190 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v9.json
+-rw-r--r--   0        0        0     4622 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/run-results/run-results_v1.json
+-rw-r--r--   0        0        0     4777 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/run-results/run-results_v2.json
+-rw-r--r--   0        0        0     9817 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/run-results/run-results_v3.json
+-rw-r--r--   0        0        0    10272 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/run-results/run-results_v4.json
+-rw-r--r--   0        0        0     5568 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/sources/sources_v1.json
+-rw-r--r--   0        0        0     6790 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/sources/sources_v2.json
+-rw-r--r--   0        0        0     7249 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/sources/sources_v3.json
+-rw-r--r--   0        0        0     1017 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/utils.py
+-rw-r--r--   0        0        0     1773 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-08-03 00:05:18.000000 dbt_artifacts_parser-0.4.1/setup.py
+-rw-r--r--   0        0        0    11221 1970-01-01 00:00:00.000000 dbt_artifacts_parser-0.4.1/PKG-INFO
```

### Comparing `dbt_artifacts_parser-0.4.0rc1/LICENSE` & `dbt_artifacts_parser-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/README.md` & `dbt_artifacts_parser-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -255,10 +255,17 @@
     </td>
     <td align="center">
         <a href="https://github.com/dlawin">
             <img src="https://avatars.githubusercontent.com/u/11282254?v=4" width="100;" alt="dlawin"/>
             <br />
             <sub><b>Null</b></sub>
         </a>
+    </td>
+    <td align="center">
+        <a href="https://github.com/meyer-glean">
+            <img src="https://avatars.githubusercontent.com/u/134302890?v=4" width="100;" alt="meyer-glean"/>
+            <br />
+            <sub><b>Null</b></sub>
+        </a>
     </td></tr>
 </table>
 <!-- readme: contributors -end -->
```

#### html2text {}

```diff
@@ -94,10 +94,11 @@
 parse_sources_v1(sources=sources_dict) # parse sources.json v2 from
 dbt_artifacts_parser.parser import parse_sources_v2 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v2(sources=sources_dict) # parse sources.json v3 from
 dbt_artifacts_parser.parser import parse_sources_v3 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v3(sources=sources_dict) ``` ## Contributors
-[yu-iskw]_   [bbrewington]_  [judahrand]_          [nabilm]_          [dlawin]_
-Yu_Ishikawa Brent_Brewington  Judah_Rand  Mohamed_Nabil_Mahmoud_Hafez   Null
+[yu-iskw]_  [bbrewington]_ [judahrand]_   [nabilm]_   [dlawin]_ [meyer-glean]_
+Yu_Ishikawa     Brent       Judah_Rand  Mohamed_Nabil   Null         Null
+              Brewington                Mahmoud_Hafez
```

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/__init__.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 """
 A dbt artifacts parser in python
 """
-__version__ = "0.4.0-rc1"
+__version__ = "0.4.1"
```

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parser.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     Returns:
         Union[CatalogV1]
     """
     dbt_schema_version = get_dbt_schema_version(artifact_json=catalog)
     if dbt_schema_version == ArtifactTypes.CATALOG_V1.value.dbt_schema_version:
         return CatalogV1(**catalog)
-    raise ValueError("Not a soft of catalog.json")
+    raise ValueError("Not a catalog.json")
 
 
 def parse_catalog_v1(catalog: dict) -> CatalogV1:
     """Parse catalog.json v1"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=catalog)
     if dbt_schema_version == ArtifactTypes.CATALOG_V1.value.dbt_schema_version:
         return CatalogV1(**catalog)
@@ -96,15 +96,15 @@
         return ManifestV7(**manifest)
     elif dbt_schema_version == ArtifactTypes.MANIFEST_V8.value.dbt_schema_version:
         return ManifestV8(**manifest)
     elif dbt_schema_version == ArtifactTypes.MANIFEST_V9.value.dbt_schema_version:
         return ManifestV9(**manifest)
     elif dbt_schema_version == ArtifactTypes.MANIFEST_V10.value.dbt_schema_version:
         return ManifestV10(**manifest)
-    raise ValueError("Not a soft of manifest.json")
+    raise ValueError("Not a manifest.json")
 
 
 def parse_manifest_v1(manifest: dict) -> ManifestV1:
     """Parse manifest.json ver.1"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V1.value.dbt_schema_version:
         return ManifestV1(**manifest)
@@ -201,15 +201,15 @@
         return RunResultsV1(**run_results)
     elif dbt_schema_version == ArtifactTypes.RUN_RESULTS_V2.value.dbt_schema_version:
         return RunResultsV2(**run_results)
     elif dbt_schema_version == ArtifactTypes.RUN_RESULTS_V3.value.dbt_schema_version:
         return RunResultsV3(**run_results)
     elif dbt_schema_version == ArtifactTypes.RUN_RESULTS_V4.value.dbt_schema_version:
         return RunResultsV4(**run_results)
-    raise ValueError("Not a soft of manifest.json")
+    raise ValueError("Not a manifest.json")
 
 
 def parse_run_results_v1(run_results: dict) -> RunResultsV1:
     """Parse run-results.json v1"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=run_results)
     if dbt_schema_version == ArtifactTypes.RUN_RESULTS_V1.value.dbt_schema_version:
         return RunResultsV1(**run_results)
@@ -255,15 +255,15 @@
     dbt_schema_version = get_dbt_schema_version(artifact_json=sources)
     if dbt_schema_version == ArtifactTypes.SOURCES_V1.value.dbt_schema_version:
         return SourcesV1(**sources)
     elif dbt_schema_version == ArtifactTypes.SOURCES_V2.value.dbt_schema_version:
         return SourcesV2(**sources)
     elif dbt_schema_version == ArtifactTypes.SOURCES_V3.value.dbt_schema_version:
         return SourcesV3(**sources)
-    raise ValueError("Not a soft of manifest.json")
+    raise ValueError("Not a manifest.json")
 
 
 def parse_sources_v1(sources: dict) -> SourcesV1:
     """Parse sources.json v1"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=sources)
     if dbt_schema_version == ArtifactTypes.SOURCES_V1.value.dbt_schema_version:
         return SourcesV1(**sources)
```

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/__init__.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/base.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/base.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/catalog/__init__.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/catalog/catalog_v1.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/catalog/catalog_v1.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/__init__.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v1.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v1.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v10.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v10.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v2.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v2.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v3.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v3.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v4.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v4.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v5.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v5.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v6.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v6.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v7.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v7.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v8.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v8.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/manifest/manifest_v9.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/manifest/manifest_v9.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/run_results/__init__.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/run_results/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/run_results/run_results_v1.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/run_results/run_results_v1.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/run_results/run_results_v2.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/run_results/run_results_v2.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/run_results/run_results_v3.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/run_results/run_results_v3.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/run_results/run_results_v4.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/run_results/run_results_v4.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/sources/__init__.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/sources/sources_v1.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/sources/sources_v1.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/sources/sources_v2.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/sources/sources_v2.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/sources/sources_v3.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/sources/sources_v3.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/utils.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/parsers/version_map.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/parsers/version_map.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/catalog/catalog_v1.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/catalog/catalog_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v1.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v10.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v10.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v2.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v2.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v3.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v3.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v4.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v4.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v5.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v5.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v6.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v6.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v7.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v7.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v8.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v8.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/manifest/manifest_v9.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/manifest/manifest_v9.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/run-results/run-results_v1.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/run-results/run-results_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/run-results/run-results_v2.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/run-results/run-results_v2.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/run-results/run-results_v3.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/run-results/run-results_v3.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/run-results/run-results_v4.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/run-results/run-results_v4.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/sources/sources_v1.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/sources/sources_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/sources/sources_v2.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/sources/sources_v2.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/resources/sources/sources_v3.json` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/resources/sources/sources_v3.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/dbt_artifacts_parser/utils.py` & `dbt_artifacts_parser-0.4.1/dbt_artifacts_parser/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/pyproject.toml` & `dbt_artifacts_parser-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/setup.py` & `dbt_artifacts_parser-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.4.0rc1/PKG-INFO` & `dbt_artifacts_parser-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-artifacts-parser
-Version: 0.4.0rc1
+Version: 0.4.1
 Summary: A dbt artifacts parser in python
 Author: yu-iskw
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -296,11 +296,18 @@
     </td>
     <td align="center">
         <a href="https://github.com/dlawin">
             <img src="https://avatars.githubusercontent.com/u/11282254?v=4" width="100;" alt="dlawin"/>
             <br />
             <sub><b>Null</b></sub>
         </a>
+    </td>
+    <td align="center">
+        <a href="https://github.com/meyer-glean">
+            <img src="https://avatars.githubusercontent.com/u/134302890?v=4" width="100;" alt="meyer-glean"/>
+            <br />
+            <sub><b>Null</b></sub>
+        </a>
     </td></tr>
 </table>
 <!-- readme: contributors -end -->
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.4.0rc1 Summary: A
-dbt artifacts parser in python Author: yu-iskw Requires-Python: >=3.7.0
+Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.4.1 Summary: A dbt
+artifacts parser in python Author: yu-iskw Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Topic :: Software Development :: Libraries Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -117,10 +117,11 @@
 parse_sources_v1(sources=sources_dict) # parse sources.json v2 from
 dbt_artifacts_parser.parser import parse_sources_v2 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v2(sources=sources_dict) # parse sources.json v3 from
 dbt_artifacts_parser.parser import parse_sources_v3 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v3(sources=sources_dict) ``` ## Contributors
-[yu-iskw]_   [bbrewington]_  [judahrand]_          [nabilm]_          [dlawin]_
-Yu_Ishikawa Brent_Brewington  Judah_Rand  Mohamed_Nabil_Mahmoud_Hafez   Null
+[yu-iskw]_  [bbrewington]_ [judahrand]_   [nabilm]_   [dlawin]_ [meyer-glean]_
+Yu_Ishikawa     Brent       Judah_Rand  Mohamed_Nabil   Null         Null
+              Brewington                Mahmoud_Hafez
```

