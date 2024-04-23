# Comparing `tmp/gd_excelexporter-3.0.0a1.tar.gz` & `tmp/gd_excelexporter-3.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gd_excelexporter-3.0.0a1.tar", max compression
+gzip compressed data, was "gd_excelexporter-3.0.1a0.tar", max compression
```

## Comparing `gd_excelexporter-3.0.0a1.tar` & `gd_excelexporter-3.0.1a0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1065 2024-04-19 01:40:07.975489 gd_excelexporter-3.0.0a1/LICENSE
--rw-r--r--   0        0        0    11006 2024-04-19 01:40:07.975489 gd_excelexporter-3.0.0a1/README.md
--rw-r--r--   0        0        0     2696 2024-04-19 01:40:27.891445 gd_excelexporter-3.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      132 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/__init__.py
--rw-r--r--   0        0        0      212 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/__main__.py
--rw-r--r--   0        0        0        0 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/__init__.py
--rw-r--r--   0        0        0     3338 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/csharp.py
--rw-r--r--   0        0        0     8496 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/godot.py
--rw-r--r--   0        0        0     4237 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/json.py
--rw-r--r--   0        0        0     4427 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/cli.py
--rw-r--r--   0        0        0     2286 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/config.py
--rw-r--r--   0        0        0      136 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/__init__.py
--rw-r--r--   0        0        0     9177 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/engine.py
--rw-r--r--   0        0        0     1578 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/generator.py
--rw-r--r--   0        0        0     1078 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/models.py
--rw-r--r--   0        0        0     2421 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/type_define.py
--rw-r--r--   0        0        0      136 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/engines/__init__.py
--rw-r--r--   0        0        0     1042 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/engines/xlrd_engine.py
--rw-r--r--   0        0        0     2107 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/engines/xlwings_engine.py
--rw-r--r--   0        0        0      547 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/exceptions.py
--rw-r--r--   0        0        0      433 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/__init__.py
--rw-r--r--   0        0        0     2233 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds1/__init__.py
--rw-r--r--   0        0        0      616 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds1/data_template.gd
--rw-r--r--   0        0        0      144 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds1/setting_template.gd
--rw-r--r--   0        0        0     2234 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds2/__init__.py
--rw-r--r--   0        0        0      616 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds2/data_template.gd
--rw-r--r--   0        0        0      144 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds2/setting_template.gd
--rw-r--r--   0        0        0     2280 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/json1/__init__.py
--rw-r--r--   0        0        0     2295 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/json2/__init__.py
--rw-r--r--   0        0        0     3103 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/resource/__init__.py
--rw-r--r--   0        0        0      513 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/logger.py
--rw-r--r--   0        0        0      278 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/babel.cfg
--rw-r--r--   0        0        0       16 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/gen_all.bat
--rw-r--r--   0        0        0       16 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/gen_pot.bat
--rw-r--r--   0        0        0      144 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/reg/删除右键导出.reg
--rw-r--r--   0        0        0      266 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/reg/删除右键导出所有.reg
--rw-r--r--   0        0        0      178 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/reg/添加右键导出.reg
--rw-r--r--   0        0        0      354 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/reg/添加右键导出所有.reg
--rw-r--r--   0        0        0    16102 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/sample/示例.xlsx
--rw-r--r--   0        0        0      700 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/__init__.py
--rw-r--r--   0        0        0      370 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/array.py
--rw-r--r--   0        0        0      448 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/array_bool.py
--rw-r--r--   0        0        0      374 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/array_str.py
--rw-r--r--   0        0        0      591 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/bool.py
--rw-r--r--   0        0        0      371 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/dict.py
--rw-r--r--   0        0        0      307 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/float.py
--rw-r--r--   0        0        0      351 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/function.py
--rw-r--r--   0        0        0      310 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/int.py
--rw-r--r--   0        0        0      346 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/string.py
--rw-r--r--   0        0        0      443 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/tr_array_str.py
--rw-r--r--   0        0        0      489 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/tr_dict.py
--rw-r--r--   0        0        0      460 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/tr_string.py
--rw-r--r--   0        0        0    11970 1970-01-01 00:00:00.000000 gd_excelexporter-3.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-23 05:09:54.908782 gd_excelexporter-3.0.1a0/LICENSE
+-rw-r--r--   0        0        0    11095 2024-04-23 05:09:54.908782 gd_excelexporter-3.0.1a0/README.md
+-rw-r--r--   0        0        0     2696 2024-04-23 05:10:09.332691 gd_excelexporter-3.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/babel/__init__.py
+-rw-r--r--   0        0        0     3338 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/babel/csharp.py
+-rw-r--r--   0        0        0     8496 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/babel/godot.py
+-rw-r--r--   0        0        0     4237 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/babel/json.py
+-rw-r--r--   0        0        0     4340 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/cli.py
+-rw-r--r--   0        0        0     2286 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/config.py
+-rw-r--r--   0        0        0      136 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/core/__init__.py
+-rw-r--r--   0        0        0     9177 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/core/engine.py
+-rw-r--r--   0        0        0     1578 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/core/generator.py
+-rw-r--r--   0        0        0     1078 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/core/models.py
+-rw-r--r--   0        0        0     2421 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/core/type_define.py
+-rw-r--r--   0        0        0      136 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/engines/__init__.py
+-rw-r--r--   0        0        0     1042 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/engines/xlrd_engine.py
+-rw-r--r--   0        0        0     2107 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/engines/xlwings_engine.py
+-rw-r--r--   0        0        0      547 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/exceptions.py
+-rw-r--r--   0        0        0      433 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/__init__.py
+-rw-r--r--   0        0        0     2454 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/gds1/__init__.py
+-rw-r--r--   0        0        0      622 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/gds1/data_template.gd
+-rw-r--r--   0        0        0      144 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/gds1/setting_template.gd
+-rw-r--r--   0        0        0     2456 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/gds2/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/gds2/data_template.gd
+-rw-r--r--   0        0        0      144 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/gds2/setting_template.gd
+-rw-r--r--   0        0        0     2280 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/json1/__init__.py
+-rw-r--r--   0        0        0     2295 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/json2/__init__.py
+-rw-r--r--   0        0        0     3120 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/resource/__init__.py
+-rw-r--r--   0        0        0      531 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/logger.py
+-rw-r--r--   0        0        0      278 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/template/babel.cfg
+-rw-r--r--   0        0        0       16 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/template/gen_all.bat
+-rw-r--r--   0        0        0       16 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/template/gen_pot.bat
+-rw-r--r--   0        0        0      144 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/template/reg/删除右键导出.reg
+-rw-r--r--   0        0        0      266 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/template/reg/删除右键导出所有.reg
+-rw-r--r--   0        0        0      178 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/template/reg/添加右键导出.reg
+-rw-r--r--   0        0        0      354 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/template/reg/添加右键导出所有.reg
+-rw-r--r--   0        0        0    16181 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/template/sample/示例.xlsx
+-rw-r--r--   0        0        0      700 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/__init__.py
+-rw-r--r--   0        0        0      370 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/array.py
+-rw-r--r--   0        0        0      448 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/array_bool.py
+-rw-r--r--   0        0        0      374 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/array_str.py
+-rw-r--r--   0        0        0      591 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/bool.py
+-rw-r--r--   0        0        0      371 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/dict.py
+-rw-r--r--   0        0        0      307 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/float.py
+-rw-r--r--   0        0        0      351 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/function.py
+-rw-r--r--   0        0        0      310 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/int.py
+-rw-r--r--   0        0        0      346 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/string.py
+-rw-r--r--   0        0        0      443 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/tr_array_str.py
+-rw-r--r--   0        0        0      489 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/tr_dict.py
+-rw-r--r--   0        0        0      460 2024-04-23 05:09:54.928781 gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/tr_string.py
+-rw-r--r--   0        0        0    12059 1970-01-01 00:00:00.000000 gd_excelexporter-3.0.1a0/PKG-INFO
```

### Comparing `gd_excelexporter-3.0.0a1/LICENSE` & `gd_excelexporter-3.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/README.md` & `gd_excelexporter-3.0.1a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 Platform: Windows(xlwings只支持Windows)
 
 Godot版本:^3.4
 
 ### 安装
 通过pip （建议）
 ```
-pip install gd-gd_excelexporter
+pip install gd_excelexporter
 ```
 
 或者直接去右边release里下载已经打包好的可执行文件（ee.exe，你需要将这个exe加到环境变量）。
 
 ### 创建配置表项目
 
 打开你的Godot游戏项目，项目根目录下右键打开命令行（此处打开powershell）
@@ -248,10 +248,12 @@
 
 ## 最后
 希望这个工具能够给一些独立游戏人或者业余自娱自乐的人一些帮助。
 如果你用上了我的工具，有什么问题最好直接提issue。
 
 如果你在你的独立游戏项目中使用了我的工具，希望你能够在游戏结尾员工名单或者开源证书页面中特别鸣谢加上我的名字，让我也占个光，谢谢。
 
-## 联系方式
+![Snipaste_2024-04-19_17-01-18](/assets/Snipaste_2024-04-19_17-01-18.png)
 
+## 联系方式
+QQ群：118258918
 ![Snipaste_2024-04-19_06-50-25](/assets/Snipaste_2024-04-19_06-50-25_icwxbsqi8.png)
```

### Comparing `gd_excelexporter-3.0.0a1/pyproject.toml` & `gd_excelexporter-3.0.1a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gd_excelexporter"
-version = "3.0.0a1"
+version = "3.0.1a0"
 description = "Godot Excel导表工具"
 authors = ["kaluluosi <kaluluosi@gamil.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "gd_excelexporter", from = "src" }]
 
 [tool.poetry.scripts]
```

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/csharp.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/babel/csharp.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/godot.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/babel/godot.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/json.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/babel/json.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/cli.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import os
 import pkg_resources
 import gd_excelexporter
 
 from gd_excelexporter.core.generator import Generator
 from gd_excelexporter.core.engine import Engine
 
-# from babel import *  # noqa
-from babel.messages.frontend import CommandLineInterface
 from gd_excelexporter.config import Configuration
 
 
 logger = logging.getLogger(__name__)
 
 
 @click.group
```

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/config.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/config.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/engine.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/core/engine.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/generator.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/core/generator.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/models.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/core/models.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/type_define.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/core/type_define.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/engines/xlrd_engine.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/engines/xlrd_engine.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/engines/xlwings_engine.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/engines/xlwings_engine.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/exceptions.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/exceptions.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds1/__init__.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/gds2/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 import glob
 import os
 import logging
 import jinja2
 import pkg_resources
+import textwrap
 
 from gd_excelexporter.core.generator import Generator, Table
 from gd_excelexporter.config import Configuration
 from gd_excelexporter.core.models import Variant
-from gd_excelexporter.type_defines import Function
+from gd_excelexporter.type_defines import Function, String, TrString
 
 # jinja2 docs: http://doc.yonyoucloud.com/doc/jinja2-docs-cn/templates.html#id2
 
 logger = logging.getLogger(__name__)
 
 
 def converter(var: Variant):
     type_define = var.type_define
-    if isinstance(var.value, str):
-        value = var.value.replace("\n", "\\n")
+    if isinstance(type_define, (String, TrString)):
+        value = escape(var.value)
         return f"'{value}'"
+
     if isinstance(type_define, Function):
-        func_name = f"{var.type_define.type_name}_{var.field_name}_{var.id}"
-        return f"funcref(self,'{func_name}')"
+        func_name = f"{var.field_name}_{var.id}"
+        return f"Callable(self,'{func_name}')"
+
     return var.value
 
 
-class GDS1Generator(Generator):
+def escape(text: str):
+    return text.replace("\n", "\\n")
+
+
+def indent(text: str):
+    txt = textwrap.indent(text, "\t")
+    return txt
+
+
+class GDS2Generator(Generator):
     # 导出格式
     __extension__ = "gd"
 
     loader = jinja2.FileSystemLoader(
         pkg_resources.resource_filename(__package__, "")  # type: ignore
     )
     env = jinja2.Environment(autoescape=False, loader=loader)
     env.filters["cvt"] = converter
+    env.filters["escape"] = escape
+    env.filters["indent"] = indent
 
     @classmethod
     def generate(cls, table: Table, config: Configuration):
         # 表格数据脚本模板
         template = cls.env.get_template("data_template.gd")
         code = template.render(table=table)
         return code
```

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds1/data_template.gd` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/gds2/data_template.gd`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # warnings-disable
-extends Reference
+extends RefCounted
 
+@warning_ignore("unused_variable")
 var True = true
+@warning_ignore("unused_variable")
 var False = false
+@warning_ignore("unused_variable")
 var None = null
 
+
 var data = \
 {
 {% for id,row in table.items()-%}
-    {{id}}:{% raw %}{{% endraw %}{% for field,value in row.items() %} "{{field}}":{{value|cvt|safe}}, {% endfor %}{% raw %}}{% endraw %},
+    {{id}}:{% raw %}{{% endraw %}{% for field,variant in row.items() %} "{{field}}":{{variant|cvt|safe}}, {% endfor %}{% raw %}}{% endraw %},
 {% endfor %}
 }
 
 {% for id,row in table.items()-%}
-    {% for field,value in row.items() -%} 
-
-{% if value.type_define.type_name == "function" %}
-func {{value.field_name}}_{{id}}{{value.type_define.params}}:
-    {% if value.value -%}
-    {{value.value}}
-    {%- else -%}
+    {% for field,variant in row.items() -%} 
+{% if variant.type_define.type_name == "function" %}
+@warning_ignore("unused_parameter")
+func {{variant.field_name}}_{{id}}{{variant.type_define.params}}:
+{% if variant.value -%}
+{{variant.value|indent}}
+{%- else -%}
     pass
-    {%- endif %}
+{%- endif %}
 {% endif %}
-
     {%- endfor %}
-
-{% endfor %}
+{%- endfor %}
```

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds2/__init__.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/resource/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,100 @@
 import glob
 import os
+import pprint
 import logging
-import jinja2
-import pkg_resources
-
+import textwrap
+import re
 from gd_excelexporter.core.generator import Generator, Table
 from gd_excelexporter.config import Configuration
-from gd_excelexporter.core.models import Variant
-from gd_excelexporter.type_defines import Function
-
-# jinja2 docs: http://doc.yonyoucloud.com/doc/jinja2-docs-cn/templates.html#id2
 
 logger = logging.getLogger(__name__)
 
 
-def converter(var: Variant):
-    type_define = var.type_define
-    if isinstance(var.value, str):
-        value = var.value.replace("\n", "\\n")
-        return f"'{value}'"
-    if isinstance(type_define, Function):
-        func_name = f"{var.type_define.type_name}_{var.field_name}_{var.id}"
-        return f"Callable(self,'{func_name}')"
-    return var.value
-
-
-class GDS2Generator(Generator):
+class ResourceGenerator(Generator):
     # 导出格式
-    __extension__ = "gd"
-
-    loader = jinja2.FileSystemLoader(
-        pkg_resources.resource_filename(__package__, "")  # type: ignore
-    )
-    env = jinja2.Environment(autoescape=False, loader=loader)
-    env.filters["cvt"] = converter
+    __extension__ = "tres"
+    __datatable_class__ = """
+    class_name EEDataTable
+    extends Resource
+
+    @export
+    var data = {}
+    """
 
     @classmethod
     def generate(cls, table: Table, config: Configuration):
         # 表格数据脚本模板
-        template = cls.env.get_template("data_template.gd")
-        code = template.render(table=table)
+        abs_output = os.path.abspath(config.output)
+        relpath = os.path.relpath(abs_output, config.project_root).replace("\\", "/")
+        template = """
+        [gd_resource type="Resource" script_class="EEDataTable" load_steps=2 format=3] 
+
+        [ext_resource type="Script" path="res://{relpath}/ee_data_table.gd" id="1"]
+
+        [resource]
+        script = ExtResource("1")
+        data = {data}
+        """  # noqa
+        template = textwrap.dedent(template)
+        new_table = {}
+
+        for id, row in table.items():
+            row_data = {}
+
+            for field, var in row.items():
+                field_name: str = field
+                row_data[field_name] = var.value
+
+            new_table[id] = row_data
+
+        code = template.format(
+            data=pprint.pformat(
+                new_table, indent=4, width=1000000000, compact=True, sort_dicts=True
+            ),
+            relpath=relpath,
+        )
+
+        code = textwrap.dedent(code)
+        code = re.sub(r"\b(True|False)\b", lambda m: m.group(1).lower(), code)
+        code = code.replace("'", '"')
         return code
 
     @classmethod
     def completed_hook(cls, config: Configuration):
         output = config.output
         settings_file_path = os.path.join(output, "settings.gd")
+        data_class_file_path = os.path.join(output, "ee_data_table.gd")
         project_root = config.project_root
 
         lines = []
 
         for path in glob.glob(f"{output}/**/*.{cls.__extension__}", recursive=True):
             if path == settings_file_path:
                 continue  # 跳过 settings.gd
+            if path == data_class_file_path:
+                continue  # 跳过数据表类
             basename = os.path.basename(path)
             setting_name = os.path.splitext(basename)[0]
             relpath = os.path.relpath(path, project_root).replace("\\", "/")
-            lines.append(f"var {setting_name} = load('res://{relpath}').new()")
+            lines.append(f"var {setting_name} = load('res://{relpath}')")
+
+            # 去掉缩进
+        code = textwrap.dedent(
+            """
+        extends Node
+        # 这个脚本你需要挂到游戏的Autoload才能全局读表
+
+        {refs_code}
+        """
+        )
+        refs_code = "\n".join(lines)
 
-        template = cls.env.get_template("setting_template.gd")
-        code = template.render(lines=lines)
+        code = code.format(refs_code=refs_code)
 
         with open(settings_file_path, "w", encoding="utf-8", newline="\n") as f:
             f.write(code)
-            logger.info(f"创建：{settings_file_path}")
+            logger.info("创建setting.gd")
+
+        with open(data_class_file_path, "w", encoding="utf-8", newline="\n") as f:
+            f.write(textwrap.dedent(cls.__datatable_class__))
+            logger.info("创建DataTable类")
```

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/json1/__init__.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/json1/__init__.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/json2/__init__.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/generators/json2/__init__.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/logger.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import sys
 
 FORMAT = "%(name)s-%(levelname)s:%(message)s"
 
-fh = logging.FileHandler("log.txt", "w")
+fh = logging.FileHandler("log.txt", "w", encoding="utf-8")
 fh.setLevel(logging.DEBUG)
 fh.setFormatter(logging.Formatter(FORMAT))
 
 ch = logging.StreamHandler(sys.stdout)
 ch.setLevel(logging.DEBUG)
 ch.setFormatter(logging.Formatter(FORMAT))
```

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/sample/示例.xlsx` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/template/sample/示例.xlsx`

 * *Files 20% similar despite different names*

```diff
@@ -20,988 +20,993 @@
 00000130: 6598 dfa5 e45c 7a28 6b23 5a48 a7a5 c150  e....\z(k#ZH...P
 00000140: 5fc6 eaa3 d269 eed1 89f7 e7fb c5eb ede7  _....i..........
 00000150: fc91 b3e0 d76f 956c 469b 5a6f 8b5e 1508  .....o.lF.Zo.^..
 00000160: 623d 5816 d41c c158 271c 694c c19f 2443  b=X....X'.iL..$C
 00000170: e9f0 17e0 5e13 b862 a871 6b9c abe5 c3cd  ....^..b.qk.....
 00000180: 72fe d404 5ca1 7edc bd2c deae 5b31 64f6  r...\.~..,..[1d.
 00000190: 2fbf db0c acb1 fea0 63df bf46 7c01 504b  /.......c..F|.PK
-000001a0: 0304 1400 0000 0800 874e e240 b205 0148  .........N.@...H
-000001b0: 4201 0000 3e02 0000 1100 0000 646f 6350  B...>.......docP
+000001a0: 0304 1400 0000 0800 874e e240 0a45 e12f  .........N.@.E./
+000001b0: 4301 0000 3e02 0000 1100 0000 646f 6350  C...>.......docP
 000001c0: 726f 7073 2f63 6f72 652e 786d 6c7d 9151  rops/core.xml}.Q
-000001d0: 4bc3 3014 85df 05ff 43c9 7b9b 64dd 460d  K.0.....C.{.d.F.
+000001d0: 4bc3 3014 85df 05ff 43c9 7b9b a4dd 860b  K.0.....C.{.....
 000001e0: 6d07 2a7b 7220 5851 7c0b c9dd 566c d292  m.*{r XQ|...Vl..
 000001f0: 44bb bd0a bef8 ea8f 14ff 8559 d7d5 89e2  D..........Y....
 00000200: 6338 e77e f7dc 9374 b651 55f0 0cc6 96b5  c8.~...t.QU.....
-00000210: ce10 8d08 0a40 8b5a 967a 95a1 db62 1e26  .....@.Z.z...b.&
-00000220: 28b0 8e6b c9ab 5a43 86b6 60d1 2c3f 3d49  (..k..ZC..`.,?=I
-00000230: 45c3 446d e0da d40d 1857 820d 3c49 5b26  E.Dm.....W..<I[&
-00000240: 9a0c ad9d 6b18 c656 ac41 711b 7987 f6e2  ....k..V.Aq.y...
-00000250: b236 8a3b ff34 2bdc 70f1 c857 8047 844c  .6.;.4+.p..W.G.L
-00000260: b102 c725 771c ef80 6133 1051 8f94 6240  ...%w...a3.Q..b@
-00000270: 364f a6ea 0052 60a8 4081 7616 d388 e26f  6O...R`.@.v....o
-00000280: af03 a3ec 9f03 9d72 e454 a5db 36fe a63e  .......r.T..6..>
-00000290: ee31 5b8a bd38 b837 b61c 8c6d db46 6ddc  .1[..8.7...m.Fm.
-000002a0: c5f0 f929 be5f 5cdd 74a7 86a5 de75 2500  ...)._\.t....u%.
-000002b0: e5bb 7e2a 6edd c257 b92c 419e 6ff3 cf97  ..~*n..W.,A.o...
-000002c0: f78f d7b7 14ff 5652 29ba 6c4c 18e0 0e64  ......VR).lL...d
-000002d0: e0b7 b17d b683 7217 5f5c 1673 948f 089d  ...}..r._\.s....
-000002e0: 8464 1a92 4941 1346 cf18 210f 293e b8fa  .d..IA.F..!.)>..
-000002f0: f97c 00aa 7efd bfc4 d138 24e3 9026 058d  .|..~....8$..&..
-00000300: d924 6124 3e22 1e00 7997 fbe7 8fe7 5f50  .$a$>"..y....._P
-00000310: 4b03 0414 0000 0008 0087 4ee2 40c4 2d55  K.........N.@.-U
-00000320: 0328 0100 000e 0200 0013 0000 0064 6f63  .(...........doc
-00000330: 5072 6f70 732f 6375 7374 6f6d 2e78 6d6c  Props/custom.xml
-00000340: a591 416b 8330 1886 ef83 fd07 c93d 26a6  ..Ak.0.......=&.
-00000350: d5d4 a296 1a15 c60e 1bac f32e 31b6 8249  ............1..I
-00000360: c4c4 6e65 ecbf 2fa5 ebc6 0ebb 6cc7 8fef  ..ne../.....l...
-00000370: e5e1 79bf 2fd9 bcca c13b 8ac9 f45a a520  ..y./....;...Z. 
-00000380: f031 f084 e2ba edd5 3e05 cfbb 0aae 8067  .1......>......g
-00000390: 6ca3 da66 d04a a4e0 240c d864 b737 c9e3  l..f.J..$..d.7..
-000003a0: a447 31d9 5e18 cf21 9449 c1c1 da71 8d90  .G1.^..!.I...q..
-000003b0: e107 211b e3bb b572 9b4e 4fb2 b16e 9cf6  ..!....r.NO..n..
-000003c0: 4877 5dcf 45a1 f92c 85b2 8860 1c21 3e1b  Hw].E..,...`.!>.
-000003d0: ab25 1cbf 70e0 c25b 1fed 5f91 ade6 673b  .%..p..[.._...g;
-000003e0: 53ef 4ea3 d3cd 924f f8c9 eba4 eddb 14bc  S.N....O........
-000003f0: 1521 2b8a 1087 9094 3183 010e 7218 2f62  .!+.....1...r./b
-00000400: 0af1 0a63 9213 56c5 dbf2 1d78 e339 4c80  ...c..V....x.9L.
-00000410: a71a e9aa dfb1 dab1 8e76 3d8c 2fc6 4e19  .........v=./.N.
-00000420: 0da2 92c6 8456 118b 960b badd c645 b5cc  .....V.......E..
-00000430: d92a 0a4b 5ab0 1027 e83b 9ba0 abc3 3f6d  .*.KZ..'.;....?m
-00000440: 1657 9bfb a707 57b2 9db9 cde7 7e68 6b31  .W....W.....~hk1
-00000450: fd90 2338 2430 20be fba8 1f44 94c4 bfd9  ..#8$0 ....D....
-00000460: a0f3 a92e 8fcc 3e00 504b 0304 0a00 0000  ......>.PK......
-00000470: 0000 874e e240 0000 0000 0000 0000 0000  ...N.@..........
-00000480: 0000 0300 0000 786c 2f50 4b03 0414 0000  ......xl/PK.....
-00000490: 0008 0087 4ee2 40a0 000b 0877 0100 0019  ....N.@....w....
-000004a0: 0400 0010 0000 0078 6c2f 636f 6d6d 656e  .......xl/commen
-000004b0: 7473 312e 786d 6cdd 93c1 4ac3 301c c6ef  ts1.xml...J.0...
-000004c0: 82ef 5022 7873 6937 119d 6d87 9781 e0c1  ..P"xsi7..m.....
-000004d0: 833e 406c b3b5 d0a6 2589 433d 0a4e 700c  .>@l....%.C=.Np.
-000004e0: 0613 641e 76d0 8363 e840 8620 caf0 6596  ..d.v..c.@. ..e.
-000004f0: 6e7b 0bd3 b5dd 4110 0fde 0621 e4fb f2cf  n{....A....!....
-00000500: 97f0 4ba2 97ce 7c4f a961 cadc 8018 40cb  ..K...|O.a....@.
-00000510: a940 c1c4 0a6c 9754 0d70 7c54 ded8 060a  .@...l.T.p|T....
-00000520: e388 d8c8 0b08 36c0 3966 a064 aeae e856  ......6.9f.d...V
-00000530: e0fb 9870 a6c8 00c2 0ce0 701e 1621 6496  ...p......p..!d.
-00000540: 837d c472 4188 899c a904 d447 5c4a 5a85  .}.rA......G\JZ.
-00000550: 2ca4 18d9 ccc1 98fb 1ecc abea 16f4 914b  ,..............K
-00000560: 80a9 a353 ee04 9465 0373 76d9 9e5c dde8  ...S...e.sv..\..
-00000570: 30f1 cd6c 200b d25d 0f5c c617 42a1 b862  0..l ..].\..B..b
-00000580: 803d 0d28 49fd be6d 0055 a672 7c26 8ba8  .=.(I..m.U.r|&..
-00000590: 6c87 b23b 81a6 ce2e 941a f20c b003 a4a0  l..;............
-000005a0: e580 f044 8b41 633c 6ac7 a6e5 20ca 706a  ...D.Ac<j... .pj
-000005b0: 6b85 cdd8 83f3 f53c 3d55 5187 3215 c6b1  k......<=UQ.2...
-000005c0: 69f2 bf52 637c 4516 224b b295 7c18 a635  i..Rc|E."K..|..5
-000005d0: 0ccc f535 4ddd 152f 77d1 e06d f2fa 29ba  ...5M../w..m..).
-000005e0: 8db9 31fd ea8c dffb 8921 ea43 31b8 1f7f  ..1......!.C1...
-000005f0: d427 b73d d1ee 2ffc e9e8 396a 3e88 4e6f  .'.=../...9j>.No
-00000600: faf4 1875 5b8b c3c2 8406 4c01 fe84 975f  ...u[.....L...._
-00000610: 4e78 d1b0 37bb 960f 29bd b13f 2014 9613  Nx..7...)..? ...
-00000620: 8268 357f 2790 3d88 e447 658a 99df 504b  .h5.'.=..Ge...PK
-00000630: 0304 1400 0000 0800 874e e240 a000 0b08  .........N.@....
-00000640: 7701 0000 1904 0000 1000 0000 786c 2f63  w...........xl/c
-00000650: 6f6d 6d65 6e74 7332 2e78 6d6c dd93 c14a  omments2.xml...J
-00000660: c330 1cc6 ef82 ef50 2278 7369 3711 9d6d  .0.....P"xsi7..m
-00000670: 8797 81e0 c183 3e40 6cb3 b5d0 a625 8943  ......>@l....%.C
-00000680: 3d0a 4e70 0c06 1364 1e76 d083 63e8 4086  =.Np...d.v..c.@.
-00000690: 20ca f065 966e 7b0b d3b5 dd41 100f de06   ..e.n{....A....
-000006a0: 21e4 fbf2 cf97 f04b a297 ce7c 4fa9 61ca  !......K...|O.a.
-000006b0: dc80 1840 cba9 40c1 c40a 6c97 540d 707c  ...@..@...l.T.p|
-000006c0: 54de d806 0ae3 88d8 c80b 0836 c039 66a0  T..........6.9f.
-000006d0: 64ae aee8 56e0 fb98 70a6 c800 c20c e070  d...V...p......p
-000006e0: 1e16 2164 9683 7dc4 7241 8889 9ca9 04d4  ..!d..}.rA......
-000006f0: 475c 4a5a 852c a418 d9cc c198 fb1e ccab  G\JZ.,..........
-00000700: ea16 f491 4b80 a9a3 53ee 0494 6503 7376  ....K...S...e.sv
-00000710: d99e 5cdd e830 f1cd 6c20 0bd2 5d0f 5cc6  ..\..0..l ..].\.
-00000720: 1742 a1b8 6280 3d0d 2849 fdbe 6d00 55a6  .B..b.=.(I..m.U.
-00000730: 727c 268b a86c 87b2 3b81 a6ce 2e94 1af2  r|&..l..;.......
-00000740: 0cb0 03a4 a0e5 80f0 448b 4163 3c6a c7a6  ........D.Ac<j..
-00000750: e520 ca70 6a6b 85cd d883 f3f5 3c3d 5551  . .pjk......<=UQ
-00000760: 8732 15c6 b169 f2bf 5263 7c45 1622 4bb2  .2...i..Rc|E."K.
-00000770: 957c 18a6 350c ccf5 354d dd15 2f77 d1e0  .|..5...5M../w..
-00000780: 6df2 fa29 ba8d b931 fdea 8cdf fb89 21ea  m..)...1......!.
-00000790: 4331 b81f 7fd4 27b7 3dd1 ee2f fce9 e839  C1....'.=../...9
-000007a0: 6a3e 884e 6ffa f418 755b 8bc3 c284 064c  j>.No...u[.....L
-000007b0: 01fe 8497 5f4e 78d1 b037 bb96 0f29 bdb1  ...._Nx..7...)..
-000007c0: 3f20 1496 1382 6835 7f27 903d 88e4 4765  ? ....h5.'.=..Ge
-000007d0: 8a99 df50 4b03 040a 0000 0000 0087 4ee2  ...PK.........N.
-000007e0: 4000 0000 0000 0000 0000 0000 000e 0000  @...............
-000007f0: 0078 6c2f 776f 726b 7368 6565 7473 2f50  .xl/worksheets/P
-00000800: 4b03 0414 0000 0008 0087 4ee2 403c b21c  K.........N.@<..
-00000810: a9f1 0100 0005 0400 0018 0000 0078 6c2f  .............xl/
-00000820: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00000830: 312e 786d 6c8d 936d 6f9b 3010 c7df 4fda  1.xml..mo.0...O.
-00000840: 77b0 fcbe 9890 ae6d 22a0 5212 459b b449  w......m".R.E..I
-00000850: d5b4 87d7 8e39 8215 dbc7 6c27 b4df 7e07  .....9....l'..~.
-00000860: 8c2c 6d27 ad2f 10e7 bbe3 e7ff 3d90 df3f  .,m'./......=..?
-00000870: 5ac3 4ee0 8346 57f0 5992 7206 4e61 a5dd  Z.N..FW.Y.r.Na..
-00000880: bee0 dfbf 6daf ee38 0b51 ba4a 1a74 50f0  ....m..8.Q.J.tP.
-00000890: 2708 fcbe 7cff 2eef d01f 4203 1019 115c  '...|.....B....\
-000008a0: 2878 1363 bb14 22a8 06ac 0c09 b6e0 2852  (x.c..".......(R
-000008b0: a3b7 32d2 d1ef 4568 3dc8 6af8 c81a 91a5  ..2...Eh=.j.....
-000008c0: e98d b052 3b3e 1296 fe2d 0cac 6bad 6083  ...R;>...-..k.`.
-000008d0: ea68 c1c5 11e2 c1c8 48fa 43a3 db30 d11e  .h......H.C..0..
-000008e0: ab37 f12a 2f3b aa75 d273 2171 3346 cebc  .7.*/;.u.s!q3F..
-000008f0: d9f5 2b7d 562b 8f01 eb98 28b4 6294 f6ba  ..+}V+....(.b...
-00000900: ca85 583c abd3 aa57 a07f 34cb 4a7f 38b6  ..X<...W..4.J.8.
-00000910: 5704 6ea9 b89d 363a 3e0d e54e 8220 fee5  W.n...6:>..N. ..
-00000920: 745d 9774 6d48 94fb a3e2 a241 b35b 0171  t].tmH.....A.[.q
-00000930: 7d0c 11ed 4646 c9cb 7c98 c083 1765 5e69  }...FF..|....e^i
-00000940: ea62 3f7a e6a1 2ef8 2a5b aee6 9cfc 43c6  .b?z....*[....C.
-00000950: 0f0d 5db8 b059 3ff2 1de2 a10f 7caa 0a9e  ..]..Y?.....|...
-00000960: f62c 30a0 fae6 3349 af13 acc1 9882 afe7  .,0...3I........
-00000970: 1f68 6d7e 0dd0 de26 a438 332f ed89 bf1d  .hm~...&.83/....
-00000980: d6e4 c1b3 0a6a 7934 718d e6a7 ae62 53f0  .....jy4q....bS.
-00000990: 059f 7c5f b1fb 087a df44 dad3 eb24 a31b  ..|_...z.D...$..
-000009a0: f018 8d76 f019 4e60 285a f0ec b98f 2894  ...v..N`(Z....(.
-000009b0: 7b2e a82f bfcc 3d76 8c56 8352 7bd2 dd62  {../..=v.V.R{..b
-000009c0: 2085 56f6 3b9c 2d33 aa49 f5f1 1525 90e7   .V.;.-3.I...%..
-000009d0: 8633 ca0a e43d 9569 2e4e 245e d143 9033  .3...=.i.N$^.C.3
-000009e0: 69fe 3f12 25bc 20cd 5e90 c6e6 8cfa 5ab9  i.?.%. .^.....Z.
-000009f0: 872f d2ef b50b cc40 4db7 a7c9 2d67 7eac  ./.....@M...-g~.
-00000a00: 7cb0 23b6 8397 5ab0 c348 839d 4e0d fd5f  |.#...Z..H..N.._
-00000a10: 40e2 d384 eeac 11e3 74a0 018c b1ed e0ec  @.......t.......
-00000a20: e771 fe81 cbdf 504b 0304 0a00 0000 0000  .q....PK........
-00000a30: 874e e240 0000 0000 0000 0000 0000 0000  .N.@............
-00000a40: 0c00 0000 786c 2f64 7261 7769 6e67 732f  ....xl/drawings/
-00000a50: 504b 0304 1400 0000 0800 874e e240 5842  PK.........N.@XB
-00000a60: 137c d402 0000 c10a 0000 1b00 0000 786c  .|............xl
-00000a70: 2f64 7261 7769 6e67 732f 766d 6c44 7261  /drawings/vmlDra
-00000a80: 7769 6e67 312e 766d 6ced 565d 6f9b 3014  wing1.vml.V]o.0.
-00000a90: 7d8f b4ff 80dc 5792 006a d2d6 01aa a95b  }.....W..j.....[
-00000aa0: dfb6 495b a73d 560e 38c1 adf1 45f8 8690  ..I[.=V.8...E...
-00000ab0: fdfa 5d43 a8ca d44d d534 f5a5 8d14 e2dc  ..]C...M.4......
-00000ac0: eb73 bfce b145 7cd9 96da 6b64 6d15 9884  .s...E|...kdm...
-00000ad0: 85b3 8079 d264 902b b34d d8f7 9beb e939  ...y.d.+.M.....9
-00000ae0: f32c 0a93 0b0d 4626 ec20 2dbb 4cdf 4d62  .,....F&. -.L.Mb
-00000af0: 87a3 afb1 1c44 c276 b5e1 362b 6429 ecb4  .....D.v..6+d)..
-00000b00: 5459 0d16 3638 cda0 e4b0 d9a8 4c72 91a1  TY..68......Lr..
-00000b10: 6a04 5216 7684 55cf 4055 b097 7505 cae0  j.R.v.U.@U..u...
-00000b20: 806a 9f81 926d 26f5 0080 6700 fa1a 0744  .j...m&...g....D
-00000b30: f337 4453 6a96 c6c0 6d21 2aa9 c501 76e8  .7DSj...m!*...v.
-00000b40: 355c b698 3099 2bec 7c2a 2f45 35b2 7ab9  5\..0.+.|*/E5.z.
-00000b50: 409a 52c8 e669 3c1f 81d3 b8e9 63e1 a192  @.R..i<.....c...
-00000b60: 9eca 1376 db06 f4b9 c528 8898 9701 d4b9  ...v.....(......
-00000b70: 553f 69f2 51b8 0c02 bf7b 328f 6254 94b2  U?i.Q....{2.bT..
-00000b80: db53 092c 1256 067e a08f fe7e d7e8 19b4  .S.,.V.~...~....
-00000b90: 92a5 13cf 73e9 b086 7be9 ddd1 582d 1e34  ....s...{...X-.4
-00000ba0: 852e 15ca 9a6a ebfd 2e9e b7ad 45ae a4c1  .....j......E...
-00000bb0: ae4f b84f 1831 003c 0363 6486 aed6 84d5  .O.O.1.<.cd.....
-00000bc0: b472 a078 fea8 8574 3219 3a7a dc8d 0d83  .r.x...t2.:z....
-00000bd0: 6831 2ebb 0f72 326a f758 4f05 5639 a970  h1...r2j.XO.V9.p
-00000be0: b1b6 a077 2857 5a6e 9007 15ae 10aa eeb7  ...w(WZn........
-00000bf0: 14f5 5699 6967 5f2e 66d1 827c 479b db12  ..V.ig_.f..|G...
-00000c00: 85f4 bf90 6a5b 205f 5cf4 eebd cab1 e017  ....j[ _\.......
-00000c10: 4bf2 34ca aab5 d20a 0fbc 5079 2ecd 8a79  K.4.......Py...y
-00000c20: 1ba5 7506 1aea 849d 5cd3 e763 d8db 2471  ..u.....\..c..$q
-00000c30: 42cd f753 ebd7 c069 7412 4bc8 690c 6287  B..S...it.K.i.b.
-00000c40: f047 a21c bd6e 9ec4 7bc3 5d06 cf1d 330a  .G...n..{.]...3.
-00000c50: d765 8a1e a782 6c67 7ba6 8949 2794 07a6  .e....lg{..I'...
-00000c60: 86aa 9c2e 023a a04f 3047 9b55 29b6 d2e9  .....:.O0G.U)...
-00000c70: 8c78 4285 8e57 1705 b886 ec7e ac46 612b  .xB..W.....~.Fa+
-00000c80: e2ae 76c7 3161 9b3e 1792 86d7 d052 9f9d  ..v.1a.>.....R..
-00000c90: 2472 e5e8 751c 68ac 57bd d0a7 1b0d 7b5e  $r..u.h.W.....{^
-00000ca0: 40ad 7e82 41a1 57a5 8569 0d28 50f2 6045  @.~.A.W..i.(P.`E
-00000cb0: d2cf 5533 e05d b8a9 d06a 4b01 883b 9783  ..U3.]...jK..;..
-00000cc0: 6472 4c92 c62d bfd2 4e5e 1f5c bd5f d677  drL..-..N^.\._.w
-00000cd0: 94eb a613 d567 4012 2af9 3f41 237f 282c  .....g@.*.?A#.(,
-00000ce0: aea4 d696 d02d ff46 c760 6c79 6f32 aa26  .....-.F.`lyo2.&
-00000cf0: 0dfd 70e1 87fe 851f f967 a1bf f0cf e379  ..p......g.....y
-00000d00: cb8f 3ec2 7d85 7d1a 3993 5bb8 cc24 a9d2  ..>.}.}.9.[..$..
-00000d10: a481 331d d7dd f2a1 a0ae d44e f80f a7f3  ..3........N....
-00000d20: 772d 2f5f 50cb cbd9 9953 f79b 9a5f 919a  w-/_P....S..._..
-00000d30: 8341 cda7 4fa9 39fc cf6a 3e7b 4135 87b3  .A..O.9..j>{A5..
-00000d40: 3731 bfb2 ab99 de4a faab f9d4 ef94 3bbe  71.....J......;.
-00000d50: 9abb 7bf8 5fae e639 bd7e a6bf 0050 4b03  ..{._..9.~...PK.
-00000d60: 0414 0000 0008 0087 4ee2 4086 7690 7bd7  ........N.@.v.{.
-00000d70: 0400 0071 1100 0018 0000 0078 6c2f 776f  ...q.......xl/wo
-00000d80: 726b 7368 6565 7473 2f73 6865 6574 322e  rksheets/sheet2.
-00000d90: 786d 6c8d 58db 72a3 3810 7ddf aafd 078a  xml.X.r.8.}.....
-00000da0: f701 6363 3b4e 194f 25be c44e 9cc4 b5b3  ..cc;N.O%..N....
-00000db0: 9767 02b2 4d0d 2016 9438 99af df96 642e  .g..M. ..8....d.
-00000dc0: 6a69 e3bc 8050 9f6e 759f 6edd 987e 7fcf  ji...P.nu.n..~..
-00000dd0: 52eb 8d94 5542 f3c0 f69c 9e6d 913c a271  R...UB.....m.<.q
-00000de0: 921f 02fb af3f 57df ae6c ab62 611e 8729  .....?W..l.ba..)
-00000df0: cd49 607f 90ca fe3e fbfd b7e9 8996 3fab  .I`....>......?.
-00000e00: 2321 cc02 0b79 15d8 47c6 8a6b d7ad a223  #!...y..G..k...#
-00000e10: c9c2 caa1 05c9 41b2 a765 1632 f82c 0f6e  ......A..e.2.,.n
-00000e20: 5594 248c 8552 96ba fd5e 6fe4 6661 92db  U.$..R...^o.fa..
-00000e30: d2c2 75f9 151b 74bf 4f22 b2a0 d16b 4672  ..u...t.O"...kFr
-00000e40: 268d 9424 0d19 f85f 1d93 a2aa adbd c75f  &..$..._......._
-00000e50: b217 97e1 0962 adfd e9b8 b890 92c6 9ee7  .....b..........
-00000e60: 6bfe 6549 54d2 8aee 9913 d1cc 95ae e951  k.eIT..........Q
-00000e70: 4edc 8912 6716 6986 0c64 6561 f9f3 b5f8  N...g.i..dea....
-00000e80: 0686 0b08 ee25 4913 f621 c2ad 1d22 acb5  .....%I..!..."..
-00000e90: 733a 9d9c 5351 3951 7ef6 a243 9037 7609  s:..SQ9Q~..C.7v.
-00000ea0: 9bbf 568c 668b 9085 f66c 2a32 b02b ddd9  ..V.f....l*2.+..
-00000eb0: 344e 8045 9e7a ab24 fbc0 bef1 ae77 131b  4N.E.z.$.....w..
-00000ec0: fa05 e2ef 849c aa4e db62 b4d8 923d 9b93  .......N.b...=..
-00000ed0: 340d ec95 675b bc06 5e28 fdc9 919b 38b0  4...g[..^(....8.
-00000ee0: 7bdc 3849 49c4 b361 85f0 7a23 12bd e9f3  {.8II..a..z#....
-00000ef0: 3afa 578c c2db 3086 db0c d26d d703 ae44  :.W...0....m...D
-00000f00: ddec 4a2b 26fb f035 6573 9afe 93c4 ec18  ..J+&..5es......
-00000f10: d813 bbee fb83 9ed6 2439 1c19 14ae eff4  ........$9......
-00000f20: 87dc 6a44 5330 014f 2b4b a0a0 7ddb cac2  ..jDS0.O+K..}...
-00000f30: 77f1 3e49 f591 ef5c 8d87 b615 0946 ce36  w.>I...\.....F.6
-00000f40: bdb3 aa54 0257 8512 bccf 4a5e 8f9b ff4c  ...T.W....J^...L
-00000f50: 07bc 123a f03e ebf4 af2e 0ee4 c16c 135a  ...:.>.......l.Z
-00000f60: bcd1 aa5d 70cf 03e6 a516 4f81 8c6a 0006  ...]p.....O..j..
-00000f70: 3e89 c8eb d72a d038 ab7c 8108 6f50 ab41  >....*.8.|..oP.A
-00000f80: e3ac e60d 9dcf 99f0 6ace 79a3 0e6a e45c  ........j.y..j.\
-00000f90: 0a0a 8cca a0a0 510f 3570 4617 68f7 46b5  ......Q.5pF.h.F.
-00000fa0: 1a34 eac1 fe97 7857 5687 283c 3e17 66d3  .4....xWV.(<>.f.
-00000fb0: 929e 2c58 2780 4858 c1e0 2939 94c5 27bb  ..,X'.HX..)9..'.
-00000fc0: 8b90 2f6e de35 8c04 75c5 c137 0d1a 0aaf  ../n.5..u..7....
-00000fd0: 82de b759 7fea be41 1547 67c4 ed45 c45c  ...Y...A.Gg..E.\
-00000fe0: 470c 541b 0b1d e1ab 88a5 8e18 aa08 3e47  G.T...........>G
-00000ff0: 655c 8da7 2315 71a7 23c6 2a62 ad23 ae54  e\..#.q.#.*b.#.T
-00001000: c446 474c 54c4 bd8e f07a 2ae4 c100 f154  .FGLT....z*....T
-00001010: c856 8720 461e 7584 8752 f374 19f2 6c80  .V. F.u..R.t..l.
-00001020: a0e4 ec0c 90d6 1717 aaaa 292d 9870 95a1  ..........)-.p..
-00001030: 8678 7760 c3b3 c98c 8792 776b 80a0 eccd  .xw`......wk....
-00001040: 0d10 94be 8501 82f2 b734 4050 0257 3aa4  .........4@P.W:.
-00001050: 8f12 7867 80a0 04ae 0d10 949e 8d01 82b8  ..xg............
-00001060: bf37 405a eec5 0c7d 3040 10bb 5b03 04b1  .7@Z...}0@..[...
-00001070: fb68 8020 769f 0c10 c4ee b301 82d8 dde9  .h. v...........
-00001080: 9041 cbae 524d b00e 8bed 6edc d98f 9a3d  .A..RM....n....=
-00001090: d05c 69a0 0295 06cf a6d2 0628 2fb7 3a04  .\i........(/.:.
-000010a0: a565 ae23 5056 163a 0225 65a9 2350 4e56  .e.#PV.:.%e.#PNV
-000010b0: 3a02 a5e4 4e47 a08c ac75 044a c846 47a0  :...NG...u.J.FG.
-000010c0: 7cdc eb08 6db9 d221 03c4 d9d6 0041 a43d  |...m..!.....A.=
-000010d0: ea10 6dbd aa21 fc6c c377 9fe7 baa3 cda7  ..m..!.l.w......
-000010e0: 87cc ee0c 9036 194a 3dc1 166d 5a9d 7cb1  .....6.J=..mZ.|.
-000010f0: abe1 3231 f6ce 8dbd 0b6e 581c bbda aa6b  ..21.....nX....k
-00001100: 5d10 812c 0102 c217 d350 2b29 939b eb00  ]..,.....P+)....
-00001110: 95c9 9d22 4415 b256 84a8 3836 8a10 d5c5  ..."D..V..86....
-00001120: bd22 4425 f100 4214 8fdf 4e51 11cf d600  ."D%..B...NQ....
-00001130: 410c 3e1a 20a8 6a9e 0c10 94de 6780 b4ac  A.>. .j.....g...
-00001140: a2f8 778a b00d 51c9 3a1c b19a acf3 f409  ..w...Q.:.......
-00001150: ff6f 86a6 a3cc 02b0 cd60 7e9b 42c5 1e9c  .o.......`~.B...
-00001160: bd1a 7b9d 7312 3f31 bdcd 064e 0fd1 702b  ..{.s.?1...N..p+
-00001170: 0528 f2b9 b177 09b6 9b2a 418c afa4 4c56  .(...w...*A...LV
-00001180: 898f ab44 1122 96d6 8a10 5749 5738 6829  ...D."....WIW8h)
-00001190: 94d3 af2b f491 d95d 57d8 d154 c81a 77c8  ...+...]W..T..w.
-000011a0: e294 4bf2 c782 2bdf 4151 dcca 7e54 01f3  ..K...+.AQ..~T..
-000011b0: 73af c6ec 128c b7d9 6a5d 571c 806b 0ddf  s.......j]W..k..
-000011c0: 4386 5d47 e082 507b 7225 3cc1 7ec8 de36  C.]G..P{r%<.~..6
-000011d0: ffc2 eb05 bfd4 81a5 eea0 68e2 6c6b 08bf  ..........h.lk..
-000011e0: f175 cf45 7051 6a6b a619 7c22 066f 6995  .u.EpQjk..|".oi.
-000011f0: 2af2 aa28 4fec 4578 208f 6179 48f2 ca4a  *..(O.Ex .ayH..J
-00001200: e136 0ab7 4e07 2229 e53d 50b4 e19e 2a7a  .6..N.").=P...*z
-00001210: c1af 17ca e0de 5b7f 1de1 f703 8135 b4e7  ......[......5..
-00001220: c00a b9a7 94d5 1fe0 1cb7 fb83 b0d7 c22a  ...............*
-00001230: c282 943f 925f f0b7 039c a465 023f 1ac4  ...?._.....e.?..
-00001240: ff85 c02e 68c9 ca30 61fc ba28 8dad 8415  ....h..0a..(....
-00001250: f84c c921 8c3e ce3f 0dac f23a 8903 bbdc  .L.!.>.?...:....
-00001260: c47d 71d5 6d7e 96cc fe03 504b 0304 1400  .}q.m~....PK....
-00001270: 0000 0800 874e e240 8ae2 eb49 d202 0000  .....N.@...I....
-00001280: c10a 0000 1b00 0000 786c 2f64 7261 7769  ........xl/drawi
-00001290: 6e67 732f 766d 6c44 7261 7769 6e67 322e  ngs/vmlDrawing2.
-000012a0: 766d 6ced 565d 6fd3 3014 7daf c47f 88bc  vml.V]o.0.}.....
-000012b0: d7b4 4da2 755b dd24 131a ec0d 9060 88c7  ..M.u[.$.....`..
-000012c0: c94d dcc6 9be3 1bc5 b769 caaf e73a 4947  .M.......i...:IG
-000012d0: 0b03 4d08 78d9 5235 b5ee f5b9 5fe7 d86a  ..M.x.R5...._..j
-000012e0: 7cd9 96da 6b64 6d15 9884 8593 8079 d264  |...kdm......y.d
-000012f0: 902b b34e d8e7 9beb f105 f32c 0a93 0b0d  .+.N.......,....
-00001300: 4626 6c27 2dbb 4c5f 8d62 87a3 afb1 1c44  F&l'-.L_.b.....D
-00001310: c236 b5e1 362b 6429 ecb8 5459 0d16 5638  .6..6+d)..TY..V8
-00001320: cea0 e4b0 5aa9 4c72 91a1 6a04 5216 36c0  ....Z.Lr..j.R.6.
-00001330: aa27 a02a d8ca ba02 6570 8f6a 9f80 926d  .'.*....ep.j...m
-00001340: 26f5 1e00 4f00 f435 ee11 cdef 104d a959  &...O..5.....M.Y
-00001350: 1a03 b785 a8a4 163b d8a0 d770 d962 c264  .......;...p.b.d
-00001360: aeb0 f3a9 bc14 d591 d5cb 05d2 9422 364d  ............."6M
-00001370: e3e9 1138 8d9b 3e16 ee2a e9a9 3c61 b76d  ...8..>..*..<a.m
-00001380: 40cf 2d46 41c4 bc0c a0ce adfa 4a93 8fc2  @.-FA.......J...
-00001390: b320 f0bb 37f3 2846 4529 bb3d 95c0 2261  . ..7.(FE).=.."a
-000013a0: 65e0 077a f0f7 bb8e de41 2b59 3af2 3c97  e..z.....A+Y:.<.
-000013b0: 0e6b b897 de1d 8dd5 e24e 53e8 52a1 aca9  .k.......NS.R...
-000013c0: b6de efe2 79eb 5ae4 4a1a ecfa 84fb 8411  ....y.Z.J.......
-000013d0: 03c0 3330 4666 e86a 4d58 4d2b 078a a707  ..30Ff.jMXM+....
-000013e0: 2da4 a3d1 bea3 c36e 6c14 9cce 8fcb ee83  -......nl.......
-000013f0: 9c1c b53b d453 8155 4e2a 5c2c 2de8 0dca  ...;.S.UN*\,-...
-00001400: 8596 2be4 4185 0b84 aafb 2d45 bd56 66dc  ..+.A.....-E.Vf.
-00001410: d9cf 6693 6846 bec1 e6b6 8413 6728 a45a  ..f.hF......g(.Z
-00001420: 17c8 67f3 debf 5539 167c 7e46 9e46 59b5  ..g...U9.|~F.FY.
-00001430: 545a e18e 172a cfa5 5930 6fa5 b4ce 4043  TZ...*..Y0o...@C
-00001440: 9db0 936b 7ade 86bd 4d12 29d4 7d3f b67e  ...kz...M.).}?.~
-00001450: 0d9c 6627 b184 9ce6 2036 08bf 64ca f1eb  ..f'.... 6..d...
-00001460: 064a c437 dc65 f0dc 39a3 705d a6e8 3015  .J.7.e..9.p]..0.
-00001470: 641b db53 4d54 3aa5 3c50 b5af ca09 23a0  d..SMT:.<P....#.
-00001480: 13fa 0875 b459 9562 2d9d d088 2854 e888  ...u.Y.b-...(T..
-00001490: 7551 806b c8ee 8fe5 286c 45e4 d5ee 3c26  uQ.k....(lE...<&
-000014a0: 6cd5 e742 12f1 125a eab3 d344 ae1c bf8e  l..B...Z...D....
-000014b0: 048d f5a2 57fa 78a5 61cb 0ba8 d557 3028  ....W.x.a....W0(
-000014c0: f4a2 b430 ae01 054a 1e2c 48fb b96a f678  ...0...J.,H..j.x
-000014d0: 176e 2cb4 5a53 0022 cfe5 209d 0c49 d2b8  .n,.ZS.".. ..I..
-000014e0: e557 dae9 eb8d abf7 c3f2 8e72 dd74 aa7a  .W.........r.t.z
-000014f0: 0f48 4a25 ff3b 68e4 1785 c595 d4da 12ba  .HJ%.;h.........
-00001500: e59f e81c 1c5b 5e9b 8caa 4943 3f9c f9a4  .....[^...IC?...
-00001510: 7dfa 9c87 fea9 1fc6 d396 0f3e c27d 846d  }..........>.}.m
-00001520: 1a38 935b b8cc a4a9 d2f4 a661 edbc df0b  .8.[.......a....
-00001530: ea4a ed94 ff70 3c7f 10f3 8c58 383c 83ff  .J...p<....X8<..
-00001540: 54cc 6793 f317 353f 3b35 cff7 6abe f859  T.g...5?;5..j..Y
-00001550: cd9d c0ff a29a e9a6 fb6f 6a8e c297 9bf9  .........oj.....
-00001560: 79dd cca1 3f68 79e6 3fa2 e5e8 4f6f e629  y...?hy.?...Oo.)
-00001570: fdfd 4cbf 0150 4b03 0414 0000 0008 0087  ..L..PK.........
-00001580: 4ee2 406c 2e61 f7fa 0400 00fd 1100 0018  N.@l.a..........
-00001590: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-000015a0: 2f73 6865 6574 332e 786d 6c8d 58db 72e2  /sheet3.xml.X.r.
-000015b0: 3810 7ddf aafd 0797 dfc7 c660 6e29 606a  8.}........`n)`j
-000015c0: c225 9040 a036 7b79 766c 01ae b191 d756  .%.@.6{yvl.....V
-000015d0: 4232 5fbf 2dc9 37b5 b449 5e40 569f 6e75  B2_.-.7..I^@V.nu
-000015e0: 9f3e 962d 4fbe bfa5 89f5 4af2 22a6 97a9  .>.-O.....J."...
-000015f0: ed39 1ddb 2297 9046 f1e5 34b5 fffa 73f5  .9.."..F..4...s.
-00001600: 6d64 5b05 0b2e 5190 d00b 99da efa4 b0bf  md[...Q.........
-00001610: cf7e ff6d 72a5 f9cf e24c 08b3 20c2 a598  .~.mr....L.. ...
-00001620: da67 c6b2 1bd7 2dc2 3349 83c2 a119 b980  .g....-.3I......
-00001630: e548 f334 6070 999f dc22 cb49 1009 a734  .H.4`p...".I...4
-00001640: 71bb 9dce c04d 83f8 62cb 0837 f957 62d0  q....M..b..7.Wb.
-00001650: e331 0ec9 8286 2f29 b930 1924 2749 c020  .1..../).0.$'I. 
-00001660: ffe2 1c67 4515 ed2d fa52 bc28 0fae 506b  ...gE..-.R.(..Pk
-00001670: 954f 2bc5 85b4 d4f1 3c5f cb2f 8dc3 9c16  .O+.....<_./....
-00001680: f4c8 9c90 a6ae 4c4d af72 ec8e 953a d350  ......LM.r...:.P
-00001690: 0b64 202b 0df2 9f2f d937 089c 4171 cf71  .d +.../.7..Aq.q
-000016a0: 12b3 7751 6e95 1061 4d9c ebf5 ea5c b3c2  ..wQn..aM....\..
-000016b0: 092f 6516 2d82 bca1 4bd8 fca5 6034 5d04  ./e.-...K...`4].
-000016c0: 2cb0 6713 d181 43ee ce26 510c 2cf2 d65b  ,.g...C..&Q.,..[
-000016d0: 3939 4eed 1fde cd61 6cc3 bc40 fc1d 936b  99N....al..@...k
-000016e0: d11a 5b2c 787e 2209 0919 8940 2ab6 f58b  ..[,x~"....@*...
-000016f0: d2f4 290c 1290 c5a8 dfba 7ce4 3d4f e424  ..).......|.=O.$
-00001700: a3d9 961c d99c 2430 710f 4e5c 37cf 94fe  ......$0q.N\7...
-00001710: e4d1 3710 a7c3 1312 5179 1a41 c8e2 5722  ..7.....Qy.A..W"
-00001720: d1fb 3148 ef5f 9118 0c21 2bb7 4eab 3dae  ..1H._...!+.N.=.
-00001730: 525c 09a5 1d72 2b22 c7e0 2561 739a fc13  R\...r+"..%as...
-00001740: 47ec 3cb5 214e 39f7 07bd ae49 7c3a 33c8  G.<.!N9....I|:3.
-00001750: df77 ba7d 1e35 a409 8480 5f2b 8de1 16f0  .w.}.5...._+....
-00001760: 6d2b 0dde c4ff 55ba 0f7c 6734 84fa 42c1  m+....U..|g4..B.
-00001770: 6119 d32b 5da5 13dc 24c2 09fe 4b27 afc3  a..+]...$...K'..
-00001780: c37f e403 5909 1ff8 2f7d baa3 4f17 f2e0  ....Y.../}..O...
-00001790: fe14 5e7c d0b8 7d92 9e07 bc4b 2fde 0059  ..^|..}....K/..Y
-000017a0: 550f 027c 5091 d7ad 5c60 50ba 7c81 08af  U..|P...\`P.|...
-000017b0: 57b9 c1a0 74f3 face c74c 7815 e77c 5015  W...t....Lx..|P.
-000017c0: 3570 3e2b 0a82 caa2 6050 2dd5 7306 9fd0  5p>+....`P-.s...
-000017d0: ee0d 2a37 1854 8bfd 2ff1 ae54 8710 1ebf  ..*7.T../..T....
-000017e0: 7b66 939c 5e2d d859 8048 d8f3 e057 7228  {f..^-.Y.H...Wr(
-000017f0: c527 a7b3 806f 87de 0dac 04ba e2e0 1f35  .'...o.........5
-00001800: 1a84 57c0 eceb ace7 4ddc 5790 7158 426e  ..W.....M.W.qXBn
-00001810: 7548 5745 cc75 444f 452c 7484 af22 963a  uHWE.uDOE,t..".:
-00001820: a2af 2256 3a62 a022 ee74 c450 45ac 75c4  .."V:b.".t.PE.u.
-00001830: 4845 6c74 c458 45f0 ad42 125c 53e6 7554  HElt.XE..B.\S.uT
-00001840: c883 0182 58dd ea10 c4c8 4e47 7888 f8c7  ....X.....NGx...
-00001850: cf21 7b03 0435 e760 8034 b9b8 20ab 5a5b  .!{..5.`.4.. .Z[
-00001860: 70c7 1506 11f1 e9a9 0dbf 0d23 a879 b706  p..........#.y..
-00001870: 08ea dedc 0041 ed5b 1820 a87f 4b03 0435  .....A.[. ..K..5
-00001880: 70a5 43ba a881 7706 086a e0da 0041 edd9  p.C...w..j...A..
-00001890: 1820 88fb 7b03 a4e1 5edc a20f 0608 6277  . ..{...^.....bw
-000018a0: 6b80 2076 7706 0862 f7d1 0041 ecee 0d10  k. vw..b...A....
-000018b0: c4ee 4187 f41a 7615 35c1 462c 9e77 c3d6  ..A...v.5.F,.w..
-000018c0: 03a9 7e08 9a95 062e a034 f8ad 95a6 6d57  ..~......4....mW
-000018d0: 3a04 b565 ae23 5057 163a 0235 65a9 2350  :..e.#PW.:.5e.#P
-000018e0: 4f56 3a02 b5e4 4e47 a08e ac75 046a c846  OV:...NG...u.j.F
-000018f0: 47a0 7edc eb08 6dbb d221 3dc4 d9d6 0041  G.~...m..!=....A
-00001900: a4ed 7488 b65f 5510 fe72 c31f 3ffb 6aa2  ..t.._U..r..?.j.
-00001910: e9a7 87c2 1e0c 90a6 198a 9ee0 196d da9d  .............m..
-00001920: 7cf1 5843 b7ef ad71 766e 9c5d f0c0 e2bd  |.XC...qvn.]....
-00001930: ab51 5d93 8228 6409 1030 3e9b 965a 495b  .Q]..(d..0>..ZI[
-00001940: f974 4532 b953 8c48 216b c588 c4b1 518c  .tE2.S.H!k....Q.
-00001950: 4817 f78a 1149 e201 8ca8 1ebf b945 453d  H....I.......EE=
-00001960: 5b03 0431 b8d3 217d 14e5 5187 f8a8 bd7b  [..1..!}..Q....{
-00001970: 8034 aca2 fa0f 8ab1 2951 e93a bc63 355d  .4......)Q.:.c5]
-00001980: efd5 2f36 7dd1 0a24 e305 80eb d57c d4c3  ../6}..$.....|..
-00001990: 5ddb d82a 4559 0d5e cd9a d59a d728 3e82  ]..*EY.^.....(>.
-000019a0: 5727 a783 48ba 9506 94c6 dc38 bb84 d8b5  W'..H......8....
-000019b0: 8610 932b 6993 1af2 b186 1423 e270 ad18  ...+i......#.p..
-000019c0: b186 dac6 5e43 b0d0 c0ae 6dec a3c2 f66d  ....^C....m....m
-000019d0: a38f d63c b48d adb0 0a93 4333 9343 c1a4  ...<......C3.C..
-000019e0: efa0 1a6f e53c 52cf bc9c d578 5f42 f4a6  ...o.<R....x_B..
-000019f0: d1a8 b043 dbd8 6f7a a3a4 0707 26fe 70ea  ...C..oz....&.p.
-00001a00: 2b69 766b 798d 449a 3849 398b 74b5 e01f  +ivky.D.8I9.t...
-00001a10: 2a20 523b 2374 476e 2b08 3f4b b65f b8f8  * R;#tGn+.?K._..
-00001a20: 41b3 7ee1 aa17 1f8b c51b d2a5 8b3c 84ca  A.~..........<..
-00001a30: b340 169c c82e c84f f1a5 b012 38e5 c269  .@.....O....8..i
-00001a40: d681 4a72 79c2 1463 38ff 8a59 c8eb 9932  ..Jry..c8..Y...2
-00001a50: 3883 5757 67f8 1442 6073 ee38 b0f5 1e29  8.WWg..B`s.8...)
-00001a60: 65d5 0524 c7e3 3e11 f692 5959 9091 fc29  e..$..>...YY...)
-00001a70: fe05 476c 4892 e631 7cf4 10df 3aa6 7646  ..GlH..1|...:.vF
-00001a80: 7396 0731 e307 5119 6c25 a2c0 6542 4e41  s..1..Q.l%..eBNA
-00001a90: f85e 7ec0 b0f2 9b38 9ada f926 ea8a 4374  .^~....8...&..Ct
-00001aa0: fde1 66f6 1f50 4b03 040a 0000 0000 0087  ..f..PK.........
-00001ab0: 4ee2 4000 0000 0000 0000 0000 0000 0009  N.@.............
-00001ac0: 0000 0078 6c2f 7468 656d 652f 504b 0304  ...xl/theme/PK..
-00001ad0: 1400 0000 0800 874e e240 f88e 8c59 f305  .......N.@...Y..
-00001ae0: 0000 2b19 0000 1300 0000 786c 2f74 6865  ..+.......xl/the
-00001af0: 6d65 2f74 6865 6d65 312e 786d 6ced 594b  me/theme1.xml.YK
-00001b00: 6f1b 3710 be17 e87f 58ec bd91 64eb 1119  o.7.....X...d...
-00001b10: 9103 5b8f b88d 9d04 9192 2247 6a97 da65  ..[......."Gj..e
-00001b20: c45d 2e48 ca8e 6e41 722a 0a14 2890 16b9  .].H..nAr*..(...
-00001b30: 1428 7ae9 a128 1aa0 011a b487 fe97 ba48  .(z..(.........H
-00001b40: 90a6 3fa2 43ae b422 252a 7ec0 8734 88ec  ..?.C.."%*~..4..
-00001b50: 8396 fbcd ccc7 19ee 37e4 eaca d507 09f5  ........7.......
-00001b60: 0e31 1784 a52d bf72 a9ec 7b38 0d58 48d2  .1...-.r..{8.XH.
-00001b70: a8e5 df19 f43e b9ec 7b42 a234 4494 a5b8  .....>..{B.4D...
-00001b80: e54f b1f0 af6e 7ffc d115 b425 639c 600f  .O...n.....%c.`.
-00001b90: ec53 b185 5a7e 2c65 b655 2a89 0086 91b8  .S..Z~,e.U*.....
-00001ba0: c432 9cc2 bd11 e309 9270 c9a3 52c8 d111  .2.......p..R...
-00001bb0: f84d 6869 a35c ae97 1244 52df 4b51 026e  .Mhi.\...DR.KQ.n
-00001bc0: 6f8e 4624 c0de df2f fe78 fdc3 d3bf 1e7e  o.F$.../.x.....~
-00001bd0: 09ff fef6 3c46 9742 a054 0a35 1050 de57  ....<F.B.T.5.P.W
-00001be0: 11b0 65a8 b1e1 b8a2 1062 2ada 947b 8788  ..e......b*..{..
-00001bf0: b67c 0817 b2a3 017e 207d 8f22 21e1 46cb  .|.....~ }."!.F.
-00001c00: 2feb 8f5f dabe 5242 5b33 232a d7d8 1a76  /.._..RB[3#*...v
-00001c10: 3dfd 99d9 cd0c c2f1 868e c9a3 6111 b45a  =...........a..Z
-00001c20: ad55 eb3b 857f 0da0 7215 d76d 74eb dd7a  .U.;....r..mt..z
-00001c30: e14f 0350 10c0 4c73 2ea6 cfda 6e73 b753  .O.P..Ls....ns.S
-00001c40: 9b61 0d50 fed5 e1bb d3e8 6c56 2cbc e17f  .a.P......lV,...
-00001c50: 7385 f34e 4dfd 5978 0dca fd57 57f0 bd5e  s..NM.Yx...WW..^
-00001c60: 1bb2 68e1 3528 c7d7 56f0 d56a 63a3 5db5  ..h.5(..V..jc.].
-00001c70: f01a 94e3 eb2b f846 79a7 536d 5878 0d8a  .....+.Fy.SmXx..
-00001c80: 2949 c72b e872 adbe d99e cfb6 808c 18dd  )I.+.r..........
-00001c90: 73c2 9bb5 6aaf b131 73be 40c1 6a28 5697  s...j..1s.@.j(V.
-00001ca0: 0a31 62a9 5cb7 d612 749f f11e 0014 9022  .1b.\...t......"
-00001cb0: 4952 4f4e 333c 4201 2ce6 36a2 64c8 89b7  IRON3<B.,.6.d...
-00001cc0: 4fa2 58aa 3068 0b23 e37e 3e14 8895 2115  O.X.0h.#.~>...!.
-00001cd0: d113 0127 996c f99f 6508 1e8f 85d7 972f  ...'.l..e....../
-00001ce0: 5e1c 3f7a 7efc e8b7 e3c7 8f8f 1ffd 627a  ^.?z~.........bz
-00001cf0: b7ec f650 1a99 766f 7efc fadf ef1e 7aff  ...P..vo~.....z.
-00001d00: fcfa fd9b 27df e4a1 97f1 c2c4 bffa f98b  ....'...........
-00001d10: 57bf fff9 36f7 f030 19b4 be7d f6ea f9b3  W...6..0...}....
-00001d20: 974f bf7a fdd3 1387 f71d 8e86 267c 4012  .O.z........&|@.
-00001d30: 2cbc 1bf8 c8bb cd12 98a0 ce8e cd07 0ff9  ,...............
-00001d40: d92c 0631 2296 058a c1b7 c375 57c6 16f0  .,.1"......uW...
-00001d50: c614 5117 6e17 db29 bccb 4147 5cc0 6b93  ..Q.n..)..AG\.k.
-00001d60: fb16 d77e cc27 9238 225f 8f13 0b78 c018  ...~.'.8"_...x..
-00001d70: dd65 dc99 80eb 2a96 91e1 c124 8ddc c1f9  .e....*....$....
-00001d80: c4c4 dd46 e8d0 15bb 8d52 abc0 dd49 0602  ...F.....R...I..
-00001d90: 4a5c 2edb 31b6 68de a228 9528 c229 969e  J\..1.h..(.(.)..
-00001da0: bac7 c618 3b66 778f 102b af07 24e0 4cb0  ....;fw..+..$.L.
-00001db0: 91f4 ee11 6f17 1167 4a06 6468 2da4 85d1  ....o..gJ.dh-...
-00001dc0: 1e49 a02e 5317 4128 b595 9b83 bbde 2ea3  .I..S.A(........
-00001dd0: ae59 77f0 a18d 84c7 0251 07f9 01a6 561a  .Yw......Q....V.
-00001de0: afa1 8944 89cb e500 25d4 4cf8 3e92 b18b  ...D....%.L.>...
-00001df0: 647f ca03 13d7 1512 2a1d 61ca bc6e 8885  d.......*.a..n..
-00001e00: 70d9 dce4 305f a3e8 d741 43dc 653f a0d3  p...0_...AC.e?..
-00001e10: c446 7249 c62e 9ffb 8831 13d9 61e3 768c  .FrI.....1..a.v.
-00001e20: 92cc 85ed 9334 36b1 9f8a 312c 51e4 dd62  .....46...1,Q..b
-00001e30: d205 3f60 f613 a2ae a10e 285d 5bee bb04  ..?`......(][...
-00001e40: 5be5 3e59 08ee 807c 9a94 160b 44dd 9970  [.>Y...|....D..p
-00001e50: 472d af61 66ad dffe 948e 10d6 2a03 ea6e  G-.af.......*..n
-00001e60: 8976 42d2 1315 3c8f 70f1 daed 607e 31aa  .vB...<.p...`~1.
-00001e70: ed76 6ce5 fde5 d9f4 7a87 13e7 53b3 b7a4  .vl.....z...S...
-00001e80: d2eb 70ff 436d eea0 497a 0bc3 e3b0 da9b  ..p.Cm..Iz......
-00001e90: 3e48 f307 69f6 df7b 695e f72c 5fbc 202f  >H..i..{i^.,_. /
-00001ea0: 3418 e459 ed02 f3fd b6de 7d27 6b37 df23  4..Y......}'k7.#
-00001eb0: 4269 5f4e 29de 177a ff2d a0f3 843d 1854  Bi_N)..z.-...=.T
-00001ec0: 76fa fc89 8bc3 5816 c357 f524 4300 0b17  v.....X..W.$C...
-00001ed0: 71a4 6d3c cee4 e744 c6fd 1865 b077 aff8  q.m<...D...e.w..
-00001ee0: ca49 2466 ae23 e165 4cc0 9951 0f3b 7d2b  .I$f.#.eL..Q.;}+
-00001ef0: 3c9d 2407 2ccc cf9c 958a 3a5f e6e2 2190  <.$.,.....:_..!.
-00001f00: 5c8c 976b c538 9c17 648e ae37 16e7 a8c2  \..k.8..d..7....
-00001f10: bd66 1be9 f3ee 9c80 b23d 0b09 2398 4d62  .f.......=..#.Mb
-00001f20: d341 a231 1f54 49d2 a76b 489a 8384 9ed9  .A.1.TI..kH.....
-00001f30: 85b0 683a 585c 56ee e7a5 5a61 01d4 8aaa  ..h:X\V...Za....
-00001f40: c0d6 c883 0d55 cbaf 55c1 048c e0d0 8428  .....U..U......(
-00001f50: 0e55 9df2 52cf abab 8b79 9195 5e97 4c6b  .U..R....y..^.Lk
-00001f60: 0594 e1fd c66c 052c 2add 545c d74e 4fcd  .....l.,*.T\.NO.
-00001f70: 2e5f 6aa7 a8b4 45c2 586e 3609 9d19 ddc3  ._j...E.Xn6.....
-00001f80: 448c 423c 5b9d 6af4 3434 ce5a ebe6 a2a4  D.B<[.j.44.Z....
-00001f90: 163d 958a 592e 0c1a 8dcb 6f63 71de 5a83  .=..Y.....ocq.Z.
-00001fa0: ddb2 36d0 d454 0a9a 7a47 2dbf be59 8325  ..6..T..zG-..Y.%
-00001fb0: 13a0 ace5 8fe0 ec0e 5f93 0cd6 8e50 5b5a  ........_....P[Z
-00001fc0: 4423 780f 1648 9e3f f0e7 5196 8c0b d941  D#x..H.?..Q....A
-00001fd0: 22ce 13ae 4527 5783 8448 cc3d 4a92 96af  "...E'W..H.=J...
-00001fe0: a65f 9481 a65a 4334 b7ca 0608 c23b 4bae  ._...ZC4.....;K.
-00001ff0: 09b2 f2ae 9183 a2db 45c6 a311 0ea4 5976  ........E.....Yv
-00002000: 6344 653a bf04 85cf b5c2 7957 9b9f 1fac  cDe:......yW....
-00002010: 2cd9 04ca dd8f c323 6f48 27fc 3682 2556  ,......#oH'.6.%V
-00002020: 6b54 5402 4322 e005 4f25 cf66 48e0 9d64  kTT.C"..O%.fH..d
-00002030: 2164 8bf5 b7d4 9866 b26b be14 d46b 281f  !d.....f.k...k(.
-00002040: 4734 8bd1 aca3 9862 9ec3 b594 1774 f455  G4.....b.....t.U
-00002050: 9103 e36a 3667 48a8 9192 5923 1c46 aac1  ...j6gH...Y#.F..
-00002060: 9a49 b5ba 69d1 3572 0e6b bbee c946 2a73  .I..i.5r.k...F*s
-00002070: 8668 2e7a a6a5 2aaa 6bba 55cc 8a30 6f03  .h.z..*.k.U..0o.
-00002080: 4bb9 3c5f 9337 58cd 530c edd2 ecf0 b974  K.<_.7X.S......t
-00002090: 2f4b 6e73 ae75 4bfb 84a2 4b40 c28b fc39  /Kns.uK...K@...9
-000020a0: baee 291a 8241 6d11 cca2 a618 afca b0d2  ..)..Am.........
-000020b0: ecd9 a8dd 3be6 133c 81da 699a 84a1 faf5  ....;..<..i.....
-000020c0: b9db a5bc 153d c219 0e06 cfd5 f9c1 6e79  .....=........ny
-000020d0: d5c2 d068 beaf d499 d6bf 6198 bf2f b0e1  ...h......a../..
-000020e0: 7d10 8f0e bcc9 9d50 2972 81d0 a0ed ff00  }......P)r......
-000020f0: 504b 0304 1400 0000 0800 874e e240 ef84  PK.........N.@..
-00002100: c8be 7d0a 0000 1651 0000 0d00 0000 786c  ..}....Q......xl
-00002110: 2f73 7479 6c65 732e 786d 6cd5 5ceb 8fdb  /styles.xml.\...
-00002120: 5815 ff8e c4ff 60b9 820f 8899 d88e 3349  X.....`.......3I
-00002130: 6627 533a 99b1 b4d2 8256 6a91 9000 559e  f'S:.....Vj...U.
-00002140: c499 b170 e2e0 38dd 1910 52a1 5b66 1f2a  ...p..8...R.[f.*
-00002150: 122a 5058 adc4 b2ab 523e d001 16c4 5665  .*PX....R>....Ve
-00002160: dbfe 334d 66e6 13ff c29e 7bfd b8e7 3ad7  ..3Mf.....{...:.
-00002170: 893b 1dc7 9e8e d4f8 75de bf7b ce7d d91b  .;......u..{.}..
-00002180: 570f fa8e 74cb f246 b63b 68c9 eaaa 224b  W...t..F.;h..."K
-00002190: d6a0 e376 edc1 5e4b fefe 0d63 a521 4b23  ...v..^K...c.!K#
-000021a0: df1c 744d c71d 582d f9d0 1ac9 5737 bffe  ..tM..X-....W7..
-000021b0: b58d 917f e858 d7f7 2dcb 9780 c560 d492  .....X..-....`..
-000021c0: f77d 7fb8 5ea9 8c3a fb56 df1c adba 436b  .}..^..:.V....Ck
-000021d0: 0077 7aae d737 7d38 f5f6 2aa3 a167 99dd  .wz..7}8..*..g..
-000021e0: 1121 ea3b 154d 51d6 2a7d d31e c801 87f5  .!.;.MQ.*}......
-000021f0: 7e27 0b93 bee9 fd64 3c5c e9b8 fda1 e9db  ~'.....d<\......
-00002200: bbb6 63fb 8794 972c f53b eb6f ee0d 5ccf  ..c....,.;.o..\.
-00002210: dc75 40d5 03af 1971 86c3 19d6 7dbb e3b9  .u@....q....}...
-00002220: 23b7 e7af 02ab 8adb ebd9 1d6b 4643 75ad  #..........kFCu.
-00002230: e259 b76c e29d a6bc b931 18f7 8dbe 3f92  .Y.l.....1....?.
-00002240: 3aee 78e0 b764 3dbe 2405 77de ecc2 4555  :.x..d=.$.w...EU
-00002250: 9602 a3db 6e17 d4b8 297d 4bba f2ed 2b57  ....n...)}K...+W
-00002260: 949b d21b e4f8 472b f8ec 9b3f 1dbb fe1b  ......G+...?....
-00002270: 2bc1 0f7d e23b 3725 b912 89c2 7cb5 24df  +..}.;7%....|.$.
-00002280: 80e8 ff2f 1e06 0758 cccc 2d2c 75e6 6670  .../...X..-,u.fp
-00002290: 2193 12d5 a412 a1d4 5525 611f bbc0 71bf  !.......U%a...q.
-000022a0: 7a75 be91 7a92 ff8c b2d4 7b11 f799 bba1  zu..z.....{.....
-000022b0: 9da9 f7e7 2853 09a3 bbb9 d173 072c c81a  ....(S.....s.,..
-000022c0: 8932 b9b2 b931 fa99 74cb 74a0 99a8 2442  .2...1..t.t...$B
-000022d0: 1dd7 713d c907 b443 94e9 9581 d9b7 8227  ..q=...C.......'
-000022e0: 4e1e bf7f f2f4 057d 6adf f446 d048 02c2  N......}j..F.H..
-000022f0: aa4e aed1 2612 3ed9 b701 b0e4 6225 9091  .N..&.>.....b%..
-00002300: 2ec9 dbdb 6dc9 86d1 6c2b d070 0845 bee2  ....m...l+.p.E..
-00002310: 42c3 94fc 25c5 86d5 ea4a 4ee2 ea1a 3123  B...%....JN...1#
-00002320: cf88 8d49 5c05 f808 8d83 9829 8691 c997  ...I\......)....
-00002330: d405 8b21 b240 6003 0436 b279 33a3 c039  ...!.@`..6.y3..9
-00002340: d619 06b1 ef22 addb c5ee 6ccc 04af 9a49  ....."....l....I
-00002350: 969a b5b9 d958 1a6a dc61 f0ea 06f9 cb24  .....X.j.a.....$
-00002360: 32a3 2f39 f36a 799b c749 a3ae e35a c205  2./9.jy..I...Z..
-00002370: 3b93 9386 9c19 2694 0b96 3607 9555 a36a  ;.....&...6..U.j
-00002380: d4b3 65ca f384 0d99 16e2 8408 ace6 8793  ..e.............
-00002390: 5981 c6b5 fa76 8eed 4e20 d020 ff08 5e17  Y....v..N . ..^.
-000023a0: 169f 8c2e 9d13 bfe5 59f7 4a45 fcf5 0d83  ........Y.JE....
-000023b0: faad 5e6c d844 5e7c a502 fe1a 46e5 e13c  ..^l.D^|....F..<
-000023c0: 9c43 9a3c dc26 c71f be7c 769f 5ceb 08ba  .C.<.&...|v.\...
-000023d0: 56c2 5ed4 7938 5046 23e8 f9d9 8e13 77f8  V.^.y8PF#.....w.
-000023e0: a19e 0457 3637 60f0 e15b dec0 80db 5278  ...W67`..[....Rx
-000023f0: 7ce3 7008 3dc1 018c 9388 7615 42b9 f0e9  |.p.=.....v.B...
-00002400: 3dcf 3c54 355a 01b2 118c 5cc7 ee12 2df6  =.<T5Z....\...-.
-00002410: dab4 ff19 a61e c368 d7db 3b44 ee6e 78c3  .......h..;D.nx.
-00002420: 1e74 ad03 0b06 246b b4cf 5941 0a67 552e  .t....$k..YA.gU.
-00002430: 290b 473a 4731 b149 3b5b cd76 ce26 c5b2  ).G:G1.I;[.v.&..
-00002440: c081 4b93 d56e 3729 2497 e043 cd80 bfe5  ..K..n7)$..C....
-00002450: f8f0 5a8d fc2d 4756 7b6d c758 16dc 69f3  ..Z..-GV{m.X..i.
-00002460: c931 5461 ab82 91af 6f93 5905 65b5 de6c  .1Ta....o.Y.e..l
-00002470: 361b ea5a a3d1 68ea 5575 f9f2 6b20 bf59  6..Z..h.Uu..k .Y
-00002480: 6d34 d734 5043 c93b a4b3 f657 417c bd56  m4.4PC.;...WA|.V
-00002490: 6bd4 d4a6 a6ab 7937 9550 fe92 ccac 151c  k.....y7.P......
-000024a0: 6624 bf90 3023 f985 8499 8e07 f26f cd6b  f$..0#.......o.k
-000024b0: 0587 19c9 2f24 cc48 7e21 61ae e75c 87c2  ..../$.H~!a..\..
-000024c0: a451 2f38 cc48 7e21 6146 f20b 0933 9d19  .Q/8.H~!aF...3..
-000024d0: cabf 35c3 2248 a1b5 19c9 2f24 cc48 7e21  ..5."H..../$.H~!
-000024e0: 615e 5217 00d6 8b0a 0d33 925f 4898 91fc  a^R......3._H...
-000024f0: d70c 331d cbc2 e879 d7f5 bab0 b828 850b  ..3....y.....(..
-00002500: 6664 0d2d b8b4 b9e1 583d 1f86 ab9e bdb7  fd.-....X=......
-00002510: 4f7e 7d77 4806 afae efc3 6adc e646 d736  O~}wH.....j..F.6
-00002520: f7dc 81e9 c061 25a2 887e 0925 2c4a c2fa  .....a%..~.%,J..
-00002530: 634b f6f7 61fd 309a d90f 0773 5b1a f923  cK..a.0....s[..#
-00002540: 05a0 421e 0d65 64a4 a0fa 5075 3212 80e2  ..B..ed...Pu2...
-00002550: 91de 1929 0223 17db 0806 88bc 1349 e95b  ...).#.......I.[
-00002560: 5d7b dc8f 8d8f bbd1 81cb 881f 7313 1137  ]{..........s..7
-00002570: 139d 8c54 f4ba aed4 f59a b616 f83c ab79  ...T.........<.y
-00002580: 911d a210 b219 f7ac 2144 14d9 4288 0832  ........!D..B..2
-00002590: 8610 515c 848d 6cb6 38ab 8d88 229b 8d88  ..Q\..l.8..."...
-000025a0: 20a3 8d88 e255 6dec ba63 5877 8ff1 1836   ....Um..cXw...6
-000025b0: 46c4 50d0 1817 d2cc dab9 9044 60e9 429a  F.P........D`.B.
-000025c0: acb6 2e68 9262 3986 018b 7174 2e1d 52d9  ...h.b9...qt..R.
-000025d0: 79da a5b0 a570 ed7d b1cd dce3 f3d4 08d3  y....p.}........
-000025e0: 2d24 ef8e e538 d749 9afd 412f cee0 3a49  -$...8.I..A/..:I
-000025f0: e107 3db4 2f01 768c 9035 6bb2 f581 1cc2  ..=./.v..5k.....
-00002600: a467 7818 a4eb e004 fcc6 11e9 741f c122  .gx.........t.."
-00002610: 2ac9 1c0e 9d43 03b8 53de c119 0860 675b  *....C..S....`g[
-00002620: b4be b0f3 6b8e bd37 e85b 98e0 6dcf f5ad  ....k..7.[..m...
-00002630: 8e4f f7b7 28a0 bc19 3d42 b6bd f876 872c  .O..(...=B...v.,
-00002640: e877 80c2 f268 c538 e825 55a5 5b12 2e85  .w...h.8.%U.[...
-00002650: aa50 bf17 87a2 1c4e a59b 642e 8553 75ba  .P.....N..d..Su.
-00002660: efe6 52a8 8a9a 224c b3a4 34c5 20fe df1b  ..R..."L..4. ...
-00002670: f777 2dcf a09b b358 f321 ab19 ec6c 098d  .w-....X.!...l..
-00002680: 0b69 0c33 0697 4c63 94ee c0dd 2cdd 01b6  .i.3..Lc....,...
-00002690: 69aa 4af1 3197 ce72 4858 c8a7 303c bf64  i.J.1..rHX..0<.d
-000026a0: 3e85 91e6 25d3 9824 5d71 d19b 8b82 025b  >...%..$]q.....[
-000026b0: 9a8a 800b 870c b890 e9e6 0197 5339 5fe0  ............S9_.
-000026c0: c20e 3bb1 574b a422 a90b a2c0 43d7 a62c  ..;.WK."....C..,
-000026d0: 5e4c 5311 a29e 59c5 e556 0195 740c 43af  ^LS...Y..V..t.C.
-000026e0: 4245 60d8 845e d81c 9573 4623 e902 864a  BE`..^...sF#...J
-000026f0: 414a 654a 41da 2f4e 2954 e239 a50a f514  AJeJA./N)T.9....
-00002700: aae2 90ca 99a7 e07a 719e 4a2b 8370 7d8e  .......zq.J+.p}.
-00002710: 52c6 32f3 5d5a dd83 eb65 5111 153a 3864  R.2.]Z...eQ..:8d
-00002720: a19d 9f4c b6f2 1fa1 9172 168e 4051 d980  ...L.....r..@Q..
-00002730: dc57 4e1d 5186 83a6 5a4e 1d35 e2d3 30e3  .WN.Q...ZN.5..0.
-00002740: 91ee 4249 b544 e126 3d86 4ba0 6569 51c9  ..BI.D.&=.K.eiQ.
-00002750: 451c 205a 525f 625c 96b7 f560 5c72 4343  E. ZR_b\...`\rCC
-00002760: 507f 4e3a df5a 6aae d4b0 965c 5fab 545a  P.N:.Zj....\_.TZ
-00002770: e288 73fd 9cd2 6ac9 757c 4aa5 258e 7869  ..s...j.u|J.%.xi
-00002780: 6b38 c625 c94a e5cf 4444 e34b a065 796b  k8.%.J..DD.K.eyk
-00002790: 0fc2 a556 deda 83b5 2c6f ed41 f912 f695  ...V....,o.A....
-000027a0: 5f06 5c96 b7f6 e088 97b7 f660 2dcb 5b7b  _.\........`-.[{
-000027b0: 302e cb5b 7b90 96d5 f2d6 1e14 f12a 1c97  0..[{........*..
-000027c0: b4f6 602d cb5b 7b70 c40b af3d 15bc e61e  ..`-.[{p...=....
-000027d0: acc0 a3c5 f7fa b9d6 dea5 839e 7811 9e58  ............x..X
-000027e0: be78 de24 a026 6599 8e5c d04c 2bdd d2c0  .x.$.&e..\.L+...
-000027f0: 2deb 238e 10f0 6802 21e9 d548 9f80 61b0  -.#...h.!..H..a.
-00002800: bc0f 58a1 ec83 49b7 b99c 815d c439 5985  ..X...I....].9Y.
-00002810: 435d e1f2 2be9 8a20 0087 5c6b 12eb 9adc  C]..+.. ..\k....
-00002820: ce80 ecce cc8b 7324 de96 f08e 670e 6f58  ......s$....g.oX
-00002830: 07b0 e721 d833 32b3 2301 4903 4b23 5f64  ...!.32.#.I.K#_d
-00002840: d69c 620c 5085 3678 f0db 3b62 0c4a e425  ..b.P.6x..;b.J.%
-00002850: cf96 3c79 f2e4 f4d1 bbf0 2d8d 1047 d2ee  ..<y......-..G..
-00002860: d876 60a3 648c aa19 827b 775e 3ebb 3779  .v`.d....{w^>.7y
-00002870: efd7 671f fd2e 2223 698a 91d1 9780 9364  ..g..."#i......d
-00002880: a7ff 7934 79f2 cb88 8064 0c46 405f 8249  ..y4y....d.F@_.I
-00002890: 129c fce9 3908 99fe 2316 4290 c668 e81b  ....9...#.B..h..
-000028a0: 1d49 9a09 d2ed 87ca 8f23 69e0 4844 495f  .I.......#i.HDI_
-000028b0: 1248 5206 ea21 1ad2 bb62 d2e8 8ef3 199a  .HR..!...b......
-000028c0: ffde 3dbb ff7c fa9b 8791 1cd2 d761 34c1  ..=..|.......a4.
-000028d0: 8bed d136 9bc8 dd5f 7c7e 7afc e2ec c1f1  ...6..._|~z.....
-000028e0: c947 ef9e 26e9 492f 84d1 d37d b149 99d3  .G..&.I/...}.I..
-000028f0: 7fff edec e883 4820 e910 3002 98cb 03ec  ......H ..0.....
-00002900: 2629 4e1f ff75 f2db 0fa6 7f38 9a7e fcf7  &)N..u.....8.~..
-00002910: 888e 9468 4447 a198 a49b 7e72 74f6 e91f  ...hDG....~rt...
-00002920: 230a 3a4f 8848 84ee 3f7d f419 2837 bdfd  #.:O.H..?}..(7..
-00002930: 8897 4667 ef18 6d4d 888f 409c 0448 0a90  ..Fg..mM..@..H..
-00002940: a8f2 1051 8551 0b89 e0d1 9088 c788 2a0c  ...Q.Q........*.
-00002950: 5b48 048f 8644 3c3c 5461 dc42 2278 3424  [H...D<<Ta.B"x4$
-00002960: e2f1 11bc c794 74e1 e9f3 fb93 bb31 3ac0  ......t......1:.
-00002970: 04ec 7518 fd8a a205 2447 4f63 293c 2260  ..u.....$GOc)<"`
-00002980: 282a 2239 fecb c9f1 8398 84c7 8446 b76d  (*"9.........F.m
-00002990: 2615 9b7e 767b fae7 8793 7bbf 9fdc bd33  &..~v{....{....3
-000029a0: fde4 cb98 96c7 0594 0581 b800 f233 b474  .............3.t
-000029b0: 30cf 820c 1f56 11d0 4eff 7534 bdfd bf48  0....V..N.u4...H
-000029c0: 1c1d 5923 1221 a626 0f9f c5cf f390 d084  ..Y#.!.&........
-000029d0: 9098 7c71 1c3f cfa3 4113 a2e1 ecf6 af5e  ..|q.?..A......^
-000029e0: 3e79 1c93 f058 d084 5898 7cf9 f4f4 9f77  >y...X..X.|....w
-000029f0: 00e3 93c7 0fce 3efd f8f4 fdcf 196c e9a8  ......>......l..
-00002a00: 0cd9 246c c49a f20d 6945 9acb 86c7 0af4  ..$l....iE......
-00002a10: 5605 ded4 17b3 e1f1 03dd 4901 9bb5 c56c  V.........I....l
-00002a20: 784c 5585 9812 9813 b74b 8d07 5655 08ac  xLU......K..VU..
-00002a30: 54af c46c 68a7 9d39 37f8 0048 12db a95e  T..lh..97..H...^
-00002a40: 616c 12e5 4a88 bb54 af30 3670 84b2 6855  al..J..T.06p..hU
-00002a50: 0cc7 59ac c489 07dc c031 10e2 33d5 2b8c  ..Y......1..3.+.
-00002a60: 0d8f d9aa 10b3 a95e 616c f88c 5615 2237  .......^al..V."7
-00002a70: d52b 8c0d 8f5c 5d88 5c01 56e2 cc5a e531  .+...\].\.V..Z.1
-00002a80: 0b5f dc12 6036 d52b 8c0d 8f59 d8e8 2760  ._..`6.+...Y..'`
-00002a90: 93ea 15c6 8647 2e6c 6d15 b049 f54a cc06  .....G.lm..I.J..
-00002aa0: dc80 43ad 0bb3 a3c0 2b10 93a0 de90 0f8f  ..C.....+.......
-00002ab0: 21b0 e942 cca6 7a85 b1e1 31ab 0b31 9bea  !..B..z...1..1..
-00002ac0: 15c6 8647 ae2e 446e aa57 181b f00f 364a  ...G..Dn.W....6J
-00002ad0: 885c 8157 0062 a157 8015 6620 c46c aa57  .\.W.b.W..f .l.W
-00002ae0: 181b 1eb3 3521 6653 bdc2 d8f0 c8ad 0991  ....5!fS........
-00002af0: 9bea 15c6 8647 6e8d 2297 8d1d a16b ef93  .....Gn."....k..
-00002b00: 6fe0 d1cd db71 df1e f0d5 b57a e6d8 f16f  o....q.....z...o
-00002b10: c437 5b32 3bfe 2e7d 9f04 a21f 3ef5 b67d  .7[2;..}....>..}
-00002b20: cbf5 298b 96cc 8edf 22ef eb04 5d2d 18a3  ..)....."...]-..
-00002b30: bc35 82d7 6be0 571a 7b76 4bfe f9ce 56bd  .5..k.W.{vK...V.
-00002b40: b9bd 6368 2b0d 65ab b1a2 57ad da4a b3b6  ..ch+.e...W..J..
-00002b50: b5bd 52d3 db5b dbdb 4653 d194 f62f 2032  ..R..[..FS.../ 2
-00002b60: e483 81eb 07aa 7ebe 8ff2 29cd 4a33 f870  ......~...).J3.p
-00002b70: 206c d556 f5f5 9103 9fee f342 6343 e5af   l.V.......BcC..
-00002b80: b36b 2d19 9d04 ea93 165a 01b5 83ff a911  .k-......Z......
-00002b90: 9551 fc41 c3cd af00 504b 0304 1400 0000  .Q.A....PK......
-00002ba0: 0800 874e e240 e692 7e5d 5003 0000 e307  ...N.@..~]P.....
-00002bb0: 0000 1400 0000 786c 2f73 6861 7265 6453  ......xl/sharedS
-00002bc0: 7472 696e 6773 2e78 6d6c 9d55 6d4f d350  trings.xml.UmO.P
-00002bd0: 14fe 6ee2 7f58 6a42 9020 7b01 8c81 adc4  ..n..XjB. {.....
-00002be0: 18f4 8bf1 83c2 6772 d90a 2cd9 dad1 de11  ......gr..,.....
-00002bf0: 49f6 611b 2003 c141 90b7 5103 1821 04d9  I.a. ..A..Q..!..
-00002c00: 8653 b07b 69f6 63ec 6dbb 4ffc 054f 57b6  .S.{i.c.m.O..OW.
-00002c10: 98bb 628c 4dd3 db3e cf39 cf3d e79e 736f  ..b.M..>.9.=..so
-00002c20: fd23 6fa3 11d7 1c27 4a61 810f 30de 3e0f  .#o....'Ja..0.>.
-00002c30: e3e2 f8a0 100a f3d3 0166 7cec f9a3 278c  .........f|...'.
-00002c40: 4bc2 880f a188 c073 0166 9e93 9811 f6fe  K......s.f......
-00002c50: 3dbf 2461 17f8 f252 8099 c138 36e4 764b  =.$a...R...86.vK
-00002c60: c119 2e8a a43e 21c6 f1c0 4c09 6214 61f8  .....>!...L.b.a.
-00002c70: 14a7 dd52 4ce4 5048 9ae1 381c 8db8 7d1e  ...RL.PH..8...}.
-00002c80: cf63 7714 8579 c615 14e2 3c86 7907 bc8c  .cw..y....<.y...
-00002c90: 2bce 8767 e3dc 331b 19ec 6758 bf14 66fd  +..g..3...gX..f.
-00002ca0: 98d5 5379 b223 6bea d14d 2de5 7763 d6ef  ..Sy.#k..M-.wc..
-00002cb0: b670 9b03 54cf 6c90 d5c3 c6d2 baa1 16c8  .p..T.l.........
-00002cc0: 89aa 55de bd10 4202 26c5 9a79 7cd6 382e  ..U...B.&..y|.8.
-00002cd0: 1b07 855f c934 ed18 e631 0559 d90c 4931  ..._.4...1.Y..I1
-00002ce0: 1484 2c21 5c89 13e7 3886 9d8a 0808 bb28  ..,!\...8......(
-00002cf0: 5356 c222 2c10 8d4e 0a42 84c6 9028 a279  SV.",..N.B...(.y
-00002d00: 4770 0244 9c09 279d 5038 4807 cc4e c5f9  Gp.D..'.P8H..N..
-00002d10: 2086 bad1 2a2d bc1b f54e 06f8 7824 d21b   ...*-...N..x$..
-00002d20: 6c0e 0f69 432c 5a41 3864 0244 3370 a718  l..iC,ZA8d.D3p..
-00002d30: 8173 0ac6 a8ed 90ec 4f7a 067d fb07 513f  .s......Oz.}..Q?
-00002d40: 77a0 5705 235d a651 92df 352e 4e35 a5d4  w.W.#].Q..5.N5..
-00002d50: 4128 0be4 f223 8dea db97 4675 9146 6d91  A(...#....Fu.Fm.
-00002d60: 3bb8 a6ce 1d5c 7e97 2c29 1d6a cb2a 9877  ;....\~.,).j.*.w
-00002d70: a007 1552 c891 6c1a 38e2 68d1 43ea aab1  ...R..l.8.h.C...
-00002d80: 7d02 c1e8 85ab 9b5a 4653 d6b5 5a0e 5a92  }......ZFS..Z.Z.
-00002d90: 2c57 6e6a 2bb4 a051 af9a c5cd 3bf3 d7e5  ,Wnj+..Q....;...
-00002da0: 73b2 a992 8d75 5bef 6fde cec9 b5f5 1d52  s....u[.o......R
-00002db0: 0c87 68bd 56fb 4cc4 9088 a212 4df7 38b7  ..h.V.L.....M.8.
-00002dc0: cc9f bbf4 ffb6 a437 e14b f427 0612 83f4  .......7.K.'....
-00002dd0: 8c28 3199 08d2 e0d8 ebf1 d1c4 f3a7 2fdf  .(1.........../.
-00002de0: 8cd2 4cd7 6c5c c0c3 3c8a 72f6 db90 3d8c  ..L.l\..<.r...=.
-00002df0: 0951 fb25 610f 68ba c57b 3db4 440c 3605  .Q.%a.h..{=.D.6.
-00002e00: ee46 e2b4 d4b1 676e a90e dcac ef43 adcd  .F....gn.....C..
-00002e10: e227 3892 887c 669d 3dcb 6b86 fc1e 4a4f  .'8..|f.=.k...JO
-00002e20: 321d 2dd4 b66e c849 f334 6517 888e 028c  2.-..n.I.4e.....
-00002e30: 34e5 dc2e ba5e 3ab6 7be0 a6b6 6649 365b  4....^:.{...fI6[
-00002e40: 8976 4088 469a 6b4a 830e abf9 0a0e 77da  .v@.F.kJ......w.
-00002e50: 8c6c 65e0 a651 48cf 900f 49b6 a8a7 4b56  .le..QH...I...KV
-00002e60: 2cea 9156 4d6a e54c 6341 85b8 f4bd a20d  ,..VMj.LcA......
-00002e70: eac5 affa ee91 a6ca 9a02 1d6f 99c1 a779  ...........o...y
-00002e80: fddd 54ab 8de5 f55b 4725 0920 b890 2f8b  ..T....[G%. ../.
-00002e90: 7044 773d f07a 86f5 cc26 9070 6c58 991f  pDw=.z...&.plX..
-00002ea0: 7e20 4a1a 84c1 0470 23d7 b632 f22b 66fe  ~ J....p#..2.+f.
-00002eb0: 9414 0ff5 d52d 4dcd 3683 b800 5edf bd26  .....-M.6...^..&
-00002ec0: c9fd bee6 6581 b59c 9eaf 5a78 331a 7d31  ....e.....Zx3.}1
-00002ed0: ab95 5760 2658 5828 4e5b 95c8 97c6 c15e  ..W`&XX(N[.....^
-00002ee0: 2b02 f003 7ffb 690d e4f2 1b58 6a95 8a56  +.....i....Xj..V
-00002ef0: bd80 5299 9552 2355 074d 4d91 cd93 bac3  ..R..R#U.MM.....
-00002f00: afc5 b1b6 5e7a 1d1d ad7c b495 ddaa 4ebd  ....^z...|....N.
-00002f10: ecfb 8766 76c3 4f9a fd0d 504b 0304 1400  ...fv.O...PK....
-00002f20: 0000 0800 874e e240 68c7 46ac 1002 0000  .....N.@h.F.....
-00002f30: 5504 0000 0f00 0000 786c 2f77 6f72 6b62  U.......xl/workb
-00002f40: 6f6f 6b2e 786d 6c8d 54cb 6ed3 4014 dd23  ook.xml.T.n.@..#
-00002f50: f10f d6ec 9df1 2369 1e8a 53c5 4d2c 2a35  ......#i..S.M,*5
-00002f60: 5515 420a 2b34 b5c7 f1a8 f68c 3533 6952  U.B.+4......53iR
-00002f70: 21f8 01f6 ec91 107f c086 055f 8384 fa17  !.........._....
-00002f80: dcb1 9334 a880 bc1a df3b e79e 7bee c333  ...4.....;..{..3
-00002f90: 3cdd 16b9 7547 a562 8207 c86d 39c8 a23c  <...uG.b...m9..<
-00002fa0: 1609 e3ab 00bd 5a44 760f 594a 139e 905c  ......ZDv.YJ...\
-00002fb0: 701a a07b aad0 e9e8 f9b3 e146 c8db 1b21  p..{.......F...!
-00002fc0: 6e2d 20e0 2a40 99d6 e500 6315 67b4 20aa  n- .*@....c.g. .
-00002fd0: 254a cae1 2615 b220 1a4c b9c2 aa94 9424  %J..&.. .L.....$
-00002fe0: 2aa3 5417 39f6 1ce7 0417 8471 5433 0c64  *.T.9......qT3.d
-00002ff0: 130e 91a6 2ca6 1311 af0b ca75 4d22 694e  ....,......uM"iN
-00003000: 34c8 5719 2b15 1a0d 5396 d365 5d91 45ca  4.W.+...S..e].E.
-00003010: f292 14a0 7b9b 232b 274a 4f13 a669 1220  ....{.#+'JO..i. 
-00003020: 1f4c b1a1 8f8e 0eb2 e4ba 0cd7 2c87 dbbe  .L..........,...
-00003030: ef78 088f 0e45 5e49 304c b54b 4637 ead1  .x...E^I0L.KF7..
-00003040: 6f4c 6bc3 7822 36d7 2cd1 5980 3cc7 eb41  oLk.x"6.,.Y.<..A
-00003050: 0f6b df0b ca56 9986 b676 db5d e027 b166  .k...V...v.].'.f
-00003060: 7774 416e 0066 d8f1 1163 d516 60ae 4e8b  wtAn.f...c..`.N.
-00003070: 579a 3f3c 7cfd f4f0 f91b 0cc0 f4ec 1c74  W.?<|..........t
-00003080: 7920 72c0 e043 9e27 aea1 3886 fffa f2fd  y r..C.'..8.....
-00003090: e78f 8f76 420b 7114 e21e 8554 59ff 1102  ...vB.q....TY...
-000030a0: d487 34d0 9c43 1abf 525a 5d81 bc98 e4f1  ..4..C..RZ].....
-000030b0: 95b4 cc61 f4b8 7dd7 f1fa 0641 b7fa 42e9  ...a..}....A..B.
-000030c0: eab4 d692 05e8 5dd8 e985 8edf f7ec 76e4  ......].......v.
-000030d0: 4676 dbed 3b76 189e b4ed ce24 f23b 5d77  Fv..;v.....$.;]w
-000030e0: 7236 ed44 eff7 c3df 1ac6 f4c9 0614 2c96  r6.D..........,.
-000030f0: 4289 54b7 6251 e07a f84f f6c8 ede1 2a9a  B.T.bQ.z.O....*.
-00003100: 12bd 96b0 9ea3 61cd 3630 de68 e73d 38d3  ......a.60.h.=8.
-00003110: dab1 6bf1 1f09 06f3 8929 6517 fd3f e04b  ..k......)e..?.K
-00003120: f83d 72da 101c 2d1b 02cf 2e67 8b59 43ec  .=r...-....g.YC.
-00003130: c574 f1f6 3a6a 0a1e cfc2 c9b8 397e 3c9f  .t..:j......9~<.
-00003140: 8fdf 2ca6 aff7 29f0 5f1b 8a61 e6b0 c4fb  ..,...)._..a....
-00003150: c9e3 fd8b 30fa 0d50 4b03 040a 0000 0000  ....0..PK.......
-00003160: 0087 4ee2 4000 0000 0000 0000 0000 0000  ..N.@...........
-00003170: 0006 0000 005f 7265 6c73 2f50 4b03 0414  ....._rels/PK...
-00003180: 0000 0008 0087 4ee2 407b 3876 bcff 0000  ......N.@{8v....
-00003190: 00df 0200 000b 0000 005f 7265 6c73 2f2e  ........._rels/.
-000031a0: 7265 6c73 ad92 cf4a c430 10c6 ef82 ef10  rels...J.0......
-000031b0: e6be 4d77 1511 d974 2f22 ec4d 647d 8098  ..Mw...t/".Md}..
-000031c0: 4cff d026 1392 59ed bebd 4151 2cd4 ba07  L..&..Y...AQ,...
-000031d0: 8f99 f9e6 9bdf 7c64 bb1b dd20 5e31 a68e  ......|d... ^1..
-000031e0: bc82 7551 8240 6fc8 76be 51f0 7c78 58dd  ..uQ.@o.v.Q.|xX.
-000031f0: 8248 acbd d503 7954 70c2 04bb eaf2 62fb  .H....yTp.....b.
-00003200: 8483 e63c 94da 2e24 915d 7c52 d032 873b  ...<...$.]|R.2.;
-00003210: 2993 69d1 e954 5040 9f3b 3545 a739 3f63  ).i..TP@.;5E.9?c
-00003220: 2383 36bd 6e50 6eca f246 c69f 1e50 4d3c  #.6.nPn..F...PM<
-00003230: c5de 2a88 7bbb 0671 3885 bcf9 6f6f aaeb  ..*.{..q8...oo..
-00003240: cee0 3d99 a343 cf33 2be4 5491 9d75 6c90  ..=..C.3+.T..ul.
-00003250: 158c 837c a3d8 bf10 f545 0606 39cf 7275  ...|.....E..9.ru
-00003260: 3ecb ef77 4a87 acad 662d 0d45 5c85 9853  >..wJ...f-.E\..S
-00003270: 8adc e55c bf71 2c99 c75c 4e1f 8a25 a0cd  ...\.q,..\N..%..
-00003280: f940 d3d3 e7c2 c191 d15b b4cb 483a 8425  .@.......[..H:.%
-00003290: a2eb ff24 32c7 c4e4 9679 3e35 5f48 72f2  ...$2....y>5_Hr.
-000032a0: 2dab 7750 4b03 040a 0000 0000 0087 4ee2  -.wPK.........N.
-000032b0: 4000 0000 0000 0000 0000 0000 0009 0000  @...............
-000032c0: 0078 6c2f 5f72 656c 732f 504b 0304 1400  .xl/_rels/PK....
-000032d0: 0000 0800 874e e240 20f8 ee19 fb00 0000  .....N.@ .......
-000032e0: d403 0000 1a00 0000 786c 2f5f 7265 6c73  ........xl/_rels
-000032f0: 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e 7265  /workbook.xml.re
-00003300: 6c73 bd93 cb6a c330 1045 f785 fe83 987d  ls...j.0.E.....}
-00003310: 2ddb 6943 0991 b329 856c dbf4 0384 3d7e  -.iC...).l....=~
-00003320: 105b 329a e9c3 7fdf c18b b886 e06e 4c36  .[2..........nL6
-00003330: 8299 41f7 9ed1 45fb c34f d7aa 2f0c d478  ..A...E..O../..x
-00003340: 6720 8962 50e8 725f 34ae 32f0 717a 7d78  g .bP.r_4.2.qz}x
-00003350: 0645 6c5d 615b efd0 c080 0487 ecfe 6eff  .El]a[........n.
-00003360: 86ad 65b9 4475 d393 1215 4706 6ae6 7ea7  ..e.Du....G.j.~.
-00003370: 35e5 3576 9622 dfa3 9349 e943 6759 ca50  5.5v."...I.CgY.P
-00003380: e9de e667 5ba1 4ee3 78ab c35f 0dc8 669a  ...g[.N.x.._..f.
-00003390: ea58 1808 c762 0bea 34f4 e2fc bfb6 2fcb  .X...b..4...../.
-000033a0: 26c7 179f 7f76 e8f8 8a85 a6da 062c de39  &....v.......,.9
-000033b0: c87a 24c2 3654 c806 66ed 4888 415f 8779  .z$.6T..f.H.A_.y
-000033c0: 5a15 8687 565e 73a2 18eb 25fb c735 ed59  Z...V^s...%..5.Y
-000033d0: 32c2 c97d 2cf5 7826 4b0c 9b35 19be 7d38  2..},.x&K..5..}8
-000033e0: 538d c813 c7a5 4592 964c 364b 30e9 8d61  S.....E..L6K0..a
-000033f0: d225 98e4 c630 9798 f4ec 2f66 bf50 4b03  .%...0..../f.PK.
-00003400: 040a 0000 0000 0087 4ee2 4000 0000 0000  ........N.@.....
-00003410: 0000 0000 0000 0014 0000 0078 6c2f 776f  ...........xl/wo
-00003420: 726b 7368 6565 7473 2f5f 7265 6c73 2f50  rksheets/_rels/P
-00003430: 4b03 0414 0000 0008 0087 4ee2 4069 1f49  K.........N.@i.I
-00003440: c5cf 0000 00b8 0100 0023 0000 0078 6c2f  .........#...xl/
-00003450: 776f 726b 7368 6565 7473 2f5f 7265 6c73  worksheets/_rels
-00003460: 2f73 6865 6574 322e 786d 6c2e 7265 6c73  /sheet2.xml.rels
-00003470: ad90 c96a 0331 0c40 ef85 fe83 d13d d64c  ...j.1.@.....=.L
-00003480: 0ea1 9478 7209 855c 43fa 01c2 d62c 74bc  ...xr..\C....,t.
-00003490: 60b9 69f2 f775 2885 0c04 7ae9 51db d393  `.i..u(...z.Q...
-000034a0: b6bb 8b9f d599 b34c 3118 6875 038a 838d  .......L1.hu....
-000034b0: 6e0a 8381 f7d3 dbea 0594 140a 8ee6 18d8  n...............
-000034c0: c095 0576 ddf3 d3f6 c833 953a 24e3 9444  ...v.....3.:$..D
-000034d0: 554a 1003 6329 e915 51ec c89e 44c7 c4a1  UJ..c)..Q...D...
-000034e0: 56fa 983d 951a e601 13d9 0f1a 18d7 4db3  V..=..........M.
-000034f0: c17c cf80 6ec1 5407 6720 1fdc 1ad4 e99a  .|..n.T.g ......
-00003500: eae6 bfd9 b1ef 27cb fb68 3f3d 87f2 6005  ......'..h?=..`.
-00003510: 9efd bccf f455 8fab 54ca 0317 035a a3fb  .....U..T....Z..
-00003520: c9c9 5dbd d5b5 17f0 b153 fb9f 4e36 fa9b  ..]......S..N6..
-00003530: ae2c 8c7e 93ad aeff bb69 e0e2 dfdd 3750  .,.~.....i....7P
-00003540: 4b03 0414 0000 0008 0087 4ee2 40d9 a106  K.........N.@...
-00003550: c4cf 0000 00b8 0100 0023 0000 0078 6c2f  .........#...xl/
-00003560: 776f 726b 7368 6565 7473 2f5f 7265 6c73  worksheets/_rels
-00003570: 2f73 6865 6574 332e 786d 6c2e 7265 6c73  /sheet3.xml.rels
-00003580: ad90 c96a 0331 0c40 ef85 fe83 d13d d664  ...j.1.@.....=.d
-00003590: 0ea1 9478 7209 855c 43fa 01c6 d62c 74bc  ...xr..\C....,t.
-000035a0: 60b9 69f2 f755 2885 0c04 7ae9 51db d393  `.i..U(...z.Q...
-000035b0: b6bb 4b98 d599 0a4f 291a 58eb 0614 4597  ..K....O).X...E.
-000035c0: fc14 0703 efa7 b7d5 0b28 ae36 7a3b a748  .........(.6z;.H
-000035d0: 06ae c4b0 eb9e 9fb6 479a 6d95 211e a7cc  ........G.m.!...
-000035e0: 4a28 910d 8cb5 e657 4476 2305 cb3a 658a  J(.....WDv#..:e.
-000035f0: 52e9 5309 b64a 5806 ccd6 7dd8 81b0 6d9a  R.S..JX...}...m.
-00003600: 0d96 7b06 740b a63a 7803 e5e0 5b50 a76b  ..{.t..:x...[P.k
-00003610: 96cd 7fb3 53df 4f8e f6c9 7d06 8af5 c10a  ....S.O...}.....
-00003620: 3c87 795f ec97 1c27 545b 06aa 06b4 46ff  <.y_...'T[....F.
-00003630: 93e3 bb7a aba5 17f0 b1d3 fa3f 9d5c 0a37  ...z.......?.\.7
-00003640: 5d5e 18fd 265b 2dff bb69 e0e2 dfdd 3750  ]^..&[-..i....7P
-00003650: 4b03 0414 0000 0008 0087 4ee2 4022 d07e  K.........N.@".~
-00003660: 1991 0100 007c 0700 0013 0000 005b 436f  .....|.......[Co
-00003670: 6e74 656e 745f 5479 7065 735d 2e78 6d6c  ntent_Types].xml
-00003680: c595 dd4e c240 1085 ef4d 7c87 666f 0d5d  ...N.@...M|.fo.]
-00003690: c0c4 1843 e142 f452 4dc4 0758 7707 dab0  ...C.B.RM..Xw...
-000036a0: 7fd9 5910 dede e902 46fc c34a 136f dab4  ..Y.....F..J.o..
-000036b0: db39 df39 b3d3 7630 5a19 9d2d 2160 e56c  .9.9..v0Z..-!`.l
-000036c0: c17a 7997 6560 a553 959d 15ec 6972 dbb9  .zy.e`.S....ir..
-000036d0: 6419 4661 95d0 ce42 c1d6 806c 343c 3d19  d.Fa...B...l4<=.
-000036e0: 4cd6 1e30 a36a 8b05 2b63 f457 9ca3 2cc1  L..0.j..+c.W..,.
-000036f0: 08cc 9d07 4b2b 5317 8c88 7419 66dc 0b39  ....K+S...t.f..9
-00003700: 1733 e0fd 6ef7 824b 6723 d8d8 89b5 061b  .3..n..Kg#......
-00003710: 0ec6 3015 0b1d b39b 15dd de38 591a cdb2  ..0........8Y...
-00003720: ebcd 7335 aa60 c27b 5d49 11c9 285f 5af5  ..s5.`.{]I..(_Z.
-00003730: 01d2 71d3 6925 4139 b930 249d 53fd 3888  ..q.i%A9.0$.S.8.
-00003740: 178a c1f8 9780 001a 9b11 b611 72aa 4c2e  ............r.L.
-00003750: b0ac 3c9e 51ce 6f08 f5ca f711 b675 f7d4  ..<.Q.o......u..
-00003760: fb50 29c8 1e44 8877 c250 504e 211e 82f3  .P)..D.w.PPN!...
-00003770: c829 72fe b3ca e146 40dd 5305 aae3 4912  .)r....F@.S...I.
-00003780: 42ac e0cd f38f 6ce9 0234 87ef 7a54 5737  B.....l..4..zTW7
-00003790: 262e 303a d39c f961 e765 92f9 257c a569  &.0:...a.e..%|.i
-000037a0: 184d 3d31 d83b 9a8c 3e80 5058 0244 a3f3  .M=1.;..>.PX.D..
-000037b0: 9dee 6e42 beea f63b 7cff 7ff0 588a 00ea  ..nB...;|...X...
-000037c0: 3106 7a53 b065 0b7b da07 da80 71ad a175  1.zS.e.{....q..u
-000037d0: 0349 f400 39d2 370b 783a 1e3f 0249 e600  .I..9.7.x:.?.I..
-000037e0: f0c5 85f9 b373 f3d6 bb4d 7397 1b51 d95f  .....s...Ms..Q._
-000037f0: f0d3 9022 4fa7 e353 ef0f 7e9d 2f09 37f4  ..."O..S..~./.7.
-00003800: d1f6 1bf0 571f e72d 6fcc 271f 3cfd 3b87  ....W..-o.'.<.;.
-00003810: af50 4b01 0214 0014 0000 0008 0087 4ee2  .PK...........N.
-00003820: 4022 d07e 1991 0100 007c 0700 0013 0000  @".~.....|......
-00003830: 0000 0000 0001 0020 0000 004f 3600 005b  ....... ...O6..[
-00003840: 436f 6e74 656e 745f 5479 7065 735d 2e78  Content_Types].x
-00003850: 6d6c 504b 0102 1400 0a00 0000 0000 874e  mlPK...........N
-00003860: e240 0000 0000 0000 0000 0000 0000 0600  .@..............
-00003870: 0000 0000 0000 0000 1000 0000 5731 0000  ............W1..
-00003880: 5f72 656c 732f 504b 0102 1400 1400 0000  _rels/PK........
-00003890: 0800 874e e240 7b38 76bc ff00 0000 df02  ...N.@{8v.......
-000038a0: 0000 0b00 0000 0000 0000 0100 2000 0000  ............ ...
-000038b0: 7b31 0000 5f72 656c 732f 2e72 656c 7350  {1.._rels/.relsP
-000038c0: 4b01 0214 000a 0000 0000 0087 4ee2 4000  K...........N.@.
-000038d0: 0000 0000 0000 0000 0000 0009 0000 0000  ................
-000038e0: 0000 0000 0010 0000 0000 0000 0064 6f63  .............doc
-000038f0: 5072 6f70 732f 504b 0102 1400 1400 0000  Props/PK........
-00003900: 0800 874e e240 53d3 bb54 4901 0000 7b02  ...N.@S..TI...{.
-00003910: 0000 1000 0000 0000 0000 0100 2000 0000  ............ ...
-00003920: 2700 0000 646f 6350 726f 7073 2f61 7070  '...docProps/app
-00003930: 2e78 6d6c 504b 0102 1400 1400 0000 0800  .xmlPK..........
-00003940: 874e e240 b205 0148 4201 0000 3e02 0000  .N.@...HB...>...
-00003950: 1100 0000 0000 0000 0100 2000 0000 9e01  .......... .....
-00003960: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
-00003970: 786d 6c50 4b01 0214 0014 0000 0008 0087  xmlPK...........
-00003980: 4ee2 40c4 2d55 0328 0100 000e 0200 0013  N.@.-U.(........
-00003990: 0000 0000 0000 0001 0020 0000 000f 0300  ......... ......
-000039a0: 0064 6f63 5072 6f70 732f 6375 7374 6f6d  .docProps/custom
-000039b0: 2e78 6d6c 504b 0102 1400 0a00 0000 0000  .xmlPK..........
-000039c0: 874e e240 0000 0000 0000 0000 0000 0000  .N.@............
-000039d0: 0300 0000 0000 0000 0000 1000 0000 6804  ..............h.
-000039e0: 0000 786c 2f50 4b01 0214 000a 0000 0000  ..xl/PK.........
-000039f0: 0087 4ee2 4000 0000 0000 0000 0000 0000  ..N.@...........
-00003a00: 0009 0000 0000 0000 0000 0010 0000 00a3  ................
-00003a10: 3200 0078 6c2f 5f72 656c 732f 504b 0102  2..xl/_rels/PK..
-00003a20: 1400 1400 0000 0800 874e e240 20f8 ee19  .........N.@ ...
-00003a30: fb00 0000 d403 0000 1a00 0000 0000 0000  ................
-00003a40: 0100 2000 0000 ca32 0000 786c 2f5f 7265  .. ....2..xl/_re
-00003a50: 6c73 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e  ls/workbook.xml.
-00003a60: 7265 6c73 504b 0102 1400 1400 0000 0800  relsPK..........
-00003a70: 874e e240 a000 0b08 7701 0000 1904 0000  .N.@....w.......
-00003a80: 1000 0000 0000 0000 0100 2000 0000 8904  .......... .....
-00003a90: 0000 786c 2f63 6f6d 6d65 6e74 7331 2e78  ..xl/comments1.x
-00003aa0: 6d6c 504b 0102 1400 1400 0000 0800 874e  mlPK...........N
-00003ab0: e240 a000 0b08 7701 0000 1904 0000 1000  .@....w.........
-00003ac0: 0000 0000 0000 0100 2000 0000 2e06 0000  ........ .......
-00003ad0: 786c 2f63 6f6d 6d65 6e74 7332 2e78 6d6c  xl/comments2.xml
-00003ae0: 504b 0102 1400 0a00 0000 0000 874e e240  PK...........N.@
-00003af0: 0000 0000 0000 0000 0000 0000 0c00 0000  ................
-00003b00: 0000 0000 0000 1000 0000 260a 0000 786c  ..........&...xl
-00003b10: 2f64 7261 7769 6e67 732f 504b 0102 1400  /drawings/PK....
-00003b20: 1400 0000 0800 874e e240 5842 137c d402  .......N.@XB.|..
-00003b30: 0000 c10a 0000 1b00 0000 0000 0000 0100  ................
-00003b40: 2000 0000 500a 0000 786c 2f64 7261 7769   ...P...xl/drawi
-00003b50: 6e67 732f 766d 6c44 7261 7769 6e67 312e  ngs/vmlDrawing1.
-00003b60: 766d 6c50 4b01 0214 0014 0000 0008 0087  vmlPK...........
-00003b70: 4ee2 408a e2eb 49d2 0200 00c1 0a00 001b  N.@...I.........
-00003b80: 0000 0000 0000 0001 0020 0000 006a 1200  ......... ...j..
-00003b90: 0078 6c2f 6472 6177 696e 6773 2f76 6d6c  .xl/drawings/vml
-00003ba0: 4472 6177 696e 6732 2e76 6d6c 504b 0102  Drawing2.vmlPK..
-00003bb0: 1400 1400 0000 0800 874e e240 e692 7e5d  .........N.@..~]
-00003bc0: 5003 0000 e307 0000 1400 0000 0000 0000  P...............
-00003bd0: 0100 2000 0000 982b 0000 786c 2f73 6861  .. ....+..xl/sha
-00003be0: 7265 6453 7472 696e 6773 2e78 6d6c 504b  redStrings.xmlPK
-00003bf0: 0102 1400 1400 0000 0800 874e e240 ef84  ...........N.@..
-00003c00: c8be 7d0a 0000 1651 0000 0d00 0000 0000  ..}....Q........
-00003c10: 0000 0100 2000 0000 f020 0000 786c 2f73  .... .... ..xl/s
-00003c20: 7479 6c65 732e 786d 6c50 4b01 0214 000a  tyles.xmlPK.....
-00003c30: 0000 0000 0087 4ee2 4000 0000 0000 0000  ......N.@.......
-00003c40: 0000 0000 0009 0000 0000 0000 0000 0010  ................
-00003c50: 0000 00a5 1a00 0078 6c2f 7468 656d 652f  .......xl/theme/
-00003c60: 504b 0102 1400 1400 0000 0800 874e e240  PK...........N.@
-00003c70: f88e 8c59 f305 0000 2b19 0000 1300 0000  ...Y....+.......
-00003c80: 0000 0000 0100 2000 0000 cc1a 0000 786c  ...... .......xl
-00003c90: 2f74 6865 6d65 2f74 6865 6d65 312e 786d  /theme/theme1.xm
-00003ca0: 6c50 4b01 0214 0014 0000 0008 0087 4ee2  lPK...........N.
-00003cb0: 4068 c746 ac10 0200 0055 0400 000f 0000  @h.F.....U......
-00003cc0: 0000 0000 0001 0020 0000 001a 2f00 0078  ....... ..../..x
-00003cd0: 6c2f 776f 726b 626f 6f6b 2e78 6d6c 504b  l/workbook.xmlPK
-00003ce0: 0102 1400 0a00 0000 0000 874e e240 0000  ...........N.@..
-00003cf0: 0000 0000 0000 0000 0000 0e00 0000 0000  ................
-00003d00: 0000 0000 1000 0000 d307 0000 786c 2f77  ............xl/w
-00003d10: 6f72 6b73 6865 6574 732f 504b 0102 1400  orksheets/PK....
-00003d20: 0a00 0000 0000 874e e240 0000 0000 0000  .......N.@......
-00003d30: 0000 0000 0000 1400 0000 0000 0000 0000  ................
-00003d40: 1000 0000 fd33 0000 786c 2f77 6f72 6b73  .....3..xl/works
-00003d50: 6865 6574 732f 5f72 656c 732f 504b 0102  heets/_rels/PK..
-00003d60: 1400 1400 0000 0800 874e e240 691f 49c5  .........N.@i.I.
-00003d70: cf00 0000 b801 0000 2300 0000 0000 0000  ........#.......
-00003d80: 0100 2000 0000 2f34 0000 786c 2f77 6f72  .. .../4..xl/wor
-00003d90: 6b73 6865 6574 732f 5f72 656c 732f 7368  ksheets/_rels/sh
-00003da0: 6565 7432 2e78 6d6c 2e72 656c 7350 4b01  eet2.xml.relsPK.
-00003db0: 0214 0014 0000 0008 0087 4ee2 40d9 a106  ..........N.@...
-00003dc0: c4cf 0000 00b8 0100 0023 0000 0000 0000  .........#......
-00003dd0: 0001 0020 0000 003f 3500 0078 6c2f 776f  ... ...?5..xl/wo
-00003de0: 726b 7368 6565 7473 2f5f 7265 6c73 2f73  rksheets/_rels/s
-00003df0: 6865 6574 332e 786d 6c2e 7265 6c73 504b  heet3.xml.relsPK
-00003e00: 0102 1400 1400 0000 0800 874e e240 3cb2  ...........N.@<.
-00003e10: 1ca9 f101 0000 0504 0000 1800 0000 0000  ................
-00003e20: 0000 0100 2000 0000 ff07 0000 786c 2f77  .... .......xl/w
-00003e30: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00003e40: 2e78 6d6c 504b 0102 1400 1400 0000 0800  .xmlPK..........
-00003e50: 874e e240 8676 907b d704 0000 7111 0000  .N.@.v.{....q...
-00003e60: 1800 0000 0000 0000 0100 2000 0000 5d0d  .......... ...].
-00003e70: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00003e80: 7368 6565 7432 2e78 6d6c 504b 0102 1400  sheet2.xmlPK....
-00003e90: 1400 0000 0800 874e e240 6c2e 61f7 fa04  .......N.@l.a...
-00003ea0: 0000 fd11 0000 1800 0000 0000 0000 0100  ................
-00003eb0: 2000 0000 7515 0000 786c 2f77 6f72 6b73   ...u...xl/works
-00003ec0: 6865 6574 732f 7368 6565 7433 2e78 6d6c  heets/sheet3.xml
-00003ed0: 504b 0506 0000 0000 1b00 1b00 bf06 0000  PK..............
-00003ee0: 1138 0000 0000                           .8....
+00000210: ce10 8d08 0a40 8b5a 967a 95a1 db62 1e9e  .....@.Z.z...b..
+00000220: a1c0 3aae 25af 6a0d 19da 8245 b3fc f424  ..:.%.j....E...$
+00000230: 150d 13b5 816b 5337 605c 0936 f024 6d99  .....kS7`\.6.$m.
+00000240: 6832 b476 ae61 185b b106 c56d e41d da8b  h2.v.a.[...m....
+00000250: cbda 28ee fcd3 ac70 c3c5 235f 018e 0999  ..(....p..#_....
+00000260: 6005 8e4b ee38 de01 c366 20a2 1e29 c580  `..K.8...f ..)..
+00000270: 6c9e 4cd5 01a4 c050 8102 ed2c a611 c5df  l.L....P...,....
+00000280: 5e07 46d9 3f07 3ae5 c8a9 4ab7 6dfc 4d7d  ^.F.?.:...J.m.M}
+00000290: dc63 b614 7b71 706f 6c39 18db b68d daa4  .c..{qpol9......
+000002a0: 8be1 f353 7cbf b8ba e94e 0d4b bdeb 4a00  ...S|....N.K..J.
+000002b0: ca77 fd54 dcba 85af 7259 823c dfe6 9f2f  .w.T....rY.<.../
+000002c0: ef1f af6f 29fe ada4 5274 d998 30c0 1dc8  ...o)...Rt..0...
+000002d0: c06f 63fb 6c07 e52e b9b8 2ce6 288f 091d  .oc.l.....,.(...
+000002e0: 8764 1292 7141 cf18 9d32 421e 527c 70f5  .d..qA...2B.R|p.
+000002f0: f3f9 0054 fdfa 7f89 f128 24a3 904e 0b92  ...T.....($..N..
+00000300: b071 cc48 7244 3c00 f22e f7cf 1fcf bf00  .q.HrD<.........
+00000310: 504b 0304 1400 0000 0800 874e e240 c42d  PK.........N.@.-
+00000320: 5503 2801 0000 0e02 0000 1300 0000 646f  U.(...........do
+00000330: 6350 726f 7073 2f63 7573 746f 6d2e 786d  cProps/custom.xm
+00000340: 6ca5 9141 6b83 3018 86ef 83fd 07c9 3d26  l..Ak.0.......=&
+00000350: a6d5 d4a2 961a 15c6 0e1b acf3 2e31 b682  .............1..
+00000360: 49c4 c46e 65ec bf2f a5eb c60e bb6c c78f  I..ne../.....l..
+00000370: efe5 e179 bf2f d9bc cac1 3b8a c9f4 5aa5  ...y./....;...Z.
+00000380: 20f0 31f0 84e2 baed d53e 05cf bb0a ae80   .1......>......
+00000390: 676c a3da 66d0 4aa4 e024 0cd8 64b7 37c9  gl..f.J..$..d.7.
+000003a0: e3a4 4731 d95e 18cf 2194 49c1 c1da 718d  ..G1.^..!.I...q.
+000003b0: 90e1 0721 1be3 bbb5 729b 4e4f b2b1 6e9c  ...!....r.NO..n.
+000003c0: f648 775d cf45 a1f9 2c85 b288 601c 213e  .Hw].E..,...`.!>
+000003d0: 1bab 251c bf70 e0c2 5b1f ed5f 91ad e667  ..%..p..[.._...g
+000003e0: 3b53 ef4e a3d3 cd92 4ff8 c9eb a4ed db14  ;S.N....O.......
+000003f0: bc15 212b 8a10 8790 9431 8301 0e72 182f  ..!+.....1...r./
+00000400: 620a f10a 6392 1356 c5db f21d 78e3 394c  b...c..V....x.9L
+00000410: 80a7 1ae9 aadf b1da b18e 763d 8c2f c64e  ..........v=./.N
+00000420: 190d a292 c684 5611 8b96 0bba ddc6 45b5  ......V.......E.
+00000430: ccd9 2a0a 4b5a b010 27e8 3b9b a0ab c33f  ..*.KZ..'.;....?
+00000440: 6d16 579b fba7 0757 b29d b9cd e77e 686b  m.W....W.....~hk
+00000450: 31fd 9023 3824 3020 befb a81f 4494 c4bf  1..#8$0 ....D...
+00000460: d9a0 f3a9 2e8f cc3e 0050 4b03 040a 0000  .......>.PK.....
+00000470: 0000 0087 4ee2 4000 0000 0000 0000 0000  ....N.@.........
+00000480: 0000 0003 0000 0078 6c2f 504b 0304 1400  .......xl/PK....
+00000490: 0000 0800 874e e240 a000 0b08 7701 0000  .....N.@....w...
+000004a0: 1904 0000 1000 0000 786c 2f63 6f6d 6d65  ........xl/comme
+000004b0: 6e74 7331 2e78 6d6c dd93 c14a c330 1cc6  nts1.xml...J.0..
+000004c0: ef82 ef50 2278 7369 3711 9d6d 8797 81e0  ...P"xsi7..m....
+000004d0: c183 3e40 6cb3 b5d0 a625 8943 3d0a 4e70  ..>@l....%.C=.Np
+000004e0: 0c06 1364 1e76 d083 63e8 4086 20ca f065  ...d.v..c.@. ..e
+000004f0: 966e 7b0b d3b5 dd41 100f de06 21e4 fbf2  .n{....A....!...
+00000500: cf97 f04b a297 ce7c 4fa9 61ca dc80 1840  ...K...|O.a....@
+00000510: cba9 40c1 c40a 6c97 540d 707c 54de d806  ..@...l.T.p|T...
+00000520: 0ae3 88d8 c80b 0836 c039 66a0 64ae aee8  .......6.9f.d...
+00000530: 56e0 fb98 70a6 c800 c20c e070 1e16 2164  V...p......p..!d
+00000540: 9683 7dc4 7241 8889 9ca9 04d4 475c 4a5a  ..}.rA......G\JZ
+00000550: 852c a418 d9cc c198 fb1e ccab ea16 f491  .,..............
+00000560: 4b80 a9a3 53ee 0494 6503 7376 d99e 5cdd  K...S...e.sv..\.
+00000570: e830 f1cd 6c20 0bd2 5d0f 5cc6 1742 a1b8  .0..l ..].\..B..
+00000580: 6280 3d0d 2849 fdbe 6d00 55a6 727c 268b  b.=.(I..m.U.r|&.
+00000590: a86c 87b2 3b81 a6ce 2e94 1af2 0cb0 03a4  .l..;...........
+000005a0: a0e5 80f0 448b 4163 3c6a c7a6 e520 ca70  ....D.Ac<j... .p
+000005b0: 6a6b 85cd d883 f3f5 3c3d 5551 8732 15c6  jk......<=UQ.2..
+000005c0: b169 f2bf 5263 7c45 1622 4bb2 957c 18a6  .i..Rc|E."K..|..
+000005d0: 350c ccf5 354d dd15 2f77 d1e0 6df2 fa29  5...5M../w..m..)
+000005e0: ba8d b931 fdea 8cdf fb89 21ea 4331 b81f  ...1......!.C1..
+000005f0: 7fd4 27b7 3dd1 ee2f fce9 e839 6a3e 884e  ..'.=../...9j>.N
+00000600: 6ffa f418 755b 8bc3 c284 064c 01fe 8497  o...u[.....L....
+00000610: 5f4e 78d1 b037 bb96 0f29 bdb1 3f20 1496  _Nx..7...)..? ..
+00000620: 1382 6835 7f27 903d 88e4 4765 8a99 df50  ..h5.'.=..Ge...P
+00000630: 4b03 0414 0000 0008 0087 4ee2 40a0 000b  K.........N.@...
+00000640: 0877 0100 0019 0400 0010 0000 0078 6c2f  .w...........xl/
+00000650: 636f 6d6d 656e 7473 322e 786d 6cdd 93c1  comments2.xml...
+00000660: 4ac3 301c c6ef 82ef 5022 7873 6937 119d  J.0.....P"xsi7..
+00000670: 6d87 9781 e0c1 833e 406c b3b5 d0a6 2589  m......>@l....%.
+00000680: 433d 0a4e 700c 0613 641e 76d0 8363 e840  C=.Np...d.v..c.@
+00000690: 8620 caf0 6596 6e7b 0bd3 b5dd 4110 0fde  . ..e.n{....A...
+000006a0: 0621 e4fb f2cf 97f0 4ba2 97ce 7c4f a961  .!......K...|O.a
+000006b0: cadc 8018 40cb a940 c1c4 0a6c 9754 0d70  ....@..@...l.T.p
+000006c0: 7c54 ded8 060a e388 d8c8 0b08 36c0 3966  |T..........6.9f
+000006d0: a064 aeae e856 e0fb 9870 a6c8 00c2 0ce0  .d...V...p......
+000006e0: 701e 1621 6496 837d c472 4188 899c a904  p..!d..}.rA.....
+000006f0: d447 5c4a 5a85 2ca4 18d9 ccc1 98fb 1ecc  .G\JZ.,.........
+00000700: abea 16f4 914b 80a9 a353 ee04 9465 0373  .....K...S...e.s
+00000710: 76d9 9e5c dde8 30f1 cd6c 200b d25d 0f5c  v..\..0..l ..].\
+00000720: c617 42a1 b862 803d 0d28 49fd be6d 0055  ..B..b.=.(I..m.U
+00000730: a672 7c26 8ba8 6c87 b23b 81a6 ce2e 941a  .r|&..l..;......
+00000740: f20c b003 a4a0 e580 f044 8b41 633c 6ac7  .........D.Ac<j.
+00000750: a6e5 20ca 706a 6b85 cdd8 83f3 f53c 3d55  .. .pjk......<=U
+00000760: 5187 3215 c6b1 69f2 bf52 637c 4516 224b  Q.2...i..Rc|E."K
+00000770: b295 7c18 a635 0ccc f535 4ddd 152f 77d1  ..|..5...5M../w.
+00000780: e06d f2fa 29ba 8db9 31fd ea8c dffb 8921  .m..)...1......!
+00000790: ea43 31b8 1f7f d427 b73d d1ee 2ffc e9e8  .C1....'.=../...
+000007a0: 396a 3e88 4e6f faf4 1875 5b8b c3c2 8406  9j>.No...u[.....
+000007b0: 4c01 fe84 975f 4e78 d1b0 37bb 960f 29bd  L...._Nx..7...).
+000007c0: b13f 2014 9613 8268 357f 2790 3d88 e447  .? ....h5.'.=..G
+000007d0: 658a 99df 504b 0304 0a00 0000 0000 874e  e...PK.........N
+000007e0: e240 0000 0000 0000 0000 0000 0000 0e00  .@..............
+000007f0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00000800: 504b 0304 1400 0000 0800 874e e240 0c07  PK.........N.@..
+00000810: 082d f101 0000 0504 0000 1800 0000 786c  .-............xl
+00000820: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00000830: 7431 2e78 6d6c 8d93 6d6f 9b30 10c7 df4f  t1.xml..mo.0...O
+00000840: da77 407e 5f4c 48b7 3611 5029 89aa 4dda  .w@~_LH.6.P)..M.
+00000850: a4aa dac3 6bc7 1cc1 8aed 63b6 13da 6fbf  ....k.....c...o.
+00000860: 338c 2c6d 26ad 2f10 e7bb e3e7 ff3d 50dc  3.,m&./......=P.
+00000870: 3d19 9d1c c179 85b6 64b3 3463 0958 89b5  =....y..d.4c.X..
+00000880: b2bb 927d ff76 7f75 cb12 1f84 ad85 460b  ...}.v.u......F.
+00000890: 257b 06cf eeaa f7ef 8a1e ddde b700 2121  %{............!!
+000008a0: 82f5 256b 43e8 969c 7bd9 8211 3ec5 0e2c  ..%kC...{...>..,
+000008b0: 451a 7446 043a ba1d f79d 0351 0f1f 19cd  E.tF.:.....Q....
+000008c0: f32c fbc8 8d50 968d 84a5 7b0b 039b 4649  .,...P....{...FI
+000008d0: d8a0 3c18 b061 8438 d022 907e dfaa ce4f  ..<..a.8.".~...O
+000008e0: b4a7 fa4d bcda 899e 6a9d f49c 49dc 8c91  ...M....j...I...
+000008f0: 136f 767d a1cf 28e9 d063 1352 8986 8fd2  .ov}..(..c.R....
+00000900: 2eab 5cf0 c58b 3a8d bc00 fda3 5946 b8fd  ..\...:.....YF..
+00000910: a1bb 2270 47c5 6d95 56e1 7928 7712 04e1  .."pG.m.V.y(w...
+00000920: 2fa7 effb b4ef 7c2a ed1f 1567 0d9a dd70  /.....|*...g...p
+00000930: 08eb 830f 6836 2208 5615 c304 1e1c af8a  ....h6".V.......
+00000940: 5a51 17e3 e813 074d c956 f972 3567 e41f  ZQ.....M.V.r5g..
+00000950: 327e 28e8 fd99 9dc4 916f 11f7 31f0 b92e  2~(......o..1...
+00000960: 5916 59a0 41c6 e627 825e 4758 83d6 255b  Y.Y.A..'.^GX..%[
+00000970: cf3f d0da fc1a a0d1 2624 3f31 cfed 897f  .?......&$?1....
+00000980: 3fac c983 4b6a 68c4 4187 35ea 9faa 0e6d  ?...Kjh.A.5....m
+00000990: c916 6cf2 3d62 ff09 d4ae 0db4 a7d7 694e  ..l.=b........iN
+000009a0: 37e0 2168 65e1 0b1c 4153 b464 f94b 1f51  7.!he...AS.d.K.Q
+000009b0: 28f7 5450 2cbf 2a1c f609 ad06 a546 d2ed  (.TP,.*......F..
+000009c0: 6220 f94e c41d ce97 39d5 2463 7c45 09e4  b .N....9.$c|E..
+000009d0: b961 0965 79f2 1eab ace0 4712 2fe9 21c8  .a.ey.....G./.!.
+000009e0: 8934 ff1f 8912 5e91 66af 4863 7346 7d9d  .4....^.f.HcsF}.
+000009f0: d8c1 57e1 76ca fa44 4343 b767 29a9 7063  ..W.v..DCC.g).pc
+00000a00: e583 1db0 1bbc d482 2d06 1aec 746a e9ff  ........-...tj..
+00000a10: 0212 9fa5 7467 8318 a603 0d60 8cdd 0fce  ....tg.....`....
+00000a20: 388f d30f 5cfd 0650 4b03 040a 0000 0000  8...\..PK.......
+00000a30: 0087 4ee2 4000 0000 0000 0000 0000 0000  ..N.@...........
+00000a40: 000c 0000 0078 6c2f 6472 6177 696e 6773  .....xl/drawings
+00000a50: 2f50 4b03 0414 0000 0008 0087 4ee2 40df  /PK.........N.@.
+00000a60: ec4e b6da 0200 00c7 0a00 001b 0000 0078  .N.............x
+00000a70: 6c2f 6472 6177 696e 6773 2f76 6d6c 4472  l/drawings/vmlDr
+00000a80: 6177 696e 6731 2e76 6d6c ed56 5d6f d330  awing1.vml.V]o.0
+00000a90: 147d afc4 7f88 bcd7 b44d c2d6 3237 c984  .}.......M..27..
+00000aa0: 067b 0324 18e2 7172 13b7 f1e6 f846 f16d  .{.$..qr.....F.m
+00000ab0: 9aee d773 9db4 5583 004d 0878 d922 b5b5  ...s..U..M.x."..
+00000ac0: eef5 b95f e7d8 697c d596 da6b 646d 1598  ..._..i|...kdm..
+00000ad0: 8485 9380 79d2 6490 2bb3 4ed8 d7db 9bf1  ....y.d.+.N.....
+00000ae0: 1be6 5914 2617 1a8c 4cd8 4e5a 7695 be1a  ..Y.&...L.NZv...
+00000af0: c50e 471f 6339 8884 6d6a c36d 56c8 52d8  ..G.c9..mj.mV.R.
+00000b00: 71a9 b21a 2cac 709c 41c9 61b5 5299 e422  q...,.p.A.a.R.."
+00000b10: 43d5 08a4 2c6c 0fab 9e80 aa60 2beb 0a94  C...,l.....`+...
+00000b20: c103 aa7d 024a b699 d407 003c 01d0 d778  ...}.J.....<...x
+00000b30: 4034 bf43 34a5 6669 0cdc 16a2 925a ec60  @4.C4.fi.....Z.`
+00000b40: 835e c365 8b09 93b9 c2ce a7f2 5254 03ab  .^.e........RT..
+00000b50: 970b a429 856c 9ac6 d301 388d 9b3e 16ee  ...).l....8..>..
+00000b60: 2ae9 a93c 6177 6d40 cf1d 4641 c4bc 0ca0  *..<awm@..FA....
+00000b70: cead 7aa4 c947 e12c 08fc ee9b 7914 a3a2  ..z..G.,....y...
+00000b80: 94dd 9e4a 6091 b032 f003 bdf7 f7bb 06df  ...J`..2........
+00000b90: 412b 593a f23c 970e 6b78 90de 3d8d d5e2  A+Y:.<..kx..=...
+00000ba0: 4e53 e852 a1ac a9b6 deef e279 eb5a e44a  NS.R.......y.Z.J
+00000bb0: 1aec fa84 8784 1103 c033 3046 66e8 6a4d  .........30Ff.jM
+00000bc0: 584d 2b07 8aa7 272d a4a3 d1a1 a3d3 6e6c  XM+...'-......nl
+00000bd0: 1844 b361 d97d 90b3 41bb fb7a 2ab0 ca49  .D.a.}..A..z*..I
+00000be0: 858b a505 bd41 b9d0 7285 3ca8 7081 5075  .....A..r.<.p.Pu
+00000bf0: bfa5 a8d7 ca8c 3bfb ec62 125d 906f 6f73  ......;..b.].oos
+00000c00: 5b66 93b9 b314 52ad 0be4 1797 fd86 adca  [f....R.........
+00000c10: b1e0 9733 f234 caaa a5d2 0a77 bc50 792e  ...3.4.....w.Py.
+00000c20: cd82 792b a575 061a ea84 9ddd d0f3 3eec  ..y+.u........>.
+00000c30: 6d92 58a1 f6fb b9f5 6be0 343c 8925 e434  m.X.....k.4<.%.4
+00000c40: 08b1 41f8 2555 8e60 3751 62be e12e 83e7  ..A.%U.`7Qb.....
+00000c50: 0e1a 85eb 3245 a7a9 20db d89e 6be2 d249  ....2E.. ...k..I
+00000c60: e5c8 d5a1 2aa7 8c80 8ee8 4fb8 a3cd aa14  ....*.....O.....
+00000c70: 6be9 9446 4ca1 42c7 ac8b 025c 43f6 30d4  k..FL.B....\C.0.
+00000c80: a3b0 15b1 57bb 0399 b055 9f0b 49c5 4b68  ....W....U..I.Kh
+00000c90: a9cf 4e14 b972 043b 1634 d68b 5eea e395  ..N..r.;.4..^...
+00000ca0: 862d 2fa0 568f 6050 e845 6961 5c03 0a94  .-/.V.`P.Eia\...
+00000cb0: 3c58 90f8 73d5 1cf0 2edc 5868 b5a6 00c4  <X..s.....Xh....
+00000cc0: 9ecb 4142 d927 49e3 965f 6b27 b077 aede  ..AB.'I.._k'.w..
+00000cd0: 4fcb 7bca 75db c9ea 2320 4995 fc1f a091  O.{.u...# I.....
+00000ce0: df14 16d7 526b 4be8 967f a183 30b4 bc35  ....RkK.....0..5
+00000cf0: 1955 9386 7e78 e107 fea5 1ff9 f3d0 7fed  .U..~x..........
+00000d00: 47f3 78da f2bd 9380 9f61 9b86 cee4 162e  G.x......a......
+00000d10: 35a9 aa34 69e0 4cfb 75b7 3c56 d4d5 da69  5..4i.L.u.<V...i
+00000d20: ff78 407f 94f3 fc3f ca39 9cbc a8f9 d9a9  .x@....?.9......
+00000d30: 393a aab9 d3e9 50cd 9de9 2faa 995e f3a7  9:....P.../..^..
+00000d40: ef94 7f7a 3987 f3fe 3a7e b99d 9fd1 ed1c  ...z9...:~......
+00000d50: fae7 073d 9f77 57f1 50cf d19f dece 53fa  ...=.wW.P.....S.
+00000d60: 139a 7e07 504b 0304 1400 0000 0800 874e  ..~.PK.........N
+00000d70: e240 fb5c 74f7 cf04 0000 8911 0000 1800  .@.\t...........
+00000d80: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00000d90: 7368 6565 7432 2e78 6d6c 8d58 5b77 b238  sheet2.xml.X[w.8
+00000da0: 147d 9fb5 e63f b078 ff40 14b5 76a9 dfaa  .}...?.x.@..v...
+00000db0: b76a afae e95c 9e29 4465 1508 1362 6de7  .j...\.)De...bm.
+00000dc0: d7cf 4922 971c f2d5 be60 4cf6 3939 d97b  ..I".....`L.99.{
+00000dd0: 1308 e39f 1f69 62bd 1356 c434 9bd8 9ed3  .....ib..V.4....
+00000de0: b12d 9285 348a b3fd c4fe ebcf d58f 2bdb  .-..4.........+.
+00000df0: 2a78 9045 4142 3332 b13f 4961 ff9c fefe  *x.EAB32.?Ia....
+00000e00: dbf8 44d9 5b71 2084 5b90 212b 26f6 81f3  ..D.[q .[.!+&...
+00000e10: fcda 758b f040 d2a0 7068 4e32 18d9 5196  ..u..@..phN2..Q.
+00000e20: 061c feb2 bd5b e48c 0491 0c4a 13b7 dbe9  .....[.....J....
+00000e30: 0cdc 3488 335b 65b8 66df c941 77bb 3824  ..4.3[e.f..Aw.8$
+00000e40: 0b1a 1e53 9271 9584 9124 e050 7f71 88f3  ...S.q...$.P.q..
+00000e50: a2cc f611 7d2b 5fc4 8213 acb5 aca7 51e2  ....}+_.......Q.
+00000e60: 428d 54f9 3cbf 555f 1a87 8c16 74c7 9d90  B.T.<.U_....t...
+00000e70: a6ae 2aad bdca 913b d2d6 9986 ad44 06b2  ..*....;.....D..
+00000e80: d280 bd1d f31f 9038 87c5 bdc6 49cc 3fe5  .......8....I.?.
+00000e90: 72cb 8208 aff3 9c4e 27e7 9417 4e98 9dab  r......N'...N...
+00000ea0: 6810 e40d 5dc2 e7c7 82d3 7411 f0c0 9e8e  h...].....t.....
+00000eb0: a502 5be6 4ec7 510c 2c0a e92d 4676 13fb  ..[.N.Q.,..-Fv..
+00000ec0: c6bb de8e 6ce8 9788 bf63 722a 1a6d 8b07  ....l....cr*.m..
+00000ed0: af2f 2421 2127 1158 c5b6 8405 5e29 7d13  ./$!!'.X....^)}.
+00000ee0: c00d 7475 446e 0910 1983 90c7 ef64 4e92  ..tuDn.......dN.
+00000ef0: 6462 6fbc 3ed8 e85f 3989 68c3 146e 3547  dbo.>.._9.h..n5G
+00000f00: b35d ceb7 92b6 d932 2b22 bbe0 98f0 394d  .].....2+"....9M
+00000f10: fe89 237e 98d8 23bb ecfb 839e d624 de1f  ..#~..#......$..
+00000f20: 3814 e33b 5d99 35a4 09a4 80ab 95c6 e067  8..;].5........g
+00000f30: dfb6 d2e0 43fe 9e54 f8c0 77ae 8650 4c28  ....C..T..w..PL(
+00000f40: 0939 e7f4 4441 5510 385e 06c1 ef39 c8eb  .9..DAU.8^...9..
+00000f50: 88f4 5fc5 4055 3206 7ecf 31dd ab8b 1379  .._.@U2.~.1....y
+00000f60: 70b3 c928 d1a8 c32e 94e7 01f3 2a4a 48a0  p..(........*JH.
+00000f70: 56d5 8304 5fac c8eb 9621 d038 877c 8308  V..._....!.8.|..
+00000f80: af57 8641 e31c e6f5 9daf 99f0 4ace 45a3  .W.A........J.E.
+00000f90: 5cd4 c0b9 b428 48aa 1605 8d72 aa9e 33b8  \....(H....r..3.
+00000fa0: 40bb 3728 c3a0 514e f64b e25d e50e 693c  @.7(..QN.K.]..i<
+00000fb0: 712b 4cc7 8c9e 2cd8 2680 48d8 c0e0 aa38  q+L...,.&.H....8
+00000fc0: 54e6 53dd 7920 f636 ef1a 6602 8b08 f04d  T.S.y .6..f....M
+00000fd0: 8506 e315 d0fb 3eed 8edd 7770 7178 46cc  ......>...wpqxF.
+00000fe0: 2e22 e66d 444f cfb1 6823 7c1d b16c 23fa  .".mDO..h#|..l#.
+00000ff0: 3a62 d546 0c74 c46d 1b31 d411 eb36 e24a  :b.F.t.m.1...6.J
+00001000: 476c da88 918e b86b 23bc 8e0e b937 403c  Gl.....k#....7@<
+00001010: 1df2 d086 2046 1edb 080f 49f3 7419 f26c  .... F....I.t..l
+00001020: 8020 71b6 0648 5d8b 0bae aaac 0537 5c61  . q..H]......7\a
+00001030: f090 e89e d870 ad3c e421 f166 0608 526f  .....p.<.!.f..Ro
+00001040: 6e80 20f9 1606 08d2 6f69 8020 0157 6d48  n. .....oi. .WmH
+00001050: 1709 786b 8020 01d7 0608 9267 6380 20ee  ..xk. .....gc. .
+00001060: ef0c 909a 7b79 87de 1b20 88dd 0703 04b1  ....{y... ......
+00001070: fb68 8020 769f 0c10 c4ee b301 82d8 ddb6  .h. v...........
+00001080: 21bd 9a5d cd4d b00f cbc7 ddb0 f13c aa9e  !..].M.......<..
+00001090: 8166 a741 0838 0dae 95d3 7a48 9799 0182  .f.A.8....zH....
+000010a0: 7499 1b20 4897 8501 8274 591a 2048 9795  t.. H....tY. H..
+000010b0: 0182 74b9 3540 902e 6b03 04e9 b231 4090  ..t.5@..k....1@.
+000010c0: 2e77 6d88 5feb a29c 6680 2076 1f0c 10c4  .wm._...f. v....
+000010d0: eea3 0182 d87d 2a21 e245 453c 859e cb8e  .....}*!.EE<....
+000010e0: 5a57 1fd1 bd35 406a ba35 5fc1 a35a f8ca  ZW...5@j.5_..Z..
+000010f0: efca e7b4 69c3 f2e5 830e ad6d 66ec 9d1b  ....i......mf...
+00001100: 7b17 3007 1811 ae95 117d a4ec 520d be9a  {.0......}..R...
+00001110: a65a 6981 48ef 5b6d 1029 bdd6 0691 c69b  .Zi.H.[m.)......
+00001120: e660 1fa9 7b07 8350 32bc 9154 25f7 1103  .`..{..P2..T%...
+00001130: f70a 026f 1f35 04a9 fba0 20da 4448 dd47  ...o.5.... .DH.G
+00001140: 0304 89f9 6480 d462 2a4b 34a7 f011 0bdb  ....d..b*K4.....
+00001150: e660 63a1 9a0d 60a5 95f6 4244 99f6 a66f  .`c...`...BD...o
+00001160: 7ac7 5968 acd4 426a f980 962a 5fe3 054a  z.Yh..Bj...*_..J
+00001170: bc4a bd4f 7b4e 0791 3953 0388 bfb9 b177  .J.O{N..9S.....w
+00001180: a928 575e 41ba ad34 39b0 57b4 41c4 d25a  .(W^A..49.W.A..Z
+00001190: 1bc4 5ed1 06d1 9ccf da20 4abb d506 eb48  ..^...... J....H
+000011a0: 8dac 6183 2c41 b922 7f28 b9f2 1da4 f54c  ..a.,A.".(.....L
+000011b0: f523 1fcd cfbd 2d66 9790 bc32 e8e0 1705  .#....-f...2....
+000011c0: c079 476c 02fd 6621 7072 282b b992 95e0  .yGl..f!pr(+....
+000011d0: 3a54 2f32 eb42 7c34 d06f 9c01 d2fa a184  :T/2.B|4.o......
+000011e0: 88a3 60f3 8509 4e50 b567 aac9 4772 726c  ..`...NP.g..Grrl
+000011f0: 3375 8654 aff2 79b0 278f 01db c759 6125  3u.T..y.'....Ya%
+00001200: 6407 0be9 38b0 12a6 0e88 b2cd 692e 7bc1  d...8.......i.{.
+00001210: baaf 94c3 79b8 fc77 80cf 1204 36d5 8e03  ....y..w....6...
+00001220: 5be6 8e52 5efe 81e2 44de 17c2 8fb9 9507  [..R^...D.......
+00001230: 3961 2ff1 7ff0 1504 8aa4 2c86 0f10 f2bb  9a/.......,.....
+00001240: c3c4 ce29 e32c 88b9 3847 aa64 2b99 05fe  ...).,..8G.d+...
+00001250: 2664 1f84 9fe7 8f09 16bb 8ea3 89cd 3651  &d............6Q
+00001260: 579e 81ab 8f28 d3ff 0150 4b03 0414 0000  W....(...PK.....
+00001270: 0008 0087 4ee2 408a e2eb 49d2 0200 00c1  ....N.@...I.....
+00001280: 0a00 001b 0000 0078 6c2f 6472 6177 696e  .......xl/drawin
+00001290: 6773 2f76 6d6c 4472 6177 696e 6732 2e76  gs/vmlDrawing2.v
+000012a0: 6d6c ed56 5d6f d330 147d afc4 7f88 bcd7  ml.V]o.0.}......
+000012b0: b44d a275 5bdd 2413 1aec 0d90 6088 c7c9  .M.u[.$.....`...
+000012c0: 4ddc c69b e31b c5b7 69ca afe7 3a49 470b  M.......i...:IG.
+000012d0: 034d 0878 d952 35b5 eef5 b95f e7d8 6a7c  .M.x.R5...._..j|
+000012e0: d996 da6b 646d 1598 8485 9380 79d2 6490  ...kdm......y.d.
+000012f0: 2bb3 4ed8 e79b ebf1 05f3 2c0a 930b 0d46  +.N.......,....F
+00001300: 266c 272d bb4c 5f8d 6287 a3af b11c 44c2  &l'-.L_.b.....D.
+00001310: 36b5 e136 2b64 29ec b854 590d 1656 38ce  6..6+d)..TY..V8.
+00001320: a0e4 b05a a94c 7291 a16a 0452 1636 c0aa  ...Z.Lr..j.R.6..
+00001330: 27a0 2ad8 caba 0265 708f 6a9f 8092 6d26  '.*....ep.j...m&
+00001340: f51e 004f 00f4 35ee 11cd ef10 4da9 591a  ...O..5.....M.Y.
+00001350: 03b7 85a8 a416 3bd8 a0d7 70d9 62c2 64ae  ......;...p.b.d.
+00001360: b0f3 a9bc 14d5 91d5 cb05 d294 2236 4de3  ............"6M.
+00001370: e911 388d 9b3e 16ee 2ae9 a93c 61b7 6d40  ..8..>..*..<a.m@
+00001380: cf2d 4641 c4bc 0ca0 cead fa4a 938f c2b3  .-FA.......J....
+00001390: 20f0 bb37 f328 4645 29bb 3d95 c022 6165   ..7.(FE).=.."ae
+000013a0: e007 7af0 f7bb 8ede 412b 593a f23c 970e  ..z.....A+Y:.<..
+000013b0: 6bb8 97de 1d8d d5e2 4e53 e852 a1ac a9b6  k.......NS.R....
+000013c0: deef e279 eb5a e44a 1aec fa84 fb84 1103  ...y.Z.J........
+000013d0: c033 3046 66e8 6a4d 584d 2b07 8aa7 072d  .30Ff.jMXM+....-
+000013e0: a4a3 d1be a3c3 6e6c 149c ce8f cbee 839c  ......nl........
+000013f0: 1cb5 3bd4 5381 554e 2a5c 2c2d e80d ca85  ..;.S.UN*\,-....
+00001400: 962b e441 850b 84aa fb2d 45bd 5666 dcd9  .+.A.....-E.Vf..
+00001410: cf66 9368 46be c1e6 b684 1367 28a4 5a17  .f.hF......g(.Z.
+00001420: c867 f3de bf55 3916 7c7e 469e 4659 b554  .g...U9.|~F.FY.T
+00001430: 5ae1 8e17 2acf a559 306f a5b4 ce40 439d  Z...*..Y0o...@C.
+00001440: b093 6b7a de86 bd4d 1229 d47d 3fb6 7e0d  ..kz...M.).}?.~.
+00001450: 9c66 27b1 849c e620 3608 bf64 caf1 eb06  .f'.... 6..d....
+00001460: 4ac4 37dc 65f0 dc39 a370 5da6 e830 1564  J.7.e..9.p]..0.d
+00001470: 1bdb 534d 543a a53c 50b5 afca 0923 a013  ..SMT:.<P....#..
+00001480: fa08 75b4 5995 622d 9dd0 8828 54e8 8875  ..u.Y.b-...(T..u
+00001490: 5180 6bc8 ee8f e528 6c45 e4d5 ee3c 266c  Q.k....(lE...<&l
+000014a0: d5e7 4212 f112 5aea b3d3 44ae 1cbf 8e04  ..B...Z...D.....
+000014b0: 8df5 a257 fa78 a561 cb0b a8d5 5730 28f4  ...W.x.a....W0(.
+000014c0: a2b4 30ae 0105 4a1e 2c48 fbb9 6af6 7817  ..0...J.,H..j.x.
+000014d0: 6e2c b45a 5300 22cf e520 9d0c 49d2 b8e5  n,.ZS.".. ..I...
+000014e0: 57da e9eb 8dab f7c3 f28e 72dd 74aa 7a0f  W.........r.t.z.
+000014f0: 484a 25ff 3b68 e417 85c5 95d4 da12 bae5  HJ%.;h..........
+00001500: 9fe8 1c1c 5b5e 9b8c aa49 433f 9cf9 a47d  ....[^...IC?...}
+00001510: fa9c 87fe a91f c6d3 960f 3ec2 7d84 6d1a  ..........>.}.m.
+00001520: 3893 5bb8 cca4 a9d2 f4a6 61ed bcdf 0bea  8.[.......a.....
+00001530: 4aed 94ff 703c 7f10 f38c 5838 3c83 ff54  J...p<....X8<..T
+00001540: cc67 93f3 1735 3f3b 35cf f76a bef8 59cd  .g...5?;5..j..Y.
+00001550: 9dc0 ffa2 9ae9 a6fb 6f6a 8ec2 979b f979  ........oj.....y
+00001560: ddcc a13f 6879 e63f a2e5 e84f 6fe6 29fd  ...?hy.?...Oo.).
+00001570: fd4c bf01 504b 0304 1400 0000 0800 874e  .L..PK.........N
+00001580: e240 7112 a71b f004 0000 eb11 0000 1800  .@q.............
+00001590: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+000015a0: 7368 6565 7433 2e78 6d6c 8d58 d972 a338  sheet3.xml.X.r.8
+000015b0: 147d 9faa f907 8aea d706 6303 5eca 7657  .}........c.^.vW
+000015c0: e225 7612 27ae c96c af04 649b 0a58 0ce0  .%v.'..l..d..X..
+000015d0: 38e9 afef 2bc9 2cba d224 79b1 85ee b98b  8...+.,..$y.....
+000015e0: ee39 20c4 f8c7 5b9a 18af 242f 627a 9c98  .9 ...[...$/bz..
+000015f0: 8ed5 310d 720c 6914 1ff7 13f3 af3f 97df  ..1.r.i......?..
+00001600: 07a6 5194 c131 0a12 7a24 13f3 9d14 e68f  ..Q..1..z$......
+00001610: e9ef bf8d cf34 7f29 0e84 9406 4438 1613  .....4.)....D8..
+00001620: f350 96d9 c8b6 8bf0 40d2 a0b0 6846 8e60  .P......@...hF.`
+00001630: d9d1 3c0d 4ab8 ccf7 7691 e524 88b8 539a  ..<.J...v..$..S.
+00001640: d8dd 4ec7 b7d3 203e 9a22 c228 ff4a 0cba  ..N... >.".(.J..
+00001650: dbc5 2199 d3f0 9492 6329 82e4 2409 4aa8  ..!.....c)..$.J.
+00001660: bf38 c459 5145 7b8b be14 2fca 8333 acb5  .8.YQE{.../..3..
+00001670: aaa7 55e2 5c58 ea78 8eab d497 c661 4e0b  ..U.\X.x.....aN.
+00001680: ba2b ad90 a6b6 284d 5de5 d01e 4aeb 4c43  .+....(M]...J.LC
+00001690: 2590 a659 6990 bf9c b2ef 1038 83c5 3dc7  %..Yi......8..=.
+000016a0: 495c bef3 e556 0591 b289 733e 9fad 7356  I\...V....s>..sV
+000016b0: 58e1 f152 45ab 414e df26 e5ec 5494 349d  X..RE.AN.&..T.4.
+000016c0: 0765 604e c79c 816d 6e4f c751 0c5d 64d4  .e`N...mnO.Q.]d.
+000016d0: 1b39 d94d cc2b 67b4 1d9a 30cf 117f c7e4  .9.M.+g...0.....
+000016e0: 5cb4 c6c6 4f4a d3a7 3048 4006 03cf 6c2e  \...OJ..0H@...l.
+000016f0: 1f18 c789 9864 b278 a6f4 8539 afa3 89d9  .....d.x...9....
+00001700: 61f9 4842 4246 9011 c0df 2b99 9104 d057  a.HBBF....+....W
+00001710: 3d50 d67f 3cef b7ab dee8 dbbf cb79 8fe5  =P..<........y..
+00001720: b6eb e4ed 7155 c892 eb69 9b1b 11d9 05a7  ....qU...i......
+00001730: a49c d1e4 9f38 2a0f 1373 6856 737f d0f3  .....8*..shVs...
+00001740: 8ac4 fb43 0982 76ad aec7 a286 3481 10f0  ...C..v.....4...
+00001750: 6ba4 3108 dd35 8d34 78e3 ff67 e1ee bbd6  k.1..5.4x..g....
+00001760: a00f ab0a 79a7 2e31 9d8b ab70 825b 813b  ....y..1...p.[.;
+00001770: c1ff c5c9 e9b0 f01f f940 55dc 07fe 2f3e  .........@U.../>
+00001780: ddc1 a789 1cb8 0bb9 171b 346e 9f94 e738  ..........4n...8
+00001790: 9517 0c2e 5e3d 08f0 c18a 9c6e e502 838b  ....^=.....n....
+000017a0: cb17 1ae1 0075 a23e 185c dc1c cffa b813  .....u.>.\......
+000017b0: 4ed5 7336 a816 e55b 9f2d 0a82 8a54 30a8  N.s6...[.-...T0.
+000017c0: 52f5 2cff 93b6 3b7e e506 832a d9ff 36de  R.,...;~...*..6.
+000017d0: 16ea e0c2 63f7 c874 9cd3 b301 cf0f 6824  ....c..t......h$
+000017e0: 3cd9 e057 f450 884f 4c67 017b e839 23c8  <..W.P.OLg.{.9#.
+000017f0: 04ba 62e0 ab1a 0dc2 2b60 f675 da73 c6f6  ..b.....+`.u.s..
+00001800: 2bc8 38bc 40ae 5548 5746 cc54 444f 46cc  +.8.@.UHWF.TDOF.
+00001810: 5584 2b23 162a c293 114b 15e1 cb88 1b15  U.+#.*...K......
+00001820: d197 112b 1531 9011 6b15 3194 11b7 2ac2  ...+.1..k.1...*.
+00001830: e9c8 903b 0d04 75f5 5e85 a08e 6c54 8483  ...;..u.^...lT..
+00001840: 1aff f039 e451 0341 e46c 3590 a616 1b64  ...9.Q.A.l5....d
+00001850: 556b 0bee b842 2322 363d 31e1 b716 9183  Uk...B#"6=1.....
+00001860: c8bb d640 107b 330d 04d1 37d7 4010 7f0b  ...@.{3...7.@...
+00001870: 0d04 11b8 5421 5d44 e08d 0682 085c 6920  ....T!]D.....\i 
+00001880: 889e b506 827a 7fab 8134 bde7 b7e8 9d06  .....z...4......
+00001890: 82ba 7baf 81a0 ee6e 3410 d4dd 070d 0475  ..{....n4......u
+000018a0: f751 0341 dddd aa90 5ed3 5d49 4df0 20e6  .Q.A....^.]IM. .
+000018b0: fb5d bfb5 21d5 9ba0 5e69 6cff 9d98 f05b  .]..!...^il....[
+000018c0: 2b4d 795c 6920 8897 990a f111 04b6 7525  +My\i ........u%
+000018d0: 11e2 65a1 8120 5e96 1a08 e2e5 4603 41bc  ..e.. ^.....F.A.
+000018e0: ac34 10c4 cb5a 0341 bcdc aa10 b7e1 4528  .4...Z.A......E(
+000018f0: 4d03 41aa bfd7 4050 eb36 1a08 52fd 4305  M.A...@P.6..R.C.
+00001900: 612f 396c 1b7a ac26 1a5e 5dd4 eead 06d2  a/9l.z.&.^].....
+00001910: b45b d215 ecd5 baa7 94cb b737 b4a0 6bed  .[.........7..k.
+00001920: ec4c 3b3b 6781 f9fb 57ad 3e17 d1b9 0008  .L;;g...W.>.....
+00001930: 189f 75a9 96c2 2676 5917 917c 2319 11bd  ..u...&vY..|#...
+00001940: 2bc9 8888 5db7 8d1e a2f4 b66d f411 0d77  +...]......m...w
+00001950: 6044 ebf1 51d7 ef55 8887 a26c 5488 df10  `D..Q..U...lT...
+00001960: c3e9 7d50 211e 823c 02a4 e92a 5aff b66d  ..}P!..<...*Z..m
+00001970: 6c2d 5162 1dde b51a d67b f50b 8ec7 a940  l-Qb.....{.....@
+00001980: 1a9d 03b8 cee6 210e 376d 636b 2952 3678  ......!.7mck)R6x
+00001990: 456b b235 af53 6c04 af50 5607 cb4c 1850  Ek.5.Sl..PV..L.P
+000019a0: 1933 edec 0262 d71a 427c 2e85 4d68 c8c3  .3...b..B|..Mh..
+000019b0: 1a92 8ca8 872b c988 3524 1951 ce4d dbe8  .....+..5$.Q.M..
+000019c0: a366 3db6 8d1e cab9 958c 4d58 a993 7d7d  .f=.......MX..}}
+000019d0: 27fb bc93 ae85 7472 2de6 9106 6797 59a5  '.....tr-...g.Y.
+000019e0: ef0b 885e 13ed 3715 7059 6e25 63d3 4ca9  ...^..7.pYn%c.L.
+000019f0: 3c38 38b1 4dca 93ca ecd6 f21a f032 7191  <88.M........2q.
+00001a00: 6216 dd4b 73f6 5902 22b5 2b42 32b9 af20  b..Ks.Y.".+B2.. 
+00001a10: ec4c d97e f182 a358 23b7 3af9 9027 6f18  .L.~...X#.:..'o.
+00001a20: 112e e230 2ace 0459 b027 9b20 dfc7 c7c2  ...0*..Y.'. ....
+00001a30: 48c8 0e16 d2b1 6025 b938 69f2 7149 333e  H.....`%.8i.qI3>
+00001a40: 0b75 3dd3 124e dcd5 d501 3e7c 1078 3877  .u=..N....>|.x8w
+00001a50: 2c78 f4ee 282d ab0b 288e c57d 22e5 2933  ,x..(-..(..}".)3
+00001a60: b220 23f9 53fc 130e d850 24cd 63f8 c4c1  . #.S....P$.c...
+00001a70: bf6c 4ccc 8ce6 651e c425 3b90 8a60 4b1e  .lL...e..%;..`K.
+00001a80: 052e 13b2 0fc2 f7cb e70a 231f c5d1 c4cc  ..........#.....
+00001a90: d751 971f a6eb cf34 d35f 504b 0304 0a00  .Q.....4._PK....
+00001aa0: 0000 0000 874e e240 0000 0000 0000 0000  .....N.@........
+00001ab0: 0000 0000 0900 0000 786c 2f74 6865 6d65  ........xl/theme
+00001ac0: 2f50 4b03 0414 0000 0008 0087 4ee2 40f8  /PK.........N.@.
+00001ad0: 8e8c 59f3 0500 002b 1900 0013 0000 0078  ..Y....+.......x
+00001ae0: 6c2f 7468 656d 652f 7468 656d 6531 2e78  l/theme/theme1.x
+00001af0: 6d6c ed59 4b6f 1b37 10be 17e8 7f58 ecbd  ml.YKo.7.....X..
+00001b00: 9164 eb11 1991 035b 8fb8 8d9d 0491 9222  .d.....[......."
+00001b10: 476a 97da 65c4 5d2e 48ca 8e6e 4172 2a0a  Gj..e.].H..nAr*.
+00001b20: 1428 9016 b914 287a e9a1 281a a001 1ab4  .(....(z..(.....
+00001b30: 87fe 97ba 4890 a63f a243 aeb4 2225 2a7e  ....H..?.C.."%*~
+00001b40: c087 3488 ec83 96fb cdcc c719 ee37 e4ea  ..4..........7..
+00001b50: cad5 0709 f50e 3117 84a5 2dbf 72a9 ec7b  ......1...-.r..{
+00001b60: 380d 5848 d2a8 e5df 19f4 3eb9 ec7b 42a2  8.XH......>..{B.
+00001b70: 3444 94a5 b8e5 4fb1 f0af 6e7f fcd1 15b4  4D....O...n.....
+00001b80: 2563 9c60 0fec 53b1 855a 7e2c 65b6 552a  %c.`..S..Z~,e.U*
+00001b90: 8900 8691 b8c4 329c c2bd 11e3 0992 70c9  ......2.......p.
+00001ba0: a352 c8d1 11f8 4d68 69a3 5cae 9712 4452  .R....Mhi.\...DR
+00001bb0: df4b 5102 6e6f 8e46 24c0 dedf 2ffe 78fd  .KQ.no.F$.../.x.
+00001bc0: c3d3 bf1e 7e09 fffe f63c 4697 42a0 540a  ....~....<F.B.T.
+00001bd0: 3510 50de 5711 b065 a8b1 e1b8 a210 622a  5.P.W..e......b*
+00001be0: da94 7b87 88b6 7c08 17b2 a301 7e20 7d8f  ..{...|.....~ }.
+00001bf0: 2221 e146 cb2f eb8f 5fda be52 425b 3323  "!.F./.._..RB[3#
+00001c00: 2ad7 d81a 763d fd99 d9cd 0cc2 f186 8ec9  *...v=..........
+00001c10: a361 11b4 5aad 55eb 3b85 7f0d a072 15d7  .a..Z.U.;....r..
+00001c20: 6d74 ebdd 7ae1 4f03 5010 c04c 732e a6cf  mt..z.O.P..Ls...
+00001c30: da6e 73b7 539b 610d 50fe d5e1 bbd3 e86c  .ns.S.a.P......l
+00001c40: 562c bce1 7f73 85f3 4e4d fd59 780d cafd  V,...s..NM.Yx...
+00001c50: 5757 f0bd 5e1b b268 e135 28c7 d756 f0d5  WW..^..h.5(..V..
+00001c60: 6a63 a35d b5f0 1a94 e3eb 2bf8 4679 a753  jc.]......+.Fy.S
+00001c70: 6d58 780d 8a29 49c7 2be8 72ad bed9 9ecf  mXx..)I.+.r.....
+00001c80: b680 8c18 dd73 c29b b56a afb1 3173 be40  .....s...j..1s.@
+00001c90: c16a 2856 970a 3162 a95c b7d6 1274 9ff1  .j(V..1b.\...t..
+00001ca0: 1e00 1490 2249 524f 4e33 3c42 012c e636  ...."IRON3<B.,.6
+00001cb0: a264 c889 b74f a258 aa30 680b 23e3 7e3e  .d...O.X.0h.#.~>
+00001cc0: 1488 9521 15d1 1301 2799 6cf9 9f65 081e  ...!....'.l..e..
+00001cd0: 8f85 d797 2f5e 1c3f 7a7e fce8 b7e3 c78f  ..../^.?z~......
+00001ce0: 8f1f fd62 7ab7 ecf6 501a 9976 6f7e fcfa  ...bz...P..vo~..
+00001cf0: dfef 1e7a fffc fafd 9b27 dfe4 a197 f1c2  ...z.....'......
+00001d00: c4bf faf9 8b57 bfff f936 f7f0 3019 b4be  .....W...6..0...
+00001d10: 7df6 eaf9 b397 4fbf 7afd d313 87f7 1d8e  }.....O.z.......
+00001d20: 8626 7c40 122c bc1b f8c8 bbcd 1298 a0ce  .&|@.,..........
+00001d30: 8ecd 070f f9d9 2c06 3122 9605 8ac1 b7c3  ......,.1"......
+00001d40: 7557 c616 f0c6 1451 176e 17db 29bc cb41  uW.....Q.n..)..A
+00001d50: 475c c06b 93fb 16d7 7ecc 2792 3822 5f8f  G\.k....~.'.8"_.
+00001d60: 130b 78c0 18dd 65dc 9980 eb2a 9691 e1c1  ..x...e....*....
+00001d70: 248d dcc1 f9c4 c4dd 46e8 d015 bb8d 52ab  $.......F.....R.
+00001d80: c0dd 4906 024a 5c2e db31 b668 dea2 2895  ..I..J\..1.h..(.
+00001d90: 28c2 2996 9eba c7c6 183b 6677 8f10 2baf  (.)......;fw..+.
+00001da0: 0724 e04c b091 f4ee 116f 1711 674a 0664  .$.L.....o..gJ.d
+00001db0: 682d a485 d11e 49a0 2e53 1741 28b5 959b  h-....I..S.A(...
+00001dc0: 83bb de2e a3ae 5977 f0a1 8d84 c702 5107  ......Yw......Q.
+00001dd0: f901 a656 1aaf a189 4489 cbe5 0025 d44c  ...V....D....%.L
+00001de0: f83e 92b1 8b64 7fca 0313 d715 122a 1d61  .>...d.......*.a
+00001df0: cabc 6e88 8570 d9dc e430 5fa3 e8d7 4143  ..n..p...0_...AC
+00001e00: dc65 3fa0 d3c4 4672 49c6 2e9f fb88 3113  .e?...FrI.....1.
+00001e10: d961 e376 8c92 cc85 ed93 3436 b19f 8a31  .a.v......46...1
+00001e20: 2c51 e4dd 62d2 053f 60f6 13a2 aea1 0e28  ,Q..b..?`......(
+00001e30: 5d5b eebb 045b e53e 5908 ee80 7c9a 9416  ][...[.>Y...|...
+00001e40: 0b44 dd99 7047 2daf 6166 addf fe94 8e10  .D..pG-.af......
+00001e50: d62a 03ea 6e89 7642 d213 153c 8f70 f1da  .*..n.vB...<.p..
+00001e60: ed60 7e31 aaed 766c e5fd e5d9 f47a 8713  .`~1..vl.....z..
+00001e70: e753 b3b7 a4d2 eb70 ff43 6dee a049 7a0b  .S.....p.Cm..Iz.
+00001e80: c3e3 b0da 9b3e 48f3 0769 f6df 7b69 5ef7  .....>H..i..{i^.
+00001e90: 2c5f bc20 2f34 18e4 59ed 02f3 fdb6 de7d  ,_. /4..Y......}
+00001ea0: 276b 37df 2342 695f 4e29 de17 7aff 2da0  'k7.#Bi_N)..z.-.
+00001eb0: f384 3d18 5476 fafc 898b c358 16c3 57f5  ..=.Tv.....X..W.
+00001ec0: 2443 000b 1771 a46d 3cce e4e7 44c6 fd18  $C...q.m<...D...
+00001ed0: 65b0 77af f8ca 4924 66ae 23e1 654c c099  e.w...I$f.#.eL..
+00001ee0: 510f 3b7d 2b3c 9d24 072c cccf 9c95 8a3a  Q.;}+<.$.,.....:
+00001ef0: 5fe6 e221 905c 8c97 6bc5 389c 1764 8eae  _..!.\..k.8..d..
+00001f00: 3716 e7a8 c2bd 661b e9f3 ee9c 80b2 3d0b  7.....f.......=.
+00001f10: 0923 984d 62d3 41a2 311f 5449 d2a7 6b48  .#.Mb.A.1.TI..kH
+00001f20: 9a83 849e d985 b068 3a58 5c56 eee7 a55a  .......h:X\V...Z
+00001f30: 6101 d48a aac0 d6c8 830d 55cb af55 c104  a.........U..U..
+00001f40: 8ce0 d084 280e 559d f252 cfab ab8b 7991  ....(.U..R....y.
+00001f50: 955e 974c 6b05 94e1 fdc6 6c05 2c2a dd54  .^.Lk.....l.,*.T
+00001f60: 5cd7 4e4f cd2e 5f6a a7a8 b445 c258 6e36  \.NO.._j...E.Xn6
+00001f70: 099d 19dd c344 8c42 3c5b 9d6a f434 34ce  .....D.B<[.j.44.
+00001f80: 5aeb e6a2 a416 3d95 8a59 2e0c 1a8d cb6f  Z.....=..Y.....o
+00001f90: 6371 de5a 83dd b236 d0d4 540a 9a7a 472d  cq.Z...6..T..zG-
+00001fa0: bfbe 5983 2513 a0ac e58f e0ec 0e5f 930c  ..Y.%........_..
+00001fb0: d68e 505b 5a44 2378 0f16 489e 3ff0 e751  ..P[ZD#x..H.?..Q
+00001fc0: 968c 0bd9 4122 ce13 ae45 2757 8384 48cc  ....A"...E'W..H.
+00001fd0: 3d4a 9296 afa6 5f94 81a6 5a43 34b7 ca06  =J...._...ZC4...
+00001fe0: 08c2 3b4b ae09 b2f2 ae91 83a2 db45 c6a3  ..;K.........E..
+00001ff0: 110e a459 7663 4465 3abf 0485 cfb5 c279  ...YvcDe:......y
+00002000: 579b 9f1f ac2c d904 cadd 8fc3 236f 4827  W....,......#oH'
+00002010: fc36 8225 566b 5454 0243 22e0 054f 25cf  .6.%VkTT.C"..O%.
+00002020: 6648 e09d 6421 648b f5b7 d498 66b2 6bbe  fH..d!d.....f.k.
+00002030: 14d4 6b28 1f47 348b d1ac a398 629e c3b5  ..k(.G4.....b...
+00002040: 9417 74f4 5591 03e3 6a36 6748 a891 9259  ..t.U...j6gH...Y
+00002050: 231c 46aa c19a 49b5 ba69 d135 720e 6bbb  #.F...I..i.5r.k.
+00002060: eec9 462a 7386 682e 7aa6 a52a aa6b ba55  ..F*s.h.z..*.k.U
+00002070: cc8a 306f 034b b93c 5f93 3758 cd53 0ced  ..0o.K.<_.7X.S..
+00002080: d2ec f0b9 742f 4b6e 73ae 754b fb84 a24b  ....t/Kns.uK...K
+00002090: 40c2 8bfc 39ba ee29 1a82 416d 11cc a2a6  @...9..)..Am....
+000020a0: 18af cab0 d2ec d9a8 dd3b e613 3c81 da69  .........;..<..i
+000020b0: 9a84 a1fa f5b9 dba5 bc15 3dc2 190e 06cf  ..........=.....
+000020c0: d5f9 c16e 79d5 c2d0 68be afd4 99d6 bf61  ...ny...h......a
+000020d0: 98bf 2fb0 e17d 108f 0ebc c99d 5029 7281  ../..}......P)r.
+000020e0: d0a0 edff 0050 4b03 0414 0000 0008 0087  .....PK.........
+000020f0: 4ee2 4074 e6b0 2283 0a00 0092 5100 000d  N.@t..".....Q...
+00002100: 0000 0078 6c2f 7374 796c 6573 2e78 6d6c  ...xl/styles.xml
+00002110: d55c eb8f db58 15ff 8ec4 ff60 b982 0f88  .\...X.....`....
+00002120: 99d8 8e33 4966 2753 3a99 b1b4 d282 566a  ...3If'S:.....Vj
+00002130: 9190 0055 9ec4 99b1 70e2 e038 dd19 1052  ...U....p..8...R
+00002140: a15b 661f 2a12 2a50 58ad c4b2 ab52 3ed0  .[f.*.*PX....R>.
+00002150: 0116 c456 65db fe33 4d66 e613 ffc2 9e7b  ...Ve..3Mf.....{
+00002160: fdb8 e73a d789 3b1d c79e 8ed4 f875 debf  ...:..;......u..
+00002170: 7bce 7dd9 1b57 0ffa 8e74 cbf2 46b6 3b68  {.}..W...t..F.;h
+00002180: c9ea aa22 4bd6 a0e3 76ed c15e 4bfe fe0d  ..."K...v..^K...
+00002190: 63a5 214b 23df 1c74 4dc7 1d58 2df9 d01a  c.!K#..tM..X-...
+000021a0: c957 37bf feb5 8d91 7fe8 58d7 f72d cb97  .W7.......X..-..
+000021b0: 80c5 60d4 92f7 7d7f b85e a98c 3afb 56df  ..`...}..^..:.V.
+000021c0: 1cad ba43 6b00 777a aed7 377d 38f5 f62a  ...Ck.wz..7}8..*
+000021d0: a3a1 6799 dd11 21ea 3b15 4d51 d62a 7dd3  ..g...!.;.MQ.*}.
+000021e0: 1ec8 0187 f57e 270b 93be e9fd 643c 5ce9  .....~'.....d<\.
+000021f0: b8fd a1e9 dbbb b663 fb87 9497 2cf5 3beb  .......c....,.;.
+00002200: 6fee 0d5c cfdc 7540 d503 af19 7186 c319  o..\..u@....q...
+00002210: d67d bbe3 b923 b7e7 af02 ab8a dbeb d91d  .}...#..........
+00002220: 6b46 4375 ade2 59b7 6ce2 9da6 bcb9 3118  kFCu..Y.l.....1.
+00002230: f78d be3f 923a ee78 e0b7 643d be24 0577  ...?.:.x..d=.$.w
+00002240: deec c245 5596 02a3 db6e 17d4 b829 7d4b  ...EU....n...)}K
+00002250: baf2 ed2b 5794 9bd2 1be4 f847 2bf8 ec9b  ...+W......G+...
+00002260: 3f1d bbfe 1b2b c10f 7de2 3b37 25b9 1289  ?....+..}.;7%...
+00002270: c27c b524 df80 e8ff 2f1e 0607 58cc cc2d  .|.$..../...X..-
+00002280: 2c75 e666 7021 9312 d5a4 12a1 d455 2561  ,u.fp!.......U%a
+00002290: 1fbb c071 bf7a 75be 917a 92ff 8cb2 d47b  ...q.zu..z.....{
+000022a0: 11f7 99bb a19d a9f7 e728 5309 a3bb b9d1  .........(S.....
+000022b0: 7307 2cc8 1a89 32b9 b2b9 31fa 9974 cb74  s.,...2...1..t.t
+000022c0: a099 a824 421d d771 3dc9 07b4 4394 e995  ...$B..q=...C...
+000022d0: 81d9 b782 274e 1ebf 7ff2 f405 7d6a dff4  ....'N......}j..
+000022e0: 46d0 4802 c2aa 4eae d126 123e d9b7 01b0  F.H...N..&.>....
+000022f0: e462 2590 912e c9db db6d c986 d16c 2bd0  .b%......m...l+.
+00002300: 7008 45be e242 c394 fc25 c586 d5ea 4a4e  p.E..B...%....JN
+00002310: e2ea 1a31 23cf 888d 495c 05f8 088d 8398  ...1#...I\......
+00002320: 2986 91c9 97d4 058b 21b2 4060 0304 36b2  ).......!.@`..6.
+00002330: 7933 a3c0 39d6 1906 b1ef 22ad dbc5 ee6c  y3..9....."....l
+00002340: cc04 af9a 4996 9ab5 b9d9 581a 6adc 61f0  ....I.....X.j.a.
+00002350: ea06 f9cb 2432 a32f 39f3 6a79 9bc7 49a3  ....$2./9.jy..I.
+00002360: aee3 5ac2 053b 9393 869c 1926 940b 9636  ..Z..;.....&...6
+00002370: 0795 55a3 6ad4 b365 caf3 840d 9916 e284  ..U.j..e........
+00002380: 08ac e687 9359 81c6 b5fa 768e ed4e 20d0  .....Y....v..N .
+00002390: 20ff 085e 1716 9f8c 2e9d 13bf e559 f74a   ..^.........Y.J
+000023a0: 45fc f50d 83fa ad5e 6cd8 445e 7ca5 02fe  E......^l.D^|...
+000023b0: 1a46 e5e1 3c9c 439a 3cdc 26c7 1fbe 7c76  .F..<.C.<.&...|v
+000023c0: 9f5c eb08 ba56 c25e d479 3850 4623 e8f9  .\...V.^.y8PF#..
+000023d0: d98e 1377 f8a1 9e04 5736 3760 f0e1 5bde  ...w....W67`..[.
+000023e0: c080 db52 787c e370 083d c101 8c93 8876  ...Rx|.p.=.....v
+000023f0: 1542 b9f0 e93d cf3c 5435 5a01 b211 8c5c  .B...=.<T5Z....\
+00002400: c7ee 122d f6da b4ff 19a6 1ec3 68d7 db3b  ...-........h..;
+00002410: 44ee 6e78 c31e 74ad 030b 0624 6bb4 cf59  D.nx..t....$k..Y
+00002420: 410a 6755 2e29 0b47 3a47 31b1 493b 5bcd  A.gU.).G:G1.I;[.
+00002430: 76ce 26c5 b2c0 814b 93d5 6e37 2924 97e0  v.&....K..n7)$..
+00002440: 43cd 80bf e5f8 f05a 8dfc 2d47 567b 6dc7  C......Z..-GV{m.
+00002450: 5816 dc69 f3c9 3154 61ab 8291 af6f 9359  X..i..1Ta....o.Y
+00002460: 0565 b5de 6c36 1bea 5aa3 d168 ea55 75f9  .e..l6..Z..h.Uu.
+00002470: f26b 20bf 596d 34d7 3450 43c9 3ba4 b3f6  .k .Ym4.4PC.;...
+00002480: 5741 7cbd 566b d4d4 a6a6 ab79 3795 50fe  WA|.Vk.....y7.P.
+00002490: 92cc ac15 1c66 24bf 9030 23f9 8584 998e  .....f$..0#.....
+000024a0: 07f2 6fcd 6b05 8719 c92f 24cc 487e 2161  ..o.k..../$.H~!a
+000024b0: aee7 5c87 c2a4 512f 38cc 487e 2161 46f2  ..\...Q/8.H~!aF.
+000024c0: 0b09 339d 19ca bf35 c322 48a1 b519 c92f  ..3....5."H..../
+000024d0: 24cc 487e 2161 5e52 1700 d68b 0a0d 3392  $.H~!a^R......3.
+000024e0: 5f48 9891 fcd7 0c33 1dcb c2e8 79d7 f5ba  _H.....3....y...
+000024f0: b0b8 2885 0b66 640d 2db8 b4b9 e158 3d1f  ..(..fd.-....X=.
+00002500: 86ab 9ebd b74f 7e7d 7748 06af aeef c36a  .....O~}wH.....j
+00002510: dce6 46d7 36f7 dc81 e9c0 6125 a288 7e09  ..F.6.....a%..~.
+00002520: 252c 4ac2 fa63 4bf6 f761 fd30 9ad9 0f07  %,J..cK..a.0....
+00002530: 735b 1af9 2305 a042 1e0d 6564 a4a0 fa50  s[..#..B..ed...P
+00002540: 7532 1280 e291 de19 2902 2317 db08 0688  u2......).#.....
+00002550: bc13 49e9 5b5d 7bdc 8f8d 8fbb d181 cb88  ..I.[]{.........
+00002560: 1f73 1311 3713 9d8c 54f4 baae d4f5 9ab6  .s..7...T.......
+00002570: 16f8 3cab 7991 1da2 10b2 19f7 ac21 4414  ..<.y........!D.
+00002580: d942 8808 3286 1051 5c84 8d6c b638 ab8d  .B..2..Q\..l.8..
+00002590: 8822 9b8d 8820 a38d 88e2 556d ecba 6358  ."... ....Um..cX
+000025a0: 778f f118 3646 c450 d018 17d2 ccda b990  w...6F.P........
+000025b0: 4460 e942 9aac b62e 6892 6239 8601 8b71  D`.B....h.b9...q
+000025c0: 742e 1d52 d979 daa5 b0a5 70ed 7db1 cddc  t..R.y....p.}...
+000025d0: e3f3 d408 d32d 24ef 8ee5 38d7 499a fd41  .....-$...8.I..A
+000025e0: 2fce e03a 49e1 073d b42f 0176 8c90 356b  /..:I..=./.v..5k
+000025f0: b2f5 811c c2a4 6778 18a4 ebe0 04fc c611  ......gx........
+00002600: e974 1fc1 222a c91c 0e9d 4303 b853 dec1  .t.."*....C..S..
+00002610: 1908 6067 5bb4 beb0 f36b 8ebd 37e8 5b98  ..`g[....k..7.[.
+00002620: e06d cff5 ad8e 4ff7 b728 a0bc 193d 42b6  .m....O..(...=B.
+00002630: bdf8 7687 2ce8 7780 c2f2 68c5 38e8 2555  ..v.,.w...h.8.%U
+00002640: a55b 122e 85aa 50bf 1787 a21c 4ea5 9b64  .[....P.....N..d
+00002650: 2e85 5375 baef e652 a88a 9a22 4cb3 a434  ..Su...R..."L..4
+00002660: c520 fedf 1bf7 772d cfa0 9bb3 58f3 21ab  . ....w-....X.!.
+00002670: 19ec 6c09 8d0b 690c 3306 974c 6394 eec0  ..l...i.3..Lc...
+00002680: dd2c dd01 b669 aa4a f131 97ce 7248 58c8  .,...i.J.1..rHX.
+00002690: a730 3cbf 643e 8591 e625 d398 245d 71d1  .0<.d>...%..$]q.
+000026a0: 9b8b 8202 5b9a 8a80 0b87 0cb8 90e9 e601  ....[...........
+000026b0: 9753 395f e0c2 0e3b b157 4ba4 22a9 0ba2  .S9_...;.WK."...
+000026c0: c043 d7a6 2c5e 4c53 11a2 9e59 c5e5 5601  .C..,^LS...Y..V.
+000026d0: 9574 0c43 af42 4560 d884 5ed8 1c95 7346  .t.C.BE`..^...sF
+000026e0: 23e9 0286 4a41 4a65 4a41 da2f 4e29 54e2  #...JAJeJA./N)T.
+000026f0: 39a5 0af5 14aa e290 ca99 a7e0 7a71 9e4a  9...........zq.J
+00002700: 2b83 707d 8e52 c632 f35d 5add 83eb 6551  +.p}.R.2.]Z...eQ
+00002710: 1115 3a38 64a1 9d9f 4cb6 f21f a191 7216  ..:8d...L.....r.
+00002720: 8e40 51d9 80dc 574e 1d51 8683 a65a 4e1d  .@Q...WN.Q...ZN.
+00002730: 35e2 d330 e391 ee42 49b5 44e1 263d 864b  5..0...BI.D.&=.K
+00002740: a065 6951 c945 1c20 5a52 5f62 5c96 b7f5  .eiQ.E. ZR_b\...
+00002750: 605c 7243 4350 7f4e 3adf 5a6a aed4 b096  `\rCCP.N:.Zj....
+00002760: 5c5f ab54 5ae2 8873 fd9c d26a c975 7c4a  \_.TZ..s...j.u|J
+00002770: a525 8e78 696b 38c6 25c9 4ae5 cf44 44e3  .%.xik8.%.J..DD.
+00002780: 4ba0 6579 6b0f c2a5 56de da83 b52c 6fed  K.eyk...V....,o.
+00002790: 41f9 12f6 955f 065c 96b7 f6e0 8897 b7f6  A...._.\........
+000027a0: 602d cb5b 7b30 2ecb 5b7b 9096 d5f2 d61e  `-.[{0..[{......
+000027b0: 14f1 2a1c 97b4 f660 2dcb 5b7b 70c4 0baf  ..*....`-.[{p...
+000027c0: 3d15 bce6 1eac c0a3 c5f7 c6b9 d6de a583  =...............
+000027d0: 9e78 119e 58be 78de 24a0 2665 998e 5cd0  .x..X.x.$.&e..\.
+000027e0: 4c2b ddd2 c02d eb23 8e10 f068 0221 e9d5  L+...-.#...h.!..
+000027f0: 489f 8061 b0bc 0f58 a1ec 8349 b7b9 9c81  H..a...X...I....
+00002800: 5dc4 3959 8543 5de1 f22b e98a 2000 875c  ].9Y.C]..+.. ..\
+00002810: 6b12 eb9a dcce 80ec cecc 8b73 24de 96f0  k..........s$...
+00002820: 8e67 0e6f 5807 b0e7 21d8 3332 b323 e13c  .g.oX...!.32.#.<
+00002830: d278 2f5f 886c f072 1487 cc5e a3f8 0644  .x/_.l.r...^...D
+00002840: a3cd 25fc d692 18ff 1279 c1b4 254f 9e3c  ..%......y..%O.<
+00002850: 397d f42e 7cc7 23c4 b0b4 3bb6 1dd8 a419  9}..|.#...;.....
+00002860: 237a 86e0 de9d 97cf ee4d defb f5d9 47bf  #z.......M....G.
+00002870: 8bc8 488a 6464 f405 e424 d9e9 7f1e 4d9e  ..H.dd...$....M.
+00002880: fc32 2220 d98a 11d0 1770 9204 277f 7a0e  .2" .....p..'.z.
+00002890: 42a6 ff88 8510 9433 1afa 3649 9266 8274  B......3..6I.f.t
+000028a0: fba1 f2e3 481a 3812 51d2 1714 9294 817a  ....H.8.Q......z
+000028b0: 8886 f4ec 9834 badb 7d86 e6bf 77cf ee3f  .....4..}...w..?
+000028c0: 9ffe e661 2487 f4b3 184d f052 7db4 c527  ...a$....M.R}..'
+000028d0: 72f7 179f 9f1e bf38 7b70 7cf2 d1bb a749  r......8{p|....I
+000028e0: 7ad2 0362 f474 4f6e 52e6 f4df 7f3b 3bfa  z..b.tOnR....;;.
+000028f0: 2012 483a 238c 00e6 11a1 dd24 294e 1fff   .H:#......$)N..
+00002900: 75f2 db0f a67f 389a 7efc f788 8e74 0f10  u.....8.~....t..
+00002910: 1d6d 0649 bae9 2747 679f fe31 a2a0 7394  .m.I..'Gg..1..s.
+00002920: 8844 e8fe d347 9f81 72d3 db8f 7869 74e6  .D...G..r...xit.
+00002930: 90d1 d684 f808 c449 80a4 0089 2a0f 1155  .......I....*..U
+00002940: 18b5 9008 1e0d 8978 8ca8 c2b0 8544 f068  .......x.....D.h
+00002950: 48c4 c343 15c6 2d24 8247 4322 1e1f c13b  H..C..-$.GC"...;
+00002960: 5449 179e 3ebf 3fb9 1ba3 034c c05e 8791  TI..>.?....L.^..
+00002970: b728 5a40 72f4 3496 c223 0286 c122 92e3  .(Z@r.4..#..."..
+00002980: bf9c 1c3f 8849 784c 6874 cb68 52b1 e967  ...?.IxLht.hR..g
+00002990: b7a7 7f7e 38b9 f7fb c9dd 3bd3 4fbe 8c69  ...~8.....;.O..i
+000029a0: 795c 4049 1288 0b20 3f43 4b27 1258 90e1  y\@I... ?CK'.X..
+000029b0: a32e 02da e9bf 8ea6 b7ff 1789 a3a3 7a44  ..............zD
+000029c0: 22c4 d4e4 e1b3 f879 1e12 9a10 1293 2f8e  "......y....../.
+000029d0: e3e7 7934 6842 349c ddfe d5cb 278f 6312  ..y4hB4.....'.c.
+000029e0: 1e0b 9a10 0b93 2f9f 9efe f30e 607c f2f8  ....../.....`|..
+000029f0: c1d9 a71f 9fbe ff39 832d 1d11 229b 848d  .......9.-.."...
+00002a00: 5853 be21 ad48 73d9 f058 819e b2c0 9bfa  XS.!.Hs..X......
+00002a10: 6236 3c7e a02b 2b60 b3b6 980d 8fa9 aa10  b6<~.++`........
+00002a20: 5302 73e2 76a9 f1c0 aa0a 8195 ea95 980d  S.s.v...........
+00002a30: 1d30 30e7 061f 1f49 623b d52b 8c4d a25c  .00....Ib;.+.M.\
+00002a40: 0971 97ea 15c6 068e 5016 ad8a e138 8b95  .q......P....8..
+00002a50: 38f1 801b 3806 427c a67a 85b1 e131 5b15  8...8.B|.z...1[.
+00002a60: 6236 d52b 8c0d 9fd1 aa42 e4a6 7a85 b1e1  b6.+.....B..z...
+00002a70: 91ab 0b91 2bc0 4a9c 59ab 3c66 e16b 5f02  ....+.J.Y.<f.k_.
+00002a80: cca6 7a85 b1e1 310b 9b0c 056c 52bd c2d8  ..z...1....lR...
+00002a90: f0c8 856d b502 36a9 5e89 d980 1b70 a875  ...m..6.^....p.u
+00002aa0: 6176 1478 0562 12d4 1bf2 d133 0436 5d88  av.x.b.....3.6].
+00002ab0: d954 af30 363c 6675 2166 53bd c2d8 f0c8  .T.06<fu!fS.....
+00002ac0: d585 c84d f50a 6303 fec1 4609 912b f00a  ...M..c...F..+..
+00002ad0: 402c f40a b0c2 0c84 984d f50a 63c3 63b6  @,.......M..c.c.
+00002ae0: 26c4 6caa 5718 1b1e b935 2172 53bd c2d8  &.l.W....5!rS...
+00002af0: f0c8 ad51 e4b2 712b 74ed 7df2 fd3d ba71  ...Q..q+t.}..=.q
+00002b00: 3cee db03 beba 56cf 1c3b fe8d f866 4b66  <.....V..;...fKf
+00002b10: c7df a5ef b240 f4c3 a7de b66f b93e 65d1  .....@.....o.>e.
+00002b20: 92d9 f15b e45d a1a0 ab05 e3a3 b746 f06a  ...[.].......F.j
+00002b30: 0ffc 4a63 cf6e c93f dfd9 aa37 b777 0c6d  ..Jc.n.?...7.w.m
+00002b40: a5a1 6c35 56f4 aa55 5b69 d6b6 b657 6a7a  ..l5V..U[i...Wjz
+00002b50: 7b6b 7bdb 682a 9ad2 fe05 4486 7cac 70fd  {k{.h*....D.|.p.
+00002b60: 40d5 cff7 4140 a559 6906 1f2d 846d e2aa  @...A@.Yi..-.m..
+00002b70: be3e 72e0 b381 5e68 6ca8 fc75 76ad 25a3  .>r...^hl..uv.%.
+00002b80: 9340 7dd2 422b a076 f03f 35a2 328a 3fa6  .@}.B+.v.?5.2.?.
+00002b90: b8f9 1550 4b03 0414 0000 0008 0087 4ee2  ...PK.........N.
+00002ba0: 40f4 d54e 5ea6 0300 00a3 0900 0014 0000  @..N^...........
+00002bb0: 0078 6c2f 7368 6172 6564 5374 7269 6e67  .xl/sharedString
+00002bc0: 732e 786d 6c9d 56df 4fd3 5014 7e37 f17f  s.xml.V.O.P.~7..
+00002bd0: 586a 62d4 20db f047 0c6e 35c6 a82f c607  Xjb. ..G.n5../..
+00002be0: 8527 6396 4b57 60c9 d6ce f6ce 68b2 8731  .'c.KW`.....h..1
+00002bf0: 5006 8a93 28a2 5003 1821 46d9 86f8 ab6c  P...(.P..!F....l
+00002c00: 6bf6 c7d8 db76 4ffc 0b9e f632 426e ef8c  k....vO....2Bn..
+00002c10: 7159 d6f6 3bdf f9ee 39f7 9e73 bac4 9547  qY..;...9..s...G
+00002c20: b96c e4a1 ace9 1955 490a f1c1 9810 9115  .l.....UI.......
+00002c30: 494d 6794 89a4 303a 72e3 ec25 21a2 63a4  IMg...0:r..%!.c.
+00002c40: a451 5655 e4a4 f058 d685 2be2 f163 095d  .QVU...X..+..c.]
+00002c50: c711 f055 f4a4 3089 717e 381a d5a5 4939  ...U..0.q~8...I9
+00002c60: 87f4 4135 2f2b 6019 57b5 1cc2 f0a8 4d44  ..A5/+`.W.....MD
+00002c70: f5bc 26a3 b43e 29cb 3897 8d0e c562 17a3  ..&..>).8....b..
+00002c80: 3994 5184 88a4 1614 0ceb 9e8f 0b91 8292  9.Q.............
+00002c90: 7950 90af 51e4 e225 414c e819 3181 4567  yP..Q..%AL..1.Eg
+00002ca0: aa46 de18 b6b5 bedf 9e4a 44b1 9888 fa38  .F.......JD....8
+00002cb0: b501 ea54 5e92 f9b5 ee93 05d7 aa93 4dcb  ...T^.........M.
+00002cc0: 6e3e bda9 a655 4c1a 6d6f e353 7763 cf5d  n>...UL.mo.Swc.]
+00002cd0: adff 2e95 59c7 8c82 19c8 cf66 58cf 2309  ....Y......fX.#.
+00002ce0: b284 7075 597b 280b e278 5645 38c2 5045  ..puY{(..xVE8.PE
+00002cf0: 1d6b b041 2c3a a6aa 5916 439a 861e 73c1  .k.A,:..Y.C...s.
+00002d00: 1488 f00d 3c9d 7446 6203 16c7 0b8a 84e1  ....<.tFb.......
+00002d10: dc58 951e 7e0a 0d8c 2595 4236 3b20 0597  .X..~...%.B6; ..
+00002d20: d32c 116b 7e10 9c4c c010 04ce 8b11 6cbc  .,.k~..L......l.
+00002d30: 60dc f61b 52fd c5ae e02c 7d27 d687 10fa  `...R....,}'....
+00002d40: a3ee 96f7 5894 d496 dded 2ddb dc0d 19cc  ....X.....-.....
+00002d50: 69b2 f39a 459d a51d b735 c3a2 54a4 8f2d  i...E....5..T..-
+00002d60: d0e9 63ab 2d93 2766 486d d602 7a08 5d6d  ..c.-.'fHm..z.]m
+00002d70: 92fa 0aa9 96c1 46b8 8c33 a463 b94b 9b10  ......F..3.c.K..
+00002d80: 8c53 ffb1 dfae d8e6 82dd 5e81 9224 b3cd  .S........^..$..
+00002d90: fdf6 1c2b e876 5a5e 63b1 6ffe 8ef1 992c  ...+.vZ^c.o....,
+00002da0: 5ae4 e502 d5fb 9b37 3fb9 437d 4e8a 9934  Z......7?.C}N..4
+00002db0: ab97 0af7 8698 0afa 20c4 e457 4f8a 57c0  ........ ..WO.W.
+00002dc0: b4a0 420a 7dcb eca0 00b9 52bc fa4b f5aa  ..B.}.....R..K..
+00002dd0: 3eb4 44cf 90ca 230d e574 d67e a64f 127d  >.D...#..t.~.O.}
+00002de0: 9b23 f5b7 eef0 8dbc f08e 0eb1 ff9b 58f1  .#............X.
+00002df0: e250 f15c f17c f102 9b00 2a8e 1525 161c  .P.\.|....*..%..
+00002e00: b933 7abd 78e3 eaad bbd7 59cb c907 0515  .3z.x.....Y.....
+00002e10: 5f56 504e a677 c3f4 32a2 e6e8 4d91 5ed0  _VPN.w..2...M.^.
+00002e20: 44cf 1e8f 3112 fc49 9987 4182 4f21 6d42  D...1..I..A.O!mB
+00002e30: 3f7d f244 3c76 5993 7141 5322 3e10 3c33  ?}.D<vY.qAS">.<3
+00002e40: 22e2 019f 928f 7adc 83b1 3520 dd67 f95e  ".....z...5 .g.^
+00002e50: e71d 3493 d778 0f33 9f18 9ffc e13e fbdc  ..4..x.3.....>..
+00002e60: 359e 416f 914a a847 0fd9 5da3 e46d 4dd1  5.Ao.J.G..]..mM.
+00002e70: 0ee0 48da e667 da55 ceee 066d b2fd f673  ..H..g.U...m...s
+00002e80: 5f32 e855 d601 2116 094e 8505 39e7 711b  _2.U..!..N..9.q.
+00002e90: de9e 2c8d bcaa c097 4521 3dd7 5823 d586  ..,.....E!=.X#..
+00002ea0: 53de f563 b1d6 ed56 c9de ab74 a72d 88cb  S..c...V...t.-..
+00002eb0: 79db a0a0 d3f8 e22c afdb 9661 9b30 527c  y......,...a.0R|
+00002ec0: 1a3c 7a3f bf79 56ab 3bbb 70e0 6896 0004  .<z?.yV.;.p.h...
+00002ed0: 17f2 7106 de81 c126 3b95 4530 c25c f633  ..q....&;.E0.\.3
+00002ee0: 5f7b 41cc 3208 0305 7077 e590 e5d6 e6bc  _{A.2...pw......
+00002ef0: da16 69ac 39f3 af6c ab1a 04b1 0d76 67f9  ..i.9..l.....vg.
+00002f00: 2729 bd1b 0c3e 3ed8 5e71 6a2d 1f0f a271  ')...>>.^qj-...q
+00002f10: 66aa f6de 1cac 04bb 0f87 73a8 4a8c 1d77  f.........s.J..w
+00002f20: f56d 2f02 f003 7ffa eb5f c8ce 5760 dacd  .m/......_..W`..
+00002f30: a6dd da86 a3f2 9abb dda9 0e68 daa6 e16d  ...........h...m
+00002f40: 76c2 ef6e 7ef9 d109 157a 531f a94a 76a3  v..n~....zS..Jv.
+00002f50: 7b05 c8e2 dcd2 89ff 136b 8865 d15e e235  {........k.e.^.5
+00002f60: dbd0 3f74 5b14 fe64 897f 0050 4b03 0414  ..?t[..d...PK...
+00002f70: 0000 0008 0087 4ee2 40e6 7389 e30e 0200  ......N.@.s.....
+00002f80: 0055 0400 000f 0000 0078 6c2f 776f 726b  .U.......xl/work
+00002f90: 626f 6f6b 2e78 6d6c 8d54 cb6e d340 14dd  book.xml.T.n.@..
+00002fa0: 23f1 0fd6 ec9d b19d a424 519c 2a6e 6251  #........$Q.*nbQ
+00002fb0: a9a9 aa10 5258 a1a9 7d1d 8f6a cf58 3393  ....RX..}..j.X3.
+00002fc0: 2608 c10f b067 8f84 f803 362c f81a 24d4  &....g....6,..$.
+00002fd0: bfe0 da4e d2a0 02f2 6a32 67ce 3df7 dc47  ...N....j2g.=..G
+00002fe0: 3c3c dde6 9975 074a 7329 7ce2 b61c 6281  <<...u.Js)|...b.
+00002ff0: 8864 ccc5 ca27 2f17 a1dd 2396 364c c42c  .d...'/...#.6L.,
+00003000: 9302 7cf2 1634 391d 3d7d 32dc 4875 7b23  ..|..49.=}2.Hu{#
+00003010: e5ad 8502 42fb 2435 a618 50aa a314 72a6  ....B.$5..P...r.
+00003020: 5bb2 0081 2f89 5439 3378 552b aa0b 052c  [.../.T93xU+...,
+00003030: d629 80c9 33ea 39ce 09cd 1917 a456 18a8  .)..3.9......V..
+00003040: 261a 3249 7804 1319 ad73 10a6 1651 9031  &.2Ix....s...Q.1
+00003050: 83f6 75ca 0b4d 46c3 8467 b0ac 2bb2 5851  ..u..MF..g..+.XQ
+00003060: 5cb2 1c7d 6f33 6265 4c9b 69cc 0dc4 3e69  \..}o3beL.i...>i
+00003070: e355 6ee0 01e8 124b ad8b 60cd 337c edb7  .Un....K..`.3|..
+00003080: 1d8f d0d1 a1c8 2b85 97b2 da25 878d 7ec0  ......+....%..~.
+00003090: cbab b5e1 2296 9b6b 1e9b 1475 3dcf 41a9  ...."..k...u=.A.
+000030a0: 1a7b 0e7c 951a 6c6b cf39 c1c6 b2c8 f03b  .{.|..lk.9.....;
+000030b0: 58b0 1b44 4a75 7aa4 58b5 0595 abd3 1295  X..DJuz.X.......
+000030c0: e70f f75f 3fdd 7ffe 8603 287b 768e be3c  ..._?.....({v..<
+000030d0: 3439 e0f8 439d c795 c431 fdd7 97ef 3f7f  49..C....1....?.
+000030e0: 7cb4 63c8 e551 887b 1452 d5f4 8f10 943e  |.c..Q.{.R.....>
+000030f0: a4c1 e61c d2b4 2ba7 d513 da8b 5816 5d29  ......+.....X.])
+00003100: ab3c 4a3f 6edf 75bc 7ec9 80ad b9d0 a63a  .<J?n.u.~......:
+00003110: adb5 e23e 7917 747b 81d3 ee7b 7627 7443  ...>y.t{...{v'tC
+00003120: bbe3 f61d 3b08 4e3a 7677 12b6 bbcf dcc9  ....;.N:vw......
+00003130: d9b4 1bbe df0f 7f5b 2a26 8f36 20e7 9192  .......[*&.6 ...
+00003140: 5a26 a615 c99c d6c3 7fb4 476e 8f56 d1c0  Z&........Gn.V..
+00003150: cc5a e17a 8e86 b5da a044 c31d 7a00 931a  .Z.z.....D..z...
+00003160: d8b5 f88f 0483 f9a4 2c65 17fd 3fe2 0bfc  ........,e..?...
+00003170: 7b64 d090 1c2e 1b12 cf2e 678b 5943 eec5  {d........g.YC..
+00003180: 74f1 e63a 6c4a 1ecf 82c9 b839 7f3c 9f8f  t..:lJ.....9.<..
+00003190: 5f2f a6af f629 e85f 1b4a 71e6 b8c4 fbc9  _/...)._.Jq.....
+000031a0: d3fd 1761 f41b 504b 0304 0a00 0000 0000  ...a..PK........
+000031b0: 874e e240 0000 0000 0000 0000 0000 0000  .N.@............
+000031c0: 0600 0000 5f72 656c 732f 504b 0304 1400  ...._rels/PK....
+000031d0: 0000 0800 874e e240 7b38 76bc ff00 0000  .....N.@{8v.....
+000031e0: df02 0000 0b00 0000 5f72 656c 732f 2e72  ........_rels/.r
+000031f0: 656c 73ad 92cf 4ac4 3010 c6ef 82ef 10e6  els...J.0.......
+00003200: be4d 7715 11d9 742f 22ec 4d64 7d80 984c  .Mw...t/".Md}..L
+00003210: ffd0 2613 9259 edbe bd41 512c d4ba 078f  ..&..Y...AQ,....
+00003220: 99f9 e69b df7c 64bb 1bdd 205e 31a6 8ebc  .....|d... ^1...
+00003230: 8275 5182 406f c876 be51 f07c 7858 dd82  .uQ.@o.v.Q.|xX..
+00003240: 48ac bdd5 0379 5470 c204 bbea f262 fb84  H....yTp.....b..
+00003250: 83e6 3c94 da2e 2491 5d7c 52d0 3287 3b29  ..<...$.]|R.2.;)
+00003260: 9369 d1e9 5450 409f 3b35 45a7 393f 6323  .i..TP@.;5E.9?c#
+00003270: 8336 bd6e 506e caf2 46c6 9f1e 504d 3cc5  .6.nPn..F...PM<.
+00003280: de2a 887b bb06 7138 85bc f96f 6faa ebce  .*.{..q8...oo...
+00003290: e03d 99a3 43cf 332b e454 919d 756c 9015  .=..C.3+.T..ul..
+000032a0: 8c83 7ca3 d8bf 10f5 4506 0639 cf72 753e  ..|.....E..9.ru>
+000032b0: cbef 774a 87ac ad66 2d0d 455c 8598 538a  ..wJ...f-.E\..S.
+000032c0: dce5 5cbf 712c 99c7 5c4e 1f8a 25a0 cdf9  ..\.q,..\N..%...
+000032d0: 40d3 d3e7 c2c1 91d1 5bb4 cb48 3a84 25a2  @.......[..H:.%.
+000032e0: ebff 2432 c7c4 e496 793e 355f 4872 f22d  ..$2....y>5_Hr.-
+000032f0: ab77 504b 0304 0a00 0000 0000 874e e240  .wPK.........N.@
+00003300: 0000 0000 0000 0000 0000 0000 0900 0000  ................
+00003310: 786c 2f5f 7265 6c73 2f50 4b03 0414 0000  xl/_rels/PK.....
+00003320: 0008 0087 4ee2 4020 f8ee 19fb 0000 00d4  ....N.@ ........
+00003330: 0300 001a 0000 0078 6c2f 5f72 656c 732f  .......xl/_rels/
+00003340: 776f 726b 626f 6f6b 2e78 6d6c 2e72 656c  workbook.xml.rel
+00003350: 73bd 93cb 6ac3 3010 45f7 85fe 8398 7d2d  s...j.0.E.....}-
+00003360: db69 4309 91b3 2985 6cdb f403 843d 7e10  .iC...).l....=~.
+00003370: 5b32 9ae9 c37f dfc1 8bb8 86e0 6e4c 3682  [2..........nL6.
+00003380: 9941 f79e d145 fbc3 4fd7 aa2f 0cd4 7867  .A...E..O../..xg
+00003390: 2089 6250 e872 5f34 ae32 f071 7a7d 7806   .bP.r_4.2.qz}x.
+000033a0: 456c 5d61 5bef d0c0 8004 87ec fe6e ff86  El]a[........n..
+000033b0: ad65 b944 75d3 9312 1547 066a e67e a735  .e.Du....G.j.~.5
+000033c0: e535 7696 22df a393 49e9 4367 59ca 50e9  .5v."...I.CgY.P.
+000033d0: dee6 675b a14e e378 abc3 5f0d c866 9aea  ..g[.N.x.._..f..
+000033e0: 5818 08c7 620b ea34 f4e2 fcbf b62f cb26  X...b..4...../.&
+000033f0: c717 9f7f 76e8 f88a 85a6 da06 2cde 39c8  ....v.......,.9.
+00003400: 7a24 c236 54c8 0666 ed48 8841 5f87 795a  z$.6T..f.H.A_.yZ
+00003410: 1586 8756 5e73 a218 eb25 fbc7 35ed 5932  ...V^s...%..5.Y2
+00003420: c2c9 7d2c f578 264b 0c9b 3519 be7d 3853  ..},.x&K..5..}8S
+00003430: 8dc8 13c7 a545 9296 4c36 4b30 e98d 61d2  .....E..L6K0..a.
+00003440: 2598 e4c6 3097 98f4 ec2f 66bf 504b 0304  %...0..../f.PK..
+00003450: 0a00 0000 0000 874e e240 0000 0000 0000  .......N.@......
+00003460: 0000 0000 0000 1400 0000 786c 2f77 6f72  ..........xl/wor
+00003470: 6b73 6865 6574 732f 5f72 656c 732f 504b  ksheets/_rels/PK
+00003480: 0304 1400 0000 0800 874e e240 691f 49c5  .........N.@i.I.
+00003490: cf00 0000 b801 0000 2300 0000 786c 2f77  ........#...xl/w
+000034a0: 6f72 6b73 6865 6574 732f 5f72 656c 732f  orksheets/_rels/
+000034b0: 7368 6565 7432 2e78 6d6c 2e72 656c 73ad  sheet2.xml.rels.
+000034c0: 90c9 6a03 310c 40ef 85fe 83d1 3dd6 4c0e  ..j.1.@.....=.L.
+000034d0: a194 7872 0985 5c43 fa01 c2d6 2c74 bc60  ..xr..\C....,t.`
+000034e0: b969 f2f7 7528 850c 047a e951 dbd3 93b6  .i..u(...z.Q....
+000034f0: bb8b 9fd5 99b3 4c31 1868 7503 8a83 8d6e  ......L1.hu....n
+00003500: 0a83 81f7 d3db ea05 9414 0a8e e618 d8c0  ................
+00003510: 9505 76dd f3d3 f6c8 3395 3a24 e394 4455  ..v.....3.:$..DU
+00003520: 4a10 0363 29e9 1551 ecc8 9e44 c7c4 a156  J..c)..Q...D...V
+00003530: fa98 3d95 1ae6 0113 d90f 1a18 d74d b3c1  ..=..........M..
+00003540: 7ccf 806e c154 0767 201f dc1a d4e9 9aea  |..n.T.g .......
+00003550: e6bf d9b1 ef27 cbfb 683f 3d87 f260 059e  .....'..h?=..`..
+00003560: fdbc cff4 558f ab54 ca03 1703 5aa3 fbc9  ....U..T....Z...
+00003570: c95d bdd5 b517 f0b1 53fb 9f4e 36fa 9bae  .]......S..N6...
+00003580: 2c8c 7e93 adae ffbb 69e0 e2df dd37 504b  ,.~.....i....7PK
+00003590: 0304 1400 0000 0800 874e e240 d9a1 06c4  .........N.@....
+000035a0: cf00 0000 b801 0000 2300 0000 786c 2f77  ........#...xl/w
+000035b0: 6f72 6b73 6865 6574 732f 5f72 656c 732f  orksheets/_rels/
+000035c0: 7368 6565 7433 2e78 6d6c 2e72 656c 73ad  sheet3.xml.rels.
+000035d0: 90c9 6a03 310c 40ef 85fe 83d1 3dd6 640e  ..j.1.@.....=.d.
+000035e0: a194 7872 0985 5c43 fa01 c6d6 2c74 bc60  ..xr..\C....,t.`
+000035f0: b969 f2f7 5528 850c 047a e951 dbd3 93b6  .i..U(...z.Q....
+00003600: bb4b 98d5 990a 4f29 1a58 eb06 1445 97fc  .K....O).X...E..
+00003610: 1407 03ef a7b7 d50b 28ae 367a 3ba7 4806  ........(.6z;.H.
+00003620: aec4 b0eb 9e9f b647 9a6d 9521 1ea7 cc4a  .......G.m.!...J
+00003630: 2891 0d8c b5e6 5744 7623 05cb 3a65 8a52  (.....WDv#..:e.R
+00003640: e953 09b6 4a58 06cc d67d d881 b06d 9a0d  .S..JX...}...m..
+00003650: 967b 0674 0ba6 3a78 03e5 e05b 50a7 6b96  .{.t..:x...[P.k.
+00003660: cd7f b353 df4f 8ef6 c97d 068a f5c1 0a3c  ...S.O...}.....<
+00003670: 8779 5fec 971c 2754 5b06 aa06 b446 ff93  .y_...'T[....F..
+00003680: e3bb 7aab a517 f0b1 d3fa 3f9d 5c0a 375d  ..z.......?.\.7]
+00003690: 5e18 fd26 5b2d ffbb 69e0 e2df dd37 504b  ^..&[-..i....7PK
+000036a0: 0304 1400 0000 0800 874e e240 22d0 7e19  .........N.@".~.
+000036b0: 9101 0000 7c07 0000 1300 0000 5b43 6f6e  ....|.......[Con
+000036c0: 7465 6e74 5f54 7970 6573 5d2e 786d 6cc5  tent_Types].xml.
+000036d0: 95dd 4ec2 4010 85ef 4d7c 8766 6f0d 5dc0  ..N.@...M|.fo.].
+000036e0: c418 43e1 42f4 524d c407 5877 07da b07f  ..C.B.RM..Xw....
+000036f0: d959 10de dee9 0246 fcc3 4a13 6fda b4db  .Y.....F..J.o...
+00003700: 39df 39b3 d376 305a 199d 2d21 60e5 6cc1  9.9..v0Z..-!`.l.
+00003710: 7a79 9765 60a5 5395 9d15 ec69 72db b964  zy.e`.S....ir..d
+00003720: 1946 6195 d0ce 42c1 d680 6c34 3c3d 194c  .Fa...B...l4<=.L
+00003730: d61e 30a3 6a8b 052b 63f4 579c a32c c108  ..0.j..+c.W..,..
+00003740: cc9d 074b 2b53 178c 8874 1966 dc0b 3917  ...K+S...t.f..9.
+00003750: 33e0 fd6e f782 4b67 23d8 d889 b506 1b0e  3..n..Kg#.......
+00003760: c630 150b 1db3 9b15 ddde 3859 1acd b2eb  .0........8Y....
+00003770: cd73 35aa 60c2 7b5d 4911 c928 5f5a f501  .s5.`.{]I..(_Z..
+00003780: d271 d369 2541 39b9 3024 9d53 fd38 8817  .q.i%A9.0$.S.8..
+00003790: 8ac1 f897 8000 1a9b 11b6 1172 aa4c 2eb0  ...........r.L..
+000037a0: ac3c 9e51 ce6f 08f5 caf7 11b6 75f7 d4fb  .<.Q.o......u...
+000037b0: 5029 c81e 4488 77c2 5050 4e21 1e82 f3c8  P)..D.w.PPN!....
+000037c0: 2972 feb3 cae1 4640 dd53 05aa e349 1242  )r....F@.S...I.B
+000037d0: ace0 cdf3 8f6c e902 3487 ef7a 5457 3726  .....l..4..zTW7&
+000037e0: 2e30 3ad3 9cf9 61e7 6592 f925 7ca5 6918  .0:...a.e..%|.i.
+000037f0: 4d3d 31d8 3b9a 8c3e 8050 5802 44a3 f39d  M=1.;..>.PX.D...
+00003800: ee6e 42be eaf6 3b7c ff7f f058 8a00 ea31  .nB...;|...X...1
+00003810: 067a 53b0 650b 7bda 07da 8071 ada1 7503  .zS.e.{....q..u.
+00003820: 49f4 0039 d237 0b78 3a1e 3f02 49e6 00f0  I..9.7.x:.?.I...
+00003830: c585 f9b3 73f3 d6bb 4d73 971b 51d9 5ff0  ....s...Ms..Q._.
+00003840: d390 224f a7e3 53ef 0f7e 9d2f 0937 f4d1  .."O..S..~./.7..
+00003850: f61b f057 1fe7 2d6f cc27 1f3c fd3b 87af  ...W..-o.'.<.;..
+00003860: 504b 0102 1400 1400 0000 0800 874e e240  PK...........N.@
+00003870: 22d0 7e19 9101 0000 7c07 0000 1300 0000  ".~.....|.......
+00003880: 0000 0000 0100 2000 0000 9e36 0000 5b43  ...... ....6..[C
+00003890: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
+000038a0: 6c50 4b01 0214 000a 0000 0000 0087 4ee2  lPK...........N.
+000038b0: 4000 0000 0000 0000 0000 0000 0006 0000  @...............
+000038c0: 0000 0000 0000 0010 0000 00a6 3100 005f  ............1.._
+000038d0: 7265 6c73 2f50 4b01 0214 0014 0000 0008  rels/PK.........
+000038e0: 0087 4ee2 407b 3876 bcff 0000 00df 0200  ..N.@{8v........
+000038f0: 000b 0000 0000 0000 0001 0020 0000 00ca  ........... ....
+00003900: 3100 005f 7265 6c73 2f2e 7265 6c73 504b  1.._rels/.relsPK
+00003910: 0102 1400 0a00 0000 0000 874e e240 0000  ...........N.@..
+00003920: 0000 0000 0000 0000 0000 0900 0000 0000  ................
+00003930: 0000 0000 1000 0000 0000 0000 646f 6350  ............docP
+00003940: 726f 7073 2f50 4b01 0214 0014 0000 0008  rops/PK.........
+00003950: 0087 4ee2 4053 d3bb 5449 0100 007b 0200  ..N.@S..TI...{..
+00003960: 0010 0000 0000 0000 0001 0020 0000 0027  ........... ...'
+00003970: 0000 0064 6f63 5072 6f70 732f 6170 702e  ...docProps/app.
+00003980: 786d 6c50 4b01 0214 0014 0000 0008 0087  xmlPK...........
+00003990: 4ee2 400a 45e1 2f43 0100 003e 0200 0011  N.@.E./C...>....
+000039a0: 0000 0000 0000 0001 0020 0000 009e 0100  ......... ......
+000039b0: 0064 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
+000039c0: 6d6c 504b 0102 1400 1400 0000 0800 874e  mlPK...........N
+000039d0: e240 c42d 5503 2801 0000 0e02 0000 1300  .@.-U.(.........
+000039e0: 0000 0000 0000 0100 2000 0000 1003 0000  ........ .......
+000039f0: 646f 6350 726f 7073 2f63 7573 746f 6d2e  docProps/custom.
+00003a00: 786d 6c50 4b01 0214 000a 0000 0000 0087  xmlPK...........
+00003a10: 4ee2 4000 0000 0000 0000 0000 0000 0003  N.@.............
+00003a20: 0000 0000 0000 0000 0010 0000 0069 0400  .............i..
+00003a30: 0078 6c2f 504b 0102 1400 0a00 0000 0000  .xl/PK..........
+00003a40: 874e e240 0000 0000 0000 0000 0000 0000  .N.@............
+00003a50: 0900 0000 0000 0000 0000 1000 0000 f232  ...............2
+00003a60: 0000 786c 2f5f 7265 6c73 2f50 4b01 0214  ..xl/_rels/PK...
+00003a70: 0014 0000 0008 0087 4ee2 4020 f8ee 19fb  ........N.@ ....
+00003a80: 0000 00d4 0300 001a 0000 0000 0000 0001  ................
+00003a90: 0020 0000 0019 3300 0078 6c2f 5f72 656c  . ....3..xl/_rel
+00003aa0: 732f 776f 726b 626f 6f6b 2e78 6d6c 2e72  s/workbook.xml.r
+00003ab0: 656c 7350 4b01 0214 0014 0000 0008 0087  elsPK...........
+00003ac0: 4ee2 40a0 000b 0877 0100 0019 0400 0010  N.@....w........
+00003ad0: 0000 0000 0000 0001 0020 0000 008a 0400  ......... ......
+00003ae0: 0078 6c2f 636f 6d6d 656e 7473 312e 786d  .xl/comments1.xm
+00003af0: 6c50 4b01 0214 0014 0000 0008 0087 4ee2  lPK...........N.
+00003b00: 40a0 000b 0877 0100 0019 0400 0010 0000  @....w..........
+00003b10: 0000 0000 0001 0020 0000 002f 0600 0078  ....... .../...x
+00003b20: 6c2f 636f 6d6d 656e 7473 322e 786d 6c50  l/comments2.xmlP
+00003b30: 4b01 0214 000a 0000 0000 0087 4ee2 4000  K...........N.@.
+00003b40: 0000 0000 0000 0000 0000 000c 0000 0000  ................
+00003b50: 0000 0000 0010 0000 0027 0a00 0078 6c2f  .........'...xl/
+00003b60: 6472 6177 696e 6773 2f50 4b01 0214 0014  drawings/PK.....
+00003b70: 0000 0008 0087 4ee2 40df ec4e b6da 0200  ......N.@..N....
+00003b80: 00c7 0a00 001b 0000 0000 0000 0001 0020  ............... 
+00003b90: 0000 0051 0a00 0078 6c2f 6472 6177 696e  ...Q...xl/drawin
+00003ba0: 6773 2f76 6d6c 4472 6177 696e 6731 2e76  gs/vmlDrawing1.v
+00003bb0: 6d6c 504b 0102 1400 1400 0000 0800 874e  mlPK...........N
+00003bc0: e240 8ae2 eb49 d202 0000 c10a 0000 1b00  .@...I..........
+00003bd0: 0000 0000 0000 0100 2000 0000 6912 0000  ........ ...i...
+00003be0: 786c 2f64 7261 7769 6e67 732f 766d 6c44  xl/drawings/vmlD
+00003bf0: 7261 7769 6e67 322e 766d 6c50 4b01 0214  rawing2.vmlPK...
+00003c00: 0014 0000 0008 0087 4ee2 40f4 d54e 5ea6  ........N.@..N^.
+00003c10: 0300 00a3 0900 0014 0000 0000 0000 0001  ................
+00003c20: 0020 0000 0093 2b00 0078 6c2f 7368 6172  . ....+..xl/shar
+00003c30: 6564 5374 7269 6e67 732e 786d 6c50 4b01  edStrings.xmlPK.
+00003c40: 0214 0014 0000 0008 0087 4ee2 4074 e6b0  ..........N.@t..
+00003c50: 2283 0a00 0092 5100 000d 0000 0000 0000  ".....Q.........
+00003c60: 0001 0020 0000 00e5 2000 0078 6c2f 7374  ... .... ..xl/st
+00003c70: 796c 6573 2e78 6d6c 504b 0102 1400 0a00  yles.xmlPK......
+00003c80: 0000 0000 874e e240 0000 0000 0000 0000  .....N.@........
+00003c90: 0000 0000 0900 0000 0000 0000 0000 1000  ................
+00003ca0: 0000 9a1a 0000 786c 2f74 6865 6d65 2f50  ......xl/theme/P
+00003cb0: 4b01 0214 0014 0000 0008 0087 4ee2 40f8  K...........N.@.
+00003cc0: 8e8c 59f3 0500 002b 1900 0013 0000 0000  ..Y....+........
+00003cd0: 0000 0001 0020 0000 00c1 1a00 0078 6c2f  ..... .......xl/
+00003ce0: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
+00003cf0: 504b 0102 1400 1400 0000 0800 874e e240  PK...........N.@
+00003d00: e673 89e3 0e02 0000 5504 0000 0f00 0000  .s......U.......
+00003d10: 0000 0000 0100 2000 0000 6b2f 0000 786c  ...... ...k/..xl
+00003d20: 2f77 6f72 6b62 6f6f 6b2e 786d 6c50 4b01  /workbook.xmlPK.
+00003d30: 0214 000a 0000 0000 0087 4ee2 4000 0000  ..........N.@...
+00003d40: 0000 0000 0000 0000 000e 0000 0000 0000  ................
+00003d50: 0000 0010 0000 00d4 0700 0078 6c2f 776f  ...........xl/wo
+00003d60: 726b 7368 6565 7473 2f50 4b01 0214 000a  rksheets/PK.....
+00003d70: 0000 0000 0087 4ee2 4000 0000 0000 0000  ......N.@.......
+00003d80: 0000 0000 0014 0000 0000 0000 0000 0010  ................
+00003d90: 0000 004c 3400 0078 6c2f 776f 726b 7368  ...L4..xl/worksh
+00003da0: 6565 7473 2f5f 7265 6c73 2f50 4b01 0214  eets/_rels/PK...
+00003db0: 0014 0000 0008 0087 4ee2 4069 1f49 c5cf  ........N.@i.I..
+00003dc0: 0000 00b8 0100 0023 0000 0000 0000 0001  .......#........
+00003dd0: 0020 0000 007e 3400 0078 6c2f 776f 726b  . ...~4..xl/work
+00003de0: 7368 6565 7473 2f5f 7265 6c73 2f73 6865  sheets/_rels/she
+00003df0: 6574 322e 786d 6c2e 7265 6c73 504b 0102  et2.xml.relsPK..
+00003e00: 1400 1400 0000 0800 874e e240 d9a1 06c4  .........N.@....
+00003e10: cf00 0000 b801 0000 2300 0000 0000 0000  ........#.......
+00003e20: 0100 2000 0000 8e35 0000 786c 2f77 6f72  .. ....5..xl/wor
+00003e30: 6b73 6865 6574 732f 5f72 656c 732f 7368  ksheets/_rels/sh
+00003e40: 6565 7433 2e78 6d6c 2e72 656c 7350 4b01  eet3.xml.relsPK.
+00003e50: 0214 0014 0000 0008 0087 4ee2 400c 0708  ..........N.@...
+00003e60: 2df1 0100 0005 0400 0018 0000 0000 0000  -...............
+00003e70: 0001 0020 0000 0000 0800 0078 6c2f 776f  ... .......xl/wo
+00003e80: 726b 7368 6565 7473 2f73 6865 6574 312e  rksheets/sheet1.
+00003e90: 786d 6c50 4b01 0214 0014 0000 0008 0087  xmlPK...........
+00003ea0: 4ee2 40fb 5c74 f7cf 0400 0089 1100 0018  N.@.\t..........
+00003eb0: 0000 0000 0000 0001 0020 0000 0064 0d00  ......... ...d..
+00003ec0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00003ed0: 6865 6574 322e 786d 6c50 4b01 0214 0014  heet2.xmlPK.....
+00003ee0: 0000 0008 0087 4ee2 4071 12a7 1bf0 0400  ......N.@q......
+00003ef0: 00eb 1100 0018 0000 0000 0000 0001 0020  ............... 
+00003f00: 0000 0074 1500 0078 6c2f 776f 726b 7368  ...t...xl/worksh
+00003f10: 6565 7473 2f73 6865 6574 332e 786d 6c50  eets/sheet3.xmlP
+00003f20: 4b05 0600 0000 001b 001b 00bf 0600 0060  K..............`
+00003f30: 3800 0000 00                             8....
```

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/__init__.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/__init__.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/bool.py` & `gd_excelexporter-3.0.1a0/src/gd_excelexporter/type_defines/bool.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-3.0.0a1/PKG-INFO` & `gd_excelexporter-3.0.1a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gd_excelexporter
-Version: 3.0.0a1
+Version: 3.0.1a0
 Summary: Godot Excel导表工具
 License: MIT
 Author: kaluluosi
 Author-email: kaluluosi@gamil.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -80,15 +80,15 @@
 Platform: Windows(xlwings只支持Windows)
 
 Godot版本:^3.4
 
 ### 安装
 通过pip （建议）
 ```
-pip install gd-gd_excelexporter
+pip install gd_excelexporter
 ```
 
 或者直接去右边release里下载已经打包好的可执行文件（ee.exe，你需要将这个exe加到环境变量）。
 
 ### 创建配置表项目
 
 打开你的Godot游戏项目，项目根目录下右键打开命令行（此处打开powershell）
@@ -274,10 +274,12 @@
 
 ## 最后
 希望这个工具能够给一些独立游戏人或者业余自娱自乐的人一些帮助。
 如果你用上了我的工具，有什么问题最好直接提issue。
 
 如果你在你的独立游戏项目中使用了我的工具，希望你能够在游戏结尾员工名单或者开源证书页面中特别鸣谢加上我的名字，让我也占个光，谢谢。
 
-## 联系方式
+![Snipaste_2024-04-19_17-01-18](/assets/Snipaste_2024-04-19_17-01-18.png)
 
+## 联系方式
+QQ群：118258918
 ![Snipaste_2024-04-19_06-50-25](/assets/Snipaste_2024-04-19_06-50-25_icwxbsqi8.png)
```

