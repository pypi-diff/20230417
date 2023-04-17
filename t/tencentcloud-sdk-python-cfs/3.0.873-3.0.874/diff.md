# Comparing `tmp/tencentcloud-sdk-python-cfs-3.0.873.tar.gz` & `tmp/tencentcloud-sdk-python-cfs-3.0.874.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.873.tar", last modified: Fri Apr 14 00:24:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.874.tar", last modified: Mon Apr 17 00:24:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfs-3.0.873.tar` & `tencentcloud-sdk-python-cfs-3.0.874.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/cfs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)    13386 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    33132 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/cfs/v20190719/cfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95368 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/cfs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud_sdk_python_cfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 00:24:31.000000 tencentcloud-sdk-python-cfs-3.0.873/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/cfs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)    13561 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    37934 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112598 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/cfs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud_sdk_python_cfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:24:09.000000 tencentcloud-sdk-python-cfs-3.0.874/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.873/README.rst` & `tencentcloud-sdk-python-cfs-3.0.874/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,23 @@
 
 # 该地域无法提供服务。
 INVALIDPARAMETERVALUE_UNAVAILABLEZONE = 'InvalidParameterValue.UnavailableZone'
 
 # ZoneId和Region不匹配。
 INVALIDPARAMETERVALUE_ZONEIDREGIONNOTMATCH = 'InvalidParameterValue.ZoneIdRegionNotMatch'
 
+# 缺少参数错误。
+MISSINGPARAMETER = 'MissingParameter'
+
+# 操作被拒绝。
+OPERATIONDENIED = 'OperationDenied'
+
+# 资源被占用。
+RESOURCEINUSE = 'ResourceInUse'
+
 # 文件系统数量达到上限。
 RESOURCEINSUFFICIENT_FILESYSTEMLIMITEXCEEDED = 'ResourceInsufficient.FileSystemLimitExceeded'
 
 # 权限组数量达到上限。
 RESOURCEINSUFFICIENT_PGROUPNUMBERLIMITEXCEEDED = 'ResourceInsufficient.PgroupNumberLimitExceeded'
 
 # 区域资源售罄。
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -160,14 +160,38 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateMigrationTask(self, request):
+        """用于创建迁移任务。
+        此接口需提交工单，开启白名单之后才能使用。
+
+        :param request: Request instance for CreateMigrationTask.
+        :type request: :class:`tencentcloud.cfs.v20190719.models.CreateMigrationTaskRequest`
+        :rtype: :class:`tencentcloud.cfs.v20190719.models.CreateMigrationTaskResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateMigrationTask", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateMigrationTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteAutoSnapshotPolicy(self, request):
         """删除快照定期策略
 
         :param request: Request instance for DeleteAutoSnapshotPolicy.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DeleteAutoSnapshotPolicyRequest`
         :rtype: :class:`tencentcloud.cfs.v20190719.models.DeleteAutoSnapshotPolicyResponse`
 
@@ -275,14 +299,38 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteMigrationTask(self, request):
+        """用于删除迁移任务。
+        此接口需提交工单，开启白名单之后才能使用。
+
+        :param request: Request instance for DeleteMigrationTask.
+        :type request: :class:`tencentcloud.cfs.v20190719.models.DeleteMigrationTaskRequest`
+        :rtype: :class:`tencentcloud.cfs.v20190719.models.DeleteMigrationTaskResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteMigrationTask", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteMigrationTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteMountTarget(self, request):
         """本接口（DeleteMountTarget）用于删除挂载点
 
         :param request: Request instance for DeleteMountTarget.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DeleteMountTargetRequest`
         :rtype: :class:`tencentcloud.cfs.v20190719.models.DeleteMountTargetResponse`
 
@@ -367,14 +415,38 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeBucketList(self, request):
+        """用于获取数据源桶列表。
+        此接口需提交工单，开启白名单之后才能使用。
+
+        :param request: Request instance for DescribeBucketList.
+        :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeBucketListRequest`
+        :rtype: :class:`tencentcloud.cfs.v20190719.models.DescribeBucketListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeBucketList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeBucketListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeCfsFileSystemClients(self, request):
         """查询挂载该文件系统的客户端。此功能需要客户端安装CFS监控插件。
 
         :param request: Request instance for DescribeCfsFileSystemClients.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeCfsFileSystemClientsRequest`
         :rtype: :class:`tencentcloud.cfs.v20190719.models.DescribeCfsFileSystemClientsResponse`
 
@@ -528,14 +600,38 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeMigrationTasks(self, request):
+        """用于获取迁移任务列表。
+        此接口需提交工单，开启白名单之后才能使用。
+
+        :param request: Request instance for DescribeMigrationTasks.
+        :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeMigrationTasksRequest`
+        :rtype: :class:`tencentcloud.cfs.v20190719.models.DescribeMigrationTasksResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeMigrationTasks", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeMigrationTasksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeMountTargets(self, request):
         """本接口（DescribeMountTargets）用于查询文件系统挂载点信息
 
         :param request: Request instance for DescribeMountTargets.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeMountTargetsRequest`
         :rtype: :class:`tencentcloud.cfs.v20190719.models.DescribeMountTargetsResponse`
 
@@ -641,14 +737,38 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def StopMigrationTask(self, request):
+        """用于终止迁移任务。
+        此接口需提交工单，开启白名单之后才能使用。
+
+        :param request: Request instance for StopMigrationTask.
+        :type request: :class:`tencentcloud.cfs.v20190719.models.StopMigrationTaskRequest`
+        :rtype: :class:`tencentcloud.cfs.v20190719.models.StopMigrationTaskResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StopMigrationTask", params, headers=headers)
+            response = json.loads(body)
+            model = models.StopMigrationTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def UnbindAutoSnapshotPolicy(self, request):
         """解除文件系统绑定的快照策略
 
         :param request: Request instance for UnbindAutoSnapshotPolicy.
         :type request: :class:`tencentcloud.cfs.v20190719.models.UnbindAutoSnapshotPolicyRequest`
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/cfs/v20190719/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -305,14 +305,43 @@
 
 
     def _deserialize(self, params):
         self.AutoSnapshotPolicyId = params.get("AutoSnapshotPolicyId")
         self.RequestId = params.get("RequestId")
 
 
+class BucketInfo(AbstractModel):
+    """对象存储桶
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 桶名称
+        :type Name: str
+        :param Region: 桶所在地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        """
+        self.Name = None
+        self.Region = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Region = params.get("Region")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CreateAutoSnapshotPolicyRequest(AbstractModel):
     """CreateAutoSnapshotPolicy请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -704,14 +733,115 @@
 
 
     def _deserialize(self, params):
         self.SnapshotId = params.get("SnapshotId")
         self.RequestId = params.get("RequestId")
 
 
+class CreateMigrationTaskRequest(AbstractModel):
+    """CreateMigrationTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskName: 迁移任务名称
+        :type TaskName: str
+        :param MigrationType: 迁移方式标志位，默认为0。0: 桶迁移；1: 清单迁移
+        :type MigrationType: int
+        :param MigrationMode: 迁移模式，默认为0。0: 全量迁移
+        :type MigrationMode: int
+        :param SrcSecretId: 数据源账号的SecretId
+        :type SrcSecretId: str
+        :param SrcSecretKey: 数据源账号的SecretKey
+        :type SrcSecretKey: str
+        :param FileSystemId: 文件系统实例Id
+        :type FileSystemId: str
+        :param FsPath: 文件系统路径
+        :type FsPath: str
+        :param CoverType: 同名文件迁移时覆盖策略，默认为0。0: 最后修改时间优先；1: 全覆盖；2: 不覆盖
+        :type CoverType: int
+        :param SrcService: 数据源服务商。COS: 腾讯云COS，OSS: 阿里云OSS，OBS:华为云OBS
+        :type SrcService: str
+        :param BucketName: 数据源桶名称，名称和地址至少有一个
+        :type BucketName: str
+        :param BucketRegion: 数据源桶地域
+        :type BucketRegion: str
+        :param BucketAddress: 数据源桶地址，名称和地址至少有一个
+        :type BucketAddress: str
+        :param ListAddress: 清单地址，迁移方式为清单迁移时必填
+        :type ListAddress: str
+        :param FsName: 目标文件系统名称
+        :type FsName: str
+        :param BucketPath: 源桶路径，默认为/
+        :type BucketPath: str
+        """
+        self.TaskName = None
+        self.MigrationType = None
+        self.MigrationMode = None
+        self.SrcSecretId = None
+        self.SrcSecretKey = None
+        self.FileSystemId = None
+        self.FsPath = None
+        self.CoverType = None
+        self.SrcService = None
+        self.BucketName = None
+        self.BucketRegion = None
+        self.BucketAddress = None
+        self.ListAddress = None
+        self.FsName = None
+        self.BucketPath = None
+
+
+    def _deserialize(self, params):
+        self.TaskName = params.get("TaskName")
+        self.MigrationType = params.get("MigrationType")
+        self.MigrationMode = params.get("MigrationMode")
+        self.SrcSecretId = params.get("SrcSecretId")
+        self.SrcSecretKey = params.get("SrcSecretKey")
+        self.FileSystemId = params.get("FileSystemId")
+        self.FsPath = params.get("FsPath")
+        self.CoverType = params.get("CoverType")
+        self.SrcService = params.get("SrcService")
+        self.BucketName = params.get("BucketName")
+        self.BucketRegion = params.get("BucketRegion")
+        self.BucketAddress = params.get("BucketAddress")
+        self.ListAddress = params.get("ListAddress")
+        self.FsName = params.get("FsName")
+        self.BucketPath = params.get("BucketPath")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateMigrationTaskResponse(AbstractModel):
+    """CreateMigrationTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 迁移任务Id
+        :type TaskId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteAutoSnapshotPolicyRequest(AbstractModel):
     """DeleteAutoSnapshotPolicy请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -941,14 +1071,55 @@
 
 
     def _deserialize(self, params):
         self.SnapshotId = params.get("SnapshotId")
         self.RequestId = params.get("RequestId")
 
 
+class DeleteMigrationTaskRequest(AbstractModel):
+    """DeleteMigrationTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 迁移任务ID
+        :type TaskId: str
+        """
+        self.TaskId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteMigrationTaskResponse(AbstractModel):
+    """DeleteMigrationTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteMountTargetRequest(AbstractModel):
     """DeleteMountTarget请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1146,14 +1317,77 @@
             for item in params.get("RegionZones"):
                 obj = AvailableRegion()
                 obj._deserialize(item)
                 self.RegionZones.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeBucketListRequest(AbstractModel):
+    """DescribeBucketList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SrcService: 数据源服务商。COS: 腾讯云COS，OSS: 阿里云OSS，OBS:华为云OBS
+        :type SrcService: str
+        :param SrcSecretId: 数据源账号的SecretId
+
+        :type SrcSecretId: str
+        :param SrcSecretKey: 数据源账号的SecretKey
+        :type SrcSecretKey: str
+        """
+        self.SrcService = None
+        self.SrcSecretId = None
+        self.SrcSecretKey = None
+
+
+    def _deserialize(self, params):
+        self.SrcService = params.get("SrcService")
+        self.SrcSecretId = params.get("SrcSecretId")
+        self.SrcSecretKey = params.get("SrcSecretKey")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeBucketListResponse(AbstractModel):
+    """DescribeBucketList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 桶的数量
+        :type TotalCount: int
+        :param BucketList: 桶列表
+        :type BucketList: list of BucketInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.BucketList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("BucketList") is not None:
+            self.BucketList = []
+            for item in params.get("BucketList"):
+                obj = BucketInfo()
+                obj._deserialize(item)
+                self.BucketList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeCfsFileSystemClientsRequest(AbstractModel):
     """DescribeCfsFileSystemClients请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1486,14 +1720,95 @@
                 obj = SnapshotInfo()
                 obj._deserialize(item)
                 self.Snapshots.append(obj)
         self.TotalSize = params.get("TotalSize")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeMigrationTasksRequest(AbstractModel):
+    """DescribeMigrationTasks请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Offset: 分页的偏移量，默认值为0。
+        :type Offset: int
+        :param Limit: 分页单页限制数目，默认值为20，最大值100。
+        :type Limit: int
+        :param Filters: <br><li> taskId
+
+按照【迁移任务id】进行过滤。
+类型：String
+
+必选：否
+
+<br><li> taskName
+
+按照【迁移任务名字】进行模糊搜索过滤。
+类型：String
+
+必选：否
+
+每次请求的Filters的上限为10，Filter.Values的上限为100。
+        :type Filters: list of Filter
+        """
+        self.Offset = None
+        self.Limit = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeMigrationTasksResponse(AbstractModel):
+    """DescribeMigrationTasks返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 迁移任务的数量
+        :type TotalCount: int
+        :param MigrationTasks: 迁移任务详情
+        :type MigrationTasks: list of MigrationTaskInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.MigrationTasks = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("MigrationTasks") is not None:
+            self.MigrationTasks = []
+            for item in params.get("MigrationTasks"):
+                obj = MigrationTaskInfo()
+                obj._deserialize(item)
+                self.MigrationTasks.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeMountTargetsRequest(AbstractModel):
     """DescribeMountTargets请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1919,14 +2234,150 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class MigrationTaskInfo(AbstractModel):
+    """CFS数据迁移任务信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskName: 迁移任务名称
+        :type TaskName: str
+        :param TaskId: 迁移任务id
+        :type TaskId: str
+        :param MigrationType: 迁移方式标志位，默认为0。0: 桶迁移；1: 清单迁移
+        :type MigrationType: int
+        :param MigrationMode: 迁移模式，默认为0。0: 全量迁移
+        :type MigrationMode: int
+        :param BucketName: 数据源桶名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BucketName: str
+        :param BucketRegion: 数据源桶地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BucketRegion: str
+        :param BucketAddress: 数据源桶地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BucketAddress: str
+        :param ListAddress: 清单地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ListAddress: str
+        :param FsName: 文件系统实例名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FsName: str
+        :param FileSystemId: 文件系统实例Id
+        :type FileSystemId: str
+        :param FsPath: 文件系统路径
+        :type FsPath: str
+        :param CoverType: 同名文件迁移时覆盖策略，默认为0。0: 最后修改时间优先；1: 全覆盖；2: 不覆盖
+        :type CoverType: int
+        :param CreateTime: 创建时间
+        :type CreateTime: int
+        :param EndTime: 完成/终止时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EndTime: int
+        :param Status: 迁移状态。0: 已完成；1: 进行中；2: 已终止
+        :type Status: int
+        :param FileTotalCount: 文件数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileTotalCount: int
+        :param FileMigratedCount: 已迁移文件数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileMigratedCount: int
+        :param FileFailedCount: 迁移失败文件数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileFailedCount: int
+        :param FileTotalSize: 文件容量，单位Byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileTotalSize: int
+        :param FileMigratedSize: 已迁移文件容量，单位Byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileMigratedSize: int
+        :param FileFailedSize: 迁移失败文件容量，单位Byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileFailedSize: int
+        :param FileTotalList: 全部清单
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileTotalList: str
+        :param FileCompletedList: 已完成文件清单
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileCompletedList: str
+        :param FileFailedList: 失败文件清单
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileFailedList: str
+        :param BucketPath: 源桶路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BucketPath: str
+        """
+        self.TaskName = None
+        self.TaskId = None
+        self.MigrationType = None
+        self.MigrationMode = None
+        self.BucketName = None
+        self.BucketRegion = None
+        self.BucketAddress = None
+        self.ListAddress = None
+        self.FsName = None
+        self.FileSystemId = None
+        self.FsPath = None
+        self.CoverType = None
+        self.CreateTime = None
+        self.EndTime = None
+        self.Status = None
+        self.FileTotalCount = None
+        self.FileMigratedCount = None
+        self.FileFailedCount = None
+        self.FileTotalSize = None
+        self.FileMigratedSize = None
+        self.FileFailedSize = None
+        self.FileTotalList = None
+        self.FileCompletedList = None
+        self.FileFailedList = None
+        self.BucketPath = None
+
+
+    def _deserialize(self, params):
+        self.TaskName = params.get("TaskName")
+        self.TaskId = params.get("TaskId")
+        self.MigrationType = params.get("MigrationType")
+        self.MigrationMode = params.get("MigrationMode")
+        self.BucketName = params.get("BucketName")
+        self.BucketRegion = params.get("BucketRegion")
+        self.BucketAddress = params.get("BucketAddress")
+        self.ListAddress = params.get("ListAddress")
+        self.FsName = params.get("FsName")
+        self.FileSystemId = params.get("FileSystemId")
+        self.FsPath = params.get("FsPath")
+        self.CoverType = params.get("CoverType")
+        self.CreateTime = params.get("CreateTime")
+        self.EndTime = params.get("EndTime")
+        self.Status = params.get("Status")
+        self.FileTotalCount = params.get("FileTotalCount")
+        self.FileMigratedCount = params.get("FileMigratedCount")
+        self.FileFailedCount = params.get("FileFailedCount")
+        self.FileTotalSize = params.get("FileTotalSize")
+        self.FileMigratedSize = params.get("FileMigratedSize")
+        self.FileFailedSize = params.get("FileFailedSize")
+        self.FileTotalList = params.get("FileTotalList")
+        self.FileCompletedList = params.get("FileCompletedList")
+        self.FileFailedList = params.get("FileFailedList")
+        self.BucketPath = params.get("BucketPath")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class MountInfo(AbstractModel):
     """挂载点信息
 
     """
 
     def __init__(self):
         r"""
@@ -2328,14 +2779,63 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class StopMigrationTaskRequest(AbstractModel):
+    """StopMigrationTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 迁移任务名称
+        :type TaskId: str
+        """
+        self.TaskId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class StopMigrationTaskResponse(AbstractModel):
+    """StopMigrationTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 迁移任务Id
+        :type TaskId: str
+        :param Status: 迁移状态。0: 已完成；1: 进行中；2: 已终止
+        :type Status: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskId = None
+        self.Status = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.Status = params.get("Status")
+        self.RequestId = params.get("RequestId")
+
+
 class TagInfo(AbstractModel):
     """Tag信息单元
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.873/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfs-3.0.874/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.873'
+__version__ = '3.0.874'
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.873/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.874/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.873/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.874/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.873/setup.py` & `tencentcloud-sdk-python-cfs-3.0.874/setup.py`

 * *Files identical despite different names*

