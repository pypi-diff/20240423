# Comparing `tmp/gti_scnu-0.0.8-py3-none-any.whl.zip` & `tmp/gti_scnu-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 18997 bytes, number of entries: 13
+Zip file size: 19228 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat        2 b- defN 23-Sep-22 08:56 gti/__init__.py
 -rw-rw-rw-  2.0 fat    10238 b- defN 23-Oct-09 04:58 gti/client.py
 -rw-rw-rw-  2.0 fat     2918 b- defN 23-Oct-08 13:32 gti/data_packet.py
 -rw-rw-rw-  2.0 fat     2413 b- defN 23-Oct-10 04:19 gti/decoder.py
 -rw-rw-rw-  2.0 fat     1915 b- defN 23-Sep-26 13:34 gti/encoder.py
 -rw-rw-rw-  2.0 fat     1574 b- defN 23-Oct-09 03:30 gti/json_builder.py
--rw-rw-rw-  2.0 fat    14209 b- defN 23-Oct-10 06:26 gti/parser.py
+-rw-rw-rw-  2.0 fat    15187 b- defN 23-Oct-10 07:08 gti/parser.py
 -rw-rw-rw-  2.0 fat    19770 b- defN 23-Oct-10 04:19 gti/server.py
 -rw-rw-rw-  2.0 fat      864 b- defN 23-Oct-09 03:30 gti/utils.py
--rw-rw-rw-  2.0 fat      549 b- defN 23-Oct-10 06:27 gti_scnu-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Oct-10 06:27 gti_scnu-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Oct-10 06:27 gti_scnu-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      943 b- defN 23-Oct-10 06:27 gti_scnu-0.0.8.dist-info/RECORD
-13 files, 55491 bytes uncompressed, 17461 bytes compressed:  68.5%
+-rw-rw-rw-  2.0 fat      780 b- defN 23-Oct-10 07:10 gti_scnu-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Oct-10 07:10 gti_scnu-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Oct-10 07:10 gti_scnu-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      943 b- defN 23-Oct-10 07:10 gti_scnu-0.0.9.dist-info/RECORD
+13 files, 56700 bytes uncompressed, 17692 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: gti/server.py
 Comment: 
 
 Filename: gti/utils.py
 Comment: 
 
-Filename: gti_scnu-0.0.8.dist-info/METADATA
+Filename: gti_scnu-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: gti_scnu-0.0.8.dist-info/WHEEL
+Filename: gti_scnu-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: gti_scnu-0.0.8.dist-info/top_level.txt
+Filename: gti_scnu-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: gti_scnu-0.0.8.dist-info/RECORD
+Filename: gti_scnu-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gti/parser.py

```diff
@@ -153,28 +153,41 @@
             # ast.walk 的遍历方式：广度优先，一层一层地遍历
             # ast.iter_child_nodes：只会遍历传入节点的子节点，不会遍历孙子节点之后的节点
             self.parse_node(node, body_list)
             # print(ast.dump(node))
         return body_list
 
     def parse_node(self, node, ast_list):
-        if isinstance(node, ast.ImportFrom) or isinstance(node, ast.Import):
-            # 说明这个节点是导入模块的语句
+        if isinstance(node, ast.ImportFrom):
+            # 说明这个节点是从模块导入模块的语句
             # 判断是否不是 gpio 库，如果不是则将该语句也加入到 body_list 中，本地也运行该语句
             # print('import: ', ast.dump(node), node.names[0].name)  # node.names[0].name 库名，例如 numpy；node.names[0].asname 库别名，例如 np
             # 需要判断是否是导入 gti 的库，如果在 gti 的库中，则不需要将该语句加入到 ast_list 中
             if astor.to_source(node).strip() == 'from gti.parser import Parser':
                 return
-            if node.names[0].name != 'gpio':
+            # 现阶段只需要将 control 库中的函数调用语句发送到机器人端，所以只需要判断是否是 control 库即可
+            if node.module == 'control':
+                if node.names[0].name != 'gpio':
+                    ast_list.append(node)
+                # 构造 client.send() 语句，用于机器人端导入模块
+                node = ast.Expr(
+                    value=ast.Call(
+                        func=ast.Attribute(value=ast.Name(id='client', ctx=ast.Load()), attr='send', ctx=ast.Load()),
+                        args=[ast.Constant(value=astor.to_source(node)), ast.Constant(value=1)], keywords=[]))
+        elif isinstance(node, ast.Import):
+            # 说明这个节点是导入模块的语句
+            # 判断这个类需不需要上传给机器人端运行
+            if node.names[0].name not in self.func_mapping.get('no_upload_module'):
+                # 说明这个类需要上传给机器人端运行，先将该语句加入到 ast_list 中
                 ast_list.append(node)
-            # 构造 client.send() 语句，用于机器人端导入模块
-            node = ast.Expr(
-                value=ast.Call(
-                    func=ast.Attribute(value=ast.Name(id='client', ctx=ast.Load()), attr='send', ctx=ast.Load()),
-                    args=[ast.Constant(value=astor.to_source(node)), ast.Constant(value=1)], keywords=[]))
+                # 构造 client.send() 语句，用于机器人端导入模块
+                node = ast.Expr(
+                    value=ast.Call(
+                        func=ast.Attribute(value=ast.Name(id='client', ctx=ast.Load()), attr='send', ctx=ast.Load()),
+                        args=[ast.Constant(value=astor.to_source(node)), ast.Constant(value=1)], keywords=[]))
         elif isinstance(node, ast.Assign) and isinstance(node.value, ast.Call):
             # 说明这个节点是赋值语句，有 = 的语句都是赋值语句
             if isinstance(node.value.func, ast.Attribute):
                 # 先获取赋值语句的 value 的函数名，然后判断是否是需要两端都运行的函数
                 class_name = node.value.func.attr
                 if class_name in self.func_mapping.get('both_class'):
                     # 说明是两端都需要运行的类，需要将该语句加入到 body_list 中
```

## Comparing `gti_scnu-0.0.8.dist-info/METADATA` & `gti_scnu-0.0.9.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: gti-scnu
-Version: 0.0.8
+Version: 0.0.9
 Summary: The remote control system for the HuaGuangEdu team
 Home-page: http://42.192.82.19/
 Author: gyanano
 Author-email: 1624055384@qq.com
 License: GPLv3
 Requires-Dist: astor
 
 The remote system for the HuaguangEdu Team
 >  The remote control system allows you to control the smart robot made by HuaguangEdu team remotely.
 
+version: 0.0.9
+1. fix the bug of the function of process the import and fromimport statement, and add the new field `no_upload_module` in the `AppFuncMapClient.json` to judge whether the module need to be uploaded to the robot
+
 version: 0.0.8
 1. fix the bug of the encoding of the code file when reading and writing the file
 
 version: 0.0.7
 1. add the function of saving the xml file
```

## Comparing `gti_scnu-0.0.8.dist-info/RECORD` & `gti_scnu-0.0.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 gti/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
 gti/client.py,sha256=zrwvklLuBWjWZ-Wqq6Pi_s4DIwin2-aGxI5nBbLORzM,10238
 gti/data_packet.py,sha256=RhMRh3GJfJPMxdMHJqBagOEY4iFgh0YWMu7JxBlZ97I,2918
 gti/decoder.py,sha256=oWoePZ7gPudF8JbTZPk1ZXWTpmVnX-blhbR2TAEzi9c,2413
 gti/encoder.py,sha256=fgs_mDXI0h7cdxsOE2jb9rR5e58fqaEeMyCzld8WQYc,1915
 gti/json_builder.py,sha256=mUObv85xn60ncKOk6GdCE0PyfQknGx06VHvv2JPx_Dw,1574
-gti/parser.py,sha256=qV27_f1TofX2ohdD236t9s5L0XWOjAF8NSYKhu5uM6A,14209
+gti/parser.py,sha256=uZTvmmmkffxLfAxWvH2TMmDrsXVZwwGAN9Mvi4rcnrs,15187
 gti/server.py,sha256=3hsY0LWVkeIn1DD4IzBQNNFwquK_vY0vD4Y1R5U-97Q,19770
 gti/utils.py,sha256=GfTe0eh1eOfxkXVpKwXmtdTGcBE4QT_6Q7w38UQp3ZA,864
-gti_scnu-0.0.8.dist-info/METADATA,sha256=1Ggmy1po1z7EbMqQ6Y7Xx-cA5-F2CoTJsck41pDzVtI,549
-gti_scnu-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-gti_scnu-0.0.8.dist-info/top_level.txt,sha256=LnnP-s67N5DoMOF-pEZtY4JkFn1sRe7ADEouj7y4jX0,4
-gti_scnu-0.0.8.dist-info/RECORD,,
+gti_scnu-0.0.9.dist-info/METADATA,sha256=b8HkZvNjdIp8wWh6JbkJQsZ2ocymlbpMInpDEIwPPPg,780
+gti_scnu-0.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+gti_scnu-0.0.9.dist-info/top_level.txt,sha256=LnnP-s67N5DoMOF-pEZtY4JkFn1sRe7ADEouj7y4jX0,4
+gti_scnu-0.0.9.dist-info/RECORD,,
```

