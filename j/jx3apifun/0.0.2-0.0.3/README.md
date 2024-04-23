# Comparing `tmp/jx3apifun-0.0.2.tar.gz` & `tmp/jx3apifun-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jx3apifun-0.0.2.tar", last modified: Sun Apr 21 15:22:22 2024, max compression
+gzip compressed data, was "jx3apifun-0.0.3.tar", last modified: Tue Apr 23 17:34:10 2024, max compression
```

## Comparing `jx3apifun-0.0.2.tar` & `jx3apifun-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:22:22.449480 jx3apifun-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-21 15:22:22.449480 jx3apifun-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:22:22.445479 jx3apifun-0.0.2/jx3apifun/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/jx3apifun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/jx3apifun/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/jx3apifun/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28054 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/jx3apifun/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    28431 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/jx3apifun/interface_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/jx3apifun/jx3api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/jx3apifun/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    28662 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/jx3apifun/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/jx3apifun/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:22:22.449480 jx3apifun-0.0.2/jx3apifun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-21 15:22:22.000000 jx3apifun-0.0.2/jx3apifun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-21 15:22:22.000000 jx3apifun-0.0.2/jx3apifun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 15:22:22.000000 jx3apifun-0.0.2/jx3apifun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 15:22:22.000000 jx3apifun-0.0.2/jx3apifun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 15:22:22.449480 jx3apifun-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-21 15:22:13.000000 jx3apifun-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:10.827708 jx3apifun-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-23 17:34:10.827708 jx3apifun-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:10.827708 jx3apifun-0.0.3/jx3apifun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/jx3apifun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/jx3apifun/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/jx3apifun/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28054 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/jx3apifun/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28431 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/jx3apifun/interface_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/jx3apifun/jx3api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/jx3apifun/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28614 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/jx3apifun/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/jx3apifun/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:10.827708 jx3apifun-0.0.3/jx3apifun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-23 17:34:10.000000 jx3apifun-0.0.3/jx3apifun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-23 17:34:10.000000 jx3apifun-0.0.3/jx3apifun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:34:10.000000 jx3apifun-0.0.3/jx3apifun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 17:34:10.000000 jx3apifun-0.0.3/jx3apifun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:34:10.827708 jx3apifun-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-23 17:33:54.000000 jx3apifun-0.0.3/setup.py
```

### Comparing `jx3apifun-0.0.2/LICENSE` & `jx3apifun-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jx3apifun-0.0.2/PKG-INFO` & `jx3apifun-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: jx3apifun
-Version: 0.0.2
+Version: 0.0.3
 Summary: 女生自用jx3api sdk for python
 Home-page: https://github.com/JX3API/jx3api-fun-py
 Author: JustUndertaker
 Author-email: 806792561@qq.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Jx3api for fun
 一款女生自用的jx3api sdk，本仓库主要是为了整活儿，正经使用应该选择受姐姐的[jx3api](https://github.com/JX3API/jx3api-py)。
```

### Comparing `jx3apifun-0.0.2/README.md` & `jx3apifun-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jx3apifun-0.0.2/jx3apifun/__init__.py` & `jx3apifun-0.0.3/jx3apifun/__init__.py`

 * *Files identical despite different names*

### Comparing `jx3apifun-0.0.2/jx3apifun/exceptions.py` & `jx3apifun-0.0.3/jx3apifun/exceptions.py`

 * *Files identical despite different names*

### Comparing `jx3apifun-0.0.2/jx3apifun/interface.py` & `jx3apifun-0.0.3/jx3apifun/interface.py`

 * *Files identical despite different names*

### Comparing `jx3apifun-0.0.2/jx3apifun/interface_async.py` & `jx3apifun-0.0.3/jx3apifun/interface_async.py`

 * *Files identical despite different names*

### Comparing `jx3apifun-0.0.2/jx3apifun/jx3api.py` & `jx3apifun-0.0.3/jx3apifun/jx3api.py`

 * *Files identical despite different names*

### Comparing `jx3apifun-0.0.2/jx3apifun/logger.py` & `jx3apifun-0.0.3/jx3apifun/logger.py`

 * *Files identical despite different names*

### Comparing `jx3apifun-0.0.2/jx3apifun/model.py` & `jx3apifun-0.0.3/jx3apifun/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from typing import Optional, Union
 
-from pydantic import BaseModel, Field
+from msgspec import Struct, field
 
 
-class Request(BaseModel):
+class Request(Struct):
     """
     发送请求模型
     """
 
     name: str
     """请求函数名"""
     url: str
     """请求地址"""
     data: dict
     """请求参数"""
 
 
-class Response(BaseModel):
+class Response(Struct):
     """
     返回值模型
     """
 
     code: int
     """返回码"""
     msg: str
     """返回信息"""
     time: int
     """时间"""
     data: Union[dict, list]
     """返回数据"""
 
 
-class BaseData(BaseModel):
+class BaseData(Struct):
     """
     基础数据模型
     """
 
     ...
 
 
-class DataActiveCalendar(BaseData):
+class DataActiveCalendar(BaseData, kw_only=True):
     """
     日常活动接口返回值模型
     """
 
     date: str
     """日期"""
     week: str
@@ -64,15 +64,15 @@
     """美人画图"""
     luck: list[str]
     """福源"""
     card: list[str]
     """卡牌"""
 
 
-class ToDayData(BaseModel):
+class ToDayData(Struct):
     """
     当天日期
     """
 
     date: str
     """日期"""
     week: str
@@ -138,15 +138,15 @@
     """
     家园花卉接口返回值模型
     """
 
     model_config = {"extra": "allow"}
 
 
-class DataHomeTravel(BaseData):
+class DataHomeTravel(BaseData, kw_only=True):
     """
     家园装饰接口返回值模型
     """
 
     id: int
     """id"""
     name: str
@@ -177,15 +177,15 @@
     """产出"""
     image: str
     """图片"""
     tip: str
     """提示"""
 
 
-class DataAllNews(BaseModel):
+class DataAllNews(Struct):
     """
     单个新闻模型
     """
 
     id: int
     """id"""
     value: int
@@ -196,22 +196,22 @@
     """标题"""
     date: str
     """日期"""
     url: str
     """链接"""
 
 
-class DataSchoolToxic(BaseModel):
+class DataSchoolToxic(Struct):
     """
     单个小药模型
     """
 
     id: int
     """id"""
-    type: str = Field(alias="class")
+    type: str = field(name="class")
     """类型"""
     name: str
     """名称"""
     toxic: str
     """小药名"""
     attribute: str
     """属性"""
@@ -272,15 +272,15 @@
     """区服"""
     server: str
     """服务器"""
     status: str
     """状态"""
 
 
-class DataDetailed(BaseData):
+class DataDetailed(BaseData, kw_only=True):
     """
     更新角色信息
     """
 
     zoneName: str
     """区服名称"""
     serverName: str
@@ -311,15 +311,15 @@
     """人物名称"""
     personId: str
     """人物id"""
     personAvatar: str
     """人物头像"""
 
 
-class OneSchoolMatrixDescs(BaseModel):
+class OneSchoolMatrixDescs(Struct):
     """
     单个职业阵眼描述
     """
 
     desc: str
     """描述"""
     level: int
@@ -337,45 +337,45 @@
     """名称"""
     skillName: str
     """阵法名称"""
     descs: list[OneSchoolMatrixDescs]
     """描述列表"""
 
 
-class OneDataSchoolForceData(BaseModel):
+class OneDataSchoolForceData(Struct):
     """
     单个奇穴数据
     """
 
     name: str
     """名称"""
-    type: int = Field(alias="class")
+    type: int = field(name="class")
     """分类"""
     desc: str
     """描述"""
     icon: str
     """图标"""
     kind: str
     """类型"""
     subKind: str
     """子类型"""
 
 
-class DataSchoolForce(BaseModel):
+class DataSchoolForce(Struct):
     """
     单个门派奇穴
     """
 
     level: int
     """等级"""
     data: list[OneDataSchoolForceData]
     """数据"""
 
 
-class DataSchoolSkillsData(BaseModel):
+class DataSchoolSkillsData(Struct):
     """
     单个门派技能
     """
 
     name: str
     """名称"""
     simpleDesc: str
@@ -403,21 +403,21 @@
 
 
 class DataSchoolSkills(BaseData):
     """
     门派技能
     """
 
-    type: str = Field(alias="class")
+    type: str = field(name="class")
     """分类"""
     data: list[DataSchoolSkillsData]
     """数据"""
 
 
-class DataTiebaRandom(BaseModel):
+class DataTiebaRandom(Struct):
     """
     贴吧帖子
     """
 
     id: int
     """id"""
     subclass: str
@@ -432,15 +432,15 @@
     """标题"""
     url: int
     """链接"""
     date: str
     """日期"""
 
 
-class OneFiveStone(BaseModel):
+class OneFiveStone(Struct):
     """
     五行石数据
     """
 
     name: str
     """名称"""
     level: str
@@ -457,53 +457,53 @@
     """子类型"""
     desc: str
     """描述"""
     percent: bool
     """百分比"""
 
 
-class OneColorStoneAttr(BaseModel):
+class OneColorStoneAttr(Struct):
     """
     五彩石属性
     """
 
     max: str
     """最大值"""
     min: str
     """最小值"""
     desc: str
     """描述"""
     percent: bool
     """百分比"""
 
 
-class ColorStone(BaseModel):
+class ColorStone(Struct):
     """
     五彩石数据
     """
 
     id: str
     """id"""
     name: str
     """名称"""
-    type: str = Field(alias="class")
+    type: str = field(name="class")
     """分类"""
     level: str
     """等级"""
     icon: str
     """图标"""
     kind: str
     """类型"""
     subKind: str
     """子类型"""
     attribute: list[OneColorStoneAttr]
     """属性"""
 
 
-class OneModifyType(BaseModel):
+class OneModifyType(Struct):
     """
     属性类型
     """
 
     name: str
     """名称"""
     max: str
@@ -512,37 +512,37 @@
     """最小值"""
     desc: str
     """描述"""
     percent: bool
     """百分比"""
 
 
-class OnePerManentEnchantAttriDesc(BaseModel):
+class OnePerManentEnchantAttriDesc(Struct):
     """
     附魔属性描述
     """
 
     desc: str
     """描述"""
 
 
-class OnePerManentEnchantAttri(BaseModel):
+class OnePerManentEnchantAttri(Struct):
     """
     附魔属性
     """
 
     max: str
     """最大值"""
     min: str
     """最小值"""
     attrib: list[OnePerManentEnchantAttriDesc]
     """属性描述"""
 
 
-class OnePerManentEnchant(BaseModel):
+class OnePerManentEnchant(Struct):
     """
     附魔数据
     """
 
     id: str
     """id"""
     name: str
@@ -551,15 +551,15 @@
     """等级"""
     icon: str
     """图标"""
     attributes: list[OnePerManentEnchantAttri]
     """属性"""
 
 
-class BaseTypeAttri(BaseModel):
+class BaseTypeAttri(Struct, kw_only=True):
     """
     基础属性
     """
 
     GeneratedBase: str
     """基础属性"""
     GeneratedMagic: str
@@ -570,67 +570,67 @@
     """坐骑魔法属性"""
     Type: Optional[str] = None
     """类型"""
     percent: bool
     """百分比"""
 
 
-class Base1Type(BaseModel):
+class Base1Type(Struct):
     """
     基础属性
     """
 
     Attrib: BaseTypeAttri
     """属性"""
     Base1Max: str
     """最大值"""
     Base1Min: str
     """最小值"""
     Desc: str
     """描述"""
 
 
-class Base2Type(BaseModel):
+class Base2Type(Struct):
     """
     基础属性
     """
 
     Attrib: BaseTypeAttri
     """属性"""
     Base2Max: str
     """最大值"""
     Base2Min: str
     """最小值"""
     Desc: str
     """描述"""
 
 
-class CommonEnchant(BaseModel):
+class CommonEnchant(Struct):
     """
     通用附魔
     """
 
     id: str
     """id"""
     name: str
     """名称"""
     icon: str
     """图标"""
     desc: str
     """描述"""
 
 
-class DataRoleEquip(BaseModel):
+class DataRoleEquip(Struct, kw_only=True):
     """
     装备数据
     """
 
     name: str
     """名称"""
-    type: str = Field(alias="class")
+    type: str = field(name="class")
     """分类"""
     icon: str
     """图标"""
     kind: str
     """类型"""
     subKind: str
     """子类型"""
@@ -658,15 +658,15 @@
     """通用附魔"""
     Base1Type: Base1Type
     """基础属性1"""
     Base2Type: Base2Type
     """基础属性2"""
 
 
-class DataRoleQixue(BaseModel):
+class DataRoleQixue(Struct):
     """
     奇穴数据
     """
 
     name: str
     """名称"""
     level: int
@@ -677,28 +677,28 @@
     """类型"""
     subKind: str
     """子类型"""
     desc: str
     """描述"""
 
 
-class DataRolePanelData(BaseModel):
+class DataRolePanelData(Struct):
     """
     角色面板数据
     """
 
     name: str
     """名称"""
     percent: bool
     """百分比"""
     value: Union[int, float]
     """数值"""
 
 
-class DataRolePanel(BaseModel):
+class DataRolePanel(Struct):
     """
     角色面板
     """
 
     score: int
     """评分"""
     panel: list[DataRolePanelData]
@@ -714,15 +714,15 @@
     """装备列表"""
     qixueList: list[DataRoleQixue]
     """奇穴列表"""
     panelList: DataRolePanel
     """面板数据"""
 
 
-class BossProgress(BaseModel):
+class BossProgress(Struct):
     """
     Boss进度
     """
 
     finished: bool
     """是否完成"""
     icon: str
@@ -731,15 +731,15 @@
     """序号"""
     name: str
     """名称"""
     progressId: str
     """进度id"""
 
 
-class OneTeamMapData(BaseModel):
+class OneTeamMapData(Struct):
     """
     单个副本数据
     """
 
     mapIcon: str
     """地图图标"""
     mapId: str
@@ -803,54 +803,54 @@
     """奇遇名"""
     status: int
     """状态"""
     time: int
     """时间"""
 
 
-class DataLuckCollectData(BaseModel):
+class DataLuckCollectData(Struct):
     """
     奇遇汇总数据
     """
 
     name: str
     """触发人"""
     time: int
     """触发时间"""
 
 
-class DataLuckCollect(BaseModel):
+class DataLuckCollect(Struct):
     """
     单个奇遇汇总
     """
 
     server: str
     """服务器"""
     event: str
     """奇遇名"""
     count: int
     """数量"""
     data: DataLuckCollectData
     """数据"""
 
 
-class DataRoleAchievementData(BaseModel):
+class DataRoleAchievementData(Struct, kw_only=True):
     """
     角色成就数据
     """
 
     id: int
     """id"""
     icon: str
     """图标"""
     likes: int
     """点赞数"""
     name: str
     """奇遇名称"""
-    upClass: str = Field(alias="class")
+    upClass: str = field(name="class")
     """类型"""
     subClass: str
     """子类型"""
     desc: str
     """描述"""
     detail: str
     """详情"""
@@ -883,15 +883,15 @@
     角色成就进度
     """
 
     data: list[DataRoleAchievementData]
     """成就列表"""
 
 
-class OneDataMatchPerformance(BaseModel):
+class OneDataMatchPerformance(Struct):
     """
     战绩表现
     """
 
     mmr: int
     """MMR"""
     grade: int
@@ -906,28 +906,28 @@
     """MVP次数"""
     pvpType: str
     """PVP类型"""
     winRate: int
     """胜率"""
 
 
-class DataMatchPerformance(BaseModel):
+class DataMatchPerformance(Struct):
     """
     战绩表现
     """
 
-    match22: Optional[OneDataMatchPerformance] = Field(alias="2v2", default=None)
+    match22: Optional[OneDataMatchPerformance] = field(name="2v2", default=None)
     """2v2表现"""
-    match33: Optional[OneDataMatchPerformance] = Field(alias="3v3", default=None)
+    match33: Optional[OneDataMatchPerformance] = field(name="3v3", default=None)
     """3v3表现"""
-    match55: Optional[OneDataMatchPerformance] = Field(alias="5v5", default=None)
+    match55: Optional[OneDataMatchPerformance] = field(name="5v5", default=None)
     """5v5表现"""
 
 
-class DataMatchHistory(BaseModel):
+class DataMatchHistory(Struct):
     """
     战绩历史
     """
 
     zone: str
     """区服"""
     server: str
@@ -948,15 +948,15 @@
     """是否MVP"""
     startTime: int
     """开始时间"""
     endTime: int
     """结束时间"""
 
 
-class DataMatchTrend(BaseModel):
+class DataMatchTrend(Struct):
     """
     战绩走势
     """
 
     matchDate: int
     """比赛日期"""
     mmr: int
@@ -999,28 +999,28 @@
     """分数"""
     upNum: str
     """上升名次"""
     winRate: str
     """胜率"""
 
 
-class DataMatchSchools(BaseModel):
+class DataMatchSchools(Struct):
     """
     名剑统计
     """
 
     name: str
     """门派名称"""
     this: int
     """当前排名"""
     last: int
     """上次排名"""
 
 
-class DataMemberRecruitData(BaseModel):
+class DataMemberRecruitData(Struct):
     """
     团队招募信息
     """
 
     crossServer: bool
     """是否跨服"""
     activityId: int
@@ -1060,15 +1060,15 @@
     """服务器"""
     data: list[DataMemberRecruitData]
     """招募信息"""
     time: int
     """时间"""
 
 
-class DataMemberData(BaseModel):
+class DataMemberData(Struct, kw_only=True):
     """
     师徒列表数据
     """
 
     roleId: int
     """角色id"""
     roleName: str
@@ -1104,15 +1104,15 @@
     """区服"""
     server: str
     """服务器"""
     data: list[DataMemberData]
     """师徒列表"""
 
 
-class OneDataServerSand(BaseModel):
+class OneDataServerSand(Struct):
     """
     服务器沙盘数据
     """
 
     tongId: int
     """帮派id"""
     tongName: str
@@ -1144,15 +1144,15 @@
     """重置时间"""
     update: int
     """更新时间"""
     data: list[OneDataServerSand]
     """沙盘数据"""
 
 
-class DataServerEvent(BaseModel):
+class DataServerEvent(Struct):
     """
     全服阵营大事件
     """
 
     id: int
     """id"""
     camp_name: str
@@ -1167,15 +1167,15 @@
     """友方服务器名"""
     role_name: str
     """角色名"""
     add_time: int
     """添加时间"""
 
 
-class DataTradeDemon(BaseModel):
+class DataTradeDemon(Struct):
     """
     金价比例数据
     """
 
     id: int
     """id"""
     zone: str
@@ -1186,34 +1186,34 @@
     """贴吧数据"""
     wanbaolou: str
     """万宝楼数据"""
     dd373: str
     """373数据"""
     uu898: str
     """898数据"""
-    from_5173: str = Field(alias="5173")
+    from_5173: str = field(name="5173")
     """5173数据"""
-    from_7881: str = Field(alias="7881")
+    from_7881: str = field(name="7881")
     """7881数据"""
     time: int
     """时间"""
     date: str
     """日期"""
 
 
-class DataTradeRecordData(BaseModel):
+class DataTradeRecordData(Struct):
     """
     物价数据
     """
 
     id: int
     """id"""
     index: int
     """序号"""
-    type: str = Field(alias="class")
+    type: str = field(name="class")
     """类型"""
     zone: str
     """区服"""
     server: str
     """服务器"""
     value: int
     """价格"""
@@ -1227,30 +1227,30 @@
     """日期"""
     status: int
     """状态"""
     datetime: str
     """时间"""
 
 
-class DataTradeRecord(BaseData):
+class DataTradeRecord(BaseData, kw_only=True):
     """
     物价记录
     """
 
     id: int
     """id"""
-    type: str = Field(alias="class")
+    type: str = field(name="class")
     """类型"""
     subclass: str
     """子类别"""
     name: str
     """名称"""
-    alias: str
+    name: str
     """别名"""
-    subalias: str
+    subname: Optional[str] = None
     """子别名"""
     row: str
     """行"""
     level: int
     """等级"""
     desc: str
     """描述"""
@@ -1258,15 +1258,15 @@
     """图片"""
     date: str
     """日期"""
     data: list[list[DataTradeRecordData]]
     """数据"""
 
 
-class DataTieBaItemRecords(BaseModel):
+class DataTieBaItemRecords(Struct):
     """
     贴吧物品记录
     """
 
     id: int
     """id"""
     zone: str
@@ -1285,15 +1285,15 @@
     """token"""
     floor: int
     """楼层"""
     time: int
     """时间"""
 
 
-class DataValuablesStatistical(BaseModel):
+class DataValuablesStatistical(Struct):
     """
     物品统计
     """
 
     id: int
     """id"""
     zone: str
@@ -1306,28 +1306,28 @@
     """角色名"""
     map_name: str
     """地图名"""
     time: int
     """时间"""
 
 
-class DataValuablesCollect(BaseModel):
+class DataValuablesCollect(Struct):
     """
     掉落汇总数据
     """
 
     name: str
     """名称"""
     count: int
     """数量"""
     data: DataValuablesStatistical
     """数据"""
 
 
-class DataServerAntivice(BaseModel):
+class DataServerAntivice(Struct):
     """
     诛恶事件数据
     """
 
     id: int
     """id"""
     zone: str
@@ -1336,22 +1336,22 @@
     """服务器"""
     map_name: str
     """地图名"""
     time: int
     """时间"""
 
 
-class DataRankStatistical(BaseModel):
+class DataRankStatistical(Struct, kw_only=True):
     """
     风云榜单数据
     """
 
     id: int
     """id"""
-    type: str = Field(alias="class")
+    type: str = field(name="class")
     """类型"""
     zone: str
     """区服"""
     server: str
     """服务器"""
     name: str
     """名称"""
@@ -1367,15 +1367,15 @@
     """帮派"""
     score: int
     """分数"""
     datetime: str
     """时间"""
 
 
-class DataSchoolRankStatistical(BaseModel):
+class DataSchoolRankStatistical(Struct):
     """
     资历榜单数据
     """
 
     name: str
     """名称"""
     role: str
@@ -1388,15 +1388,15 @@
     """区服"""
     value: int
     """值"""
     avatar: str
     """头像"""
 
 
-class DataDuowanStatisticalData(BaseModel):
+class DataDuowanStatisticalData(Struct):
     """
     单个频道数据
     """
 
     campName: str
     """阵营名"""
     sid: int
@@ -1435,15 +1435,15 @@
     """名称"""
     list: list[str]
     """技能列表"""
     desc: str
     """描述"""
 
 
-class DataActiveMonsterData(BaseModel):
+class DataActiveMonsterData(Struct):
     """
     百战数据
     """
 
     index: int
     """序号"""
     name: str
@@ -1461,15 +1461,15 @@
     """开始时间"""
     end: int
     """结束时间"""
     data: list[DataActiveMonsterData]
     """数据"""
 
 
-class DataHorseRecord(BaseModel):
+class DataHorseRecord(Struct):
     """
     的卢记录
     """
 
     id: int
     """id"""
     zone: str
@@ -1500,24 +1500,24 @@
     """拍卖金额"""
     start_time: int
     """开始时间"""
     end_time: int
     """结束时间"""
 
 
-class DataHorseData(BaseModel):
+class DataHorseData(Struct):
     """
     马场事件数据
     """
 
-    yinshan: list[str] = Field(alias="阴山大草原")
+    yinshan: list[str] = field(name="阴山大草原")
     """阴山大草原"""
-    kunpengdao: list[str] = Field(alias="鲲鹏岛")
+    kunpengdao: list[str] = field(name="鲲鹏岛")
     """鲲鹏岛"""
-    heigebi: list[str] = Field(alias="黑戈壁")
+    heigebi: list[str] = field(name="黑戈壁")
     """黑戈壁"""
 
 
 class DataHorseEvent(BaseData):
     """
     马场事件
     """
@@ -1643,30 +1643,30 @@
     """歌手名"""
     PlayUrl: str
     """播放链接"""
     Img: str
     """图片"""
 
 
-class DataFraudTiebaData(BaseModel):
+class DataFraudTiebaData(Struct):
     """
     贴吧详情
     """
 
     title: str
     """标题"""
     tid: int
     """贴吧帖子id"""
     text: str
     """内容"""
     time: int
     """时间"""
 
 
-class DataFraudRecord(BaseModel):
+class DataFraudRecord(Struct):
     """
     骗子记录
     """
 
     server: str
     """区服"""
     tieba: str
@@ -1680,15 +1680,15 @@
     骗子记录
     """
 
     records: list[DataFraudRecord]
     """记录"""
 
 
-class DataIdiomSolitaireData(BaseModel):
+class DataIdiomSolitaireData(Struct):
     """
     成语接龙记录
     """
 
     id: int
     """id"""
     name: str
@@ -1742,15 +1742,15 @@
     """文本"""
     token: str
     """token"""
     url: str
     """链接"""
 
 
-class DataRoleMonsterSkill(BaseModel):
+class DataRoleMonsterSkill(Struct):
     """
     个人百战技能
     """
 
     bDeprecated: bool
     """是否过期"""
     dwInSkillID: int
```

### Comparing `jx3apifun-0.0.2/jx3apifun/permission.py` & `jx3apifun-0.0.3/jx3apifun/permission.py`

 * *Files identical despite different names*

### Comparing `jx3apifun-0.0.2/jx3apifun.egg-info/PKG-INFO` & `jx3apifun-0.0.3/jx3apifun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: jx3apifun
-Version: 0.0.2
+Version: 0.0.3
 Summary: 女生自用jx3api sdk for python
 Home-page: https://github.com/JX3API/jx3api-fun-py
 Author: JustUndertaker
 Author-email: 806792561@qq.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Jx3api for fun
 一款女生自用的jx3api sdk，本仓库主要是为了整活儿，正经使用应该选择受姐姐的[jx3api](https://github.com/JX3API/jx3api-py)。
```

### Comparing `jx3apifun-0.0.2/setup.py` & `jx3apifun-0.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jx3apifun",
-    version="0.0.2",
+    version="0.0.3",
     author="JustUndertaker",
     author_email="806792561@qq.com",
     description="女生自用jx3api sdk for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JX3API/jx3api-fun-py",
     packages=["jx3apifun"],
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ],
     python_requires=">=3.9",
 )
```

