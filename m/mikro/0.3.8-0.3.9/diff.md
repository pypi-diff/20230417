# Comparing `tmp/mikro-0.3.8.tar.gz` & `tmp/mikro-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikro-0.3.8.tar", max compression
+gzip compressed data, was "mikro-0.3.9.tar", max compression
```

## Comparing `mikro-0.3.8.tar` & `mikro-0.3.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      101 2022-08-25 11:10:14.051638 mikro-0.3.8/mikro/__init__.py
--rw-r--r--   0        0        0       38 2022-11-21 13:25:24.312569 mikro-0.3.8/mikro/api/__init__.py
--rw-r--r--   0        0        0   236651 2022-12-15 13:08:13.967403 mikro-0.3.8/mikro/api/schema.py
--rw-r--r--   0        0        0        0 2022-11-21 13:19:21.452118 mikro-0.3.8/mikro/builders.py
--rw-r--r--   0        0        0     4468 2022-12-08 12:30:42.620796 mikro-0.3.8/mikro/cli/main.py
--rw-r--r--   0        0        0        0 2022-08-25 14:13:51.564206 mikro-0.3.8/mikro/contrib/__init__.py
--rw-r--r--   0        0        0        0 2022-02-03 16:40:05.361043 mikro-0.3.8/mikro/contrib/fakts/__init__.py
--rw-r--r--   0        0        0     1303 2022-11-21 13:24:56.296558 mikro-0.3.8/mikro/contrib/fakts/datalayer.py
--rw-r--r--   0        0        0     4531 2022-11-21 17:10:07.795408 mikro-0.3.8/mikro/datalayer.py
--rw-r--r--   0        0        0      156 2022-03-21 13:01:57.991994 mikro-0.3.8/mikro/errors.py
--rw-r--r--   0        0        0     1174 2022-11-21 13:16:43.067875 mikro-0.3.8/mikro/funcs.py
--rw-r--r--   0        0        0       92 2022-03-21 13:01:58.083994 mikro-0.3.8/mikro/links/__init__.py
--rw-r--r--   0        0        0     2413 2022-11-21 13:12:09.135444 mikro-0.3.8/mikro/links/datalayer.py
--rw-r--r--   0        0        0        0 2022-05-17 11:20:06.504915 mikro-0.3.8/mikro/links/errors.py
--rw-r--r--   0        0        0      903 2022-11-21 13:21:58.284355 mikro-0.3.8/mikro/mikro.py
--rw-r--r--   0        0        0     1522 2022-11-21 13:25:20.364567 mikro-0.3.8/mikro/rath.py
--rw-r--r--   0        0        0    11140 2022-12-15 13:11:50.270311 mikro-0.3.8/mikro/scalars.py
--rw-r--r--   0        0        0     4098 2022-12-12 14:45:25.646781 mikro-0.3.8/mikro/structures.py
--rw-r--r--   0        0        0     5750 2022-12-15 10:05:28.013204 mikro-0.3.8/mikro/traits.py
--rw-r--r--   0        0        0      805 2022-09-26 09:28:04.741028 mikro-0.3.8/mikro/widgets.py
--rw-r--r--   0        0        0     1241 2022-12-15 13:39:36.922995 mikro-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 mikro-0.3.8/setup.py
--rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 mikro-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      101 2022-08-25 11:10:14.051638 mikro-0.3.9/mikro/__init__.py
+-rw-r--r--   0        0        0       38 2022-11-21 13:25:24.312569 mikro-0.3.9/mikro/api/__init__.py
+-rw-r--r--   0        0        0   242929 2022-12-15 13:54:09.942241 mikro-0.3.9/mikro/api/schema.py
+-rw-r--r--   0        0        0        0 2022-11-21 13:19:21.452118 mikro-0.3.9/mikro/builders.py
+-rw-r--r--   0        0        0     4468 2022-12-08 12:30:42.620796 mikro-0.3.9/mikro/cli/main.py
+-rw-r--r--   0        0        0        0 2022-08-25 14:13:51.564206 mikro-0.3.9/mikro/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-03 16:40:05.361043 mikro-0.3.9/mikro/contrib/fakts/__init__.py
+-rw-r--r--   0        0        0     1303 2022-11-21 13:24:56.296558 mikro-0.3.9/mikro/contrib/fakts/datalayer.py
+-rw-r--r--   0        0        0     4531 2022-11-21 17:10:07.795408 mikro-0.3.9/mikro/datalayer.py
+-rw-r--r--   0        0        0      156 2022-03-21 13:01:57.991994 mikro-0.3.9/mikro/errors.py
+-rw-r--r--   0        0        0     1174 2022-11-21 13:16:43.067875 mikro-0.3.9/mikro/funcs.py
+-rw-r--r--   0        0        0       92 2022-03-21 13:01:58.083994 mikro-0.3.9/mikro/links/__init__.py
+-rw-r--r--   0        0        0     2413 2022-11-21 13:12:09.135444 mikro-0.3.9/mikro/links/datalayer.py
+-rw-r--r--   0        0        0        0 2022-05-17 11:20:06.504915 mikro-0.3.9/mikro/links/errors.py
+-rw-r--r--   0        0        0      903 2022-11-21 13:21:58.284355 mikro-0.3.9/mikro/mikro.py
+-rw-r--r--   0        0        0     1522 2022-11-21 13:25:20.364567 mikro-0.3.9/mikro/rath.py
+-rw-r--r--   0        0        0    12037 2022-12-15 13:54:02.174160 mikro-0.3.9/mikro/scalars.py
+-rw-r--r--   0        0        0     4098 2022-12-12 14:45:25.646781 mikro-0.3.9/mikro/structures.py
+-rw-r--r--   0        0        0     5750 2022-12-15 10:05:28.013204 mikro-0.3.9/mikro/traits.py
+-rw-r--r--   0        0        0      805 2022-09-26 09:28:04.741028 mikro-0.3.9/mikro/widgets.py
+-rw-r--r--   0        0        0     1241 2022-12-15 14:13:59.916979 mikro-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 mikro-0.3.9/setup.py
+-rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 mikro-0.3.9/PKG-INFO
```

### Comparing `mikro-0.3.8/mikro/api/schema.py` & `mikro-0.3.9/mikro/api/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from mikro.funcs import aexecute, asubscribe, subscribe, execute
-from mikro.traits import Vectorizable, Table, Stage, Objective, ROI, Representation
+from mikro.traits import Representation, Table, ROI, Objective, Vectorizable, Stage
+from mikro.rath import MikroRath
 from enum import Enum
+from mikro.funcs import subscribe, execute, aexecute, asubscribe
 from mikro.scalars import (
-    XArrayInput,
-    Store,
-    FeatureValue,
-    Parquet,
     ModelFile,
+    Parquet,
+    File,
+    Model,
+    Store,
     MetricValue,
     ParquetInput,
-    File,
+    FeatureValue,
+    XArrayInput,
 )
-from mikro.rath import MikroRath
-from rath.scalars import ID
-from typing import Literal, AsyncIterator, List, Iterator, Optional, Tuple, Dict
+from typing import Dict, Literal, Iterator, Tuple, List, Optional, AsyncIterator
 from datetime import datetime
+from rath.scalars import ID
 from pydantic import Field, BaseModel
 
 
 class CommentableModels(str, Enum):
     GRUNNLAG_USERMETA = "GRUNNLAG_USERMETA"
     GRUNNLAG_ANTIBODY = "GRUNNLAG_ANTIBODY"
     GRUNNLAG_OBJECTIVE = "GRUNNLAG_OBJECTIVE"
@@ -1236,16 +1237,16 @@
     class Config:
         frozen = True
 
 
 class ImageToImageModelFragment(BaseModel):
     typename: Optional[Literal["ImageToImageModel"]] = Field(alias="__typename")
     id: ID
-    data: Optional[str]
-    "The model"
+    data: Optional[Model]
+    "The model data"
     kind: Optional[ModelKind]
     "The kind of model"
     name: str
     "The name of the model"
     training_data: Tuple[ImageToImageModelFragmentTrainingdata, ...] = Field(
         alias="trainingData"
     )
@@ -1946,29 +1947,29 @@
         sample: Optional[ID] = None
         variety: Optional[RepresentationVarietyInput] = None
 
     class Meta:
         document = "fragment Representation on Representation {\n  sample {\n    id\n    name\n  }\n  shape\n  id\n  store\n  variety\n  name\n  omero {\n    scale\n    physicalSize {\n      x\n      y\n      z\n      t\n      c\n    }\n  }\n  origins {\n    id\n    store\n    variety\n  }\n}\n\nmutation update_representation($id: ID!, $tags: [String], $sample: ID, $variety: RepresentationVarietyInput) {\n  updateRepresentation(rep: $id, tags: $tags, sample: $sample, variety: $variety) {\n    ...Representation\n  }\n}"
 
 
-class Create_i2i_modelMutation(BaseModel):
+class Create_image_to_image_modelMutation(BaseModel):
     create_image_to_image_model: Optional[ImageToImageModelFragment] = Field(
         alias="createImageToImageModel"
     )
     "Creates an Instrument\n    \n    This mutation creates an Instrument and returns the created Instrument.\n    The serial number is required and the manufacturer is inferred from the serial number.\n    "
 
     class Arguments(BaseModel):
         data: ModelFile
         kind: ModelKind
         name: str
         training_data: Optional[List[Optional[ID]]] = None
         experiments: Optional[List[Optional[ID]]] = None
 
     class Meta:
-        document = "fragment ImageToImageModel on ImageToImageModel {\n  id\n  data\n  kind\n  name\n  trainingData {\n    id\n  }\n}\n\nmutation create_i2i_model($data: ModelFile!, $kind: ModelKind!, $name: String!, $training_data: [ID], $experiments: [ID]) {\n  createImageToImageModel(\n    data: $data\n    kind: $kind\n    name: $name\n    trainingData: $training_data\n    experiments: $experiments\n  ) {\n    ...ImageToImageModel\n  }\n}"
+        document = "fragment ImageToImageModel on ImageToImageModel {\n  id\n  data\n  kind\n  name\n  trainingData {\n    id\n  }\n}\n\nmutation create_image_to_image_model($data: ModelFile!, $kind: ModelKind!, $name: String!, $training_data: [ID], $experiments: [ID]) {\n  createImageToImageModel(\n    data: $data\n    kind: $kind\n    name: $name\n    trainingData: $training_data\n    experiments: $experiments\n  ) {\n    ...ImageToImageModel\n  }\n}"
 
 
 class Create_metricMutation(BaseModel):
     create_metric: Optional[MetricFragment] = Field(alias="createMetric")
     "Create a metric\n\n    This mutation creates a metric and returns the created metric.\n    \n    "
 
     class Arguments(BaseModel):
@@ -2721,14 +2722,61 @@
     class Arguments(BaseModel):
         search: Optional[str] = None
 
     class Meta:
         document = "query search_tags($search: String) {\n  options: tags(name: $search) {\n    value: slug\n    label: name\n  }\n}"
 
 
+class Get_image_to_image_modelQuery(BaseModel):
+    image_to_image_model: Optional[ImageToImageModelFragment] = Field(
+        alias="imageToImageModel"
+    )
+    "Get a single label by ID\n    \n    Returns a single label by ID. If the user does not have access\n    to the label, an error will be raised."
+
+    class Arguments(BaseModel):
+        id: ID
+
+    class Meta:
+        document = "fragment ImageToImageModel on ImageToImageModel {\n  id\n  data\n  kind\n  name\n  trainingData {\n    id\n  }\n}\n\nquery get_image_to_image_model($id: ID!) {\n  imageToImageModel(id: $id) {\n    ...ImageToImageModel\n  }\n}"
+
+
+class Expand_image_to_image_modelQuery(BaseModel):
+    label: Optional[LabelFragment]
+    "Get a single label by ID\n    \n    Returns a single label by ID. If the user does not have access\n    to the label, an error will be raised."
+
+    class Arguments(BaseModel):
+        id: ID
+
+    class Meta:
+        document = "fragment Label on Label {\n  instance\n  id\n  representation {\n    id\n    name\n  }\n}\n\nquery expand_image_to_image_model($id: ID!) {\n  label(id: $id) {\n    ...Label\n  }\n}"
+
+
+class Search_image_to_image_modelsQueryOptions(BaseModel):
+    """ImageToImageModel(id, created_by, created_through, kind, data, name, created_at, creator, model_ptr)"""
+
+    typename: Optional[Literal["ImageToImageModel"]] = Field(alias="__typename")
+    label: str
+    "The name of the model"
+    value: ID
+
+    class Config:
+        frozen = True
+
+
+class Search_image_to_image_modelsQuery(BaseModel):
+    options: Optional[Tuple[Optional[Search_image_to_image_modelsQueryOptions], ...]]
+    "All Labels\n    \n    This query returns all Labels that are stored on the platform\n    depending on the user's permissions. Generally, this query will return\n    all Labels that the user has access to. If the user is an amdin\n    or superuser, all Labels will be returned.\n    "
+
+    class Arguments(BaseModel):
+        search: Optional[str] = None
+
+    class Meta:
+        document = "query search_image_to_image_models($search: String) {\n  options: imageToImageModels(name: $search, limit: 20) {\n    label: name\n    value: id\n  }\n}"
+
+
 class Expand_metricQuery(BaseModel):
     """Creates a new representation"""
 
     metric: Optional[MetricFragment]
     "Get a single Metric by ID\n    \n    Returns a single Metric by ID. If the user does not have access\n    to the Metric, an error will be raised.\n    "
 
     class Arguments(BaseModel):
@@ -4146,23 +4194,23 @@
     return execute(
         Update_representationMutation,
         {"id": id, "tags": tags, "sample": sample, "variety": variety},
         rath=rath,
     ).update_representation
 
 
-async def acreate_i2i_model(
+async def acreate_image_to_image_model(
     data: ModelFile,
     kind: ModelKind,
     name: str,
     training_data: Optional[List[Optional[ID]]] = None,
     experiments: Optional[List[Optional[ID]]] = None,
     rath: MikroRath = None,
 ) -> Optional[ImageToImageModelFragment]:
-    """create_i2i_model
+    """create_image_to_image_model
 
 
      createImageToImageModel: ImageToImageModel(id, created_by, created_through, kind, data, name, created_at, creator, model_ptr)
 
 
     Arguments:
         data (ModelFile): data
@@ -4172,36 +4220,36 @@
         experiments (Optional[List[Optional[ID]]], optional): experiments.
         rath (mikro.rath.MikroRath, optional): The mikro rath client
 
     Returns:
         Optional[ImageToImageModelFragment]"""
     return (
         await aexecute(
-            Create_i2i_modelMutation,
+            Create_image_to_image_modelMutation,
             {
                 "data": data,
                 "kind": kind,
                 "name": name,
                 "training_data": training_data,
                 "experiments": experiments,
             },
             rath=rath,
         )
     ).create_image_to_image_model
 
 
-def create_i2i_model(
+def create_image_to_image_model(
     data: ModelFile,
     kind: ModelKind,
     name: str,
     training_data: Optional[List[Optional[ID]]] = None,
     experiments: Optional[List[Optional[ID]]] = None,
     rath: MikroRath = None,
 ) -> Optional[ImageToImageModelFragment]:
-    """create_i2i_model
+    """create_image_to_image_model
 
 
      createImageToImageModel: ImageToImageModel(id, created_by, created_through, kind, data, name, created_at, creator, model_ptr)
 
 
     Arguments:
         data (ModelFile): data
@@ -4210,15 +4258,15 @@
         training_data (Optional[List[Optional[ID]]], optional): training_data.
         experiments (Optional[List[Optional[ID]]], optional): experiments.
         rath (mikro.rath.MikroRath, optional): The mikro rath client
 
     Returns:
         Optional[ImageToImageModelFragment]"""
     return execute(
-        Create_i2i_modelMutation,
+        Create_image_to_image_modelMutation,
         {
             "data": data,
             "kind": kind,
             "name": name,
             "training_data": training_data,
             "experiments": experiments,
         },
@@ -6238,14 +6286,152 @@
         rath (mikro.rath.MikroRath, optional): The mikro rath client
 
     Returns:
         Optional[List[Optional[Search_tagsQueryTags]]]"""
     return execute(Search_tagsQuery, {"search": search}, rath=rath).tags
 
 
+async def aget_image_to_image_model(
+    id: ID, rath: MikroRath = None
+) -> Optional[ImageToImageModelFragment]:
+    """get_image_to_image_model
+
+
+     imageToImageModel: ImageToImageModel(id, created_by, created_through, kind, data, name, created_at, creator, model_ptr)
+
+
+    Arguments:
+        id (ID): id
+        rath (mikro.rath.MikroRath, optional): The mikro rath client
+
+    Returns:
+        Optional[ImageToImageModelFragment]"""
+    return (
+        await aexecute(Get_image_to_image_modelQuery, {"id": id}, rath=rath)
+    ).image_to_image_model
+
+
+def get_image_to_image_model(
+    id: ID, rath: MikroRath = None
+) -> Optional[ImageToImageModelFragment]:
+    """get_image_to_image_model
+
+
+     imageToImageModel: ImageToImageModel(id, created_by, created_through, kind, data, name, created_at, creator, model_ptr)
+
+
+    Arguments:
+        id (ID): id
+        rath (mikro.rath.MikroRath, optional): The mikro rath client
+
+    Returns:
+        Optional[ImageToImageModelFragment]"""
+    return execute(
+        Get_image_to_image_modelQuery, {"id": id}, rath=rath
+    ).image_to_image_model
+
+
+async def aexpand_image_to_image_model(
+    id: ID, rath: MikroRath = None
+) -> Optional[LabelFragment]:
+    """expand_image_to_image_model
+
+
+     label: A Label is a trough model for image and features.
+
+        Its map an instance value of a representation
+        (e.g. a pixel value of a segmentation mask) to a set of corresponding features of the segmented
+        class instance.
+
+        There can only be one label per representation and class instance. You can then attach
+        features to the label.
+
+
+
+
+
+    Arguments:
+        id (ID): id
+        rath (mikro.rath.MikroRath, optional): The mikro rath client
+
+    Returns:
+        Optional[LabelFragment]"""
+    return (
+        await aexecute(Expand_image_to_image_modelQuery, {"id": id}, rath=rath)
+    ).label
+
+
+def expand_image_to_image_model(
+    id: ID, rath: MikroRath = None
+) -> Optional[LabelFragment]:
+    """expand_image_to_image_model
+
+
+     label: A Label is a trough model for image and features.
+
+        Its map an instance value of a representation
+        (e.g. a pixel value of a segmentation mask) to a set of corresponding features of the segmented
+        class instance.
+
+        There can only be one label per representation and class instance. You can then attach
+        features to the label.
+
+
+
+
+
+    Arguments:
+        id (ID): id
+        rath (mikro.rath.MikroRath, optional): The mikro rath client
+
+    Returns:
+        Optional[LabelFragment]"""
+    return execute(Expand_image_to_image_modelQuery, {"id": id}, rath=rath).label
+
+
+async def asearch_image_to_image_models(
+    search: Optional[str] = None, rath: MikroRath = None
+) -> Optional[List[Optional[Search_image_to_image_modelsQueryOptions]]]:
+    """search_image_to_image_models
+
+
+     options: ImageToImageModel(id, created_by, created_through, kind, data, name, created_at, creator, model_ptr)
+
+
+    Arguments:
+        search (Optional[str], optional): search.
+        rath (mikro.rath.MikroRath, optional): The mikro rath client
+
+    Returns:
+        Optional[List[Optional[Search_image_to_image_modelsQueryImagetoimagemodels]]]"""
+    return (
+        await aexecute(Search_image_to_image_modelsQuery, {"search": search}, rath=rath)
+    ).image_to_image_models
+
+
+def search_image_to_image_models(
+    search: Optional[str] = None, rath: MikroRath = None
+) -> Optional[List[Optional[Search_image_to_image_modelsQueryOptions]]]:
+    """search_image_to_image_models
+
+
+     options: ImageToImageModel(id, created_by, created_through, kind, data, name, created_at, creator, model_ptr)
+
+
+    Arguments:
+        search (Optional[str], optional): search.
+        rath (mikro.rath.MikroRath, optional): The mikro rath client
+
+    Returns:
+        Optional[List[Optional[Search_image_to_image_modelsQueryImagetoimagemodels]]]"""
+    return execute(
+        Search_image_to_image_modelsQuery, {"search": search}, rath=rath
+    ).image_to_image_models
+
+
 async def aexpand_metric(id: ID, rath: MikroRath = None) -> Optional[MetricFragment]:
     """expand_metric
 
      Creates a new representation
 
     Arguments:
         id (ID): id
```

### Comparing `mikro-0.3.8/mikro/cli/main.py` & `mikro-0.3.9/mikro/cli/main.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.8/mikro/contrib/fakts/datalayer.py` & `mikro-0.3.9/mikro/contrib/fakts/datalayer.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.8/mikro/datalayer.py` & `mikro-0.3.9/mikro/datalayer.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.8/mikro/funcs.py` & `mikro-0.3.9/mikro/funcs.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.8/mikro/links/datalayer.py` & `mikro-0.3.9/mikro/links/datalayer.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.8/mikro/mikro.py` & `mikro-0.3.9/mikro/mikro.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.8/mikro/rath.py` & `mikro-0.3.9/mikro/rath.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.8/mikro/scalars.py` & `mikro-0.3.9/mikro/scalars.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,52 @@
 
     def __repr__(self):
         return f"File({self.value})"
 
 
 
 class ModelFile:
+    """A custom scalar to enable uploading files to the datalayer
+    it enables serialization of everythign
+    """
+
+    __file__ = True
+
+    def __init__(self, value) -> None:
+        self.value = value
+
+
+    @classmethod
+    def __get_validators__(cls):
+        # one or more validators may be yielded which will be called in the
+        # order to validate the input, each validator will receive as an input
+        # the value returned from the previous validator
+
+
+        yield cls.validate
+
+    @classmethod
+    def validate(cls, v):
+        # you could also return a string here which would mean model.post_code
+        # would be a string, pydantic won't care but you could end up with some
+        # confusion since the value's type won't match the type annotation
+        # exactly
+        if isinstance(v, str):
+            return cls(open(v, "rb"))
+        
+
+        return cls(v)
+
+    def __repr__(self):
+        return f"ModelFile({self.value})"
+
+
+
+
+class Model:
     """A custom scalar for ensuring an interface to files api supported by mikro. It converts the graphql value
     (a string pointed to a zarr store) into a downloadable file. To access the file you need to call the download
     method. This is done to avoid unnecessary requests to the datalayer api.
     """
 
     __file__ = True
 
@@ -332,15 +370,11 @@
 
     @classmethod
     def validate(cls, v):
         # you could also return a string here which would mean model.post_code
         # would be a string, pydantic won't care but you could end up with some
         # confusion since the value's type won't match the type annotation
         # exactly
-        if isinstance(v, str):
-            return cls(open(v, "rb"))
-        
-
         return cls(v)
 
     def __repr__(self):
-        return f"ModelFile({self.value})"
+        return f"Model({self.value})"
```

### Comparing `mikro-0.3.8/mikro/structures.py` & `mikro-0.3.9/mikro/structures.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.8/mikro/traits.py` & `mikro-0.3.9/mikro/traits.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.8/mikro/widgets.py` & `mikro-0.3.9/mikro/widgets.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.8/pyproject.toml` & `mikro-0.3.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mikro"
-version = "0.3.8"
+version = "0.3.9"
 description = "images for arkitekt"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "mikro" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `mikro-0.3.8/setup.py` & `mikro-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 extras_require = \
 {'complete:python_version >= "3.9"': ['turms>=0.2.3,<0.3.0'],
  'turms:python_version >= "3.9"': ['turms>=0.2.3,<0.3.0']}
 
 setup_kwargs = {
     'name': 'mikro',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'images for arkitekt',
     'long_description': 'None',
     'author': 'jhnnsrs',
     'author_email': 'jhnnsrs@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mikro-0.3.8/PKG-INFO` & `mikro-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikro
-Version: 0.3.8
+Version: 0.3.9
 Summary: images for arkitekt
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

