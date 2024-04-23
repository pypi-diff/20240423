# Comparing `tmp/Plametal_calc-0.0.1-py3-none-any.whl.zip` & `tmp/Plametal_calc-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1522 bytes, number of entries: 6
--rw-r--r--  2.0 unx       53 b- defN 24-Apr-03 01:38 Plametal_calc/calc.py
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 01:53 Plametal_calc-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      262 b- defN 24-Apr-03 01:53 Plametal_calc-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 01:53 Plametal_calc-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Apr-03 01:53 Plametal_calc-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      488 b- defN 24-Apr-03 01:53 Plametal_calc-0.0.1.dist-info/RECORD
-6 files, 910 bytes uncompressed, 624 bytes compressed:  31.4%
+Zip file size: 1816 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      609 b- defN 24-Apr-23 16:56 Plametal_calc/calc.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-23 17:00 Plametal_calc-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      262 b- defN 24-Apr-23 17:00 Plametal_calc-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 17:00 Plametal_calc-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-23 17:00 Plametal_calc-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      489 b- defN 24-Apr-23 17:00 Plametal_calc-0.0.2.dist-info/RECORD
+6 files, 1467 bytes uncompressed, 918 bytes compressed:  37.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: Plametal_calc/calc.py
 Comment: 
 
-Filename: Plametal_calc-0.0.1.dist-info/LICENSE
+Filename: Plametal_calc-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: Plametal_calc-0.0.1.dist-info/METADATA
+Filename: Plametal_calc-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: Plametal_calc-0.0.1.dist-info/WHEEL
+Filename: Plametal_calc-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: Plametal_calc-0.0.1.dist-info/top_level.txt
+Filename: Plametal_calc-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: Plametal_calc-0.0.1.dist-info/RECORD
+Filename: Plametal_calc-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Plametal_calc/calc.py

```diff
@@ -1,5 +1,22 @@
 
-def plus(a+b):
-  return a + b
+def capitalize_first_letter(sentence):
+    
+    words = sentence.split()  # 문장을 단어 단위로 분리
+    capitalized_words = [word.capitalize() for word in words]  # 각 단어의 첫 글자를 대문자로 변환
+    return ' '.join(capitalized_words)  # 변환된 단어들을 다시 조합하여 문장으로 반환
+
+# 사용 예시
+    sentence = input()
+    result = capitalize_first_letter(sentence)
+    print(result)  # 출력: "Hello World"
+
+
+
+def remove_duplicates(lst):
+    return list(set(lst))
+
+
+    my_list = input().split()  
+    result = remove_duplicates(my_list)
+    print(result)
 
-print(plus(10, 100))
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

