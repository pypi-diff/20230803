# Comparing `tmp/d_geolib-1.1.0.tar.gz` & `tmp/d_geolib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d_geolib-1.1.0.tar", max compression
+gzip compressed data, was "d_geolib-1.2.0.tar", max compression
```

## Comparing `d_geolib-1.1.0.tar` & `d_geolib-1.2.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0       97 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/__init__.py
--rw-r--r--   0        0        0      631 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/errors.py
--rw-r--r--   0        0        0       86 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/geometry/__init__.py
--rw-r--r--   0        0        0     1023 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/geometry/one.py
--rw-r--r--   0        0        0      510 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/__init__.py
--rw-r--r--   0        0        0    11570 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/base_model.py
--rw-r--r--   0        0        0      749 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/base_model_structure.py
--rw-r--r--   0        0        0      109 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/__init__.py
--rw-r--r--   0        0        0    12325 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_model.py
--rw-r--r--   0        0        0     1619 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_parserprovider.py
--rw-r--r--   0        0        0     3539 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_structures.py
--rw-r--r--   0        0        0    27768 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/internal.py
--rw-r--r--   0        0        0     3020 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/internal_soil.py
--rw-r--r--   0        0        0    19272 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/piles.py
--rw-r--r--   0        0        0     3958 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/profiles.py
--rw-r--r--   0        0        0      603 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/serializer.py
--rw-r--r--   0        0        0     4350 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv
--rw-r--r--   0        0        0     4337 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv
--rw-r--r--   0        0        0    27924 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dfoundations/templates/input.foi.j2
--rw-r--r--   0        0        0      114 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dgeoflow/__init__.py
--rw-r--r--   0        0        0    16831 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dgeoflow/dgeoflow_model.py
--rw-r--r--   0        0        0     4275 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py
--rw-r--r--   0        0        0      333 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dgeoflow/dgeoflow_validator.py
--rw-r--r--   0        0        0    31320 2023-07-24 14:30:47.406016 d_geolib-1.1.0/geolib/models/dgeoflow/internal.py
--rw-r--r--   0        0        0     3513 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dgeoflow/serializer.py
--rw-r--r--   0        0        0      581 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dgeoflow/utils.py
--rw-r--r--   0        0        0    54527 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dseries_parser.py
--rw-r--r--   0        0        0      106 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/__init__.py
--rw-r--r--   0        0        0      301 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/drain_types.py
--rw-r--r--   0        0        0     5529 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/drains.py
--rw-r--r--   0        0        0    21412 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_model.py
--rw-r--r--   0        0        0     1518 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_parserprovider.py
--rw-r--r--   0        0        0     7147 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_structures.py
--rw-r--r--   0        0        0    34035 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/internal.py
--rw-r--r--   0        0        0     5500 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/internal_soil.py
--rw-r--r--   0        0        0     5960 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/loads.py
--rw-r--r--   0        0        0      233 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/probabilistic_calculation_types.py
--rw-r--r--   0        0        0      559 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/serializer.py
--rw-r--r--   0        0        0    18393 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/templates/input.sli.j2
--rw-r--r--   0        0        0     4965 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsettlement/templates/soil_template.j2
--rw-r--r--   0        0        0      110 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/__init__.py
--rw-r--r--   0        0        0    11250 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/calculation_options.py
--rw-r--r--   0        0        0    21608 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/constructions.py
--rw-r--r--   0        0        0    19431 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_model.py
--rw-r--r--   0        0        0     1528 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py
--rw-r--r--   0        0        0     4647 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_structures.py
--rw-r--r--   0        0        0     3841 2023-07-24 14:30:47.421641 d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_validator.py
--rw-r--r--   0        0        0    53609 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/internal.py
--rw-r--r--   0        0        0    15559 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/internal_partial_factors.py
--rw-r--r--   0        0        0     9894 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/loads.py
--rw-r--r--   0        0        0     1726 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/profiles.py
--rw-r--r--   0        0        0      561 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/serializer.py
--rw-r--r--   0        0        0     5062 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/settings.py
--rw-r--r--   0        0        0     3465 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/supports.py
--rw-r--r--   0        0        0     1700 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/surface.py
--rw-r--r--   0        0        0    35235 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/templates/input.shi.j2
--rw-r--r--   0        0        0      462 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dsheetpiling/water_level.py
--rw-r--r--   0        0        0      118 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/__init__.py
--rw-r--r--   0        0        0    12506 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/analysis.py
--rw-r--r--   0        0        0    36730 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/dstability_model.py
--rw-r--r--   0        0        0     4189 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/dstability_parserprovider.py
--rw-r--r--   0        0        0     2865 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/dstability_validator.py
--rw-r--r--   0        0        0    90867 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/internal.py
--rw-r--r--   0        0        0     2931 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/loads.py
--rw-r--r--   0        0        0     3435 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/reinforcements.py
--rw-r--r--   0        0        0     3525 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/serializer.py
--rw-r--r--   0        0        0     3331 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/states.py
--rw-r--r--   0        0        0      581 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/dstability/utils.py
--rw-r--r--   0        0        0      142 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/internal.py
--rw-r--r--   0        0        0     1781 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/meta.py
--rw-r--r--   0        0        0       89 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/model_enums.py
--rw-r--r--   0        0        0     1821 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/parsers.py
--rw-r--r--   0        0        0      840 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/serializers.py
--rw-r--r--   0        0        0     2433 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/utils.py
--rw-r--r--   0        0        0      314 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/models/validators.py
--rw-r--r--   0        0        0       55 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/service/__init__.py
--rw-r--r--   0        0        0     5849 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/service/main.py
--rw-r--r--   0        0        0      546 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/service/README.md
--rw-r--r--   0        0        0      797 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/soils/__init__.py
--rw-r--r--   0        0        0     1720 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/soils/layers.py
--rw-r--r--   0        0        0      592 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/soils/library.py
--rw-r--r--   0        0        0    37608 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/soils/soil.py
--rw-r--r--   0        0        0      775 2023-07-24 14:30:47.437267 d_geolib-1.1.0/geolib/soils/soil_utils.py
--rw-r--r--   0        0        0     1574 2023-07-24 14:30:47.452890 d_geolib-1.1.0/geolib/utils.py
--rw-r--r--   0        0        0     1086 2023-07-24 14:30:47.374791 d_geolib-1.1.0/LICENSE
--rw-r--r--   0        0        0     2013 2023-07-24 14:30:47.452890 d_geolib-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2955 2023-07-24 14:30:47.374791 d_geolib-1.1.0/README.rst
--rw-r--r--   0        0        0     4037 1970-01-01 00:00:00.000000 d_geolib-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-08-03 11:43:42.632799 d_geolib-1.2.0/geolib/__init__.py
+-rw-r--r--   0        0        0      631 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/errors.py
+-rw-r--r--   0        0        0       86 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/geometry/__init__.py
+-rw-r--r--   0        0        0     1023 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/geometry/one.py
+-rw-r--r--   0        0        0      510 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/__init__.py
+-rw-r--r--   0        0        0    11570 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/base_model.py
+-rw-r--r--   0        0        0      749 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/base_model_structure.py
+-rw-r--r--   0        0        0      109 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/__init__.py
+-rw-r--r--   0        0        0    12325 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/dfoundations_model.py
+-rw-r--r--   0        0        0     1619 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/dfoundations_parserprovider.py
+-rw-r--r--   0        0        0     3539 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/dfoundations_structures.py
+-rw-r--r--   0        0        0    27768 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/internal.py
+-rw-r--r--   0        0        0     3020 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/internal_soil.py
+-rw-r--r--   0        0        0    19272 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/piles.py
+-rw-r--r--   0        0        0     3958 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/profiles.py
+-rw-r--r--   0        0        0      603 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/serializer.py
+-rw-r--r--   0        0        0     4350 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv
+-rw-r--r--   0        0        0     4337 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv
+-rw-r--r--   0        0        0    27924 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dfoundations/templates/input.foi.j2
+-rw-r--r--   0        0        0      114 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dgeoflow/__init__.py
+-rw-r--r--   0        0        0    16831 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dgeoflow/dgeoflow_model.py
+-rw-r--r--   0        0        0     4275 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py
+-rw-r--r--   0        0        0      333 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dgeoflow/dgeoflow_validator.py
+-rw-r--r--   0        0        0    31320 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dgeoflow/internal.py
+-rw-r--r--   0        0        0     3513 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dgeoflow/serializer.py
+-rw-r--r--   0        0        0      581 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dgeoflow/utils.py
+-rw-r--r--   0        0        0    54527 2023-08-03 11:21:56.974539 d_geolib-1.2.0/geolib/models/dseries_parser.py
+-rw-r--r--   0        0        0      106 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/__init__.py
+-rw-r--r--   0        0        0      301 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/drain_types.py
+-rw-r--r--   0        0        0     5529 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/drains.py
+-rw-r--r--   0        0        0    21412 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/dsettlement_model.py
+-rw-r--r--   0        0        0     1518 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/dsettlement_parserprovider.py
+-rw-r--r--   0        0        0     7147 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/dsettlement_structures.py
+-rw-r--r--   0        0        0    34035 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/internal.py
+-rw-r--r--   0        0        0     5500 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/internal_soil.py
+-rw-r--r--   0        0        0     5960 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/loads.py
+-rw-r--r--   0        0        0      233 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/probabilistic_calculation_types.py
+-rw-r--r--   0        0        0      559 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/serializer.py
+-rw-r--r--   0        0        0    18393 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/templates/input.sli.j2
+-rw-r--r--   0        0        0     4965 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsettlement/templates/soil_template.j2
+-rw-r--r--   0        0        0      110 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/__init__.py
+-rw-r--r--   0        0        0    11250 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/calculation_options.py
+-rw-r--r--   0        0        0    21608 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/constructions.py
+-rw-r--r--   0        0        0    19431 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/dsheetpiling_model.py
+-rw-r--r--   0        0        0     1528 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py
+-rw-r--r--   0        0        0     4647 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/dsheetpiling_structures.py
+-rw-r--r--   0        0        0     3841 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/dsheetpiling_validator.py
+-rw-r--r--   0        0        0    53609 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/internal.py
+-rw-r--r--   0        0        0    15559 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/internal_partial_factors.py
+-rw-r--r--   0        0        0     9894 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/loads.py
+-rw-r--r--   0        0        0     1726 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/profiles.py
+-rw-r--r--   0        0        0      561 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/serializer.py
+-rw-r--r--   0        0        0     5062 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/settings.py
+-rw-r--r--   0        0        0     3465 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/supports.py
+-rw-r--r--   0        0        0     1700 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/surface.py
+-rw-r--r--   0        0        0    35235 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/templates/input.shi.j2
+-rw-r--r--   0        0        0      462 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dsheetpiling/water_level.py
+-rw-r--r--   0        0        0      118 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dstability/__init__.py
+-rw-r--r--   0        0        0    12506 2023-08-03 11:21:56.990166 d_geolib-1.2.0/geolib/models/dstability/analysis.py
+-rw-r--r--   0        0        0    42618 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/dstability/dstability_model.py
+-rw-r--r--   0        0        0     4189 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/dstability/dstability_parserprovider.py
+-rw-r--r--   0        0        0     2865 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/dstability/dstability_validator.py
+-rw-r--r--   0        0        0    90818 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/dstability/internal.py
+-rw-r--r--   0        0        0     2963 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/dstability/loads.py
+-rw-r--r--   0        0        0     3435 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/dstability/reinforcements.py
+-rw-r--r--   0        0        0     3525 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/dstability/serializer.py
+-rw-r--r--   0        0        0     3331 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/dstability/states.py
+-rw-r--r--   0        0        0      581 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/dstability/utils.py
+-rw-r--r--   0        0        0      142 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/internal.py
+-rw-r--r--   0        0        0     1781 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/meta.py
+-rw-r--r--   0        0        0       89 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/model_enums.py
+-rw-r--r--   0        0        0     1821 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/parsers.py
+-rw-r--r--   0        0        0      840 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/serializers.py
+-rw-r--r--   0        0        0     2433 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/utils.py
+-rw-r--r--   0        0        0      314 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/models/validators.py
+-rw-r--r--   0        0        0       55 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/service/__init__.py
+-rw-r--r--   0        0        0     5849 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/service/main.py
+-rw-r--r--   0        0        0      546 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/service/README.md
+-rw-r--r--   0        0        0      797 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/soils/__init__.py
+-rw-r--r--   0        0        0     1720 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/soils/layers.py
+-rw-r--r--   0        0        0      592 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/soils/library.py
+-rw-r--r--   0        0        0    37671 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/soils/soil.py
+-rw-r--r--   0        0        0      775 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/soils/soil_utils.py
+-rw-r--r--   0        0        0     1574 2023-08-03 11:21:57.005790 d_geolib-1.2.0/geolib/utils.py
+-rw-r--r--   0        0        0     1086 2023-08-03 11:21:56.943297 d_geolib-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2055 2023-08-03 11:43:42.632799 d_geolib-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2955 2023-08-03 11:21:56.943297 d_geolib-1.2.0/README.rst
+-rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 d_geolib-1.2.0/PKG-INFO
```

### Comparing `d_geolib-1.1.0/geolib/errors.py` & `d_geolib-1.2.0/geolib/errors.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/geometry/one.py` & `d_geolib-1.2.0/geolib/geometry/one.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/base_model.py` & `d_geolib-1.2.0/geolib/models/base_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/base_model_structure.py` & `d_geolib-1.2.0/geolib/models/base_model_structure.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_model.py` & `d_geolib-1.2.0/geolib/models/dfoundations/dfoundations_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_parserprovider.py` & `d_geolib-1.2.0/geolib/models/dfoundations/dfoundations_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dfoundations/dfoundations_structures.py` & `d_geolib-1.2.0/geolib/models/dfoundations/dfoundations_structures.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dfoundations/internal.py` & `d_geolib-1.2.0/geolib/models/dfoundations/internal.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dfoundations/internal_soil.py` & `d_geolib-1.2.0/geolib/models/dfoundations/internal_soil.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dfoundations/piles.py` & `d_geolib-1.2.0/geolib/models/dfoundations/piles.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dfoundations/profiles.py` & `d_geolib-1.2.0/geolib/models/dfoundations/profiles.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dfoundations/serializer.py` & `d_geolib-1.2.0/geolib/models/dfoundations/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv` & `d_geolib-1.2.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv` & `d_geolib-1.2.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dfoundations/templates/input.foi.j2` & `d_geolib-1.2.0/geolib/models/dfoundations/templates/input.foi.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dgeoflow/dgeoflow_model.py` & `d_geolib-1.2.0/geolib/models/dgeoflow/dgeoflow_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py` & `d_geolib-1.2.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dgeoflow/internal.py` & `d_geolib-1.2.0/geolib/models/dgeoflow/internal.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dgeoflow/serializer.py` & `d_geolib-1.2.0/geolib/models/dgeoflow/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dgeoflow/utils.py` & `d_geolib-1.2.0/geolib/models/dgeoflow/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dseries_parser.py` & `d_geolib-1.2.0/geolib/models/dseries_parser.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsettlement/drains.py` & `d_geolib-1.2.0/geolib/models/dsettlement/drains.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_model.py` & `d_geolib-1.2.0/geolib/models/dsettlement/dsettlement_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_parserprovider.py` & `d_geolib-1.2.0/geolib/models/dsettlement/dsettlement_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsettlement/dsettlement_structures.py` & `d_geolib-1.2.0/geolib/models/dsettlement/dsettlement_structures.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsettlement/internal.py` & `d_geolib-1.2.0/geolib/models/dsettlement/internal.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsettlement/internal_soil.py` & `d_geolib-1.2.0/geolib/models/dsettlement/internal_soil.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsettlement/loads.py` & `d_geolib-1.2.0/geolib/models/dsettlement/loads.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsettlement/serializer.py` & `d_geolib-1.2.0/geolib/models/dsettlement/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsettlement/templates/input.sli.j2` & `d_geolib-1.2.0/geolib/models/dsettlement/templates/input.sli.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsettlement/templates/soil_template.j2` & `d_geolib-1.2.0/geolib/models/dsettlement/templates/soil_template.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/calculation_options.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/calculation_options.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/constructions.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/constructions.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_model.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/dsheetpiling_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_structures.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/dsheetpiling_structures.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/dsheetpiling_validator.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/dsheetpiling_validator.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/internal.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/internal.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/internal_partial_factors.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/internal_partial_factors.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/loads.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/loads.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/profiles.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/profiles.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/serializer.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/settings.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/settings.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/supports.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/supports.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/surface.py` & `d_geolib-1.2.0/geolib/models/dsheetpiling/surface.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dsheetpiling/templates/input.shi.j2` & `d_geolib-1.2.0/geolib/models/dsheetpiling/templates/input.shi.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dstability/analysis.py` & `d_geolib-1.2.0/geolib/models/dstability/analysis.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dstability/dstability_model.py` & `d_geolib-1.2.0/geolib/models/dstability/dstability_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import abc
-import re
 from enum import Enum
 from pathlib import Path
-from typing import BinaryIO, Dict, List, Optional, Set, Type, Union
+from typing import BinaryIO, List, Optional, Set, Type, Union
 
+import matplotlib.pyplot as plt
 from pydantic import DirectoryPath, FilePath
+from shapely.geometry import LineString, Point, Polygon
+from shapely.ops import polygonize
+from shapely.validation import make_valid
 
 from geolib.geometry import Point
-from geolib.models import BaseDataClass, BaseModel
+from geolib.models import BaseModel
 from geolib.soils import Soil
 
-from ...utils import camel_to_snake, snake_to_camel
 from .analysis import DStabilityAnalysisMethod
 from .dstability_parserprovider import DStabilityParserProvider
 from .internal import (
     AnalysisType,
     BishopSlipCircleResult,
     CalculationSettings,
-    CalculationType,
     DStabilityResult,
     DStabilityStructure,
+    PersistableLayer,
     PersistablePoint,
     PersistableSoil,
     PersistableStateCorrelation,
     Scenario,
     SoilCollection,
     SoilCorrelation,
+    SoilLayerCollection,
+    SoilVisualisation,
     SpencerSlipPlaneResult,
     UpliftVanSlipCircleResult,
     Waternet,
 )
 from .loads import Consolidation, DStabilityLoad
 from .reinforcements import DStabilityReinforcement
 from .serializer import DStabilityInputSerializer, DStabilityInputZipSerializer
@@ -489,30 +493,124 @@
         """
         scenario_index = self.get_scenario_index(scenario_index)
         stage_index = self.get_stage_index(stage_index)
 
         geometry = self._get_geometry(scenario_index, stage_index)
         soil_layers = self._get_soil_layers(scenario_index, stage_index)
 
-        # do we have this soil code?
+        # Check if we have the soil code
         if not self.soils.has_soil_code(soil_code):
             raise ValueError(
                 f"The soil with code {soil_code} is not defined in the soil collection."
             )
 
-        # add the layer to the geometry
-        # the checks on the validity of the points are done in the PersistableLayer class
-        persistable_layer = geometry.add_layer(
-            id=str(self._get_next_id()), label=label, points=points, notes=notes
+        # Make sure the points are valid
+        persistable_points = self.make_points_valid(points)
+
+        # Create the new layer
+        new_layer = PersistableLayer(
+            Id=str(self._get_next_id()),
+            Label=label,
+            Points=persistable_points,
+            Notes=notes,
         )
 
-        # add the connection between the layer and the soil to soillayers
+        # Add the layer to the geometry
+        self.add_layer_and_connect_points(geometry.Layers, new_layer)
+
+        # Add the connection between the layer and the soil to soillayers
         soil = self.soils.get_soil(soil_code)
-        soil_layers.add_soillayer(layer_id=persistable_layer.Id, soil_id=soil.Id)
-        return int(persistable_layer.Id)
+        soil_layers.add_soillayer(layer_id=new_layer.Id, soil_id=soil.Id)
+        return int(new_layer.Id)
+
+    def make_points_valid(self, points: List[Point]) -> List[PersistablePoint]:
+        valid_points = make_valid(self.geolib_points_to_shapely_polygon(points))
+        return self.to_dstability_points(valid_points)
+
+    def connect_layers(self, layer1: PersistableLayer, layer2: PersistableLayer):
+        """Connects two polygons by adding a the missing points on the polygon edges. Returns the two new polygons."""
+        linestring1 = self.to_shapely_linestring(layer1.Points)
+        linestring2 = self.to_shapely_linestring(layer2.Points)
+
+        # Create a union of the two polygons and polygonize it creating two connected polygons
+        union = linestring1.union(linestring2)
+        result = [geom for geom in polygonize(union)]
+
+        # If the result has two polygons, we return them, otherwise we return the original polygons
+        if len(result) == 2:
+            return result[0].exterior, result[1].exterior
+        else:
+            return linestring1, linestring2
+
+    def add_layer_and_connect_points(
+        self, current_layers: List[PersistableLayer], new_layer: PersistableLayer
+    ):
+        """Adds a new layer to the list of layers and connects the points of the new layer to the existing layers."""
+
+        current_layers.append(new_layer)
+
+        # Check if the new layer intersects with any of the existing layers
+        for layer in current_layers:
+            if layer != new_layer and self.dstability_points_to_shapely_polygon(
+                layer.Points
+            ).exterior.intersects(
+                self.dstability_points_to_shapely_polygon(new_layer.Points).exterior
+            ):
+                # If it does, connect the layers
+                linestring1, linestring2 = self.connect_layers(layer, new_layer)
+
+                # Update the points of the layers
+                current_layers[
+                    current_layers.index(layer)
+                ].Points = self.to_dstability_points(linestring1)
+                current_layers[
+                    current_layers.index(new_layer)
+                ].Points = self.to_dstability_points(linestring2)
+
+    def to_shapely_linestring(self, points: List[PersistablePoint]) -> LineString:
+        converted_points = [(p.X, p.Z) for p in points]
+        converted_points.append(converted_points[0])
+        return LineString(converted_points)
+
+    def dstability_points_to_shapely_polygon(
+        self, points: List[PersistablePoint]
+    ) -> Polygon:
+        return Polygon([(p.X, p.Z) for p in points])
+
+    def geolib_points_to_shapely_polygon(self, points: List[Point]) -> Polygon:
+        return Polygon([(p.x, p.z) for p in points])
+
+    def to_dstability_points(
+        self, shapely_object: Union[LineString, Polygon]
+    ) -> List[PersistablePoint]:
+        if isinstance(shapely_object, LineString):
+            coords = shapely_object.coords
+        elif isinstance(shapely_object, Polygon):
+            coords = shapely_object.exterior.coords
+        else:
+            raise ValueError(
+                "shapely_object must be a LineString or Polygon, not {}".format(
+                    type(shapely_object)
+                )
+            )
+
+        persistable_points = [PersistablePoint(X=p[0], Z=p[1]) for p in list(coords)]
+
+        # Remove duplicate points
+        persistable_points = [
+            i
+            for n, i in enumerate(persistable_points)
+            if i not in persistable_points[n + 1 :]
+        ]
+
+        # Remove last point if it is the same as the first
+        if persistable_points[0] == persistable_points[-1]:
+            persistable_points.pop(-1)
+
+        return persistable_points
 
     def get_soil(self, code: str) -> PersistableSoil:
         """
         Gets an existing soil with the given soil code.
 
         Args:
             code (str): the code of the soil
@@ -946,7 +1044,57 @@
             return stage_index
 
     def get_calculation_index(self, calculation_index: Optional[int]):
         if calculation_index is None:
             return self.current_calculation
         else:
             return calculation_index
+
+    @staticmethod
+    def get_soil_id_from_layer_id(
+        layers: SoilLayerCollection, layer_id: str
+    ) -> Union[str, None]:
+        for layer in layers.SoilLayers:
+            if layer.LayerId == layer_id:
+                return layer.SoilId
+        return None
+
+    @staticmethod
+    def get_color_from_soil_id(
+        soil_visualizations: SoilVisualisation, soil_id: str
+    ) -> str:
+        for soil_visualization in soil_visualizations.SoilVisualizations:
+            if soil_visualization.SoilId == soil_id:
+                return soil_visualization.Color
+        return "#000000"
+
+    def _get_color_of_layer(
+        self, layers_collection: SoilLayerCollection, layer: PersistableLayer
+    ) -> str:
+        layer_id = layer.Id
+        # use the layer id to get the soil type id
+        soil_type_id = DStabilityModel.get_soil_id_from_layer_id(
+            layers_collection, layer_id
+        )
+        # get the color of the soil type
+        color = DStabilityModel.get_color_from_soil_id(
+            self.input.soilvisualizations, soil_type_id
+        )
+        return color.replace("#80", "#")
+
+    def plot(
+        self, scenario_index: Optional[int] = None, stage_index: Optional[int] = None
+    ):
+        geometry = self._get_geometry(scenario_index, stage_index)
+        layers_collection = self._get_soil_layers(scenario_index, stage_index)
+        fig, ax = plt.subplots()
+        # loop over the layers
+        for layer in geometry.Layers:
+            # get list of x and y coordinates
+            x = [p.X for p in layer.Points]
+            y = [p.Z for p in layer.Points]
+            # get color of layer
+            color = self._get_color_of_layer(layers_collection, layer)
+            # create a polygon
+            ax.fill(x, y, color=color)
+        plt.axis("off")
+        return fig, ax
```

### Comparing `d_geolib-1.1.0/geolib/models/dstability/dstability_parserprovider.py` & `d_geolib-1.2.0/geolib/models/dstability/dstability_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dstability/dstability_validator.py` & `d_geolib-1.2.0/geolib/models/dstability/dstability_validator.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dstability/internal.py` & `d_geolib-1.2.0/geolib/models/dstability/internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """
 The internal data model structure.
 """
 
-import json
 from collections import defaultdict
 from datetime import date, datetime
 from enum import Enum
 from itertools import chain
 from math import isfinite
-from typing import Dict, Generator, List, Optional, Set, Tuple, Union
+from typing import Dict, List, Optional, Set, Tuple, Union
 
 from pydantic import ValidationError, conlist, root_validator, validator
 
 from geolib import __version__ as version
 from geolib.geometry import Point
 from geolib.models.base_model_structure import BaseModelStructure
 from geolib.soils import Soil
-from geolib.utils import snake_to_camel
 
 from .dstability_validator import DStabilityValidator
 from .utils import children
 
 
 class DStabilityBaseModelStructure(BaseModelStructure):
     def dict(_, *args, **kwargs):
@@ -1092,15 +1090,17 @@
     LayerLoads: Optional[List[Optional[PersistableLayerLoad]]] = []
     LineLoads: Optional[List[Optional[PersistableLineLoad]]] = []
     Trees: Optional[List[Optional[PersistableTree]]] = []
     UniformLoads: Optional[List[Optional[PersistableUniformLoad]]] = []
 
     def add_load(
         self, load: "DStabilityLoad", consolidations: List["Consolidation"]
-    ) -> Union[PersistableUniformLoad, PersistableLineLoad, PersistableLayerLoad, PersistableTree]:
+    ) -> Union[
+        PersistableUniformLoad, PersistableLineLoad, PersistableLayerLoad, PersistableTree
+    ]:
         internal_datastructure = load.to_internal_datastructure()
 
         # Add consolidations if the load supports it
         if hasattr(internal_datastructure, "Consolidations"):
             internal_datastructure.Consolidations = [
                 c.to_internal_datastructure() for c in consolidations
             ]
```

### Comparing `d_geolib-1.1.0/geolib/models/dstability/loads.py` & `d_geolib-1.2.0/geolib/models/dstability/loads.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,17 @@
     wind_force: float
     width_of_root_zone: float
     angle_of_distribution: float
 
     def to_internal_datastructure(self) -> PersistableTree:
         return PersistableTree(
             Label=self.label,
-            Location=PersistablePoint(X=self.tree_top_location.x, Z=self.tree_top_location.z),
+            Location=PersistablePoint(
+                X=self.tree_top_location.x, Z=self.tree_top_location.z
+            ),
             Force=self.wind_force,
             RootZoneWidth=self.width_of_root_zone,
             Spread=self.angle_of_distribution,
         )
 
 
 class Earthquake(DStabilityLoad):
```

### Comparing `d_geolib-1.1.0/geolib/models/dstability/reinforcements.py` & `d_geolib-1.2.0/geolib/models/dstability/reinforcements.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dstability/serializer.py` & `d_geolib-1.2.0/geolib/models/dstability/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dstability/states.py` & `d_geolib-1.2.0/geolib/models/dstability/states.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/dstability/utils.py` & `d_geolib-1.2.0/geolib/models/dstability/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/meta.py` & `d_geolib-1.2.0/geolib/models/meta.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/parsers.py` & `d_geolib-1.2.0/geolib/models/parsers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/serializers.py` & `d_geolib-1.2.0/geolib/models/serializers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/models/utils.py` & `d_geolib-1.2.0/geolib/models/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/service/main.py` & `d_geolib-1.2.0/geolib/service/main.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/service/README.md` & `d_geolib-1.2.0/geolib/service/README.md`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/soils/__init__.py` & `d_geolib-1.2.0/geolib/soils/__init__.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/soils/layers.py` & `d_geolib-1.2.0/geolib/soils/layers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/soils/library.py` & `d_geolib-1.2.0/geolib/soils/library.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/soils/soil.py` & `d_geolib-1.2.0/geolib/soils/soil.py`

 * *Files 1% similar despite different names*

```diff
@@ -662,15 +662,15 @@
             "soilstdseccompindex": self.isotache_parameters.primary_compression_constant_b.standard_deviation,
             "soilstdseccomprate": self.isotache_parameters.secondary_compression_constant_c.standard_deviation,
             "soilstdocr": self.soil_state.ocr_layer.standard_deviation,
             "soilstdpermeabilityver": self.storage_parameters.vertical_permeability.standard_deviation,
             "soilstdpop": self.soil_state.pop_layer.standard_deviation,
             "soilstdpermeabilityhorfactor": self.storage_parameters.permeability_horizontal_factor.standard_deviation,
             "soilstdinitialvoidratio": self.soil_classification_parameters.initial_void_ratio.standard_deviation,
-            "soilstdpermeabilitystrainmodulus": None,
+            "soilstdpermeabilitystrainmodulus": self.storage_parameters.permeability_strain_type.standard_deviation,
             "soilstdlimitstress": None,
             "soilstdcp": self.koppejan_parameters.primary_Cp.standard_deviation,
             "soilstdcp1": self.koppejan_parameters.primary_Cp_point.standard_deviation,
             "soilstdcs": self.koppejan_parameters.secular_Cs.standard_deviation,
             "soilstdcs1": self.koppejan_parameters.secular_Cs_point.standard_deviation,
             "soilstdap": self.koppejan_parameters.primary_Ap.standard_deviation,
             "soilstdasec": self.koppejan_parameters.primary_Asec.standard_deviation,
```

### Comparing `d_geolib-1.1.0/geolib/soils/soil_utils.py` & `d_geolib-1.2.0/geolib/soils/soil_utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/geolib/utils.py` & `d_geolib-1.2.0/geolib/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/LICENSE` & `d_geolib-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/pyproject.toml` & `d_geolib-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "d-geolib"
-version = "1.1.0"
+version = "1.2.0"
 description = "Python wrappers around the input and output files of the Deltares D-Serie and D-GEO Suite models"
 authors = ["Maarten Pronk <maarten.pronk@deltares.nl>", "Deltares"]
 license = "MIT"
 homepage = "https://deltares.github.io/GEOLib/"
 documentation = "https://deltares.github.io/GEOLib/"
 repository = "https://github.com/Deltares/GEOLib"
 readme = "README.rst"
@@ -18,15 +18,17 @@
 zipp = "^3.15.0"
 fastapi = {version = "^0.95.1", optional = true}
 uvicorn = {version = "^0.21.1", optional = true}
 requests = "^2.29.0"
 jinja2 = "^3.1.2"
 httpx = {version = "^0.24.0", optional = true}
 starlette = "^0.26.1"
+shapely = "^2.0.1"
 python-dotenv = "^1.0.0"
+matplotlib = ">=3.7.2"
 
 [tool.poetry.group.dev.dependencies]
 teamcity-messages = "^1.32"
 flake8 = "^6.0.0"
 black = "^23.3.0"
 devtools = "^0.11.0"
 pytest = "^7.3.1"
@@ -68,15 +70,15 @@
 force_grid_wrap=0
 use_parentheses=true
 line_length=90
 profile = "black"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.1.0"
+version = "1.2.0"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:^version",
     "tests/test_geolib.py",
     "geolib/__init__.py:__version__",
 ]
-annotated_tag = true
+annotated_tag = true
```

### Comparing `d_geolib-1.1.0/README.rst` & `d_geolib-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `d_geolib-1.1.0/PKG-INFO` & `d_geolib-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d-geolib
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python wrappers around the input and output files of the Deltares D-Serie and D-GEO Suite models
 Home-page: https://deltares.github.io/GEOLib/
 License: MIT
 Author: Maarten Pronk
 Author-email: maarten.pronk@deltares.nl
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,17 +12,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: server
 Requires-Dist: fastapi (>=0.95.1,<0.96.0) ; extra == "server"
 Requires-Dist: httpx (>=0.24.0,<0.25.0) ; extra == "server"
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: matplotlib (>=3.7.2)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Requires-Dist: starlette (>=0.26.1,<0.27.0) ; extra == "server"
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0) ; extra == "server"
 Requires-Dist: zipp (>=3.15.0,<4.0.0)
 Project-URL: Documentation, https://deltares.github.io/GEOLib/
 Project-URL: Repository, https://github.com/Deltares/GEOLib
 Description-Content-Type: text/x-rst
```

