# Comparing `tmp/tencentcloud-sdk-python-faceid-3.0.873.tar.gz` & `tmp/tencentcloud-sdk-python-faceid-3.0.874.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.873.tar", last modified: Fri Apr 14 00:37:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.874.tar", last modified: Mon Apr 17 00:30:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-faceid-3.0.873.tar` & `tencentcloud-sdk-python-faceid-3.0.874.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/
--rw-r--r--   0 root         (0) root         (0)      746 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/faceid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)    34030 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/faceid/v20180301/faceid_client.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)   139760 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/faceid/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud_sdk_python_faceid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 00:37:28.000000 tencentcloud-sdk-python-faceid-3.0.873/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/faceid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)    34030 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/faceid/v20180301/faceid_client.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   141050 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/faceid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud_sdk_python_faceid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:30:12.000000 tencentcloud-sdk-python-faceid-3.0.874/setup.cfg
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.873/README.rst` & `tencentcloud-sdk-python-faceid-3.0.874/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/faceid/v20180301/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2440,18 +2440,39 @@
 class IntentionQuestionResult(AbstractModel):
     """意愿核身问答模式结果
 
     """
 
     def __init__(self):
         r"""
-        :param FinalResultCode: 意愿核身最终结果：
-0：认证通过，-1：认证未通过，-2：浏览器内核不兼容，无法进行意愿校验
+        :param FinalResultDetailCode: 意愿核身错误码：
+0: "成功"       
+-1: "参数错误"    
+-2: "系统异常"    
+-101: "请保持人脸在框内"    
+-102: "检测到多张人脸"   
+-103: "人脸检测失败"   
+-104: "人脸检测不完整"   
+-105: "请勿遮挡眼睛"    
+-106: "请勿遮挡嘴巴"     
+-107: "请勿遮挡鼻子"     
+-201: "人脸比对相似度低"    
+-202: "人脸比对失败"    
+-301: "意愿核验不通过"   
+-800: "前端不兼容错误"    
+-801: "用户未授权摄像头和麦克风权限"   
+-802: "获取视频流失败"   
+-803: "用户主动关闭链接/异常断开链接"   
+-998: "系统数据异常"   
+-999: "系统未知错误，请联系人工核实"   
 注意：此字段可能返回 null，表示取不到有效值。
-        :type FinalResultCode: str
+        :type FinalResultDetailCode: int
+        :param FinalResultMessage: 意愿核身错误信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinalResultMessage: str
         :param Video: 视频base64（其中包含全程问题和回答音频，mp4格式）
 注意：此字段可能返回 null，表示取不到有效值。
         :type Video: str
         :param ScreenShot: 屏幕截图base64列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type ScreenShot: list of str
         :param ResultCode: 和答案匹配结果列表
@@ -2460,30 +2481,38 @@
         :type ResultCode: list of str
         :param AsrResult: 回答问题语音识别结果列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type AsrResult: list of str
         :param Audios: 答案录音音频
 注意：此字段可能返回 null，表示取不到有效值。
         :type Audios: list of str
+        :param FinalResultCode: 意愿核身最终结果：
+0：认证通过，-1：认证未通过，-2：浏览器内核不兼容，无法进行意愿校验。建议使用“FinalResultDetailCode”参数获取详细的错误码信息。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinalResultCode: str
         """
-        self.FinalResultCode = None
+        self.FinalResultDetailCode = None
+        self.FinalResultMessage = None
         self.Video = None
         self.ScreenShot = None
         self.ResultCode = None
         self.AsrResult = None
         self.Audios = None
+        self.FinalResultCode = None
 
 
     def _deserialize(self, params):
-        self.FinalResultCode = params.get("FinalResultCode")
+        self.FinalResultDetailCode = params.get("FinalResultDetailCode")
+        self.FinalResultMessage = params.get("FinalResultMessage")
         self.Video = params.get("Video")
         self.ScreenShot = params.get("ScreenShot")
         self.ResultCode = params.get("ResultCode")
         self.AsrResult = params.get("AsrResult")
         self.Audios = params.get("Audios")
+        self.FinalResultCode = params.get("FinalResultCode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.873/tencentcloud/__init__.py` & `tencentcloud-sdk-python-faceid-3.0.874/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-faceid-3.0.873/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.874/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.873/setup.py` & `tencentcloud-sdk-python-faceid-3.0.874/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.873/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.874/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

