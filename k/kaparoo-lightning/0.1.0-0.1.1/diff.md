# Comparing `tmp/kaparoo_lightning-0.1.0.tar.gz` & `tmp/kaparoo_lightning-0.1.1.tar.gz`

## Comparing `kaparoo_lightning-0.1.0.tar` & `kaparoo_lightning-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/common/__init__.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/common/spec.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/common/types.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/data/__init__.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/data/constants.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/data/dataloaders.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/data/datamodules.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/data/dataset/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/data/dataset/datasets.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/data/dataset/traits.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/kaparoo_lightning/data/dataset/types.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/LICENSE
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/README.md
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/common/__init__.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/common/spec.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/common/types.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/__init__.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/constants.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/dataloaders.py
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/datamodules.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/datasets/datasets.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/datasets/traits.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/datasets/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/nn/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/nn/models/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/nn/models/gan.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/README.md
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/PKG-INFO
```

### Comparing `kaparoo_lightning-0.1.0/kaparoo_lightning/common/spec.py` & `kaparoo_lightning-0.1.1/kaparoo_lightning/common/spec.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.0/kaparoo_lightning/data/__init__.py` & `kaparoo_lightning-0.1.1/kaparoo_lightning/data/__init__.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.0/kaparoo_lightning/data/constants.py` & `kaparoo_lightning-0.1.1/kaparoo_lightning/data/constants.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.0/kaparoo_lightning/data/dataloaders.py` & `kaparoo_lightning-0.1.1/kaparoo_lightning/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.0/kaparoo_lightning/data/datamodules.py` & `kaparoo_lightning-0.1.1/kaparoo_lightning/data/datamodules.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,33 +5,34 @@
 __all__ = (
     "DataModuleBase",
     "DataModule",
     "TransformableDataModule",
     "LabelTransformableDataModule",
 )
 
-from typing import TYPE_CHECKING, Generic
+from typing import TYPE_CHECKING, Generic, TypeVar
 
 from kaparoo.utils.optional import unwrap_or_default
 from lightning import LightningDataModule
 from torch.utils.data import DataLoader, Dataset
 
 from kaparoo_lightning.common.spec import update_spec
 from kaparoo_lightning.data.constants import BATCH_SIZE, NUM_WORKERS, SUBSETS
 
 if TYPE_CHECKING:
-    from typing import Any, TypeVar
+    from typing import Any
 
     from kaparoo.utils.types import T_co
     from typing_extensions import LiteralString
 
     from kaparoo_lightning.data.dataloaders import DataLoaderSpec
 
-    TransformType = TypeVar("TransformType")
-    LabelTransformType = TypeVar("LabelTransformType")
+
+TransformType = TypeVar("TransformType")
+LabelTransformType = TypeVar("LabelTransformType")
 
 
 class DataModuleBase(LightningDataModule, Generic[T_co]):
     def __init__(self) -> None:
         super().__init__()
         self.dataset_train: Dataset[T_co] | None = None
         self.dataset_valid: Dataset[T_co] | None = None
```

### Comparing `kaparoo_lightning-0.1.0/kaparoo_lightning/data/dataset/datasets.py` & `kaparoo_lightning-0.1.1/kaparoo_lightning/data/datasets/datasets.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 __all__ = ("MultiDomainDataset", "DoubleDomainDataset")
 
 from typing import TYPE_CHECKING, Generic
 
 from torch.utils.data import Dataset
 
-from kaparoo_lightning.data.dataset.traits import MultiDomain
+from kaparoo_lightning.data.datasets.traits import MultiDomain
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from torch import Tensor
+    from typing_extensions import LiteralString
 
     from kaparoo_lightning.common.types import TensorFn
-    from kaparoo_lightning.data.dataset.types import DataType, TransformType
+    from kaparoo_lightning.data.datasets.types import DataType, TransformType
 
 
 class _MultiDomainDataset(
     MultiDomain[DataType, TransformType],
     Dataset[DataType],
     Generic[DataType, TransformType],
 ):
@@ -28,14 +29,26 @@
         self,
         num_domains: int,
         transforms: TransformType | Sequence[TransformType | None] | None = None,
     ) -> None:
         MultiDomain.__init__(self, num_domains, transforms)
         Dataset.__init__(self)
 
+    def __str__(self) -> LiteralString:
+        return self.__class__.__name__
+
 
 class MultiDomainDataset(_MultiDomainDataset[tuple[Tensor, ...], TensorFn]):
-    pass
+    def __init__(
+        self,
+        num_domains: int,
+        transforms: TensorFn | Sequence[TensorFn | None] | None = None,
+    ) -> None:
+        super().__init__(num_domains, transforms)
 
 
 class DoubleDomainDataset(_MultiDomainDataset[tuple[Tensor, Tensor], TensorFn]):
-    pass
+    def __init__(
+        self,
+        transforms: TensorFn | Sequence[TensorFn | None] | None = None,
+    ) -> None:
+        super().__init__(2, transforms)
```

### Comparing `kaparoo_lightning-0.1.0/kaparoo_lightning/data/dataset/traits.py` & `kaparoo_lightning-0.1.1/kaparoo_lightning/data/datasets/traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 __all__ = ("MultiDomain", "MultiLabeled")
 
 from collections.abc import Sequence
 from typing import TYPE_CHECKING, Generic
 
 if TYPE_CHECKING:
-    from kaparoo_lightning.data.dataset.types import DataType, LabelType, TransformType
+    from kaparoo_lightning.data.datasets.types import DataType, LabelType, TransformType
 
 
 def unwrap_transforms(
     transforms: TransformType | Sequence[TransformType | None] | None,
     max_transforms: int,
 ) -> tuple[TransformType | None, ...]:
     if not isinstance(max_transforms, int) or max_transforms < 1:
```

### Comparing `kaparoo_lightning-0.1.0/.gitignore` & `kaparoo_lightning-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.0/LICENSE` & `kaparoo_lightning-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.0/README.md` & `kaparoo_lightning-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.0/pyproject.toml` & `kaparoo_lightning-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.0/PKG-INFO` & `kaparoo_lightning-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-lightning
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for (personally) common and useful features for PyTorch Lightning.
 Project-URL: GitHub, https://www.github.com/kaparoo/lightning-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
```

