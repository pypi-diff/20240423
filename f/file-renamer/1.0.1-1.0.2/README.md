# Comparing `tmp/file_renamer-1.0.1.tar.gz` & `tmp/file_renamer-1.0.2.tar.gz`

## Comparing `file_renamer-1.0.1.tar` & `file_renamer-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 file_renamer-1.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 file_renamer-1.0.1/src/file-renamer/__init__.py
--rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 file_renamer-1.0.1/src/file-renamer/form.ui
--rw-r--r--   0        0        0    17416 2020-02-02 00:00:00.000000 file_renamer-1.0.1/src/file-renamer/rename.py
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 file_renamer-1.0.1/src/file-renamer/ui_form.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 file_renamer-1.0.1/src/file-renamer/widget.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 file_renamer-1.0.1/src/file-renamer/lib/case_insensitive.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 file_renamer-1.0.1/src/file-renamer/lib/exceptions.py
--rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 file_renamer-1.0.1/src/file-renamer/lib/files.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 file_renamer-1.0.1/src/file-renamer/style/default.qss
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 file_renamer-1.0.1/src/file-renamer/style/default_macos.qss
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 file_renamer-1.0.1/src/file-renamer/style/default_win.qss
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 file_renamer-1.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 file_renamer-1.0.1/LICENSE
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 file_renamer-1.0.1/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 file_renamer-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 file_renamer-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 file_renamer-1.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 file_renamer-1.0.2/src/file-renamer/__init__.py
+-rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 file_renamer-1.0.2/src/file-renamer/form.ui
+-rw-r--r--   0        0        0    17082 2020-02-02 00:00:00.000000 file_renamer-1.0.2/src/file-renamer/rename.py
+-rw-r--r--   0        0        0     9122 2020-02-02 00:00:00.000000 file_renamer-1.0.2/src/file-renamer/ui_form.py
+-rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 file_renamer-1.0.2/src/file-renamer/widget.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 file_renamer-1.0.2/src/file-renamer/lib/case_insensitive.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 file_renamer-1.0.2/src/file-renamer/lib/exceptions.py
+-rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 file_renamer-1.0.2/src/file-renamer/lib/files.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 file_renamer-1.0.2/src/file-renamer/style/default.qss
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 file_renamer-1.0.2/src/file-renamer/style/default_macos.qss
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 file_renamer-1.0.2/src/file-renamer/style/default_win.qss
+-rwxr-xr-x   0        0        0    35149 2020-02-02 00:00:00.000000 file_renamer-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 file_renamer-1.0.2/README.md
+-rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 file_renamer-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 file_renamer-1.0.2/PKG-INFO
```

### Comparing `file_renamer-1.0.1/src/file-renamer/form.ui` & `file_renamer-1.0.2/src/file-renamer/form.ui`

 * *Files 6% similar despite different names*

#### Comparing `file_renamer-1.0.1/src/file-renamer/form.ui` & `file_renamer-1.0.2/src/file-renamer/form.ui`

```diff
@@ -7,19 +7,22 @@
         <x>0</x>
         <y>0</y>
         <width>800</width>
         <height>600</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>RENAMER</string>
+      <string>File Renamer</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
       <item row="0" column="0">
         <widget class="QGroupBox" name="browse">
+          <property name="focusPolicy">
+            <enum>Qt::StrongFocus</enum>
+          </property>
           <property name="title">
             <string/>
           </property>
           <layout class="QFormLayout" name="formLayout">
             <item row="0" column="0">
               <widget class="QPushButton" name="dir_btn">
                 <property name="text">
@@ -165,16 +168,19 @@
                 <property name="text">
                   <string>Search</string>
                 </property>
               </widget>
             </item>
             <item>
               <widget class="QLineEdit" name="search">
+                <property name="tabletTracking">
+                  <bool>false</bool>
+                </property>
                 <property name="focusPolicy">
-                  <enum>Qt::ClickFocus</enum>
+                  <enum>Qt::StrongFocus</enum>
                 </property>
                 <property name="text">
                   <string notr="true"/>
                 </property>
                 <property name="placeholderText">
                   <string notr="true"/>
                 </property>
@@ -185,16 +191,19 @@
                 <property name="text">
                   <string>Replace</string>
                 </property>
               </widget>
             </item>
             <item>
               <widget class="QLineEdit" name="replace">
+                <property name="tabletTracking">
+                  <bool>false</bool>
+                </property>
                 <property name="focusPolicy">
-                  <enum>Qt::ClickFocus</enum>
+                  <enum>Qt::StrongFocus</enum>
                 </property>
                 <property name="text">
                   <string/>
                 </property>
               </widget>
             </item>
             <item>
@@ -212,14 +221,29 @@
               </widget>
             </item>
           </layout>
         </widget>
       </item>
     </layout>
   </widget>
+  <tabstops>
+    <tabstop>dir_btn</tabstop>
+    <tabstop>dir_txt</tabstop>
+    <tabstop>dir_output</tabstop>
+    <tabstop>recursively</tabstop>
+    <tabstop>id</tabstop>
+    <tabstop>extension</tabstop>
+    <tabstop>comboBox</tabstop>
+    <tabstop>clear_btn</tabstop>
+    <tabstop>rename_btn</tabstop>
+    <tabstop>search</tabstop>
+    <tabstop>replace</tabstop>
+    <tabstop>regex</tabstop>
+    <tabstop>find_btn</tabstop>
+  </tabstops>
   <resources/>
   <connections>
     <connection>
       <sender>dir_btn</sender>
       <signal>clicked()</signal>
       <receiver>Widget</receiver>
       <slot>open_dir()</slot>
@@ -249,24 +273,24 @@
           <y>45</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>clear_btn</sender>
       <signal>clicked()</signal>
-      <receiver>dir_output</receiver>
+      <receiver>Widget</receiver>
       <slot>clear()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>523</x>
           <y>519</y>
         </hint>
         <hint type="destinationlabel">
-          <x>411</x>
-          <y>395</y>
+          <x>399</x>
+          <y>299</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>comboBox</sender>
       <signal>activated(int)</signal>
       <receiver>Widget</receiver>
@@ -385,9 +409,10 @@
     <slot>rename_files()</slot>
     <slot>add_recursively()</slot>
     <slot>keep_ext()</slot>
     <slot>keep_id()</slot>
     <slot>search_replace()</slot>
     <slot>regex()</slot>
     <slot>find()</slot>
+    <slot>clear()</slot>
   </slots>
 </ui>
```

### Comparing `file_renamer-1.0.1/src/file-renamer/rename.py` & `file_renamer-1.0.2/src/file-renamer/rename.py`

 * *Files 5% similar despite different names*

```diff
@@ -432,22 +432,14 @@
         self.files.find(**params)
         filename = ""
         filename2 = ""
         params["msg"] = ""
         pattern = ''
         replace = ''
 
-        """
-        # Metachars
-        char = [".", "^", "$", "*", "+", "?", "{", "}", "[", "]" "\\", "|"]
-        char.append("(")
-        char.append(")")
-        logging.info('char: %s', char)
-        """
-
         try:
             for filename in self.files.filelist:
                 logging.info("------------------------------")
                 params["filename"] = Path(filename)
                 logging.info('params["filename"]: %s', params["filename"])
                 self.file.clear()
                 self.file = self.files.split_name(**params)
@@ -462,19 +454,15 @@
                     p = re.compile(pattern)
 
                     result = p.search(filename2)
                     if result:
                         logging.info('result.group(): %s', result.group())
                         replace = params["ui"].replace.displayText()
                         raw_replace = repr(replace)[1:-1]  # raw string
-                        self.file['new'] = filename2.replace(
-                            result.group(),
-                            raw_replace,
-                            1
-                        )
+                        self.file['new'] = re.sub(pattern, replace, filename2)
                     else:
                         self.file['new'] = filename2
                 else:
                     logging.info('pattern: %s', pattern)
                     p = re.compile(re.escape(pattern))
                     result = p.search(filename2)
                     if result:
```

### Comparing `file_renamer-1.0.1/src/file-renamer/ui_form.py` & `file_renamer-1.0.2/src/file-renamer/ui_form.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'form.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.1
+## Created by: Qt User Interface Compiler version 6.6.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
@@ -25,14 +25,15 @@
         if not Widget.objectName():
             Widget.setObjectName(u"Widget")
         Widget.resize(800, 600)
         self.gridLayout = QGridLayout(Widget)
         self.gridLayout.setObjectName(u"gridLayout")
         self.browse = QGroupBox(Widget)
         self.browse.setObjectName(u"browse")
+        self.browse.setFocusPolicy(Qt.StrongFocus)
         self.formLayout = QFormLayout(self.browse)
         self.formLayout.setObjectName(u"formLayout")
         self.dir_btn = QPushButton(self.browse)
         self.dir_btn.setObjectName(u"dir_btn")
 
         self.formLayout.setWidget(0, QFormLayout.LabelRole, self.dir_btn)
 
@@ -113,28 +114,30 @@
         self.search_label = QLabel(self.search_replace)
         self.search_label.setObjectName(u"search_label")
 
         self.horizontalLayout_2.addWidget(self.search_label)
 
         self.search = QLineEdit(self.search_replace)
         self.search.setObjectName(u"search")
-        self.search.setFocusPolicy(Qt.ClickFocus)
+        self.search.setTabletTracking(False)
+        self.search.setFocusPolicy(Qt.StrongFocus)
         self.search.setText(u"")
         self.search.setPlaceholderText(u"")
 
         self.horizontalLayout_2.addWidget(self.search)
 
         self.replace_label = QLabel(self.search_replace)
         self.replace_label.setObjectName(u"replace_label")
 
         self.horizontalLayout_2.addWidget(self.replace_label)
 
         self.replace = QLineEdit(self.search_replace)
         self.replace.setObjectName(u"replace")
-        self.replace.setFocusPolicy(Qt.ClickFocus)
+        self.replace.setTabletTracking(False)
+        self.replace.setFocusPolicy(Qt.StrongFocus)
 
         self.horizontalLayout_2.addWidget(self.replace)
 
         self.regex = QCheckBox(self.search_replace)
         self.regex.setObjectName(u"regex")
 
         self.horizontalLayout_2.addWidget(self.regex)
@@ -143,32 +146,44 @@
         self.find_btn.setObjectName(u"find_btn")
 
         self.horizontalLayout_2.addWidget(self.find_btn)
 
 
         self.gridLayout.addWidget(self.search_replace, 4, 0, 1, 1)
 
+        QWidget.setTabOrder(self.dir_btn, self.dir_txt)
+        QWidget.setTabOrder(self.dir_txt, self.dir_output)
+        QWidget.setTabOrder(self.dir_output, self.recursively)
+        QWidget.setTabOrder(self.recursively, self.id)
+        QWidget.setTabOrder(self.id, self.extension)
+        QWidget.setTabOrder(self.extension, self.comboBox)
+        QWidget.setTabOrder(self.comboBox, self.clear_btn)
+        QWidget.setTabOrder(self.clear_btn, self.rename_btn)
+        QWidget.setTabOrder(self.rename_btn, self.search)
+        QWidget.setTabOrder(self.search, self.replace)
+        QWidget.setTabOrder(self.replace, self.regex)
+        QWidget.setTabOrder(self.regex, self.find_btn)
 
         self.retranslateUi(Widget)
         self.dir_btn.clicked.connect(Widget.open_dir)
         self.dir_btn.clicked.connect(self.dir_txt.update)
-        self.clear_btn.clicked.connect(self.dir_output.clear)
+        self.clear_btn.clicked.connect(Widget.clear)
         self.comboBox.activated.connect(Widget.index_changed)
         self.rename_btn.clicked.connect(Widget.rename_files)
         self.recursively.clicked.connect(Widget.add_recursively)
         self.id.clicked.connect(Widget.keep_id)
         self.extension.clicked.connect(Widget.keep_ext)
         self.regex.clicked.connect(Widget.regex)
         self.find_btn.clicked.connect(Widget.find)
 
         QMetaObject.connectSlotsByName(Widget)
     # setupUi
 
     def retranslateUi(self, Widget):
-        Widget.setWindowTitle(QCoreApplication.translate("Widget", u"RENAMER", None))
+        Widget.setWindowTitle(QCoreApplication.translate("Widget", u"File Renamer", None))
         self.browse.setTitle("")
         self.dir_btn.setText(QCoreApplication.translate("Widget", u"Browse", None))
         self.options.setTitle("")
         self.recursively.setText(QCoreApplication.translate("Widget", u"Add Files Recursively", None))
         self.id.setText(QCoreApplication.translate("Widget", u"Keep ID", None))
         self.extension.setText(QCoreApplication.translate("Widget", u"Keep Extension", None))
         self.groupBox.setTitle("")
```

### Comparing `file_renamer-1.0.1/src/file-renamer/widget.py` & `file_renamer-1.0.2/src/file-renamer/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,18 @@
                 elif index == 7:
                     self.rename.lower_case(**self.params)
                 elif index == 8:
                     self.rename.title_case(**self.params)
                 elif index == 9:
                     self.rename.remove_ids(**self.params)
 
+    def clear(self):
+        self.params["ui"].dir_output.clear()
+        self.params["ui"].rename_btn.setEnabled(False)
+
     def rename_files(self):
         self.params["title"] = ""
         index = self.params["ui"].comboBox.currentIndex()
         if index == 0:
             self.params["title"] = "Search & Replace"
         else:
             self.params["title"] = self.params["ui"].comboBox.currentText()
```

### Comparing `file_renamer-1.0.1/src/file-renamer/lib/case_insensitive.py` & `file_renamer-1.0.2/src/file-renamer/lib/case_insensitive.py`

 * *Files identical despite different names*

### Comparing `file_renamer-1.0.1/src/file-renamer/lib/exceptions.py` & `file_renamer-1.0.2/src/file-renamer/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `file_renamer-1.0.1/src/file-renamer/lib/files.py` & `file_renamer-1.0.2/src/file-renamer/lib/files.py`

 * *Files identical despite different names*

### Comparing `file_renamer-1.0.1/src/file-renamer/style/default_macos.qss` & `file_renamer-1.0.2/src/file-renamer/style/default_macos.qss`

 * *Files identical despite different names*

### Comparing `file_renamer-1.0.1/src/file-renamer/style/default_win.qss` & `file_renamer-1.0.2/src/file-renamer/style/default_win.qss`

 * *Files identical despite different names*

### Comparing `file_renamer-1.0.1/LICENSE` & `file_renamer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `file_renamer-1.0.1/pyproject.toml` & `file_renamer-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/file-renamer"]
+packages = ["file-renamer"]
 
 [project]
 name = "file-renamer"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Carlos", email="mcarlos@tuta.io" },
 ]
 description = "Rename files using a GUI desktop app for Linux & Windows. MacOS not yet tested."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = "==3.11"
 dependencies = [
-  "PySide6>=6.6.2",
-  "PySide6-Addons>=6.6.2",
-  "PySide6-Essentials>=6.6.2",
-  "shiboken6>=6.6.2",
-  "Unidecode>=1.3.8",
+  "PySide6==6.6.2",
+  "PySide6-Addons==6.6.2",
+  "PySide6-Essentials==6.6.2",
+  "shiboken6==6.6.2",
+  "Unidecode==1.3.8",
 ]
+keywords = ["rename", "file"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/mcarlos101/file-renamer"
-Issues = "https://github.com/mcarlos101/file-renamer/issues"
+Repository = "https://github.com/mcarlos101/file-renamer.git"
+
```

